# Comparing `tmp/hilly-0.1.2a0.tar.gz` & `tmp/hilly-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilly-0.1.2a0.tar", max compression
+gzip compressed data, was "hilly-0.1.3.tar", max compression
```

## Comparing `hilly-0.1.2a0.tar` & `hilly-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-06 21:10:21.625217 hilly-0.1.2a0/LICENSE
--rw-r--r--   0        0        0     1979 2023-05-06 18:30:35.386359 hilly-0.1.2a0/README.md
--rw-r--r--   0        0        0      491 2023-05-06 17:51:43.415570 hilly-0.1.2a0/hilly/__init__.py
--rw-r--r--   0        0        0      126 2023-05-06 17:29:56.362666 hilly-0.1.2a0/hilly/constants.py
--rw-r--r--   0        0        0     3015 2023-05-05 04:28:25.917707 hilly-0.1.2a0/hilly/io.py
--rw-r--r--   0        0        0     4202 2023-05-05 04:11:43.516707 hilly-0.1.2a0/hilly/ski.py
--rw-r--r--   0        0        0     5360 2023-05-05 04:28:25.921707 hilly-0.1.2a0/hilly/utils.py
--rw-r--r--   0        0        0      729 2023-05-06 21:18:11.722575 hilly-0.1.2a0/pyproject.toml
--rw-r--r--   0        0        0     2934 1970-01-01 00:00:00.000000 hilly-0.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-06 21:23:55.430355 hilly-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1979 2023-05-06 21:23:55.430355 hilly-0.1.3/README.md
+-rw-r--r--   0        0        0      491 2023-05-06 21:23:55.434355 hilly-0.1.3/hilly/__init__.py
+-rw-r--r--   0        0        0      126 2023-05-06 21:23:55.434355 hilly-0.1.3/hilly/constants.py
+-rw-r--r--   0        0        0     3015 2023-05-06 21:23:55.434355 hilly-0.1.3/hilly/io.py
+-rw-r--r--   0        0        0     4202 2023-05-06 21:23:55.434355 hilly-0.1.3/hilly/ski.py
+-rw-r--r--   0        0        0     5360 2023-05-06 21:23:55.434355 hilly-0.1.3/hilly/utils.py
+-rw-r--r--   0        0        0      728 2023-05-06 21:23:55.435355 hilly-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2932 1970-01-01 00:00:00.000000 hilly-0.1.3/PKG-INFO
```

### Comparing `hilly-0.1.2a0/LICENSE` & `hilly-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hilly-0.1.2a0/README.md` & `hilly-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hilly-0.1.2a0/hilly/io.py` & `hilly-0.1.3/hilly/io.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.2a0/hilly/ski.py` & `hilly-0.1.3/hilly/ski.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.2a0/hilly/utils.py` & `hilly-0.1.3/hilly/utils.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.2a0/pyproject.toml` & `hilly-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hilly"
-version = "0.1.2a"
+version = "0.1.3"
 description = "Tools for summarizing and viewing sporty GPX traces"
 authors = ["Ryan <code+git@mcginger.net>"]
 readme = "README.md"
 keywords = ["gpx", "maps", "outdoors"]
 repository = "https://gitlab.com/ryanmcginger/hilly"
 
 [tool.poetry.dependencies]
```

### Comparing `hilly-0.1.2a0/PKG-INFO` & `hilly-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilly
-Version: 0.1.2a0
+Version: 0.1.3
 Summary: Tools for summarizing and viewing sporty GPX traces
 Home-page: https://gitlab.com/ryanmcginger/hilly
 Keywords: gpx,maps,outdoors
 Author: Ryan
 Author-email: code+git@mcginger.net
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
```

