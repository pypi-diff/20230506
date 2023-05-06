# Comparing `tmp/OnloadTable-0.3.0.tar.gz` & `tmp/OnloadTable-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnloadTable-0.3.0.tar", last modified: Fri May  5 12:18:26 2023, max compression
+gzip compressed data, was "OnloadTable-0.3.1.tar", last modified: Sat May  6 02:35:46 2023, max compression
```

## Comparing `OnloadTable-0.3.0.tar` & `OnloadTable-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:18:26.144567 OnloadTable-0.3.0/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 OnloadTable-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 OnloadTable-0.3.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-05 12:18:26.121767 OnloadTable-0.3.0/OnloadTable/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:18:26.132821 OnloadTable-0.3.0/OnloadTable/Function/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:18:26.135825 OnloadTable-0.3.0/OnloadTable/Function/Function/
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.0/OnloadTable/Function/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:18:26.139825 OnloadTable-0.3.0/OnloadTable/Function/Ui/
--rw-rw-rw-   0        0        0    46080 2023-04-28 06:34:36.000000 OnloadTable-0.3.0/OnloadTable/Function/Ui/ExcelUi.pyd
--rw-rw-rw-   0        0        0    40448 2023-04-28 06:34:44.000000 OnloadTable-0.3.0/OnloadTable/Function/Ui/MaskWin.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.0/OnloadTable/Function/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.0/OnloadTable/Function/__init__.py
--rw-rw-rw-   0        0        0   290816 2023-05-05 11:08:53.000000 OnloadTable-0.3.0/OnloadTable/Function/mysqlexcel.pyd
--rw-rw-rw-   0        0        0    69632 2023-04-28 06:24:23.000000 OnloadTable-0.3.0/OnloadTable/Function/optionDb.pyd
--rw-rw-rw-   0        0        0       36 2023-03-01 03:36:33.000000 OnloadTable-0.3.0/OnloadTable/Function/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:18:26.143556 OnloadTable-0.3.0/OnloadTable/Ui/
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.0/OnloadTable/Ui/__init__.py
--rw-rw-rw-   0        0        0    90112 2023-05-05 10:30:39.000000 OnloadTable-0.3.0/OnloadTable/Ui/onloadUi.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.0/OnloadTable/__init__.py
--rw-rw-rw-   0        0        0   244224 2023-05-05 09:28:06.000000 OnloadTable-0.3.0/OnloadTable/onload.pyd
-drwxrwxrwx   0        0        0        0 2023-05-05 12:18:26.127820 OnloadTable-0.3.0/OnloadTable.egg-info/
--rw-rw-rw-   0        0        0      400 2023-05-05 12:18:26.000000 OnloadTable-0.3.0/OnloadTable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-05-05 12:18:26.000000 OnloadTable-0.3.0/OnloadTable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:18:26.000000 OnloadTable-0.3.0/OnloadTable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 12:18:26.000000 OnloadTable-0.3.0/OnloadTable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      400 2023-05-05 12:18:26.144567 OnloadTable-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 OnloadTable-0.3.0/README.md
--rw-rw-rw-   0        0        0      135 2023-05-05 12:18:26.145573 OnloadTable-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      962 2023-05-05 12:18:21.000000 OnloadTable-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.071701 OnloadTable-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 OnloadTable-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 OnloadTable-0.3.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.044693 OnloadTable-0.3.1/OnloadTable/
+drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.059695 OnloadTable-0.3.1/OnloadTable/Function/
+drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.060693 OnloadTable-0.3.1/OnloadTable/Function/Function/
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Function/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.065693 OnloadTable-0.3.1/OnloadTable/Function/Ui/
+-rw-rw-rw-   0        0        0    46080 2023-04-28 06:34:36.000000 OnloadTable-0.3.1/OnloadTable/Function/Ui/ExcelUi.pyd
+-rw-rw-rw-   0        0        0    40448 2023-04-28 06:34:44.000000 OnloadTable-0.3.1/OnloadTable/Function/Ui/MaskWin.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Function/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Function/__init__.py
+-rw-rw-rw-   0        0        0   290816 2023-05-05 11:08:53.000000 OnloadTable-0.3.1/OnloadTable/Function/mysqlexcel.pyd
+-rw-rw-rw-   0        0        0    69632 2023-04-28 06:24:23.000000 OnloadTable-0.3.1/OnloadTable/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0       36 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Function/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.068693 OnloadTable-0.3.1/OnloadTable/Ui/
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Ui/__init__.py
+-rw-rw-rw-   0        0        0    90112 2023-05-05 10:30:39.000000 OnloadTable-0.3.1/OnloadTable/Ui/onloadUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/__init__.py
+-rw-rw-rw-   0        0        0   244224 2023-05-06 02:29:25.000000 OnloadTable-0.3.1/OnloadTable/onload.pyd
+drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.050693 OnloadTable-0.3.1/OnloadTable.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-05-06 02:35:45.000000 OnloadTable-0.3.1/OnloadTable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-05-06 02:35:46.000000 OnloadTable-0.3.1/OnloadTable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 02:35:45.000000 OnloadTable-0.3.1/OnloadTable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 02:35:45.000000 OnloadTable-0.3.1/OnloadTable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      400 2023-05-06 02:35:46.072693 OnloadTable-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 OnloadTable-0.3.1/README.md
+-rw-rw-rw-   0        0        0      135 2023-05-06 02:35:46.073590 OnloadTable-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      962 2023-05-06 02:35:27.000000 OnloadTable-0.3.1/setup.py
```

### Comparing `OnloadTable-0.3.0/LICENSE.txt` & `OnloadTable-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnloadTable-0.3.0/OnloadTable.egg-info/SOURCES.txt` & `OnloadTable-0.3.1/OnloadTable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OnloadTable-0.3.0/setup.py` & `OnloadTable-0.3.1/setup.py`

 * *Files 2% similar despite different names*

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
 	name = "OnloadTable",
```

