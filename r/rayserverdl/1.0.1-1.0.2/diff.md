# Comparing `tmp/rayserverdl-1.0.1.tar.gz` & `tmp/rayserverdl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayserverdl-1.0.1.tar", last modified: Sat May  6 04:38:19 2023, max compression
+gzip compressed data, was "rayserverdl-1.0.2.tar", last modified: Sat May  6 17:48:12 2023, max compression
```

## Comparing `rayserverdl-1.0.1.tar` & `rayserverdl-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 04:38:19.546754 rayserverdl-1.0.1/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 rayserverdl-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1026 2023-05-06 04:38:19.542754 rayserverdl-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-05-06 04:21:57.000000 rayserverdl-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 04:38:19.467750 rayserverdl-1.0.1/rayserverdl/
--rw-rw-rw-   0        0        0     3580 2023-05-06 04:18:53.000000 rayserverdl-1.0.1/rayserverdl/__init__.py
--rw-rw-rw-   0        0        0     3580 2023-05-06 04:18:53.000000 rayserverdl-1.0.1/rayserverdl/d.py
--rw-rw-rw-   0        0        0       75 2023-05-06 04:36:54.000000 rayserverdl-1.0.1/rayserverdl/version.py
-drwxrwxrwx   0        0        0        0 2023-05-06 04:38:19.537754 rayserverdl-1.0.1/rayserverdl.egg-info/
--rw-rw-rw-   0        0        0     1026 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 04:38:18.000000 rayserverdl-1.0.1/rayserverdl.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-06 04:38:19.547754 rayserverdl-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1653 2023-05-06 04:28:01.000000 rayserverdl-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:48:12.811535 rayserverdl-1.0.2/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 rayserverdl-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1026 2023-05-06 17:48:12.803535 rayserverdl-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-05-06 04:21:57.000000 rayserverdl-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 17:48:12.657527 rayserverdl-1.0.2/rayserverdl/
+-rw-rw-rw-   0        0        0     3580 2023-05-06 04:18:53.000000 rayserverdl-1.0.2/rayserverdl/d.py
+-rw-rw-rw-   0        0        0       75 2023-05-06 17:45:00.000000 rayserverdl-1.0.2/rayserverdl/version.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:48:12.784534 rayserverdl-1.0.2/rayserverdl.egg-info/
+-rw-rw-rw-   0        0        0     1026 2023-05-06 17:48:07.000000 rayserverdl-1.0.2/rayserverdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-06 17:48:09.000000 rayserverdl-1.0.2/rayserverdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:48:07.000000 rayserverdl-1.0.2/rayserverdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-06 17:48:07.000000 rayserverdl-1.0.2/rayserverdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 17:48:07.000000 rayserverdl-1.0.2/rayserverdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 17:48:07.000000 rayserverdl-1.0.2/rayserverdl.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:48:12.816536 rayserverdl-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1653 2023-05-06 04:28:01.000000 rayserverdl-1.0.2/setup.py
```

### Comparing `rayserverdl-1.0.1/LICENSE` & `rayserverdl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rayserverdl-1.0.1/PKG-INFO` & `rayserverdl-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayserverdl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/rayserverdl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,downloader,stream,files
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rayserverdl-1.0.1/rayserverdl/__init__.py` & `rayserverdl-1.0.2/rayserverdl/d.py`

 * *Files identical despite different names*

### Comparing `rayserverdl-1.0.1/rayserverdl.egg-info/PKG-INFO` & `rayserverdl-1.0.2/rayserverdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayserverdl
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/rayserverdl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,downloader,stream,files
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rayserverdl-1.0.1/setup.py` & `rayserverdl-1.0.2/setup.py`

 * *Files identical despite different names*

