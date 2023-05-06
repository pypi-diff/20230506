# Comparing `tmp/Stixx-0.1.1.tar.gz` & `tmp/Stixx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Stixx-0.1.1.tar", last modified: Mon Mar 27 02:21:43 2023, max compression
+gzip compressed data, was "Stixx-0.1.2.tar", last modified: Sat May  6 20:50:42 2023, max compression
```

## Comparing `Stixx-0.1.1.tar` & `Stixx-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-03-27 02:21:43.050007 Stixx-0.1.1/
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)      290 2023-03-27 02:14:38.000000 Stixx-0.1.1/.bumpversion.cfg
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     5514 2023-03-26 01:28:57.000000 Stixx-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     3107 2023-03-26 01:28:57.000000 Stixx-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)    11990 2023-03-26 01:28:57.000000 Stixx-0.1.1/LICENSE
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)      402 2023-03-26 01:28:57.000000 Stixx-0.1.1/MANIFEST.in
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     2213 2023-03-27 02:14:38.000000 Stixx-0.1.1/Makefile
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)    17956 2023-03-27 02:21:43.046673 Stixx-0.1.1/PKG-INFO
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     3417 2023-03-27 00:44:34.000000 Stixx-0.1.1/README.md
-drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-03-27 02:21:43.046673 Stixx-0.1.1/Stixx.egg-info/
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)    17956 2023-03-27 02:21:42.000000 Stixx-0.1.1/Stixx.egg-info/PKG-INFO
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)      360 2023-03-27 02:21:43.000000 Stixx-0.1.1/Stixx.egg-info/SOURCES.txt
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)        1 2023-03-27 02:21:42.000000 Stixx-0.1.1/Stixx.egg-info/dependency_links.txt
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)      183 2023-03-27 02:21:42.000000 Stixx-0.1.1/Stixx.egg-info/requires.txt
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)        6 2023-03-27 02:21:42.000000 Stixx-0.1.1/Stixx.egg-info/top_level.txt
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     2201 2023-03-27 02:14:38.000000 Stixx-0.1.1/pyproject.toml
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)       38 2023-03-27 02:21:43.050007 Stixx-0.1.1/setup.cfg
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)       39 2023-03-26 01:28:57.000000 Stixx-0.1.1/setup.py
-drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-03-27 02:21:43.046673 Stixx-0.1.1/stixx/
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)      114 2023-03-27 02:14:38.000000 Stixx-0.1.1/stixx/__init__.py
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     4310 2023-03-27 02:14:38.000000 Stixx-0.1.1/stixx/game.py
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     1081 2023-03-27 02:14:38.000000 Stixx-0.1.1/stixx/players.py
-drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-03-27 02:21:43.046673 Stixx-0.1.1/stixx/tests/
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     4108 2023-03-27 00:44:34.000000 Stixx-0.1.1/stixx/tests/test_game.py
--rw-r--r--   0 mg4145    (1000) mg4145    (1000)     1567 2023-03-27 00:44:34.000000 Stixx-0.1.1/stixx/tests/test_players.py
+drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-05-06 20:50:42.216159 Stixx-0.1.2/
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      290 2023-05-06 20:10:49.000000 Stixx-0.1.2/.bumpversion.cfg
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      609 2023-05-06 20:49:16.000000 Stixx-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     5514 2023-05-06 03:37:16.000000 Stixx-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     3107 2023-05-06 03:37:16.000000 Stixx-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)    11990 2023-05-06 03:37:16.000000 Stixx-0.1.2/LICENSE
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      550 2023-05-06 20:49:16.000000 Stixx-0.1.2/MANIFEST.in
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     2625 2023-05-06 20:10:49.000000 Stixx-0.1.2/Makefile
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)    17312 2023-05-06 20:50:42.216159 Stixx-0.1.2/PKG-INFO
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     2773 2023-05-06 20:49:14.000000 Stixx-0.1.2/README.md
+drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-05-06 20:50:42.216159 Stixx-0.1.2/Stixx.egg-info/
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)    17312 2023-05-06 20:50:42.000000 Stixx-0.1.2/Stixx.egg-info/PKG-INFO
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      442 2023-05-06 20:50:42.000000 Stixx-0.1.2/Stixx.egg-info/SOURCES.txt
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)        1 2023-05-06 20:50:42.000000 Stixx-0.1.2/Stixx.egg-info/dependency_links.txt
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      183 2023-05-06 20:50:42.000000 Stixx-0.1.2/Stixx.egg-info/requires.txt
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)        6 2023-05-06 20:50:42.000000 Stixx-0.1.2/Stixx.egg-info/top_level.txt
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)   769222 2023-05-06 03:37:16.000000 Stixx-0.1.2/demo.gif
+drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-05-06 20:50:42.216159 Stixx-0.1.2/docs/
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      634 2023-05-06 03:37:16.000000 Stixx-0.1.2/docs/Makefile
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     2302 2023-05-06 20:29:52.000000 Stixx-0.1.2/docs/conf.py
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      959 2023-05-06 20:10:49.000000 Stixx-0.1.2/docs/index.md
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      765 2023-05-06 03:37:16.000000 Stixx-0.1.2/docs/make.bat
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     2201 2023-05-06 20:10:49.000000 Stixx-0.1.2/pyproject.toml
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)       38 2023-05-06 20:50:42.216159 Stixx-0.1.2/setup.cfg
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)       39 2023-05-06 03:37:16.000000 Stixx-0.1.2/setup.py
+drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-05-06 20:50:42.216159 Stixx-0.1.2/stixx/
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)      114 2023-05-06 20:10:49.000000 Stixx-0.1.2/stixx/__init__.py
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     6055 2023-05-06 20:10:49.000000 Stixx-0.1.2/stixx/game.py
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     1760 2023-05-06 03:37:16.000000 Stixx-0.1.2/stixx/players.py
+drwxr-xr-x   0 mg4145    (1000) mg4145    (1000)        0 2023-05-06 20:50:42.216159 Stixx-0.1.2/stixx/tests/
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     8787 2023-05-06 20:10:49.000000 Stixx-0.1.2/stixx/tests/test_game.py
+-rw-r--r--   0 mg4145    (1000) mg4145    (1000)     1567 2023-05-06 03:37:16.000000 Stixx-0.1.2/stixx/tests/test_players.py
```

### Comparing `Stixx-0.1.1/CODE_OF_CONDUCT.md` & `Stixx-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Stixx-0.1.1/CONTRIBUTING.md` & `Stixx-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Stixx-0.1.1/LICENSE` & `Stixx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Stixx-0.1.1/Makefile` & `Stixx-0.1.2/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #########
 # BUILD #
 #########
