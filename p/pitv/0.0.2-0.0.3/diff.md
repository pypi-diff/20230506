# Comparing `tmp/pitv-0.0.2.tar.gz` & `tmp/pitv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitv-0.0.2.tar", max compression
+gzip compressed data, was "pitv-0.0.3.tar", max compression
```

## Comparing `pitv-0.0.2.tar` & `pitv-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1081 2023-05-06 19:25:58.253937 pitv-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      981 2023-05-06 20:09:48.257944 pitv-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1038 2023-05-06 19:25:58.253937 pitv-0.0.2/src/pitv/__init__.py
--rw-r--r--   0        0        0      553 2023-05-06 19:25:58.253937 pitv-0.0.2/src/pitv/pitv.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 pitv-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-06 19:25:58.253937 pitv-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      882 2023-05-06 20:32:21.318107 pitv-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1038 2023-05-06 19:25:58.253937 pitv-0.0.3/src/pitv/__init__.py
+-rw-r--r--   0        0        0      553 2023-05-06 19:25:58.253937 pitv-0.0.3/src/pitv/pitv.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pitv-0.0.3/PKG-INFO
```

### Comparing `pitv-0.0.2/LICENSE.txt` & `pitv-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pitv-0.0.2/src/pitv/__init__.py` & `pitv-0.0.3/src/pitv/__init__.py`

 * *Files identical despite different names*

### Comparing `pitv-0.0.2/src/pitv/pitv.py` & `pitv-0.0.3/src/pitv/pitv.py`

 * *Files identical despite different names*

