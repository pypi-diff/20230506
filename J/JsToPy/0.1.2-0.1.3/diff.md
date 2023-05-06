# Comparing `tmp/JsToPy-0.1.2.tar.gz` & `tmp/JsToPy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsToPy-0.1.2.tar", last modified: Fri May  5 19:30:37 2023, max compression
+gzip compressed data, was "JsToPy-0.1.3.tar", last modified: Sat May  6 14:34:34 2023, max compression
```

## Comparing `JsToPy-0.1.2.tar` & `JsToPy-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:30:37.132024 JsToPy-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-05 19:30:37.110926 JsToPy-0.1.2/JsToPy/
--rw-rw-rw-   0        0        0      120 2023-05-05 18:14:19.000000 JsToPy-0.1.2/JsToPy/__init__.py
--rw-rw-rw-   0        0        0     1486 2023-05-05 18:11:13.000000 JsToPy-0.1.2/JsToPy/console.py
--rw-rw-rw-   0        0        0      199 2023-05-05 18:28:08.000000 JsToPy-0.1.2/JsToPy/require.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:30:37.124871 JsToPy-0.1.2/JsToPy.egg-info/
--rw-rw-rw-   0        0        0      906 2023-05-05 19:30:37.000000 JsToPy-0.1.2/JsToPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-05-05 19:30:37.000000 JsToPy-0.1.2/JsToPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:30:37.000000 JsToPy-0.1.2/JsToPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 19:30:37.000000 JsToPy-0.1.2/JsToPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      906 2023-05-05 19:30:37.130025 JsToPy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-05-05 18:26:46.000000 JsToPy-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 19:30:37.132024 JsToPy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      690 2023-05-05 19:30:20.000000 JsToPy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:34:34.556286 JsToPy-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-06 14:34:34.547306 JsToPy-0.1.3/JsToPy/
+-rw-rw-rw-   0        0        0      148 2023-05-06 14:33:35.000000 JsToPy-0.1.3/JsToPy/__init__.py
+-rw-rw-rw-   0        0        0     1486 2023-05-05 18:11:13.000000 JsToPy-0.1.3/JsToPy/console.py
+-rw-rw-rw-   0        0        0      199 2023-05-05 18:28:08.000000 JsToPy-0.1.3/JsToPy/require.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:34:34.552292 JsToPy-0.1.3/JsToPy.egg-info/
+-rw-rw-rw-   0        0        0      906 2023-05-06 14:34:34.000000 JsToPy-0.1.3/JsToPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-05-06 14:34:34.000000 JsToPy-0.1.3/JsToPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 14:34:34.000000 JsToPy-0.1.3/JsToPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 14:34:34.000000 JsToPy-0.1.3/JsToPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-05-06 14:34:34.554286 JsToPy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-05-05 18:26:46.000000 JsToPy-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 14:34:34.557279 JsToPy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-05-06 14:34:23.000000 JsToPy-0.1.3/setup.py
```

### Comparing `JsToPy-0.1.2/JsToPy/console.py` & `JsToPy-0.1.3/JsToPy/console.py`

 * *Files identical despite different names*

### Comparing `JsToPy-0.1.2/JsToPy.egg-info/PKG-INFO` & `JsToPy-0.1.3/JsToPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsToPy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library that add to python some js functions.
 Home-page: https://github.com/F1reWs/JsToPy
 Author: Firew
 Author-email: road.of.programming@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `JsToPy-0.1.2/PKG-INFO` & `JsToPy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsToPy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library that add to python some js functions.
 Home-page: https://github.com/F1reWs/JsToPy
 Author: Firew
 Author-email: road.of.programming@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `JsToPy-0.1.2/setup.py` & `JsToPy-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="JsToPy",
-    version="0.1.2",
+    version="0.1.3",
     author="Firew",
     author_email="road.of.programming@gmail.com",
     description=(
         "A library that add to python some js functions."
     ),
     install_requires=None,
     long_description=long_description,
```

