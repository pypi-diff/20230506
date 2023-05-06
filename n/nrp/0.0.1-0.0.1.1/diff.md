# Comparing `tmp/nrp-0.0.1.tar.gz` & `tmp/nrp-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrp-0.0.1.tar", last modified: Fri Apr 21 14:54:00 2023, max compression
+gzip compressed data, was "nrp-0.0.1.1.tar", last modified: Sat May  6 13:52:38 2023, max compression
```

## Comparing `nrp-0.0.1.tar` & `nrp-0.0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-21 14:54:00.452240 nrp-0.0.1/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-20 19:31:35.000000 nrp-0.0.1/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-04-21 14:54:00.452102 nrp-0.0.1/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      556 2023-04-21 14:48:38.000000 nrp-0.0.1/README.md
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-21 14:54:00.450908 nrp-0.0.1/nrp/
--rw-r--r--   0 ubaid      (501) staff       (20)       31 2023-04-21 12:46:47.000000 nrp-0.0.1/nrp/__init__.py
--rw-r--r--   0 ubaid      (501) staff       (20)      378 2023-04-21 14:48:44.000000 nrp-0.0.1/nrp/nr.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-21 14:54:00.451893 nrp-0.0.1/nrp.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)     1019 2023-04-21 14:54:00.000000 nrp-0.0.1/nrp.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      186 2023-04-21 14:54:00.000000 nrp-0.0.1/nrp.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-21 14:54:00.000000 nrp-0.0.1/nrp.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-04-21 14:54:00.000000 nrp-0.0.1/nrp.egg-info/requires.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        4 2023-04-21 14:54:00.000000 nrp-0.0.1/nrp.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-21 14:54:00.452281 nrp-0.0.1/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1915 2023-04-21 14:48:48.000000 nrp-0.0.1/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:52:38.290311 nrp-0.0.1.1/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-20 19:31:35.000000 nrp-0.0.1.1/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)     1021 2023-05-06 13:52:38.290188 nrp-0.0.1.1/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      553 2023-05-06 13:52:09.000000 nrp-0.0.1.1/README.md
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:52:38.289414 nrp-0.0.1.1/nrp/
+-rw-r--r--   0 ubaid      (501) staff       (20)       31 2023-04-21 12:46:47.000000 nrp-0.0.1.1/nrp/__init__.py
+-rw-r--r--   0 ubaid      (501) staff       (20)      378 2023-05-06 13:52:09.000000 nrp-0.0.1.1/nrp/nr.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:52:38.290025 nrp-0.0.1.1/nrp.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1021 2023-05-06 13:52:38.000000 nrp-0.0.1.1/nrp.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      186 2023-05-06 13:52:38.000000 nrp-0.0.1.1/nrp.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-05-06 13:52:38.000000 nrp-0.0.1.1/nrp.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       18 2023-05-06 13:52:38.000000 nrp-0.0.1.1/nrp.egg-info/requires.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        4 2023-05-06 13:52:38.000000 nrp-0.0.1.1/nrp.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-05-06 13:52:38.290348 nrp-0.0.1.1/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1928 2023-05-06 13:52:12.000000 nrp-0.0.1.1/setup.py
```

### Comparing `nrp-0.0.1/LICENSE` & `nrp-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrp-0.0.1/PKG-INFO` & `nrp-0.0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nrp
-Version: 0.0.1
-Summary: A package for root computation of functions
+Version: 0.0.1.1
+Summary: Package for root computation of math functions
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Smit Lunagariya
 Author-email: smitlunagariya.mat18@itbhu.ac.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -16,19 +16,19 @@
 
 This is a small package for computing roots of a given function using newton-raphson method.
 
 The user needs to supply an initial root guess, the function as well as the first derivative of the function as callbacks.
 
 ## Usage
 
-(We are actively adding supporting for passing functions as callback.)
+(We are actively adding support for passing functions as callback.)
 **Example:**
 ```python
 from nrp import newton_raphson
-from lptypes import f64, i32
+from lpython import f64, i32
 
 
 def check():
     x0: f64 = 20.0
     c: f64 = 3.0
     maxiter: i32 = 20
     x: f64
```

### Comparing `nrp-0.0.1/README.md` & `nrp-0.0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 This is a small package for computing roots of a given function using newton-raphson method.
 
 The user needs to supply an initial root guess, the function as well as the first derivative of the function as callbacks.
 
 ## Usage
 
-(We are actively adding supporting for passing functions as callback.)
+(We are actively adding support for passing functions as callback.)
 **Example:**
 ```python
 from nrp import newton_raphson
-from lptypes import f64, i32
+from lpython import f64, i32
 
 
 def check():
     x0: f64 = 20.0
     c: f64 = 3.0
     maxiter: i32 = 20
     x: f64
```

### Comparing `nrp-0.0.1/nrp.egg-info/PKG-INFO` & `nrp-0.0.1.1/nrp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nrp
-Version: 0.0.1
-Summary: A package for root computation of functions
+Version: 0.0.1.1
+Summary: Package for root computation of math functions
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Smit Lunagariya
 Author-email: smitlunagariya.mat18@itbhu.ac.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -16,19 +16,19 @@
 
 This is a small package for computing roots of a given function using newton-raphson method.
 
 The user needs to supply an initial root guess, the function as well as the first derivative of the function as callbacks.
 
 ## Usage
 
-(We are actively adding supporting for passing functions as callback.)
+(We are actively adding support for passing functions as callback.)
 **Example:**
 ```python
 from nrp import newton_raphson
-from lptypes import f64, i32
+from lpython import f64, i32
 
 
 def check():
     x0: f64 = 20.0
     c: f64 = 3.0
     maxiter: i32 = 20
     x: f64
```

### Comparing `nrp-0.0.1/setup.py` & `nrp-0.0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # The setup.py file is used as the build script for setuptools. Setuptools is a
 # package that allows you to easily build and distribute Python distributions.
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
-REQUIRED_PACKAGES=["lptypes"]
+REQUIRED_PACKAGES=["lpython_emulation"]
 
-VERSION="0.0.1"
+VERSION="0.0.1.1"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nrp",                                                 # name of project
     install_requires=REQUIRED_PACKAGES,                         # all requirements used by this package
     version=VERSION,                                            # project version, read from version.py
     author="Smit Lunagariya",                                   # Author, shown on PyPI
     author_email="smitlunagariya.mat18@itbhu.ac.in",            # Author email
-    description="A package for root computation of functions",  # Short description of project
+    description="Package for root computation of math functions",# Short description of project
     long_description=long_description,                          # Long description, shown on PyPI
     long_description_content_type="text/markdown",              # Content type. Here, we used a markdown file.
     url="https://github.com/Shaikh-Ubaid/lpython_packages",     # github path
     packages=setuptools.find_packages(),                        # automatically finds packages in the current directory. You can also explictly list them.
     classifiers=[                                               # Classifiers give pip metadata about your project. See https://pypi.org/classifiers/ for a list of available classifiers.
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

