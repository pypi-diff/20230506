# Comparing `tmp/alacorder-80.2.9.tar.gz` & `tmp/alacorder-80.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.2.9.tar", max compression
+gzip compressed data, was "alacorder-80.3.0.tar", max compression
```

## Comparing `alacorder-80.2.9.tar` & `alacorder-80.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.9/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.9/README.md
--rw-r--r--   0        0        0      697 2023-05-05 21:04:13.328849 alacorder-80.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   220075 2023-05-05 21:03:50.354455 alacorder-80.2.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   220075 2023-05-05 21:03:45.400426 alacorder-80.2.9/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.0/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.3.0/README.md
+-rw-r--r--   0        0        0      697 2023-05-06 14:56:47.024333 alacorder-80.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   220085 2023-05-06 14:56:15.899998 alacorder-80.3.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   220085 2023-05-06 14:55:46.422287 alacorder-80.3.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.3.0/PKG-INFO
```

### Comparing `alacorder-80.2.9/LICENSE` & `alacorder-80.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.9/README.md` & `alacorder-80.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.9/pyproject.toml` & `alacorder-80.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.2.9"
+version = "80.3.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.2.9/src/alacorder/__main__.py` & `alacorder-80.3.0/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.9"
+version = "80.3.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -398,15 +398,15 @@
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
     start = time.time()
     print(
         "Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf
     )
-    vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
+    vr = _vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
@@ -417,15 +417,15 @@
 
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
     start = time.time()
     print("Combining cases by AIS / Unique ID to create charges summary...", cf=cf)
-    ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
+    ch = _charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             ch,
             sheet_names=["ChargesSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
@@ -440,15 +440,15 @@
 
 def convictions_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
     start = time.time()
     print("Combining cases by AIS / Unique ID to create convictions summary...", cf=cf)
-    conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
+    conv = _convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             conv,
             sheet_names=["ConvictionsSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
@@ -1006,15 +1006,15 @@
 
 def pairs(cf):
     """
     Create AIS / Unique ID pairs template using configuration object `cf`.
     """
     print("Creating empty pairs template...", cf=cf)
     df = read(cf)
-    tp = make_pairs_template(df)
+    tp = _make_pairs_template(df)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             tp, sheet_names=["Pairs"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
     print("Created template successfully.", cf=cf)
     if cf["WINDOW"]:
@@ -1231,15 +1231,15 @@
                 cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
             cf["WINDOW"].write_event_value("PROGRESS", i + 1)
         cf["WINDOW"].write_event_value("RN-COMPLETE", True)
 
 
-def make_pairs_template(df, debug=False):
+def _make_pairs_template(df, debug=False):
     if isinstance(df, str):
         df = read(df)
     names = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
@@ -1259,42 +1259,42 @@
             .str.strip()
             .alias("Name"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace_all(r"[^\d/]", "")
             .str.strip()
             .alias("DOB"),
-            pl.col("AllPagesText")
-            .str.extract(r"(SSN)(.+)(Alias)", group_index=2)
+            pl.col("AllPagesTextNoNewLine")
+            .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
             .str.replace(r"(SSN)", "")
             .str.replace(r"Alias", "")
             .str.replace(r"\:", "")
             .str.strip()
             .alias("Alias"),
         ]
     )
     names = (
         names.groupby("Name")
-        .agg("CaseNumber", "DOB")
+        .agg("CaseNumber","Alias","DOB")
         .select(
             [
                 pl.lit("").alias("AIS / Unique ID"),
                 pl.col("Name"),
-                pl.col("Alias").arr.get(0).str.replace("null", ""),
+                pl.col("Alias").arr.get(0),
                 pl.col("DOB").arr.get(0),
                 pl.col("CaseNumber").arr.lengths().alias("CaseCount"),
                 pl.col("CaseNumber").arr.join(", ").alias("Cases"),
             ]
         )
     )
     names = names.sort("Name")
     return names
 
 
-def charges_summary_from_pairs(src, pairs, debug=False):
+def _charges_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
@@ -1360,15 +1360,15 @@
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
 
-def convictions_summary_from_pairs(src, pairs, debug=False):
+def _convictions_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
@@ -1444,15 +1444,15 @@
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
 
-def vrr_summary_from_pairs(src, pairs, debug=False):
+def _vrr_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (  # pair AIS to cases sheet
         src["cases"]
```

### Comparing `alacorder-80.2.9/src/alacorder/alac.py` & `alacorder-80.3.0/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.9"
+version = "80.3.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -398,15 +398,15 @@
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
     start = time.time()
     print(
         "Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf
     )
-    vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
+    vr = _vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
@@ -417,15 +417,15 @@
 
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
     start = time.time()
     print("Combining cases by AIS / Unique ID to create charges summary...", cf=cf)
-    ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
+    ch = _charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             ch,
             sheet_names=["ChargesSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
@@ -440,15 +440,15 @@
 
 def convictions_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
     start = time.time()
     print("Combining cases by AIS / Unique ID to create convictions summary...", cf=cf)
-    conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
+    conv = _convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             conv,
             sheet_names=["ConvictionsSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
@@ -1006,15 +1006,15 @@
 
 def pairs(cf):
     """
     Create AIS / Unique ID pairs template using configuration object `cf`.
     """
     print("Creating empty pairs template...", cf=cf)
     df = read(cf)
-    tp = make_pairs_template(df)
+    tp = _make_pairs_template(df)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             tp, sheet_names=["Pairs"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
     print("Created template successfully.", cf=cf)
     if cf["WINDOW"]:
@@ -1231,15 +1231,15 @@
                 cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
             cf["WINDOW"].write_event_value("PROGRESS", i + 1)
         cf["WINDOW"].write_event_value("RN-COMPLETE", True)
 
 
-def make_pairs_template(df, debug=False):
+def _make_pairs_template(df, debug=False):
     if isinstance(df, str):
         df = read(df)
     names = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
@@ -1259,42 +1259,42 @@
             .str.strip()
             .alias("Name"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace_all(r"[^\d/]", "")
             .str.strip()
             .alias("DOB"),
-            pl.col("AllPagesText")
-            .str.extract(r"(SSN)(.+)(Alias)", group_index=2)
+            pl.col("AllPagesTextNoNewLine")
+            .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
             .str.replace(r"(SSN)", "")
             .str.replace(r"Alias", "")
             .str.replace(r"\:", "")
             .str.strip()
             .alias("Alias"),
         ]
     )
     names = (
         names.groupby("Name")
-        .agg("CaseNumber", "DOB")
+        .agg("CaseNumber","Alias","DOB")
         .select(
             [
                 pl.lit("").alias("AIS / Unique ID"),
                 pl.col("Name"),
-                pl.col("Alias").arr.get(0).str.replace("null", ""),
+                pl.col("Alias").arr.get(0),
                 pl.col("DOB").arr.get(0),
                 pl.col("CaseNumber").arr.lengths().alias("CaseCount"),
                 pl.col("CaseNumber").arr.join(", ").alias("Cases"),
             ]
         )
     )
     names = names.sort("Name")
     return names
 
 
-def charges_summary_from_pairs(src, pairs, debug=False):
+def _charges_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
@@ -1360,15 +1360,15 @@
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
 
-def convictions_summary_from_pairs(src, pairs, debug=False):
+def _convictions_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
@@ -1444,15 +1444,15 @@
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
 
-def vrr_summary_from_pairs(src, pairs, debug=False):
+def _vrr_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (  # pair AIS to cases sheet
         src["cases"]
```

### Comparing `alacorder-80.2.9/PKG-INFO` & `alacorder-80.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.2.9
+Version: 80.3.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

