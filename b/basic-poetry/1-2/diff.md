# Comparing `tmp/basic_poetry-1.tar.gz` & `tmp/basic_poetry-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_poetry-1.tar", max compression
+gzip compressed data, was "basic_poetry-2.tar", max compression
```

## Comparing `basic_poetry-1.tar` & `basic_poetry-2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-05 13:07:54.871909 basic_poetry-1/README.md
--rw-r--r--   0        0        0      621 2023-05-06 12:15:17.523675 basic_poetry-1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-05 13:07:54.871909 basic_poetry-1/sandbox/__init__.py
--rw-r--r--   0        0        0      105 2023-05-06 10:48:11.139817 basic_poetry-1/sandbox/sandbox.py
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 basic_poetry-1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-05 13:07:54.871909 basic_poetry-2/README.md
+-rw-r--r--   0        0        0      646 2023-05-06 12:25:01.323659 basic_poetry-2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-05 13:07:54.871909 basic_poetry-2/sandbox/__init__.py
+-rw-r--r--   0        0        0      105 2023-05-06 10:48:11.139817 basic_poetry-2/sandbox/sandbox.py
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 basic_poetry-2/PKG-INFO
```

### Comparing `basic_poetry-1/pyproject.toml` & `basic_poetry-2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basic_poetry"
-version = "1"
+version = "2"
 description = "basic dependencies for poetry"
 authors = ["BloodSpy <hahaclassik@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sandbox"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -15,11 +15,12 @@
 pep8-naming = "^0.13.3"
 flake8-commas = "^2.1.0"
 flake8-variables-names = "^0.0.5"
 flake8-import-order = "^0.18.2"
 flake8-comprehensions = "^3.12.0"
 flake8-quotes = "^3.3.2"
 flake8-docstrings = "^1.7.0"
+flake8-alfred = "^1.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `basic_poetry-1/PKG-INFO` & `basic_poetry-2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: basic-poetry
-Version: 1
+Version: 2
 Summary: basic dependencies for poetry
 Author: BloodSpy
 Author-email: hahaclassik@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
+Requires-Dist: flake8-alfred (>=1.1.1,<2.0.0)
 Requires-Dist: flake8-bugbear (>=23.3.23,<24.0.0)
 Requires-Dist: flake8-builtins (>=2.1.0,<3.0.0)
 Requires-Dist: flake8-commas (>=2.1.0,<3.0.0)
 Requires-Dist: flake8-comprehensions (>=3.12.0,<4.0.0)
 Requires-Dist: flake8-docstrings (>=1.7.0,<2.0.0)
 Requires-Dist: flake8-import-order (>=0.18.2,<0.19.0)
 Requires-Dist: flake8-quotes (>=3.3.2,<4.0.0)
```

