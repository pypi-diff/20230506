# Comparing `tmp/texonomy-0.1.1.tar.gz` & `tmp/texonomy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texonomy-0.1.1.tar", last modified: Mon Mar 27 03:13:12 2023, max compression
+gzip compressed data, was "texonomy-0.2.0.tar", last modified: Sat May  6 00:59:55 2023, max compression
```

## Comparing `texonomy-0.1.1.tar` & `texonomy-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 ivy       (1000) ivy       (1000)        0 2023-03-27 03:13:12.304763 texonomy-0.1.1/
--rw-r--r--   0 ivy       (1000) ivy       (1000)     3377 2023-03-27 02:46:15.000000 texonomy-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 ivy       (1000) ivy       (1000)    11357 2023-03-27 02:46:15.000000 texonomy-0.1.1/LICENSE
--rw-r--r--   0 ivy       (1000) ivy       (1000)      363 2023-03-27 02:46:15.000000 texonomy-0.1.1/MANIFEST.in
--rw-r--r--   0 ivy       (1000) ivy       (1000)     2018 2023-03-27 02:46:15.000000 texonomy-0.1.1/Makefile
--rw-r--r--   0 ivy       (1000) ivy       (1000)    15624 2023-03-27 03:13:12.304763 texonomy-0.1.1/PKG-INFO
--rw-r--r--   0 ivy       (1000) ivy       (1000)     2303 2023-03-27 02:46:15.000000 texonomy-0.1.1/README.md
-drwxr-xr-x   0 ivy       (1000) ivy       (1000)        0 2023-03-27 03:13:12.284765 texonomy-0.1.1/examples/
--rw-r--r--   0 ivy       (1000) ivy       (1000)    19824 2023-03-27 02:46:15.000000 texonomy-0.1.1/examples/journal.pdf
--rw-r--r--   0 ivy       (1000) ivy       (1000)     1721 2023-03-27 02:54:59.000000 texonomy-0.1.1/pyproject.toml
--rw-r--r--   0 ivy       (1000) ivy       (1000)       38 2023-03-27 03:13:12.304763 texonomy-0.1.1/setup.cfg
--rw-r--r--   0 ivy       (1000) ivy       (1000)      174 2023-03-27 02:46:15.000000 texonomy-0.1.1/setup.py
-drwxr-xr-x   0 ivy       (1000) ivy       (1000)        0 2023-03-27 03:13:12.288765 texonomy-0.1.1/texonomy/
--rw-r--r--   0 ivy       (1000) ivy       (1000)       92 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/__init__.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)       22 2023-03-27 02:54:59.000000 texonomy-0.1.1/texonomy/_version.py
-drwxr-xr-x   0 ivy       (1000) ivy       (1000)        0 2023-03-27 03:13:12.296764 texonomy-0.1.1/texonomy/templates/
--rw-r--r--   0 ivy       (1000) ivy       (1000)        0 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/templates/__init__.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)     2662 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/templates/template.tex
-drwxr-xr-x   0 ivy       (1000) ivy       (1000)        0 2023-03-27 03:13:12.296764 texonomy-0.1.1/texonomy/tests/
-drwxr-xr-x   0 ivy       (1000) ivy       (1000)        0 2023-03-27 03:13:12.304763 texonomy-0.1.1/texonomy/tests/integration_tests/
--rw-r--r--   0 ivy       (1000) ivy       (1000)      118 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/integration_tests/Makefile
--rw-r--r--   0 ivy       (1000) ivy       (1000)      346 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/integration_tests/entity.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)     1296 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/integration_tests/kitchensink.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)      560 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/integration_tests/relattr.py
--rwxr-xr-x   0 ivy       (1000) ivy       (1000)      350 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/integration_tests/run_tests.sh
--rw-r--r--   0 ivy       (1000) ivy       (1000)      461 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/integration_tests/specialization.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)      657 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/integration_tests/weakentity.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)     1543 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/test_entity.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)     1571 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/test_erd.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)     1081 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/tests/test_line.py
--rw-r--r--   0 ivy       (1000) ivy       (1000)     7808 2023-03-27 02:46:15.000000 texonomy-0.1.1/texonomy/texonomy.py
-drwxr-xr-x   0 ivy       (1000) ivy       (1000)        0 2023-03-27 03:13:12.292764 texonomy-0.1.1/texonomy.egg-info/
--rw-r--r--   0 ivy       (1000) ivy       (1000)    15624 2023-03-27 03:13:12.000000 texonomy-0.1.1/texonomy.egg-info/PKG-INFO
--rw-r--r--   0 ivy       (1000) ivy       (1000)      790 2023-03-27 03:13:12.000000 texonomy-0.1.1/texonomy.egg-info/SOURCES.txt
--rw-r--r--   0 ivy       (1000) ivy       (1000)        1 2023-03-27 03:13:12.000000 texonomy-0.1.1/texonomy.egg-info/dependency_links.txt
--rw-r--r--   0 ivy       (1000) ivy       (1000)      136 2023-03-27 03:13:12.000000 texonomy-0.1.1/texonomy.egg-info/requires.txt
--rw-r--r--   0 ivy       (1000) ivy       (1000)        9 2023-03-27 03:13:12.000000 texonomy-0.1.1/texonomy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:59:55.255008 texonomy-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-05-06 00:56:16.000000 texonomy-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-06 00:56:16.000000 texonomy-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-06 00:56:16.000000 texonomy-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-05-06 00:56:16.000000 texonomy-0.2.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3277 2023-05-06 00:59:55.255008 texonomy-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-05-06 00:56:16.000000 texonomy-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:59:55.251008 texonomy-0.2.0/examples/
+-rw-r--r--   0 root         (0) root         (0)    19824 2023-05-06 00:56:16.000000 texonomy-0.2.0/examples/journal.pdf
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-05-06 00:56:16.000000 texonomy-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 00:59:55.255008 texonomy-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-06 00:59:46.000000 texonomy-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:59:55.251008 texonomy-0.2.0/texonomy/
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:59:55.251008 texonomy-0.2.0/texonomy/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/templates/template.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:59:55.255008 texonomy-0.2.0/texonomy/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:59:55.255008 texonomy-0.2.0/texonomy/tests/integration_tests/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/integration_tests/Makefile
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/integration_tests/entity.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/integration_tests/kitchensink.py
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/integration_tests/relattr.py
+-rwxr-xr-x   0 root         (0) root         (0)      350 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/integration_tests/run_tests.sh
+-rw-r--r--   0 root         (0) root         (0)      461 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/integration_tests/specialization.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/integration_tests/weakentity.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/test_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/test_erd.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/tests/test_line.py
+-rw-r--r--   0 root         (0) root         (0)    12183 2023-05-06 00:56:16.000000 texonomy-0.2.0/texonomy/texonomy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:59:55.251008 texonomy-0.2.0/texonomy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3277 2023-05-06 00:59:55.000000 texonomy-0.2.0/texonomy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      759 2023-05-06 00:59:55.000000 texonomy-0.2.0/texonomy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 00:59:55.000000 texonomy-0.2.0/texonomy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-06 00:59:55.000000 texonomy-0.2.0/texonomy.egg-info/top_level.txt
```

### Comparing `texonomy-0.1.1/CONTRIBUTING.md` & `texonomy-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/LICENSE` & `texonomy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/Makefile` & `texonomy-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/README.md` & `texonomy-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 `texonomy`* is a Python tool that facilitates the generation of
 entity-relationship diagrams in $\LaTeX$ using TikZ.
 
 [![License](https://img.shields.io/github/license/basseches/texonomy)](https://github.com/basseches/texonomy)
 [![Build Status](https://github.com/basseches/texonomy/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/basseches/texonomy/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/basseches/texonomy/branch/main/graph/badge.svg)](https://codecov.io/gh/basseches/texonomy)
+[![PyPI](https://img.shields.io/pypi/v/texonomy)](https://pypi.org/project/texonomy/)
+[![Docs](https://img.shields.io/badge/-docs-blueviolet)](https://basseches.github.io/texonomy)
 
 *An entity-relationship diagram is more of an ontology than a taxonomy, but
 when the shoe fits...
 
 ## Overview
 
 Writing $\LaTeX$ code can be tedious; `texonomy` makes it easier. This tool
```

### Comparing `texonomy-0.1.1/examples/journal.pdf` & `texonomy-0.2.0/examples/journal.pdf`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/pyproject.toml` & `texonomy-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "texonomy"
 authors = [{name = "Ivy Basseches", email = "imb2139@columbia.edu"}]
 description="A tool that generates entity-relationship diagrams in LaTeX."
 readme = "README.md"
-version = "0.1.1"
+version = "0.2.0"
 requires-python = ">=3.8"
 
 dependencies = []
 
 [project.license]
 file = "LICENSE"
 
@@ -43,22 +43,15 @@
 skip-string-normalization = true
 
 [tool.check-manifest]
 ignore = [
 ]
 
 [tool.flake8]
-ignore = ['E203', 'W503']
 max-line-length=120
-exclude=[
-    'example_project_python/tests/*'
-]
-per-file-ignores= [
-    'example_project_python/__init__.py:F401, F403'
-]
 
 [tool.isort]
 line_length = 120
 known_first_party = 'pydantic'
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
```

### Comparing `texonomy-0.1.1/texonomy/templates/template.tex` & `texonomy-0.2.0/texonomy/templates/template.tex`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/texonomy/tests/integration_tests/kitchensink.py` & `texonomy-0.2.0/texonomy/tests/integration_tests/kitchensink.py`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/texonomy/tests/integration_tests/relattr.py` & `texonomy-0.2.0/texonomy/tests/integration_tests/relattr.py`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/texonomy/tests/integration_tests/weakentity.py` & `texonomy-0.2.0/texonomy/tests/integration_tests/weakentity.py`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/texonomy/tests/test_entity.py` & `texonomy-0.2.0/texonomy/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/texonomy/tests/test_erd.py` & `texonomy-0.2.0/texonomy/tests/test_erd.py`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/texonomy/tests/test_line.py` & `texonomy-0.2.0/texonomy/tests/test_line.py`

 * *Files identical despite different names*

### Comparing `texonomy-0.1.1/texonomy.egg-info/SOURCES.txt` & `texonomy-0.2.0/texonomy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 examples/journal.pdf
 texonomy/__init__.py
 texonomy/_version.py
 texonomy/texonomy.py
 texonomy.egg-info/PKG-INFO
 texonomy.egg-info/SOURCES.txt
 texonomy.egg-info/dependency_links.txt
-texonomy.egg-info/requires.txt
 texonomy.egg-info/top_level.txt
 texonomy/templates/__init__.py
 texonomy/templates/template.tex
 texonomy/tests/test_entity.py
 texonomy/tests/test_erd.py
 texonomy/tests/test_line.py
 texonomy/tests/integration_tests/Makefile
```

