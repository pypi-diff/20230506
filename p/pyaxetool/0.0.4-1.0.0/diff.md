# Comparing `tmp/pyaxetool-0.0.4.tar.gz` & `tmp/pyaxetool-1.0.0.tar.gz`

## Comparing `pyaxetool-0.0.4.tar` & `pyaxetool-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/.gitignore
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/LICENSE
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/README.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/TODO.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/PyAxeTool/MD5.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/PyAxeTool/PyInstaller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/PyAxeTool/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/PyAxeTool/__main__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/oldbak/MANIFEST.in
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/oldbak/setup.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyaxetool-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/.gitignore
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/LICENSE
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/README.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/TODO.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PyAxeTool/MD5.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PyAxeTool/PyInstaller.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PyAxeTool/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PyAxeTool/__main__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/oldbak/MANIFEST.in
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/oldbak/setup.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 pyaxetool-1.0.0/PKG-INFO
```

### Comparing `pyaxetool-0.0.4/.gitignore` & `pyaxetool-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyaxetool-0.0.4/LICENSE` & `pyaxetool-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaxetool-0.0.4/pyproject.toml` & `pyaxetool-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyAxeTool"
-version = "0.0.4"
+version = "1.0.0"
 authors = [
   { name="Sun Jin", email="412640665@qq.com" },
 ]
 description = "An utility tool collection for make life easily"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyaxetool-0.0.4/PyAxeTool/PyInstaller.py` & `pyaxetool-1.0.0/PyAxeTool/PyInstaller.py`

 * *Files identical despite different names*

### Comparing `pyaxetool-0.0.4/PyAxeTool/__main__.py` & `pyaxetool-1.0.0/PyAxeTool/__main__.py`

 * *Files identical despite different names*

### Comparing `pyaxetool-0.0.4/oldbak/setup.py` & `pyaxetool-1.0.0/oldbak/setup.py`

 * *Files identical despite different names*

