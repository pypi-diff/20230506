# Comparing `tmp/readable_number-0.1.1.tar.gz` & `tmp/readable_number-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readable_number-0.1.1.tar", last modified: Sat May  6 00:02:52 2023, max compression
+gzip compressed data, was "readable_number-0.1.2.tar", last modified: Sat May  6 00:47:14 2023, max compression
```

## Comparing `readable_number-0.1.1.tar` & `readable_number-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:02:52.825119 readable_number-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-06 00:02:41.000000 readable_number-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 00:02:41.000000 readable_number-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-06 00:02:52.825119 readable_number-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-06 00:02:41.000000 readable_number-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:02:52.825119 readable_number-0.1.1/readable_number/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 00:02:41.000000 readable_number-0.1.1/readable_number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-05-06 00:02:41.000000 readable_number-0.1.1/readable_number/readable_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:02:52.825119 readable_number-0.1.1/readable_number.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-06 00:02:52.000000 readable_number-0.1.1/readable_number.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-06 00:02:52.000000 readable_number-0.1.1/readable_number.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:02:52.000000 readable_number-0.1.1/readable_number.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 00:02:52.000000 readable_number-0.1.1/readable_number.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-06 00:02:52.825119 readable_number-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-06 00:02:41.000000 readable_number-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:02:52.825119 readable_number-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-05-06 00:02:41.000000 readable_number-0.1.1/tests/test_readable_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:47:14.132539 readable_number-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-06 00:46:57.000000 readable_number-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 00:46:57.000000 readable_number-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-06 00:47:14.132539 readable_number-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-06 00:46:57.000000 readable_number-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:47:14.132539 readable_number-0.1.2/readable_number/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 00:46:57.000000 readable_number-0.1.2/readable_number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-05-06 00:46:57.000000 readable_number-0.1.2/readable_number/readable_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:47:14.132539 readable_number-0.1.2/readable_number.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-06 00:47:14.000000 readable_number-0.1.2/readable_number.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-06 00:47:14.000000 readable_number-0.1.2/readable_number.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:47:14.000000 readable_number-0.1.2/readable_number.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 00:47:14.000000 readable_number-0.1.2/readable_number.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-06 00:47:14.132539 readable_number-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-06 00:46:57.000000 readable_number-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:47:14.132539 readable_number-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-05-06 00:46:57.000000 readable_number-0.1.2/tests/test_readable_number.py
```

### Comparing `readable_number-0.1.1/LICENSE` & `readable_number-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `readable_number-0.1.1/PKG-INFO` & `readable_number-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readable_number
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library to print numbers in human readable format
 Home-page: https://github.com/jsh9/readable-number
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `readable_number-0.1.1/README.md` & `readable_number-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `readable_number-0.1.1/readable_number/readable_number.py` & `readable_number-0.1.2/readable_number/readable_number.py`

 * *Files identical despite different names*

### Comparing `readable_number-0.1.1/readable_number.egg-info/PKG-INFO` & `readable_number-0.1.2/readable_number.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readable-number
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library to print numbers in human readable format
 Home-page: https://github.com/jsh9/readable-number
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `readable_number-0.1.1/setup.cfg` & `readable_number-0.1.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = readable_number
-version = v0.1.1
+version = v0.1.2
 description = A Python library to print numbers in human readable format
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/readable-number
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `readable_number-0.1.1/tests/test_readable_number.py` & `readable_number-0.1.2/tests/test_readable_number.py`

 * *Files identical despite different names*

