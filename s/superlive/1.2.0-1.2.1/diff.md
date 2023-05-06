# Comparing `tmp/superlive-1.2.0.tar.gz` & `tmp/superlive-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/superlive-1.2.0.tar", last modified: Sat May  6 02:34:22 2023, max compression
+gzip compressed data, was "dist/superlive-1.2.1.tar", last modified: Sat May  6 02:37:26 2023, max compression
```

## Comparing `superlive-1.2.0.tar` & `superlive-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:34:22.241406 superlive-1.2.0/
--rw-r--r--   0 sher       (501) staff       (20)     1050 2023-05-06 02:03:51.000000 superlive-1.2.0/LICENSE
--rw-r--r--   0 sher       (501) staff       (20)      545 2023-05-06 02:34:22.241483 superlive-1.2.0/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)       30 2023-05-05 03:48:28.000000 superlive-1.2.0/README.md
--rw-r--r--   0 sher       (501) staff       (20)       80 2023-05-06 02:31:09.000000 superlive-1.2.0/pyproject.toml
--rw-r--r--   0 sher       (501) staff       (20)      708 2023-05-06 02:34:22.241843 superlive-1.2.0/setup.cfg
--rw-r--r--   0 sher       (501) staff       (20)     1253 2023-05-06 02:32:51.000000 superlive-1.2.0/setup.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:34:22.238482 superlive-1.2.0/src/
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:34:22.239677 superlive-1.2.0/src/superlive/
--rw-r--r--   0 sher       (501) staff       (20)        0 2023-05-06 01:58:26.000000 superlive-1.2.0/src/superlive/__init__.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:34:22.240799 superlive-1.2.0/src/superlive/core/
--rw-r--r--   0 sher       (501) staff       (20)       86 2023-05-05 07:15:25.000000 superlive-1.2.0/src/superlive/core/__init__.py
--rw-r--r--   0 sher       (501) staff       (20)      965 2023-05-05 03:26:05.000000 superlive-1.2.0/src/superlive/core/http_client.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:34:22.241105 superlive-1.2.0/src/superlive/streams/
--rw-r--r--   0 sher       (501) staff       (20)       73 2023-05-05 07:15:46.000000 superlive-1.2.0/src/superlive/streams/__init__.py
--rw-r--r--   0 sher       (501) staff       (20)     2242 2023-05-06 01:58:53.000000 superlive-1.2.0/src/superlive/streams/host.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:34:22.240450 superlive-1.2.0/src/superlive.egg-info/
--rw-r--r--   0 sher       (501) staff       (20)      545 2023-05-06 02:34:22.000000 superlive-1.2.0/src/superlive.egg-info/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      415 2023-05-06 02:34:22.000000 superlive-1.2.0/src/superlive.egg-info/SOURCES.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-06 02:34:22.000000 superlive-1.2.0/src/superlive.egg-info/dependency_links.txt
--rw-r--r--   0 sher       (501) staff       (20)       89 2023-05-06 02:34:22.000000 superlive-1.2.0/src/superlive.egg-info/requires.txt
--rw-r--r--   0 sher       (501) staff       (20)       10 2023-05-06 02:34:22.000000 superlive-1.2.0/src/superlive.egg-info/top_level.txt
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:34:22.241276 superlive-1.2.0/tests/
--rw-r--r--   0 sher       (501) staff       (20)     1082 2023-05-06 01:58:53.000000 superlive-1.2.0/tests/test_api_client.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:37:26.262346 superlive-1.2.1/
+-rw-r--r--   0 sher       (501) staff       (20)     1050 2023-05-06 02:03:51.000000 superlive-1.2.1/LICENSE
+-rw-r--r--   0 sher       (501) staff       (20)      545 2023-05-06 02:37:26.262417 superlive-1.2.1/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)       30 2023-05-05 03:48:28.000000 superlive-1.2.1/README.md
+-rw-r--r--   0 sher       (501) staff       (20)       80 2023-05-06 02:31:09.000000 superlive-1.2.1/pyproject.toml
+-rw-r--r--   0 sher       (501) staff       (20)      708 2023-05-06 02:37:26.262749 superlive-1.2.1/setup.cfg
+-rw-r--r--   0 sher       (501) staff       (20)     1253 2023-05-06 02:32:51.000000 superlive-1.2.1/setup.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:37:26.258828 superlive-1.2.1/src/
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:37:26.260161 superlive-1.2.1/src/superlive/
+-rw-r--r--   0 sher       (501) staff       (20)        0 2023-05-06 01:58:26.000000 superlive-1.2.1/src/superlive/__init__.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:37:26.261304 superlive-1.2.1/src/superlive/core/
+-rw-r--r--   0 sher       (501) staff       (20)       86 2023-05-05 07:15:25.000000 superlive-1.2.1/src/superlive/core/__init__.py
+-rw-r--r--   0 sher       (501) staff       (20)      965 2023-05-05 03:26:05.000000 superlive-1.2.1/src/superlive/core/http_client.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:37:26.261866 superlive-1.2.1/src/superlive/streams/
+-rw-r--r--   0 sher       (501) staff       (20)       73 2023-05-05 07:15:46.000000 superlive-1.2.1/src/superlive/streams/__init__.py
+-rw-r--r--   0 sher       (501) staff       (20)     2242 2023-05-06 01:58:53.000000 superlive-1.2.1/src/superlive/streams/host.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:37:26.260841 superlive-1.2.1/src/superlive.egg-info/
+-rw-r--r--   0 sher       (501) staff       (20)      545 2023-05-06 02:37:26.000000 superlive-1.2.1/src/superlive.egg-info/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      415 2023-05-06 02:37:26.000000 superlive-1.2.1/src/superlive.egg-info/SOURCES.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-06 02:37:26.000000 superlive-1.2.1/src/superlive.egg-info/dependency_links.txt
+-rw-r--r--   0 sher       (501) staff       (20)       89 2023-05-06 02:37:26.000000 superlive-1.2.1/src/superlive.egg-info/requires.txt
+-rw-r--r--   0 sher       (501) staff       (20)       10 2023-05-06 02:37:26.000000 superlive-1.2.1/src/superlive.egg-info/top_level.txt
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-06 02:37:26.262116 superlive-1.2.1/tests/
+-rw-r--r--   0 sher       (501) staff       (20)     1082 2023-05-06 01:58:53.000000 superlive-1.2.1/tests/test_api_client.py
```

### Comparing `superlive-1.2.0/LICENSE` & `superlive-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superlive-1.2.0/PKG-INFO` & `superlive-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlive
-Version: 1.2.0
+Version: 1.2.1
 Summary: Superlive Python SDK
 Home-page: https://github.com/sophatahsher/superlive_sdk_python
 Author: DR-Tech
 Author-email: dev@dr-tech.co
 Project-URL: Bug Tracker, https://github.com/sophatahsher/superlive_sdk_python/-/issues
 Project-URL: repository, https://github.com/sophatahsher/superlive_sdk_python
 Keywords: Superlive
