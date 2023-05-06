# Comparing `tmp/mlgenotype-0.1.6.tar.gz` & `tmp/mlgenotype-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlgenotype-0.1.6.tar", last modified: Sat May  6 00:46:19 2023, max compression
+gzip compressed data, was "/cluster/ifs/projects/AlphaThal/github/mlgenotype/dist/.tmp-4ifvcbq1/mlgenotype-0.1.7.tar", last modified: Sat May  6 01:49:34 2023, max compression
```

## Comparing `mlgenotype-0.1.6.tar` & `mlgenotype-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:19.031657 mlgenotype-0.1.6/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      995 2023-05-03 18:24:26.000000 mlgenotype-0.1.6/LICENSE.md
--rw-rw-r--   0 nhansen   (6175) zoo        (101)       35 2023-05-05 19:32:32.000000 mlgenotype-0.1.6/MANIFEST.in
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 00:46:19.033861 mlgenotype-0.1.6/PKG-INFO
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      524 2023-05-03 22:37:53.000000 mlgenotype-0.1.6/README.md
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      990 2023-05-06 00:46:05.000000 mlgenotype-0.1.6/pyproject.toml
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      693 2023-05-06 00:46:19.040300 mlgenotype-0.1.6/setup.cfg
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     8803 2023-05-04 01:38:57.000000 mlgenotype-0.1.6/setup.py
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:18.897711 mlgenotype-0.1.6/src/
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:18.900908 mlgenotype-0.1.6/src/mlgenotype/
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:18.998867 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/PKG-INFO
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      382 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/SOURCES.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)        1 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/dependency_links.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      202 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/entry_points.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      106 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/requires.txt
--rw-rw-r--   0 nhansen   (6175) zoo        (101)        5 2023-05-06 00:46:18.000000 mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/top_level.txt
-drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 00:46:19.007072 mlgenotype-0.1.6/tests/
--rw-rw-r--   0 nhansen   (6175) zoo        (101)      188 2023-05-05 21:37:26.000000 mlgenotype-0.1.6/tests/test_calls.py
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      995 2023-05-03 18:24:26.000000 mlgenotype-0.1.7/LICENSE.md
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       35 2023-05-05 19:32:32.000000 mlgenotype-0.1.7/MANIFEST.in
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/PKG-INFO
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      524 2023-05-03 22:37:53.000000 mlgenotype-0.1.7/README.md
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      864 2023-05-06 01:42:57.000000 mlgenotype-0.1.7/pyproject.toml
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      693 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/setup.cfg
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     8803 2023-05-04 01:38:57.000000 mlgenotype-0.1.7/setup.py
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/mlgenotype/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       92 2023-05-05 21:28:24.000000 mlgenotype-0.1.7/src/mlgenotype/__init__.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       89 2023-05-03 22:40:34.000000 mlgenotype-0.1.7/src/mlgenotype/__main__.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     4888 2023-05-04 01:37:25.000000 mlgenotype-0.1.7/src/mlgenotype/figure1calcs.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     3207 2023-05-03 18:24:26.000000 mlgenotype-0.1.7/src/mlgenotype/rfgenotype.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     2752 2023-05-05 20:52:52.000000 mlgenotype-0.1.7/src/mlgenotype/rfmodelpredict.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     3713 2023-05-03 18:24:26.000000 mlgenotype-0.1.7/src/mlgenotype/rfmodeltrain.py
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     3792 2023-05-03 22:49:34.000000 mlgenotype-0.1.7/src/mlgenotype/rftrainpredict.py
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/mlgenotype.egg-info/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)     1241 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/mlgenotype.egg-info/PKG-INFO
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      527 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/mlgenotype.egg-info/SOURCES.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)        1 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/mlgenotype.egg-info/dependency_links.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      202 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/mlgenotype.egg-info/entry_points.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      106 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/mlgenotype.egg-info/requires.txt
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)       11 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/src/mlgenotype.egg-info/top_level.txt
+drwxrwsr-x   0 nhansen   (6175) zoo        (101)        0 2023-05-06 01:49:34.000000 mlgenotype-0.1.7/tests/
+-rw-rw-r--   0 nhansen   (6175) zoo        (101)      188 2023-05-05 21:37:26.000000 mlgenotype-0.1.7/tests/test_calls.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mlgenotype-0.1.6/LICENSE.md` & `mlgenotype-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.6/PKG-INFO` & `mlgenotype-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlgenotype
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package with utilities for training classifiers to recognize SVs in short read datasets
 Home-page: https://github.com/nhansen/mlgenotype
 Author: Nancy F Hansen, Gracelyn Hill, Jennifer Lin
 Author-email: "Nancy F. Hansen" <nhansen@mail.nih.gov>
 Project-URL: Homepage, https://github.com/nhansen/mlgenotype
 Project-URL: Bug Tracker, https://github.com/nhansen/mlgenotype/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlgenotype-0.1.6/README.md` & `mlgenotype-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.6/pyproject.toml` & `mlgenotype-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 48", "pytest"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlgenotype"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Nancy F. Hansen", email="nhansen@mail.nih.gov" },
 ]
 description = "A package with utilities for training classifiers to recognize SVs in short read datasets"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -30,12 +30,7 @@
     "pylint ~=2.14.0",
     "toml ~=0.10.2",
     "yapf ~=0.32.0",
 ]
 test = [
     "pytest-cov ~=3.0.0",
 ]
-[tool.setuptools.packages.find]
-where = ["src/mlgenotype"]
-
-[tool.setuptools.exclude-package-data]
-mypkg = [".gitattributes"]
```

### Comparing `mlgenotype-0.1.6/setup.cfg` & `mlgenotype-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.6/setup.py` & `mlgenotype-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `mlgenotype-0.1.6/src/mlgenotype/mlgenotype.egg-info/PKG-INFO` & `mlgenotype-0.1.7/src/mlgenotype.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlgenotype
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package with utilities for training classifiers to recognize SVs in short read datasets
 Home-page: https://github.com/nhansen/mlgenotype
 Author: Nancy F Hansen, Gracelyn Hill, Jennifer Lin
 Author-email: "Nancy F. Hansen" <nhansen@mail.nih.gov>
 Project-URL: Homepage, https://github.com/nhansen/mlgenotype
 Project-URL: Bug Tracker, https://github.com/nhansen/mlgenotype/issues
 Classifier: Programming Language :: Python :: 3
```

