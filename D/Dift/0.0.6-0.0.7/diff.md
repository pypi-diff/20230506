# Comparing `tmp/dift-0.0.6.tar.gz` & `tmp/dift-0.0.7.tar.gz`

## Comparing `dift-0.0.6.tar` & `dift-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 dift-0.0.6/PKG-INFO
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dift-0.0.6/src/Dift/Dift.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dift-0.0.6/src/Dift/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dift-0.0.6/LICENSE
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 dift-0.0.6/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dift-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dift-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 dift-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 dift-0.0.7/src/Dift/Dift.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dift-0.0.7/src/Dift/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dift-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 dift-0.0.7/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dift-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dift-0.0.7/PKG-INFO
```

### Comparing `dift-0.0.6/PKG-INFO` & `dift-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dift
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library to read data from  a file and convert it into python dictionary
 Project-URL: Homepage, https://github.com/NisheshTyagi/Dift
 Project-URL: Bug Tracker, https://github.com/NisheshTyagi/Dift/issues
 Author-email: Nishesh Tyagi <eyetrack9182@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dift-0.0.6/LICENSE` & `dift-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dift-0.0.6/README.md` & `dift-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dift-0.0.6/pyproject.toml` & `dift-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Dift"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Nishesh Tyagi", email="eyetrack9182@gmail.com" },
 ]
 description = "A library to read data from  a file and convert it into python dictionary"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

