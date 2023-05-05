# Comparing `tmp/mpl-smithchart-0.1.0.tar.gz` & `tmp/mpl-smithchart-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl-smithchart-0.1.0.tar", last modified: Fri May  5 23:05:15 2023, max compression
+gzip compressed data, was "mpl-smithchart-0.1.1.tar", last modified: Fri May  5 23:32:57 2023, max compression
```

## Comparing `mpl-smithchart-0.1.0.tar` & `mpl-smithchart-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 spencer   (1000) spencer   (1000)        0 2023-05-05 23:05:15.521320 mpl-smithchart-0.1.0/
-drwxr-xr-x   0 spencer   (1000) spencer   (1000)        0 2023-05-05 23:05:15.517987 mpl-smithchart-0.1.0/.github/
-drwxr-xr-x   0 spencer   (1000) spencer   (1000)        0 2023-05-05 23:05:15.517987 mpl-smithchart-0.1.0/.github/workflows/
--rw-r--r--   0 spencer   (1000) spencer   (1000)     1385 2023-05-05 21:30:45.000000 mpl-smithchart-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 spencer   (1000) spencer   (1000)     1135 2023-05-05 21:30:45.000000 mpl-smithchart-0.1.0/.gitignore
--rw-r--r--   0 spencer   (1000) spencer   (1000)     1034 2023-05-05 21:30:45.000000 mpl-smithchart-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 spencer   (1000) spencer   (1000)     1457 2023-05-05 21:30:45.000000 mpl-smithchart-0.1.0/COPYING
--rw-r--r--   0 spencer   (1000) spencer   (1000)     4781 2023-05-05 23:05:15.521320 mpl-smithchart-0.1.0/PKG-INFO
--rwxr-xr-x   0 spencer   (1000) spencer   (1000)     4358 2023-05-05 23:00:31.000000 mpl-smithchart-0.1.0/README.md
-drwxr-xr-x   0 spencer   (1000) spencer   (1000)        0 2023-05-05 23:05:15.517987 mpl-smithchart-0.1.0/mpl_smithchart/
--rw-r--r--   0 spencer   (1000) spencer   (1000)      340 2023-05-05 21:55:33.000000 mpl-smithchart-0.1.0/mpl_smithchart/__init__.py
--rw-r--r--   0 spencer   (1000) spencer   (1000)      160 2023-05-05 23:05:15.000000 mpl-smithchart-0.1.0/mpl_smithchart/_version.py
--rw-r--r--   0 spencer   (1000) spencer   (1000)    60665 2023-05-05 22:51:59.000000 mpl-smithchart-0.1.0/mpl_smithchart/smithaxes.py
--rw-r--r--   0 spencer   (1000) spencer   (1000)     1345 2023-05-05 21:56:45.000000 mpl-smithchart-0.1.0/mpl_smithchart/smithhelper.py
-drwxr-xr-x   0 spencer   (1000) spencer   (1000)        0 2023-05-05 23:05:15.517987 mpl-smithchart-0.1.0/mpl_smithchart.egg-info/
--rw-r--r--   0 spencer   (1000) spencer   (1000)     4781 2023-05-05 23:05:15.000000 mpl-smithchart-0.1.0/mpl_smithchart.egg-info/PKG-INFO
--rw-r--r--   0 spencer   (1000) spencer   (1000)      433 2023-05-05 23:05:15.000000 mpl-smithchart-0.1.0/mpl_smithchart.egg-info/SOURCES.txt
--rw-r--r--   0 spencer   (1000) spencer   (1000)        1 2023-05-05 23:05:15.000000 mpl-smithchart-0.1.0/mpl_smithchart.egg-info/dependency_links.txt
--rw-r--r--   0 spencer   (1000) spencer   (1000)       43 2023-05-05 23:05:15.000000 mpl-smithchart-0.1.0/mpl_smithchart.egg-info/requires.txt
--rw-r--r--   0 spencer   (1000) spencer   (1000)       15 2023-05-05 23:05:15.000000 mpl-smithchart-0.1.0/mpl_smithchart.egg-info/top_level.txt
--rw-r--r--   0 spencer   (1000) spencer   (1000)    71338 2023-05-05 23:02:15.000000 mpl-smithchart-0.1.0/pdm.lock
--rw-r--r--   0 spencer   (1000) spencer   (1000)      962 2023-05-05 22:59:12.000000 mpl-smithchart-0.1.0/pyproject.toml
--rw-r--r--   0 spencer   (1000) spencer   (1000)       38 2023-05-05 23:05:15.521320 mpl-smithchart-0.1.0/setup.cfg
-drwxr-xr-x   0 spencer   (1000) spencer   (1000)        0 2023-05-05 23:05:15.521320 mpl-smithchart-0.1.0/tests/
--rw-r--r--   0 spencer   (1000) spencer   (1000)      584 2023-05-05 22:45:11.000000 mpl-smithchart-0.1.0/tests/plotting_test.py
--rw-r--r--   0 spencer   (1000) spencer   (1000)      431 2023-05-05 21:50:24.000000 mpl-smithchart-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.763656 mpl-smithchart-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4358 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/mpl_smithchart/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/mpl_smithchart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60665 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/mpl_smithchart/smithaxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/mpl_smithchart/smithhelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    87334 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 23:32:57.763656 mpl-smithchart-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/tests/plotting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/tox.ini
```

### Comparing `mpl-smithchart-0.1.0/.github/workflows/ci.yml` & `mpl-smithchart-0.1.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   build:
     name: Python ${{matrix.python-version}}
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10']
+        python-version: [3.8, 3.9]
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{matrix.python-version}}
       uses: actions/setup-python@v4
       with:
```

### Comparing `mpl-smithchart-0.1.0/.gitignore` & `mpl-smithchart-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.0/.pre-commit-config.yaml` & `mpl-smithchart-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.0/COPYING` & `mpl-smithchart-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.0/PKG-INFO` & `mpl-smithchart-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mpl-smithchart
-Version: 0.1.0
+Version: 0.1.1
 Summary: An extension for matplotlib providing a projection class to generate high quality Smith Chart plots.
 Author-email: Paul Staerke <paul.staerke@gmail.com>, Spencer Chang <spencer@sycee.xyz>
 License: BSD
 Project-URL: repository, https://github.com/schang412/mpl-smithchart
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # mpl-smithchart
 
 [![ci](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml/badge.svg)](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml)
```

### Comparing `mpl-smithchart-0.1.0/README.md` & `mpl-smithchart-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.0/mpl_smithchart/smithaxes.py` & `mpl-smithchart-0.1.1/mpl_smithchart/smithaxes.py`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.0/mpl_smithchart/smithhelper.py` & `mpl-smithchart-0.1.1/mpl_smithchart/smithhelper.py`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.0/mpl_smithchart.egg-info/PKG-INFO` & `mpl-smithchart-0.1.1/mpl_smithchart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mpl-smithchart
-Version: 0.1.0
+Version: 0.1.1
 Summary: An extension for matplotlib providing a projection class to generate high quality Smith Chart plots.
 Author-email: Paul Staerke <paul.staerke@gmail.com>, Spencer Chang <spencer@sycee.xyz>
 License: BSD
 Project-URL: repository, https://github.com/schang412/mpl-smithchart
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # mpl-smithchart
 
 [![ci](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml/badge.svg)](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml)