+
+# TMPREPO=/tmp/docs/stixx # used for docs
+TMPREPO=tmp
+
 develop:  ## install dependencies and build library
 	python -m pip install -e .[develop]
 
 build:  ## build the python library
 	python setup.py build build_ext --inplace
 
 install:  ## install library
 	python -m pip install .
 
 #########
 # LINTS #
 #########
 lint:  ## run static analysis with flake8
-	python -m black --check stixx setup.py #
-	python -m flake8 stixx setup.py #
+	python -m black --check stixx setup.py
+	python -m flake8 stixx setup.py
 
 # Alias
 lints: lint
 
 format:  ## run autoformatting with black
 	python -m black stixx/ setup.py
 
@@ -81,18 +85,31 @@
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
 
+docs: ## build the docs
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages: ## build the docs and push to gh-pages
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages https://github.com/mg4145/stixx.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
 ############################################################################################
 
 # Thanks to Francoise at marmelab.com for this
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
-.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help docs pages
```

### Comparing `Stixx-0.1.1/PKG-INFO` & `Stixx-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stixx
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple two-player video game.
 Author-email: Mauricio Guerrero <mg4145@columbia.edu>
 License: Copyright 2023 Mauricio Guerrero
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
@@ -240,46 +240,28 @@
 
 Stixx is an up and coming two-player game where the objective of the game is
 to deplete your opponent of their sticks. Players start with a stick in each of
 their hands and add sticks to the opponent based on how many sticks they
 currently have. If either player gets exactly five sticks, they lose said hand.
 
 <!-- ![GitHub](https://img.shields.io/github/license/mg4145/stixx)-->
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Issues](https://img.shields.io/github/issues/mg4145/stixx)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![Build Status](https://github.com/mg4145/stixx/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/mg4145/stixx/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/mg4145/stixx/branch/main/graph/badge.svg)](https://codecov.io/gh/mg4145/stixx)
-<!--[![PyPI](https://img.shields.io/pypi/v/stixx)](https://pypi.org/project/stixx/)-->
-
-
-<!--[![Codecov](https://codecov.io/gh/mg4145/stixx/branch/main/graph/badge.svg)][codecov]-->
+[![PyPI](https://img.shields.io/pypi/v/stixx)](https://pypi.org/project/stixx/)
+[![Docs](https://img.shields.io/readthedocs/stixx)](https://stixx.readthedocs.io/)
 
 # Overview
 Stixx is childhood game that many of us have played under different names or
 rules. The purpose of this project is to give back the nostalgia that this
 childhood game gave us. The current plan is to have a bare-bones UI of the game
 that works. There are also exciting plans in for future of this game.
-<!--
-[![PyPI](https://img.shields.io/pypi/v/stixx.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/stixx.svg)][status]
-[![Python Version](https://img.shields.io/pypi/pyversions/stixx)][python version]
-[![License](https://img.shields.io/pypi/l/stixx)][license]
-
-[![Read the documentation at https://stixx.readthedocs.io/](https://img.shields.io/readthedocs/stixx/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
-
-[pypi_]: https://pypi.org/project/stixx/
-[status]: https://pypi.org/project/stixx/
-[python version]: https://pypi.org/project/stixx
-[read the docs]: https://stixx.readthedocs.io/
-[codecov]: https://app.codecov.io/gh/mg4145/stixx
-[pre-commit]: https://github.com/pre-commit/pre-commit
--->
 
-[tests]: https://github.com/mg4145/stixx/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 <!--
 ## Features
 
 - TODO
 
@@ -292,21 +274,31 @@
 
 You can install _stixx_ via [pip] from [PyPI]:
 
 ```console
 $ pip install stixx
 ```
 
-## Usage
-
-<!--Please see the [Command-line Reference] for details. -->
-```python
-python game.py
+# Running
+  - Locate the directory
+```bash
+$ pip show stixx | grep "Location"
+```
+  - Once the location has been found change directories to said location
+  ```bash
+  $ cd <location>
+  ```
+  -  Run the game
+```bash
+$ python game.py
 ```
 
+## Demo
+![](demo.gif)
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `Stixx-0.1.1/README.md` & `Stixx-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,46 +2,28 @@
 
 Stixx is an up and coming two-player game where the objective of the game is
 to deplete your opponent of their sticks. Players start with a stick in each of
 their hands and add sticks to the opponent based on how many sticks they
 currently have. If either player gets exactly five sticks, they lose said hand.
 
 <!-- ![GitHub](https://img.shields.io/github/license/mg4145/stixx)-->
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Issues](https://img.shields.io/github/issues/mg4145/stixx)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![Build Status](https://github.com/mg4145/stixx/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/mg4145/stixx/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/mg4145/stixx/branch/main/graph/badge.svg)](https://codecov.io/gh/mg4145/stixx)
-<!--[![PyPI](https://img.shields.io/pypi/v/stixx)](https://pypi.org/project/stixx/)-->
-
-
-<!--[![Codecov](https://codecov.io/gh/mg4145/stixx/branch/main/graph/badge.svg)][codecov]-->
+[![PyPI](https://img.shields.io/pypi/v/stixx)](https://pypi.org/project/stixx/)
+[![Docs](https://img.shields.io/readthedocs/stixx)](https://stixx.readthedocs.io/)
 
 # Overview
 Stixx is childhood game that many of us have played under different names or
 rules. The purpose of this project is to give back the nostalgia that this
 childhood game gave us. The current plan is to have a bare-bones UI of the game
 that works. There are also exciting plans in for future of this game.
-<!--
-[![PyPI](https://img.shields.io/pypi/v/stixx.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/stixx.svg)][status]
-[![Python Version](https://img.shields.io/pypi/pyversions/stixx)][python version]
-[![License](https://img.shields.io/pypi/l/stixx)][license]
-
-[![Read the documentation at https://stixx.readthedocs.io/](https://img.shields.io/readthedocs/stixx/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
-
-[pypi_]: https://pypi.org/project/stixx/
-[status]: https://pypi.org/project/stixx/
-[python version]: https://pypi.org/project/stixx
-[read the docs]: https://stixx.readthedocs.io/
-[codecov]: https://app.codecov.io/gh/mg4145/stixx
-[pre-commit]: https://github.com/pre-commit/pre-commit
--->
 
-[tests]: https://github.com/mg4145/stixx/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 <!--
 ## Features
 
 - TODO
 
@@ -54,21 +36,31 @@
 
 You can install _stixx_ via [pip] from [PyPI]:
 
 ```console
 $ pip install stixx
 ```
 
-## Usage
-
-<!--Please see the [Command-line Reference] for details. -->
-```python
-python game.py
+# Running
+  - Locate the directory
+```bash
+$ pip show stixx | grep "Location"
+```
+  - Once the location has been found change directories to said location
+  ```bash
+  $ cd <location>
+  ```
+  -  Run the game
+```bash
+$ python game.py
 ```
 
+## Demo
+![](demo.gif)
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `Stixx-0.1.1/Stixx.egg-info/PKG-INFO` & `Stixx-0.1.2/Stixx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stixx
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple two-player video game.
 Author-email: Mauricio Guerrero <mg4145@columbia.edu>
 License: Copyright 2023 Mauricio Guerrero
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
@@ -240,46 +240,28 @@
 
 Stixx is an up and coming two-player game where the objective of the game is
 to deplete your opponent of their sticks. Players start with a stick in each of
 their hands and add sticks to the opponent based on how many sticks they
 currently have. If either player gets exactly five sticks, they lose said hand.
 
 <!-- ![GitHub](https://img.shields.io/github/license/mg4145/stixx)-->
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Issues](https://img.shields.io/github/issues/mg4145/stixx)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![Build Status](https://github.com/mg4145/stixx/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/mg4145/stixx/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/mg4145/stixx/branch/main/graph/badge.svg)](https://codecov.io/gh/mg4145/stixx)
-<!--[![PyPI](https://img.shields.io/pypi/v/stixx)](https://pypi.org/project/stixx/)-->
-
-
-<!--[![Codecov](https://codecov.io/gh/mg4145/stixx/branch/main/graph/badge.svg)][codecov]-->
+[![PyPI](https://img.shields.io/pypi/v/stixx)](https://pypi.org/project/stixx/)
+[![Docs](https://img.shields.io/readthedocs/stixx)](https://stixx.readthedocs.io/)
 
 # Overview
 Stixx is childhood game that many of us have played under different names or
 rules. The purpose of this project is to give back the nostalgia that this
 childhood game gave us. The current plan is to have a bare-bones UI of the game
 that works. There are also exciting plans in for future of this game.
-<!--
-[![PyPI](https://img.shields.io/pypi/v/stixx.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/stixx.svg)][status]
-[![Python Version](https://img.shields.io/pypi/pyversions/stixx)][python version]
-[![License](https://img.shields.io/pypi/l/stixx)][license]
-
-[![Read the documentation at https://stixx.readthedocs.io/](https://img.shields.io/readthedocs/stixx/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
-
-[pypi_]: https://pypi.org/project/stixx/
-[status]: https://pypi.org/project/stixx/
-[python version]: https://pypi.org/project/stixx
-[read the docs]: https://stixx.readthedocs.io/
-[codecov]: https://app.codecov.io/gh/mg4145/stixx
-[pre-commit]: https://github.com/pre-commit/pre-commit
--->
 
-[tests]: https://github.com/mg4145/stixx/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 <!--
 ## Features
 
 - TODO
 
@@ -292,21 +274,31 @@
 
 You can install _stixx_ via [pip] from [PyPI]:
 
 ```console
 $ pip install stixx
 ```
 
-## Usage
-
-<!--Please see the [Command-line Reference] for details. -->
-```python
-python game.py
+# Running
+  - Locate the directory
+```bash
+$ pip show stixx | grep "Location"
+```
+  - Once the location has been found change directories to said location
+  ```bash
+  $ cd <location>
+  ```
+  -  Run the game
+```bash
+$ python game.py
 ```
 
+## Demo
+![](demo.gif)
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `Stixx-0.1.1/pyproject.toml` & `Stixx-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "Stixx"
 authors = [{name = "Mauricio Guerrero", email = "mg4145@columbia.edu"}]
 description="A simple two-player video game."
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.9.15"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `Stixx-0.1.1/stixx/game.py` & `Stixx-0.1.2/stixx/game.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,93 @@
-""" Game module """
+"""Stixx game module.
+
+This module contains the Game class and the main function.
+To play the game, run this module.
+
+
+Typical usage example:
+    player_1 = Player(input("Player 1 name: ").strip())
+    player_2 = Player(input("Player 2 name: ").strip())
+    stixx_game = Game(player_1, player_2)
+    stixx_game.play()
+
+"""
 
 import players
 from players import Player
 import random
 
 
 # TODO: Create is_valid method for Player class to check if the move is valid
 # TODO: Add an extra move for the players
 
 
 class Game:
-    """Game class"""
+    """Game class for the Stixx game.
+
+    This class contains the game logic and the game play.
+
+    Attributes:
+        player1: The first player.
+        player2: The second player.
+        current_player: The current player.
+        opponent: The opponent of the current player.
+        winner: The winner of the game.
+    """
 
     def __init__(self, player1: players.Player, player2: players.Player) -> None:
-        """Initialize a new game"""
+        """Initialize a new game.
+
+        Args:
+            player1: The first player.
+            player2: The second player.
+        """
+
         self.player1 = player1
         self.player2 = player2
         self.current_player = self.coin_toss()
         self.opponent = self.player1 if self.current_player == self.player2 else self.player2
         self.winner = None
 
+        self.value = 0
+        self.which_hand = None
+        self.opponent_hand = None
+
     def coin_toss(self) -> players.Player:
-        """Randomly select who goes first"""
+        """Randomly select who goes first."""
         return random.choice([self.player1, self.player2])
 
     def is_over(self) -> bool:
-        """Check if the game is over"""
+        """Check if the game is over."""
         return self.player1.is_both_empty() or self.player2.is_both_empty()
 
     def get_winner(self) -> None:
-        """Get the winner of the game"""
+        """Get the winner of the game."""
         if self.player1.is_both_empty():
             self.winner = self.player2.name
         elif self.player2.is_both_empty():
             self.winner = self.player1.name
 
     def valid_input(self, hand: str) -> bool:
-        """Check if the hand is valid"""
+        """Check if the hand is valid."""
         if hand != "L" and hand != "R":
             return False
         return True
 
     def switch_players(self) -> None:
-        """Switch players"""
+        """Switch players."""
         self.current_player, self.opponent = self.opponent, self.current_player
 
     def prompt_dialog(self, which_dialog: str) -> None:
-        """Print the dialog of the game"""
+        """Print the dialog of the game.
+
+        Args:
+            which_dialog: The dialog to print.
+        """
+
         LINE = "-" * 80
         if which_dialog == "start":
             print(LINE + f"\n{self.current_player.name} goes first!")
 
         elif which_dialog == "turn":
             line_1 = f"\n{self.current_player.name} it's your turn!"
             line_2 = f"\nYour current hand is: {self.current_player.current_hand()}"
@@ -65,49 +102,73 @@
             line_2 = "\nFinal Hands: "
             line_3 = f"\n{self.player1.name}: {self.player1.current_hand()}"
             line_4 = f"\n{self.player2.name}: {self.player2.current_hand()}\n"
 
             dialog = LINE.replace("-", "*") + line_1 + line_2 + line_3 + line_4 + LINE.replace("-", "*")
             print(dialog)
 
+        elif which_dialog == "invalid":
+            line_1 = "\nInvalid input!\nPlease type \"R\" or \"L\""
+            line_2 = f"\nYour current hand is: {self.current_player.current_hand()}"
+            line_3 = f"\n{self.opponent.name}'s hand is: {self.opponent.current_hand()}\n"
+
+            dialog = LINE + line_1 + line_2 + line_3
+            print(dialog)
+
+        elif which_dialog == "empty":
+            line_1 = "\nHand is empty!\nPlease try again."
+            line_2 = f"\nYour current hand is: {self.current_player.current_hand()}"
+            line_3 = f"\n{self.opponent.name}'s hand is: {self.opponent.current_hand()}\n"
+
+            dialog = LINE + line_1 + line_2 + line_3
+            print(dialog)
+
+    def select_hand(self) -> None:
+        """Get the move of the current player."""
+        while True:
+            self.which_hand = input("Which hand? (L/R): ").strip().upper()
+            if not self.valid_input(self.which_hand):
+                self.prompt_dialog("invalid")
+            elif self.current_player.is_empty(self.which_hand):
+                self.prompt_dialog("empty")
+            else:
+                if self.which_hand == "L":
+                    self.value = self.current_player.left
+                else:
+                    self.value = self.current_player.right
+                break
+
+    def select_hand_opponent(self) -> None:
+        """Select the opponent's hand."""
+        while True:
+            self.opponent_hand = input("Which opponent's hand? (L/R): ").strip().upper()
+            if not self.valid_input(self.opponent_hand):
+                self.prompt_dialog("invalid")
+            elif self.opponent.is_empty(self.opponent_hand):
+                self.prompt_dialog("empty")
+            else:
+                self.opponent.update(self.opponent_hand, self.value)
+                break
+
     def play(self) -> None:
         """Play the game"""
 
         # Print the start dialog
         self.prompt_dialog("start")
 
         # Play the game
         while True:
             # Print the dialog of the game
             self.prompt_dialog("turn")
 
-            # Get the current player's move
-            while True:
-                which_hand = input("Which hand? (L/R): ").strip().upper()
-                if not self.valid_input(which_hand):
-                    print("Invalid input!\nPlease type \"R\" or \"L\"")
-                elif self.current_player.is_empty(which_hand):
-                    print("Hand is empty!\nPlease try again.")
-                else:
-                    if which_hand == "L":
-                        value = self.current_player.left
-                    else:
-                        value = self.current_player.right
-                    break
-
-            # Get the opponent's move
-            while True:
-                opponent_hand = input("Which opponent's hand? (L/R): ").strip().upper()
-                if not self.valid_input(opponent_hand):
-                    print("Invalid input!\nPlease type \"R\" or \"L\"")
-                elif self.opponent.is_empty(opponent_hand):
-                    print("Opponent's hand is empty!\nPlease try again.")
-                else:
-                    self.opponent.update(opponent_hand, value)
-                    break
+            # Current player select hand
+            self.select_hand()
+
+            # Current player select opponent's hand
+            self.select_hand_opponent()
 
             # Check if the game is over
             if self.is_over():
                 self.prompt_dialog("over")
                 break
 
             # Switch players
```

### Comparing `Stixx-0.1.1/stixx/tests/test_players.py` & `Stixx-0.1.2/stixx/tests/test_players.py`

 * *Files identical despite different names*

