# Comparing `tmp/babi-1.5.3.tar.gz` & `tmp/babi-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babi-1.5.3.tar", last modified: Fri May 27 19:06:35 2022, max compression
+gzip compressed data, was "babi-1.5.4.tar", last modified: Sat May  6 20:19:47 2023, max compression
```

## Comparing `babi-1.5.3.tar` & `babi-1.5.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-27 19:06:35.780697 babi-1.5.3/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2021-10-03 22:55:17.000000 babi-1.5.3/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6505 2022-05-27 19:06:35.780697 babi-1.5.3/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5665 2022-05-27 16:29:21.000000 babi-1.5.3/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-27 19:06:35.780697 babi-1.5.3/babi/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2021-10-03 22:55:17.000000 babi-1.5.3/babi/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      120 2021-10-30 17:09:23.000000 babi-1.5.3/babi/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      162 2021-10-03 22:55:17.000000 babi-1.5.3/babi/_types.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    10869 2022-04-08 20:06:49.000000 babi-1.5.3/babi/buf.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      766 2022-01-13 19:36:16.000000 babi-1.5.3/babi/cached_property.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      600 2021-10-03 22:55:17.000000 babi-1.5.3/babi/color.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2075 2021-10-03 22:55:17.000000 babi-1.5.3/babi/color_kd.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1485 2022-03-12 21:28:38.000000 babi-1.5.3/babi/color_manager.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      144 2022-03-11 21:06:03.000000 babi-1.5.3/babi/dim.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1196 2021-10-03 22:55:17.000000 babi-1.5.3/babi/fdict.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    35102 2022-05-27 19:06:34.000000 babi-1.5.3/babi/file.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    24942 2022-03-23 20:18:59.000000 babi-1.5.3/babi/highlight.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1249 2021-10-03 22:55:17.000000 babi-1.5.3/babi/history.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-27 19:06:35.780697 babi-1.5.3/babi/hl/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2021-10-03 22:55:17.000000 babi-1.5.3/babi/hl/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      577 2022-03-15 18:47:50.000000 babi-1.5.3/babi/hl/interface.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8630 2022-04-05 17:14:49.000000 babi-1.5.3/babi/hl/lint_errors.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2021-10-03 22:55:17.000000 babi-1.5.3/babi/hl/replace.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1914 2021-10-03 22:55:17.000000 babi-1.5.3/babi/hl/selection.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5055 2022-03-23 20:18:59.000000 babi-1.5.3/babi/hl/syntax.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1615 2021-10-03 22:55:17.000000 babi-1.5.3/babi/hl/trailing_whitespace.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1051 2021-10-03 22:55:17.000000 babi-1.5.3/babi/horizontal_scrolling.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-27 19:06:35.780697 babi-1.5.3/babi/linters/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-03-23 20:18:59.000000 babi-1.5.3/babi/linters/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      537 2022-03-23 20:18:59.000000 babi-1.5.3/babi/linters/flake8.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2345 2022-03-23 20:18:59.000000 babi-1.5.3/babi/linters/pre_commit.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1349 2022-04-05 17:14:49.000000 babi-1.5.3/babi/linting.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5811 2022-03-11 21:06:03.000000 babi-1.5.3/babi/main.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1622 2021-10-03 22:55:17.000000 babi-1.5.3/babi/perf.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      311 2022-03-23 20:18:59.000000 babi-1.5.3/babi/proc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5759 2022-03-11 21:06:03.000000 babi-1.5.3/babi/prompt.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2295 2021-10-03 22:55:17.000000 babi-1.5.3/babi/reg.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-27 19:06:35.780697 babi-1.5.3/babi/resources/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-03-09 20:57:36.000000 babi-1.5.3/babi/resources/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13089 2022-03-09 20:57:36.000000 babi-1.5.3/babi/resources/default-theme.json
--rw-r--r--   0 asottile  (1000) asottile  (1000)    29300 2022-05-27 18:39:36.000000 babi-1.5.3/babi/screen.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1225 2022-03-18 19:34:39.000000 babi-1.5.3/babi/status.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2217 2022-03-21 19:00:25.000000 babi-1.5.3/babi/textmate_demo.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5057 2022-03-22 17:35:09.000000 babi-1.5.3/babi/theme.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      535 2021-10-03 22:55:17.000000 babi-1.5.3/babi/user_data.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-27 19:06:35.780697 babi-1.5.3/babi.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6505 2022-05-27 19:06:35.000000 babi-1.5.3/babi.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      939 2022-05-27 19:06:35.000000 babi-1.5.3/babi.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-05-27 19:06:35.000000 babi-1.5.3/babi.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       85 2022-05-27 19:06:35.000000 babi-1.5.3/babi.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      137 2022-05-27 19:06:35.000000 babi-1.5.3/babi.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        5 2022-05-27 19:06:35.000000 babi-1.5.3/babi.egg-info/top_level.txt
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-05-27 19:06:35.780697 babi-1.5.3/licenses/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1191 2022-03-09 20:57:36.000000 babi-1.5.3/licenses/microsoft_vscode_LICENSE.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1596 2022-05-27 19:06:35.784697 babi-1.5.3/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2021-10-03 22:55:17.000000 babi-1.5.3/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.635421 babi-1.5.4/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-04-30 16:59:38.000000 babi-1.5.4/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6105 2023-05-06 20:19:47.635421 babi-1.5.4/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5486 2022-12-29 22:23:55.000000 babi-1.5.4/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.627421 babi-1.5.4/babi/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.4/babi/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      120 2022-04-30 16:59:38.000000 babi-1.5.4/babi/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      162 2022-04-30 16:59:38.000000 babi-1.5.4/babi/_types.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    10869 2022-04-30 16:59:38.000000 babi-1.5.4/babi/buf.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      766 2022-04-30 16:59:38.000000 babi-1.5.4/babi/cached_property.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      600 2022-04-30 16:59:38.000000 babi-1.5.4/babi/color.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1825 2022-10-29 23:19:26.000000 babi-1.5.4/babi/color_kd.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1485 2022-04-30 16:59:38.000000 babi-1.5.4/babi/color_manager.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      144 2022-04-30 16:59:38.000000 babi-1.5.4/babi/dim.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1196 2022-04-30 16:59:38.000000 babi-1.5.4/babi/fdict.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    35102 2022-10-29 23:19:26.000000 babi-1.5.4/babi/file.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    24091 2022-10-29 23:19:26.000000 babi-1.5.4/babi/highlight.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1249 2022-04-30 16:59:38.000000 babi-1.5.4/babi/history.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.631421 babi-1.5.4/babi/hl/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      577 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/interface.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8630 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/lint_errors.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/replace.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1914 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/selection.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5055 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/syntax.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1615 2022-04-30 16:59:38.000000 babi-1.5.4/babi/hl/trailing_whitespace.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1051 2022-04-30 16:59:38.000000 babi-1.5.4/babi/horizontal_scrolling.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.635421 babi-1.5.4/babi/linters/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.4/babi/linters/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      537 2022-04-30 16:59:38.000000 babi-1.5.4/babi/linters/flake8.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2345 2022-04-30 16:59:38.000000 babi-1.5.4/babi/linters/pre_commit.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1349 2022-04-30 16:59:38.000000 babi-1.5.4/babi/linting.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5811 2022-04-30 16:59:38.000000 babi-1.5.4/babi/main.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1622 2022-04-30 16:59:38.000000 babi-1.5.4/babi/perf.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      311 2022-04-30 16:59:38.000000 babi-1.5.4/babi/proc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5759 2022-04-30 16:59:38.000000 babi-1.5.4/babi/prompt.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2295 2022-04-30 16:59:38.000000 babi-1.5.4/babi/reg.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.635421 babi-1.5.4/babi/resources/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:38.000000 babi-1.5.4/babi/resources/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13089 2022-04-30 16:59:38.000000 babi-1.5.4/babi/resources/default-theme.json
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    29300 2022-10-29 23:19:26.000000 babi-1.5.4/babi/screen.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1225 2022-04-30 16:59:38.000000 babi-1.5.4/babi/status.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2217 2022-04-30 16:59:38.000000 babi-1.5.4/babi/textmate_demo.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4870 2022-10-29 23:19:26.000000 babi-1.5.4/babi/theme.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      535 2022-04-30 16:59:38.000000 babi-1.5.4/babi/user_data.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.631421 babi-1.5.4/babi.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6105 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      939 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       85 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      144 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        5 2023-05-06 20:19:47.000000 babi-1.5.4/babi.egg-info/top_level.txt
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:19:47.635421 babi-1.5.4/licenses/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1191 2022-04-30 16:59:38.000000 babi-1.5.4/licenses/microsoft_vscode_LICENSE.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1450 2023-05-06 20:19:47.635421 babi-1.5.4/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:38.000000 babi-1.5.4/setup.py
```

### Comparing `babi-1.5.3/LICENSE` & `babi-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/PKG-INFO` & `babi-1.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 Metadata-Version: 2.1
 Name: babi
