# Comparing `tmp/mlgenotype-0.1.5.tar.gz` & `tmp/mlgenotype-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlgenotype-0.1.5.tar", last modified: Thu May  4 19:20:13 2023, max compression
+gzip compressed data, was "mlgenotype-0.1.6.tar", last modified: Sat May  6 00:46:19 2023, max compression
```

## Comparing `mlgenotype-0.1.5.tar` & `mlgenotype-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-04 19:20:13.535176 mlgenotype-0.1.5/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      995 2023-05-03 18:24:26.000000 mlgenotype-0.1.5/LICENSE.md
--rw-rw-r--   0 nhansen   (6175) zoo        (101)       30 2023-05-03 18:40:57.000000 mlgenotype-0.1.5/MANIFEST.in
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-04 19:20:13.537136 mlgenotype-0.1.5/PKG-INFO
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      524 2023-05-03 22:37:53.000000 mlgenotype-0.1.5/README.md
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      863 2023-05-04 03:24:23.000000 mlgenotype-0.1.5/pyproject.toml
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      719 2023-05-04 19:20:13.543924 mlgenotype-0.1.5/setup.cfg
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     8803 2023-05-04 01:38:57.000000 mlgenotype-0.1.5/setup.py
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-04 19:20:13.364417 mlgenotype-0.1.5/src/
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-04 19:20:13.468619 mlgenotype-0.1.5/src/mlgenotype/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)        0 2023-05-03 19:09:36.000000 mlgenotype-0.1.5/src/mlgenotype/__init__.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)       89 2023-05-03 22:40:34.000000 mlgenotype-0.1.5/src/mlgenotype/__main__.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     4888 2023-05-04 01:37:25.000000 mlgenotype-0.1.5/src/mlgenotype/figure1calcs.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     3207 2023-05-03 18:24:26.000000 mlgenotype-0.1.5/src/mlgenotype/rfgenotype.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     2616 2023-05-04 01:20:03.000000 mlgenotype-0.1.5/src/mlgenotype/rfmodelpredict.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     3713 2023-05-03 18:24:26.000000 mlgenotype-0.1.5/src/mlgenotype/rfmodeltrain.py
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     3792 2023-05-03 22:49:34.000000 mlgenotype-0.1.5/src/mlgenotype/rftrainpredict.py
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-04 19:20:13.519153 mlgenotype-0.1.5/src/mlgenotype.egg-info/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-04 19:20:13.000000 mlgenotype-0.1.5/src/mlgenotype.egg-info/PKG-INFO
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      527 2023-05-04 19:20:13.000000 mlgenotype-0.1.5/src/mlgenotype.egg-info/SOURCES.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)        1 2023-05-04 19:20:13.000000 mlgenotype-0.1.5/src/mlgenotype.egg-info/dependency_links.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      202 2023-05-04 19:20:13.000000 mlgenotype-0.1.5/src/mlgenotype.egg-info/entry_points.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      105 2023-05-04 19:20:13.000000 mlgenotype-0.1.5/src/mlgenotype.egg-info/requires.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)       11 2023-05-04 19:20:13.000000 mlgenotype-0.1.5/src/mlgenotype.egg-info/top_level.txt
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-04 19:20:13.528096 mlgenotype-0.1.5/tests/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      131 2023-05-04 02:54:47.000000 mlgenotype-0.1.5/tests/test_calls.py
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:19.031657 mlgenotype-0.1.6/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      995 2023-05-03 18:24:26.000000 mlgenotype-0.1.6/LICENSE.md
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       35 2023-05-05 19:32:32.000000 mlgenotype-0.1.6/MANIFEST.in
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 00:46:19.033861 mlgenotype-0.1.6/PKG-INFO
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      524 2023-05-03 22:37:53.000000 mlgenotype-0.1.6/README.md
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      990 2023-05-06 00:46:05.000000 mlgenotype-0.1.6/pyproject.toml
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      693 2023-05-06 00:46:19.040300 mlgenotype-0.1.6/setup.cfg
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     8803 2023-05-04 01:38:57.000000 mlgenotype-0.1.6/setup.py
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:18.897711 mlgenotype-0.1.6/src/
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:18.900908 mlgenotype-0.1.6/src/mlgenotype/
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:18.998867 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/PKG-INFO
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      382 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/SOURCES.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)        1 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/dependency_links.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      202 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/entry_points.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      106 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/requires.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)        5 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/top_level.txt
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:19.007072 mlgenotype-0.1.6/tests/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      188 2023-05-05 21:37:26.000000 mlgenotype-0.1.6/tests/test_calls.py
```

### Comparing `mlgenotype-0.1.5/LICENSE.md` & `mlgenotype-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.5/PKG-INFO` & `mlgenotype-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlgenotype
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package with utilities for training classifiers to recognize SVs in short read datasets
 Home-page: https://github.com/nhansen/mlgenotype
 Author: Nancy F Hansen, Gracelyn Hill, Jennifer Lin
 Author-email: "Nancy F. Hansen" <nhansen@mail.nih.gov>
 Project-URL: Homepage, https://github.com/nhansen/mlgenotype
 Project-URL: Bug Tracker, https://github.com/nhansen/mlgenotype/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlgenotype-0.1.5/README.md` & `mlgenotype-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.5/pyproject.toml` & `mlgenotype-0.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools >= 48", "pytest"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlgenotype"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Nancy F. Hansen", email="nhansen@mail.nih.gov" },
 ]
 description = "A package with utilities for training classifiers to recognize SVs in short read datasets"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'pandas >= 1.0',
-  'scikit-learn >= 0.20',
+  'scikit-learn == 1.0.2',
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
@@ -30,7 +30,12 @@
     "pylint ~=2.14.0",
     "toml ~=0.10.2",
     "yapf ~=0.32.0",
 ]
 test = [
     "pytest-cov ~=3.0.0",
 ]
+[tool.setuptools.packages.find]
+where = ["src/mlgenotype"]
+
+[tool.setuptools.exclude-package-data]
+mypkg = [".gitattributes"]
```

### Comparing `mlgenotype-0.1.5/setup.cfg` & `mlgenotype-0.1.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 name = mlgenotype
 description = a Python library for calling genotypes from short read sequence features
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/nhansen/mlgenotype
 author = Nancy F Hansen, Gracelyn Hill, Jennifer Lin
 author_email = nhansen@mail.nih.gov,
-license_file = LICENSE.md
 project_urls = 
 	Documentation = https://mlgenotype.readthedocs.io
 	Source = https://github.com/nhansen/mlgenotype
 	Tracker = https://github.com/nhansen/mlgenotype/issues
 
 [options]
 python_requires = >=3.7
```

### Comparing `mlgenotype-0.1.5/setup.py` & `mlgenotype-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.5/src/mlgenotype.egg-info/PKG-INFO` & `mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlgenotype
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package with utilities for training classifiers to recognize SVs in short read datasets
 Home-page: https://github.com/nhansen/mlgenotype
 Author: Nancy F Hansen, Gracelyn Hill, Jennifer Lin
 Author-email: "Nancy F. Hansen" <nhansen@mail.nih.gov>
 Project-URL: Homepage, https://github.com/nhansen/mlgenotype
 Project-URL: Bug Tracker, https://github.com/nhansen/mlgenotype/issues
 Classifier: Programming Language :: Python :: 3
```

