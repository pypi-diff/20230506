# Comparing `tmp/syssqlitedbextension-1.0.0.tar.gz` & `tmp/syssqlitedbextension-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlitedbextension-1.0.0.tar", last modified: Sat May  6 20:39:23 2023, max compression
+gzip compressed data, was "syssqlitedbextension-1.1.0.tar", last modified: Sat May  6 20:41:29 2023, max compression
```

## Comparing `syssqlitedbextension-1.0.0.tar` & `syssqlitedbextension-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 20:39:23.849841 syssqlitedbextension-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-06 20:39:23.849841 syssqlitedbextension-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 20:39:23.849841 syssqlitedbextension-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-06 20:39:23.000000 syssqlitedbextension-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 20:39:23.849841 syssqlitedbextension-1.0.0/syssqlitedbextension/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-06 20:39:23.000000 syssqlitedbextension-1.0.0/syssqlitedbextension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 20:39:23.849841 syssqlitedbextension-1.0.0/syssqlitedbextension.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-06 20:39:23.000000 syssqlitedbextension-1.0.0/syssqlitedbextension.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-05-06 20:39:23.000000 syssqlitedbextension-1.0.0/syssqlitedbextension.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 20:39:23.000000 syssqlitedbextension-1.0.0/syssqlitedbextension.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-06 20:39:23.000000 syssqlitedbextension-1.0.0/syssqlitedbextension.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 20:41:29.624476 syssqlitedbextension-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-06 20:41:29.624476 syssqlitedbextension-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 20:41:29.624476 syssqlitedbextension-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-06 20:41:29.000000 syssqlitedbextension-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 20:41:29.624476 syssqlitedbextension-1.1.0/syssqlitedbextension/
+-rw-r--r--   0 root         (0) root         (0)    72010 2023-05-06 20:41:29.000000 syssqlitedbextension-1.1.0/syssqlitedbextension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 20:41:29.624476 syssqlitedbextension-1.1.0/syssqlitedbextension.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-06 20:41:29.000000 syssqlitedbextension-1.1.0/syssqlitedbextension.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-05-06 20:41:29.000000 syssqlitedbextension-1.1.0/syssqlitedbextension.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 20:41:29.000000 syssqlitedbextension-1.1.0/syssqlitedbextension.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-06 20:41:29.000000 syssqlitedbextension-1.1.0/syssqlitedbextension.egg-info/top_level.txt
```

### Comparing `syssqlitedbextension-1.0.0/setup.py` & `syssqlitedbextension-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syssqlitedbextension",
     version=VERSION,
```

