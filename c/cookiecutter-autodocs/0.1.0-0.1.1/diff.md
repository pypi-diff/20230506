# Comparing `tmp/cookiecutter_autodocs-0.1.0.tar.gz` & `tmp/cookiecutter_autodocs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter_autodocs-0.1.0.tar", max compression
+gzip compressed data, was "cookiecutter_autodocs-0.1.1.tar", max compression
```

## Comparing `cookiecutter_autodocs-0.1.0.tar` & `cookiecutter_autodocs-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1063 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/LICENSE
--rw-r--r--   0        0        0     2907 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/__init__.py
--rw-r--r--   0        0        0      779 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/__init__.py
--rw-r--r--   0        0        0      542 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/_async.py
--rw-r--r--   0        0        0      182 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/app.py
--rw-r--r--   0        0        0     4244 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/generate.py
--rw-r--r--   0        0        0     1844 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/gha.py
--rw-r--r--   0        0        0     1403 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/validate.py
--rw-r--r--   0        0        0        0 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/lib/__init__.py
--rw-r--r--   0        0        0     2015 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/lib/files.py
--rw-r--r--   0        0        0      239 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/lib/typing.py
--rw-r--r--   0        0        0        0 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/py.typed
--rw-r--r--   0        0        0      161 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/schemas/__init__.py
--rw-r--r--   0        0        0      502 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/schemas/_base.py
--rw-r--r--   0        0        0     5573 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/schemas/description.py
--rw-r--r--   0        0        0     1432 2023-05-06 19:54:34.636563 cookiecutter_autodocs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 cookiecutter_autodocs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-06 20:24:39.952691 cookiecutter_autodocs-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2907 2023-05-06 20:24:39.952691 cookiecutter_autodocs-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/__init__.py
+-rw-r--r--   0        0        0      779 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/__init__.py
+-rw-r--r--   0        0        0      542 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/_async.py
+-rw-r--r--   0        0        0      182 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/app.py
+-rw-r--r--   0        0        0     4244 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/generate.py
+-rw-r--r--   0        0        0     1844 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/gha.py
+-rw-r--r--   0        0        0     1403 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/lib/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/lib/files.py
+-rw-r--r--   0        0        0      239 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/lib/typing.py
+-rw-r--r--   0        0        0        0 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/py.typed
+-rw-r--r--   0        0        0      161 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/schemas/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/schemas/_base.py
+-rw-r--r--   0        0        0     5573 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/schemas/description.py
+-rw-r--r--   0        0        0     1432 2023-05-06 20:24:39.956691 cookiecutter_autodocs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 cookiecutter_autodocs-0.1.1/PKG-INFO
```

### Comparing `cookiecutter_autodocs-0.1.0/LICENSE` & `cookiecutter_autodocs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/README.md` & `cookiecutter_autodocs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/__init__.py` & `cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/_async.py` & `cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/_async.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/generate.py` & `cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/generate.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/gha.py` & `cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/gha.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/validate.py` & `cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/cli/validate.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/lib/files.py` & `cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/lib/files.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/schemas/description.py` & `cookiecutter_autodocs-0.1.1/cookiecutter_autodocs/schemas/description.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.1.0/pyproject.toml` & `cookiecutter_autodocs-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cookiecutter-autodocs"
-version = "0.1.0"
+version = "0.1.1"
 description = "Generate docs from your cookiecutter template"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cookiecutter_autodocs"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cookiecutter_autodocs-0.1.0/PKG-INFO` & `cookiecutter_autodocs-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-autodocs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate docs from your cookiecutter template
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

