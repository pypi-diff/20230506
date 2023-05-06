# Comparing `tmp/PicsToPdfs-0.3.3.tar.gz` & `tmp/PicsToPdfs-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PicsToPdfs-0.3.3.tar", last modified: Sat May  6 03:48:31 2023, max compression
+gzip compressed data, was "PicsToPdfs-0.3.5.tar", last modified: Sat May  6 08:10:28 2023, max compression
```

## Comparing `PicsToPdfs-0.3.3.tar` & `PicsToPdfs-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.236891 PicsToPdfs-0.3.3/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      387 2023-05-06 03:48:31.236891 PicsToPdfs-0.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.222896 PicsToPdfs-0.3.3/PicsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.231889 PicsToPdfs-0.3.3/PicsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.3/PicsToPdfs/Function/__init__.py
--rw-rw-rw-   0        0        0    59904 2023-04-28 06:28:35.000000 PicsToPdfs-0.3.3/PicsToPdfs/Function/imgToPdf.pyd
--rw-rw-rw-   0        0        0   110592 2023-05-05 07:05:23.000000 PicsToPdfs-0.3.3/PicsToPdfs/PicToPdf.pyd
-drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.235891 PicsToPdfs-0.3.3/PicsToPdfs/Ui/
--rw-rw-rw-   0        0        0    79360 2023-04-28 06:28:53.000000 PicsToPdfs-0.3.3/PicsToPdfs/Ui/PicToPdfUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.3/PicsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.3/PicsToPdfs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.229891 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      387 2023-05-06 03:48:31.000000 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-05-06 03:48:31.000000 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:48:31.000000 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 03:48:31.000000 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.3/README.md
--rw-rw-rw-   0        0        0      135 2023-05-06 03:48:31.237889 PicsToPdfs-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-06 03:41:29.000000 PicsToPdfs-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.534897 PicsToPdfs-0.3.5/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      387 2023-05-06 08:10:28.534897 PicsToPdfs-0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.519895 PicsToPdfs-0.3.5/PicsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.528898 PicsToPdfs-0.3.5/PicsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.5/PicsToPdfs/Function/__init__.py
+-rw-rw-rw-   0        0        0    59904 2023-04-28 06:28:35.000000 PicsToPdfs-0.3.5/PicsToPdfs/Function/imgToPdf.pyd
+-rw-rw-rw-   0        0        0   110592 2023-05-06 08:08:30.000000 PicsToPdfs-0.3.5/PicsToPdfs/PicsToPdfs.pyd
+drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.533938 PicsToPdfs-0.3.5/PicsToPdfs/Ui/
+-rw-rw-rw-   0        0        0    79360 2023-04-28 06:28:53.000000 PicsToPdfs-0.3.5/PicsToPdfs/Ui/PicToPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.5/PicsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.5/PicsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.524895 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      387 2023-05-06 08:10:28.000000 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-05-06 08:10:28.000000 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 08:10:28.000000 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 08:10:28.000000 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.5/README.md
+-rw-rw-rw-   0        0        0      135 2023-05-06 08:10:28.535894 PicsToPdfs-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-06 08:10:19.000000 PicsToPdfs-0.3.5/setup.py
```

### Comparing `PicsToPdfs-0.3.3/LICENSE.txt` & `PicsToPdfs-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PicsToPdfs-0.3.3/setup.py` & `PicsToPdfs-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 3
+PATCH = 5
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "PicsToPdfs",
```

