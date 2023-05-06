# Comparing `tmp/PicsToPdfs-0.3.0.tar.gz` & `tmp/PicsToPdfs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PicsToPdfs-0.3.0.tar", last modified: Fri May  5 12:21:18 2023, max compression
+gzip compressed data, was "PicsToPdfs-0.3.1.tar", last modified: Sat May  6 03:27:43 2023, max compression
```

## Comparing `PicsToPdfs-0.3.0.tar` & `PicsToPdfs-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.802842 PicsToPdfs-0.3.0/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      481 2023-05-05 12:21:18.802842 PicsToPdfs-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.791833 PicsToPdfs-0.3.0/PicsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.799861 PicsToPdfs-0.3.0/PicsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.0/PicsToPdfs/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.800831 PicsToPdfs-0.3.0/PicsToPdfs/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.0/PicsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.0/PicsToPdfs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.797831 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      481 2023-05-05 12:21:18.000000 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-05 12:21:18.000000 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:21:18.000000 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-05 12:21:18.000000 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.0/README.md
--rw-rw-rw-   0        0        0      135 2023-05-05 12:21:18.803829 PicsToPdfs-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-05-05 12:21:12.000000 PicsToPdfs-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.977662 PicsToPdfs-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      481 2023-05-06 03:27:43.977662 PicsToPdfs-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.967663 PicsToPdfs-0.3.1/PicsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.974666 PicsToPdfs-0.3.1/PicsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.1/PicsToPdfs/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.976708 PicsToPdfs-0.3.1/PicsToPdfs/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.1/PicsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.1/PicsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.972662 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-05-06 03:27:43.000000 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-06 03:27:43.000000 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 03:27:43.000000 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 03:27:43.000000 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.1/README.md
+-rw-rw-rw-   0        0        0      135 2023-05-06 03:27:43.978662 PicsToPdfs-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2023-05-06 03:27:26.000000 PicsToPdfs-0.3.1/setup.py
```

### Comparing `PicsToPdfs-0.3.0/LICENSE.txt` & `PicsToPdfs-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PicsToPdfs-0.3.0/setup.py` & `PicsToPdfs-0.3.1/setup.py`

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
 	name = "PicsToPdfs",
```

