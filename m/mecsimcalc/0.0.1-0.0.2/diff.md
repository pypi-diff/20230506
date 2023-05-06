# Comparing `tmp/MecSimCalc-0.0.1.tar.gz` & `tmp/mecsimcalc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MecSimCalc-0.0.1.tar", last modified: Sat May  6 03:34:34 2023, max compression
+gzip compressed data, was "mecsimcalc-0.0.2.tar", last modified: Sat May  6 03:56:47 2023, max compression
```

## Comparing `MecSimCalc-0.0.1.tar` & `mecsimcalc-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:34:34.674298 MecSimCalc-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-05-01 03:16:58.000000 MecSimCalc-0.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-06 03:34:34.668296 MecSimCalc-0.0.1/MecSimCalc.egg-info/
--rw-rw-rw-   0        0        0      908 2023-05-06 03:34:34.000000 MecSimCalc-0.0.1/MecSimCalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-06 03:34:34.000000 MecSimCalc-0.0.1/MecSimCalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:34:34.000000 MecSimCalc-0.0.1/MecSimCalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-06 03:34:34.000000 MecSimCalc-0.0.1/MecSimCalc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 03:34:34.000000 MecSimCalc-0.0.1/MecSimCalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      908 2023-05-06 03:34:34.673298 MecSimCalc-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-05-01 03:16:58.000000 MecSimCalc-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 03:34:34.672296 MecSimCalc-0.0.1/mecsimcalc/
--rw-rw-rw-   0        0        0     4814 2023-05-05 20:26:51.000000 MecSimCalc-0.0.1/mecsimcalc/MecSimCalc.py
--rw-rw-rw-   0        0        0        0 2023-05-01 03:16:58.000000 MecSimCalc-0.0.1/mecsimcalc/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-06 03:34:34.674298 MecSimCalc-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-05-06 03:33:49.000000 MecSimCalc-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:56:47.148438 mecsimcalc-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-05-01 03:16:58.000000 mecsimcalc-0.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-06 03:56:47.140931 mecsimcalc-0.0.2/MecSimCalc.egg-info/
+-rw-rw-rw-   0        0        0      908 2023-05-06 03:56:46.000000 mecsimcalc-0.0.2/MecSimCalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-06 03:56:47.000000 mecsimcalc-0.0.2/MecSimCalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 03:56:46.000000 mecsimcalc-0.0.2/MecSimCalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-06 03:56:46.000000 mecsimcalc-0.0.2/MecSimCalc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 03:56:46.000000 mecsimcalc-0.0.2/MecSimCalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      908 2023-05-06 03:56:47.147437 mecsimcalc-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-05-01 03:16:58.000000 mecsimcalc-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 03:56:47.144437 mecsimcalc-0.0.2/mecsimcalc/
+-rw-rw-rw-   0        0        0     4814 2023-05-06 03:45:21.000000 mecsimcalc-0.0.2/mecsimcalc/MecSimCalc.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 03:45:22.000000 mecsimcalc-0.0.2/mecsimcalc/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 03:56:47.148438 mecsimcalc-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-05-06 03:55:46.000000 mecsimcalc-0.0.2/setup.py
```

### Comparing `MecSimCalc-0.0.1/LICENSE` & `mecsimcalc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MecSimCalc-0.0.1/MecSimCalc.egg-info/PKG-INFO` & `mecsimcalc-0.0.2/MecSimCalc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: MecSimCalc
-Version: 0.0.1
+Name: mecsimcalc
+Version: 0.0.2
 Summary: Useful functions for MecSimCalc.com
 Author: MecSimCalc
 Author-email: <info@mecsimcalc.com>
 Keywords: python,MecSimCalc,Calculator,Simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `MecSimCalc-0.0.1/PKG-INFO` & `mecsimcalc-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: MecSimCalc
-Version: 0.0.1
+Name: mecsimcalc
+Version: 0.0.2
 Summary: Useful functions for MecSimCalc.com
 Author: MecSimCalc
 Author-email: <info@mecsimcalc.com>
 Keywords: python,MecSimCalc,Calculator,Simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `MecSimCalc-0.0.1/mecsimcalc/MecSimCalc.py` & `mecsimcalc-0.0.2/mecsimcalc/MecSimCalc.py`

 * *Files identical despite different names*

### Comparing `MecSimCalc-0.0.1/setup.py` & `mecsimcalc-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "Useful functions for MecSimCalc.com"
 LONG_DESCRIPTION = "Useful functions for MecSimCalc.com"
 
 # Setting up
 setup(
-    name="MecSimCalc",
+    name="mecsimcalc",
     version=VERSION,
     author="MecSimCalc",
     author_email="<info@mecsimcalc.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

