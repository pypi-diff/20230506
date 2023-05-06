# Comparing `tmp/cshelph-2.3.1.tar.gz` & `tmp/cshelph-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshelph-2.3.1.tar", last modified: Sat May  6 17:45:09 2023, max compression
+gzip compressed data, was "cshelph-2.3.2.tar", last modified: Sat May  6 18:55:12 2023, max compression
```

## Comparing `cshelph-2.3.1.tar` & `cshelph-2.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 17:45:09.689202 cshelph-2.3.1/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.3.1/LICENSE.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 17:45:09.689076 cshelph-2.3.1/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1165 2023-05-02 19:47:21.000000 cshelph-2.3.1/README.md
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 17:45:09.688903 cshelph-2.3.1/cshelph.egg-info/
--rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 17:45:09.000000 cshelph-2.3.1/cshelph.egg-info/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-06 17:45:09.000000 cshelph-2.3.1/cshelph.egg-info/SOURCES.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 17:45:09.000000 cshelph-2.3.1/cshelph.egg-info/dependency_links.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-06 17:45:09.000000 cshelph-2.3.1/cshelph.egg-info/top_level.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)    18618 2023-05-06 15:38:00.000000 cshelph-2.3.1/cshelph.py
--rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-06 17:45:09.689238 cshelph-2.3.1/setup.cfg
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1571 2023-05-06 17:44:02.000000 cshelph-2.3.1/setup.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 18:55:12.853869 cshelph-2.3.2/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.3.2/LICENSE.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3067 2023-05-06 18:55:12.853721 cshelph-2.3.2/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     2559 2023-05-06 18:41:33.000000 cshelph-2.3.2/README.md
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 18:55:12.853512 cshelph-2.3.2/cshelph.egg-info/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3067 2023-05-06 18:55:12.000000 cshelph-2.3.2/cshelph.egg-info/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-06 18:55:12.000000 cshelph-2.3.2/cshelph.egg-info/SOURCES.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 18:55:12.000000 cshelph-2.3.2/cshelph.egg-info/dependency_links.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-06 18:55:12.000000 cshelph-2.3.2/cshelph.egg-info/top_level.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    18618 2023-05-06 15:38:00.000000 cshelph-2.3.2/cshelph.py
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-06 18:55:12.853921 cshelph-2.3.2/setup.cfg
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-05-06 18:55:08.000000 cshelph-2.3.2/setup.py
```

### Comparing `cshelph-2.3.1/LICENSE.txt` & `cshelph-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cshelph-2.3.1/cshelph.py` & `cshelph-2.3.2/cshelph.py`

 * *Files identical despite different names*

### Comparing `cshelph-2.3.1/setup.py` & `cshelph-2.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,25 +23,27 @@
 #
 #
 # Purpose:  Installation of the C-SHELPh software
 #
 # Author: Nathan Thomas
 # Email: nmthomas28@gmail.com
 # Date: 05/05/2023
-# Version: 2.3.1
+# Version: 2.3.2
 #
 # History:
-# Version 2.3.1
+# Version 2.3.2
 
 from distutils.core import setup
 import os
 
 setup(name='cshelph',
-    version='2.3.1',
+    version='2.3.2',
     description='Classification of Sub-aquatic Height Extracted Photons',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author='Nathan Thomas and Brian Lee',
     author_email='nmthomas28@gmail.com',
     scripts=['cshelph.py'],
     package_dir={},
     data_files=[],
     license='LICENSE.txt',
     url='https://github.com/nmt28/C-SHELPh',
```

