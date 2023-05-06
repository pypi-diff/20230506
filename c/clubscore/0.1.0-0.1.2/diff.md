# Comparing `tmp/clubscore-0.1.0.tar.gz` & `tmp/clubscore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clubscore-0.1.0.tar", last modified: Sat May  6 09:09:05 2023, max compression
+gzip compressed data, was "dist/clubscore-0.1.2.tar", last modified: Sat May  6 09:47:48 2023, max compression
```

## Comparing `clubscore-0.1.0.tar` & `clubscore-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:09:05.000000 clubscore-0.1.0/
--rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.0/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)      895 2023-05-06 09:09:05.000000 clubscore-0.1.0/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)        9 2023-05-06 08:49:34.000000 clubscore-0.1.0/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:09:05.000000 clubscore-0.1.0/clubscore/
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.0/clubscore/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     3209 2023-04-06 23:23:45.000000 clubscore-0.1.0/clubscore/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:09:05.000000 clubscore-0.1.0/clubscore.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      895 2023-05-06 09:09:05.000000 clubscore-0.1.0/clubscore.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      231 2023-05-06 09:09:05.000000 clubscore-0.1.0/clubscore.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-06 09:09:05.000000 clubscore-0.1.0/clubscore.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-06 09:09:05.000000 clubscore-0.1.0/clubscore.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-06 09:09:05.000000 clubscore-0.1.0/clubscore.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-06 09:09:05.000000 clubscore-0.1.0/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-06 09:06:21.000000 clubscore-0.1.0/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:47:48.000000 clubscore-0.1.2/
+-rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.2/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-06 09:47:48.000000 clubscore-0.1.2/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.2/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore/
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.2/clubscore/__init__.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore/objects/
+-rw-r--r--   0 dave       (501) staff       (20)     4792 2023-05-06 08:35:20.000000 clubscore-0.1.2/clubscore/objects/CONTAINER.py
+-rw-r--r--   0 dave       (501) staff       (20)     2204 2023-05-06 08:35:20.000000 clubscore-0.1.2/clubscore/objects/IMG.py
+-rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.2/clubscore/objects/RECTANGLE.py
+-rw-r--r--   0 dave       (501) staff       (20)     3899 2023-05-06 08:35:20.000000 clubscore-0.1.2/clubscore/objects/TEXT.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.2/clubscore/objects/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     3209 2023-04-06 23:23:45.000000 clubscore-0.1.2/clubscore/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      374 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-06 09:47:48.000000 clubscore-0.1.2/clubscore.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-06 09:47:48.000000 clubscore-0.1.2/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-06 09:41:10.000000 clubscore-0.1.2/setup.py
```

### Comparing `clubscore-0.1.0/LICENSE` & `clubscore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.0/PKG-INFO` & `clubscore-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.0
+Version: 0.1.2
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
@@ -18,7 +18,9 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Clubscore
+
+Basic readme
```

### Comparing `clubscore-0.1.0/clubscore/utils.py` & `clubscore-0.1.2/clubscore/utils.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.0/clubscore.egg-info/PKG-INFO` & `clubscore-0.1.2/clubscore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.0
+Version: 0.1.2
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
@@ -18,7 +18,9 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Clubscore
+
+Basic readme
```

### Comparing `clubscore-0.1.0/setup.py` & `clubscore-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clubscore',
-    version='0.1.0',
+    version='0.1.2',
     author='Davide Gimondo',
     author_email='davegimo@gmail.com',
     description='A package for creating customizable templates in XML',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clubscore',
     packages=find_packages(),
```

