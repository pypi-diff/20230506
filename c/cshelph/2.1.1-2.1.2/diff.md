# Comparing `tmp/cshelph-2.1.1.tar.gz` & `tmp/cshelph-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshelph-2.1.1.tar", last modified: Sat May  6 02:22:40 2023, max compression
+gzip compressed data, was "cshelph-2.1.2.tar", last modified: Sat May  6 02:39:50 2023, max compression
```

## Comparing `cshelph-2.1.1.tar` & `cshelph-2.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 02:22:40.625347 cshelph-2.1.1/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.1.1/LICENSE.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 02:22:40.625231 cshelph-2.1.1/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1165 2023-05-02 19:47:21.000000 cshelph-2.1.1/README.md
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 02:22:40.624337 cshelph-2.1.1/bin/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    19075 2023-05-04 16:18:29.000000 cshelph-2.1.1/bin/bathy_utils.py
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 02:22:40.625080 cshelph-2.1.1/cshelph.egg-info/
--rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 02:22:40.000000 cshelph-2.1.1/cshelph.egg-info/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)      173 2023-05-06 02:22:40.000000 cshelph-2.1.1/cshelph.egg-info/SOURCES.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 02:22:40.000000 cshelph-2.1.1/cshelph.egg-info/dependency_links.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 02:22:40.000000 cshelph-2.1.1/cshelph.egg-info/top_level.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-06 02:22:40.625383 cshelph-2.1.1/setup.cfg
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1579 2023-05-06 02:21:07.000000 cshelph-2.1.1/setup.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 02:39:50.514748 cshelph-2.1.2/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.1.2/LICENSE.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 02:39:50.514597 cshelph-2.1.2/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1165 2023-05-02 19:47:21.000000 cshelph-2.1.2/README.md
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    19075 2023-05-04 16:18:29.000000 cshelph-2.1.2/bathy_utils.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 02:39:50.514424 cshelph-2.1.2/cshelph.egg-info/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 02:39:50.000000 cshelph-2.1.2/cshelph.egg-info/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      169 2023-05-06 02:39:50.000000 cshelph-2.1.2/cshelph.egg-info/SOURCES.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 02:39:50.000000 cshelph-2.1.2/cshelph.egg-info/dependency_links.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       12 2023-05-06 02:39:50.000000 cshelph-2.1.2/cshelph.egg-info/top_level.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-06 02:39:50.514787 cshelph-2.1.2/setup.cfg
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1575 2023-05-06 02:39:43.000000 cshelph-2.1.2/setup.py
```

### Comparing `cshelph-2.1.1/LICENSE.txt` & `cshelph-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cshelph-2.1.1/README.md` & `cshelph-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cshelph-2.1.1/bin/bathy_utils.py` & `cshelph-2.1.2/bathy_utils.py`

 * *Files identical despite different names*

### Comparing `cshelph-2.1.1/setup.py` & `cshelph-2.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 #
 #
 # Purpose:  Installation of the C-SHELPh software
 #
 # Author: Nathan Thomas
 # Email: nmthomas28@gmail.com
 # Date: 05/05/2023
-# Version: 2.1.1
+# Version: 2.1.2
 #
 # History:
 # Version 2.1.1
 
 from distutils.core import setup
 import os
 
 setup(name='cshelph',
-    version='2.1.1',
+    version='2.1.2',
     description='Classification of Sub-aquatic Height Extracted Photons',
     author='Nathan Thomas and Brian Lee',
     author_email='nmthomas28@gmail.com',
-    scripts=['bin/bathy_utils.py'],
+    scripts=['bathy_utils.py'],
     package_dir={},
     data_files=[],
     license='LICENSE.txt',
     url='https://github.com/nmt28/C-SHELPh',
     classifiers=['Intended Audience :: Developers',
                  'Intended Audience :: Science/Research',
                  'Operating System :: OS Independent',
```

