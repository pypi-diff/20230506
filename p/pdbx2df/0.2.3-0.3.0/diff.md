# Comparing `tmp/pdbx2df-0.2.3.tar.gz` & `tmp/pdbx2df-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbx2df-0.2.3.tar", last modified: Fri May  5 16:27:37 2023, max compression
+gzip compressed data, was "pdbx2df-0.3.0.tar", last modified: Sat May  6 01:06:47 2023, max compression
```

## Comparing `pdbx2df-0.2.3.tar` & `pdbx2df-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-05-05 16:27:37.028664 pdbx2df-0.2.3/
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1542 2023-01-06 18:27:27.000000 pdbx2df-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 rliu      (2718) Shen      (2001)      174 2023-01-04 17:52:02.000000 pdbx2df-0.2.3/.readthedocs.yaml
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1067 2023-01-04 17:51:08.000000 pdbx2df-0.2.3/LICENSE
--rw-r--r--   0 rliu      (2718) Shen      (2001)      348 2023-01-04 18:04:18.000000 pdbx2df-0.2.3/MANIFEST.in
--rw-r--r--   0 rliu      (2718) Shen      (2001)     2332 2023-05-05 16:27:37.028664 pdbx2df-0.2.3/PKG-INFO
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1780 2023-01-06 19:34:13.000000 pdbx2df-0.2.3/README.md
-drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-05-05 16:27:37.012664 pdbx2df-0.2.3/pdbx2df/
--rw-r--r--   0 rliu      (2718) Shen      (2001)      258 2023-01-06 14:31:26.000000 pdbx2df-0.2.3/pdbx2df/__init__.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)        0 2023-01-05 03:15:10.000000 pdbx2df-0.2.3/pdbx2df/py.typed
--rw-r--r--   0 rliu      (2718) Shen      (2001)     5805 2023-05-05 16:27:14.000000 pdbx2df-0.2.3/pdbx2df/read_pdbx.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)     2212 2023-01-06 19:10:17.000000 pdbx2df-0.2.3/pdbx2df/split_line.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)       22 2023-05-05 16:27:14.000000 pdbx2df-0.2.3/pdbx2df/version.py
-drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-05-05 16:27:37.012664 pdbx2df-0.2.3/pdbx2df.egg-info/
--rw-r--r--   0 rliu      (2718) Shen      (2001)     2332 2023-05-05 16:27:36.000000 pdbx2df-0.2.3/pdbx2df.egg-info/PKG-INFO
--rw-r--r--   0 rliu      (2718) Shen      (2001)      489 2023-05-05 16:27:36.000000 pdbx2df-0.2.3/pdbx2df.egg-info/SOURCES.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)        1 2023-05-05 16:27:36.000000 pdbx2df-0.2.3/pdbx2df.egg-info/dependency_links.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)       61 2023-05-05 16:27:36.000000 pdbx2df-0.2.3/pdbx2df.egg-info/requires.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)       14 2023-05-05 16:27:36.000000 pdbx2df-0.2.3/pdbx2df.egg-info/top_level.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)      327 2023-01-06 14:11:27.000000 pdbx2df-0.2.3/pyproject.toml
--rw-r--r--   0 rliu      (2718) Shen      (2001)       12 2023-01-04 18:02:53.000000 pdbx2df-0.2.3/requirements.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)       38 2023-01-04 17:52:29.000000 pdbx2df-0.2.3/requirements_dev.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)      240 2023-05-05 16:27:37.032664 pdbx2df-0.2.3/setup.cfg
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1202 2023-01-06 19:37:41.000000 pdbx2df-0.2.3/setup.py
-drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-05-05 16:27:37.024664 pdbx2df-0.2.3/tests/
--rw-r--r--   0 rliu      (2718) Shen      (2001)        0 2023-01-05 20:19:15.000000 pdbx2df-0.2.3/tests/__init__.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)      304 2023-01-05 20:19:46.000000 pdbx2df-0.2.3/tests/conftest.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)     2038 2023-01-06 19:28:03.000000 pdbx2df-0.2.3/tests/test_read_pdbx.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1999 2023-01-06 14:17:27.000000 pdbx2df-0.2.3/tests/test_split_line.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)      306 2023-01-06 18:37:06.000000 pdbx2df-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:06:47.957222 pdbx2df-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-06 01:06:47.957222 pdbx2df-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:06:47.953222 pdbx2df-0.3.0/pdbx2df/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/pdbx2df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/pdbx2df/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/pdbx2df/read_pdbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/pdbx2df/split_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/pdbx2df/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/pdbx2df/write_pdbx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:06:47.957222 pdbx2df-0.3.0/pdbx2df.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-06 01:06:47.000000 pdbx2df-0.3.0/pdbx2df.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-06 01:06:47.000000 pdbx2df-0.3.0/pdbx2df.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:06:47.000000 pdbx2df-0.3.0/pdbx2df.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 01:06:47.000000 pdbx2df-0.3.0/pdbx2df.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 01:06:47.000000 pdbx2df-0.3.0/pdbx2df.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-06 01:06:47.957222 pdbx2df-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:06:47.957222 pdbx2df-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/tests/test_read_pdbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/tests/test_split_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/tests/test_write_pdbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-06 01:06:29.000000 pdbx2df-0.3.0/tox.ini
```

### Comparing `pdbx2df-0.2.3/.pre-commit-config.yaml` & `pdbx2df-0.3.0/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-builtin-literals
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
-        exclude: WHEEL
+        exclude: tests/test_files
       - id: forbid-new-submodules
       - id: trailing-whitespace
         exclude: tests/test_files
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3.9
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
           [
-            "flake8-bugbear==20.1.4",
-            "flake8-logging-format==0.6.0",
-            "flake8-implicit-str-concat==0.2.0",
+            "flake8-bugbear==23.3.23",
+            "flake8-logging-format==0.9.0",
+            "flake8-implicit-str-concat==0.4.0",
           ]
