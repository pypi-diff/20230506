# Comparing `tmp/pyatproto-0.0.1.tar.gz` & `tmp/pyatproto-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatproto-0.0.1.tar", last modified: Tue Mar  7 21:58:15 2023, max compression
+gzip compressed data, was "pyatproto-0.1.tar", last modified: Sat May  6 10:58:25 2023, max compression
```

## Comparing `pyatproto-0.0.1.tar` & `pyatproto-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-03-07 21:58:15.047307 pyatproto-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      904 2023-03-07 21:50:06.000000 pyatproto-0.0.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     1315 2023-03-07 21:58:15.047379 pyatproto-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      780 2023-03-07 21:55:36.000000 pyatproto-0.0.1/README.md
--rw-r--r--   0 james      (501) staff       (20)      257 2023-03-07 21:56:43.000000 pyatproto-0.0.1/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)      659 2023-03-07 21:58:15.047641 pyatproto-0.0.1/setup.cfg
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-03-07 21:58:15.045955 pyatproto-0.0.1/src/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-03-07 21:58:15.047190 pyatproto-0.0.1/src/pyatproto.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     1315 2023-03-07 21:58:15.000000 pyatproto-0.0.1/src/pyatproto.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      190 2023-03-07 21:58:15.000000 pyatproto-0.0.1/src/pyatproto.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-03-07 21:58:15.000000 pyatproto-0.0.1/src/pyatproto.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-03-07 21:58:15.000000 pyatproto-0.0.1/src/pyatproto.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-06 10:58:25.153661 pyatproto-0.1/
+-rw-r--r--   0 james      (501) staff       (20)      904 2023-03-07 21:50:06.000000 pyatproto-0.1/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     1313 2023-05-06 10:58:25.153761 pyatproto-0.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      780 2023-05-06 10:58:18.000000 pyatproto-0.1/README.md
+-rw-r--r--   0 james      (501) staff       (20)      257 2023-03-07 21:56:43.000000 pyatproto-0.1/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)      657 2023-05-06 10:58:25.154582 pyatproto-0.1/setup.cfg
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-06 10:58:25.152279 pyatproto-0.1/src/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-06 10:58:25.153547 pyatproto-0.1/src/pyatproto.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     1313 2023-05-06 10:58:25.000000 pyatproto-0.1/src/pyatproto.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      190 2023-05-06 10:58:25.000000 pyatproto-0.1/src/pyatproto.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-05-06 10:58:25.000000 pyatproto-0.1/src/pyatproto.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-05-06 10:58:25.000000 pyatproto-0.1/src/pyatproto.egg-info/top_level.txt
```

### Comparing `pyatproto-0.0.1/LICENSE` & `pyatproto-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatproto-0.0.1/PKG-INFO` & `pyatproto-0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatproto
-Version: 0.0.1
+Version: 0.1
 Summary: A wrapper for interacting with the AT Protocol API.
 Home-page: https://github.com/capjamesg/pyatproto
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Project-URL: Bug Tracker, https://github.com/capjamesg/pyatproto/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyatproto-0.0.1/README.md` & `pyatproto-0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyatproto-0.0.1/setup.cfg` & `pyatproto-0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyatproto
-version = 0.0.1
+version = 0.1
 author = capjamesg
 author_email = jamesg@jamesg.blog
 description = A wrapper for interacting with the AT Protocol API.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/capjamesg/pyatproto
 project_urls =
```

### Comparing `pyatproto-0.0.1/src/pyatproto.egg-info/PKG-INFO` & `pyatproto-0.1/src/pyatproto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatproto
-Version: 0.0.1
+Version: 0.1
 Summary: A wrapper for interacting with the AT Protocol API.
 Home-page: https://github.com/capjamesg/pyatproto
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Project-URL: Bug Tracker, https://github.com/capjamesg/pyatproto/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

