# Comparing `tmp/findmyorder-1.3.1.tar.gz` & `tmp/findmyorder-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.3.1.tar", max compression
+gzip compressed data, was "findmyorder-1.3.2.tar", max compression
```

## Comparing `findmyorder-1.3.1.tar` & `findmyorder-1.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-06 04:19:05.144565 findmyorder-1.3.1/LICENSE
--rw-r--r--   0        0        0     2155 2023-05-06 04:19:05.144565 findmyorder-1.3.1/README.md
--rw-r--r--   0        0        0      113 2023-05-06 04:19:05.948622 findmyorder-1.3.1/findmyorder/__init__.py
--rw-r--r--   0        0        0      631 2023-05-06 04:19:05.144565 findmyorder-1.3.1/findmyorder/config.py
--rw-r--r--   0        0        0      566 2023-05-06 04:19:05.144565 findmyorder-1.3.1/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     4127 2023-05-06 04:19:05.144565 findmyorder-1.3.1/findmyorder/main.py
--rw-r--r--   0        0        0     1758 2023-05-06 04:19:05.944622 findmyorder-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-06 04:29:32.633521 findmyorder-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2155 2023-05-06 04:29:32.633521 findmyorder-1.3.2/README.md
+-rw-r--r--   0        0        0      113 2023-05-06 04:29:33.309527 findmyorder-1.3.2/findmyorder/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-06 04:29:32.633521 findmyorder-1.3.2/findmyorder/config.py
+-rw-r--r--   0        0        0      566 2023-05-06 04:29:32.633521 findmyorder-1.3.2/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     4127 2023-05-06 04:29:32.633521 findmyorder-1.3.2/findmyorder/main.py
+-rw-r--r--   0        0        0     1758 2023-05-06 04:29:33.309527 findmyorder-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.2/PKG-INFO
```

### Comparing `findmyorder-1.3.1/LICENSE` & `findmyorder-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.1/README.md` & `findmyorder-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.1/findmyorder/config.py` & `findmyorder-1.3.2/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.1/findmyorder/default_settings.toml` & `findmyorder-1.3.2/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.1/findmyorder/main.py` & `findmyorder-1.3.2/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.1/pyproject.toml` & `findmyorder-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.3.1"
+version = "1.3.2"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.3.1/PKG-INFO` & `findmyorder-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.3.1
+Version: 1.3.2
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

