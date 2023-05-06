# Comparing `tmp/adept-augmentations-0.1.0.tar.gz` & `tmp/adept-augmentations-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adept-augmentations-0.1.0.tar", max compression
+gzip compressed data, was "adept-augmentations-0.1.1.tar", max compression
```

## Comparing `adept-augmentations-0.1.0.tar` & `adept-augmentations-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0    11357 2022-11-25 08:22:18.508448 adept-augmentations-0.1.0/LICENSE
--rw-r--r--   0        0        0       93 2022-11-25 08:22:18.508518 adept-augmentations-0.1.0/README.md
--rw-r--r--   0        0        0      122 2022-12-01 09:55:23.008556 adept-augmentations-0.1.0/adept_augmentations/__init__.py
--rw-r--r--   0        0        0        0 2022-12-01 09:55:28.661259 adept-augmentations-0.1.0/adept_augmentations/analyzers/__init__.py
--rw-r--r--   0        0        0       33 2022-12-01 09:38:33.149386 adept-augmentations-0.1.0/adept_augmentations/analyzers/analyzer.py
--rw-r--r--   0        0        0        0 2022-12-01 09:55:25.837738 adept-augmentations-0.1.0/adept_augmentations/augmentors/__init__.py
--rw-r--r--   0        0        0       34 2022-12-01 09:43:22.847638 adept-augmentations-0.1.0/adept_augmentations/augmentors/augmentor.py
--rw-r--r--   0        0        0     1570 2022-12-05 10:33:45.218681 adept-augmentations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 adept-augmentations-0.1.0/setup.py
--rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 adept-augmentations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-25 08:22:18.508448 adept-augmentations-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4138 2023-05-06 14:03:41.077960 adept-augmentations-0.1.1/README.md
+-rw-r--r--   0        0        0      170 2023-05-06 14:03:41.078288 adept-augmentations-0.1.1/adept_augmentations/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-01 09:55:28.661259 adept-augmentations-0.1.1/adept_augmentations/analyzers/__init__.py
+-rw-r--r--   0        0        0       33 2022-12-01 09:38:33.149386 adept-augmentations-0.1.1/adept_augmentations/analyzers/analyzer.py
+-rw-r--r--   0        0        0       78 2023-05-06 14:03:41.078669 adept-augmentations-0.1.1/adept_augmentations/augmenters/__init__.py
+-rw-r--r--   0        0        0     6020 2023-05-06 14:03:41.078957 adept-augmentations-0.1.1/adept_augmentations/augmenters/augmenter.py
+-rw-r--r--   0        0        0      126 2023-05-06 14:03:41.079231 adept-augmentations-0.1.1/adept_augmentations/augmenters/constants.py
+-rw-r--r--   0        0        0     5516 2023-05-06 14:03:41.079470 adept-augmentations-0.1.1/adept_augmentations/augmenters/extractors.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:45:11.978216 adept-augmentations-0.1.1/adept_augmentations/profilers/__init__.py
+-rw-r--r--   0        0        0     3632 2023-05-06 14:03:41.079656 adept-augmentations-0.1.1/adept_augmentations/utils.py
+-rw-r--r--   0        0        0     2082 2023-05-06 14:03:51.634905 adept-augmentations-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 adept-augmentations-0.1.1/setup.py
+-rw-r--r--   0        0        0     5651 1970-01-01 00:00:00.000000 adept-augmentations-0.1.1/PKG-INFO
```

### Comparing `adept-augmentations-0.1.0/LICENSE` & `adept-augmentations-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adept-augmentations-0.1.0/pyproject.toml` & `adept-augmentations-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "adept-augmentations"
-version = "0.1.0"
-description = "A Python library aimed at dissecting and augmenting NLP training data."
+version = "0.1.1"
+description = "A Python library aimed at adeptly, augmenting NLP training data."
 authors = ["david <david.m.berenstein@gmail.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/davidberenstein1957/adept-augmentations"
 repository = "https://github.com/davidberenstein1957/adept-augmentations"
 documentation = "https://github.com/davidberenstein1957/adept-augmentations"
 keywords = ["spacy", "explainable AI", "xai", "nlu", "visualization", "datasets", "nlproc", "data-centricity", "augmentation", "data-augmentation"]
@@ -28,24 +28,49 @@
 spacy = "^3"
 datasets = "^2.5"
 pydantic = "^1.8"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
+pytest-cov = "^4.0.0"
 jupyter = "^1.0.0"
 pre-commit = "^2.20.0"
+jupyterlab = "^3.6.1"
+black = "^23.3.0"
+ruff = "0.0.262"
+
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-testpaths = "tests"
+testpaths = [
+    "tests"
+]
+filterwarnings = [
+    "ignore::DeprecationWarning:tensorboard.*:"
+]
+addopts = "--cov=adept_augmentations --durations=10"
+
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    "def __repr__",
+    "def __str__",
+    "raise AssertionError",
+    "raise NotImplementedError",
+    "if __name__ == .__main__.:",
+    "if TYPE_CHECKING:",
+    "if _TYPE_CHECKING:",
+    "if typing.TYPE_CHECKING:",
+    "@abstractmethod"
+]
 
 [tool.black]
 line-length = 119
 experimental-string-processing = true
 
 [tool.isort]
 profile = "black"
-src_paths = ["adept_augmentations"]
+src_paths = ["adept_augmentations"]
```

