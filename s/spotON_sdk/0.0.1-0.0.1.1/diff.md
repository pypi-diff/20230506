# Comparing `tmp/spotON_sdk-0.0.1.tar.gz` & `tmp/spotON_sdk-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.1.tar", last modified: Sat May  6 14:45:21 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.1.1.tar", last modified: Sat May  6 15:08:29 2023, max compression
```

## Comparing `spotON_sdk-0.0.1.tar` & `spotON_sdk-0.0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1/LICENSE
--rw-r--r--   0        0        0      282 2023-05-06 14:26:30.570888 spotON_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      347 2023-05-06 14:32:25.325306 spotON_sdk-0.0.1/spotON_sdk/__init__.py
--rw-r--r--   0        0        0     2786 2023-05-06 14:30:27.688605 spotON_sdk-0.0.1/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      216 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.1/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.1/LICENSE
+-rw-r--r--   0        0        0      282 2023-05-06 14:26:30.570888 spotON_sdk-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      390 2023-05-06 15:08:07.562681 spotON_sdk-0.0.1.1/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0     2786 2023-05-06 14:30:27.688605 spotON_sdk-0.0.1.1/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.1/PKG-INFO
```

### Comparing `spotON_sdk-0.0.1/.gitignore` & `spotON_sdk-0.0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1/LICENSE` & `spotON_sdk-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.1.1/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

