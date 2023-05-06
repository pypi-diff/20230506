# Comparing `tmp/loggerml-1.0.0.tar.gz` & `tmp/loggerml-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerml-1.0.0.tar", last modified: Fri May  5 22:37:05 2023, max compression
+gzip compressed data, was "loggerml-1.1.0.tar", last modified: Sat May  6 01:13:39 2023, max compression
```

## Comparing `loggerml-1.0.0.tar` & `loggerml-1.1.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.998105 loggerml-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 22:36:41.000000 loggerml-1.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.982105 loggerml-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.990105 loggerml-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 22:36:41.000000 loggerml-1.0.0/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 22:36:41.000000 loggerml-1.0.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-05 22:36:41.000000 loggerml-1.0.0/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 22:36:41.000000 loggerml-1.0.0/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-05 22:36:41.000000 loggerml-1.0.0/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-05 22:36:41.000000 loggerml-1.0.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-05 22:36:41.000000 loggerml-1.0.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-05 22:36:41.000000 loggerml-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-05 22:36:41.000000 loggerml-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-05 22:36:41.000000 loggerml-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-05 22:36:41.000000 loggerml-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-05 22:37:04.998105 loggerml-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-05 22:36:41.000000 loggerml-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-05 22:36:41.000000 loggerml-1.0.0/README_pipy.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.990105 loggerml-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.994105 loggerml-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   234446 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/_static/advanced.gif
--rw-r--r--   0 runner    (1001) docker     (123)    45761 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/_static/advanced.png
--rw-r--r--   0 runner    (1001) docker     (123)   501978 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/_static/base.gif
--rw-r--r--   0 runner    (1001) docker     (123)    28005 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/_static/base.png
--rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/_static/no_n_batches.png
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/_static/regex.png
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/contribute.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.994105 loggerml-1.0.0/docs/features/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/features/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/features/no_batches.md
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/features/regex.md
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/features/with_tracker.md
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/logml_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-05 22:36:41.000000 loggerml-1.0.0/docs/vs_tqdm.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.994105 loggerml-1.0.0/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 22:36:41.000000 loggerml-1.0.0/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 22:36:41.000000 loggerml-1.0.0/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 22:36:41.000000 loggerml-1.0.0/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-05 22:36:41.000000 loggerml-1.0.0/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-05 22:36:41.000000 loggerml-1.0.0/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.994105 loggerml-1.0.0/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-05 22:36:41.000000 loggerml-1.0.0/licenses_tier/RICH_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.994105 loggerml-1.0.0/loggerml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-05 22:37:04.000000 loggerml-1.0.0/loggerml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-05 22:37:04.000000 loggerml-1.0.0/loggerml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:37:04.000000 loggerml-1.0.0/loggerml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 22:37:04.000000 loggerml-1.0.0/loggerml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 22:37:04.000000 loggerml-1.0.0/loggerml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.998105 loggerml-1.0.0/logml/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-05 22:36:41.000000 loggerml-1.0.0/logml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 22:37:04.000000 loggerml-1.0.0/logml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20836 2023-05-05 22:36:41.000000 loggerml-1.0.0/logml/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-05 22:36:41.000000 loggerml-1.0.0/logml/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-05 22:36:41.000000 loggerml-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 22:36:41.000000 loggerml-1.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 22:36:41.000000 loggerml-1.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.998105 loggerml-1.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-05 22:36:41.000000 loggerml-1.0.0/scripts/integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-05 22:36:41.000000 loggerml-1.0.0/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:37:04.998105 loggerml-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 22:36:41.000000 loggerml-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.986105 loggerml-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.998105 loggerml-1.0.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-05 22:36:41.000000 loggerml-1.0.0/tests/integration/inte_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 22:36:41.000000 loggerml-1.0.0/tests/integration/inte_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-05 22:36:41.000000 loggerml-1.0.0/tests/integration/inte_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 22:36:41.000000 loggerml-1.0.0/tests/integration/inte_two_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:37:04.998105 loggerml-1.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-05 22:36:41.000000 loggerml-1.0.0/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 22:36:41.000000 loggerml-1.0.0/tests/unit/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.973788 loggerml-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-06 01:13:18.000000 loggerml-1.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.953788 loggerml-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.957788 loggerml-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-06 01:13:18.000000 loggerml-1.1.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 01:13:18.000000 loggerml-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-06 01:13:18.000000 loggerml-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-06 01:13:18.000000 loggerml-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 01:13:18.000000 loggerml-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-06 01:13:39.973788 loggerml-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-06 01:13:18.000000 loggerml-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-06 01:13:18.000000 loggerml-1.1.0/README_pipy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.961788 loggerml-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.961788 loggerml-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   234446 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/advanced.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    45761 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/advanced.png
+-rw-r--r--   0 runner    (1001) docker     (123)   501978 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/base.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    28005 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/base.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/no_n_batches.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/_static/regex.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/contribute.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.965788 loggerml-1.1.0/docs/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/features/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/features/no_batches.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/features/regex.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/features/with_tracker.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/logml_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-06 01:13:18.000000 loggerml-1.1.0/docs/vs_tqdm.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.965788 loggerml-1.1.0/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-06 01:13:18.000000 loggerml-1.1.0/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.965788 loggerml-1.1.0/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-06 01:13:18.000000 loggerml-1.1.0/licenses_tier/RICH_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.969788 loggerml-1.1.0/loggerml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 01:13:39.000000 loggerml-1.1.0/loggerml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.969788 loggerml-1.1.0/logml/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-06 01:13:18.000000 loggerml-1.1.0/logml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 01:13:39.000000 loggerml-1.1.0/logml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-05-06 01:13:18.000000 loggerml-1.1.0/logml/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-06 01:13:18.000000 loggerml-1.1.0/logml/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-06 01:13:18.000000 loggerml-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 01:13:18.000000 loggerml-1.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 01:13:18.000000 loggerml-1.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.969788 loggerml-1.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-06 01:13:18.000000 loggerml-1.1.0/scripts/integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-06 01:13:18.000000 loggerml-1.1.0/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:13:39.973788 loggerml-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 01:13:18.000000 loggerml-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.953788 loggerml-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.973788 loggerml-1.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_multi_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/integration/inte_two_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:13:39.973788 loggerml-1.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-06 01:13:18.000000 loggerml-1.1.0/tests/unit/test_time_utils.py
```

### Comparing `loggerml-1.0.0/.github/workflows/pipy_deployment.yaml` & `loggerml-1.1.0/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/.github/workflows/pydocstyle.yaml` & `loggerml-1.1.0/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/.github/workflows/pylint.yaml` & `loggerml-1.1.0/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/.github/workflows/tests.yaml` & `loggerml-1.1.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/.pylintrc` & `loggerml-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/CONTRIBUTING.md` & `loggerml-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/LICENSE` & `loggerml-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/PKG-INFO` & `loggerml-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 1.0.0
+Version: 1.1.0
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-1.0.0/README.md` & `loggerml-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -151,22 +151,20 @@
 ```
 
 Everyone can contribute to LogML, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ### Todo
 
-Priority:
-
-- [ ] Finalize tests for 1.0.0 major release
-
-Secondary:
+To do:
 
 Done:
 
+- [x] Allow multiple logs on the same batch
+- [x] Finalize tests for 1.0.0 major release
 - [x] Add docs sections: comparison with tqdm and how to use mean_vals
   (with exp tracker)
 - [x] Use regex for `styles`, `sizes` and `average` keys
 - [x] Be compatible with notebooks
 - [x] Get back the cursor when interrupting the training
 - [x] `logger.tqdm()` feature (used like `tqdm.tqdm`)
 - [x] Doc with Sphinx
```

