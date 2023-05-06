# Comparing `tmp/superlive_sdk-1.0.0.tar.gz` & `tmp/superlive_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/superlive_sdk-1.0.0.tar", last modified: Sat May  6 03:24:41 2023, max compression
+gzip compressed data, was "dist/superlive_sdk-1.0.1.tar", last modified: Sat May  6 03:28:41 2023, max compression
```

## Comparing `superlive_sdk-1.0.0.tar` & `superlive_sdk-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:24:41.865743 superlive_sdk-1.0.0/
--rw-r--r--   0 sher       (501) staff       (20)     1050 2023-05-06 02:03:51.000000 superlive_sdk-1.0.0/LICENSE
--rw-r--r--   0 sher       (501) staff       (20)      412 2023-05-06 03:24:41.865590 superlive_sdk-1.0.0/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)       30 2023-05-05 03:48:28.000000 superlive_sdk-1.0.0/README.md
--rw-r--r--   0 sher       (501) staff       (20)       80 2023-05-06 02:31:09.000000 superlive_sdk-1.0.0/pyproject.toml
--rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-06 03:24:41.865782 superlive_sdk-1.0.0/setup.cfg
--rw-r--r--   0 sher       (501) staff       (20)     1269 2023-05-06 03:23:59.000000 superlive_sdk-1.0.0/setup.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:24:41.862690 superlive_sdk-1.0.0/src/
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:24:41.863835 superlive_sdk-1.0.0/src/superlive/
--rw-r--r--   0 sher       (501) staff       (20)      259 2023-05-06 03:18:55.000000 superlive_sdk-1.0.0/src/superlive/__init__.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:24:41.864140 superlive_sdk-1.0.0/src/superlive/core/
--rw-r--r--   0 sher       (501) staff       (20)      285 2023-05-06 03:11:46.000000 superlive_sdk-1.0.0/src/superlive/core/__init__.py
--rw-r--r--   0 sher       (501) staff       (20)      965 2023-05-05 03:26:05.000000 superlive_sdk-1.0.0/src/superlive/core/http_client.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:24:41.864449 superlive_sdk-1.0.0/src/superlive/streams/
--rw-r--r--   0 sher       (501) staff       (20)       59 2023-05-06 03:19:07.000000 superlive_sdk-1.0.0/src/superlive/streams/__init__.py
--rw-r--r--   0 sher       (501) staff       (20)     2229 2023-05-06 03:18:23.000000 superlive_sdk-1.0.0/src/superlive/streams/host.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:24:41.865228 superlive_sdk-1.0.0/superlive_sdk.egg-info/
--rw-r--r--   0 sher       (501) staff       (20)      412 2023-05-06 03:24:41.000000 superlive_sdk-1.0.0/superlive_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      405 2023-05-06 03:24:41.000000 superlive_sdk-1.0.0/superlive_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-06 03:24:41.000000 superlive_sdk-1.0.0/superlive_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sher       (501) staff       (20)       89 2023-05-06 03:24:41.000000 superlive_sdk-1.0.0/superlive_sdk.egg-info/requires.txt
--rw-r--r--   0 sher       (501) staff       (20)       10 2023-05-06 03:24:41.000000 superlive_sdk-1.0.0/superlive_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:24:41.865399 superlive_sdk-1.0.0/tests/
--rw-r--r--   0 sher       (501) staff       (20)     1074 2023-05-06 03:16:58.000000 superlive_sdk-1.0.0/tests/test_api_client.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:28:41.506737 superlive_sdk-1.0.1/
+-rw-r--r--   0 sher       (501) staff       (20)     1050 2023-05-06 02:03:51.000000 superlive_sdk-1.0.1/LICENSE
+-rw-r--r--   0 sher       (501) staff       (20)      412 2023-05-06 03:28:41.506541 superlive_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)       30 2023-05-05 03:48:28.000000 superlive_sdk-1.0.1/README.md
+-rw-r--r--   0 sher       (501) staff       (20)       80 2023-05-06 02:31:09.000000 superlive_sdk-1.0.1/pyproject.toml
+-rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-06 03:28:41.506810 superlive_sdk-1.0.1/setup.cfg
+-rw-r--r--   0 sher       (501) staff       (20)     1269 2023-05-06 03:28:39.000000 superlive_sdk-1.0.1/setup.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:28:41.502915 superlive_sdk-1.0.1/src/
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:28:41.504124 superlive_sdk-1.0.1/src/superlive/
+-rw-r--r--   0 sher       (501) staff       (20)      259 2023-05-06 03:18:55.000000 superlive_sdk-1.0.1/src/superlive/__init__.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:28:41.504684 superlive_sdk-1.0.1/src/superlive/core/
+-rw-r--r--   0 sher       (501) staff       (20)      285 2023-05-06 03:11:46.000000 superlive_sdk-1.0.1/src/superlive/core/__init__.py
+-rw-r--r--   0 sher       (501) staff       (20)      965 2023-05-05 03:26:05.000000 superlive_sdk-1.0.1/src/superlive/core/http_client.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:28:41.505147 superlive_sdk-1.0.1/src/superlive/streams/
+-rw-r--r--   0 sher       (501) staff       (20)       69 2023-05-06 03:28:24.000000 superlive_sdk-1.0.1/src/superlive/streams/__init__.py
+-rw-r--r--   0 sher       (501) staff       (20)     2229 2023-05-06 03:18:23.000000 superlive_sdk-1.0.1/src/superlive/streams/host.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:28:41.506029 superlive_sdk-1.0.1/superlive_sdk.egg-info/
+-rw-r--r--   0 sher       (501) staff       (20)      412 2023-05-06 03:28:41.000000 superlive_sdk-1.0.1/superlive_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      405 2023-05-06 03:28:41.000000 superlive_sdk-1.0.1/superlive_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-06 03:28:41.000000 superlive_sdk-1.0.1/superlive_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sher       (501) staff       (20)       89 2023-05-06 03:28:41.000000 superlive_sdk-1.0.1/superlive_sdk.egg-info/requires.txt
+-rw-r--r--   0 sher       (501) staff       (20)       10 2023-05-06 03:28:41.000000 superlive_sdk-1.0.1/superlive_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 03:28:41.506168 superlive_sdk-1.0.1/tests/
+-rw-r--r--   0 sher       (501) staff       (20)     1074 2023-05-06 03:16:58.000000 superlive_sdk-1.0.1/tests/test_api_client.py
```

### Comparing `superlive_sdk-1.0.0/LICENSE` & `superlive_sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superlive_sdk-1.0.0/setup.py` & `superlive_sdk-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
 NAME = "Superlive SDK"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 PACKAGE_NAME = 'superlive_sdk'
 AUTHOR = "DR-Tech"
 AUTHOR_EMAIL = "dev@dr-tech.co"
 SHORT_DESCRIPTION = "Superlive Streaming Host"
 URL = 'https://github.com/sophatahsher/superlive_sdk_python'
 LICENSE = 'DR-Tech License 2.0'
 DESCRIPTION = "Superlive Python SDK"
```

### Comparing `superlive_sdk-1.0.0/src/superlive/core/http_client.py` & `superlive_sdk-1.0.1/src/superlive/core/http_client.py`

 * *Files identical despite different names*

### Comparing `superlive_sdk-1.0.0/src/superlive/streams/host.py` & `superlive_sdk-1.0.1/src/superlive/streams/host.py`

 * *Files identical despite different names*

### Comparing `superlive_sdk-1.0.0/tests/test_api_client.py` & `superlive_sdk-1.0.1/tests/test_api_client.py`

 * *Files identical despite different names*

