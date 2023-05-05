# Comparing `tmp/mcgtpy-0.0.5.tar.gz` & `tmp/mcgtpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcgtpy-0.0.5.tar", last modified: Fri May  5 18:32:06 2023, max compression
+gzip compressed data, was "mcgtpy-0.0.6.tar", last modified: Fri May  5 22:07:37 2023, max compression
```

## Comparing `mcgtpy-0.0.5.tar` & `mcgtpy-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 18:32:06.490954 mcgtpy-0.0.5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 18:32:06.490954 mcgtpy-0.0.5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 18:32:06.486955 mcgtpy-0.0.5/mcgtpy/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1262 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy/helper_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1545 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy/my_stats.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 18:32:06.490954 mcgtpy-0.0.5/mcgtpy.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-05 18:32:06.490954 mcgtpy-0.0.5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 22:07:37.413311 mcgtpy-0.0.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 22:07:37.413311 mcgtpy-0.0.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 22:07:37.409311 mcgtpy-0.0.6/mcgtpy/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/mcgtpy/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/mcgtpy/database.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1262 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/mcgtpy/helper_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1545 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/mcgtpy/my_stats.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 22:07:37.413311 mcgtpy-0.0.6/mcgtpy.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-05 22:07:37.000000 mcgtpy-0.0.6/mcgtpy.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-05 22:07:37.413311 mcgtpy-0.0.6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2023-05-05 22:07:36.000000 mcgtpy-0.0.6/setup.py
```

### Comparing `mcgtpy-0.0.5/mcgtpy/helper_functions.py` & `mcgtpy-0.0.6/mcgtpy/helper_functions.py`

 * *Files identical despite different names*

### Comparing `mcgtpy-0.0.5/mcgtpy/my_stats.py` & `mcgtpy-0.0.6/mcgtpy/my_stats.py`

 * *Files identical despite different names*

### Comparing `mcgtpy-0.0.5/setup.py` & `mcgtpy-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'My first Python Package!'
 LONG_DESCRIPTION = 'This package will have everything I use on a daily basis to make life easier when coding in Python.'
 
 author_name = "Myles Thomas"
 author_email = "mylescgthomas@gmail.com"
 
 setup(
@@ -12,15 +12,15 @@
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     author=author_name,
     author_email=author_email,
     license='MIT',
     packages=find_packages(),
-    install_requires=['timedelta', 'datetime'], # https://python-packaging.readthedocs.io/en/latest/dependencies.html
+    install_requires=['timedelta', 'datetime', 'pandas', 'requests'], # https://python-packaging.readthedocs.io/en/latest/dependencies.html
     keywords='conversion',
     classifiers= [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         'License :: OSI Approved :: MIT License',
         "Programming Language :: Python :: 3",
     ]
```

