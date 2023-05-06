# Comparing `tmp/psfmodels-0.3.2.tar.gz` & `tmp/psfmodels-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psfmodels-0.3.2.tar", last modified: Sat Apr 23 15:50:10 2022, max compression
+gzip compressed data, was "psfmodels-0.3.3.tar", last modified: Sat May  6 15:50:29 2023, max compression
```

## Comparing `psfmodels-0.3.2.tar` & `psfmodels-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.834072 psfmodels-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-04-23 15:44:16.000000 psfmodels-0.3.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.830072 psfmodels-0.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-04-23 15:44:16.000000 psfmodels-0.3.2/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.830072 psfmodels-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-04-23 15:44:16.000000 psfmodels-0.3.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-04-23 15:44:16.000000 psfmodels-0.3.2/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-04-23 15:44:16.000000 psfmodels-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-04-23 15:44:16.000000 psfmodels-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-04-23 15:44:16.000000 psfmodels-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-04-23 15:44:16.000000 psfmodels-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7068 2022-04-23 15:50:10.834072 psfmodels-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6087 2022-04-23 15:44:16.000000 psfmodels-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)   115544 2022-04-23 15:44:16.000000 psfmodels-0.3.2/fig.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.830072 psfmodels-0.3.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)    86506 2022-04-23 15:44:16.000000 psfmodels-0.3.2/notebooks/Untitled.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    21946 2022-04-23 15:44:16.000000 psfmodels-0.3.2/notebooks/Untitled1.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    29349 2022-04-23 15:44:16.000000 psfmodels-0.3.2/notebooks/Untitled2.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   239511 2022-04-23 15:44:16.000000 psfmodels-0.3.2/notebooks/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   245068 2022-04-23 15:44:16.000000 psfmodels-0.3.2/notebooks/lightsheet.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-04-23 15:44:16.000000 psfmodels-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-04-23 15:50:10.834072 psfmodels-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-04-23 15:44:16.000000 psfmodels-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.826072 psfmodels-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.830072 psfmodels-0.3.2/src/_psfmodels/
--rw-r--r--   0 runner    (1001) docker     (121)     5588 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/_psfmodels/psfmath.h
--rw-r--r--   0 runner    (1001) docker     (121)     8806 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/_psfmodels/pythonBindings.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    16272 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/_psfmodels/scalarPSF.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    27416 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/_psfmodels/vectorialPSF.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.830072 psfmodels-0.3.2/src/_psfmodels-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)     5981 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/_psfmodels-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.834072 psfmodels-0.3.2/src/psfmodels/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/psfmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20272 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/psfmodels/_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/psfmodels/_cuvec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/psfmodels/_napari.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-23 15:50:09.000000 psfmodels-0.3.2/src/psfmodels/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/psfmodels/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 15:44:16.000000 psfmodels-0.3.2/src/psfmodels/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.834072 psfmodels-0.3.2/src/psfmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7068 2022-04-23 15:50:10.000000 psfmodels-0.3.2/src/psfmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-04-23 15:50:10.000000 psfmodels-0.3.2/src/psfmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-23 15:50:10.000000 psfmodels-0.3.2/src/psfmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-04-23 15:50:10.000000 psfmodels-0.3.2/src/psfmodels.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-23 15:50:08.000000 psfmodels-0.3.2/src/psfmodels.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-04-23 15:50:10.000000 psfmodels-0.3.2/src/psfmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-23 15:50:10.000000 psfmodels-0.3.2/src/psfmodels.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 15:50:10.834072 psfmodels-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-04-23 15:44:16.000000 psfmodels-0.3.2/tests/test_napari_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-04-23 15:44:16.000000 psfmodels-0.3.2/tests/test_psf.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-04-23 15:44:16.000000 psfmodels-0.3.2/tests/test_purepy.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-04-23 15:44:16.000000 psfmodels-0.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.238651 psfmodels-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-06 15:45:26.000000 psfmodels-0.3.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.234651 psfmodels-0.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-05-06 15:45:26.000000 psfmodels-0.3.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-06 15:45:26.000000 psfmodels-0.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.234651 psfmodels-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-05-06 15:45:26.000000 psfmodels-0.3.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-06 15:45:26.000000 psfmodels-0.3.3/.github_changelog_generator
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-06 15:45:26.000000 psfmodels-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-06 15:45:26.000000 psfmodels-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-06 15:45:26.000000 psfmodels-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-06 15:45:26.000000 psfmodels-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-05-06 15:50:29.238651 psfmodels-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-05-06 15:45:26.000000 psfmodels-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)   115544 2023-05-06 15:45:26.000000 psfmodels-0.3.3/fig.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.234651 psfmodels-0.3.3/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (122)    86506 2023-05-06 15:45:26.000000 psfmodels-0.3.3/notebooks/Untitled.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    21946 2023-05-06 15:45:26.000000 psfmodels-0.3.3/notebooks/Untitled1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    29349 2023-05-06 15:45:26.000000 psfmodels-0.3.3/notebooks/Untitled2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)   239511 2023-05-06 15:45:26.000000 psfmodels-0.3.3/notebooks/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)   245068 2023-05-06 15:45:26.000000 psfmodels-0.3.3/notebooks/lightsheet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-05-06 15:45:26.000000 psfmodels-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-05-06 15:50:29.238651 psfmodels-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-06 15:45:26.000000 psfmodels-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.234651 psfmodels-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.238651 psfmodels-0.3.3/src/_psfmodels/
+-rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/_psfmodels/psfmath.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8806 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/_psfmodels/pythonBindings.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16272 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/_psfmodels/scalarPSF.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    27416 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/_psfmodels/vectorialPSF.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.238651 psfmodels-0.3.3/src/_psfmodels-stubs/
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/_psfmodels-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.238651 psfmodels-0.3.3/src/psfmodels/
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/psfmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22493 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/psfmodels/_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/psfmodels/_cuvec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5180 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/psfmodels/_jax_bessel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3065 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/psfmodels/_napari.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-06 15:50:29.000000 psfmodels-0.3.3/src/psfmodels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/psfmodels/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 15:45:26.000000 psfmodels-0.3.3/src/psfmodels/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.238651 psfmodels-0.3.3/src/psfmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-05-06 15:50:29.000000 psfmodels-0.3.3/src/psfmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-06 15:50:29.000000 psfmodels-0.3.3/src/psfmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 15:50:29.000000 psfmodels-0.3.3/src/psfmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-06 15:50:29.000000 psfmodels-0.3.3/src/psfmodels.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 15:50:28.000000 psfmodels-0.3.3/src/psfmodels.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      330 2023-05-06 15:50:29.000000 psfmodels-0.3.3/src/psfmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-06 15:50:29.000000 psfmodels-0.3.3/src/psfmodels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:50:29.238651 psfmodels-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-06 15:45:26.000000 psfmodels-0.3.3/tests/test_napari_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-05-06 15:45:26.000000 psfmodels-0.3.3/tests/test_psf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-05-06 15:45:26.000000 psfmodels-0.3.3/tests/test_purepy.py
```

### Comparing `psfmodels-0.3.2/.github/workflows/ci.yml` & `psfmodels-0.3.3/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,84 +12,81 @@
 jobs:
   test:
     name: ${{ matrix.platform }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.7, '3.10']
