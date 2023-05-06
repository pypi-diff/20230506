# Comparing `tmp/alacorder-80.3.0.tar.gz` & `tmp/alacorder-80.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.3.0.tar", max compression
+gzip compressed data, was "alacorder-80.3.1.tar", max compression
```

## Comparing `alacorder-80.3.0.tar` & `alacorder-80.3.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.0/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.3.0/README.md
--rw-r--r--   0        0        0      697 2023-05-06 14:56:47.024333 alacorder-80.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   220085 2023-05-06 14:56:15.899998 alacorder-80.3.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   220085 2023-05-06 14:55:46.422287 alacorder-80.3.0/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.1/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.3.1/README.md
+-rw-r--r--   0        0        0      697 2023-05-06 15:35:54.190603 alacorder-80.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-06 15:35:42.133455 alacorder-80.3.1/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   221323 2023-05-06 15:35:24.097717 alacorder-80.3.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   221323 2023-05-06 15:35:17.654729 alacorder-80.3.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.3.1/PKG-INFO
```

### Comparing `alacorder-80.3.0/LICENSE` & `alacorder-80.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.0/README.md` & `alacorder-80.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.0/pyproject.toml` & `alacorder-80.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.3.0"
+version = "80.3.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.3.0/src/alacorder/__main__.py` & `alacorder-80.3.1/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.0"
+version = "80.3.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1290,14 +1290,27 @@
     return names
 
 
 def _charges_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
+        src['cases'] = src['cases'].with_columns(
+            [
+                pl.col("Race").cast(pl.Utf8, strict=False),
+                pl.col("Sex").cast(pl.Utf8, strict=False)
+            ]
+        )
+        src['charges'] = src['charges'].with_columns(
+            [
+                pl.col("TypeDescription").cast(pl.Utf8, strict=False),
+                pl.col("Category").cast(pl.Utf8, strict=False),
+                pl.col("CourtAction").cast(pl.Utf8, strict=False)
+            ]
+        )
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
         .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
@@ -1309,15 +1322,15 @@
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
             pl.col("Race").arr.get(0),
             pl.col("Sex").arr.get(0),
             pl.col("CaseNumber").arr.join(", "),
         ]
