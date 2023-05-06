# Comparing `tmp/rayserverdl-1.0.0.tar.gz` & `tmp/rayserverdl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayserverdl-1.0.0.tar", last modified: Sat May  6 04:29:39 2023, max compression
+gzip compressed data, was "rayserverdl-1.0.1.tar", last modified: Sat May  6 04:38:19 2023, max compression
```

## Comparing `rayserverdl-1.0.0.tar` & `rayserverdl-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 04:29:39.838029 rayserverdl-1.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 rayserverdl-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1026 2023-05-06 04:29:39.824028 rayserverdl-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-05-06 04:21:57.000000 rayserverdl-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 04:29:39.648018 rayserverdl-1.0.0/rayserverdl/
--rw-rw-rw-   0        0        0       75 2023-05-04 19:18:17.000000 rayserverdl-1.0.0/rayserverdl/version.py
-drwxrwxrwx   0        0        0        0 2023-05-06 04:29:39.808027 rayserverdl-1.0.0/rayserverdl.egg-info/
--rw-rw-rw-   0        0        0     1026 2023-05-06 04:29:37.000000 rayserverdl-1.0.0/rayserverdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-06 04:29:38.000000 rayserverdl-1.0.0/rayserverdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 04:29:37.000000 rayserverdl-1.0.0/rayserverdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 04:29:37.000000 rayserverdl-1.0.0/rayserverdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 04:29:38.000000 rayserverdl-1.0.0/rayserverdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 04:29:37.000000 rayserverdl-1.0.0/rayserverdl.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-06 04:29:39.841029 rayserverdl-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1653 2023-05-06 04:28:01.000000 rayserverdl-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:38:19.546754 rayserverdl-1.0.1/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 rayserverdl-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1026 2023-05-06 04:38:19.542754 rayserverdl-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-05-06 04:21:57.000000 rayserverdl-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 04:38:19.467750 rayserverdl-1.0.1/rayserverdl/
+-rw-rw-rw-   0        0        0     3580 2023-05-06 04:18:53.000000 rayserverdl-1.0.1/rayserverdl/__init__.py
+-rw-rw-rw-   0        0        0     3580 2023-05-06 04:18:53.000000 rayserverdl-1.0.1/rayserverdl/d.py
+-rw-rw-rw-   0        0        0       75 2023-05-06 04:36:54.000000 rayserverdl-1.0.1/rayserverdl/version.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:38:19.537754 rayserverdl-1.0.1/rayserverdl.egg-info/
+-rw-rw-rw-   0        0        0     1026 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-06 04:38:19.547754 rayserverdl-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1653 2023-05-06 04:28:01.000000 rayserverdl-1.0.1/setup.py
```

### Comparing `rayserverdl-1.0.0/LICENSE` & `rayserverdl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rayserverdl-1.0.0/PKG-INFO` & `rayserverdl-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayserverdl
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/rayserverdl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,downloader,stream,files
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rayserverdl-1.0.0/rayserverdl.egg-info/PKG-INFO` & `rayserverdl-1.0.1/rayserverdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayserverdl
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/rayserverdl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,downloader,stream,files
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rayserverdl-1.0.0/setup.py` & `rayserverdl-1.0.1/setup.py`

 * *Files identical despite different names*

