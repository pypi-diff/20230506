# Comparing `tmp/python_travelmanager-0.2.0.tar.gz` & `tmp/python_travelmanager-0.2.1.tar.gz`

## Comparing `python_travelmanager-0.2.0.tar` & `python_travelmanager-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/travelmanager/__init__.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/LICENSE
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_travelmanager-0.2.1/travelmanager/__init__.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 python_travelmanager-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 python_travelmanager-0.2.1/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 python_travelmanager-0.2.1/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 python_travelmanager-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 python_travelmanager-0.2.1/PKG-INFO
```

### Comparing `python_travelmanager-0.2.0/.gitignore` & `python_travelmanager-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python_travelmanager-0.2.0/LICENSE` & `python_travelmanager-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_travelmanager-0.2.0/pyproject.toml` & `python_travelmanager-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_travelmanager"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="Johannes Eimer", email="johannes.eimer@jep-dev.com" },
 ]
 description = "Python TravelManager"
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
```