### Comparing `loggerml-1.0.0/README_pipy.md` & `loggerml-1.1.0/README_pipy.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/Makefile` & `loggerml-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/_static/advanced.gif` & `loggerml-1.1.0/docs/_static/advanced.gif`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/_static/advanced.png` & `loggerml-1.1.0/docs/_static/advanced.png`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/_static/base.gif` & `loggerml-1.1.0/docs/_static/base.gif`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/_static/base.png` & `loggerml-1.1.0/docs/_static/base.png`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/_static/no_n_batches.png` & `loggerml-1.1.0/docs/_static/no_n_batches.png`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/_static/regex.png` & `loggerml-1.1.0/docs/_static/regex.png`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/conf.py` & `loggerml-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/contribute.md` & `loggerml-1.1.0/docs/contribute.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 
 Everyone can contribute to LogML, and we value everyone’s contributions. Please see our
 [contributing guidelines](https://github.com/valentingol/logml/blob/main/CONTRIBUTING.md)
 for more information 🤗
 
 ## Todo list
 
-Priority:
-
-- [ ] Finalize tests for 1.0.0 major release
-
-Secondary:
+To do:
 
 Done:
 
+- [x] Allow multiple logs on the same batch
+- [x] Finalize tests for 1.0.0 major release
 - [x] Add docs sections: comparison with tqdm and how to use mean_vals
   (with exp tracker)
 - [x] Use regex for `styles`, `sizes` and `average` keys
 - [x] Be compatible with notebooks
 - [x] Get back the cursor when interrupting the training
 - [x] `logger.tqdm()` feature (used like `tqdm.tqdm`)
 - [x] Doc with Sphinx
```

### Comparing `loggerml-1.0.0/docs/features/no_batches.md` & `loggerml-1.1.0/docs/features/no_batches.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/features/regex.md` & `loggerml-1.1.0/docs/features/regex.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/features/with_tracker.md` & `loggerml-1.1.0/docs/features/with_tracker.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/index.rst` & `loggerml-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/license.md` & `loggerml-1.1.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/make.bat` & `loggerml-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/quickstart.md` & `loggerml-1.1.0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/docs/vs_tqdm.md` & `loggerml-1.1.0/docs/vs_tqdm.md`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/github_actions_utils/pydocstyle_manager.py` & `loggerml-1.1.0/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/github_actions_utils/pylint_manager.py` & `loggerml-1.1.0/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/github_actions_utils/pytest_manager.py` & `loggerml-1.1.0/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/licenses_tier/RICH_LICENSE` & `loggerml-1.1.0/licenses_tier/RICH_LICENSE`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/loggerml.egg-info/PKG-INFO` & `loggerml-1.1.0/loggerml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerml
-Version: 1.0.0
+Version: 1.1.0
 Summary: Log your ml training in the console in an attractive way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/logml
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `loggerml-1.0.0/loggerml.egg-info/SOURCES.txt` & `loggerml-1.1.0/loggerml.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -51,12 +51,13 @@
 logml/__init__.py
 logml/_version.py
 logml/logger.py
 logml/time_utils.py
 scripts/integration-tests.sh
 scripts/pre-commit-checks.sh
 tests/integration/inte_logger.py
+tests/integration/inte_multi_logs.py
 tests/integration/inte_regex.py
 tests/integration/inte_tqdm.py
 tests/integration/inte_two_loggers.py
 tests/unit/test_logger.py
 tests/unit/test_time_utils.py
```

### Comparing `loggerml-1.0.0/logml/__init__.py` & `loggerml-1.1.0/logml/__init__.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/logml/logger.py` & `loggerml-1.1.0/logml/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,17 +74,17 @@
     step : int
         Number of batches seen since the beginning.
     current_epoch : int
         Current epoch number (starting at 1).
     current_batch : int
         Current batch number (starting at 1).
     vals : Dict[str, VarType]
-        Last values called inside log (not averaged or resized).
+        Last values called inside log (not averaged nor resized).
     mean_vals : Dict[str, VarType]
-        Current mean values.
+        Current mean values (only numerical values).
     """
 
     def __init__(
         self,
         n_epochs: int,
         n_batches: Optional[int],
         log_interval: Optional[int] = 1,
@@ -100,28 +100,28 @@
         name_style: str = '',
     ) -> None:
         # Log parameters
         self.silent = silent
         self.name = name
         self.show_bar = show_bar
         self.show_time = show_time
-        # Default configs
-        self.name_style = name_style
-        self.default_styles = styles
-        self.default_sizes = sizes
-        self.default_average: Dict = {key: True for key in average} if average else {}
         self.bold_keys = bold_keys
+        # Default log configs
+        self.name_style = name_style
+        self._default_styles = styles
+        self._default_sizes = sizes
+        self._default_average: Dict = {key: True for key in average} if average else {}
         # Internal variables
         self.n_epochs = n_epochs
         self.n_batches = n_batches
         self.log_interval = log_interval
         self.step = 0
-        self.t_glob = 0.0
-        self.start()  # Now, self.t_glob = time.time()
-        self.t_epoch = 0.0
+        self._glob_time = 0.0
+        self.start()  # Now, self._glob_time = time.time()
+        self._epoch_time = 0.0
         self.current_epoch = 0
         self.current_batch = 0
         self._on_tqdm = False
         self._just_new_epoch = False
         # Internal values
         self.vals: Dict = {}  # Last vals called inside log
         self._counts: Dict = {}
@@ -129,35 +129,42 @@
         # Rich elements
         self.live = Live(
             renderable=None,
             console=RICH_CONSOLE,
             refresh_per_second=4,
             auto_refresh=False,
         )
-        self.renderable = None
+        self._renderable = None
         self.console = RICH_CONSOLE
+        # Table and message infos from the previous log of the same batch
+        self._prev_tables_list: List[Table] = []
+        self._prev_table_width = 0
+        self._prev_row: List[Text] = []
+        self._prev_flat_cell = True
+        self._prev_message = ''
+        # Force live display to end at exit
         atexit.register(self.stop)
 
     def log(
         self,
         values: Dict[str, VarType],
         *,
-        message: Optional[str] = None,
+        message: str = '',
         styles: Union[Dict[str, str], str, None] = None,
         sizes: Union[Dict[str, int], int, None] = None,
         average: Optional[List[str]] = None,
     ) -> None:
         """Log the values with style.
 
         Parameters
         ----------
         values : Dict[str, Any]
             Values to log. E.g. {'loss': 0.1, 'acc': 0.9}
-        message : Optional[str], optional
-            Message to display at the end of the log. By default None.
+        message : str, optional
+            Message to display at the end of the log. By default empty.
         styles : Union[Dict, str, None], optional
             Style of the values. Include color, bold, italic and more
             See https://rich.readthedocs.io/en/stable/style.html for more details.
             E.g.::
 
                 {'loss': 'bold red', 'acc': 'italic #af00ff'}
 
@@ -205,30 +212,30 @@
                 values,
                 styles=styles,  # type: ignore
                 sizes=sizes,  # type: ignore
                 average=average_dict,
             )
             renderables.append(vals_table)
         # Build message (if exists)
