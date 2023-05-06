# Comparing `tmp/pyfanity-0.1.1.tar.gz` & `tmp/pyfanity-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfanity-0.1.1.tar", max compression
+gzip compressed data, was "pyfanity-0.1.2.tar", max compression
```

## Comparing `pyfanity-0.1.1.tar` & `pyfanity-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2023-05-05 06:59:53.587619 pyfanity-0.1.1/LICENSE
--rw-r--r--   0        0        0      413 2023-05-05 22:20:24.545754 pyfanity-0.1.1/pyfanity/__init__.py
--rw-r--r--   0        0        0       63 2023-05-05 22:11:06.255231 pyfanity-0.1.1/pyfanity/example.py
--rw-r--r--   0        0        0      954 2023-05-05 22:28:52.402653 pyfanity-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      174 2023-05-05 06:26:08.923618 pyfanity-0.1.1/README.md
--rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 pyfanity-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-05 06:59:53.587619 pyfanity-0.1.2/LICENSE
+-rw-r--r--   0        0        0      447 2023-05-06 00:59:15.034621 pyfanity-0.1.2/pyfanity/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-05 22:11:06.255231 pyfanity-0.1.2/pyfanity/example.py
+-rw-r--r--   0        0        0      954 2023-05-06 01:08:24.402629 pyfanity-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-05-05 06:26:08.923618 pyfanity-0.1.2/README.md
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 pyfanity-0.1.2/PKG-INFO
```

### Comparing `pyfanity-0.1.1/LICENSE` & `pyfanity-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfanity-0.1.1/pyproject.toml` & `pyfanity-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfanity"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple and light weight profanity filter package."
 authors = ["bourrasque <stampixel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyfanity"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pyfanity-0.1.1/PKG-INFO` & `pyfanity-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfanity
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple and light weight profanity filter package.
 License: MIT
 Keywords: feed,reader,tutorial
 Author: bourrasque
 Author-email: stampixel@pm.me
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