```

### Comparing `mpl-smithchart-0.1.0/pdm.lock` & `mpl-smithchart-0.1.1/pdm.lock`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 [[package]]
 name = "colorama"
 version = "0.4.6"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 summary = "Cross-platform colored terminal text."
 
 [[package]]
+name = "contourpy"
+version = "1.0.7"
+requires_python = ">=3.8"
+summary = "Python library for calculating contours of 2D quadrilateral grids"
+dependencies = [
+    "numpy>=1.16",
+]
+
+[[package]]
 name = "cycler"
 version = "0.11.0"
 requires_python = ">=3.6"
 summary = "Composable style cycles"
 
 [[package]]
 name = "exceptiongroup"
@@ -27,78 +36,75 @@
 
 [[package]]
 name = "flake8"
 version = "5.0.4"
 requires_python = ">=3.6.1"
 summary = "the modular source code checker: pep8 pyflakes and co"
 dependencies = [
-    "importlib-metadata<4.3,>=1.1.0; python_version < \"3.8\"",
     "mccabe<0.8.0,>=0.7.0",
     "pycodestyle<2.10.0,>=2.9.0",
     "pyflakes<2.6.0,>=2.5.0",
 ]
 
 [[package]]
 name = "fonttools"
 version = "4.38.0"
 requires_python = ">=3.7"
 summary = "Tools to manipulate font files"
 
 [[package]]
-name = "importlib-metadata"
-version = "4.2.0"
-requires_python = ">=3.6"
-summary = "Read metadata from Python packages"
+name = "importlib-resources"
+version = "5.12.0"
+requires_python = ">=3.7"
+summary = "Read resources from Python packages"
 dependencies = [
-    "typing-extensions>=3.6.4; python_version < \"3.8\"",
-    "zipp>=0.5",
+    "zipp>=3.1.0; python_version < \"3.10\"",
 ]
 
 [[package]]
 name = "iniconfig"
 version = "2.0.0"
 requires_python = ">=3.7"
 summary = "brain-dead simple config-ini parsing"
 
 [[package]]
 name = "kiwisolver"
 version = "1.4.4"
 requires_python = ">=3.7"
 summary = "A fast implementation of the Cassowary constraint solver"
-dependencies = [
-    "typing-extensions; python_version < \"3.8\"",
-]
 
 [[package]]
 name = "matplotlib"
-version = "3.5.3"
-requires_python = ">=3.7"
+version = "3.7.1"
+requires_python = ">=3.8"
 summary = "Python plotting package"
 dependencies = [
+    "contourpy>=1.0.1",
     "cycler>=0.10",
     "fonttools>=4.22.0",
+    "importlib-resources>=3.2.0; python_version < \"3.10\"",
     "kiwisolver>=1.0.1",
-    "numpy>=1.17",
+    "numpy>=1.20",
     "packaging>=20.0",
     "pillow>=6.2.0",
-    "pyparsing>=2.2.1",
+    "pyparsing>=2.3.1",
     "python-dateutil>=2.7",
 ]
 
 [[package]]
 name = "mccabe"
 version = "0.7.0"
 requires_python = ">=3.6"
 summary = "McCabe checker, plugin for flake8"
 
 [[package]]
 name = "numpy"
-version = "1.21.1"
-requires_python = ">=3.7"
-summary = "NumPy is the fundamental package for array computing with Python."
+version = "1.24.3"
+requires_python = ">=3.8"
+summary = "Fundamental package for array computing in Python"
 
 [[package]]
 name = "packaging"
 version = "23.1"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
 
@@ -109,17 +115,14 @@
 summary = "Python Imaging Library (Fork)"
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 requires_python = ">=3.6"
 summary = "plugin and hook calling mechanisms for python"
-dependencies = [
-    "importlib-metadata>=0.12; python_version < \"3.8\"",
-]
 
 [[package]]
 name = "pycodestyle"
 version = "2.9.1"
 requires_python = ">=3.6"
 summary = "Python style guide checker"
 
@@ -139,15 +142,14 @@
 name = "pytest"
 version = "7.3.1"
 requires_python = ">=3.7"
 summary = "pytest: simple powerful testing with Python"
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
-    "importlib-metadata>=0.12; python_version < \"3.8\"",
     "iniconfig",
     "packaging",
     "pluggy<2.0,>=0.12",
     "tomli>=1.0.0; python_version < \"3.11\"",
 ]
 
 [[package]]
@@ -167,19 +169,19 @@
 summary = "Extensions to the standard Python datetime module"
 dependencies = [
     "six>=1.5",
 ]
 
 [[package]]
 name = "scipy"
-version = "1.6.1"
-requires_python = ">=3.7"
-summary = "SciPy: Scientific Library for Python"
+version = "1.9.3"
+requires_python = ">=3.8"
+summary = "Fundamental algorithms for scientific computing in Python"
 dependencies = [
-    "numpy>=1.16.5",
+    "numpy<1.26.0,>=1.18.5",
 ]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Python 2 and 3 compatibility utilities"
@@ -187,35 +189,86 @@
 [[package]]
 name = "tomli"
 version = "2.0.1"
 requires_python = ">=3.7"
 summary = "A lil' TOML parser"
 
 [[package]]
-name = "typing-extensions"
-version = "4.5.0"
-requires_python = ">=3.7"
-summary = "Backported and Experimental Type Hints for Python 3.7+"
-
-[[package]]
 name = "zipp"
 version = "3.15.0"
 requires_python = ">=3.7"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 
 [metadata]
 lock_version = "4.2"
 groups = ["default", "lint", "test"]
-content_hash = "sha256:a14336e9e62f15ff409eed7009ac9d571ecfd4f69814f5d414c7c3d79d223a2d"
+content_hash = "sha256:9a125ef58da72850abdeb9cb9e7a6833d760f203a855b4bf3a9aa49ac01e0ef2"
 
 [metadata.files]
 "colorama 0.4.6" = [
     {url = "https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {url = "https://files.pythonhosted.org/packages/d8/53/6f443c9a4a8358a93a6792e2acffb9d9d5cb0a5cfd8802644b7b1c9a02e4/colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
+"contourpy 1.0.7" = [
+    {url = "https://files.pythonhosted.org/packages/02/4d/009c25f6a3f27dab8fabd5e0f9eeb2bc2697bfcf533e9d07ee825d7fae22/contourpy-1.0.7-cp310-cp310-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f99e9486bf1bb979d95d5cffed40689cb595abb2b841f2991fc894b3452290e8"},
+    {url = "https://files.pythonhosted.org/packages/03/a4/0119e530f7926377d283ed742b120ef5cf3f37f7c5aef5e77cfc59ebabfc/contourpy-1.0.7-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:130230b7e49825c98edf0b428b7aa1125503d91732735ef897786fe5452b1ec2"},
+    {url = "https://files.pythonhosted.org/packages/08/ce/9bfe9f028cb5a8ee97898da52f4905e0e2d9ca8203ffdcdbe80e1769b549/contourpy-1.0.7-cp38-cp38-win_amd64.whl", hash = "sha256:57119b0116e3f408acbdccf9eb6ef19d7fe7baf0d1e9aaa5381489bc1aa56556"},
+    {url = "https://files.pythonhosted.org/packages/09/c4/72ffdbea5f0f2a89e544b5e91793548488b892855c170f89f4b2d8d0597e/contourpy-1.0.7-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:a9d7587d2fdc820cc9177139b56795c39fb8560f540bba9ceea215f1f66e1566"},
+    {url = "https://files.pythonhosted.org/packages/17/22/ae833bbd6ec6dc4b2134d095332dc9853d8ab81c9ced3ec18f1db1942134/contourpy-1.0.7-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5dd34c1ae752515318224cba7fc62b53130c45ac6a1040c8b7c1a223c46e8967"},
+    {url = "https://files.pythonhosted.org/packages/26/df/b5c53b350d9f8c8672fa96a756c12445854be430469a92ca081dfc0f3585/contourpy-1.0.7-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:b8d587cc39057d0afd4166083d289bdeff221ac6d3ee5046aef2d480dc4b503c"},
+    {url = "https://files.pythonhosted.org/packages/2f/e2/02a1b7aa790981af054917154e4c35d5c00fdfaa018b77369758c08918c4/contourpy-1.0.7-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0f9d350b639db6c2c233d92c7f213d94d2e444d8e8fc5ca44c9706cf72193772"},
+    {url = "https://files.pythonhosted.org/packages/30/99/a966df6cb28bab6090527e562682067737c5c6816ffcd7a02812e4a4ffdd/contourpy-1.0.7-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:31a55dccc8426e71817e3fe09b37d6d48ae40aae4ecbc8c7ad59d6893569c436"},
+    {url = "https://files.pythonhosted.org/packages/31/d7/247a889a9c425197aeac5e31286f3050dee63aa3466c939aa302cdb2b6cb/contourpy-1.0.7-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:9e20e5a1908e18aaa60d9077a6d8753090e3f85ca25da6e25d30dc0a9e84c2c6"},
+    {url = "https://files.pythonhosted.org/packages/33/2e/1338f7b7ba17815c00507d0ace2804e37eb85a8c340fd64da5e38690c6d1/contourpy-1.0.7-cp311-cp311-win32.whl", hash = "sha256:4ee3ee247f795a69e53cd91d927146fb16c4e803c7ac86c84104940c7d2cabf0"},
+    {url = "https://files.pythonhosted.org/packages/50/de/28740ce2298fee83d7ce2c935a122c8f38e46b6a904e7533ef32e7206e96/contourpy-1.0.7-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:95c3acddf921944f241b6773b767f1cbce71d03307270e2d769fd584d5d1092d"},
+    {url = "https://files.pythonhosted.org/packages/54/d0/27e77c2028f9df32184427d73f4547d8cb1aca5087e013de1ad414dd3183/contourpy-1.0.7-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:71b0bf0c30d432278793d2141362ac853859e87de0a7dee24a1cea35231f0d50"},
+    {url = "https://files.pythonhosted.org/packages/55/31/be8029093f8b1181f59f4d1f0438a7c60babaf6230947edb387e09ed5c1e/contourpy-1.0.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:fc1464c97579da9f3ab16763c32e5c5d5bb5fa1ec7ce509a4ca6108b61b84fab"},
+    {url = "https://files.pythonhosted.org/packages/59/65/33affcc4d0e1459eaa66f057260076fecd418aa00167f95670e1fbbf597a/contourpy-1.0.7-cp39-cp39-win32.whl", hash = "sha256:c5210e5d5117e9aec8c47d9156d1d3835570dd909a899171b9535cb4a3f32693"},
+    {url = "https://files.pythonhosted.org/packages/59/f6/d1b30d463175af6316e30c45e4618aaabb4d302fd53308fa7d7a62c8f677/contourpy-1.0.7-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:64757f6460fc55d7e16ed4f1de193f362104285c667c112b50a804d482777edd"},
+    {url = "https://files.pythonhosted.org/packages/5a/49/05e1215b1a528db06e4cb84d11aef00f0256ccd7b4a13a9132973e27aa62/contourpy-1.0.7-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:24847601071f740837aefb730e01bd169fbcaa610209779a78db7ebb6e6a7051"},
+    {url = "https://files.pythonhosted.org/packages/63/e6/15b60f93ba888278381cf0cb8f04a988c97f52c3dd235abf9a157b959d79/contourpy-1.0.7-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:abf298af1e7ad44eeb93501e40eb5a67abbf93b5d90e468d01fc0c4451971afa"},
+    {url = "https://files.pythonhosted.org/packages/70/a7/22a5fe12c38e978b941719b04cd81085877eb567165b93358193ec1b3bdc/contourpy-1.0.7-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:ce41676b3d0dd16dbcfabcc1dc46090aaf4688fd6e819ef343dbda5a57ef0161"},
+    {url = "https://files.pythonhosted.org/packages/72/2e/4d50b842a8747776dcd172f9c19514800844d1e67dd1dfdb41c1f74a8b58/contourpy-1.0.7-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:9056c5310eb1daa33fc234ef39ebfb8c8e2533f088bbf0bc7350f70a29bde1ac"},
+    {url = "https://files.pythonhosted.org/packages/81/ac/44b8499389fa3d88fa38fe3301a5b7e22352f1b642cf72f25dc457e9f4b2/contourpy-1.0.7-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:b6d0f9e1d39dbfb3977f9dd79f156c86eb03e57a7face96f199e02b18e58d32a"},
+    {url = "https://files.pythonhosted.org/packages/82/42/6084f3424d47cc47c3eecf926ea2718fcc3cefd5ddd599964f2bccc74b96/contourpy-1.0.7-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:69f8ff4db108815addd900a74df665e135dbbd6547a8a69333a68e1f6e368ac2"},
+    {url = "https://files.pythonhosted.org/packages/82/5b/5eaf7098f38f1b98ed56993e87dd34a5c64e6abff6d4f11394ca2091e600/contourpy-1.0.7-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:6381fa66866b0ea35e15d197fc06ac3840a9b2643a6475c8fff267db8b9f1e69"},
+    {url = "https://files.pythonhosted.org/packages/89/70/b1490db2282e28fef85a29e17ffa976efa621b24e0e36774248805125a5f/contourpy-1.0.7-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:fd7dc0e6812b799a34f6d12fcb1000539098c249c8da54f3566c6a6461d0dbad"},
+    {url = "https://files.pythonhosted.org/packages/8b/f0/eb4bce3032b612a920a044b654164040c3392d3eaa95ec482895815a0f51/contourpy-1.0.7-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:769eef00437edf115e24d87f8926955f00f7704bede656ce605097584f9966dc"},
+    {url = "https://files.pythonhosted.org/packages/8d/cc/c8e32001298b50331348312ac2a965279ddf1c20d25e68ca596fd8a7aaa2/contourpy-1.0.7-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1c71fdd8f1c0f84ffd58fca37d00ca4ebaa9e502fb49825484da075ac0b0b803"},
+    {url = "https://files.pythonhosted.org/packages/8e/d2/38b3da76c0a654dac29f7768a870b930be9a0d35fb469acb86f8d0aaeb54/contourpy-1.0.7-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:efb8f6d08ca7998cf59eaf50c9d60717f29a1a0a09caa46460d33b2924839dbd"},
+    {url = "https://files.pythonhosted.org/packages/95/f1/7e052a263afca2a36417957b7acb56290599458b84135b504dc3ef4ca88d/contourpy-1.0.7-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:366a0cf0fc079af5204801786ad7a1c007714ee3909e364dbac1729f5b0849e5"},
+    {url = "https://files.pythonhosted.org/packages/a5/54/307c937af1875abf17d007e738f244fe128a85f1ac82bbd8876a41b84261/contourpy-1.0.7-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:6c180d89a28787e4b73b07e9b0e2dac7741261dbdca95f2b489c4f8f887dd810"},
+    {url = "https://files.pythonhosted.org/packages/a7/40/0aed6d92734ffad008a841b43723ca0216292df27b706de0afbf7a84dff4/contourpy-1.0.7-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:ed33433fc3820263a6368e532f19ddb4c5990855e4886088ad84fd7c4e561c71"},
+    {url = "https://files.pythonhosted.org/packages/af/5b/1030d528eea1ba29b18681085086ae8c255aada1d38b4809bdc39d4131e0/contourpy-1.0.7-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:031154ed61f7328ad7f97662e48660a150ef84ee1bc8876b6472af88bf5a9b98"},
+    {url = "https://files.pythonhosted.org/packages/b1/5e/9da7dd3f5916f63b7cacb5d13a2eff294b3041cfbae5bc296991df8aa784/contourpy-1.0.7-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:152fd8f730c31fd67fe0ffebe1df38ab6a669403da93df218801a893645c6ccc"},
+    {url = "https://files.pythonhosted.org/packages/b3/0c/0840a89d63cc0866a5118367ae1c789269e350682e6f4aceee5a1f3d608d/contourpy-1.0.7-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:efe99298ba37e37787f6a2ea868265465410822f7bea163edcc1bd3903354ea9"},
+    {url = "https://files.pythonhosted.org/packages/b4/9b/6edb9d3e334a70a212f66a844188fcb57ddbd528cbc3b1fe7abfc317ddd7/contourpy-1.0.7.tar.gz", hash = "sha256:d8165a088d31798b59e91117d1f5fc3df8168d8b48c4acc10fc0df0d0bdbcc5e"},
+    {url = "https://files.pythonhosted.org/packages/b6/4b/18a8a0c4d4f935d3711fe1325d4f0b5277886bcef01ced6ecc45074c3f19/contourpy-1.0.7-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:54d43960d809c4c12508a60b66cb936e7ed57d51fb5e30b513934a4a23874fae"},
+    {url = "https://files.pythonhosted.org/packages/b6/b8/6894c9e851f7442ebbc054537f56021c9ebc0691799ac4b92e380f3a2712/contourpy-1.0.7-cp310-cp310-win_amd64.whl", hash = "sha256:3caea6365b13119626ee996711ab63e0c9d7496f65641f4459c60a009a1f3e80"},
+    {url = "https://files.pythonhosted.org/packages/c4/27/90f82ec9667b3b4fceced99e11c3519879e949ecb74ff976567cf1e5ba7d/contourpy-1.0.7-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:ae90d5a8590e5310c32a7630b4b8618cef7563cebf649011da80874d0aa8f414"},
+    {url = "https://files.pythonhosted.org/packages/c7/97/ba9ace011734cd01b63eb7d39b2cf97afbfa985b0239ab0db85bafa9b207/contourpy-1.0.7-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e7281244c99fd7c6f27c1c6bfafba878517b0b62925a09b586d88ce750a016d2"},
+    {url = "https://files.pythonhosted.org/packages/ca/37/fb73c2052d498f61c2208b5190c209534d2afe89980f6a567e2c0e946304/contourpy-1.0.7-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:30676ca45084ee61e9c3da589042c24a57592e375d4b138bd84d8709893a1ba4"},
+    {url = "https://files.pythonhosted.org/packages/cb/6c/cef46debcbe1cc2072f6367f4430e55331df5776a8d2ee9eb6b33a3d160f/contourpy-1.0.7-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:89ba9bb365446a22411f0673abf6ee1fea3b2cf47b37533b970904880ceb72f3"},
+    {url = "https://files.pythonhosted.org/packages/cc/89/fae9ae6d8e9d1149bed7b0377a4ee77a40293bdd8b681212ab4af2c3fbb2/contourpy-1.0.7-cp310-cp310-win32.whl", hash = "sha256:3c184ad2433635f216645fdf0493011a4667e8d46b34082f5a3de702b6ec42e3"},
+    {url = "https://files.pythonhosted.org/packages/d0/4f/ebdb24671582b56c953f79b6b1261adc0fdf6f7ec8f30cc45efefd5dbcc9/contourpy-1.0.7-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:a1e97b86f73715e8670ef45292d7cc033548266f07d54e2183ecb3c87598888f"},
+    {url = "https://files.pythonhosted.org/packages/d3/b1/e0151100124d28729622bf714462c76b2bce38e136215d9236863d130eb9/contourpy-1.0.7-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:58569c491e7f7e874f11519ef46737cea1d6eda1b514e4eb5ac7dab6aa864d02"},
+    {url = "https://files.pythonhosted.org/packages/d5/d6/6feb6ddca04c3459beaf126a81e5921b944300d5c926e439327590ab26fb/contourpy-1.0.7-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5a011cf354107b47c58ea932d13b04d93c6d1d69b8b6dce885e642531f847566"},
+    {url = "https://files.pythonhosted.org/packages/e0/10/12f2e41e84841a825b31d91c74f64761be470953823b87e340c898dffd92/contourpy-1.0.7-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:7f6979d20ee5693a1057ab53e043adffa1e7418d734c1532e2d9e915b08d8ec2"},
+    {url = "https://files.pythonhosted.org/packages/e3/95/08d6e4c5f53411fdc4ef48b451a6427d68ec761865436e84ab77a0d64db3/contourpy-1.0.7-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:e96a08b62bb8de960d3a6afbc5ed8421bf1a2d9c85cc4ea73f4bc81b4910500f"},
+    {url = "https://files.pythonhosted.org/packages/ea/75/3ed26ede7745109880373de515a273e6dbe43d31960279982fac6d6ddf1d/contourpy-1.0.7-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3e927b3868bd1e12acee7cc8f3747d815b4ab3e445a28d2e5373a7f4a6e76ba1"},
+    {url = "https://files.pythonhosted.org/packages/ea/d6/5be880ae773716ec35863e034d47914de5083cdd2da97fd6c22f84ec9245/contourpy-1.0.7-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cc331c13902d0f50845099434cd936d49d7a2ca76cb654b39691974cb1e4812d"},
+    {url = "https://files.pythonhosted.org/packages/ec/56/7736333adc941087b0f86db37b0dffce83fd4e35400ab86ce1bf0690d04f/contourpy-1.0.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8acf74b5d383414401926c1598ed77825cd530ac7b463ebc2e4f46638f56cce6"},
+    {url = "https://files.pythonhosted.org/packages/ec/59/5eac40e348a7bf803cea221bcd27f74a49cb81667b400fdfbb680e86e7bb/contourpy-1.0.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:87f4d8941a9564cda3f7fa6a6cd9b32ec575830780677932abdec7bcb61717b0"},
+    {url = "https://files.pythonhosted.org/packages/ed/71/546cbcae0cc0653b33afe445a1215f8dddea86f4dd8b31834008588eb8d7/contourpy-1.0.7-cp38-cp38-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2e9ebb4425fc1b658e13bace354c48a933b842d53c458f02c86f371cecbedecc"},
+    {url = "https://files.pythonhosted.org/packages/f2/de/7ddc513caca0e287434cd389855a5d2e185c22685fb1dc6789169dd858be/contourpy-1.0.7-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:a877ada905f7d69b2a31796c4b66e31a8068b37aa9b78832d41c82fc3e056ddd"},
+    {url = "https://files.pythonhosted.org/packages/f3/a9/3640440269719283a250df109a7f91b48d657bf9c0ceb5fe950eb894ecf7/contourpy-1.0.7-cp311-cp311-win_amd64.whl", hash = "sha256:5caeacc68642e5f19d707471890f037a13007feba8427eb7f2a60811a1fc1350"},
+    {url = "https://files.pythonhosted.org/packages/f9/a1/d5c6350a39a2cf221236883d3c6f2b50e3ef5e4f4b7ebf06ee280521a32d/contourpy-1.0.7-cp39-cp39-win_amd64.whl", hash = "sha256:60835badb5ed5f4e194a6f21c09283dd6e007664a86101431bf870d9e86266c4"},
+    {url = "https://files.pythonhosted.org/packages/f9/ca/e9208ba62f5c14d950273d2d4da75aa9f3879809d6813b058514fc5dcccb/contourpy-1.0.7-cp38-cp38-win32.whl", hash = "sha256:62398c80ef57589bdbe1eb8537127321c1abcfdf8c5f14f479dbbe27d0322e66"},
+    {url = "https://files.pythonhosted.org/packages/fa/56/ab73a8bab463df907ac2c2249bfee428900e2b88e28ccf5ab059c106e07c/contourpy-1.0.7-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:38e2e577f0f092b8e6774459317c05a69935a1755ecfb621c0a98f0e3c09c9a5"},
+]
 "cycler 0.11.0" = [
     {url = "https://files.pythonhosted.org/packages/34/45/a7caaacbfc2fa60bee42effc4bcc7d7c6dbe9c349500e04f65a861c15eb9/cycler-0.11.0.tar.gz", hash = "sha256:9c87405839a19696e837b3b818fed3f5f69f16f1eec1a1ad77e043dcea9c772f"},
     {url = "https://files.pythonhosted.org/packages/5c/f9/695d6bedebd747e5eb0fe8fad57b72fdf25411273a39791cde838d5a8f51/cycler-0.11.0-py3-none-any.whl", hash = "sha256:3a27e95f763a428a739d2add979fa7494c912a32c17c4c38c4d5f082cad165a3"},
 ]
 "exceptiongroup 1.1.1" = [
     {url = "https://files.pythonhosted.org/packages/61/97/17ed81b7a8d24d8f69b62c0db37abbd8c0042d4b3fc429c73dab986e7483/exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
     {url = "https://files.pythonhosted.org/packages/cc/38/57f14ddc8e8baeddd8993a36fe57ce7b4ba174c35048b9a6d270bb01e833/exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
@@ -228,17 +281,17 @@
     {url = "https://files.pythonhosted.org/packages/ad/00/9808c62b2d529cefc69ce4e4a1ea42c0f855effa55817b7327ec5b75e60a/flake8-5.0.4.tar.gz", hash = "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db"},
     {url = "https://files.pythonhosted.org/packages/cf/a0/b881b63a17a59d9d07f5c0cc91a29182c8e8a9aa2bde5b3b2b16519c02f4/flake8-5.0.4-py2.py3-none-any.whl", hash = "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"},
 ]
 "fonttools 4.38.0" = [
     {url = "https://files.pythonhosted.org/packages/55/5c/a4a25cf6db42d113d8f626901bb156b2f7cf7c7564a6bbc7b5cd6f7cb484/fonttools-4.38.0.zip", hash = "sha256:2bb244009f9bf3fa100fc3ead6aeb99febe5985fa20afbfbaa2f8946c2fbdaf1"},
     {url = "https://files.pythonhosted.org/packages/e3/d9/e9bae85e84737e76ebbcbea13607236da0c0699baed0ae4f1151b728a608/fonttools-4.38.0-py3-none-any.whl", hash = "sha256:820466f43c8be8c3009aef8b87e785014133508f0de64ec469e4efb643ae54fb"},
 ]
-"importlib-metadata 4.2.0" = [
-    {url = "https://files.pythonhosted.org/packages/22/51/52442c59db26637681148c21f8984eed58c9db67053a0a4783a047010c98/importlib_metadata-4.2.0-py3-none-any.whl", hash = "sha256:057e92c15bc8d9e8109738a48db0ccb31b4d9d5cfbee5a8670879a30be66304b"},
-    {url = "https://files.pythonhosted.org/packages/c7/7c/126a8686399ebe256b5e4343ea80b6f2ee91549969da2eef0bb2891b8d24/importlib_metadata-4.2.0.tar.gz", hash = "sha256:b7e52a1f8dec14a75ea73e0891f3060099ca1d8e6a462a4dff11c3e119ea1b31"},
+"importlib-resources 5.12.0" = [
+    {url = "https://files.pythonhosted.org/packages/38/71/c13ea695a4393639830bf96baea956538ba7a9d06fcce7cef10bfff20f72/importlib_resources-5.12.0-py3-none-any.whl", hash = "sha256:7b1deeebbf351c7578e09bf2f63fa2ce8b5ffec296e0d349139d43cca061a81a"},
+    {url = "https://files.pythonhosted.org/packages/4e/a2/3cab1de83f95dd15297c15bdc04d50902391d707247cada1f021bbfe2149/importlib_resources-5.12.0.tar.gz", hash = "sha256:4be82589bf5c1d7999aedf2a45159d10cb3ca4f19b2271f8792bc8e6da7b22f6"},
 ]
 "iniconfig 2.0.0" = [
     {url = "https://files.pythonhosted.org/packages/d7/4b/cbd8e699e64a6f16ca3a8220661b5f83792b3017d0f79807cb8708d33913/iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
     {url = "https://files.pythonhosted.org/packages/ef/a6/62565a6e1cf69e10f5727360368e451d4b7f58beeac6173dc9db836a5b46/iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
 ]
 "kiwisolver 1.4.4" = [
     {url = "https://files.pythonhosted.org/packages/03/93/11790e8e81b89acd3a1c8a6b501f8a05b1c41beee0990582699cdda29557/kiwisolver-1.4.4-cp37-cp37m-win_amd64.whl", hash = "sha256:03baab2d6b4a54ddbb43bba1a3a2d1627e82d205c5cf8f4c924dc49284b87166"},
@@ -306,84 +359,90 @@
     {url = "https://files.pythonhosted.org/packages/eb/db/b7ebaa2d35f9fb55f3ff8328b5e9dc049f6524dca737cea13e6235ab191d/kiwisolver-1.4.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:10ee06759482c78bdb864f4109886dff7b8a56529bc1609d4f1112b93fe6423c"},
     {url = "https://files.pythonhosted.org/packages/ed/bf/7994af5c838c761b4998044dfabecce8c9f428479e32fe77edc7336dcfd2/kiwisolver-1.4.4-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e0ea21f66820452a3f5d1655f8704a60d66ba1191359b96541eaf457710a5fc6"},
     {url = "https://files.pythonhosted.org/packages/ee/c2/99b2d61dc246844498e68571c589e37ed7a866a4914cb2da2d66d141b596/kiwisolver-1.4.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c79ebe8f3676a4c6630fd3f777f3cfecf9289666c84e775a67d1d358578dc2e3"},
     {url = "https://files.pythonhosted.org/packages/f2/e2/7ed98290955aa83598d0e5672d88bbc193192cdcd23d3a9ed7e536cf8e55/kiwisolver-1.4.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:f0a71d85ecdd570ded8ac3d1c0f480842f49a40beb423bb8014539a9f32a5897"},
     {url = "https://files.pythonhosted.org/packages/f6/e8/194a4b4eee0990a648711bfb769a7110d10fd8d8b370a0464cb3d1060381/kiwisolver-1.4.4-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:70e7c2e7b750585569564e2e5ca9845acfaa5da56ac46df68414f29fea97be9f"},
     {url = "https://files.pythonhosted.org/packages/f8/f4/724d454e95c7e9be6a05f1da3fb85251b5dbb8c3b7d06bdc61d56b16035a/kiwisolver-1.4.4-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:36dafec3d6d6088d34e2de6b85f9d8e2324eb734162fba59d2ba9ed7a2043d5b"},
 ]
-"matplotlib 3.5.3" = [
-    {url = "https://files.pythonhosted.org/packages/02/81/e8276ec6ca005b3b2bfaaad0ea47dbb3a0e389ec8ab87d08e3ccbe4b2742/matplotlib-3.5.3.tar.gz", hash = "sha256:339cac48b80ddbc8bfd05daae0a3a73414651a8596904c2a881cfd1edb65f26c"},
-    {url = "https://files.pythonhosted.org/packages/0a/0e/17a2f293bf37f3ba92600cb2f6bf4a7fd21e96d2101531ddab7e157776ab/matplotlib-3.5.3-cp37-cp37m-win32.whl", hash = "sha256:35a8ad4dddebd51f94c5d24bec689ec0ec66173bf614374a1244c6241c1595e0"},
-    {url = "https://files.pythonhosted.org/packages/29/a1/5a02f43ecc29738867f461df5749fb5ac7fa4c701aed911287266f4e6dfe/matplotlib-3.5.3-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:99482b83ebf4eb6d5fc6813d7aacdefdd480f0d9c0b52dcf9f1cc3b2c4b3361a"},
-    {url = "https://files.pythonhosted.org/packages/2d/19/dc36a8cfa795ceda35b823b3dd13c64258b4ae84a35acd9998efd58d347c/matplotlib-3.5.3-cp38-cp38-win32.whl", hash = "sha256:874df7505ba820e0400e7091199decf3ff1fde0583652120c50cd60d5820ca9a"},
-    {url = "https://files.pythonhosted.org/packages/2d/4a/3262e792d1db92939f820c8fae5ac298b201769e12bb11c89de33ac7bae2/matplotlib-3.5.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:cd45a6f3e93a780185f70f05cf2a383daed13c3489233faad83e81720f7ede24"},
-    {url = "https://files.pythonhosted.org/packages/3d/4e/da8fa069f42ea32858a556b1979c587071d5e82a2b38bf86c24a41c4ec63/matplotlib-3.5.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:3b4fa56159dc3c7f9250df88f653f085068bcd32dcd38e479bba58909254af7f"},
-    {url = "https://files.pythonhosted.org/packages/40/24/a79cbea0d0b6ca64011bfc30cd18069885308e1f1e65772dfc3a15752221/matplotlib-3.5.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6fe807e8a22620b4cd95cfbc795ba310dc80151d43b037257250faf0bfcd82bc"},
-    {url = "https://files.pythonhosted.org/packages/41/6a/b9b170360c408c1cf1515b608fccd7e3e1f4e0b378f6713c2a552a4dab8c/matplotlib-3.5.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:6ea6aef5c4338e58d8d376068e28f80a24f54e69f09479d1c90b7172bad9f25b"},
-    {url = "https://files.pythonhosted.org/packages/60/f6/81c99d3413c18b4810256ac5bca0401c0804e69ea98b448e2c644b745bbb/matplotlib-3.5.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:a206a1b762b39398efea838f528b3a6d60cdb26fe9d58b48265787e29cd1d693"},
-    {url = "https://files.pythonhosted.org/packages/61/1a/584f2e77e2f88239d66314dab14839a199424319df242c783b84ae23ae41/matplotlib-3.5.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:d62880e1f60e5a30a2a8484432bcb3a5056969dc97258d7326ad465feb7ae069"},
-    {url = "https://files.pythonhosted.org/packages/66/c4/70c5d5a4c45a5f642f3609b8b87ef18233e38e08081169a76d19988fe83f/matplotlib-3.5.3-pp37-pypy37_pp73-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:f814504e459c68118bf2246a530ed953ebd18213dc20e3da524174d84ed010b2"},
-    {url = "https://files.pythonhosted.org/packages/69/2a/6cf748ea590bcdc8a35fc9eff57505cae78f4c15035010c10cbe8bb3fae9/matplotlib-3.5.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f3840c280ebc87a48488a46f760ea1c0c0c83fcf7abbe2e6baf99d033fd35fd8"},
-    {url = "https://files.pythonhosted.org/packages/7b/10/70a26ba757ebab35cc8016502ec14c4e51b939a1c62aff5c9b9731417ad1/matplotlib-3.5.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9ab29589cef03bc88acfa3a1490359000c18186fc30374d8aa77d33cc4a51a4a"},
-    {url = "https://files.pythonhosted.org/packages/7f/88/bedb044b6df42c5e68d71df6f4ca9283c98cc4c563af4655d0128a210dfe/matplotlib-3.5.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:73dd93dc35c85dece610cca8358003bf0760d7986f70b223e2306b4ea6d1406b"},
-    {url = "https://files.pythonhosted.org/packages/83/5c/0424da282a8deb4daa6aa530be3f66c9fe8b6eb8236400b06babb6461a99/matplotlib-3.5.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:1e64ac9be9da6bfff0a732e62116484b93b02a0b4d4b19934fb4f8e7ad26ad6a"},
-    {url = "https://files.pythonhosted.org/packages/90/81/b73cb7d615a70a01bd349b8e85a7648c51f3a6346695354c1ce569db6d8f/matplotlib-3.5.3-cp310-cp310-win_amd64.whl", hash = "sha256:2e6d184ebe291b9e8f7e78bbab7987d269c38ea3e062eace1fe7d898042ef804"},
-    {url = "https://files.pythonhosted.org/packages/9e/c8/0cdbaeea02ba50bc9390d9d38d809391d9a477fd571e6e3d8b1f8cfe0a2c/matplotlib-3.5.3-cp39-cp39-win32.whl", hash = "sha256:879c7e5fce4939c6aa04581dfe08d57eb6102a71f2e202e3314d5fbc072fd5a0"},
-    {url = "https://files.pythonhosted.org/packages/a5/0c/e1d675e4f20ddc72497d422344317c227ecdd9e2bd95f4a1c53eeb2cd8e0/matplotlib-3.5.3-cp38-cp38-win_amd64.whl", hash = "sha256:b28de401d928890187c589036857a270a032961411934bdac4cf12dde3d43094"},
-    {url = "https://files.pythonhosted.org/packages/a7/57/c9b314e3c1fe451017e62b9d485c107db1f7b4fed70dc2e13c7acdc57137/matplotlib-3.5.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:b428076a55fb1c084c76cb93e68006f27d247169f056412607c5c88828d08f88"},
-    {url = "https://files.pythonhosted.org/packages/a8/6e/0ee4fdc167173d29d45d2296ed0a1f00ccbe7410a2d10d696970eb0312a0/matplotlib-3.5.3-cp39-cp39-win_amd64.whl", hash = "sha256:ab8d26f07fe64f6f6736d635cce7bfd7f625320490ed5bfc347f2cdb4fae0e56"},
-    {url = "https://files.pythonhosted.org/packages/ad/62/7b662284352867a86acfb636761ba351723fc3a235efd8397578d903413d/matplotlib-3.5.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:94ff86af56a3869a4ae26a9637a849effd7643858a1a04dd5ee50e9ab75069a7"},
-    {url = "https://files.pythonhosted.org/packages/b4/d1/398124bc31d31b57a8a660be90bf5498b703f636c4a33a7180e7e59c3deb/matplotlib-3.5.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:839d47b8ead7ad9669aaacdbc03f29656dc21f0d41a6fea2d473d856c39c8b1c"},
-    {url = "https://files.pythonhosted.org/packages/b6/7b/fd9dc05a486bf3d5a32da454b100269e5afaff3a477f319d6ceefa48e167/matplotlib-3.5.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:3211ba82b9f1518d346f6309df137b50c3dc4421b4ed4815d1d7eadc617f45a1"},
-    {url = "https://files.pythonhosted.org/packages/bf/f6/d0206285a0fc5ef590b5fe940a231cebbe49375c6edd8fd04eaf0489e83c/matplotlib-3.5.3-pp37-pypy37_pp73-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:57f1b4e69f438a99bb64d7f2c340db1b096b41ebaa515cf61ea72624279220ce"},
-    {url = "https://files.pythonhosted.org/packages/c9/99/81f70f1c7a5f61997faacd7756faac6f41d1bda514cb0e29bd4b0d817ff1/matplotlib-3.5.3-cp310-cp310-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2886cc009f40e2984c083687251821f305d811d38e3df8ded414265e4583f0c5"},
-    {url = "https://files.pythonhosted.org/packages/cc/00/cdffb0622cbf31a8a33428f77f8fe22a1509a8be417f40089174c19639f8/matplotlib-3.5.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:bf618a825deb6205f015df6dfe6167a5d9b351203b03fab82043ae1d30f16511"},
-    {url = "https://files.pythonhosted.org/packages/d6/d3/cda19d3864fff82d83604841c0f972cfa7bbd9c759595c854202ad3e97fa/matplotlib-3.5.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0bcdfcb0f976e1bac6721d7d457c17be23cf7501f977b6a38f9d38a3762841f7"},
-    {url = "https://files.pythonhosted.org/packages/dd/3e/15aefbbc4e7c9a4a16700f83e1a69020087c88935c447980e9aeabf67262/matplotlib-3.5.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:22227c976ad4dc8c5a5057540421f0d8708c6560744ad2ad638d48e2984e1dbc"},
-    {url = "https://files.pythonhosted.org/packages/df/3f/6093a23565d0f50ce433f56223fcc34af6c912cd4331dc582ba29d9b5a17/matplotlib-3.5.3-cp37-cp37m-win_amd64.whl", hash = "sha256:43e9d3fa077bf0cc95ded13d331d2156f9973dce17c6f0c8b49ccd57af94dbd9"},
-    {url = "https://files.pythonhosted.org/packages/e1/9c/8330c19f49359b0729cb1b4cbc6a45d29bb2a7526f8318f4e59050e89574/matplotlib-3.5.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:9befa5954cdbc085e37d974ff6053da269474177921dd61facdad8023c4aeb51"},
-    {url = "https://files.pythonhosted.org/packages/e5/ca/3ed0e1de9df496392a4c9d75b0c78f82fe5758c66bb875903cf7a9402f0b/matplotlib-3.5.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c995f7d9568f18b5db131ab124c64e51b6820a92d10246d4f2b3f3a66698a15b"},
-    {url = "https://files.pythonhosted.org/packages/e8/f7/12fdec2c9cdd06a406f1ba4f08b5fe94bbefc800a4c6e5fa3feda0dc1d16/matplotlib-3.5.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:dacddf5bfcec60e3f26ec5c0ae3d0274853a258b6c3fc5ef2f06a8eb23e042be"},
-    {url = "https://files.pythonhosted.org/packages/ec/13/78e0de82272ee6a24e5cf13469234accfc07cf08638477e8c516573b2a3e/matplotlib-3.5.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:5c096363b206a3caf43773abebdbb5a23ea13faef71d701b21a9c27fdcef72f4"},
-    {url = "https://files.pythonhosted.org/packages/fd/1c/5c3c71e38a408f2034ae08db6b71e7d1010f9461ab05d8b30b136a77b3e1/matplotlib-3.5.3-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:d2484b350bf3d32cae43f85dcfc89b3ed7bd2bcd781ef351f93eb6fb2cc483f9"},
-    {url = "https://files.pythonhosted.org/packages/fd/7e/ecd6784f82baa01ef7859f8093be02b0913bda487b5bdc4da23c14041f9c/matplotlib-3.5.3-cp310-cp310-win32.whl", hash = "sha256:6bb93a0492d68461bd458eba878f52fdc8ac7bdb6c4acdfe43dba684787838c2"},
+"matplotlib 3.7.1" = [
+    {url = "https://files.pythonhosted.org/packages/05/92/8a7449693adc4480a4777b407b44d21c0c6e3d2ace3250091fe1a89bc825/matplotlib-3.7.1-cp39-cp39-win_amd64.whl", hash = "sha256:3ba2af245e36990facf67fde840a760128ddd71210b2ab6406e640188d69d136"},
+    {url = "https://files.pythonhosted.org/packages/07/67/0d84ca088fa164ac9ad9bf1a896517ee9eeb98a27a315e1bcad619cde30c/matplotlib-3.7.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:3032884084f541163f295db8a6536e0abb0db464008fadca6c98aaf84ccf4717"},
+    {url = "https://files.pythonhosted.org/packages/07/76/fde990f131450f08eb06e50814b98d347b14d7916c0ec31cba0a65a9be2b/matplotlib-3.7.1-cp310-cp310-win_amd64.whl", hash = "sha256:3d7bc90727351fb841e4d8ae620d2d86d8ed92b50473cd2b42ce9186104ecbba"},
+    {url = "https://files.pythonhosted.org/packages/0e/61/255b0ab4fd319bb8274bde67eeb8b56e52c4d1b66123a6ed3de2b835d108/matplotlib-3.7.1-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:f67bfdb83a8232cb7a92b869f9355d677bce24485c460b19d01970b64b2ed476"},
+    {url = "https://files.pythonhosted.org/packages/10/94/36527e47d0719e7ae3649cc290a4d0b5faeac3453867cdf633f4b2480d87/matplotlib-3.7.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:438196cdf5dc8d39b50a45cb6e3f6274edbcf2254f85fa9b895bf85851c3a613"},
+    {url = "https://files.pythonhosted.org/packages/13/0d/a3c01d8dd48957029f5ea5eac3d778fdedefaef43533597def65e29e5414/matplotlib-3.7.1-cp310-cp310-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e99bc9e65901bb9a7ce5e7bb24af03675cbd7c70b30ac670aa263240635999a4"},
+    {url = "https://files.pythonhosted.org/packages/16/23/d81f74e722eb064e726e7b6da999fd9e50de13b28e6496d67e9f09b6fe19/matplotlib-3.7.1-cp38-cp38-macosx_10_12_x86_64.whl", hash = "sha256:cf0e4f727534b7b1457898c4f4ae838af1ef87c359b76dcd5330fa31893a3ac7"},
+    {url = "https://files.pythonhosted.org/packages/18/70/31f7b317e5575b590ed7227a9c3d6f42f8e8838ce7d5e763ff16440ac1d4/matplotlib-3.7.1-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:8704726d33e9aa8a6d5215044b8d00804561971163563e6e6591f9dcf64340cc"},
+    {url = "https://files.pythonhosted.org/packages/1d/24/72b0b7069d268b22c40f42d973f4b4971debd0f9ddc0fbf4753d5f0a2469/matplotlib-3.7.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:544764ba51900da4639c0f983b323d288f94f65f4024dc40ecb1542d74dc0500"},
+    {url = "https://files.pythonhosted.org/packages/1e/5c/bae8d15f7dec470ee0269d503132678e5ce4abd1306b70b180d66ede13d5/matplotlib-3.7.1-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:83111e6388dec67822e2534e13b243cc644c7494a4bb60584edbff91585a83c6"},
+    {url = "https://files.pythonhosted.org/packages/23/7c/3e9366cf2259785de934d0bb5a7e03828e23cd722439d1c78abc4b7d89eb/matplotlib-3.7.1-cp311-cp311-macosx_10_12_universal2.whl", hash = "sha256:770a205966d641627fd5cf9d3cb4b6280a716522cd36b8b284a8eb1581310f61"},
+    {url = "https://files.pythonhosted.org/packages/34/b3/c81bbb3de820e0eaba4d7d41b9df34ffdc3336159de5bb6c959cd2028670/matplotlib-3.7.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b867e2f952ed592237a1828f027d332d8ee219ad722345b79a001f49df0936eb"},
+    {url = "https://files.pythonhosted.org/packages/35/a8/eb84f46e133fc0be5d50c3e1bec0aaa18a58bb53fc9ea96797289ffb2cd2/matplotlib-3.7.1-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3a2cb34336110e0ed8bb4f650e817eed61fa064acbefeb3591f1b33e3a84fd96"},
+    {url = "https://files.pythonhosted.org/packages/3a/4e/83499803b641c40e33c118b461a7c110bfa8cc6b3be10a2dc174232522dd/matplotlib-3.7.1-cp311-cp311-win32.whl", hash = "sha256:fbdeeb58c0cf0595efe89c05c224e0a502d1aa6a8696e68a73c3efc6bc354304"},
+    {url = "https://files.pythonhosted.org/packages/4d/71/a0d28c6123773075f056ff2ce7b2a16a19a4ff2982f0de0f285c9866c420/matplotlib-3.7.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8bf26ade3ff0f27668989d98c8435ce9327d24cffb7f07d24ef609e33d582439"},
+    {url = "https://files.pythonhosted.org/packages/51/3e/2e266434cf7aa82ab5d860b774a1ece49debffa3f5c32f7c6e305f0f5728/matplotlib-3.7.1-cp38-cp38-win32.whl", hash = "sha256:7c9a4b2da6fac77bcc41b1ea95fadb314e92508bf5493ceff058e727e7ecf5b0"},
+    {url = "https://files.pythonhosted.org/packages/51/d8/ba69105b4b72aace5d3501af1b0886b248fa5363519df04dc17577578bab/matplotlib-3.7.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a867bf73a7eb808ef2afbca03bcdb785dae09595fbe550e1bab0cd023eba3de0"},
+    {url = "https://files.pythonhosted.org/packages/5c/b0/050bcf86c57255066915eb805d36409e2e093a07d4615249b07aa2530ef5/matplotlib-3.7.1-cp38-cp38-macosx_10_12_universal2.whl", hash = "sha256:6eb88d87cb2c49af00d3bbc33a003f89fd9f78d318848da029383bfc08ecfbfb"},
+    {url = "https://files.pythonhosted.org/packages/5d/22/f55638bea4af17edf23e1c919ad5d256141bbeec0196c450be9785f1dcb6/matplotlib-3.7.1-cp38-cp38-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:4cf327e98ecf08fcbb82685acaf1939d3338548620ab8dfa02828706402c34de"},
+    {url = "https://files.pythonhosted.org/packages/5d/7e/0647f19705d819d2249df96625d83ff5de2e913a247610b753c504b7bfd0/matplotlib-3.7.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:2bf092f9210e105f414a043b92af583c98f50050559616930d884387d0772aba"},
+    {url = "https://files.pythonhosted.org/packages/62/6d/3817522ca223796703b68ffd38577582f2dc7a0c0dd410d1803e36b5e1db/matplotlib-3.7.1-cp310-cp310-macosx_10_12_universal2.whl", hash = "sha256:95cbc13c1fc6844ab8812a525bbc237fa1470863ff3dace7352e910519e194b1"},
+    {url = "https://files.pythonhosted.org/packages/6c/70/5f8b981680fc0bdb85f0dd00174e41f98d4cdb641921295822c8e14272fe/matplotlib-3.7.1-cp39-cp39-macosx_10_12_x86_64.whl", hash = "sha256:28506a03bd7f3fe59cd3cd4ceb2a8d8a2b1db41afede01f66c42561b9be7b4b7"},
+    {url = "https://files.pythonhosted.org/packages/80/c0/1d29eafc057e516ffc1ba07da2054926f219c44ad4ea5df57ff97825182c/matplotlib-3.7.1-cp39-cp39-macosx_10_12_universal2.whl", hash = "sha256:81a6b377ea444336538638d31fdb39af6be1a043ca5e343fe18d0f17e098770b"},
+    {url = "https://files.pythonhosted.org/packages/81/f7/1c9145e24195723da3cb668637b98b6016be4692b335ba543058a7297c9e/matplotlib-3.7.1-cp39-cp39-win32.whl", hash = "sha256:4f99e1b234c30c1e9714610eb0c6d2f11809c9c78c984a613ae539ea2ad2eb4b"},
+    {url = "https://files.pythonhosted.org/packages/83/3e/08d551274d660cd38af04b14366725c195f18ad0bd359e192ecf3ec2f2bb/matplotlib-3.7.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:97cc368a7268141afb5690760921765ed34867ffb9655dd325ed207af85c7529"},
+    {url = "https://files.pythonhosted.org/packages/86/2b/a04f22015a03025a8c9c0363c4ecfd89eb45fc3af545ff838e02ac58b39d/matplotlib-3.7.1-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:08308bae9e91aca1ec6fd6dda66237eef9f6294ddb17f0d0b3c863169bf82353"},
+    {url = "https://files.pythonhosted.org/packages/89/f3/84a9a6613ab0d89931d785f13fa2606e03f07252875acc8ebf5b676fa3c5/matplotlib-3.7.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eb7d248c34a341cd4c31a06fd34d64306624c8cd8d0def7abb08792a5abfd556"},
+    {url = "https://files.pythonhosted.org/packages/8a/d3/35c62c9f64ddef5f25763580a10cb1ff4a19dc1a2bf940ad06dbb10b248d/matplotlib-3.7.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:56d94989191de3fcc4e002f93f7f1be5da476385dde410ddafbb70686acf00ea"},
+    {url = "https://files.pythonhosted.org/packages/91/ae/410dca50b2b0b4d48bfaa41a20d7344078ac63a7178d3b5716b1014c90b9/matplotlib-3.7.1-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:21e9cff1a58d42e74d01153360de92b326708fb205250150018a52c70f43c290"},
+    {url = "https://files.pythonhosted.org/packages/92/01/2c04d328db6955d77f8f60c17068dde8aa66f153b2c599ca03c2cb0d5567/matplotlib-3.7.1-cp38-cp38-win_amd64.whl", hash = "sha256:14645aad967684e92fc349493fa10c08a6da514b3d03a5931a1bac26e6792bd1"},
+    {url = "https://files.pythonhosted.org/packages/9f/77/0cd22f92f7103383cb1ce3b3efc77411b9cc3a495242c8f2a623b498f586/matplotlib-3.7.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f883a22a56a84dba3b588696a2b8a1ab0d2c3d41be53264115c71b0a942d8fdb"},
+    {url = "https://files.pythonhosted.org/packages/a8/14/83b722ae5bec25cd1b44067d2165952aa0943af287ea06f2e1e594220805/matplotlib-3.7.1-cp310-cp310-win32.whl", hash = "sha256:ce463ce590f3825b52e9fe5c19a3c6a69fd7675a39d589e8b5fbe772272b3a24"},
+    {url = "https://files.pythonhosted.org/packages/b7/65/d6e00376dbdb6c227d79a2d6ec32f66cfb163f0cd924090e3133a4f85a11/matplotlib-3.7.1.tar.gz", hash = "sha256:7b73305f25eab4541bd7ee0b96d87e53ae9c9f1823be5659b806cd85786fe882"},
+    {url = "https://files.pythonhosted.org/packages/b7/ed/32d00261ac6067b13af9181b2450d30599875ab61807defa85c05a28432a/matplotlib-3.7.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:57bfb8c8ea253be947ccb2bc2d1bb3862c2bccc662ad1b4626e1f5e004557042"},
+    {url = "https://files.pythonhosted.org/packages/bc/22/52dd9b0f8da380309ceb4c5e6a9018417b56ad3b56bfd18fe0e1d1310541/matplotlib-3.7.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:617f14ae9d53292ece33f45cba8503494ee199a75b44de7717964f70637a36aa"},
+    {url = "https://files.pythonhosted.org/packages/bd/5d/a9083be15f9bed89c1c5897473eae6dd1bab4acbcfb82fdae417149674d0/matplotlib-3.7.1-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:def58098f96a05f90af7e92fd127d21a287068202aa43b2a93476170ebd99e87"},
+    {url = "https://files.pythonhosted.org/packages/cf/2c/41b330eeb47806abc19c1a4ab22821cb5a2be2cabe34c37f0d8483ae0e26/matplotlib-3.7.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75d4725d70b7c03e082bbb8a34639ede17f333d7247f56caceb3801cb6ff703d"},
+    {url = "https://files.pythonhosted.org/packages/e0/2e/a9fc4c317bc8cc679d344dd881b97f67580b38e6eedc645c3623d6c5d139/matplotlib-3.7.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:89768d84187f31717349c6bfadc0e0d8c321e8eb34522acec8a67b1236a66332"},
+    {url = "https://files.pythonhosted.org/packages/e8/5a/2661b38ebd4b1d58f335be7e8150af0a7eb94d13bf7a6563e7c49ed40c4d/matplotlib-3.7.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:8c587963b85ce41e0a8af53b9b2de8dddbf5ece4c34553f7bd9d066148dc719c"},
+    {url = "https://files.pythonhosted.org/packages/f3/99/7010ae81984908cc655b7d24145aeed2784614957ed7f0cb5a72b17a63d3/matplotlib-3.7.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:46a561d23b91f30bccfd25429c3c706afe7d73a5cc64ef2dfaf2b2ac47c1a5dc"},
+    {url = "https://files.pythonhosted.org/packages/fb/8c/391e3c105edb7e193bb163ed48988135228d0b5ce3143e1cbec2350e23c8/matplotlib-3.7.1-cp311-cp311-win_amd64.whl", hash = "sha256:c0bd19c72ae53e6ab979f0ac6a3fafceb02d2ecafa023c5cca47acd934d10be7"},
 ]
 "mccabe 0.7.0" = [
     {url = "https://files.pythonhosted.org/packages/27/1a/1f68f9ba0c207934b35b86a8ca3aad8395a3d6dd7921c0686e23853ff5a9/mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {url = "https://files.pythonhosted.org/packages/e7/ff/0ffefdcac38932a54d2b5eed4e0ba8a408f215002cd178ad1df0f2806ff8/mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
-"numpy 1.21.1" = [
-    {url = "https://files.pythonhosted.org/packages/0b/a7/e724c8df240687b5fd62d8c71f1a6709d455c4c09432c7412e3e64f4cbe5/numpy-1.21.1.zip", hash = "sha256:dff4af63638afcc57a3dfb9e4b26d434a7a602d225b42d746ea7fe2edf1342fd"},
-    {url = "https://files.pythonhosted.org/packages/0d/fc/2a55c4d690437e09e44f40fe7a8458a72aef9da01719bd8746002999f782/numpy-1.21.1-cp38-cp38-win_amd64.whl", hash = "sha256:9749a40a5b22333467f02fe11edc98f022133ee1bfa8ab99bda5e5437b831214"},
-    {url = "https://files.pythonhosted.org/packages/16/c9/71124564deb3fd4c7572d7aa830482e8901eb84938f3629185abff60d911/numpy-1.21.1-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:95b995d0c413f5d0428b3f880e8fe1660ff9396dcd1f9eedbc311f37b5652e16"},
-    {url = "https://files.pythonhosted.org/packages/1e/69/75d67f070446c87199f7a5aaff2504b4124bedcdcdf30da5f6de0c9e8e89/numpy-1.21.1-cp39-cp39-win32.whl", hash = "sha256:88c0b89ad1cc24a5efbb99ff9ab5db0f9a86e9cc50240177a571fbe9c2860ac2"},
-    {url = "https://files.pythonhosted.org/packages/1e/f4/a7bcb5942458656882195d71df967bc74c01452cb445c10c23c40ca6a8ef/numpy-1.21.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:635e6bd31c9fb3d475c8f44a089569070d10a9ef18ed13738b03049280281267"},
-    {url = "https://files.pythonhosted.org/packages/2b/15/7c686607db98f151dc2dadcdc4dd9ed39950e8f29d712d3e42b44d1202e5/numpy-1.21.1-cp39-cp39-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:05a0f648eb28bae4bcb204e6fd14603de2908de982e761a2fc78efe0f19e96e1"},
-    {url = "https://files.pythonhosted.org/packages/31/88/e67fb244cf5998c1e8fa5eda670ae8265ae0beed0346d5a424cb612fee24/numpy-1.21.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:25b40b98ebdd272bc3020935427a4530b7d60dfbe1ab9381a39147834e985eac"},
-    {url = "https://files.pythonhosted.org/packages/3b/11/445c95be2f846be94d2425f8f1f4c9ad2bcbbb9ad425c8a9f7394f325bdb/numpy-1.21.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:9a513bd9c1551894ee3d31369f9b07460ef223694098cf27d399513415855b68"},
-    {url = "https://files.pythonhosted.org/packages/45/51/716a08ed750c660ed20edccd22aeeb8c2653c4f6e92dc8b8b0dcf9ff432a/numpy-1.21.1-cp38-cp38-win32.whl", hash = "sha256:978010b68e17150db8765355d1ccdd450f9fc916824e8c4e35ee620590e234cd"},
-    {url = "https://files.pythonhosted.org/packages/49/d2/057683bbe4f8cccbd74f9b98dee5b1c5b94c06c115790d4bb50ec31aab77/numpy-1.21.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:38e8648f9449a549a7dfe8d8755a5979b45b3538520d1e735637ef28e8c2dc50"},
-    {url = "https://files.pythonhosted.org/packages/50/9a/54c6c2da63830939bef8be068aece1ac04859fc51428710ad5cd148566fc/numpy-1.21.1-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:e46ceaff65609b5399163de5893d8f2a82d3c77d5e56d976c8b5fb01faa6b671"},
-    {url = "https://files.pythonhosted.org/packages/60/5b/97dcc2561db2b78201e61fe9e08c39f7ec9edbe412aa70f2fcf65c2813a8/numpy-1.21.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:d9e7912a56108aba9b31df688a4c4f5cb0d9d3787386b87d504762b6754fbb1b"},
-    {url = "https://files.pythonhosted.org/packages/65/4c/194a2f8b8c94f4d401a31a5a0516906829e7ead6f05b0647076680c3f36d/numpy-1.21.1-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:8a92c5aea763d14ba9d6475803fc7904bda7decc2a0a68153f587ad82941fec1"},
-    {url = "https://files.pythonhosted.org/packages/73/3e/e8b555c1230c63ef2e0dbf42fbcb4c2d1444bd5ec8e7eebcff904b922df4/numpy-1.21.1-cp37-cp37m-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:fd7d7409fa643a91d0a05c7554dd68aa9c9bb16e186f6ccfe40d6e003156e33a"},
-    {url = "https://files.pythonhosted.org/packages/87/18/608e04350d78bb3201a8ac2777b9a77e024218ec2a7f64db9b7130c714fc/numpy-1.21.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1412aa0aec3e00bc23fbb8664d76552b4efde98fb71f60737c83efbac24112f1"},
-    {url = "https://files.pythonhosted.org/packages/95/7a/da016166264ccc417f58ba097c3cfa995b77e87d2d3c5424c9e5dfffa68d/numpy-1.21.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0318c465786c1f63ac05d7c4dbcecd4d2d7e13f0959b01b534ea1e92202235c5"},
-    {url = "https://files.pythonhosted.org/packages/99/60/7b97b75a121745508a2fd92b5127dc0fe080d026d43b0fcf2863ea50c074/numpy-1.21.1-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:d7a4aeac3b94af92a9373d6e77b37691b86411f9745190d2c351f410ab3a791f"},
-    {url = "https://files.pythonhosted.org/packages/9a/ee/07eb4eb76620d95af51f16481dca8b9d1e1d9edae8cf60d5143aad270764/numpy-1.21.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:91c6f5fc58df1e0a3cc0c3a717bb3308ff850abdaa6d2d802573ee2b11f674a8"},
-    {url = "https://files.pythonhosted.org/packages/9f/4a/fc96aecce86b0e892a574680305f9d865c9845d1ca512a936c676f3c9f8b/numpy-1.21.1-cp37-cp37m-win32.whl", hash = "sha256:73101b2a1fef16602696d133db402a7e7586654682244344b8329cdcbbb82172"},
-    {url = "https://files.pythonhosted.org/packages/a0/3a/ffacce6c7d7d980a4aebb51cacf91e1443d4317aa29630c7d3054fb64e2e/numpy-1.21.1-cp38-cp38-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:791492091744b0fe390a6ce85cc1bf5149968ac7d5f0477288f78c89b385d9af"},
-    {url = "https://files.pythonhosted.org/packages/b8/46/3f1a1a1f5fa3c0325a407a98396b8ac90e4eaa058420668b4b640729c784/numpy-1.21.1-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:c6a2324085dd52f96498419ba95b5777e40b6bcbc20088fddb9e8cbb58885e8e"},
-    {url = "https://files.pythonhosted.org/packages/b8/98/1deff46537aa544bd6ffafb4405d0f57fe49308147444e27ab2fc3ca82ba/numpy-1.21.1-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:8a326af80e86d0e9ce92bcc1e65c8ff88297de4fa14ee936cb2293d414c9ec63"},
-    {url = "https://files.pythonhosted.org/packages/bf/03/bb8a4c7b5a69795e61a21459d1ff1c0730ef0faa1f3dfff525b7c4132347/numpy-1.21.1-cp39-cp39-win_amd64.whl", hash = "sha256:01721eefe70544d548425a07c80be8377096a54118070b8a62476866d5208e33"},
-    {url = "https://files.pythonhosted.org/packages/ce/73/465ec13dd21a4d66f96e7b8aca027ca965d639654268dba03c1e37f15d03/numpy-1.21.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f01f28075a92eede918b965e86e8f0ba7b7797a95aa8d35e1cc8821f5fc3ad6a"},
-    {url = "https://files.pythonhosted.org/packages/d3/6d/f53d9806d307e5d3ef0bb594d9f2236d61cb0f3c7b17edb4f0af69f0585f/numpy-1.21.1-pp37-pypy37_pp73-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:2d4d1de6e6fb3d28781c73fbde702ac97f03d79e4ffd6598b880b2d95d62ead4"},
-    {url = "https://files.pythonhosted.org/packages/de/4b/5b243d909933c387bb5253a91706a7aa49b0550147e0b144b0f8a842e0f0/numpy-1.21.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4a3d5fb89bfe21be2ef47c0614b9c9c707b7362386c9a3ff1feae63e0267ccb6"},
-    {url = "https://files.pythonhosted.org/packages/eb/a9/1e4215043cac5ffc6a5ab1f2e0e58a680fc8fd19e28eb28c01e90aeace3e/numpy-1.21.1-cp37-cp37m-win_amd64.whl", hash = "sha256:7a708a79c9a9d26904d1cca8d383bf869edf6f8e7650d85dbc77b041e8c5a0f8"},
-    {url = "https://files.pythonhosted.org/packages/f9/d5/18336e9828d2f07beb0bcd3849c660001bedea50e6219627315968900ad6/numpy-1.21.1-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:a75b4498b1e93d8b700282dc8e655b8bd559c0904b3910b144646dbbbc03e062"},
+"numpy 1.24.3" = [
+    {url = "https://files.pythonhosted.org/packages/0d/43/643629a4a278b4815541c7d69856c07ddb0e99bdc62b43538d3751eae2d8/numpy-1.24.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4719d5aefb5189f50887773699eaf94e7d1e02bf36c1a9d353d9f46703758ca4"},
+    {url = "https://files.pythonhosted.org/packages/15/b8/cbe1750b9ec78062e5a00ef39ff8bdf189ce753b411b6b35931ababaee47/numpy-1.24.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:35400e6a8d102fd07c71ed7dcadd9eb62ee9a6e84ec159bd48c28235bbb0f8e4"},
+    {url = "https://files.pythonhosted.org/packages/1a/62/af7e78a12207608b23e3b2e248fc823fbef75f17d5defc8a127c5661daca/numpy-1.24.3-cp38-cp38-win_amd64.whl", hash = "sha256:56e48aec79ae238f6e4395886b5eaed058abb7231fb3361ddd7bfdf4eed54289"},
+    {url = "https://files.pythonhosted.org/packages/2c/d4/590ae7df5044465cc9fa2db152ae12468694d62d952b1528ecff328ef7fc/numpy-1.24.3.tar.gz", hash = "sha256:ab344f1bf21f140adab8e47fdbc7c35a477dc01408791f8ba00d018dd0bc5155"},
+    {url = "https://files.pythonhosted.org/packages/53/f7/bf6e2b973c6d6a4c60f722dd95322d4997b4999347d67c5c74a4042a07b7/numpy-1.24.3-cp38-cp38-win32.whl", hash = "sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4"},
+    {url = "https://files.pythonhosted.org/packages/54/41/fb17c1d48a574c50422ff3f1b17ed979b755adc6ed291c4a44a76e226c67/numpy-1.24.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187"},
+    {url = "https://files.pythonhosted.org/packages/5a/ab/d0eff89e0c05cc86fa7955c5e54e8ed0957a8a97a2516384b9ffd82008cc/numpy-1.24.3-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:352ee00c7f8387b44d19f4cada524586f07379c0d49270f87233983bc5087ca0"},
+    {url = "https://files.pythonhosted.org/packages/62/e4/cd77d5f3d02c30d9ca8f2995df3cb3974c75cf1cc777fad445753475c4e4/numpy-1.24.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8535303847b89aa6b0f00aa1dc62867b5a32923e4d1681a35b5eef2d9591a463"},
+    {url = "https://files.pythonhosted.org/packages/65/5d/46da284b0bf6cfbf04082c3c5e84399664d69e41c11a33587ad49b0c64e5/numpy-1.24.3-cp310-cp310-win_amd64.whl", hash = "sha256:ab5f23af8c16022663a652d3b25dcdc272ac3f83c3af4c02eb8b824e6b3ab9d7"},
+    {url = "https://files.pythonhosted.org/packages/6f/72/38f9a536bdb5bfb1682f2520f133ec6e08dde8bcca1f632e347641d90763/numpy-1.24.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2d926b52ba1367f9acb76b0df6ed21f0b16a1ad87c6720a1121674e5cf63e2b6"},
+    {url = "https://files.pythonhosted.org/packages/72/eb/9c77bbc4d2b4ca17ef253621794a2d42897d896f86cd493db3eabe1a7d25/numpy-1.24.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:76e3f4e85fc5d4fd311f6e9b794d0c00e7002ec122be271f2019d63376f1d385"},
+    {url = "https://files.pythonhosted.org/packages/76/7c/cfb8ac4925defbe222aec15ac6b42b2a3d9bab7c9d13a2e767f534b35c2e/numpy-1.24.3-cp39-cp39-win_amd64.whl", hash = "sha256:d5036197ecae68d7f491fcdb4df90082b0d4960ca6599ba2659957aafced7c17"},
+    {url = "https://files.pythonhosted.org/packages/79/4a/63a79242763edde0b5025d104cc2b78c44d89310b1bbc9b0f64a96b72ea0/numpy-1.24.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:7776ea65423ca6a15255ba1872d82d207bd1e09f6d0894ee4a64678dd2204078"},
+    {url = "https://files.pythonhosted.org/packages/82/19/321d369ede7458500f59151101470129d14f3b6768bb9b99bb7156f526b5/numpy-1.24.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a1d3c026f57ceaad42f8231305d4653d5f05dc6332a730ae5c0bea3513de0950"},
+    {url = "https://files.pythonhosted.org/packages/83/be/de078ac5e4ff572b1bdac1808b77cea2013b2c6286282f89b1de3e951273/numpy-1.24.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4"},
+    {url = "https://files.pythonhosted.org/packages/89/e3/e2f478b2ff131e7c3171044a87e74df61db4b67fbcb90be479c07a44d0a7/numpy-1.24.3-cp310-cp310-win32.whl", hash = "sha256:f21c442fdd2805e91799fbe044a7b999b8571bb0ab0f7850d0cb9641a687092b"},
+    {url = "https://files.pythonhosted.org/packages/8b/d9/814a619ab84d8eb0d95e08d4c723e665f1e694b5a6068ca505a61bdc3745/numpy-1.24.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4749e053a29364d3452c034827102ee100986903263e89884922ef01a0a6fd2f"},
+    {url = "https://files.pythonhosted.org/packages/94/84/ed45416c8319c02348a5812d5647796a0833e3fb5576d01758f2a72e9200/numpy-1.24.3-cp311-cp311-win32.whl", hash = "sha256:c91c4afd8abc3908e00a44b2672718905b8611503f7ff87390cc0ac3423fb096"},
+    {url = "https://files.pythonhosted.org/packages/96/92/2a8c1356e226311cf885e04eff576df8c357b2626c47c9283024bc24e01e/numpy-1.24.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ea8282b9bcfe2b5e7d491d0bf7f3e2da29700cec05b49e64d6246923329f2b02"},
+    {url = "https://files.pythonhosted.org/packages/a7/fe/72493149c65dcd39d8c8dc09870e242bd689d1db2bde3ec479807bf0d414/numpy-1.24.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ecde0f8adef7dfdec993fd54b0f78183051b6580f606111a6d789cd14c61ea0c"},
+    {url = "https://files.pythonhosted.org/packages/ca/13/c5bc0100b425f007412c3ba5d71e5ae9c08260fecbffd620764a9df1f4de/numpy-1.24.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:ae8d0be48d1b6ed82588934aaaa179875e7dc4f3d84da18d7eae6eb3f06c242c"},
+    {url = "https://files.pythonhosted.org/packages/d5/d6/07b37e7fecad7d158aabb4782a1b941e10afe8b80ec24cd64285a5bbb81b/numpy-1.24.3-cp39-cp39-win32.whl", hash = "sha256:784c6da1a07818491b0ffd63c6bbe5a33deaa0e25a20e1b3ea20cf0e43f8046c"},
+    {url = "https://files.pythonhosted.org/packages/eb/10/2c3c672034d860bcca50b65d656e24c4e2ace9fb452fdd81da78cb7418a1/numpy-1.24.3-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812"},
+    {url = "https://files.pythonhosted.org/packages/ec/7d/f69c47ea3db0cd8ca444aec241a80b538eb176ae756820489a9d2946ec8c/numpy-1.24.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:9a7721ec204d3a237225db3e194c25268faf92e19338a35f3a224469cb6039a3"},
+    {url = "https://files.pythonhosted.org/packages/ee/6c/7217a8844dfe22e349bccbecd35571fa72c5d7fe8b33d8c5540e8cc2535c/numpy-1.24.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d6cc757de514c00b24ae8cf5c876af2a7c3df189028d68c0cb4eaa9cd5afc2bf"},
+    {url = "https://files.pythonhosted.org/packages/f0/e8/1ea9adebdccaadfc208c7517e09f5145ed5a73069779ff436393085d47a2/numpy-1.24.3-cp311-cp311-win_amd64.whl", hash = "sha256:5342cf6aad47943286afa6f1609cad9b4266a05e7f2ec408e2cf7aea7ff69d80"},
+    {url = "https://files.pythonhosted.org/packages/f3/23/7cc851bae09cf4db90d42a701dfe525780883ada86bece45e3da7a07e76b/numpy-1.24.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:3c1104d3c036fb81ab923f507536daedc718d0ad5a8707c6061cdfd6d184e570"},
+    {url = "https://files.pythonhosted.org/packages/fa/7d/8dfb40eecbb6bc83ca00ef979f5cdeca5909a250cb8b642dcf1fbd34c078/numpy-1.24.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7"},
 ]
 "packaging 23.1" = [
     {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 "pillow 9.5.0" = [
     {url = "https://files.pythonhosted.org/packages/00/d5/4903f310765e0ff2b8e91ffe55031ac6af77d982f0156061e20a4d1a8b2d/Pillow-9.5.0.tar.gz", hash = "sha256:bf548479d336726d7a0eceb6e767e179fbde37833ae42794602631a070d630f1"},
@@ -477,44 +536,42 @@
     {url = "https://files.pythonhosted.org/packages/41/69/319ff6c2bda31b0ab0710d2bb406d53f7d9c13a1c572696479a16322d9dc/pytest_xdist-3.2.1-py3-none-any.whl", hash = "sha256:37290d161638a20b672401deef1cba812d110ac27e35d213f091d15b8beb40c9"},
     {url = "https://files.pythonhosted.org/packages/e3/f8/de2dcd2938c05270c9881cb1463dea388acd0b239ee76809160420157784/pytest-xdist-3.2.1.tar.gz", hash = "sha256:1849bd98d8b242b948e472db7478e090bf3361912a8fed87992ed94085f54727"},
 ]
 "python-dateutil 2.8.2" = [
     {url = "https://files.pythonhosted.org/packages/36/7a/87837f39d0296e723bb9b62bbb257d0355c7f6128853c78955f57342a56d/python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
     {url = "https://files.pythonhosted.org/packages/4c/c4/13b4776ea2d76c115c1d1b84579f3764ee6d57204f6be27119f13a61d0a9/python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
 ]
-"scipy 1.6.1" = [
-    {url = "https://files.pythonhosted.org/packages/06/c8/78d94bf4d039fd1ef878363491f2925e29b7ccfafa3dcd9dddfaeb0f4608/scipy-1.6.1-cp37-cp37m-win_amd64.whl", hash = "sha256:5fa9c6530b1661f1370bcd332a1e62ca7881785cc0f80c0d559b636567fab63c"},
-    {url = "https://files.pythonhosted.org/packages/09/ca/1be7a6fcf9217c210c115af78a4dfbc4aac96f8b2e15f17f532380ecd761/scipy-1.6.1-cp37-cp37m-manylinux1_i686.whl", hash = "sha256:e79570979ccdc3d165456dd62041d9556fb9733b86b4b6d818af7a0afc15f092"},
-    {url = "https://files.pythonhosted.org/packages/26/68/84dbe18583e79e56e4cee8d00232a8dd7d4ae33bc3acf3be1c347991848f/scipy-1.6.1.tar.gz", hash = "sha256:c4fceb864890b6168e79b0e714c585dbe2fd4222768ee90bc1aa0f8218691b11"},
-    {url = "https://files.pythonhosted.org/packages/2c/30/518c0011f681125528b2e64ad9f5455d4f34e012b9e3a56a6d4ff5486769/scipy-1.6.1-cp38-cp38-manylinux1_x86_64.whl", hash = "sha256:0e5b0ccf63155d90da576edd2768b66fb276446c371b73841e3503be1d63fb5d"},
-    {url = "https://files.pythonhosted.org/packages/3e/26/671c3e19d9d5e55ccbe62166b82e731407d499e01e3ae2b37bc8da36716f/scipy-1.6.1-cp37-cp37m-win32.whl", hash = "sha256:6725e3fbb47da428794f243864f2297462e9ee448297c93ed1dcbc44335feb78"},
-    {url = "https://files.pythonhosted.org/packages/3f/cb/6aa7397a13a064a9bd613d02fd337e2c11d28adccd970dfdab6b941fe4a6/scipy-1.6.1-cp39-cp39-win_amd64.whl", hash = "sha256:a5193a098ae9f29af283dcf0041f762601faf2e595c0db1da929875b7570353f"},
-    {url = "https://files.pythonhosted.org/packages/4c/09/f88dc11bf0e996140079a15445392a5dd7a983cbcab3c93b002a11d27624/scipy-1.6.1-cp39-cp39-manylinux2014_aarch64.whl", hash = "sha256:5da5471aed911fe7e52b86bf9ea32fb55ae93e2f0fac66c32e58897cfb02fa07"},
-    {url = "https://files.pythonhosted.org/packages/6b/ac/20b92f916734d27d3fa0e0c3c1a25eff1d3a3efdd571d3c99e0c90cf7250/scipy-1.6.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:a15a1f3fc0abff33e792d6049161b7795909b40b97c6cc2934ed54384017ab76"},
-    {url = "https://files.pythonhosted.org/packages/6d/64/78bf382ad60646af5f2faae147b480bed9035ba09085011492f754fd2c14/scipy-1.6.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:0c8a51d33556bf70367452d4d601d1742c0e806cd0194785914daf19775f0e67"},
-    {url = "https://files.pythonhosted.org/packages/8b/2f/8d5307a9c45a2eab89b88888b09dfa2a7ee9119d42377766676c16506a02/scipy-1.6.1-cp37-cp37m-manylinux2014_aarch64.whl", hash = "sha256:33d6b7df40d197bdd3049d64e8e680227151673465e5d85723b3b8f6b15a6ced"},
-    {url = "https://files.pythonhosted.org/packages/9a/62/6caa5721d25452b5885f33b0c66c8aeff6151491f4648c48b3107caf22a9/scipy-1.6.1-cp39-cp39-win32.whl", hash = "sha256:8e403a337749ed40af60e537cc4d4c03febddcc56cd26e774c9b1b600a70d3e4"},
-    {url = "https://files.pythonhosted.org/packages/ad/d9/39ec0b85e10f4cee7d5e3982688f8db3ecd87148f5b8fe569ce483b65f73/scipy-1.6.1-cp38-cp38-win32.whl", hash = "sha256:68cb4c424112cd4be886b4d979c5497fba190714085f46b8ae67a5e4416c32b4"},
-    {url = "https://files.pythonhosted.org/packages/b6/3a/9e0649ab2d5ade703baa70ef980aa08739226e5d6a642f084bb201a92fc2/scipy-1.6.1-cp37-cp37m-manylinux1_x86_64.whl", hash = "sha256:a423533c55fec61456dedee7b6ee7dce0bb6bfa395424ea374d25afa262be261"},
-    {url = "https://files.pythonhosted.org/packages/b6/94/f91d57b1f07c9acf3d788cacb4d893960702558974941d9b95516a2aa9cf/scipy-1.6.1-cp38-cp38-manylinux1_i686.whl", hash = "sha256:f46dd15335e8a320b0fb4685f58b7471702234cba8bb3442b69a3e1dc329c345"},
-    {url = "https://files.pythonhosted.org/packages/c1/1e/39a0ed6efe26bf1c1f1abefefadc8da2fd8a627b68c0d0bb0a5f87a86796/scipy-1.6.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:bd50daf727f7c195e26f27467c85ce653d41df4358a25b32434a50d8870fc519"},
-    {url = "https://files.pythonhosted.org/packages/cc/53/cab80f57ac5768de616e351898ad37fc59ca2b4fedbe60feb4780c2cb957/scipy-1.6.1-cp39-cp39-manylinux1_x86_64.whl", hash = "sha256:794e768cc5f779736593046c9714e0f3a5940bc6dcc1dba885ad64cbfb28e9f0"},
-    {url = "https://files.pythonhosted.org/packages/e7/13/0fadfac73fd95bfa74a72dcada39fa6b134fc73a6384256356f18242fb58/scipy-1.6.1-cp38-cp38-win_amd64.whl", hash = "sha256:5f331eeed0297232d2e6eea51b54e8278ed8bb10b099f69c44e2558c090d06bf"},
-    {url = "https://files.pythonhosted.org/packages/f1/79/ff16465aef60bf212a31e2c49ca53191908b7fa341dc6b5e8853288f2623/scipy-1.6.1-cp39-cp39-manylinux1_i686.whl", hash = "sha256:83bf7c16245c15bc58ee76c5418e46ea1811edcc2e2b03041b804e46084ab627"},
-    {url = "https://files.pythonhosted.org/packages/f6/4a/e2b7c44e3c484e01e51f0b36d4c881102d9bd8a8b7aa7e846a421dc50b7e/scipy-1.6.1-cp38-cp38-manylinux2014_aarch64.whl", hash = "sha256:2481efbb3740977e3c831edfd0bd9867be26387cacf24eb5e366a6a374d3d00d"},
+"scipy 1.9.3" = [
+    {url = "https://files.pythonhosted.org/packages/0a/2e/44795c6398e24e45fa0bb61c3e98de1cfea567b1b51efd3751e2f7ff9720/scipy-1.9.3.tar.gz", hash = "sha256:fbc5c05c85c1a02be77b1ff591087c83bc44579c6d2bd9fb798bb64ea5e1a027"},
+    {url = "https://files.pythonhosted.org/packages/40/0e/3ff193b6ba6a0a6f13f8d367e8976370232e769bd609c8c11d86e0353adf/scipy-1.9.3-cp310-cp310-macosx_12_0_arm64.whl", hash = "sha256:83b89e9586c62e787f5012e8475fbb12185bafb996a03257e9675cd73d3736dd"},
+    {url = "https://files.pythonhosted.org/packages/42/14/d2500818b7bb7b862d70c1ae97e646a4795b068583c67720553764095024/scipy-1.9.3-cp38-cp38-win_amd64.whl", hash = "sha256:2318bef588acc7a574f5bfdff9c172d0b1bf2c8143d9582e05f878e580a3781e"},
+    {url = "https://files.pythonhosted.org/packages/42/81/0a64d2204c3b261380ac96c6d61f018528108b62c0e21e6153a58cebf4f6/scipy-1.9.3-cp311-cp311-win_amd64.whl", hash = "sha256:06d2e1b4c491dc7d8eacea139a1b0b295f74e1a1a0f704c375028f8320d16e31"},
+    {url = "https://files.pythonhosted.org/packages/44/8a/bae77e624391b27aeea2d33a02f2ce4a8019f1378ce92faf5780f1521f2e/scipy-1.9.3-cp38-cp38-macosx_12_0_arm64.whl", hash = "sha256:545c83ffb518094d8c9d83cce216c0c32f8c04aaf28b92cc8283eda0685162d5"},
+    {url = "https://files.pythonhosted.org/packages/56/af/6a2b90fe280e89466d84747054667f74b84a8304f75931a173090919991f/scipy-1.9.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cff3a5295234037e39500d35316a4c5794739433528310e117b8a9a0c76d20fc"},
+    {url = "https://files.pythonhosted.org/packages/59/0b/8a9acfc5c36bbf6e18d02f3a08db5b83bebba510be2df3230f53852c74a4/scipy-1.9.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d01e1dd7b15bd2449c8bfc6b7cc67d630700ed655654f0dfcf121600bad205c9"},
+    {url = "https://files.pythonhosted.org/packages/59/ef/d54d17c36b46a9b8f6e1d4bf039b7f7ad236504cfb13cf1872caec9cbeaa/scipy-1.9.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:d644a64e174c16cb4b2e41dfea6af722053e83d066da7343f333a54dae9bc31c"},
+    {url = "https://files.pythonhosted.org/packages/84/86/4f38fa30c112c3590954420f85d95b8cd23811ecc5cfc4bfd4d988d4db44/scipy-1.9.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:5a04cd7d0d3eff6ea4719371cbc44df31411862b9646db617c99718ff68d4840"},
+    {url = "https://files.pythonhosted.org/packages/92/f9/7ae2c1ae200212bc84b5a8369a10d644aa8b588140fe292d59db3b4a2545/scipy-1.9.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:abaf921531b5aeaafced90157db505e10345e45038c39e5d9b6c7922d68085cb"},
+    {url = "https://files.pythonhosted.org/packages/b5/67/c5451465ec94e654e6315cd5136961d267ae94a0f799b85d26eb9efe4c9f/scipy-1.9.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4db5b30849606a95dcf519763dd3ab6fe9bd91df49eba517359e450a7d80ce2e"},
+    {url = "https://files.pythonhosted.org/packages/bb/b7/380c9e4cd71263f03d16f8a92c0e44c9bdef38777e1a7dde1f47ba996bac/scipy-1.9.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c68db6b290cbd4049012990d7fe71a2abd9ffbe82c0056ebe0f01df8be5436b0"},
+    {url = "https://files.pythonhosted.org/packages/c3/3e/e40c52775a5d19abd43b1c245fbc5dee283a29acc45c830bc73bfad9468b/scipy-1.9.3-cp311-cp311-macosx_12_0_arm64.whl", hash = "sha256:90453d2b93ea82a9f434e4e1cba043e779ff67b92f7a0e85d05d286a3625df3c"},
+    {url = "https://files.pythonhosted.org/packages/c8/0f/d9f8c50be8670b7ba6f002679e84cd18f46a23faf62c1590f4d1bbec0c8c/scipy-1.9.3-cp39-cp39-macosx_12_0_arm64.whl", hash = "sha256:da8245491d73ed0a994ed9c2e380fd058ce2fa8a18da204681f2fe1f57f98f95"},
+    {url = "https://files.pythonhosted.org/packages/ce/28/635391e72e24bd3f4a91e374f4a186a5e4ecc95f23d8a55c9b0d25777cf7/scipy-1.9.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1a72d885fa44247f92743fc20732ae55564ff2a519e8302fb7e18717c5355a8b"},
+    {url = "https://files.pythonhosted.org/packages/cf/0e/3f1685c1fcb5dfe35ec027a5fc7a29e8818c61b2cc7fa207b4fc7b959f52/scipy-1.9.3-cp310-cp310-win_amd64.whl", hash = "sha256:68239b6aa6f9c593da8be1509a05cb7f9efe98b80f43a5861cd24c7557e98523"},
+    {url = "https://files.pythonhosted.org/packages/d0/96/4f6eac3fea18f836a0e403539556b1684e6f3361fa39aa5d5797dedecd75/scipy-1.9.3-cp39-cp39-win_amd64.whl", hash = "sha256:5b88e6d91ad9d59478fafe92a7c757d00c59e3bdc3331be8ada76a4f8d683f58"},
+    {url = "https://files.pythonhosted.org/packages/df/75/c0254dc58d1f1b00f9d3dbda029743b71b815dd512461ed20d9b7f459e37/scipy-1.9.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b41bc822679ad1c9a5f023bc93f6d0543129ca0f37c1ce294dd9d386f0a21096"},
+    {url = "https://files.pythonhosted.org/packages/f4/9d/882134b1e774a9227ab855c71a39612194e1106185595417ce92f0f1e78c/scipy-1.9.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d54222d7a3ba6022fdf5773931b5d7c56efe41ede7f7128c7b1637700409108"},
+    {url = "https://files.pythonhosted.org/packages/f9/37/5cd44af74d7178a44452b17ea162bc93996d5555b4a978877d2efd56fe84/scipy-1.9.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:83c06e62a390a9167da60bedd4575a14c1f58ca9dfde59830fc42e5197283dab"},
+    {url = "https://files.pythonhosted.org/packages/fb/ba/1733dbbc19f2aa07d100cfa220bcc83a3977bc5c9f0a5ad262dae1f3ab90/scipy-1.9.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1884b66a54887e21addf9c16fb588720a8309a57b2e258ae1c7986d4444d3bc0"},
 ]
 "six 1.16.0" = [
     {url = "https://files.pythonhosted.org/packages/71/39/171f1c67cd00715f190ba0b100d606d440a28c93c7714febeca8b79af85e/six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
     {url = "https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
 ]
 "tomli 2.0.1" = [
     {url = "https://files.pythonhosted.org/packages/97/75/10a9ebee3fd790d20926a90a2547f0bf78f371b2f13aa822c759680ca7b9/tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {url = "https://files.pythonhosted.org/packages/c0/3f/d7af728f075fb08564c5949a9c95e44352e23dee646869fa104a3b2060a3/tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
-"typing-extensions 4.5.0" = [
-    {url = "https://files.pythonhosted.org/packages/31/25/5abcd82372d3d4a3932e1fa8c3dbf9efac10cc7c0d16e78467460571b404/typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
-    {url = "https://files.pythonhosted.org/packages/d3/20/06270dac7316220643c32ae61694e451c98f8caf4c8eab3aa80a2bedf0df/typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
-]
 "zipp 3.15.0" = [
     {url = "https://files.pythonhosted.org/packages/00/27/f0ac6b846684cecce1ee93d32450c45ab607f65c2e0255f0092032d91f07/zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
     {url = "https://files.pythonhosted.org/packages/5b/fa/c9e82bbe1af6266adf08afb563905eb87cab83fde00a0a08963510621047/zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
 ]
```

### Comparing `mpl-smithchart-0.1.0/pyproject.toml` & `mpl-smithchart-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 description = "An extension for matplotlib providing a projection class to generate high quality Smith Chart plots."
 readme = "README.md"
 license = {text = "BSD"}
 authors = [
     {name = "Paul Staerke", email = "paul.staerke@gmail.com"},
     {name = "Spencer Chang", email = "spencer@sycee.xyz"},
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = [
   "version",
 ]
 dependencies = [
     "matplotlib>=1.2",
-    "numpy>=1.21.1",
-    "scipy>=1.6.1",
+    "numpy>=1.24.3",
+    "scipy>=1.9.3",
 ]
 [project.urls]
 repository = "https://github.com/schang412/mpl-smithchart"
 
 
 [tool.setuptools_scm]
 write_to = "mpl_smithchart/_version.py"
```

### Comparing `mpl-smithchart-0.1.0/tests/plotting_test.py` & `mpl-smithchart-0.1.1/tests/plotting_test.py`

 * *Files identical despite different names*

