# Comparing `tmp/katalytic-maths-0.1.0.tar.gz` & `tmp/katalytic-maths-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-maths-0.1.0.tar", last modified: Tue May  2 03:53:37 2023, max compression
+gzip compressed data, was "katalytic-maths-0.2.0.tar", last modified: Sat May  6 04:59:10 2023, max compression
```

## Comparing `katalytic-maths-0.1.0.tar` & `katalytic-maths-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-maths-0.1.0/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-maths-0.1.0/.gitignore
--rw-r--r--   0        0        0     3258 2023-04-30 14:18:45.239106 katalytic-maths-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1013 2023-05-02 03:53:19.223037 katalytic-maths-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-maths-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2122 2023-04-30 14:21:08.547541 katalytic-maths-0.1.0/README.md
--rw-r--r--   0        0        0     1290 2023-05-02 03:53:19.223037 katalytic-maths-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3376 2023-05-02 03:50:19.477953 katalytic-maths-0.1.0/src/katalytic/maths.py
--rw-r--r--   0        0        0     3868 2023-05-02 03:49:54.957201 katalytic-maths-0.1.0/tests/test_maths.py
--rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 katalytic-maths-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-maths-0.2.0/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-maths-0.2.0/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic-maths-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1181 2023-05-06 04:58:46.888399 katalytic-maths-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-maths-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1819 2023-05-03 04:08:20.003050 katalytic-maths-0.2.0/README.md
+-rw-r--r--   0        0        0     1281 2023-05-06 04:58:46.852399 katalytic-maths-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3381 2023-05-05 17:42:36.449173 katalytic-maths-0.2.0/src/katalytic/maths/__init__.py
+-rw-r--r--   0        0        0    11398 2023-05-06 04:43:38.312592 katalytic-maths-0.2.0/src/katalytic/maths/bboxes.py
+-rw-r--r--   0        0        0    13156 2023-05-06 04:53:18.580396 katalytic-maths-0.2.0/tests/test_bboxes.py
+-rw-r--r--   0        0        0     3868 2023-05-02 05:45:43.867514 katalytic-maths-0.2.0/tests/test_maths.py
+-rw-r--r--   0        0        0     2986 1970-01-01 00:00:00.000000 katalytic-maths-0.2.0/PKG-INFO
```

### Comparing `katalytic-maths-0.1.0/.gitignore` & `katalytic-maths-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-maths-0.1.0/.gitlab-ci.yml` & `katalytic-maths-0.2.0/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 include:
 - template: Security/SAST.gitlab-ci.yml
 
-image: python:3.9
+image: python:3.6
 
 stages:
   - coverage
   - test
   - security
   - release
 
 variables:
-  TOX_ENV: py39
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_CACHE_DIR: "off"
 
 coverage:
   image: python:3.6
   stage: coverage
   script:
```

### Comparing `katalytic-maths-0.1.0/CHANGELOG.md` & `katalytic-maths-0.2.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.2.0 (2023-05-06)
+### feat
+- [[`526f61a`](https://gitlab.com/katalytic/katalytic-maths/commit/526f61afcabab4f37c530cbf4e18ae5ebe01af9d)] add functions for bboxes
+
+
 ## 0.1.0 (2023-05-02)
 ### feat
 - [[`a5a76fc`](https://gitlab.com/katalytic/katalytic-maths/commit/a5a76fcf6a11ace8f1c8a42cb59e281638dc2a78)] add L1, L2, min_max, and clip
 ### fix
 - [[`da40700`](https://gitlab.com/katalytic/katalytic-maths/commit/da40700a0443156aabd69d78945d805a17210bac)] **min_max:** 'NoneType' object is not callable
```

### Comparing `katalytic-maths-0.1.0/LICENSE.txt` & `katalytic-maths-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-maths-0.1.0/README.md` & `katalytic-maths-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,27 @@
 [![coverage](https://gitlab.com/katalytic/katalytic-maths/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-maths/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-maths.svg)](https://katalytic-maths.readthedocs.io/en/latest/)
 [![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
-pip install katalytic-images
+pip install katalytic-maths
 ```
 
 As part of the [katalytic](https://gitlab.com/katalytic/katalytic) collection
 ```bash
 pip install katalytic
 ```
 
 ## Usage
 TODO: Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
 
 ## Roadmap
-- make pillow an optional dependency.
-	- setup_load_image() should pick opencv if pillow is not available
-- drawing on images with a declarative interface
-- image thresholding and masking operations
-- interactive data exploration widgets (maybe as part of another package)
-- higher level API on top of opencv
+- TODO
 
 ## Contributing
 Contributions can be made in a number of ways:
 - Propose architectural or API improvements
 - Propose new features
 - Propose packaging, building, or deployment improvements
 - Report and fix bugs
```

### Comparing `katalytic-maths-0.1.0/pyproject.toml` & `katalytic-maths-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-maths"
-version = "0.1.0"
+version = "0.2.0"
 description = "This plugin adds utilities for mathematical tasks"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -22,23 +22,23 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
-    "katalytic-checks>=0.0.1",
-    "katalytic-data>=0.5.0",
-    "katalytic-pkg>=0.2.0",
+    "katalytic-data>=0.9.0",
+    "katalytic-pkg>=0.4.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
+    "pytest-clarity",
     "pytest-randomly",
 ]
 
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-maths.git"
 repository = "https://gitlab.com/katalytic/katalytic-maths.git"
```

### Comparing `katalytic-maths-0.1.0/src/katalytic/maths.py` & `katalytic-maths-0.2.0/src/katalytic/maths/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 
-from katalytic.checks import is_number, is_sequence, is_iterable, is_iterator
+from katalytic.data.checks import is_number, is_sequence, is_iterable, is_iterator
 from katalytic.pkg import get_version
 
 __version__, __version_info__ = get_version(__name__)
 _UNDEFINED = object()
 
 
 def L1(a, b):
```

### Comparing `katalytic-maths-0.1.0/tests/test_maths.py` & `katalytic-maths-0.2.0/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `katalytic-maths-0.1.0/PKG-INFO` & `katalytic-maths-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-maths
-Version: 0.1.0
+Version: 0.2.0
 Summary: This plugin adds utilities for mathematical tasks
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -12,19 +12,19 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Dist: katalytic-checks>=0.0.1
-Requires-Dist: katalytic-data>=0.5.0
-Requires-Dist: katalytic-pkg>=0.2.0
+Requires-Dist: katalytic-data>=0.9.0
+Requires-Dist: katalytic-pkg>=0.4.0
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-maths.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-maths.git
 Provides-Extra: dev
 
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
@@ -34,32 +34,27 @@
 [![coverage](https://gitlab.com/katalytic/katalytic-maths/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-maths/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-maths.svg)](https://katalytic-maths.readthedocs.io/en/latest/)
 [![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
-pip install katalytic-images
+pip install katalytic-maths
 ```
 
 As part of the [katalytic](https://gitlab.com/katalytic/katalytic) collection
 ```bash
 pip install katalytic
 ```
 
 ## Usage
 TODO: Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
 
 ## Roadmap
-- make pillow an optional dependency.
-	- setup_load_image() should pick opencv if pillow is not available
-- drawing on images with a declarative interface
-- image thresholding and masking operations
-- interactive data exploration widgets (maybe as part of another package)
-- higher level API on top of opencv
+- TODO
 
 ## Contributing
 Contributions can be made in a number of ways:
 - Propose architectural or API improvements
 - Propose new features
 - Propose packaging, building, or deployment improvements
 - Report and fix bugs
```

