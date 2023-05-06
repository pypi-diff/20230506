# Comparing `tmp/alacorder-80.3.1.tar.gz` & `tmp/alacorder-80.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.3.1.tar", max compression
+gzip compressed data, was "alacorder-80.3.2.tar", max compression
```

## Comparing `alacorder-80.3.1.tar` & `alacorder-80.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.1/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.3.1/README.md
--rw-r--r--   0        0        0      697 2023-05-06 15:35:54.190603 alacorder-80.3.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-06 15:35:42.133455 alacorder-80.3.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   221323 2023-05-06 15:35:24.097717 alacorder-80.3.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   221323 2023-05-06 15:35:17.654729 alacorder-80.3.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.2/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.3.2/README.md
+-rw-r--r--   0        0        0      697 2023-05-06 18:26:04.387839 alacorder-80.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-06 15:35:42.133455 alacorder-80.3.2/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   220970 2023-05-06 18:25:23.993412 alacorder-80.3.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   220970 2023-05-06 18:25:09.574276 alacorder-80.3.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.3.2/PKG-INFO
```

### Comparing `alacorder-80.3.1/LICENSE` & `alacorder-80.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.1/README.md` & `alacorder-80.3.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.1/pyproject.toml` & `alacorder-80.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.3.1"
+version = "80.3.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.3.1/src/alacorder/.DS_Store` & `alacorder-80.3.2/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.1/src/alacorder/__main__.py` & `alacorder-80.3.2/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.1"
+version = "80.3.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3352,15 +3352,14 @@
         )
         return None
 
 
 def fetch(
     querypath="",
     dirpath="",
-    criminal=False,
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
     cf=None,
     no_update=False,
@@ -3369,15 +3368,14 @@
 ):
     """
     Fetch case PDFs from Alacourt.com.
     Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and download to `dirpath`.
     Args:
        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
        dirpath (str): Path to PDF output directory
-       criminal (bool): Only search criminal cases
        cID (str): Customer ID on Alacourt.com
        uID (str): User ID on Alacourt.com
        pwd (str): Password on Alacourt.com
        qmax (int): Maximum queries to conduct on Alacourt.com
        qskip (int): Skip entries at top of query file
        no_update (bool): Do not update query template after completion
        debug (bool): Print detailed runtime information to console
@@ -3404,26 +3402,24 @@
     query = read_query(cf["INPUTS"], qmax=qmax, qskip=qskip)
 
     # start browser and authenticate
     opt = webdriver.ChromeOptions()
     opt.add_experimental_option(
         "prefs",
         {
-            "download.default_directory": dirpath,  # Change default directory for downloads
+            "download.default_directory": dirpath,  # Set default directory for downloads
             "download.prompt_for_download": False,  # To auto download the file
             "download.directory_upgrade": True,
-            "plugins.always_open_pdf_externally": True,  # It will not display PDF directly in chrome
+            "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
         },
     )
     print("Starting browser... Do not close while in progress!")
     driver = webdriver.Chrome(options=opt)
     login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
 
-    if criminal:
-        query["TEMP_DIVISION"] == "Criminal Only"
 
     for i, r in enumerate(query.rows(named=True)):
         if query[i, "QUERY_COMPLETE"] == "Y":
             continue
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
             login(driver, cID, uID, pwd, window=window)
         driver.implicitly_wait(1)
@@ -3439,15 +3435,15 @@
             filed_before=r["TEMP_FILED_BEFORE"],
             filed_after=r["TEMP_FILED_AFTER"],
             window=window,
         )
 
         if len(results) > 0:
             print(
-                f"#{i}/{query.shape[0]} {query[i, 'TEMP_NAME']}) ({len(results)} records returned)"
+                f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']}) ({len(results)} records returned)"
             )
             if window:
                 window.write_event_value("PROGRESS-TEXT", 0)
                 window.write_event_value("PROGRESS-TEXT-TOTAL", 100)
                 for i, url in enumerate(results):
                     window.write_event_value("PROGRESS-TEXT", i + 1)
                     downloadPDF(driver, url)
@@ -4603,17 +4599,14 @@
     "path",
     required=True,
     prompt="PDF download path",
     type=click.Path(),
     help="Desired PDF output directory",
 )
 @click.option(
-    "--criminal-only", "-criminal", is_flag=True, help="Only search criminal cases"
-)
-@click.option(
     "--customer-id",
     "-c",
     "cID",
     required=True,
     prompt="Alacourt Customer ID",
     help="Customer ID on Alacourt.com",
 )
@@ -4662,33 +4655,31 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def _cli_fetch(querypath, path, criminal, cID, uID, pwd, qmax, qskip, no_update, debug):
+def _cli_fetch(querypath, path, cID, uID, pwd, qmax, qskip, no_update, debug):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
-        criminal (bool, optional): only search criminal cases
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
         pwd (str): Password on Alacourt.com
         qmax (int): Maximum queries to conduct on Alacourt.com
         qskip (int): Skip entries at top of query file
         no_update (bool): Do not update query template after completion
         debug (bool): Print detailed runtime information to console
     """
     fetch(
-        querypath=listpath,
+        querypath=querypath,
         dirpath=path,
-        criminal=criminal,
         cID=cID,
         uID=uID,
         pwd=pwd,
         qmax=qmax,
         qskip=qskip,
         no_update=no_update,
         debug=debug,
```

### Comparing `alacorder-80.3.1/src/alacorder/alac.py` & `alacorder-80.3.2/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.1"
+version = "80.3.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3352,15 +3352,14 @@
         )
         return None
 
 
 def fetch(
     querypath="",
     dirpath="",
-    criminal=False,
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
     cf=None,
     no_update=False,
@@ -3369,15 +3368,14 @@
 ):
     """
     Fetch case PDFs from Alacourt.com.
     Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and download to `dirpath`.
     Args:
        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
        dirpath (str): Path to PDF output directory
-       criminal (bool): Only search criminal cases
        cID (str): Customer ID on Alacourt.com
        uID (str): User ID on Alacourt.com
        pwd (str): Password on Alacourt.com
        qmax (int): Maximum queries to conduct on Alacourt.com
        qskip (int): Skip entries at top of query file
        no_update (bool): Do not update query template after completion
        debug (bool): Print detailed runtime information to console
@@ -3404,26 +3402,24 @@
     query = read_query(cf["INPUTS"], qmax=qmax, qskip=qskip)
 
     # start browser and authenticate
     opt = webdriver.ChromeOptions()
     opt.add_experimental_option(
         "prefs",
         {
-            "download.default_directory": dirpath,  # Change default directory for downloads
+            "download.default_directory": dirpath,  # Set default directory for downloads
             "download.prompt_for_download": False,  # To auto download the file
             "download.directory_upgrade": True,
-            "plugins.always_open_pdf_externally": True,  # It will not display PDF directly in chrome
+            "plugins.always_open_pdf_externally": True,  # Don't display PDF in chrome
         },
     )
     print("Starting browser... Do not close while in progress!")
     driver = webdriver.Chrome(options=opt)
     login(driver, cID=cID, uID=uID, pwd=pwd, window=window)
 
-    if criminal:
-        query["TEMP_DIVISION"] == "Criminal Only"
 
     for i, r in enumerate(query.rows(named=True)):
         if query[i, "QUERY_COMPLETE"] == "Y":
             continue
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
             login(driver, cID, uID, pwd, window=window)
         driver.implicitly_wait(1)
@@ -3439,15 +3435,15 @@
             filed_before=r["TEMP_FILED_BEFORE"],
             filed_after=r["TEMP_FILED_AFTER"],
             window=window,
         )
 
         if len(results) > 0:
             print(
-                f"#{i}/{query.shape[0]} {query[i, 'TEMP_NAME']}) ({len(results)} records returned)"
+                f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']}) ({len(results)} records returned)"
             )
             if window:
                 window.write_event_value("PROGRESS-TEXT", 0)
                 window.write_event_value("PROGRESS-TEXT-TOTAL", 100)
                 for i, url in enumerate(results):
                     window.write_event_value("PROGRESS-TEXT", i + 1)
                     downloadPDF(driver, url)
@@ -4603,17 +4599,14 @@
     "path",
     required=True,
     prompt="PDF download path",
     type=click.Path(),
     help="Desired PDF output directory",
 )
 @click.option(
-    "--criminal-only", "-criminal", is_flag=True, help="Only search criminal cases"
-)
-@click.option(
     "--customer-id",
     "-c",
     "cID",
     required=True,
     prompt="Alacourt Customer ID",
     help="Customer ID on Alacourt.com",
 )
@@ -4662,33 +4655,31 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def _cli_fetch(querypath, path, criminal, cID, uID, pwd, qmax, qskip, no_update, debug):
+def _cli_fetch(querypath, path, cID, uID, pwd, qmax, qskip, no_update, debug):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
-        criminal (bool, optional): only search criminal cases
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
         pwd (str): Password on Alacourt.com
         qmax (int): Maximum queries to conduct on Alacourt.com
         qskip (int): Skip entries at top of query file
         no_update (bool): Do not update query template after completion
         debug (bool): Print detailed runtime information to console
     """
     fetch(
-        querypath=listpath,
+        querypath=querypath,
         dirpath=path,
-        criminal=criminal,
         cID=cID,
         uID=uID,
         pwd=pwd,
         qmax=qmax,
         qskip=qskip,
         no_update=no_update,
         debug=debug,
```

### Comparing `alacorder-80.3.1/PKG-INFO` & `alacorder-80.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.3.1
+Version: 80.3.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

