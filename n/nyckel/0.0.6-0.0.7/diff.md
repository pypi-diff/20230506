# Comparing `tmp/nyckel-0.0.6.tar.gz` & `tmp/nyckel-0.0.7.tar.gz`

## Comparing `nyckel-0.0.6.tar` & `nyckel-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nyckel-0.0.6/requirements.txt
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 nyckel-0.0.6/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 nyckel-0.0.6/.github/workflows/test-all.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 nyckel-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/__about__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/__init__.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/auth.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/config.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/request_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/functions/text_classification_function.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 nyckel-0.0.6/tests/test_text_classification_function.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.6/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.6/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nyckel-0.0.6/README.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nyckel-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 nyckel-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nyckel-0.0.7/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nyckel-0.0.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nyckel-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 nyckel-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/auth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/config.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/functions/text_classification_function.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 nyckel-0.0.7/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.7/LICENSE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nyckel-0.0.7/README.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nyckel-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nyckel-0.0.7/PKG-INFO
```

### Comparing `nyckel-0.0.6/.github/workflows/deploy.yml` & `nyckel-0.0.7/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Test and deploy to PYPI
+name: build
 
 on: 
   push:
     branches:
       - master
 
 jobs:
```

### Comparing `nyckel-0.0.6/.github/workflows/test-all.yml` & `nyckel-0.0.7/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Test all python versions
+name: test
 
 on: [push]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
```

### Comparing `nyckel-0.0.6/src/nyckel/auth.py` & `nyckel-0.0.7/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.6/src/nyckel/request_utils.py` & `nyckel-0.0.7/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.6/src/nyckel/functions/text_classification_function.py` & `nyckel-0.0.7/src/nyckel/functions/text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.6/tests/test_text_classification_function.py` & `nyckel-0.0.7/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.6/.gitignore` & `nyckel-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.6/LICENSE` & `nyckel-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.6/pyproject.toml` & `nyckel-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 
 [project]
 name = "nyckel"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Oscar Beijbom", email="oscar@nyckel.com" },
 ]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nyckel-0.0.6/PKG-INFO` & `nyckel-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyckel
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,10 @@
 Requires-Dist: requests~=2.30.0
 Requires-Dist: tqdm~=4.65.0
 Description-Content-Type: text/markdown
 
 # Nyckel
 
 Python package for www.nyckel.com
+
+![build](https://github.com/NyckelAI/python-sdk/actions/workflows/build.yml/badge.svg)
+![test](https://github.com/NyckelAI/python-sdk/actions/workflows/test.yml/badge.svg)
```

