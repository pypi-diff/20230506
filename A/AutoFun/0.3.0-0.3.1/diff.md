# Comparing `tmp/AutoFun-0.3.0.tar.gz` & `tmp/AutoFun-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoFun-0.3.0.tar", last modified: Fri May  5 11:19:28 2023, max compression
+gzip compressed data, was "AutoFun-0.3.1.tar", last modified: Sat May  6 01:45:12 2023, max compression
```

## Comparing `AutoFun-0.3.0.tar` & `AutoFun-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:19:28.202097 AutoFun-0.3.0/
-drwxrwxrwx   0        0        0        0 2023-05-05 11:19:28.201096 AutoFun-0.3.0/AutoFun.egg-info/
--rw-rw-rw-   0        0        0      429 2023-05-05 11:19:28.000000 AutoFun-0.3.0/AutoFun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-05-05 11:19:28.000000 AutoFun-0.3.0/AutoFun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:19:28.000000 AutoFun-0.3.0/AutoFun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:19:28.000000 AutoFun-0.3.0/AutoFun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      429 2023-05-05 11:19:28.202097 AutoFun-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.0/README.md
--rw-rw-rw-   0        0        0      135 2023-05-05 11:19:28.203097 AutoFun-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-05-05 11:18:43.000000 AutoFun-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.105734 AutoFun-0.3.1/
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.077720 AutoFun-0.3.1/AutoFun/
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.084725 AutoFun-0.3.1/AutoFun/CutPdf/
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.086720 AutoFun-0.3.1/AutoFun/CutPdf/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/CutPdf/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.087720 AutoFun-0.3.1/AutoFun/CutPdf/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/CutPdf/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/CutPdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.088722 AutoFun-0.3.1/AutoFun/OcrFinish/
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.089758 AutoFun-0.3.1/AutoFun/OcrFinish/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrFinish/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrFinish/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.090721 AutoFun-0.3.1/AutoFun/OcrPicFun/
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.091721 AutoFun-0.3.1/AutoFun/OcrPicFun/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrPicFun/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.092721 AutoFun-0.3.1/AutoFun/OcrPicFun/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrPicFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/OcrPicFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.094721 AutoFun-0.3.1/AutoFun/OcrTableFun/
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.096721 AutoFun-0.3.1/AutoFun/OcrTableFun/Function/
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:53.000000 AutoFun-0.3.1/AutoFun/OcrTableFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:41.000000 AutoFun-0.3.1/AutoFun/OcrTableFun/Function/saveLoad.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.100725 AutoFun-0.3.1/AutoFun/OcrTableFun/Ui/
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.1/AutoFun/OcrTableFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.1/AutoFun/OcrTableFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.102727 AutoFun-0.3.1/AutoFun/SplitPdfFun/
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.103744 AutoFun-0.3.1/AutoFun/SplitPdfFun/Function/
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.1/AutoFun/SplitPdfFun/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.104727 AutoFun-0.3.1/AutoFun/SplitPdfFun/Ui/
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:00:01.000000 AutoFun-0.3.1/AutoFun/SplitPdfFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:59.000000 AutoFun-0.3.1/AutoFun/SplitPdfFun/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:17.000000 AutoFun-0.3.1/AutoFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:45:12.083734 AutoFun-0.3.1/AutoFun.egg-info/
+-rw-rw-rw-   0        0        0      429 2023-05-06 01:45:12.000000 AutoFun-0.3.1/AutoFun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2023-05-06 01:45:12.000000 AutoFun-0.3.1/AutoFun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 01:45:12.000000 AutoFun-0.3.1/AutoFun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 01:45:12.000000 AutoFun-0.3.1/AutoFun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      429 2023-05-06 01:45:12.106725 AutoFun-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.1/README.md
+-rw-rw-rw-   0        0        0      135 2023-05-06 01:45:12.106725 AutoFun-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-05-06 01:45:07.000000 AutoFun-0.3.1/setup.py
```

### Comparing `AutoFun-0.3.0/LICENSE.txt` & `AutoFun-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.0/setup.py` & `AutoFun-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 0
+PATCH = 1
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "AutoFun",
```