-Version: 1.5.3
+Version: 1.5.4
 Summary: a text editor
 Home-page: https://github.com/asottile/babi
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
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: licenses/microsoft_vscode_LICENSE.txt
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.babi?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=29&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/29/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=29&branchName=main)
+[![build status](https://github.com/asottile/babi/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/babi/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/babi/main.svg)](https://results.pre-commit.ci/latest/github/asottile/babi/main)
 
 ![babi logo](https://user-images.githubusercontent.com/1810591/89981369-9ed84e80-dc28-11ea-9708-5f4c49c09632.png)
 
 babi
 ====
 
 a text editor, eventually...
 
 ### installation
 
-`pip install babi`
+```bash
+pip install babi
+```
 
 babi works best in a virtualenv
 
 ### why is it called babi?
 
 I used to use the text editor `nano`, frequently I typo this.  on a qwerty
 keyboard, when the right hand is shifted left by one, `nano` becomes `babi`.
@@ -97,17 +93,18 @@
     - <kbd>Esc</kbd>, <kbd>M-t</kdb>: unfocus the linting panel
     - arrow keys: movement inside the linting panel
 - <kbd>esc</kbd>: open the command mode
     - <kbd>:q</kbd>: quit
     - <kbd>:w</kbd>: write the file
     - <kbd>:wq</kbd>: write the file and quit
     - <kbd>:qall</kbd>: quit every open file
-    - <kbd>:comment</kbd>: comment on the current line / selection
+    - <kbd>:comment</kbd>: comment out the current line / selection
     - <kbd>:reload</kbd>: reload the file contents
     - <kbd>:sort</kbd>: sort the file (or selection)
+    - <kbd>:tabsize X</kbd>: set the tabsize
 
 in prompts (search, search replace, command):
 - <kbd>^C</kbd>: cancel
 - <kbd>^K</kbd>: cut to end
 - <kbd>^R</kbd>: reverse search
 
 ### setting up syntax highlighting
@@ -160,9 +157,7 @@
 ![](https://i.fluffy.cc/p8lv61TCql1MJfpBDqbNPWPf27lmGWFN.png)
 
 ![](https://i.fluffy.cc/ZH5sswB4FSbpW8FfcXL1KZWdJnjxRkbW.png)
 
 ![](https://i.fluffy.cc/Rw8nZKFC3R36mNrV01fL2gk4rfwWn7wX.png)
 
 ![](https://i.fluffy.cc/FSD92ZVN4xcMFPv1V7gc0Xzk8TCQTgdg.png)
-
-
```

### Comparing `babi-1.5.3/README.md` & `babi-1.5.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.babi?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=29&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/29/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=29&branchName=main)
+[![build status](https://github.com/asottile/babi/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/babi/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/babi/main.svg)](https://results.pre-commit.ci/latest/github/asottile/babi/main)
 
 ![babi logo](https://user-images.githubusercontent.com/1810591/89981369-9ed84e80-dc28-11ea-9708-5f4c49c09632.png)
 
 babi
 ====
 
 a text editor, eventually...
 
 ### installation
 
-`pip install babi`
+```bash
+pip install babi
+```
 
 babi works best in a virtualenv
 
 ### why is it called babi?
 
 I used to use the text editor `nano`, frequently I typo this.  on a qwerty
 keyboard, when the right hand is shifted left by one, `nano` becomes `babi`.
@@ -74,17 +75,18 @@
     - <kbd>Esc</kbd>, <kbd>M-t</kdb>: unfocus the linting panel
     - arrow keys: movement inside the linting panel
 - <kbd>esc</kbd>: open the command mode
     - <kbd>:q</kbd>: quit
     - <kbd>:w</kbd>: write the file
     - <kbd>:wq</kbd>: write the file and quit
     - <kbd>:qall</kbd>: quit every open file
-    - <kbd>:comment</kbd>: comment on the current line / selection
+    - <kbd>:comment</kbd>: comment out the current line / selection
     - <kbd>:reload</kbd>: reload the file contents
     - <kbd>:sort</kbd>: sort the file (or selection)
+    - <kbd>:tabsize X</kbd>: set the tabsize
 
 in prompts (search, search replace, command):
 - <kbd>^C</kbd>: cancel
 - <kbd>^K</kbd>: cut to end
 - <kbd>^R</kbd>: reverse search
 
 ### setting up syntax highlighting
```

### Comparing `babi-1.5.3/babi/buf.py` & `babi-1.5.4/babi/buf.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/cached_property.py` & `babi-1.5.4/babi/cached_property.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/color.py` & `babi-1.5.4/babi/color.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/color_kd.py` & `babi-1.5.4/babi/color_kd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,36 @@
 from __future__ import annotations
 
 import functools
 import itertools
 from typing import NamedTuple
 
-from babi._types import Protocol
 from babi.color import Color
 
 
 def _square_distance(c1: Color, c2: Color) -> int:
     return (c1.r - c2.r) ** 2 + (c1.g - c2.g) ** 2 + (c1.b - c2.b) ** 2
 
 
-class KD(Protocol):
-    @property
-    def color(self) -> Color: ...
-    @property
-    def n(self) -> int: ...
-    @property
-    def left(self) -> KD | None: ...
-    @property
-    def right(self) -> KD | None: ...
-
-
-class _KD(NamedTuple):
+class KD(NamedTuple):
     color: Color
     n: int
     left: KD | None
     right: KD | None
 
 
 def _build(colors: list[tuple[Color, int]], depth: int = 0) -> KD | None:
     if not colors:
         return None
 
     axis = depth % 3
     colors.sort(key=lambda kv: kv[0][axis])
     pivot = len(colors) // 2
 
-    return _KD(
+    return KD(
         *colors[pivot],
         _build(colors[:pivot], depth=depth + 1),
         _build(colors[pivot + 1:], depth=depth + 1),
     )
 
 
 def nearest(color: Color, colors: KD | None) -> int:
```

### Comparing `babi-1.5.3/babi/color_manager.py` & `babi-1.5.4/babi/color_manager.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/fdict.py` & `babi-1.5.4/babi/fdict.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/file.py` & `babi-1.5.4/babi/file.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/highlight.py` & `babi-1.5.4/babi/highlight.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from babi.reg import expand_escaped
 from babi.reg import make_reg
 from babi.reg import make_regset
 
 T = TypeVar('T')
 Scope = Tuple[str, ...]
 Regions = Tuple['Region', ...]
-Captures = Tuple[Tuple[int, '_Rule'], ...]
+Captures = Tuple[Tuple[int, 'Rule'], ...]
 
 
 def uniquely_constructed(t: T) -> T:
     """avoid tuple.__hash__ for "singleton" constructed objects"""
     t.__hash__ = object.__hash__  # type: ignore
     return t
 
@@ -36,70 +36,40 @@
 def _split_name(s: str | None) -> tuple[str, ...]:
     if s is None:
         return ()
     else:
         return tuple(s.split())
 
 
-class _Rule(Protocol):
-    """hax for recursive types python/mypy#731"""
-    @property
-    def name(self) -> tuple[str, ...]: ...
-    @property
-    def match(self) -> str | None: ...
-    @property
-    def begin(self) -> str | None: ...
-    @property
-    def end(self) -> str | None: ...
-    @property
-    def while_(self) -> str | None: ...
-    @property
-    def content_name(self) -> tuple[str, ...]: ...
-    @property
-    def captures(self) -> Captures: ...
-    @property
-    def begin_captures(self) -> Captures: ...
-    @property
-    def end_captures(self) -> Captures: ...
-    @property
-    def while_captures(self) -> Captures: ...
-    @property
-    def include(self) -> str | None: ...
-    @property
-    def patterns(self) -> tuple[_Rule, ...]: ...
-    @property
-    def repository(self) -> FChainMap[str, _Rule]: ...
-
-
 @uniquely_constructed
 class Rule(NamedTuple):
     name: tuple[str, ...]
     match: str | None
     begin: str | None
     end: str | None
     while_: str | None
     content_name: tuple[str, ...]
     captures: Captures
     begin_captures: Captures
     end_captures: Captures
     while_captures: Captures
     include: str | None
-    patterns: tuple[_Rule, ...]
-    repository: FChainMap[str, _Rule]
+    patterns: tuple[Rule, ...]
+    repository: FChainMap[str, Rule]
 
     @classmethod
     def make(
             cls,
             dct: dict[str, Any],
-            parent_repository: FChainMap[str, _Rule],
-    ) -> _Rule:
+            parent_repository: FChainMap[str, Rule],
+    ) -> Rule:
         if 'repository' in dct:
             # this looks odd, but it's so we can have a self-referential
             # immutable-after-construction chain map
-            repository_dct: dict[str, _Rule] = {}
+            repository_dct: dict[str, Rule] = {}
             repository = FChainMap(parent_repository, repository_dct)
             for k, sub_dct in dct['repository'].items():
                 repository_dct[k] = Rule.make(sub_dct, repository)
         else:
             repository = parent_repository
 
         name = _split_name(dct.get('name'))
@@ -177,24 +147,24 @@
             repository=repository,
         )
 
 
 @uniquely_constructed
 class Grammar(NamedTuple):
     scope_name: str
-    repository: FChainMap[str, _Rule]
-    patterns: tuple[_Rule, ...]
+    repository: FChainMap[str, Rule]
+    patterns: tuple[Rule, ...]
 
     @classmethod
     def make(cls, data: dict[str, Any]) -> Grammar:
         scope_name = data['scopeName']
         if 'repository' in data:
             # this looks odd, but it's so we can have a self-referential
             # immutable-after-construction chain map
-            repository_dct: dict[str, _Rule] = {}
+            repository_dct: dict[str, Rule] = {}
             repository = FChainMap(repository_dct)
             for k, dct in data['repository'].items():
                 repository_dct[k] = Rule.make(dct, repository)
         else:
             repository = FChainMap()
         patterns = tuple(Rule.make(d, repository) for d in data['patterns'])
         return cls(
@@ -262,15 +232,15 @@
         ...
 
 
 class CompiledRegsetRule(CompiledRule, Protocol):
     @property
     def regset(self) -> _RegSet: ...
     @property
-    def u_rules(self) -> tuple[_Rule, ...]: ...
+    def u_rules(self) -> tuple[Rule, ...]: ...
 
 
 class Entry(NamedTuple):
     scope: tuple[str, ...]
     rule: CompiledRule
     start: tuple[str, int]
     reg: _Reg = ERR_REG
@@ -366,15 +336,15 @@
     return state, match.end(), boundary, tuple(ret)
 
 
 @uniquely_constructed
 class PatternRule(NamedTuple):
     name: tuple[str, ...]
     regset: _RegSet
-    u_rules: tuple[_Rule, ...]
+    u_rules: tuple[Rule, ...]
 
     def start(
             self,
             compiler: Compiler,
             match: Match[str],
             state: State,
     ) -> tuple[State, bool, Regions]:
@@ -423,15 +393,15 @@
 class EndRule(NamedTuple):
     name: tuple[str, ...]
     content_name: tuple[str, ...]
     begin_captures: Captures
     end_captures: Captures
     end: str
     regset: _RegSet
-    u_rules: tuple[_Rule, ...]
+    u_rules: tuple[Rule, ...]
 
     def start(
             self,
             compiler: Compiler,
             match: Match[str],
             state: State,
     ) -> tuple[State, bool, Regions]:
@@ -494,15 +464,15 @@
 class WhileRule(NamedTuple):
     name: tuple[str, ...]
     content_name: tuple[str, ...]
     begin_captures: Captures
     while_captures: Captures
     while_: str
     regset: _RegSet
-    u_rules: tuple[_Rule, ...]
+    u_rules: tuple[Rule, ...]
 
     def start(
             self,
             compiler: Compiler,
             match: Match[str],
             state: State,
     ) -> tuple[State, bool, Regions]:
@@ -549,29 +519,29 @@
 class Compiler:
     def __init__(self, grammar: Grammar, grammars: Grammars) -> None:
         self._include = functools.lru_cache(maxsize=None)(self._include_)
         self._patterns = functools.lru_cache(maxsize=None)(self._patterns_)
 
         self.root_scope = grammar.scope_name
         self._grammars = grammars
-        self._rule_to_grammar: dict[_Rule, Grammar] = {}
-        self._c_rules: dict[_Rule, CompiledRule] = {}
+        self._rule_to_grammar: dict[Rule, Grammar] = {}
+        self._c_rules: dict[Rule, CompiledRule] = {}
         root = self._compile_root(grammar)
         self.root_state = State.root(Entry(root.name, root, ('', 0)))
 
-    def _visit_rule(self, grammar: Grammar, rule: _Rule) -> _Rule:
+    def _visit_rule(self, grammar: Grammar, rule: Rule) -> Rule:
         self._rule_to_grammar[rule] = grammar
         return rule
 
     def _include_(
             self,
             grammar: Grammar,
-            repository: FChainMap[str, _Rule],
+            repository: FChainMap[str, Rule],
             s: str,
-    ) -> tuple[list[str], tuple[_Rule, ...]]:
+    ) -> tuple[list[str], tuple[Rule, ...]]:
         if s == '$self':
             return self._patterns(grammar, grammar.patterns)
         elif s == '$base':
             grammar = self._grammars.grammar_for_scope(self.root_scope)
             return self._include(grammar, grammar.repository, '$self')
         elif s.startswith('#'):
             return self._patterns(grammar, (repository[s[1:]],))
@@ -582,18 +552,18 @@
             scope, _, s = s.partition('#')
             grammar = self._grammars.grammar_for_scope(scope)
             return self._include(grammar, grammar.repository, f'#{s}')
 
     def _patterns_(
             self,
             grammar: Grammar,
-            rules: tuple[_Rule, ...],
-    ) -> tuple[list[str], tuple[_Rule, ...]]:
+            rules: tuple[Rule, ...],
+    ) -> tuple[list[str], tuple[Rule, ...]]:
         ret_regs = []
-        ret_rules: list[_Rule] = []
+        ret_rules: list[Rule] = []
         for rule in rules:
             if rule.include is not None:
                 tmp_regs, tmp_rules = self._include(
                     grammar, rule.repository, rule.include,
                 )
                 ret_regs.extend(tmp_regs)
                 ret_rules.extend(tmp_rules)
@@ -618,15 +588,15 @@
     ) -> Captures:
         return tuple((n, self._visit_rule(grammar, r)) for n, r in captures)
 
     def _compile_root(self, grammar: Grammar) -> PatternRule:
         regs, rules = self._patterns(grammar, grammar.patterns)
         return PatternRule((grammar.scope_name,), make_regset(*regs), rules)
 
-    def _compile_rule(self, grammar: Grammar, rule: _Rule) -> CompiledRule:
+    def _compile_rule(self, grammar: Grammar, rule: Rule) -> CompiledRule:
         assert rule.include is None, rule
         if rule.match is not None:
             captures_ref = self._captures_ref(grammar, rule.captures)
             return MatchRule(rule.name, captures_ref)
         elif rule.begin is not None and rule.end is not None:
             regs, rules = self._patterns(grammar, rule.patterns)
             return EndRule(
@@ -649,15 +619,15 @@
                 make_regset(*regs),
                 rules,
             )
         else:
             regs, rules = self._patterns(grammar, rule.patterns)
             return PatternRule(rule.name, make_regset(*regs), rules)
 
-    def compile_rule(self, rule: _Rule) -> CompiledRule:
+    def compile_rule(self, rule: Rule) -> CompiledRule:
         try:
             return self._c_rules[rule]
         except KeyError:
             pass
 
         grammar = self._rule_to_grammar[rule]
         ret = self._c_rules[rule] = self._compile_rule(grammar, rule)
```

### Comparing `babi-1.5.3/babi/history.py` & `babi-1.5.4/babi/history.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/hl/interface.py` & `babi-1.5.4/babi/hl/interface.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/hl/lint_errors.py` & `babi-1.5.4/babi/hl/lint_errors.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/hl/replace.py` & `babi-1.5.4/babi/hl/replace.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/hl/selection.py` & `babi-1.5.4/babi/hl/selection.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/hl/syntax.py` & `babi-1.5.4/babi/hl/syntax.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/hl/trailing_whitespace.py` & `babi-1.5.4/babi/hl/trailing_whitespace.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/horizontal_scrolling.py` & `babi-1.5.4/babi/horizontal_scrolling.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/linters/flake8.py` & `babi-1.5.4/babi/linters/flake8.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/linters/pre_commit.py` & `babi-1.5.4/babi/linters/pre_commit.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/linting.py` & `babi-1.5.4/babi/linting.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/main.py` & `babi-1.5.4/babi/main.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/perf.py` & `babi-1.5.4/babi/perf.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/prompt.py` & `babi-1.5.4/babi/prompt.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/reg.py` & `babi-1.5.4/babi/reg.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/resources/default-theme.json` & `babi-1.5.4/babi/resources/default-theme.json`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/screen.py` & `babi-1.5.4/babi/screen.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/status.py` & `babi-1.5.4/babi/status.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/textmate_demo.py` & `babi-1.5.4/babi/textmate_demo.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi/theme.py` & `babi-1.5.4/babi/theme.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import functools
 import importlib.resources
 import json
 import os.path
 from typing import Any
 from typing import NamedTuple
 
-from babi._types import Protocol
 from babi.color import Color
 from babi.color_manager import ColorManager
 from babi.fdict import FDict
 
 A_ITALIC = getattr(curses, 'A_ITALIC', 0x80000000)  # not always present
 
 
@@ -62,35 +61,28 @@
         elif dct.get('fontStyle') == 'italic':
             kv['i'] = True
         elif dct.get('fontStyle') == 'underline':
             kv['u'] = True
         return cls(**kv)
 
 
-class _TrieNode(Protocol):
-    @property
-    def style(self) -> PartialStyle: ...
-    @property
-    def children(self) -> FDict[str, _TrieNode]: ...
-
-
 class TrieNode(NamedTuple):
     style: PartialStyle
-    children: FDict[str, _TrieNode]
+    children: FDict[str, TrieNode]
 
     @classmethod
-    def from_dct(cls, dct: dict[str, Any]) -> _TrieNode:
+    def from_dct(cls, dct: dict[str, Any]) -> TrieNode:
         children = FDict({
             k: TrieNode.from_dct(v) for k, v in dct['children'].items()
         })
         return cls(PartialStyle.from_dct(dct), children)
 
 
 class Theme:
-    def __init__(self, default: Style, rules: _TrieNode) -> None:
+    def __init__(self, default: Style, rules: TrieNode) -> None:
         self.default = default
         self.rules = rules
         self.select = functools.lru_cache(maxsize=None)(self._select)
 
     def _select(self, scope: tuple[str, ...]) -> Style:
         if not scope:
             return self.default
```

### Comparing `babi-1.5.3/babi/user_data.py` & `babi-1.5.4/babi/user_data.py`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/babi.egg-info/PKG-INFO` & `babi-1.5.4/babi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 Metadata-Version: 2.1
 Name: babi
-Version: 1.5.3
+Version: 1.5.4
 Summary: a text editor
 Home-page: https://github.com/asottile/babi
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
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: licenses/microsoft_vscode_LICENSE.txt
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.babi?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=29&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/29/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=29&branchName=main)
+[![build status](https://github.com/asottile/babi/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/babi/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/babi/main.svg)](https://results.pre-commit.ci/latest/github/asottile/babi/main)
 
 ![babi logo](https://user-images.githubusercontent.com/1810591/89981369-9ed84e80-dc28-11ea-9708-5f4c49c09632.png)
 
 babi
 ====
 
 a text editor, eventually...
 
 ### installation
 
-`pip install babi`
+```bash
+pip install babi
+```
 
 babi works best in a virtualenv
 
 ### why is it called babi?
 
 I used to use the text editor `nano`, frequently I typo this.  on a qwerty
 keyboard, when the right hand is shifted left by one, `nano` becomes `babi`.
@@ -97,17 +93,18 @@
     - <kbd>Esc</kbd>, <kbd>M-t</kdb>: unfocus the linting panel
     - arrow keys: movement inside the linting panel
 - <kbd>esc</kbd>: open the command mode
     - <kbd>:q</kbd>: quit
     - <kbd>:w</kbd>: write the file
     - <kbd>:wq</kbd>: write the file and quit
     - <kbd>:qall</kbd>: quit every open file
-    - <kbd>:comment</kbd>: comment on the current line / selection
+    - <kbd>:comment</kbd>: comment out the current line / selection
     - <kbd>:reload</kbd>: reload the file contents
     - <kbd>:sort</kbd>: sort the file (or selection)
+    - <kbd>:tabsize X</kbd>: set the tabsize
 
 in prompts (search, search replace, command):
 - <kbd>^C</kbd>: cancel
 - <kbd>^K</kbd>: cut to end
 - <kbd>^R</kbd>: reverse search
 
 ### setting up syntax highlighting
@@ -160,9 +157,7 @@
 ![](https://i.fluffy.cc/p8lv61TCql1MJfpBDqbNPWPf27lmGWFN.png)
 
 ![](https://i.fluffy.cc/ZH5sswB4FSbpW8FfcXL1KZWdJnjxRkbW.png)
 
 ![](https://i.fluffy.cc/Rw8nZKFC3R36mNrV01fL2gk4rfwWn7wX.png)
 
 ![](https://i.fluffy.cc/FSD92ZVN4xcMFPv1V7gc0Xzk8TCQTgdg.png)
-
-
```

### Comparing `babi-1.5.3/babi.egg-info/SOURCES.txt` & `babi-1.5.4/babi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/licenses/microsoft_vscode_LICENSE.txt` & `babi-1.5.4/licenses/microsoft_vscode_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `babi-1.5.3/setup.cfg` & `babi-1.5.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 [metadata]
 name = babi
-version = 1.5.3
+version = 1.5.4
 description = a text editor
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/babi
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
 license_file = LICENSE
 license_files = 
 	licenses/microsoft_vscode_LICENSE.txt
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
 install_requires = 
 	babi-grammars
 	identify
 	onigurumacffi>=0.0.18
 	importlib-metadata>=1;python_version<"3.8"
-	windows-curses;sys_platform=="win32"
+	windows-curses!=2.3.1;sys_platform=="win32"
 python_requires = >=3.7
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
 
@@ -54,15 +50,15 @@
 parallel = true
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
+enable_recursive_aliases = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
```

