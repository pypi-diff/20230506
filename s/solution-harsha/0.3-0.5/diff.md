# Comparing `tmp/solution_harsha-0.3.tar.gz` & `tmp/solution_harsha-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solution_harsha-0.3.tar", last modified: Sat May  6 18:01:21 2023, max compression
+gzip compressed data, was "solution_harsha-0.5.tar", last modified: Sat May  6 18:18:50 2023, max compression
```

## Comparing `solution_harsha-0.3.tar` & `solution_harsha-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:01:21.436138 solution_harsha-0.3/
--rw-rw-rw-   0        0        0      196 2023-05-06 18:01:21.436138 solution_harsha-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2177 2023-05-06 17:44:45.000000 solution_harsha-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 18:01:21.436138 solution_harsha-0.3/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-05-06 18:01:01.000000 solution_harsha-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:01:21.426138 solution_harsha-0.3/solution_harsha/
--rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.3/solution_harsha/__init__.py
--rw-rw-rw-   0        0        0       96 2023-05-06 14:20:44.000000 solution_harsha-0.3/solution_harsha/config.yaml
--rw-rw-rw-   0        0        0     4817 2023-05-06 18:00:30.000000 solution_harsha-0.3/solution_harsha/di_testcode.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:01:21.434136 solution_harsha-0.3/solution_harsha.egg-info/
--rw-rw-rw-   0        0        0      196 2023-05-06 18:01:21.000000 solution_harsha-0.3/solution_harsha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-06 18:01:21.000000 solution_harsha-0.3/solution_harsha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:01:21.000000 solution_harsha-0.3/solution_harsha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-06 18:01:21.000000 solution_harsha-0.3/solution_harsha.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-06 18:01:21.000000 solution_harsha-0.3/solution_harsha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 18:01:21.000000 solution_harsha-0.3/solution_harsha.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 18:18:50.647801 solution_harsha-0.5/
+-rw-rw-rw-   0        0        0      196 2023-05-06 18:18:50.646801 solution_harsha-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2177 2023-05-06 17:44:45.000000 solution_harsha-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 18:18:50.647801 solution_harsha-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-05-06 18:18:36.000000 solution_harsha-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:18:50.637802 solution_harsha-0.5/solution_harsha/
+-rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.5/solution_harsha/__init__.py
+-rw-rw-rw-   0        0        0       95 2023-05-06 18:11:21.000000 solution_harsha-0.5/solution_harsha/config.yaml
+-rw-rw-rw-   0        0        0     4817 2023-05-06 18:09:34.000000 solution_harsha-0.5/solution_harsha/di_testcode.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:18:50.645801 solution_harsha-0.5/solution_harsha.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-05-06 18:18:50.000000 solution_harsha-0.5/solution_harsha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-06 18:18:50.000000 solution_harsha-0.5/solution_harsha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:18:50.000000 solution_harsha-0.5/solution_harsha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-06 18:18:50.000000 solution_harsha-0.5/solution_harsha.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-06 18:18:50.000000 solution_harsha-0.5/solution_harsha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 18:18:50.000000 solution_harsha-0.5/solution_harsha.egg-info/top_level.txt
```

### Comparing `solution_harsha-0.3/README.md` & `solution_harsha-0.5/README.md`

 * *Files identical despite different names*

### Comparing `solution_harsha-0.3/setup.py` & `solution_harsha-0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solution_harsha',
-    version='0.3',
+    version='0.5',
     description='A tool for performing string matching on text files',
     author='Sriharsha Aryasomayajula',
     author_email='harshaarya17@outlook.com',
     packages=find_packages(),
     package_data={"": ["config.yaml"]},
     include_package_data=True,
     install_requires=[
         'ruamel.yaml',
         'regex',
         'argparse',
     ],
     entry_points={
         'console_scripts': [
-            'stringapp=solution_harsha.di_testcode:main',
+            'stringapp_di=solution_harsha.di_testcode:main',
         ],
     },
 )
```

### Comparing `solution_harsha-0.3/solution_harsha/di_testcode.py` & `solution_harsha-0.5/solution_harsha/di_testcode.py`

 * *Files identical despite different names*

