# Comparing `tmp/edge_distance_aabb-1.0.tar.gz` & `tmp/edge_distance_aabb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_distance_aabb-1.0.tar", last modified: Fri May  5 22:52:13 2023, max compression
+gzip compressed data, was "edge_distance_aabb-1.0.1.tar", last modified: Sat May  6 03:19:03 2023, max compression
```

## Comparing `edge_distance_aabb-1.0.tar` & `edge_distance_aabb-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yotam      (501) staff       (20)        0 2023-05-05 22:52:13.364842 edge_distance_aabb-1.0/
--rw-r--r--   0 yotam      (501) staff       (20)     7049 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0/LICENSE
--rw-r--r--   0 yotam      (501) staff       (20)       60 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0/MANIFEST.in
--rw-r--r--   0 yotam      (501) staff       (20)     2758 2023-05-05 22:52:13.364679 edge_distance_aabb-1.0/PKG-INFO
--rw-r--r--   0 yotam      (501) staff       (20)     2151 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0/README.md
--rw-r--r--   0 yotam      (501) staff       (20)   891663 2023-05-05 22:52:13.000000 edge_distance_aabb-1.0/edge_distance_aabb.cpp
-drwxr-xr-x   0 yotam      (501) staff       (20)        0 2023-05-05 22:52:13.364468 edge_distance_aabb-1.0/edge_distance_aabb.egg-info/
--rw-r--r--   0 yotam      (501) staff       (20)     2758 2023-05-05 22:52:13.000000 edge_distance_aabb-1.0/edge_distance_aabb.egg-info/PKG-INFO
--rw-r--r--   0 yotam      (501) staff       (20)      288 2023-05-05 22:52:13.000000 edge_distance_aabb-1.0/edge_distance_aabb.egg-info/SOURCES.txt
--rw-r--r--   0 yotam      (501) staff       (20)        1 2023-05-05 22:52:13.000000 edge_distance_aabb-1.0/edge_distance_aabb.egg-info/dependency_links.txt
--rw-r--r--   0 yotam      (501) staff       (20)       19 2023-05-05 22:52:13.000000 edge_distance_aabb-1.0/edge_distance_aabb.egg-info/top_level.txt
--rw-r--r--   0 yotam      (501) staff       (20)    14723 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0/edge_distance_aabb.h
--rw-r--r--   0 yotam      (501) staff       (20)    10453 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0/edge_distance_aabb.pyx
--rw-r--r--   0 yotam      (501) staff       (20)      720 2023-05-05 21:39:27.000000 edge_distance_aabb-1.0/pyproject.toml
--rw-r--r--   0 yotam      (501) staff       (20)       38 2023-05-05 22:52:13.364974 edge_distance_aabb-1.0/setup.cfg
--rw-r--r--   0 yotam      (501) staff       (20)      399 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0/setup.py
+drwxr-xr-x   0 yotam      (501) staff       (20)        0 2023-05-06 03:19:03.898487 edge_distance_aabb-1.0.1/
+-rw-r--r--   0 yotam      (501) staff       (20)     7049 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0.1/LICENSE
+-rw-r--r--   0 yotam      (501) staff       (20)       60 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0.1/MANIFEST.in
+-rw-r--r--   0 yotam      (501) staff       (20)     2882 2023-05-06 03:19:03.898320 edge_distance_aabb-1.0.1/PKG-INFO
+-rw-r--r--   0 yotam      (501) staff       (20)     2265 2023-05-06 03:16:09.000000 edge_distance_aabb-1.0.1/README.md
+-rw-r--r--   0 yotam      (501) staff       (20)   891663 2023-05-05 22:52:13.000000 edge_distance_aabb-1.0.1/edge_distance_aabb.cpp
+drwxr-xr-x   0 yotam      (501) staff       (20)        0 2023-05-06 03:19:03.898079 edge_distance_aabb-1.0.1/edge_distance_aabb.egg-info/
+-rw-r--r--   0 yotam      (501) staff       (20)     2882 2023-05-06 03:19:03.000000 edge_distance_aabb-1.0.1/edge_distance_aabb.egg-info/PKG-INFO
+-rw-r--r--   0 yotam      (501) staff       (20)      288 2023-05-06 03:19:03.000000 edge_distance_aabb-1.0.1/edge_distance_aabb.egg-info/SOURCES.txt
+-rw-r--r--   0 yotam      (501) staff       (20)        1 2023-05-06 03:19:03.000000 edge_distance_aabb-1.0.1/edge_distance_aabb.egg-info/dependency_links.txt
+-rw-r--r--   0 yotam      (501) staff       (20)       19 2023-05-06 03:19:03.000000 edge_distance_aabb-1.0.1/edge_distance_aabb.egg-info/top_level.txt
+-rw-r--r--   0 yotam      (501) staff       (20)    14723 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0.1/edge_distance_aabb.h
+-rw-r--r--   0 yotam      (501) staff       (20)    10453 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0.1/edge_distance_aabb.pyx
+-rw-r--r--   0 yotam      (501) staff       (20)      730 2023-05-06 03:16:23.000000 edge_distance_aabb-1.0.1/pyproject.toml
+-rw-r--r--   0 yotam      (501) staff       (20)       38 2023-05-06 03:19:03.898533 edge_distance_aabb-1.0.1/setup.cfg
+-rw-r--r--   0 yotam      (501) staff       (20)      399 2023-05-05 21:33:34.000000 edge_distance_aabb-1.0.1/setup.py
```

### Comparing `edge_distance_aabb-1.0/LICENSE` & `edge_distance_aabb-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_distance_aabb-1.0/PKG-INFO` & `edge_distance_aabb-1.0.1/edge_distance_aabb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: edge_distance_aabb
-Version: 1.0
+Name: edge-distance-aabb
+Version: 1.0.1
 Summary: Relatively efficient distance and closest point from a set of points to a set of line segments.
 Author-email: Yotam Gingold <yotam@yotamgingold.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/yig/edge_distance_aabb
