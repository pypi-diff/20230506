# Comparing `tmp/cookiecutter_autodocs-0.0.4.tar.gz` & `tmp/cookiecutter_autodocs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter_autodocs-0.0.4.tar", max compression
+gzip compressed data, was "cookiecutter_autodocs-0.1.0.tar", max compression
```

## Comparing `cookiecutter_autodocs-0.0.4.tar` & `cookiecutter_autodocs-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1063 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/LICENSE
--rw-r--r--   0        0        0     2907 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/__init__.py
--rw-r--r--   0        0        0      779 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/__init__.py
--rw-r--r--   0        0        0      542 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/_async.py
--rw-r--r--   0        0        0      182 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/app.py
--rw-r--r--   0        0        0     4244 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/generate.py
--rw-r--r--   0        0        0     1844 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/gha.py
--rw-r--r--   0        0        0     1403 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/validate.py
--rw-r--r--   0        0        0        0 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/lib/__init__.py
--rw-r--r--   0        0        0     2015 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/lib/files.py
--rw-r--r--   0        0        0      239 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/lib/typing.py
--rw-r--r--   0        0        0        0 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/py.typed
--rw-r--r--   0        0        0      161 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/schemas/__init__.py
--rw-r--r--   0        0        0      502 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/schemas/_base.py
--rw-r--r--   0        0        0     5573 2023-04-23 04:11:03.060036 cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/schemas/description.py
--rw-r--r--   0        0        0     1417 2023-04-23 04:11:03.064036 cookiecutter_autodocs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 cookiecutter_autodocs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2907 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/__init__.py
+-rw-r--r--   0        0        0      779 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/__init__.py
+-rw-r--r--   0        0        0      542 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/_async.py
+-rw-r--r--   0        0        0      182 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/app.py
+-rw-r--r--   0        0        0     4244 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/generate.py
+-rw-r--r--   0        0        0     1844 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/gha.py
+-rw-r--r--   0        0        0     1403 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/lib/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/lib/files.py
+-rw-r--r--   0        0        0      239 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/lib/typing.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/py.typed
+-rw-r--r--   0        0        0      161 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/schemas/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/schemas/_base.py
+-rw-r--r--   0        0        0     5573 2023-05-06 19:54:34.632563 cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/schemas/description.py
+-rw-r--r--   0        0        0     1432 2023-05-06 19:54:34.636563 cookiecutter_autodocs-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 cookiecutter_autodocs-0.1.0/PKG-INFO
```

### Comparing `cookiecutter_autodocs-0.0.4/LICENSE` & `cookiecutter_autodocs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/README.md` & `cookiecutter_autodocs-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/__init__.py` & `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/_async.py` & `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/_async.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/generate.py` & `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/generate.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/gha.py` & `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/gha.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/cli/validate.py` & `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/cli/validate.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/lib/files.py` & `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/lib/files.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/cookiecutter_autodocs/schemas/description.py` & `cookiecutter_autodocs-0.1.0/cookiecutter_autodocs/schemas/description.py`

 * *Files identical despite different names*

### Comparing `cookiecutter_autodocs-0.0.4/pyproject.toml` & `cookiecutter_autodocs-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "cookiecutter-autodocs"
-version = "0.0.4"
+version = "0.1.0"
 description = "Generate docs from your cookiecutter template"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cookiecutter_autodocs"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-typer = "^0.7.0"
+typer = ">=0.7,<0.10"
 aiofiles = "^23.1.0"
 pydantic = "^1.10.7"
 toml = "^0.10.2"
 py-markdown-table = "^0.3.3"
 rich = "^13.3.4"
 
 [tool.poetry.scripts]
@@ -24,15 +24,15 @@
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.21.0"
 bandit = "^1.7.5"
 mypy = "^1.1.1"
 pre-commit-hooks = "^4.4.0"
 reorder-python-imports = "^3.9.0"
 pytest-xdist = "^3.2.1"
-ruff = "^0.0.261"
+ruff = ">=0.0.261,<0.0.266"
 pre-commit = "^3.2.1"
 pyupgrade = "^3.3.1"
 types-aiofiles = "^23.1.0.1"
 pytest-subtests = "^0.10.0"
 types-toml = "^0.10.8.6"
 pyflakes = "^3.0.1"
```

### Comparing `cookiecutter_autodocs-0.0.4/PKG-INFO` & `cookiecutter_autodocs-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-autodocs
-Version: 0.0.4
+Version: 0.1.0
 Summary: Generate docs from your cookiecutter template
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: py-markdown-table (>=0.3.3,<0.4.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.7,<0.10)
 Description-Content-Type: text/markdown
 
 # cookiecutter-autodocs
 
 Generate docs for a cookiecutter template's inputs. Pre-commit hook and github-action
 
 ## Why?
```