+        python-version: ["3.7", "3.10", "3.11"]
         platform: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install setuptools tox tox-gh-actions
+          python -m pip install .[testing]
 
-      - name: Test with tox
-        run: tox
-        env:
-          PLATFORM: ${{ matrix.platform }}
+      - name: Test with
+        run: pytest -v --color=yes --cov=psfmodels --cov-report=xml
 
       - name: Coverage
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
 
   build:
     name: Build wheels on ${{ matrix.os }}
-    if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-20.04, windows-2019, macos-10.15]
+        os: [ubuntu-20.04, windows-2019, macos-11]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         name: Install Python
         with:
-          python-version: "3.9"
+          python-version: "3.10"
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.4.0
+        uses: pypa/cibuildwheel@v2.12.3
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
 
       - name: Build sdist
         if: matrix.os == 'ubuntu-20.04'
         run: |
           python -m pip install build
           python -m build --sdist
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         if: matrix.os == 'ubuntu-20.04'
         with:
           path: dist/*.tar.gz
 
   upload_pypi:
     needs: [build]
     runs-on: ubuntu-latest
     if: "success() && startsWith(github.ref, 'refs/tags/')"
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.5.0
+      - uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.pypi_token }}
 
       - uses: softprops/action-gh-release@v1
         with:
           generate_release_notes: true
```

### Comparing `psfmodels-0.3.2/.gitignore` & `psfmodels-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/.pre-commit-config.yaml` & `psfmodels-0.3.3/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 ci:
   autoupdate_schedule: quarterly
+  autofix_commit_msg: "style(pre-commit.ci): auto fixes [...]"
+  autoupdate_commit_msg: "ci(pre-commit.ci): autoupdate"
+
 repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.12.2
     hooks:
-      - id: check-docstring-first
-      - id: end-of-file-fixer
-      - id: trailing-whitespace
-  - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.20.1
-    hooks:
-      - id: setup-cfg-fmt
-  - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
-    hooks:
-      - id: flake8
-        additional_dependencies: [flake8-typing-imports]
-  - repo: https://github.com/myint/autoflake
-    rev: v1.4
-    hooks:
-      - id: autoflake
-        args: ["--in-place", "--remove-all-unused-imports"]
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
+      - id: validate-pyproject
+
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.265
+    hooks:
+      - id: ruff
+        args: [--fix]
+
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.0
-    hooks:
-      - id: pyupgrade
-        args: [--py37-plus, --keep-runtime-typing]
+
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.942
+    rev: v1.2.0
     hooks:
       - id: mypy
+        files: "^src/"
+        additional_dependencies:
+          - numpy
```

### Comparing `psfmodels-0.3.2/LICENSE` & `psfmodels-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/PKG-INFO` & `psfmodels-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: psfmodels
-Version: 0.3.2
+Version: 0.3.3
 Summary: Scalar and vectorial models of the microscope point spread function (PSF).
 Home-page: https://github.com/tlambert03/psfmodels
 Author: Talley Lambert
 Author-email: talley.lambert@gmail.com
 License: GPL-3.0
 Project-URL: Source Code, https://github.com/tlambert03/psfmodels
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: napari
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -161,9 +160,7 @@
 ## Lightsheet PSF utility function
 
 The `psfmodels.tot_psf()` function provides a quick way to simulate the total
 system PSF (excitation x detection) as might be observed on a light sheet
 microscope (currently, only strictly orthogonal illumination and detection are
 supported).  See the [lightsheet.ipynb](notebooks/lightsheet.ipynb) Jupyter notebook for
 examples.
-
-
```

### Comparing `psfmodels-0.3.2/README.md` & `psfmodels-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/fig.png` & `psfmodels-0.3.3/fig.png`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/notebooks/Untitled.ipynb` & `psfmodels-0.3.3/notebooks/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/notebooks/Untitled1.ipynb` & `psfmodels-0.3.3/notebooks/Untitled1.ipynb`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/notebooks/Untitled2.ipynb` & `psfmodels-0.3.3/notebooks/Untitled2.ipynb`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/notebooks/examples.ipynb` & `psfmodels-0.3.3/notebooks/examples.ipynb`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/notebooks/lightsheet.ipynb` & `psfmodels-0.3.3/notebooks/lightsheet.ipynb`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/setup.cfg` & `psfmodels-0.3.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -57,52 +57,19 @@
 	pytest
 	pytest-cov
 	tox
 	tox-conda
 testing = 
 	pytest
 	pytest-cov
-	tox
-	tox-conda
+	jax
 	magicgui;platform_system!="Linux"
-	pyside2;platform_system!="Linux"
+	pyside2;platform_system!="Linux" and python_version<"3.11"
 	qtpy;platform_system!="Linux"
 
 [options.package_data]
 * = *.pyi, py.typed
 
-[bdist_wheel]
-universal = 1
-
-[flake8]
-exclude = docs,_version.py,.eggs,examples
-max-line-length = 88
-docstring-convention = numpy
-ignore = D100, D213, D401, D413, D107, W503
-
-[isort]
-profile = black
-src_paths = psfmodels
-
-[pydocstyle]
-match_dir = psfmodels
-convention = numpy
-add_select = D402,D415,D417
-ignore = D100, D213, D401, D413, D107
-
-[tool:pytest]
-addopts = -W error
-
-[mypy]
-files = psfmodels
-warn_unused_configs = True
-warn_unused_ignores = True
-check_untyped_defs = True
-implicit_reexport = False
-show_column_numbers = True
-show_error_codes = True
-ignore_missing_imports = True
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `psfmodels-0.3.2/src/_psfmodels/psfmath.h` & `psfmodels-0.3.3/src/_psfmodels/psfmath.h`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/src/_psfmodels/pythonBindings.cpp` & `psfmodels-0.3.3/src/_psfmodels/pythonBindings.cpp`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/src/_psfmodels/scalarPSF.cpp` & `psfmodels-0.3.3/src/_psfmodels/scalarPSF.cpp`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/src/_psfmodels/vectorialPSF.cpp` & `psfmodels-0.3.3/src/_psfmodels/vectorialPSF.cpp`

 * *Files identical despite different names*

### Comparing `psfmodels-0.3.2/src/_psfmodels-stubs/__init__.pyi` & `psfmodels-0.3.3/src/_psfmodels-stubs/__init__.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Scalar and Vectorial PSF Models."""
 import numpy
+import numpy.typing as npt
 
 __all__ = ["scalar_psf", "vectorial_psf", "vectorial_psf_deriv"]
 
-def scalar_psf(  # noqa: E302
-    zv: numpy.ndarray[numpy.float64],
+def scalar_psf(
+    zv: npt.NDArray[numpy.float64],
     nx: int,
     pz: float,
     ti0: float,
     ni0: float,
     ni: float,
     tg0: float,
     tg: float,
@@ -16,15 +17,15 @@
     ng: float,
     ns: float,
     wvl: float,
     NA: float,
     dxy: float,
     sf: int = 3,
     mode: int = 1,
-) -> numpy.ndarray[numpy.float64]:
+) -> npt.NDArray[numpy.float64]:
     """Compute scalar PSF model described by Gibson and Lanni.
 
     The model is described in F. Aguet et al., Opt. Express 17(8), pp. 6829-6848, 2009
     For more information and implementation details, see F. Aguet, Ph.D Thesis, Swiss
     Federal Institute of Technology, Lausanne (EPFL), 2009
 
     C++ code by Francois Aguet, 2009. Python bindings by Talley Lambert, 2019.
@@ -63,20 +64,20 @@
     sf : int, optional
         oversampling factor to approximate pixel integration, by default 3
     mode : int, optional
         if 0, returns oversampled PSF, by default 1
 
     Returns
     -------
-    numpy.ndarray[numpy.float64]
+    npt.NDArray[numpy.float64]
         PSF with type np.float64 and shape (len(zv), nx, nx)
     """
 
-def vectorial_psf(  # noqa: E302
-    zv: numpy.ndarray[numpy.float64],
+def vectorial_psf(
+    zv: npt.NDArray[numpy.float64],
     nx: int,
     pz: float,
     ti0: float,
     ni0: float,
     ni: float,
     tg0: float,
     tg: float,
@@ -84,15 +85,15 @@
     ng: float,
     ns: float,
     wvl: float,
     NA: float,
     dxy: float,
     sf: int = 3,
     mode: int = 1,
-) -> numpy.ndarray[numpy.float64]:
+) -> npt.NDArray[numpy.float64]:
     """Compute vectorial microscope point spread function model.
 
     The model is described in F. Aguet et al., Opt. Express 17(8), pp. 6829-6848, 2009
     For more information and implementation details, see F. Aguet, Ph.D Thesis, Swiss
     Federal Institute of Technology, Lausanne (EPFL), 2009
 
     C++ code by Francois Aguet, 2009. Python bindings by Talley Lambert, 2019.
@@ -131,23 +132,23 @@
     sf : int, optional
         oversampling factor to approximate pixel integration, by default 3
     mode : int, optional
         if 0, returns oversampled PSF, by default 1
 
     Returns
     -------
-    numpy.ndarray[numpy.float64]
+    npt.NDArray[numpy.float64]
         PSF with type np.float64 and shape (len(zv), nx, nx)
     """
 
-def vectorial_psf_deriv(  # noqa: E302
-    pixdxp: numpy.ndarray[numpy.float64],
-    pixdyp: numpy.ndarray[numpy.float64],
-    pixdzp: numpy.ndarray[numpy.float64],
-    zv: numpy.ndarray[numpy.float64],
+def vectorial_psf_deriv(
+    pixdxp: npt.NDArray[numpy.float64],
+    pixdyp: npt.NDArray[numpy.float64],
+    pixdzp: npt.NDArray[numpy.float64],
+    zv: npt.NDArray[numpy.float64],
     nx: int,
     pz: float,
     ti0: float,
     ni0: float,
     ni: float,
     tg0: float,
     tg: float,
@@ -155,19 +156,25 @@
     ng: float,
     ns: float,
     wvl: float,
     NA: float,
     dxy: float,
     sf: int = 3,
     mode: int = 1,
-) -> numpy.ndarray[numpy.float64]:
+) -> npt.NDArray[numpy.float64]:
     """Compute vectorial point spread function model, and return derivatives.
 
     Parameters
     ----------
+    pixdxp : npt.NDArray[numpy.float64]
+        Derivative of pixel x position with respect to z position
+    pixdyp : npt.NDArray[numpy.float64]
+        Derivative of pixel y position with respect to z position
+    pixdzp : npt.NDArray[numpy.float64]
+        Derivative of pixel z position with respect to z position
     zv : np.ndarray
         Vector of Z positions at which PSF is calculated (in microns, relative to
         coverslip)
     nx : int
         XY size of output PSF in pixels, must be odd.
     pz : float
         point source z position above the coverslip in microns.
```

### Comparing `psfmodels-0.3.2/src/psfmodels/_core.py` & `psfmodels-0.3.3/src/psfmodels/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import warnings
-from typing import Sequence, Union
+from typing import Sequence, Union, cast
 
 import _psfmodels
 import numpy as np
+from scipy.signal import convolve2d
 from typing_extensions import Literal
 
 
 def make_psf(
     z: Union[int, Sequence[float]] = 51,
     nx: int = 51,
     *,
@@ -86,15 +87,17 @@
     psf : np.ndarray
         The PSF array with dtype np.float64 and shape (len(zv), nx, nx)
     """
     if isinstance(z, (int, float)):
         zv: np.ndarray = _centered_zv(z, dz, pz)
     else:
         if dz != 0.05:
-            warnings.warn("dz is ignored when providing a sequence for `z`.")
+            warnings.warn(
+                "dz is ignored when providing a sequence for `z`.", stacklevel=2
+            )
         zv = np.asarray(z)
 
     _args = set(_VALID_ARGS).difference({"zv", "nx", "dxy", "pz", "wvl"})
     kwargs = {k: v for k, v in locals().items() if k in _args}
     kwargs["sf"] = oversample_factor
     kwargs["mode"] = 1 if oversample_factor else 0
 
@@ -140,40 +143,47 @@
     "NA",
     "dxy",
     "sf",
     "mode",
 ]
 
 
-def _normalize_params(mp):
+def _normalize_params(mp: dict):
     """Check and return valid microscope parameters dict, stripped of excess keys.
 
-    Args:
-        mp (dict): The microscope parameters dict
+    Parameters
+    ----------
+    mp : dict
+        Dictionary of microscope parameters
 
-    Raises:
-        ValueError: If one of the parameter values is invalid
+    Raises
+    ------
+    ValueError
+        If one of the parameters is invalid.
 
-    Returns:
-        dict: Valid parameters for use in vectorial_ or scalar_psf
+    Returns
+    -------
+    dict
+        Dictionary of valid microscope parameters.
     """
     _mp = _DEFAULT_PARAMS.copy()
     if mp is not None:
         if isinstance(mp, dict):
             _mp.update(mp)
         else:
             raise ValueError("mp argument must be dict of microscope params")
     out = {}
     for key, val in _mp.items():
         if key in _VALID_ARGS:
             out[key] = val
         else:
             warnings.warn(
                 f"parameter {key} is not one of the recognized keywords "
-                "and is being ignored"
+                "and is being ignored",
+                stacklevel=2,
             )
 
     if _mp["NA"] >= _mp["ni"]:
         raise ValueError("NA must not be greater than immersion medium RI (ni).")
     return {key: val for key, val in _mp.items() if key in _VALID_ARGS}
 
 
@@ -285,15 +295,18 @@
     Parameters derived from Zhang et al (2007). https://doi.org/10.1364/AO.46.001819
     Using the paraxial approximation for NA < 0.7 and the Nonparaxial approximation
     for NA >= 0.7.
     """
     from scipy.stats import multivariate_normal
 
     if pz != 0:
-        warnings.warn("pz != 0 currently does nothing for the gaussian approximation.")
+        warnings.warn(
+            "pz != 0 currently does nothing for the gaussian approximation.",
+            stacklevel=2,
+        )
 
     zv = _validate_args(zv, dxy, pz)
     params = _normalize_params(params)
 
     na = params["NA"]
     nimm = params["ni"]
     alpha = np.arcsin(na / nimm)
@@ -330,15 +343,16 @@
 def vectorial_psf_deriv(
     zv=0, nx=31, dxy=0.05, pz=0.0, wvl=0.6, params=None, normalize=True
 ):
     """Compute a vectorial model of the microscope point spread function.
 
     also returns derivatives in dx, dy, dz.
 
-    Returns:
+    Returns
+    -------
         4-tuple of np.ndarrays: (_psf, dxp, dyp, dzp)
 
     """
     zv = _validate_args(zv, dxy, pz)
     params = _normalize_params(params)
     pixdxp = np.zeros((len(zv), nx, nx))
     pixdyp = np.zeros((len(zv), nx, nx))
@@ -350,23 +364,25 @@
         _psf /= np.max(_psf)
     return _psf, pixdxp, pixdyp, pixdzp
 
 
 def vectorial_psf_centered(nz, dz=0.05, **kwargs):
     """Compute a vectorial model of the microscope point spread function.
 
-    The point source is always in the center of the output volume."""
+    The point source is always in the center of the output volume.
+    """
     zv = _centered_zv(nz, dz, kwargs.get("pz", 0))
     return vectorial_psf(zv, **kwargs)
 
 
 def scalar_psf_centered(nz, dz=0.05, **kwargs):
     """Compute the scalar PSF model described by Gibson and Lanni.
 
-    The point source is always in the center of the output volume."""
+    The point source is always in the center of the output volume.
+    """
     zv = _centered_zv(nz, dz, kwargs.get("pz", 0))
     return scalar_psf(zv, **kwargs)
 
 
 def _centered_zv(nz, dz, pz=0) -> np.ndarray:
     lim = (nz - 1) * dz / 2
     return np.linspace(-lim + pz, lim + pz, nz)
@@ -445,56 +461,67 @@
     em_params=None,
     psf_func="vectorial",
 ):
     """Simlulate a total system psf with orthogonal illumination & detection.
 
     (e.g. SPIM)
 
-    Args:
-        nx (int, optional): XY size of output PSF in pixels, must be odd. Defaults to
-        127. nz (int): Z size of output PSF in pixels, must be odd. Defaults to 127. dxy
-        (float, optional): XY Pixel size in sample space (microns). Defaults to 0.05. dz
-        (float, optional): Z step size of PSF in sample space. Defaults to 0.05 pz (int,
-        optional): Depth of point source relative to coverslip in microns.
-                            Defaults to 0.
-        z_offset (int, optional): Defocus between the axial position of the excitation
-            and the detection plane, with respect to the detection lens. Defaults to 0.
-        x_offset (int, optional): Mismatch between the focal point of the excitation
-        beam
-            and the point source, along the propogation direction of the excitation
-            beam. Defaults to 0.
-        ex_wvl (float, optional): Emission wavelength in microns. Defaults to 0.488.
-        em_wvl (float, optional): Emission wavelength in microns. Defaults to 0.525.
-        ex_params ([type], optional): Excitation lens parameters dict. See keys below.
-        em_params ([type], optional): Emission lens parameters dict. See keys below.
-        psf_func (str, optional): The psf model to use.  Can be any of
-            {'vectorial', 'scalar', or 'microscpsf'}.  Where 'microscpsf' uses the
-            `gLXYZFocalScan` function from MicroscPSF-Py (if installed). Defaults to
-            "vectorial".
-
-        valid params (all floats unless stated, all distances in microns):
-            NA:  Numerical Aperture. Defaults to 0.4 for excitation and 1.1 for emission
-            ni0: Immersion medium RI design value. Defaults to 1.33 ni:  Immersion
-            medium RI experimental value. Defaults to 1.33 ns:  Specimen refractive RI.
-            Defaults to 1.33 tg:  Coverslip thickness experimental value. Defaults to 0
-            (water immersion) tg0: Coverslip thickness design value. Defaults to 0
-            (water immersion) ti0: Working distance (immersion medium thickness) design
-            value.
-                 Defaults to 150
-            ng0: Coverslip RI design value. Defaults to 1.515 ng:  Coverslip RI
-            experimental value. Defaults to 1.515
+    Parameters
+    ----------
+    nx : int, optional
+        XY size of output PSF in pixels, must be odd. Defaults to 127.
+    nz : int, optional
+        Z size of output PSF in pixels, must be odd. Defaults to 127.
+    dxy : float, optional
+        XY Pixel size in sample space (microns). Defaults to 0.05.
+    dz : float, optional
+        Z step size of PSF in sample space. Defaults to 0.05
+    pz : int, optional
+        Depth of point source relative to coverslip in microns. Defaults to 0.
+    z_offset : int, optional
+        Defocus between the axial position of the excitation and the detection plane,
+        with respect to the detection lens. Defaults to 0.
+    x_offset : int, optional
+        Mismatch between the focal point of the excitation beam and the point source,
+        along the propogation direction of the excitation beam. Defaults to 0.
+    ex_wvl : float, optional
+        Emission wavelength in microns. Defaults to 0.488.
+    em_wvl : float, optional
+        Emission wavelength in microns. Defaults to 0.525.
+    ex_params : dict, optional
+        Microscope parameters dict for excitation. See optional keys below.
+    em_params : dict, optional
+        Microscope parameters dict for emission. See optional keys below.
+    psf_func : str, optional
+        The psf model to use.  Can be any of
+        {'vectorial', 'scalar', or 'microscpsf'}.  Where 'microscpsf' uses the
+        `gLXYZFocalScan` function from MicroscPSF-Py (if installed). Defaults to
+        "vectorial".
+
+    valid params (all floats unless stated, all distances in microns):
+        NA:  Numerical Aperture. Defaults to 0.4 for excitation and 1.1 for emission
+        ni0: Immersion medium RI design value. Defaults to 1.33 ni:  Immersion
+        medium RI experimental value. Defaults to 1.33 ns:  Specimen refractive RI.
+        Defaults to 1.33 tg:  Coverslip thickness experimental value. Defaults to 0
+        (water immersion) tg0: Coverslip thickness design value. Defaults to 0
+        (water immersion) ti0: Working distance (immersion medium thickness) design
+        value.
+                Defaults to 150
+        ng0: Coverslip RI design value. Defaults to 1.515 ng:  Coverslip RI
+        experimental value. Defaults to 1.515
 
-    Raises:
+    Raises
+    ------
         ImportError: If `psf_func` == 'microscpsf' and MicroscPSF-Py cannot be imported
         ValueError: If `psf_func` is not one of {'vectorial', 'scalar', or 'microscpsf'}
 
-    Returns:
+    Returns
+    -------
         3-tuple of np.ndarrays:  ex_psf, em_psf, total_system_psf
     """
-
     _x_params = _DEFAULT_PARAMS.copy()
     _x_params.update({"ni0": 1.33, "ni": 1.33, "ns": 1.33, "tg": 0, "tg0": 0})
     _x_params["NA"] = 0.4
     _m_params = _x_params.copy()
     _m_params["NA"] = 1.1
     if ex_params is not None:
         _x_params.update(ex_params)
@@ -526,28 +553,104 @@
 
     lim = (nx - 1) * dxy / 2
     emzvec = np.linspace(-lim + x_offset, lim + x_offset, nx)
     if np.mod(z_offset / dz, 1) != 0:
         z_offset = dz * np.round(z_offset / dz)
         warnings.warn(
             "Not Implemented: z_offset must be an even multiple of dz. "
-            "Coercing z_offset to nearest dz multiple: %s" % z_offset
+            "Coercing z_offset to nearest dz multiple: %s" % z_offset,
+            stacklevel=2,
         )
     _zoff = int(np.ceil(z_offset / dz))
     ex_nx = nz + 2 * np.abs(_zoff)
     exzvec = _centered_zv(nz, dz, pz)
 
     ex_psf = f(_x_params, dz, ex_nx, emzvec, pz=0, wvl=ex_wvl).T.sum(0)
     ex_psf = ex_psf[:nz] if _zoff >= 0 else ex_psf[-nz:]
     em_psf = f(_m_params, dxy, nx, exzvec, pz=pz, wvl=em_wvl)
 
     combined = ex_psf[:, :, np.newaxis] * em_psf
     return (ex_psf, em_psf, combined)
 
 
+def confocal_psf(
+    z: Union[int, Sequence[float]] = 51,
+    nx: int = 51,
+    *,
+    pinhole_au: float = 1.0,
+    dxy: float = 0.05,
+    dz: float = 0.05,
+    pz: float = 0.0,
+    NA: float = 1.4,
+    ex_wvl: float = 0.6,
+    em_wvl: float = 0.6,
+    ns: float = 1.47,
+    ni: float = 1.515,
+    ni0: float = 1.515,
+    tg: float = 170,
+    tg0: float = 170,
+    ng: float = 1.515,
+    ng0: float = 1.515,
+    ti0: float = 150.0,
+    oversample_factor: int = 3,
+    normalize: bool = True,
+    model: Literal["vectorial", "scalar", "gaussian"] = "vectorial",
+    pinhole_irrelevance_threshold: float = 50,
+):
+    kwargs = {
+        "z": z,
+        "nx": nx,
+        "dxy": dxy,
+        "dz": dz,
+        "pz": pz,
+        "NA": NA,
+        "ex_wvl": ex_wvl,
+        "em_wvl": em_wvl,
+        "ns": ns,
+        "ni": ni,
+        "ni0": ni0,
+        "tg": tg,
+        "tg0": tg0,
+        "ng": ng,
+        "ng0": ng0,
+        "ti0": ti0,
+        "oversample_factor": oversample_factor,
+        "normalize": normalize,
+        "model": model,
+    }
+    _ex_wvl = cast(float, kwargs.pop("ex_wvl"))
+    _em_wvl = cast(float, kwargs.pop("em_wvl"))
+    ex_psf = make_psf(wvl=_ex_wvl, **kwargs)  # type: ignore
+
+    if pinhole_au >= pinhole_irrelevance_threshold:
+        return ex_psf
+
+    em_psf = make_psf(wvl=_em_wvl, **kwargs)  # type: ignore
+
+    pinhole_size = pinhole_au * 0.61 * _em_wvl / NA
+    pinhole = _top_hat(nx, pinhole_size / dxy)
+
+    # convolve em_psf with pinhole, only in XY
+    em_psf = np.array([convolve2d(p, pinhole, mode="same") for p in em_psf])
+
+    return ex_psf * em_psf
+
+
+def _top_hat(nx: int, radius: float):
+    """Return a top hat function of size (nx, nx) and radius `radius`.
+
+    radius is in units of pixels. Everything inside of the radius is 1, everything
+    outside is 0.
+    """
+    x = np.arange(nx) - nx // 2
+    xx, yy = np.meshgrid(x, x)
+    r = np.sqrt(xx**2 + yy**2)
+    return (r <= radius).astype(int)
+
+
 __all__ = [
     "vectorial_psf",
     "vectorial_psf_deriv",
     "scalar_psf",
     "vectorial_psf_centered",
     "scalar_psf_centered",
     "vectorialXYZFocalScan",
```

### Comparing `psfmodels-0.3.2/src/psfmodels/_cuvec.py` & `psfmodels-0.3.3/src/psfmodels/_cuvec.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,24 @@
 import numpy as np
 
 try:
     import cupy as xp
     from cupyx.scipy.ndimage import map_coordinates
     from cupyx.scipy.special import j0, j1
 except ImportError:
-    import numpy as xp
-    from scipy.ndimage import map_coordinates
-    from scipy.special import j0, j1
+    try:
+        import jax.numpy as xp
+        from jax.scipy.ndimage import map_coordinates
+
+        from ._jax_bessel import j0, j1
+
+    except ImportError:
+        import numpy as xp
+        from scipy.ndimage import map_coordinates
+        from scipy.special import j0, j1
 
 
 @dataclass
 class Objective:
     na: float = 1.4  # numerical aperture
     coverslip_ri: float = 1.515  # coverslip RI experimental value (ng)
     coverslip_ri_spec: float = 1.515  # coverslip RI design value (ng0)
@@ -61,20 +68,39 @@
         return self.coverslip_thickness_spec * 1e-6
 
     @property
     def half_angle(self):
         return np.arcsin(self.na / self.ni)
 
 
-def _simp_like(arr):
-    simp = xp.empty_like(arr)
-    simp[::2] = 4
-    simp[1::2] = 2
-    simp[-1] = 1
-    return simp
+if xp.__name__ == "jax.numpy":
+
+    def _simp_like(arr):
+        simp = xp.empty_like(arr)
+
+        simp = simp.at[::2].set(4)
+        simp = simp.at[1::2].set(2)
+        simp = simp.at[-1].set(1)
+        return simp
+
+    def _array_assign(arr, mask, value):
+        return arr.at[mask].set(value)
+
+else:
+
+    def _simp_like(arr):
+        simp = xp.empty_like(arr)
+        simp[::2] = 4
+        simp[1::2] = 2
+        simp[-1] = 1
+        return simp
+
+    def _array_assign(arr, mask, value):
+        arr[mask] = value
+        return arr
 
 
 def simpson(
     p: Objective,
     theta: np.ndarray,
     constJ: np.ndarray,
     zv: np.ndarray,
@@ -110,15 +136,16 @@
 
     # 2.0 factor: Simpson's rule
     bessel_0 = simp * j0(constJ[:, xp.newaxis] * sintheta) * sintheta * sqrtcostheta
     bessel_1 = simp * j1(constJ[:, xp.newaxis] * sintheta) * sintheta * sqrtcostheta
 
     with np.errstate(invalid="ignore"):
         bessel_2 = 2.0 * bessel_1 / (constJ[:, xp.newaxis] * sintheta) - bessel_0
-    bessel_2[constJ == 0.0] = 0
+
+    bessel_2 = _array_assign(bessel_2, constJ == 0.0, 0)
 
     bessel_0 *= ts1ts2 + tp1tp2 / p.ns * nsroot
     bessel_1 *= tp1tp2 * p.ni / p.ns * sintheta
     bessel_2 *= ts1ts2 - tp1tp2 / p.ns * nsroot
 
     sum_I0 = xp.abs((expW * bessel_0).sum(-1))
     sum_I1 = xp.abs((expW * bessel_1).sum(-1))
@@ -178,35 +205,37 @@
     yi = yi - (ny - 1) / 2 - offy
     xi = xi - (nx - 1) / 2 - offx
     return xp.hypot(yi, xi)
 
 
 def rz_to_xyz(rz, xyshape, sf=3, off=None):
     """Use interpolation to create a 3D XYZ PSF from a 2D ZR PSF."""
-
     # Create XY grid of radius values.
     rmap = radius_map(xyshape, off) * sf
     nz = rz.shape[0]
     out = xp.zeros((nz, *xyshape))
+    out = []
     for z in range(nz):
         o = map_coordinates(
             rz, xp.asarray([xp.ones(rmap.size) * z, rmap.ravel()]), order=1
         ).reshape(xyshape)
-        out[z] = o
+        out.append(o)
+
+    out = xp.asarray(out)
     return out.get() if hasattr(out, "get") else out
 
 
 # def rz_to_xyz(rz, xyshape, sf=3, off=None):
 #     """Use interpolation to create a 3D XYZ PSF from a 2D ZR PSF."""
 #     # Create XY grid of radius values.
 #     rmap = radius_map(xyshape, off) * sf
 #     ny, nx = xyshape
 #     nz, nr = rz.shape
 #     ZZ, RR = xp.meshgrid(xp.arange(nz, dtype="float64"), rmap.ravel())
-#     o = map_coordinates(rz, xp.array([ZZ.ravel(), RR.ravel()]))
+#     o = map_coordinates(rz, xp.array([ZZ.ravel(), RR.ravel()]), order=1)
 #     return o.reshape((nx, ny, nz)).T
 
 
 def vectorial_psf(
     zv,
     nx=31,
     ny=None,
@@ -230,21 +259,21 @@
     lim = (nz - 1) * dz / 2
     return np.linspace(-lim + pz, lim + pz, nz)
 
 
 def vectorial_psf_centered(nz, dz=0.05, **kwargs):
     """Compute a vectorial model of the microscope point spread function.
 
-    The point source is always in the center of the output volume."""
+    The point source is always in the center of the output volume.
+    """
     zv = _centered_zv(nz, dz, kwargs.get("pz", 0))
     return vectorial_psf(zv, **kwargs)
 
 
 if __name__ == "__main__":
-
     zv = np.linspace(-3, 3, 61)
     from time import perf_counter
 
     t0 = perf_counter()
     psf = vectorial_psf(zv, nx=512)
     t1 = perf_counter()
     print(psf.shape)
```

### Comparing `psfmodels-0.3.2/src/psfmodels/_napari.py` & `psfmodels-0.3.3/src/psfmodels/_napari.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ni: Annotated[float, {**dRI, "label": "Imm. RI"}] = 1.515,
     ni0: Annotated[float, {**dRI, "label": "Imm. RI (spec)"}] = 1.515,
     tg: Annotated[int, {"min": 0, "max": 200, "label": "CS thickness (µm)"}] = 170,
     tg0: Annotated[int, {"min": 0, "max": 200, "label": "CS thickness (spec)"}] = 170,
     ng: Annotated[float, {**dRI, "label": "CS RI"}] = 1.515,
     ng0: Annotated[float, {**dRI, "label": "CS RI (spec)"}] = 1.515,
 ) -> "napari.types.ImageData":
-    """Generate 3D microscope PSF
+    """Generate 3D microscope PSF.
 
     Select from one of the following PSF models:
         vectorial:  Vectorial PSF (Aguet et al, 2009)
         scalar:     Scalar PSF model (Gibson & Lanni, 1992)
         gaussian:   Gaussian approximation (Zhang et al, 2007)
 
     Parameters
```

### Comparing `psfmodels-0.3.2/src/psfmodels.egg-info/PKG-INFO` & `psfmodels-0.3.3/src/psfmodels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: psfmodels
-Version: 0.3.2
+Version: 0.3.3
 Summary: Scalar and vectorial models of the microscope point spread function (PSF).
 Home-page: https://github.com/tlambert03/psfmodels
 Author: Talley Lambert
 Author-email: talley.lambert@gmail.com
 License: GPL-3.0
 Project-URL: Source Code, https://github.com/tlambert03/psfmodels
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: napari
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -161,9 +160,7 @@
 ## Lightsheet PSF utility function
 
 The `psfmodels.tot_psf()` function provides a quick way to simulate the total
 system PSF (excitation x detection) as might be observed on a light sheet
 microscope (currently, only strictly orthogonal illumination and detection are
 supported).  See the [lightsheet.ipynb](notebooks/lightsheet.ipynb) Jupyter notebook for
 examples.
-
-
```

### Comparing `psfmodels-0.3.2/src/psfmodels.egg-info/SOURCES.txt` & `psfmodels-0.3.3/src/psfmodels.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 LICENSE
 MANIFEST.in
 README.md
 fig.png
 pyproject.toml
 setup.cfg
 setup.py
-tox.ini
 .github/ISSUE_TEMPLATE.md
+.github/dependabot.yml
 .github/workflows/ci.yml
 notebooks/Untitled.ipynb
 notebooks/Untitled1.ipynb
 notebooks/Untitled2.ipynb
 notebooks/examples.ipynb
 notebooks/lightsheet.ipynb
 src/_psfmodels/psfmath.h
 src/_psfmodels/pythonBindings.cpp
 src/_psfmodels/scalarPSF.cpp
 src/_psfmodels/vectorialPSF.cpp
 src/_psfmodels-stubs/__init__.pyi
 src/psfmodels/__init__.py
 src/psfmodels/_core.py
 src/psfmodels/_cuvec.py
+src/psfmodels/_jax_bessel.py
 src/psfmodels/_napari.py
 src/psfmodels/_version.py
 src/psfmodels/napari.yaml
 src/psfmodels/py.typed
 src/psfmodels.egg-info/PKG-INFO
 src/psfmodels.egg-info/SOURCES.txt
 src/psfmodels.egg-info/dependency_links.txt
```

### Comparing `psfmodels-0.3.2/tests/test_psf.py` & `psfmodels-0.3.3/tests/test_psf.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,7 +33,15 @@
     p = psfm.scalar_psf(zvec, nx=31)
     assert p.shape == (5, 31, 31)
 
 
 def test_scalar_psf_centered():
     p = psfm.scalar_psf_centered(nx=31, nz=5)
     assert p.shape == (5, 31, 31)
+
+
+def test_confocal_psf():
+    zvec = np.linspace(-1, 1, 5)
+    p = psfm.confocal_psf(zvec, nx=31, pinhole_au=0.2)
+    assert p.shape == (5, 31, 31)
+    p = psfm.confocal_psf(zvec, nx=31, pinhole_au=3)
+    assert p.shape == (5, 31, 31)
```