-        if message:
+        if message or self._prev_message:
             renderables.append(self._build_message(message))
 
         # Create renderable group and update the live display
-        self.renderable = Group(*renderables)
+        self._renderable = Group(*renderables)
         refresh = (
             # auto refresh regularly if no log interval
             self.log_interval is None
             # refresh at log intervals
             or self.current_batch % self.log_interval == 0
             # refresh at first batch
             or self.current_batch == 1
             # refresh at last batch (if n_batches is specified)
             or (self.n_batches and self.current_batch == self.n_batches)
         )
-        self.live.update(renderable=self.renderable, refresh=refresh)
+        self.live.update(renderable=self._renderable, refresh=refresh)
 
     def tqdm(
         self,
         iterable: Iterable,
         *,
         reset_means: bool = True,
     ) -> Any:
@@ -279,37 +286,43 @@
             self.mean_vals = {key: 0 for key in self.mean_vals}
         self.live = Live(
             renderable=None,
             console=RICH_CONSOLE,
             refresh_per_second=4,
             auto_refresh=False,
         )
-        self.renderable = None
+        self._renderable = None
         # "Detach" the logs from the previous epoch
         self.detach()
         # Update epoch and batch
         self.current_epoch += 1
         self.current_batch = 0
         # Start the new live display
         self.live.start()
         # Set the new epoch start time
