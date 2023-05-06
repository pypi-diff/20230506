# Comparing `tmp/chromedriver-py-auto-0.2.1.tar.gz` & `tmp/chromedriver-py-auto-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-py-auto-0.2.1.tar", last modified: Fri Feb 17 15:03:33 2023, max compression
+gzip compressed data, was "chromedriver-py-auto-0.2.2.tar", last modified: Sat May  6 11:29:20 2023, max compression
```

## Comparing `chromedriver-py-auto-0.2.1.tar` & `chromedriver-py-auto-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-02-17 15:03:33.792421 chromedriver-py-auto-0.2.1/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1076 2023-01-27 16:56:24.000000 chromedriver-py-auto-0.2.1/LICENSE
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      115 2023-02-17 15:03:25.000000 chromedriver-py-auto-0.2.1/MANIFEST.in
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1663 2023-02-17 15:03:33.792421 chromedriver-py-auto-0.2.1/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1008 2023-02-17 13:43:29.000000 chromedriver-py-auto-0.2.1/README.md
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-02-17 15:03:33.792421 chromedriver-py-auto-0.2.1/chromedriver_py_auto/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       92 2023-02-16 20:35:00.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto/__init__.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       84 2023-02-16 22:51:00.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto/binary_path.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      647 2023-01-27 17:14:10.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto/chrome.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       27 2023-02-16 22:52:31.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto/chromedriver
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     2828 2023-02-16 23:11:31.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto/install.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-02-17 14:45:47.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto/py.typed
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1097 2023-01-27 17:14:10.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto/version.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-02-17 15:03:33.792421 chromedriver-py-auto-0.2.1/chromedriver_py_auto.egg-info/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1663 2023-02-17 15:03:33.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto.egg-info/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      442 2023-02-17 15:03:33.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto.egg-info/SOURCES.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-02-17 15:03:33.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto.egg-info/dependency_links.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       21 2023-02-17 15:03:33.000000 chromedriver-py-auto-0.2.1/chromedriver_py_auto.egg-info/top_level.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-02-17 15:03:33.792421 chromedriver-py-auto-0.2.1/setup.cfg
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      979 2023-02-17 14:49:40.000000 chromedriver-py-auto-0.2.1/setup.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-05-06 11:29:20.232452 chromedriver-py-auto-0.2.2/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1076 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/LICENSE
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      115 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/MANIFEST.in
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1663 2023-05-06 11:29:20.232452 chromedriver-py-auto-0.2.2/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1008 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/README.md
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-05-06 11:29:20.228452 chromedriver-py-auto-0.2.2/chromedriver_py_auto/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       52 2023-05-06 11:14:39.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/__init__.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       84 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/binary_path.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      647 2023-05-06 11:15:29.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/chrome.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       27 2023-05-06 11:28:41.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/chromedriver
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     2601 2023-05-06 11:22:09.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/chromedriver_py.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/py.typed
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1097 2023-05-06 10:10:57.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto/version.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-05-06 11:29:20.232452 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1663 2023-05-06 11:29:20.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      450 2023-05-06 11:29:20.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/SOURCES.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-05-06 11:29:20.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/dependency_links.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       21 2023-05-06 11:29:20.000000 chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/top_level.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-05-06 11:29:20.232452 chromedriver-py-auto-0.2.2/setup.cfg
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1134 2023-05-06 11:21:08.000000 chromedriver-py-auto-0.2.2/setup.py
```

### Comparing `chromedriver-py-auto-0.2.1/LICENSE` & `chromedriver-py-auto-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.1/PKG-INFO` & `chromedriver-py-auto-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-py-auto
-Version: 0.2.1
+Version: 0.2.2
 Summary: A wrapper around chromedriver-py library. Detects the Chrome version and installs the most suitable chromedriver-py version.
 Home-page: https://github.com/AlirezaRoshanzamir/chromedriver-py-auto
 Author: Alireza Roshanzamir
 Author-email: a.roshanzamir1996@gmail.com
 License: MIT License
 Description: # chromdriver-py-auto
         A wrapper around [chromedriver-py](https://github.com/breuerfelix/chromedriver-py)
```

### Comparing `chromedriver-py-auto-0.2.1/README.md` & `chromedriver-py-auto-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.1/chromedriver_py_auto/chrome.py` & `chromedriver-py-auto-0.2.2/chromedriver_py_auto/chrome.py`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.1/chromedriver_py_auto/install.py` & `chromedriver-py-auto-0.2.2/chromedriver_py_auto/chromedriver_py.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,51 @@
 import json
 import logging
 import os
 import shutil
-import subprocess
-import sys
 import urllib.request
-from pathlib import Path
 from typing import Iterable, List, Optional
 
 from chromedriver_py_auto.binary_path import binary_path
 from chromedriver_py_auto.chrome import extract_chrome_version
 from chromedriver_py_auto.version import Version
 
 
-def install() -> None:
+def copy_binary() -> None:
+    import chromedriver_py
+
+    logging.error(
+        'Copying "{}" to "{}".'.format(chromedriver_py.binary_path, binary_path)
+    )
+    shutil.copy2(chromedriver_py.binary_path, binary_path)
+    stat = os.stat(chromedriver_py.binary_path)
+    os.chown(binary_path, stat.st_uid, stat.st_gid)
+
+
+def extract_suitable_version() -> Version:
     chrome_version = Version.from_string(extract_chrome_version())
     logging.info('Chrome version "{}" is detected.'.format(str(chrome_version)))
 
     chromedriver_py_versions = _get_package_versions("chromedriver-py")
     logging.info(
         'Chromedriver "{}" versions are found.'.format(
             '", "'.join(map(str, chromedriver_py_versions))
         )
     )
 
     most_suitable_chromedriver_py_version = _find_most_suitable_driver_version(
         chrome_version, chromedriver_py_versions
     )
     logging.info(
-        'Chromedriver version "{}" is selected for installation.'.format(
+        'Chromedriver version "{}" is the most suitable for installation.'.format(
             str(most_suitable_chromedriver_py_version)
         )
     )
 
-    python_path = Path(sys.prefix) / "bin" / "python3"
-    subprocess.check_call(
-        [
-            str(python_path),
-            "-m",
-            "pip",
-            "install",
-            "chromedriver-py=={}".format(most_suitable_chromedriver_py_version),
-        ]
-    )
-
-    import chromedriver_py
-
-    logging.error(
-        'Copying "{}" to "{}".'.format(chromedriver_py.binary_path, binary_path)
-    )
-    shutil.copy2(chromedriver_py.binary_path, binary_path)
-    stat = os.stat(chromedriver_py.binary_path)
-    os.chown(binary_path, stat.st_uid, stat.st_gid)
+    return most_suitable_chromedriver_py_version
 
 
 def _get_package_versions(package_name: str) -> List[Version]:
     url = "https://pypi.org/pypi/%s/json" % (package_name,)
     data = json.load(urllib.request.urlopen(url))
     return sorted(map(Version.from_string, data["releases"]))
```

### Comparing `chromedriver-py-auto-0.2.1/chromedriver_py_auto/version.py` & `chromedriver-py-auto-0.2.2/chromedriver_py_auto/version.py`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.1/chromedriver_py_auto.egg-info/PKG-INFO` & `chromedriver-py-auto-0.2.2/chromedriver_py_auto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-py-auto
-Version: 0.2.1
+Version: 0.2.2
 Summary: A wrapper around chromedriver-py library. Detects the Chrome version and installs the most suitable chromedriver-py version.
 Home-page: https://github.com/AlirezaRoshanzamir/chromedriver-py-auto
 Author: Alireza Roshanzamir
 Author-email: a.roshanzamir1996@gmail.com
 License: MIT License
 Description: # chromdriver-py-auto
         A wrapper around [chromedriver-py](https://github.com/breuerfelix/chromedriver-py)
```

### Comparing `chromedriver-py-auto-0.2.1/setup.py` & `chromedriver-py-auto-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+from asyncio import subprocess
 import logging
 from pathlib import Path
 
 import setuptools
 from setuptools.command.build_py import build_py
 
-from chromedriver_py_auto import install
+from chromedriver_py_auto.chromedriver_py import copy_binary, extract_suitable_version
 
 logging.basicConfig(level=logging.INFO)
 
 
-class InstallSuitableChromedriverPy(setuptools.command.build_py.build_py):
+class CopyChromedriverPyBinary(setuptools.command.build_py.build_py):
     def run(self) -> None:
-        install()
+        copy_binary()
         build_py.run(self)
 
 
 setuptools.setup(
     name="chromedriver-py-auto",
-    version="0.2.1",
+    version="0.2.2",
     description="A wrapper around chromedriver-py library. Detects the Chrome version "
     "and installs the most suitable chromedriver-py version.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Alireza Roshanzamir",
     author_email="a.roshanzamir1996@gmail.com",
     url="https://github.com/AlirezaRoshanzamir/chromedriver-py-auto",
     packages=setuptools.find_packages(),
+    setup_requires=["chromedriver-py=={}".format(str(extract_suitable_version()))],
     include_package_data=True,
-    cmdclass={"build_py": InstallSuitableChromedriverPy},
+    cmdclass={"build_py": CopyChromedriverPyBinary},
 )
```

