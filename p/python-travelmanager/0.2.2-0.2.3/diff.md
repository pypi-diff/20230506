# Comparing `tmp/python_travelmanager-0.2.2.tar.gz` & `tmp/python_travelmanager-0.2.3.tar.gz`

## Comparing `python_travelmanager-0.2.2.tar` & `python_travelmanager-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_travelmanager-0.2.2/travelmanager/__init__.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 python_travelmanager-0.2.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 python_travelmanager-0.2.2/LICENSE
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 python_travelmanager-0.2.2/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 python_travelmanager-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 python_travelmanager-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_travelmanager-0.2.3/travelmanager/__init__.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 python_travelmanager-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 python_travelmanager-0.2.3/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 python_travelmanager-0.2.3/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 python_travelmanager-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 python_travelmanager-0.2.3/PKG-INFO
```

### Comparing `python_travelmanager-0.2.2/.gitignore` & `python_travelmanager-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `python_travelmanager-0.2.2/LICENSE` & `python_travelmanager-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_travelmanager-0.2.2/pyproject.toml` & `python_travelmanager-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_travelmanager"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     { name="Johannes Eimer", email="johannes.eimer@jep-dev.com" },
 ]
 description = "Python TravelManager"
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
```

### Comparing `python_travelmanager-0.2.2/PKG-INFO` & `python_travelmanager-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_travelmanager
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python TravelManager
 Author-email: Johannes Eimer <johannes.eimer@jep-dev.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Python,TravelManager
 Requires-Python: >=3.10
 Requires-Dist: requests==2.30.0
```

