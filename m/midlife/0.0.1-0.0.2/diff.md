# Comparing `tmp/midlife-0.0.1.tar.gz` & `tmp/midlife-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midlife-0.0.1.tar", last modified: Fri Mar  3 03:31:12 2023, max compression
+gzip compressed data, was "midlife-0.0.2.tar", last modified: Sat May  6 01:56:36 2023, max compression
```

## Comparing `midlife-0.0.1.tar` & `midlife-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-03 03:31:12.902483 midlife-0.0.1/
--rw-r--r--   0 yt        (1000) yt        (1000)      849 2023-03-03 03:31:12.902483 midlife-0.0.1/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      334 2023-03-03 03:27:54.000000 midlife-0.0.1/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-03-03 03:31:12.902483 midlife-0.0.1/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      932 2023-03-03 03:27:26.000000 midlife-0.0.1/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-03 03:31:12.886828 midlife-0.0.1/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-03 03:31:12.902483 midlife-0.0.1/src/midlife.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)      849 2023-03-03 03:31:12.000000 midlife-0.0.1/src/midlife.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      211 2023-03-03 03:31:12.000000 midlife-0.0.1/src/midlife.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-03-03 03:31:12.000000 midlife-0.0.1/src/midlife.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       42 2023-03-03 03:31:12.000000 midlife-0.0.1/src/midlife.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        8 2023-03-03 03:31:12.000000 midlife-0.0.1/src/midlife.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1217 2023-03-03 03:29:45.000000 midlife-0.0.1/src/midlife.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 01:56:36.281491 midlife-0.0.2/
+-rw-r--r--   0 yt        (1000) yt        (1000)      849 2023-05-06 01:56:36.278810 midlife-0.0.2/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      334 2023-03-03 03:27:54.000000 midlife-0.0.2/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-06 01:56:36.281491 midlife-0.0.2/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      932 2023-05-06 01:52:49.000000 midlife-0.0.2/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 01:56:36.270399 midlife-0.0.2/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 01:56:36.278810 midlife-0.0.2/src/midlife.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)      849 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      211 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       42 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        8 2023-05-06 01:56:35.000000 midlife-0.0.2/src/midlife.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     2639 2023-05-06 01:51:22.000000 midlife-0.0.2/src/midlife.py
```

### Comparing `midlife-0.0.1/PKG-INFO` & `midlife-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midlife
-Version: 0.0.1
+Version: 0.0.2
 Summary: impact of COVID-19 on mortality of midlife
 Home-page: https://github.com/ytakefuji/vuv
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/midlife
 Platform: UNKNOWN
```

### Comparing `midlife-0.0.1/setup.py` & `midlife-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="midlife",
-    version="0.0.1",
+    version="0.0.2",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="impact of COVID-19 on mortality of midlife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/vuv",
     project_urls={
```

### Comparing `midlife-0.0.1/src/midlife.egg-info/PKG-INFO` & `midlife-0.0.2/src/midlife.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midlife
-Version: 0.0.1
+Version: 0.0.2
 Summary: impact of COVID-19 on mortality of midlife
 Home-page: https://github.com/ytakefuji/vuv
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/midlife
 Platform: UNKNOWN
```

