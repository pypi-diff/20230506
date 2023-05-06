# Comparing `tmp/nyckel-0.0.5.tar.gz` & `tmp/nyckel-0.0.6.tar.gz`

## Comparing `nyckel-0.0.5.tar` & `nyckel-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nyckel-0.0.5/requirements.txt
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 nyckel-0.0.5/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 nyckel-0.0.5/.github/workflows/test-all.yml
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nyckel-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.5/src/nyckel/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.5/src/nyckel/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.0.5/src/nyckel/greeter.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nyckel-0.0.5/tests/test_greeter.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.5/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.5/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nyckel-0.0.5/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nyckel-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nyckel-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nyckel-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 nyckel-0.0.6/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 nyckel-0.0.6/.github/workflows/test-all.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 nyckel-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/auth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/config.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/functions/text_classification_function.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nyckel-0.0.6/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 nyckel-0.0.6/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.6/LICENSE
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nyckel-0.0.6/README.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nyckel-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 nyckel-0.0.6/PKG-INFO
```

### Comparing `nyckel-0.0.5/.github/workflows/deploy.yml` & `nyckel-0.0.6/.github/workflows/test-all.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-name: Test and deploy to PYPI
+name: Test all python versions
 
-on: 
-  push:
-    branches:
-      - master
+on: [push]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
+
     steps:
       - uses: actions/checkout@v3
-      - name: Set up Python
+      - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
-      - name: Install test dependencies
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install pytest
+          pip install ruff pytest
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-      - name: Set PYTHONPATH
+      - name: set pythonpath
         run: |
           echo "PYTHONPATH=src" >> $GITHUB_ENV
-      - name: Test with pytest
+      - name: Lint with ruff
         run: |
-          pytest
-      - name: Install build dependencies
+          # stop the build if there are Python syntax errors or undefined names
+          ruff --format=github --select=E9,F63,F7,F82 --target-version=py37 .
+          # default set of ruff rules with GitHub Annotations
+          ruff --format=github --target-version=py37 .
+      - name: Test with pytest
+        env: 
+          NYCKEL_CLIENT_ID: ${{ secrets.NYCKEL_CLIENT_ID }}
+          NYCKEL_CLIENT_SECRET: ${{ secrets.NYCKEL_CLIENT_SECRET }}
         run: |
-          pip install build
-      - name: Build package
-        run: python -m build
-      - name: Publish package
-        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          pytest -s
```

### Comparing `nyckel-0.0.5/.gitignore` & `nyckel-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.5/LICENSE` & `nyckel-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.5/pyproject.toml` & `nyckel-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,34 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 
 [project]
 name = "nyckel"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Oscar Beijbom", email="oscar@nyckel.com" },
 ]
 description = "Python package for the Nyckel API"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "tqdm~=4.65.0",
+  "requests~=2.30.0",
+]
+
 
 [project.urls]
 "Homepage" = "https://github.com/NyckelAI/python-sdk"
 
+[tool.ruff]
+line-length = 120
+select = [
+    "F401",
+    "F403",
+]
```