```

### Comparing `superlive-1.2.0/setup.cfg` & `superlive-1.2.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = superlive
-version = 1.2.0
+version = 1.2.1
 author = DR-Tech
 author_email = dev@dr-tech.co
 description = Superlive Streaming Host
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sophatahsher/superlive_sdk_python
 project_urls =
```

### Comparing `superlive-1.2.0/setup.py` & `superlive-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `superlive-1.2.0/src/superlive/core/http_client.py` & `superlive-1.2.1/src/superlive/core/http_client.py`

 * *Files identical despite different names*

### Comparing `superlive-1.2.0/src/superlive/streams/host.py` & `superlive-1.2.1/src/superlive/streams/host.py`

 * *Files identical despite different names*

### Comparing `superlive-1.2.0/src/superlive.egg-info/PKG-INFO` & `superlive-1.2.1/src/superlive.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlive
-Version: 1.2.0
+Version: 1.2.1
 Summary: Superlive Python SDK
 Home-page: https://github.com/sophatahsher/superlive_sdk_python
 Author: DR-Tech
 Author-email: dev@dr-tech.co
 Project-URL: Bug Tracker, https://github.com/sophatahsher/superlive_sdk_python/-/issues
 Project-URL: repository, https://github.com/sophatahsher/superlive_sdk_python
 Keywords: Superlive
```

### Comparing `superlive-1.2.0/tests/test_api_client.py` & `superlive-1.2.1/tests/test_api_client.py`

 * *Files identical despite different names*

