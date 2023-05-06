# Comparing `tmp/midlife-0.0.3.tar.gz` & `tmp/midlife-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midlife-0.0.3.tar", last modified: Sat May  6 02:05:56 2023, max compression
+gzip compressed data, was "midlife-0.0.4.tar", last modified: Sat May  6 03:23:48 2023, max compression
```

## Comparing `midlife-0.0.3.tar` & `midlife-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 02:05:56.765172 midlife-0.0.3/
--rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 02:05:56.764179 midlife-0.0.3/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      729 2023-05-06 02:04:11.000000 midlife-0.0.3/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-06 02:05:56.765172 midlife-0.0.3/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      932 2023-05-06 02:05:01.000000 midlife-0.0.3/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 02:05:56.748047 midlife-0.0.3/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 02:05:56.763179 midlife-0.0.3/src/midlife.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      211 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       42 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        8 2023-05-06 02:05:56.000000 midlife-0.0.3/src/midlife.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2639 2023-05-06 01:51:22.000000 midlife-0.0.3/src/midlife.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 03:23:48.900654 midlife-0.0.4/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 03:23:48.899697 midlife-0.0.4/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      729 2023-05-06 02:04:11.000000 midlife-0.0.4/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-06 03:23:48.900654 midlife-0.0.4/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      932 2023-05-06 03:23:26.000000 midlife-0.0.4/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 03:23:48.891521 midlife-0.0.4/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 03:23:48.898824 midlife-0.0.4/src/midlife.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      211 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       42 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        8 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     2639 2023-05-06 03:23:12.000000 midlife-0.0.4/src/midlife.py
```

### Comparing `midlife-0.0.3/PKG-INFO` & `midlife-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midlife
-Version: 0.0.3
+Version: 0.0.4
 Summary: impact of COVID-19 on mortality of midlife
 Home-page: https://github.com/ytakefuji/vuv
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/midlife
 Platform: UNKNOWN
```

### Comparing `midlife-0.0.3/README.md` & `midlife-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `midlife-0.0.3/setup.py` & `midlife-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="midlife",
-    version="0.0.3",
+    version="0.0.4",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="impact of COVID-19 on mortality of midlife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/vuv",
     project_urls={
```

### Comparing `midlife-0.0.3/src/midlife.egg-info/PKG-INFO` & `midlife-0.0.4/src/midlife.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midlife
-Version: 0.0.3
+Version: 0.0.4
 Summary: impact of COVID-19 on mortality of midlife
 Home-page: https://github.com/ytakefuji/vuv
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/midlife
 Platform: UNKNOWN
```

### Comparing `midlife-0.0.3/src/midlife.py` & `midlife-0.0.4/src/midlife.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 model=np.poly1d(np.polyfit(years[0:-2],a2[0:-2],degree))
 print('45:49 years:',round((a2[-1]-int(model(2020)))/int(model(2020)),3))
 error=r2(model(years[0:-2]),a2[0:-2])
 print('r2=',round(error,3),'\n')
 
 model=np.poly1d(np.polyfit(years[0:-2],a3[0:-2],degree))
-print('5--54 years:',round((a3[-1]-int(model(2020)))/int(model(2020)),3))
+print('50-54 years:',round((a3[-1]-int(model(2020)))/int(model(2020)),3))
 error=r2(model(years[0:-2]),a3[0:-2])
 print('r2=',round(error,3),'\n')
 
 model=np.poly1d(np.polyfit(years[0:-2],a4[0:-2],degree))
 print('55-59 years:',round((a4[-1]-int(model(2020)))/int(model(2020)),3))
 error=r2(model(years[0:-2]),a4[0:-2])
 print('r2=',round(error,3),'\n')
```

