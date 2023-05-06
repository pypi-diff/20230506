# Comparing `tmp/midlife-0.0.2.tar.gz` & `tmp/midlife-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midlife-0.0.2.tar", last modified: Sat May  6 01:56:36 2023, max compression
+gzip compressed data, was "midlife-0.0.3.tar", last modified: Sat May  6 02:05:56 2023, max compression
```

## Comparing `midlife-0.0.2.tar` & `midlife-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 01:56:36.281491 midlife-0.0.2/
--rw-r--r--   0 yt        (1000) yt        (1000)      849 2023-05-06 01:56:36.278810 midlife-0.0.2/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      334 2023-03-03 03:27:54.000000 midlife-0.0.2/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-06 01:56:36.281491 midlife-0.0.2/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      932 2023-05-06 01:52:49.000000 midlife-0.0.2/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 01:56:36.270399 midlife-0.0.2/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 01:56:36.278810 midlife-0.0.2/src/midlife.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)      849 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      211 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       42 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        8 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2639 2023-05-06 01:51:22.000000 midlife-0.0.2/src/midlife.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 02:05:56.765172 midlife-0.0.3/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 02:05:56.764179 midlife-0.0.3/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      729 2023-05-06 02:04:11.000000 midlife-0.0.3/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-06 02:05:56.765172 midlife-0.0.3/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      932 2023-05-06 02:05:01.000000 midlife-0.0.3/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 02:05:56.748047 midlife-0.0.3/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 02:05:56.763179 midlife-0.0.3/src/midlife.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      211 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       42 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        8 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     2639 2023-05-06 01:51:22.000000 midlife-0.0.3/src/midlife.py
```

### Comparing `midlife-0.0.2/PKG-INFO` & `midlife-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: midlife
-Version: 0.0.2
+Version: 0.0.3
 Summary: impact of COVID-19 on mortality of midlife
 Home-page: https://github.com/ytakefuji/vuv
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/midlife
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # midlife
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/2444117/tree)
+
 This is under review.
 
-midlife is a PyPI application for evaluating and visualzing the impact of COVID-19 on mortality of midlife from 40 to 64 years old.
+midlife is a PyPI application for evaluating and visualzing the impact of COVID-19 on mortality of midlife in five age groups from 40 to 64 years old.
 
 CDC dataset is used for this study:
 https://data.cdc.gov/api/views/chcz-j2du/rows.csv
 
 
 # How to install midlife
 $ pip install midlife
 
 # How to run midlife
 
-$ midlife
+midlife needs the degree of polynomial regression and sex: F or M. 
+The following example can show the 3rd degree of polynomial and Female.
+
+$ midlife 3 F
+
+<img src='https://github.com/ytakefuji/midlife/raw/main/Fmidlife.png' width=640 height=480>
```

### Comparing `midlife-0.0.2/setup.py` & `midlife-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="midlife",
-    version="0.0.2",
+    version="0.0.3",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="impact of COVID-19 on mortality of midlife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/vuv",
     project_urls={
```

### Comparing `midlife-0.0.2/src/midlife.egg-info/PKG-INFO` & `midlife-0.0.3/src/midlife.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: midlife
-Version: 0.0.2
+Version: 0.0.3
 Summary: impact of COVID-19 on mortality of midlife
 Home-page: https://github.com/ytakefuji/vuv
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/midlife
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # midlife
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/2444117/tree)
+
 This is under review.
 
-midlife is a PyPI application for evaluating and visualzing the impact of COVID-19 on mortality of midlife from 40 to 64 years old.
+midlife is a PyPI application for evaluating and visualzing the impact of COVID-19 on mortality of midlife in five age groups from 40 to 64 years old.
 
 CDC dataset is used for this study:
 https://data.cdc.gov/api/views/chcz-j2du/rows.csv
 
 
 # How to install midlife
 $ pip install midlife
 
 # How to run midlife
 
-$ midlife
+midlife needs the degree of polynomial regression and sex: F or M. 
+The following example can show the 3rd degree of polynomial and Female.
+
+$ midlife 3 F
+
+<img src='https://github.com/ytakefuji/midlife/raw/main/Fmidlife.png' width=640 height=480>
```

### Comparing `midlife-0.0.2/src/midlife.py` & `midlife-0.0.3/src/midlife.py`

 * *Files identical despite different names*

