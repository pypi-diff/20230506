# Comparing `tmp/solution_harsha-0.1.tar.gz` & `tmp/solution_harsha-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solution_harsha-0.1.tar", last modified: Sat May  6 14:04:34 2023, max compression
+gzip compressed data, was "solution_harsha-0.2.tar", last modified: Sat May  6 17:43:06 2023, max compression
```

## Comparing `solution_harsha-0.1.tar` & `solution_harsha-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 14:04:34.973318 solution_harsha-0.1/
--rw-rw-rw-   0        0        0       60 2023-05-06 14:04:34.973318 solution_harsha-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1723 2023-05-06 09:58:41.000000 solution_harsha-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 14:04:34.974292 solution_harsha-0.1/setup.cfg
--rw-rw-rw-   0        0        0      321 2023-05-06 14:02:12.000000 solution_harsha-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:04:34.963305 solution_harsha-0.1/solution_harsha/
--rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.1/solution_harsha/__init__.py
--rw-rw-rw-   0        0        0     4635 2023-05-06 13:53:22.000000 solution_harsha-0.1/solution_harsha/di_testcode.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:04:34.971293 solution_harsha-0.1/solution_harsha.egg-info/
--rw-rw-rw-   0        0        0       60 2023-05-06 14:04:34.000000 solution_harsha-0.1/solution_harsha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-05-06 14:04:34.000000 solution_harsha-0.1/solution_harsha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 14:04:34.000000 solution_harsha-0.1/solution_harsha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-06 14:04:34.000000 solution_harsha-0.1/solution_harsha.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 14:04:34.000000 solution_harsha-0.1/solution_harsha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 14:04:34.000000 solution_harsha-0.1/solution_harsha.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 17:43:06.463553 solution_harsha-0.2/
+-rw-rw-rw-   0        0        0      196 2023-05-06 17:43:06.461555 solution_harsha-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1723 2023-05-06 09:58:41.000000 solution_harsha-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:43:06.463553 solution_harsha-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      518 2023-05-06 15:49:46.000000 solution_harsha-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:43:06.450182 solution_harsha-0.2/solution_harsha/
+-rw-rw-rw-   0        0        0        0 2023-05-06 13:52:52.000000 solution_harsha-0.2/solution_harsha/__init__.py
+-rw-rw-rw-   0        0        0     4756 2023-05-06 14:28:59.000000 solution_harsha-0.2/solution_harsha/di_testcode.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:43:06.460553 solution_harsha-0.2/solution_harsha.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-05-06 17:43:06.000000 solution_harsha-0.2/solution_harsha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-05-06 17:43:06.000000 solution_harsha-0.2/solution_harsha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:43:06.000000 solution_harsha-0.2/solution_harsha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-06 17:43:06.000000 solution_harsha-0.2/solution_harsha.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-06 17:43:06.000000 solution_harsha-0.2/solution_harsha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 17:43:06.000000 solution_harsha-0.2/solution_harsha.egg-info/top_level.txt
```

### Comparing `solution_harsha-0.1/README.md` & `solution_harsha-0.2/README.md`

 * *Files identical despite different names*

### Comparing `solution_harsha-0.1/solution_harsha/di_testcode.py` & `solution_harsha-0.2/solution_harsha/di_testcode.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from pathlib import Path
 from ruamel.yaml import YAML
 import re
 import os
 
 log.basicConfig(level=log.INFO) #sets the basic logging level as info in that way any warnings or info statements are shown
 
+# os.chdir('../')
+
+# print(os.getcwd()) #future code to make the config path relative to the users working directry
+
 with open("config.yaml") as f:  #this opens the config.yaml
     yaml = YAML(typ='safe')
     params = yaml.load(f) #this sets the params file
     
 debug = params['test'] #if this is set to true then no need to pass arguments to di_testcode.py
 test_path = params['path'] #this is to ensure needless parameters are not passed as arguements while using test cases
```

