# Comparing `tmp/flake8_2020-1.7.0.tar.gz` & `tmp/flake8_2020-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_2020-1.7.0.tar", last modified: Mon Aug  1 16:35:59 2022, max compression
+gzip compressed data, was "flake8_2020-1.8.0.tar", last modified: Sat May  6 21:06:58 2023, max compression
```

## Comparing `flake8_2020-1.7.0.tar` & `flake8_2020-1.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-08-01 16:35:59.852547 flake8_2020-1.7.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-08-01 16:35:53.000000 flake8_2020-1.7.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4701 2022-08-01 16:35:59.852547 flake8_2020-1.7.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3905 2022-08-01 16:35:53.000000 flake8_2020-1.7.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-08-01 16:35:59.848547 flake8_2020-1.7.0/flake8_2020.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4701 2022-08-01 16:35:59.000000 flake8_2020-1.7.0/flake8_2020.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      263 2022-08-01 16:35:59.000000 flake8_2020-1.7.0/flake8_2020.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-08-01 16:35:59.000000 flake8_2020-1.7.0/flake8_2020.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       44 2022-08-01 16:35:59.000000 flake8_2020-1.7.0/flake8_2020.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2022-08-01 16:35:59.000000 flake8_2020-1.7.0/flake8_2020.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2022-08-01 16:35:59.000000 flake8_2020-1.7.0/flake8_2020.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6404 2022-08-01 16:35:53.000000 flake8_2020-1.7.0/flake8_2020.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1284 2022-08-01 16:35:59.852547 flake8_2020-1.7.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-08-01 16:35:53.000000 flake8_2020-1.7.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:06:58.591488 flake8_2020-1.8.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-06 20:25:33.000000 flake8_2020-1.8.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4262 2023-05-06 21:06:58.591488 flake8_2020-1.8.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3687 2023-05-06 20:25:33.000000 flake8_2020-1.8.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:06:58.591488 flake8_2020-1.8.0/flake8_2020.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4262 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      263 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       44 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6585 2023-05-06 21:06:58.000000 flake8_2020-1.8.0/flake8_2020.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1099 2023-05-06 21:06:58.591488 flake8_2020-1.8.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-06 20:25:33.000000 flake8_2020-1.8.0/setup.py
```

### Comparing `flake8_2020-1.7.0/LICENSE` & `flake8_2020-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_2020-1.7.0/PKG-INFO` & `flake8_2020-1.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: flake8_2020
-Version: 1.7.0
+Version: 1.8.0
 Summary: flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 Home-page: https://github.com/asottile/flake8-2020
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.flake8-2020?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=27&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/27/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=27&branchName=main)
+[![build status](https://github.com/asottile/flake8-2020/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/flake8-2020/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/flake8-2020/main.svg)](https://results.pre-commit.ci/latest/github/asottile/flake8-2020/main)
 
 flake8-2020
 ===========
 
 flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 
@@ -33,15 +27,17 @@
 
 you might also find an early build of [python3.10] useful
 
 [python3.10]: https://github.com/asottile/python3.10
 
 ## installation
 
-`pip install flake8-2020`
+```bash
+pip install flake8-2020
+```
 
 ## flake8 codes
 
 | Code   | Description                                            |
 |--------|--------------------------------------------------------|
 | YTT101 | `sys.version[:3]` referenced (python3.10)              |
 | YTT102 | `sys.version[2]` referenced (python3.10)               |
@@ -133,9 +129,7 @@
 ```yaml
 -   repo: https://github.com/pycqa/flake8
     rev: 3.7.8
     hooks:
     -   id: flake8
         additional_dependencies: [flake8-2020==1.6.1]
 ```
-
-
```

### Comparing `flake8_2020-1.7.0/README.md` & `flake8_2020-1.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.flake8-2020?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=27&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/27/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=27&branchName=main)
+[![build status](https://github.com/asottile/flake8-2020/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/flake8-2020/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/flake8-2020/main.svg)](https://results.pre-commit.ci/latest/github/asottile/flake8-2020/main)
 
 flake8-2020
 ===========
 
 flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 
@@ -12,15 +11,17 @@
 
 you might also find an early build of [python3.10] useful
 
 [python3.10]: https://github.com/asottile/python3.10
 
 ## installation
 
-`pip install flake8-2020`
+```bash
+pip install flake8-2020
+```
 
 ## flake8 codes
 
 | Code   | Description                                            |
 |--------|--------------------------------------------------------|
 | YTT101 | `sys.version[:3]` referenced (python3.10)              |
 | YTT102 | `sys.version[2]` referenced (python3.10)               |
```

### Comparing `flake8_2020-1.7.0/flake8_2020.egg-info/PKG-INFO` & `flake8_2020-1.8.0/flake8_2020.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: flake8-2020
-Version: 1.7.0
+Version: 1.8.0
 Summary: flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 Home-page: https://github.com/asottile/flake8-2020
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.flake8-2020?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=27&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/27/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=27&branchName=main)
+[![build status](https://github.com/asottile/flake8-2020/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/flake8-2020/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/flake8-2020/main.svg)](https://results.pre-commit.ci/latest/github/asottile/flake8-2020/main)
 
 flake8-2020
 ===========
 
 flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 
@@ -33,15 +27,17 @@
 
 you might also find an early build of [python3.10] useful
 
 [python3.10]: https://github.com/asottile/python3.10
 
 ## installation
 
-`pip install flake8-2020`
+```bash
+pip install flake8-2020
+```
 
 ## flake8 codes
 
 | Code   | Description                                            |
 |--------|--------------------------------------------------------|
 | YTT101 | `sys.version[:3]` referenced (python3.10)              |
 | YTT102 | `sys.version[2]` referenced (python3.10)               |
@@ -133,9 +129,7 @@
 ```yaml
 -   repo: https://github.com/pycqa/flake8
     rev: 3.7.8
     hooks:
     -   id: flake8
         additional_dependencies: [flake8-2020==1.6.1]
 ```
-
-
```

### Comparing `flake8_2020-1.7.0/flake8_2020.py` & `flake8_2020-1.8.0/flake8_2020.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     if sys.version_info >= (3, 9):  # pragma: >=3.9 cover
         node_slice = node.slice
     elif isinstance(node.slice, ast.Index):  # pragma: <3.9 cover
         node_slice = node.slice.value
     else:  # pragma: <3.9 cover
         return False
 
-    return isinstance(node_slice, ast.Num) and node_slice.n == n
+    return isinstance(node_slice, ast.Constant) and node_slice.value == n
 
 
 class Visitor(ast.NodeVisitor):
     def __init__(self) -> None:
         self.errors: list[tuple[int, int, str]] = []
         self._from_imports: dict[str, str] = {}
 
@@ -53,16 +53,16 @@
         )
 
     def _is_sys_version_upper_slice(self, node: ast.Subscript, n: int) -> bool:
         return (
             self._is_sys('version', node.value) and
             isinstance(node.slice, ast.Slice) and
             node.slice.lower is None and
-            isinstance(node.slice.upper, ast.Num) and
-            node.slice.upper.n == n and
+            isinstance(node.slice.upper, ast.Constant) and
+            node.slice.upper.value == n and
             node.slice.step is None
         )
 
     def visit_Subscript(self, node: ast.Subscript) -> None:
         if self._is_sys_version_upper_slice(node, 1):
             self.errors.append((
                 node.value.lineno, node.value.col_offset, YTT303,
@@ -85,16 +85,16 @@
     def visit_Compare(self, node: ast.Compare) -> None:
         if (
                 isinstance(node.left, ast.Subscript) and
                 self._is_sys('version_info', node.left.value) and
                 _is_index(node.left, n=0) and
                 len(node.ops) == 1 and
                 isinstance(node.ops[0], (ast.Eq, ast.NotEq)) and
-                isinstance(node.comparators[0], ast.Num) and
-                node.comparators[0].n == 3
+                isinstance(node.comparators[0], ast.Constant) and
+                node.comparators[0].value == 3
         ):
             self.errors.append((
                 node.left.lineno, node.left.col_offset, YTT201,
             ))
         elif (
                 self._is_sys('version', node.left) and
                 len(node.ops) == 1 and
@@ -110,26 +110,28 @@
             ))
         elif (
                 isinstance(node.left, ast.Subscript) and
                 self._is_sys('version_info', node.left.value) and
                 _is_index(node.left, n=1) and
                 len(node.ops) == 1 and
                 isinstance(node.ops[0], (ast.Lt, ast.LtE, ast.Gt, ast.GtE)) and
-                isinstance(node.comparators[0], ast.Num)
+                isinstance(node.comparators[0], ast.Constant) and
+                isinstance(node.comparators[0].value, (int, float))
         ):
             self.errors.append((
                 node.lineno, node.col_offset, YTT203,
             ))
         elif (
                 isinstance(node.left, ast.Attribute) and
                 self._is_sys('version_info', node.left.value) and
                 node.left.attr == 'minor' and
                 len(node.ops) == 1 and
                 isinstance(node.ops[0], (ast.Lt, ast.LtE, ast.Gt, ast.GtE)) and
-                isinstance(node.comparators[0], ast.Num)
+                isinstance(node.comparators[0], ast.Constant) and
+                isinstance(node.comparators[0].value, (int, float))
         ):
             self.errors.append((
                 node.lineno, node.col_offset, YTT204,
             ))
         self.generic_visit(node)
 
     def visit_Attribute(self, node: ast.Attribute) -> None:
```

### Comparing `flake8_2020-1.7.0/setup.cfg` & `flake8_2020-1.8.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 [metadata]
 name = flake8_2020
-version = 1.7.0
+version = 1.8.0
 description = flake8 plugin which checks for misuse of `sys.version` or `sys.version_info`
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/flake8-2020
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
 license_file = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 py_modules = flake8_2020
 install_requires = 
 	flake8>=5
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 flake8.extension = 
 	YTT=flake8_2020:Plugin
 
 [bdist_wheel]
 universal = True
@@ -36,15 +32,14 @@
 plugins = covdefaults
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
```