-    )
+    )    
     summary = summary.join(ch, on="Name", how="outer")  # join cases, convictions
     summary = summary.groupby("Name").agg(
         [
             pl.col("AIS / Unique ID"),
             pl.col("DOB"),
             pl.col("Race"),
             pl.col("Sex"),
@@ -1360,18 +1373,32 @@
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
 
+
 def _convictions_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
+        src['cases'] = src['cases'].with_columns(
+            [
+                pl.col("Race").cast(pl.Utf8, strict=False),
+                pl.col("Sex").cast(pl.Utf8, strict=False)
+            ]
+        )
+        src['charges'] = src['charges'].with_columns(
+            [
+                pl.col("TypeDescription").cast(pl.Utf8, strict=False),
+                pl.col("Category").cast(pl.Utf8, strict=False),
+                pl.col("CourtAction").cast(pl.Utf8, strict=False)
+            ]
+        )
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
         .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
@@ -1448,27 +1475,34 @@
     return summary
 
 
 def _vrr_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
+        src['cases'] = src['cases'].with_columns(
+            [
+                pl.col("Race").cast(pl.Utf8, strict=False),
+                pl.col("Sex").cast(pl.Utf8, strict=False)
+            ]
+        )
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (  # pair AIS to cases sheet
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
         .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
     )
     disq = src["charges"].filter(  # filter disqualifying convictions
         pl.col("CERVDisqConviction")
         | pl.col("PardonDisqConviction")
         | pl.col("PermanentDisqConviction")
     )
+   
     summary = summary.select(  # prepare summary for join w/ convictions
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
             pl.col("Race").arr.get(0),
@@ -1517,15 +1551,15 @@
             .str.replace(r"null", "")
             .alias("ChargesSummary"),
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
-
+    
 
 def _explode_charges(df, debug=False):
     all_charges = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
@@ -3893,14 +3927,16 @@
             sg.Text("Skip from top: "),
             sg.Input(key="SQ-SKIP", default_text="0", size=[5, 1]),
         ],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
             sg.Text("Customer ID:"),
             sg.Input(key="SQ-CUSTOMERID", size=(13, 1)),
+        ],
+        [
             sg.Text("User ID:"),
             sg.Input(key="SQ-USERID", size=(13, 1)),
         ],
         [
             sg.Text("Password:"),
             sg.InputText(key="SQ-PASSWORD", password_char="*", size=(15, 1)),
         ],
@@ -4217,17 +4253,17 @@
         expand_y=False,
         size=[0, 0],
         font="Courier",
         layout=[
             [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
             [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
-            [sg.Tab("append", layout=append_layout, pad=(2, 2))],
             [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
             [sg.Tab("rename", layout=rename_layout, pad=(2, 2))],
+            [sg.Tab("append", layout=append_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
         [sg.Text(FSHORT_NAME, font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
```

### Comparing `alacorder-80.3.0/src/alacorder/alac.py` & `alacorder-80.3.1/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.0"
+version = "80.3.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1290,14 +1290,27 @@
     return names
 
 
 def _charges_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
+        src['cases'] = src['cases'].with_columns(
+            [
+                pl.col("Race").cast(pl.Utf8, strict=False),
+                pl.col("Sex").cast(pl.Utf8, strict=False)
+            ]
+        )
+        src['charges'] = src['charges'].with_columns(
+            [
+                pl.col("TypeDescription").cast(pl.Utf8, strict=False),
+                pl.col("Category").cast(pl.Utf8, strict=False),
+                pl.col("CourtAction").cast(pl.Utf8, strict=False)
+            ]
+        )
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
         .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
@@ -1309,15 +1322,15 @@
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
             pl.col("Race").arr.get(0),
             pl.col("Sex").arr.get(0),
             pl.col("CaseNumber").arr.join(", "),
         ]
-    )
+    )    
     summary = summary.join(ch, on="Name", how="outer")  # join cases, convictions
     summary = summary.groupby("Name").agg(
         [
             pl.col("AIS / Unique ID"),
             pl.col("DOB"),
             pl.col("Race"),
             pl.col("Sex"),
@@ -1360,18 +1373,32 @@
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
 
+
 def _convictions_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
+        src['cases'] = src['cases'].with_columns(
+            [
+                pl.col("Race").cast(pl.Utf8, strict=False),
+                pl.col("Sex").cast(pl.Utf8, strict=False)
+            ]
+        )
+        src['charges'] = src['charges'].with_columns(
+            [
+                pl.col("TypeDescription").cast(pl.Utf8, strict=False),
+                pl.col("Category").cast(pl.Utf8, strict=False),
+                pl.col("CourtAction").cast(pl.Utf8, strict=False)
+            ]
+        )
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
         .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
@@ -1448,27 +1475,34 @@
     return summary
 
 
 def _vrr_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
+        src['cases'] = src['cases'].with_columns(
+            [
+                pl.col("Race").cast(pl.Utf8, strict=False),
+                pl.col("Sex").cast(pl.Utf8, strict=False)
+            ]
+        )
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (  # pair AIS to cases sheet
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
         .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
     )
     disq = src["charges"].filter(  # filter disqualifying convictions
         pl.col("CERVDisqConviction")
         | pl.col("PardonDisqConviction")
         | pl.col("PermanentDisqConviction")
     )
+   
     summary = summary.select(  # prepare summary for join w/ convictions
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
             pl.col("Race").arr.get(0),
@@ -1517,15 +1551,15 @@
             .str.replace(r"null", "")
             .alias("ChargesSummary"),
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
-
+    
 
 def _explode_charges(df, debug=False):
     all_charges = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
@@ -3893,14 +3927,16 @@
             sg.Text("Skip from top: "),
             sg.Input(key="SQ-SKIP", default_text="0", size=[5, 1]),
         ],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
             sg.Text("Customer ID:"),
             sg.Input(key="SQ-CUSTOMERID", size=(13, 1)),
+        ],
+        [
             sg.Text("User ID:"),
             sg.Input(key="SQ-USERID", size=(13, 1)),
         ],
         [
             sg.Text("Password:"),
             sg.InputText(key="SQ-PASSWORD", password_char="*", size=(15, 1)),
         ],
@@ -4217,17 +4253,17 @@
         expand_y=False,
         size=[0, 0],
         font="Courier",
         layout=[
             [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
             [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
-            [sg.Tab("append", layout=append_layout, pad=(2, 2))],
             [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
             [sg.Tab("rename", layout=rename_layout, pad=(2, 2))],
+            [sg.Tab("append", layout=append_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
         [sg.Text(FSHORT_NAME, font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
```

### Comparing `alacorder-80.3.0/PKG-INFO` & `alacorder-80.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.3.0
+Version: 80.3.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