-        self.t_epoch = time.time()
+        self._epoch_time = time.time()
 
     def start_epoch(self, *, reset_means: bool = True) -> None:
         """Declare a new epoch. Alias for :meth:`new_epoch`."""
         self.new_epoch(reset_means=reset_means)
 
     def new_batch(self) -> None:
         """Declare a new batch."""
         # No longer just new epoch
         self._just_new_epoch = False
         # On tqdm context, the batch is automatically incremented
         if not self._on_tqdm:
             self.step += 1
             self.current_batch += 1
+        # Reset the previous table info
+        self._prev_tables_list = []
+        self._prev_table_width = 0
+        self._prev_row = []
+        self._prev_flat_cell = True
+        self._prev_message = ''
 
     def start_batch(self) -> None:
         """Declare a new batch. Alias for :meth:`new_batch`."""
         self.new_batch()
 
     def detach(self, *, skipline: bool = True) -> None:
         """Stop the live display.
@@ -341,35 +354,40 @@
             at the end of an epoch. Otherwise, the print will be shown above
             the live display.
         """
         self.detach(skipline=False)
 
     def start(self) -> None:
         """Set the start time of the training (already called at initialization)."""
-        self.t_glob = time.time()
+        self._glob_time = time.time()
 
     def reset(self) -> None:
         """Reset the logger as at initialization."""
         self.stop()
         self.step = 0