-        exclude: tests/test_files/1VII.cif
+        exclude: tests/test_files
 
-  # - repo: https://github.com/PyCQA/isort
-  #   rev: 5.9.3
-  #   hooks:
-  #     - id: isort
-  #       files: \.py$
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
+        files: \.py$
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.950
+    rev: v1.2.0
     hooks:
       - id: mypy
         exclude: tests/data
         args: ["--pretty", "--show-error-codes"]
         additional_dependencies:
           [
-            "keyring==23.0.1",
-            "nox==2021.6.12",
-            "pytest==6.2.5",
-            "types-docutils==0.1.8",
-            "types-setuptools==57.0.2",
-            "types-six==0.1.9",
+            "keyring==23.13.1",
+            "nox==2023.4.22",
+            "pytest==7.3.1",
+            "types-docutils==0.19.1.9",
+            "types-setuptools==67.7.0.1",
+            "types-six==1.16.21.8",
           ]
 
   - repo: https://github.com/mgedmin/check-manifest
-    rev: "0.48"
+    rev: "0.49"
     hooks:
       - id: check-manifest
         stages: [manual]
```

### Comparing `pdbx2df-0.2.3/LICENSE` & `pdbx2df-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.3/PKG-INFO` & `pdbx2df-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pdbx2df
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python package to parse PDBx file into Pandas DataFrames.
 Home-page: https://github.com/Ruibin-Liu/pdbx2df
 Author: Ruibin Liu
 Author-email: ruibinliuphd@gmail.com
 Project-URL: Bug Tracker, https://github.com/Ruibin-Liu/pdbx2df/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # pdbx2df
 
 Parse a PDBx file (mmCIF file: pdb_id.cif) into a python dict with PDBx category names as keys and contents belonging to the category as the corresponding values. Each category content is parsed as a Pandas DataFrame whose columns are the attribute names.
```

### Comparing `pdbx2df-0.2.3/README.md` & `pdbx2df-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.3/pdbx2df/read_pdbx.py` & `pdbx2df-0.3.0/pdbx2df/read_pdbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from collections import defaultdict
 
 import pandas as pd  # type: ignore
 
 from .split_line import split_line
 
 
-def read_pdbx(pdbx_file: str, category_names: list = None) -> dict:
+def read_pdbx(pdbx_file: str, category_names: list) -> dict:
     """
     Read a pdbx file categories into Pandas DataFrame.
 
     Args:
         pdbx_file (str): file name for a PDBx file.
-        category_names (list|None): a list of names for the categories in a PDBx file that need to be read.
+        category_names (list): a list of names for the categories in a PDBx file that need to be read.
 
     Returns:
         A dict of {category_name: pd.DataFrame of the info belongs to the category}
     """
     data: dict[str, pd.DataFrame] = {}
     if not category_names:
         return data
```

### Comparing `pdbx2df-0.2.3/pdbx2df/split_line.py` & `pdbx2df-0.3.0/pdbx2df/split_line.py`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.3/pdbx2df.egg-info/PKG-INFO` & `pdbx2df-0.3.0/pdbx2df.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pdbx2df
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python package to parse PDBx file into Pandas DataFrames.
 Home-page: https://github.com/Ruibin-Liu/pdbx2df
 Author: Ruibin Liu
 Author-email: ruibinliuphd@gmail.com
 Project-URL: Bug Tracker, https://github.com/Ruibin-Liu/pdbx2df/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # pdbx2df
 
 Parse a PDBx file (mmCIF file: pdb_id.cif) into a python dict with PDBx category names as keys and contents belonging to the category as the corresponding values. Each category content is parsed as a Pandas DataFrame whose columns are the attribute names.
```

### Comparing `pdbx2df-0.2.3/setup.py` & `pdbx2df-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,9 +32,9 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(),
     install_requires=REQUIREMENTS,
-    python_requires=">=3.8",
+    python_requires=">=3.9",
 )
```

### Comparing `pdbx2df-0.2.3/tests/test_read_pdbx.py` & `pdbx2df-0.3.0/tests/test_read_pdbx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 
 import pandas as pd  # type: ignore
+
 from pdbx2df.read_pdbx import read_pdbx
 
 sys.path.append("..")
 CFD = os.path.dirname(__file__)
 
 
 def test_read_pdbx():
```

### Comparing `pdbx2df-0.2.3/tests/test_split_line.py` & `pdbx2df-0.3.0/tests/test_split_line.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 
-import pytest
+import pytest  # type: ignore
+
 from pdbx2df.split_line import split_line
 
 sys.path.append("..")
 
 
 def test_split_line():
     """
```

