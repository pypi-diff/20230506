# Comparing `tmp/whl-0.0.3-py2.py3-none-any.whl.zip` & `tmp/whl-0.0.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 12852 bytes, number of entries: 4
--rwxr-xr-x  2.0 unx    10210 b- stor 22-Apr-15 20:29 whl.py
-?rw-------  2.0 unx     1791 b- stor 22-Apr-15 20:30 whl-0.0.3.dist-info/METADATA
-?rw-------  2.0 unx       98 b- stor 22-Apr-15 20:30 whl-0.0.3.dist-info/WHEEL
-?rw-------  2.0 unx      257 b- stor 22-Apr-15 20:30 whl-0.0.3.dist-info/RECORD
-4 files, 12356 bytes uncompressed, 12356 bytes compressed:  0.0%
+Zip file size: 5060 bytes, number of entries: 4
+-rwxr-xr-x  2.0 unx    11365 b- defN 23-May-05 21:47 whl.py
+?rw-------  2.0 unx     2012 b- defN 22-Jan-01 00:00 whl-0.0.4.dist-info/METADATA
+?rw-------  2.0 unx       98 b- defN 22-Jan-01 00:00 whl-0.0.4.dist-info/WHEEL
+?rw-------  2.0 unx      257 b- defN 22-Jan-01 00:00 whl-0.0.4.dist-info/RECORD
+4 files, 13732 bytes uncompressed, 4564 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
 Filename: whl.py
 Comment: 
 
-Filename: whl-0.0.3.dist-info/METADATA
+Filename: whl-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: whl-0.0.3.dist-info/WHEEL
+Filename: whl-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: whl-0.0.3.dist-info/RECORD
+Filename: whl-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## whl.py

```diff
@@ -6,29 +6,30 @@
 import hashlib
 import logging
 import os
 import re
 import zipfile
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 log = logging.getLogger(__name__)
 
 
 # https://packaging.python.org/specifications/core-metadata/
 METADATA_TEMPLATE = """\
 Metadata-Version: 2.1
 Name: {name}
 Version: {version}
 """
 
 
 # https://www.python.org/dev/peps/pep-0427/
+# https://packaging.python.org/en/latest/specifications/binary-distribution-format/
 WHEEL_TEMPLATE = """\
 Wheel-Version: 1.0
 Generator: whl {__version__}
 Root-Is-Purelib: true
 """
 
 
@@ -110,14 +111,19 @@
     requires_python=None,
     requires_external=None,
     project_url=None,
     # provides_extra  # changed in version 2.3 but I can't find the spec for 2.3
     provides_dist=None,
     obsoletes_dist=None,
 
+    # entry points are specified here:
+    # https://packaging.python.org/en/latest/specifications/entry-points/
+    # but are not included in the core metadata fields (yet?)
+    entry_points=None,
+
     py2=True,
     py3=True,
     output_dir=".",
 ):
     if name is None:
         raise WhlError("name is required")
     if version is None:
@@ -194,15 +200,15 @@
         tags = "py3"
 
     whl_name = "{}-{}-{}-none-any.whl".format(name.replace("-", "_"), version, tags)
     dist_info_name = "{}-{}.dist-info".format(name.replace("-", "_"), version)
     whl_path = os.path.join(output_dir, whl_name)
 
     RECORD = []
-    zf = zipfile.ZipFile(whl_path, "w")
+    zf = zipfile.ZipFile(whl_path, "w", compression=zipfile.ZIP_DEFLATED)
     if src:
         if isinstance(src, (list, tuple)):
             dist_files = src
             parent = os.path.dirname(os.path.abspath(src[0]))
         else:
             dist_files = get_dist_files(src)
             parent = os.path.dirname(os.path.abspath(src))
@@ -211,26 +217,40 @@
             zf.write(path, arcname)
             record = get_record(path, arcname=arcname)
             RECORD.append(record)
             log.info(record)
 
     METADATA = METADATA.encode("utf-8")
     WHEEL = WHEEL.encode("utf-8")
+    dt = 2022, 1, 1, 0, 0, 0  # for reproducible builds
 
-    info_metadata = os.path.join(dist_info_name, "METADATA")
-    RECORD.append(get_record(info_metadata, data=METADATA))
-    zf.writestr(info_metadata, METADATA)
-
-    info_wheel = os.path.join(dist_info_name, "WHEEL")
-    RECORD.append(get_record(info_wheel, data=WHEEL))
-    zf.writestr(info_wheel, WHEEL)
+    zinfo_metadata = zipfile.ZipInfo(os.path.join(dist_info_name, "METADATA"), dt)
+    RECORD.append(get_record(zinfo_metadata.orig_filename, data=METADATA))
+    zf.writestr(zinfo_metadata, METADATA, compress_type=zipfile.ZIP_DEFLATED)
+
+    zinfo_wheel = zipfile.ZipInfo(os.path.join(dist_info_name, "WHEEL"), dt)
+    RECORD.append(get_record(zinfo_wheel.orig_filename, data=WHEEL))
+    zf.writestr(zinfo_wheel, WHEEL, compress_type=zipfile.ZIP_DEFLATED)
+
+    if entry_points is not None:
+        lines = []
+        for group, refs in entry_points.items():
+            lines.append("[{}]".format(group))
+            lines.extend(refs)
+            lines.append("")
+        entry_points_txt = "\n".join(lines).encode("utf-8")
+        fname = os.path.join(dist_info_name, "entry_points.txt")
+        zinfo_ep = zipfile.ZipInfo(fname, dt)
+        RECORD.append(get_record(zinfo_ep.orig_filename, data=entry_points_txt))
+        zf.writestr(zinfo_ep, entry_points_txt, compress_type=zipfile.ZIP_DEFLATED)
 
     RECORD.append("{},,".format(os.path.join(dist_info_name, "RECORD")))
     RECORD_BYTES = "\n".join(RECORD).encode("utf-8")
-    zf.writestr(os.path.join(dist_info_name, "RECORD"), RECORD_BYTES)
+    zinfo_record = zipfile.ZipInfo(os.path.join(dist_info_name, "RECORD"), dt)
+    zf.writestr(zinfo_record, RECORD_BYTES, compress_type=zipfile.ZIP_DEFLATED)
 
     zf.close()
     return whl_path
 
 
 def main():
     parser = argparse.ArgumentParser(
```

## Comparing `whl-0.0.3.dist-info/METADATA` & `whl-0.0.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: whl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimalist wheel building
 
 whl
 ===
 
-Quickly makes Python wheels_ from a bunch of .py files without needing a ``setup.py`` or ``pyproject.toml`` at all.
+Quickly makes Python wheels_ from a bunch of .py files without needing a ``setup.py`` at all.
 
-**You probably don't want to use this**. It doesn't have many features yet (no support for entrypoints, dependencies, extras).
+**You probably don't want to use this**. It's intentionally minimal for my own use-cases, and doesn't have many features yet (no support for entrypoints, dependencies, extras). If all you're looking for is a fast build, then consider using ``flit build --format wheel`` with a ``pyproject.toml``, this should be nearly as fast.
 
 Usage
 -----
 
 For a single file distribution:
 
 .. code-block:: python
@@ -52,7 +52,8 @@
 
 .. _wheels: https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#wheels
 .. _correct: https://pypi.org/project/build/
 .. _setuptools: https://setuptools.pypa.io/en/latest/
 .. _distutils: https://docs.python.org/3/library/distutils.html
 .. _PEP517: https://peps.python.org/pep-0517/
 .. _PEP518: https://peps.python.org/pep-0518/
+.. _flit: https://flit.pypa.io/en/latest/
```

