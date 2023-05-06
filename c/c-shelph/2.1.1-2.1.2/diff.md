# Comparing `tmp/c-shelph-2.1.1.tar.gz` & `tmp/c-shelph-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c-shelph-2.1.1.tar", last modified: Sat May  6 02:50:24 2023, max compression
+gzip compressed data, was "c-shelph-2.1.2.tar", last modified: Sat May  6 03:02:48 2023, max compression
```

## Comparing `c-shelph-2.1.1.tar` & `c-shelph-2.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 02:50:24.429448 c-shelph-2.1.1/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 c-shelph-2.1.1/LICENSE.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)      468 2023-05-06 02:50:24.429318 c-shelph-2.1.1/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1165 2023-05-02 19:47:21.000000 c-shelph-2.1.1/README.md
--rw-r--r--   0 nmthoma1   (503) staff       (20)    19075 2023-05-04 16:18:29.000000 c-shelph-2.1.1/bathy_utils.py
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 02:50:24.429149 c-shelph-2.1.1/c_shelph.egg-info/
--rw-r--r--   0 nmthoma1   (503) staff       (20)      468 2023-05-06 02:50:24.000000 c-shelph-2.1.1/c_shelph.egg-info/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)      173 2023-05-06 02:50:24.000000 c-shelph-2.1.1/c_shelph.egg-info/SOURCES.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 02:50:24.000000 c-shelph-2.1.1/c_shelph.egg-info/dependency_links.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)       12 2023-05-06 02:50:24.000000 c-shelph-2.1.1/c_shelph.egg-info/top_level.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-06 02:50:24.429490 c-shelph-2.1.1/setup.cfg
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1576 2023-05-06 02:49:34.000000 c-shelph-2.1.1/setup.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 03:02:48.779794 c-shelph-2.1.2/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 c-shelph-2.1.2/LICENSE.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      468 2023-05-06 03:02:48.779665 c-shelph-2.1.2/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1165 2023-05-02 19:47:21.000000 c-shelph-2.1.2/README.md
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 03:02:48.779505 c-shelph-2.1.2/c_shelph.egg-info/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      468 2023-05-06 03:02:48.000000 c-shelph-2.1.2/c_shelph.egg-info/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      169 2023-05-06 03:02:48.000000 c-shelph-2.1.2/c_shelph.egg-info/SOURCES.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 03:02:48.000000 c-shelph-2.1.2/c_shelph.egg-info/dependency_links.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-06 03:02:48.000000 c-shelph-2.1.2/c_shelph.egg-info/top_level.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    19075 2023-05-04 16:18:29.000000 c-shelph-2.1.2/cshelph.py
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-06 03:02:48.779840 c-shelph-2.1.2/setup.cfg
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1572 2023-05-06 03:02:45.000000 c-shelph-2.1.2/setup.py
```

### Comparing `c-shelph-2.1.1/LICENSE.txt` & `c-shelph-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `c-shelph-2.1.1/README.md` & `c-shelph-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `c-shelph-2.1.1/bathy_utils.py` & `c-shelph-2.1.2/cshelph.py`

 * *Files identical despite different names*

### Comparing `c-shelph-2.1.1/setup.py` & `c-shelph-2.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 #
 # Author: Nathan Thomas
 # Email: nmthomas28@gmail.com
 # Date: 05/05/2023
 # Version: 2.1.1
 #
 # History:
-# Version 2.1.1
+# Version 2.1.2
 
 from distutils.core import setup
 import os
 
 setup(name='c-shelph',
-    version='2.1.1',
+    version='2.1.2',
     description='Classification of Sub-aquatic Height Extracted Photons',
     author='Nathan Thomas and Brian Lee',
     author_email='nmthomas28@gmail.com',
-    scripts=['bathy_utils.py'],
+    scripts=['cshelph.py'],
     package_dir={},
     data_files=[],
     license='LICENSE.txt',
     url='https://github.com/nmt28/C-SHELPh',
     classifiers=['Intended Audience :: Developers',
                  'Intended Audience :: Science/Research',
                  'Operating System :: OS Independent',
```

