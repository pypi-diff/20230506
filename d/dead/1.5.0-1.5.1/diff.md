# Comparing `tmp/dead-1.5.0.tar.gz` & `tmp/dead-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dead-1.5.0.tar", last modified: Tue May 17 00:10:55 2022, max compression
+gzip compressed data, was "dead-1.5.1.tar", last modified: Sat May  6 20:35:39 2023, max compression
```

## Comparing `dead-1.5.0.tar` & `dead-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-17 00:10:55.724193 dead-1.5.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-05-16 22:31:56.000000 dead-1.5.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2989 2022-05-17 00:10:55.724193 dead-1.5.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2295 2022-05-17 00:10:54.000000 dead-1.5.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-17 00:10:55.724193 dead-1.5.0/dead.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2989 2022-05-17 00:10:55.000000 dead-1.5.0/dead.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      214 2022-05-17 00:10:55.000000 dead-1.5.0/dead.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-05-17 00:10:55.000000 dead-1.5.0/dead.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       35 2022-05-17 00:10:55.000000 dead-1.5.0/dead.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2022-05-17 00:10:55.000000 dead-1.5.0/dead.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        5 2022-05-17 00:10:55.000000 dead-1.5.0/dead.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11877 2022-05-17 00:10:54.000000 dead-1.5.0/dead.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1176 2022-05-17 00:10:55.724193 dead-1.5.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-05-16 22:31:56.000000 dead-1.5.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:35:39.315444 dead-1.5.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-06 20:21:19.000000 dead-1.5.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2593 2023-05-06 20:35:39.315444 dead-1.5.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2070 2023-05-06 20:35:39.000000 dead-1.5.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:35:39.315444 dead-1.5.1/dead.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2593 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      214 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       35 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        5 2023-05-06 20:35:39.000000 dead-1.5.1/dead.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12050 2023-05-06 20:35:39.000000 dead-1.5.1/dead.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1030 2023-05-06 20:35:39.319444 dead-1.5.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-06 20:21:19.000000 dead-1.5.1/setup.py
```

### Comparing `dead-1.5.0/LICENSE` & `dead-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dead-1.5.0/PKG-INFO` & `dead-1.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: dead
-Version: 1.5.0
+Version: 1.5.1
 Summary: dead simple python dead code detection
 Home-page: https://github.com/asottile/dead
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.dead?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=32&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/32/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=32&branchName=main)
+[![build status](https://github.com/asottile/dead/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/dead/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/dead/main.svg)](https://results.pre-commit.ci/latest/github/asottile/dead/main)
 
 dead
 ====
 
 dead simple python dead code detection
 
 ## installation
 
-`pip install dead`
+```bash
+pip install dead
+```
 
 
 ## cli
 
 Consult the help for the latest usage:
 
 ```console
@@ -54,15 +51,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/dead
-    rev: v1.5.0
+    rev: v1.5.1
     hooks:
     -   id: dead
 ```
 
 ### how it works
 
 1. find all files in a repository using `git ls-files` and filtering:
@@ -87,9 +84,7 @@
 
 The `# dead: disable` comment will tell `dead` to ignore
 any line which has reportedly dead code.
 
 ### is this project dead?
 
 _maybe._
-
-
```

### Comparing `dead-1.5.0/README.md` & `dead-1.5.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.dead?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=32&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/32/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=32&branchName=main)
+[![build status](https://github.com/asottile/dead/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/dead/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/dead/main.svg)](https://results.pre-commit.ci/latest/github/asottile/dead/main)
 
 dead
 ====
 
 dead simple python dead code detection
 
 ## installation
 
-`pip install dead`
+```bash
+pip install dead
+```
 
 
 ## cli
 
 Consult the help for the latest usage:
 
 ```console
@@ -34,15 +35,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/dead
-    rev: v1.5.0
+    rev: v1.5.1
     hooks:
     -   id: dead
 ```
 
 ### how it works
 
 1. find all files in a repository using `git ls-files` and filtering:
```

### Comparing `dead-1.5.0/dead.egg-info/PKG-INFO` & `dead-1.5.1/dead.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: dead
-Version: 1.5.0
+Version: 1.5.1
 Summary: dead simple python dead code detection
 Home-page: https://github.com/asottile/dead
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.dead?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=32&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/32/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=32&branchName=main)
+[![build status](https://github.com/asottile/dead/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/dead/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/dead/main.svg)](https://results.pre-commit.ci/latest/github/asottile/dead/main)
 
 dead
 ====
 
 dead simple python dead code detection
 
 ## installation
 
-`pip install dead`
+```bash
+pip install dead
+```
 
 
 ## cli
 
 Consult the help for the latest usage:
 
 ```console
@@ -54,15 +51,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/dead
-    rev: v1.5.0
+    rev: v1.5.1
     hooks:
     -   id: dead
 ```
 
 ### how it works
 
 1. find all files in a repository using `git ls-files` and filtering:
@@ -87,9 +84,7 @@
 
 The `# dead: disable` comment will tell `dead` to ignore
 any line which has reportedly dead code.
 
 ### is this project dead?
 
 _maybe._
-
-
```

### Comparing `dead-1.5.0/dead.py` & `dead-1.5.1/dead.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,16 @@
         self.define(node.name, node)
         self.generic_visit(node)
 
     def _is_stub_function(self, node: FunctionDef) -> bool:
         for stmt in node.body:
             if (
                     isinstance(stmt, ast.Expr) and
-                    isinstance(stmt.value, (ast.Str, ast.Ellipsis))
+                    isinstance(stmt.value, ast.Constant) and
+                    isinstance(stmt.value.value, (str, type(Ellipsis)))
             ):
                 continue  # docstring or ...
             elif isinstance(stmt, ast.Pass):
                 continue  # pass
             elif (
                     isinstance(stmt, ast.Raise) and
                     stmt.cause is None and (
@@ -158,16 +159,19 @@
         if (
                 len(node.targets) == 1 and
                 isinstance(node.targets[0], ast.Name) and
                 node.targets[0].id == '__all__' and
                 isinstance(node.value, (ast.Tuple, ast.List))
         ):
             for elt in node.value.elts:
-                if isinstance(elt, ast.Str):
-                    self.read(elt.s, elt)
+                if (
+                        isinstance(elt, ast.Constant) and
+                        isinstance(elt.value, str)
+                ):
+                    self.read(elt.value, elt)
 
         self.generic_visit(node)
 
     # TODO: AnnAssign
 
     def visit_Name(self, node: ast.Name) -> None:
         if isinstance(node.ctx, ast.Load):
```

