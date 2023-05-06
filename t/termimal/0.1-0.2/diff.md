# Comparing `tmp/termimal-0.1.tar.gz` & `tmp/termimal-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termimal-0.1.tar", last modified: Sat May  6 19:14:53 2023, max compression
+gzip compressed data, was "termimal-0.2.tar", last modified: Sat May  6 19:32:47 2023, max compression
```

## Comparing `termimal-0.1.tar` & `termimal-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:14:53.053402 termimal-0.1/
--rw-rw-rw-   0        0        0      627 2023-05-06 19:14:53.045215 termimal-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-05-06 17:46:56.000000 termimal-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 19:14:53.053402 termimal-0.1/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-05-06 17:49:31.000000 termimal-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:14:53.045215 termimal-0.1/termimal.egg-info/
--rw-rw-rw-   0        0        0      627 2023-05-06 19:14:52.000000 termimal-0.1/termimal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-06 19:14:52.000000 termimal-0.1/termimal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:14:52.000000 termimal-0.1/termimal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 19:14:52.000000 termimal-0.1/termimal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:14:52.000000 termimal-0.1/termimal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 19:32:47.244912 termimal-0.2/
+-rw-rw-rw-   0        0        0      613 2023-05-06 19:32:47.236731 termimal-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-05-06 17:46:56.000000 termimal-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 19:32:47.244912 termimal-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-05-06 19:32:30.000000 termimal-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:32:47.236731 termimal-0.2/termimal.egg-info/
+-rw-rw-rw-   0        0        0      613 2023-05-06 19:32:46.000000 termimal-0.2/termimal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-06 19:32:47.000000 termimal-0.2/termimal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:32:46.000000 termimal-0.2/termimal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 19:32:47.000000 termimal-0.2/termimal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:32:47.000000 termimal-0.2/termimal.egg-info/top_level.txt
```

### Comparing `termimal-0.1/PKG-INFO` & `termimal-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: termimal
-Version: 0.1
+Version: 0.2
 Summary: termimal simple
 Home-page: https://github.com/julianurielar/terminal.git
 Author: julian uriel weitzman
 Author-email: weijulian3@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-
-# terminal
```

### Comparing `termimal-0.1/setup.py` & `termimal-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='termimal',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     url='https://github.com/julianurielar/terminal.git',
     license='MIT',
     author='julian uriel weitzman',
     author_email='weijulian3@gmail.com',
     description='termimal simple',
-    long_description=open('README.md').read(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `termimal-0.1/termimal.egg-info/PKG-INFO` & `termimal-0.2/termimal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: termimal
-Version: 0.1
+Version: 0.2
 Summary: termimal simple
 Home-page: https://github.com/julianurielar/terminal.git
 Author: julian uriel weitzman
 Author-email: weijulian3@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-
-# terminal
```