-        self.t_glob = time.time()
-        self.t_epoch = 0.0
+        self._glob_time = time.time()
+        self._epoch_time = 0.0
         self.current_epoch = 0
         self.current_batch = 0
         self._on_tqdm = False
         self.vals = {}
         self.mean_vals = {}
         self._counts = {}
         self.live = Live(
             renderable=None,
             console=RICH_CONSOLE,
             refresh_per_second=4,
             auto_refresh=False,
         )
-        self.renderable = None
+        self._renderable = None
+        self._prev_tables_list = []
+        self._prev_table_width = 0
+        self._prev_row = []
+        self._prev_flat_cell = True
+        self._prev_message = ''
 
     def get_vals(self, *, average: Optional[List[str]] = None) -> Dict[str, VarType]:
         """Get the last values called with log, optionally averaged.
 
         Parameters
         ----------
         average : List[str], optional
@@ -469,16 +487,16 @@
             bar_list[(arrow_len + i) % 54] = '='
         return Text(f"[{''.join(bar_list)}]", overflow="ellipsis")
 
     def _build_time_info(self) -> Text:
         """Build time info text."""
         (delta_glob, delta_epoch, eta_glob, eta_epoch) = get_time_range(
             current_time=time.time(),
-            start_glob=self.t_glob,
-            start_epoch=self.t_epoch,
+            start_glob=self._glob_time,
+            start_epoch=self._epoch_time,
             current_epoch=self.current_epoch,
             current_batch=self.current_batch,
             n_epochs=self.n_epochs,
             n_batches=self.n_batches,
         )
         delta_glob_str = sec_to_timestr(delta_glob)
         delta_epoch_str = sec_to_timestr(delta_epoch)
@@ -497,34 +515,51 @@
         values: Dict[str, VarType],
         *,
         styles: Union[Dict[str, str], str],
         sizes: Union[Dict[str, int], int],
         average: Union[Dict[str, bool], bool],
     ) -> Group:
         """Build a group of tables containing the keys and values."""
-        tables_list = [Table(show_header=False, show_edge=False)]
-        table_width = 0
-        row: List[Text] = []
-        flat_cell = len(values) < 3
+        # flat_cell = True => log "key: value"
+        # flat_cell = False => log "key \n value"
+        if not self._prev_tables_list:
+            # No previous logged values in same epoch
+            # => Adapt flat_cell to number of values
+            flat_cell = len(values) < 3
+        else:
+            # Previous logged values in same epoch => keep same flat_cell
+            flat_cell = self._prev_flat_cell
+
+        # The row contains all the values of the last table (if any)
+        tables_list = self._prev_tables_list[:-1]
+        row = self._prev_row
+        table_width = self._prev_table_width
+
+        # New table
+        tables_list.append(Table(show_header=False, show_edge=False))
+
         for key, val in values.items():
             # Get style, size and average bool
             style = self._get_param(
-                key, styles, self.default_styles, default_value='',
+                key, styles, self._default_styles, default_value='',
             )
-            size = self._get_param(key, sizes, self.default_sizes, default_value=6)
+            size = self._get_param(key, sizes, self._default_sizes, default_value=6)
             avg = self._get_param(
-                key, average, self.default_average, default_value=False
+                key, average, self._default_average, default_value=False
             )
             # Format value and get average if needed
             if isinstance(val, (int, float)) and not isinstance(val, bool):
                 if avg:
                     val = self.mean_vals[key]
                 val = str(val)[: int(size)].ljust(int(size))
             # cell_width: expected length of the cell to be shown
-            cell_width = 3 + max(len(str(key)), len(str(val)))
+            if flat_cell:
+                cell_width = 3 + len(str(key)) + len(str(val))
+            else:
+                cell_width = 3 + max(len(str(key)), len(str(val)))
             # Create a new table when the current table is too wide
             if table_width + cell_width > self.console.width:
                 tables_list[-1].add_row(*row)
                 tables_list.append(Table(show_header=False, show_edge=False))
                 table_width = 0
                 row = []
             cell = Text(justify="center")
@@ -535,14 +570,19 @@
                 cell.append(': ' + str(val), style=style)
             else:
                 cell.append('\n' + str(val), style=style)
             row.append(cell)
             table_width += cell_width
         # Add the last row
         tables_list[-1].add_row(*row)
+        # Store the tables, last row and its width for the next log of the same batch
+        self._prev_tables_list = tables_list
+        self._prev_table_width = table_width
+        self._prev_row = row
+        self._prev_flat_cell = flat_cell
         return Group(*tables_list)
 
     @staticmethod
     def _get_param(
         key: str,
         log_configs: Union[DictVarType, VarType, None],
         default_configs: Union[DictVarType, VarType],
@@ -562,14 +602,19 @@
         val = _regex_looking(key, default_configs)
         if val:
             return val
         return default_value
 
     def _build_message(self, message: str) -> Text:
         """Build message."""
+        if not message and self._prev_message:
+            # No current message but previous message => keep previous message
+            message = self._prev_message
+        else:
+            self._prev_message = message
         return Text(message, justify='left')
 
 
 def _regex_looking(key: str, config: DictVarType) -> Optional[VarType]:
     """Look on config (dict) for pattern matching and return the value."""
     if key in config:
         return config[key]
```

### Comparing `loggerml-1.0.0/logml/time_utils.py` & `loggerml-1.1.0/logml/time_utils.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/pyproject.toml` & `loggerml-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/scripts/pre-commit-checks.sh` & `loggerml-1.1.0/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/tests/integration/inte_logger.py` & `loggerml-1.1.0/tests/integration/inte_logger.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/tests/integration/inte_regex.py` & `loggerml-1.1.0/tests/integration/inte_regex.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/tests/integration/inte_two_loggers.py` & `loggerml-1.1.0/tests/integration/inte_two_loggers.py`

 * *Files identical despite different names*

### Comparing `loggerml-1.0.0/tests/unit/test_logger.py` & `loggerml-1.1.0/tests/unit/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
                         "loss name": 'mse',
                         "best run": True,
                     },
                     message="This is...\nok?",
                     styles=styles,
                     average=["mse"],
                 )
+                logger.log({"additional loss": 0.05})
         if i == 0:
             logger.reset()
             logger.bold_keys = False
             logger.n_batches = None
     logger.log_interval = None
     logger.log(
         {f"new loss{i}": 0.4 for i in range(1, 16)},
```

### Comparing `loggerml-1.0.0/tests/unit/test_time_utils.py` & `loggerml-1.1.0/tests/unit/test_time_utils.py`

 * *Files identical despite different names*