+Project-URL: Bug Tracker, https://github.com/yig/edge_distance_aabb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -63,16 +63,25 @@
 
 1. From PyPI:
 
 ```
 pip install edge_distance_aabb
 ```
 
-2. By copying `edge_distance_aabb.pyx` and `edge_distance_aabb.h` into your directory and running `cythonize --build edge_distance_aabb.pyx`.
+2. From GitHub:
+
+```
+pip install git+https://github.com/yig/edge_distance_aabb.git
+```
+
+3. By copying `edge_distance_aabb.pyx` and `edge_distance_aabb.h` into your directory and running `cythonize --build edge_distance_aabb.pyx`.
 
 ## Dependencies
 
 `numpy` and `Cython`
 
 ## Distribution
 
-`python3 -m build`
+```
+python3 -m build
+twine upload dist/*
+```
```

### Comparing `edge_distance_aabb-1.0/README.md` & `edge_distance_aabb-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,25 @@
 
 1. From PyPI:
 
 ```
 pip install edge_distance_aabb
 ```
 
-2. By copying `edge_distance_aabb.pyx` and `edge_distance_aabb.h` into your directory and running `cythonize --build edge_distance_aabb.pyx`.
+2. From GitHub:
+
+```
+pip install git+https://github.com/yig/edge_distance_aabb.git
+```
+
+3. By copying `edge_distance_aabb.pyx` and `edge_distance_aabb.h` into your directory and running `cythonize --build edge_distance_aabb.pyx`.
 
 ## Dependencies
 
 `numpy` and `Cython`
 
 ## Distribution
 
-`python3 -m build`
+```
+python3 -m build
+twine upload dist/*
+```
```

### Comparing `edge_distance_aabb-1.0/edge_distance_aabb.cpp` & `edge_distance_aabb-1.0.1/edge_distance_aabb.cpp`

 * *Files identical despite different names*

### Comparing `edge_distance_aabb-1.0/edge_distance_aabb.egg-info/PKG-INFO` & `edge_distance_aabb-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: edge-distance-aabb
-Version: 1.0
+Name: edge_distance_aabb
+Version: 1.0.1
 Summary: Relatively efficient distance and closest point from a set of points to a set of line segments.
 Author-email: Yotam Gingold <yotam@yotamgingold.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/yig/edge_distance_aabb
+Project-URL: Bug Tracker, https://github.com/yig/edge_distance_aabb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -63,16 +63,25 @@
 
 1. From PyPI:
 
 ```
 pip install edge_distance_aabb
 ```
 
-2. By copying `edge_distance_aabb.pyx` and `edge_distance_aabb.h` into your directory and running `cythonize --build edge_distance_aabb.pyx`.
+2. From GitHub:
+
+```
+pip install git+https://github.com/yig/edge_distance_aabb.git
+```
+
+3. By copying `edge_distance_aabb.pyx` and `edge_distance_aabb.h` into your directory and running `cythonize --build edge_distance_aabb.pyx`.
 
 ## Dependencies
 
 `numpy` and `Cython`
 
 ## Distribution
 
-`python3 -m build`
+```
+python3 -m build
+twine upload dist/*
+```
```

### Comparing `edge_distance_aabb-1.0/edge_distance_aabb.h` & `edge_distance_aabb-1.0.1/edge_distance_aabb.h`

 * *Files identical despite different names*

### Comparing `edge_distance_aabb-1.0/edge_distance_aabb.pyx` & `edge_distance_aabb-1.0.1/edge_distance_aabb.pyx`

 * *Files identical despite different names*

### Comparing `edge_distance_aabb-1.0/pyproject.toml` & `edge_distance_aabb-1.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel", "numpy>=1.19.0", "Cython>=0.29.21"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edge_distance_aabb"
-version = "1.0"
+version = "1.0.1"
 authors = [
   { name="Yotam Gingold", email="yotam@yotamgingold.com" },
 ]
 description = "Relatively efficient distance and closest point from a set of points to a set of line segments."
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Homepage" = "https://github.com/yig/edge_distance_aabb"
+"Bug Tracker" = "https://github.com/yig/edge_distance_aabb/issues"
```

