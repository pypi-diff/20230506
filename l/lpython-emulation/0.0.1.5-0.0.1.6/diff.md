# Comparing `tmp/lpython_emulation-0.0.1.5.tar.gz` & `tmp/lpython_emulation-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpython_emulation-0.0.1.5.tar", last modified: Sun Apr 30 17:49:39 2023, max compression
+gzip compressed data, was "lpython_emulation-0.0.1.6.tar", last modified: Sat May  6 13:25:42 2023, max compression
```

## Comparing `lpython_emulation-0.0.1.5.tar` & `lpython_emulation-0.0.1.6.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:49:39.973613 lpython_emulation-0.0.1.5/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.5/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)     1020 2023-04-30 17:49:39.973446 lpython_emulation-0.0.1.5/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      557 2023-04-30 17:47:36.000000 lpython_emulation-0.0.1.5/README.md
--rw-r--r--   0 ubaid      (501) staff       (20)     7587 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.5/goto.py
--rw-r--r--   0 ubaid      (501) staff       (20)    15499 2023-04-30 17:14:24.000000 lpython_emulation-0.0.1.5/lpython.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-30 17:49:39.973177 lpython_emulation-0.0.1.5/lpython_emulation.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)     1020 2023-04-30 17:49:39.000000 lpython_emulation-0.0.1.5/lpython_emulation.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      209 2023-04-30 17:49:39.000000 lpython_emulation-0.0.1.5/lpython_emulation.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-30 17:49:39.000000 lpython_emulation-0.0.1.5/lpython_emulation.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       13 2023-04-30 17:49:39.000000 lpython_emulation-0.0.1.5/lpython_emulation.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-30 17:49:39.973656 lpython_emulation-0.0.1.5/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1789 2023-04-30 17:49:17.000000 lpython_emulation-0.0.1.5/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:25:42.345970 lpython_emulation-0.0.1.6/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.6/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-05-06 13:25:42.345794 lpython_emulation-0.0.1.6/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      556 2023-04-30 17:58:09.000000 lpython_emulation-0.0.1.6/README.md
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:25:42.344902 lpython_emulation-0.0.1.6/lpython/
+-rw-r--r--   0 ubaid      (501) staff       (20)        0 2023-05-06 13:19:25.000000 lpython_emulation-0.0.1.6/lpython/__init__.py
+-rw-r--r--   0 ubaid      (501) staff       (20)     7587 2023-04-21 16:22:30.000000 lpython_emulation-0.0.1.6/lpython/goto.py
+-rw-r--r--   0 ubaid      (501) staff       (20)    15499 2023-04-30 17:14:24.000000 lpython_emulation-0.0.1.6/lpython/lpython.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:25:42.345425 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-05-06 13:25:42.000000 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      245 2023-05-06 13:25:42.000000 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-05-06 13:25:42.000000 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-05-06 13:25:42.000000 lpython_emulation-0.0.1.6/lpython_emulation.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-05-06 13:25:42.346016 lpython_emulation-0.0.1.6/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1779 2023-05-06 13:24:48.000000 lpython_emulation-0.0.1.6/setup.py
```

### Comparing `lpython_emulation-0.0.1.5/LICENSE` & `lpython_emulation-0.0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.5/PKG-INFO` & `lpython_emulation-0.0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython_emulation
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,11 +34,11 @@
     print("Area of circle with radius 5.0 is", end=" ")
     print(area_of_circle(5.0))
 
 main0()
 ```
 
 ```bash
-$ python main2.py
+$ python main.py
 The sum of 5 and 3 is 8
 Area of circle with radius 5.0 is 78.5
 ```
```

### Comparing `lpython_emulation-0.0.1.5/README.md` & `lpython_emulation-0.0.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     print("Area of circle with radius 5.0 is", end=" ")
     print(area_of_circle(5.0))
 
 main0()
 ```
 
 ```bash
-$ python main2.py
+$ python main.py
 The sum of 5 and 3 is 8
 Area of circle with radius 5.0 is 78.5
 ```
```

### Comparing `lpython_emulation-0.0.1.5/goto.py` & `lpython_emulation-0.0.1.6/lpython/goto.py`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.5/lpython.py` & `lpython_emulation-0.0.1.6/lpython/lpython.py`

 * *Files identical despite different names*

### Comparing `lpython_emulation-0.0.1.5/lpython_emulation.egg-info/PKG-INFO` & `lpython_emulation-0.0.1.6/lpython_emulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpython-emulation
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: Package for adding type information to python
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ondrej Certik
 Author-email: ondrej@certik.us
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,11 +34,11 @@
     print("Area of circle with radius 5.0 is", end=" ")
     print(area_of_circle(5.0))
 
 main0()
 ```
 
 ```bash
-$ python main2.py
+$ python main.py
 The sum of 5 and 3 is 8
 Area of circle with radius 5.0 is 78.5
 ```
```

### Comparing `lpython_emulation-0.0.1.5/setup.py` & `lpython_emulation-0.0.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
 REQUIRED_PACKAGES=[]
 
-VERSION="0.0.1.5"
+VERSION="0.0.1.6"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpython_emulation",                                   # name of project
-    py_modules=["lpython", "goto"],
+    packages=["lpython"],
     install_requires=REQUIRED_PACKAGES,                         # all requirements used by this package
     version=VERSION,                                            # project version, read from version.py
     author="Ondrej Certik",                                     # Author, shown on PyPI
     author_email="ondrej@certik.us",                            # Author email
     description="Package for adding type information to python",# Short description of project
     long_description=long_description,                          # Long description, shown on PyPI
     long_description_content_type="text/markdown",              # Content type. Here, we used a markdown file.
```

