# Comparing `tmp/steammy-0.1.3.tar.gz` & `tmp/steammy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steammy-0.1.3.tar", last modified: Sat May  6 19:52:01 2023, max compression
+gzip compressed data, was "steammy-0.1.4.tar", last modified: Sat May  6 20:54:50 2023, max compression
```

## Comparing `steammy-0.1.3.tar` & `steammy-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:52:01.768300 steammy-0.1.3/
--rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steammy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      427 2023-05-06 19:52:01.768300 steammy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       47 2023-05-06 18:02:42.000000 steammy-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 19:52:01.768300 steammy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      606 2023-05-06 19:51:50.000000 steammy-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:52:01.758571 steammy-0.1.3/steammy/
--rw-rw-rw-   0        0        0       28 2023-05-06 19:50:29.000000 steammy-0.1.3/steammy/__init__.py
--rw-rw-rw-   0        0        0      543 2023-05-05 21:51:45.000000 steammy-0.1.3/steammy/exceptions.py
--rw-rw-rw-   0        0        0    10436 2023-05-06 19:48:38.000000 steammy-0.1.3/steammy/request.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:52:01.768300 steammy-0.1.3/steammy.egg-info/
--rw-rw-rw-   0        0        0      427 2023-05-06 19:52:01.000000 steammy-0.1.3/steammy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-06 19:52:01.000000 steammy-0.1.3/steammy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:52:01.000000 steammy-0.1.3/steammy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 19:52:01.000000 steammy-0.1.3/steammy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 19:52:01.000000 steammy-0.1.3/steammy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 20:54:50.241535 steammy-0.1.4/
+-rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steammy-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      427 2023-05-06 20:54:50.241535 steammy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2023-05-06 18:02:42.000000 steammy-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 20:54:50.241535 steammy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      606 2023-05-06 20:54:35.000000 steammy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 20:54:50.231274 steammy-0.1.4/steammy/
+-rw-rw-rw-   0        0        0       28 2023-05-06 19:50:29.000000 steammy-0.1.4/steammy/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-05 21:51:45.000000 steammy-0.1.4/steammy/exceptions.py
+-rw-rw-rw-   0        0        0    10444 2023-05-06 20:53:40.000000 steammy-0.1.4/steammy/request.py
+drwxrwxrwx   0        0        0        0 2023-05-06 20:54:50.240538 steammy-0.1.4/steammy.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-05-06 20:54:50.000000 steammy-0.1.4/steammy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-06 20:54:50.000000 steammy-0.1.4/steammy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 20:54:50.000000 steammy-0.1.4/steammy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 20:54:50.000000 steammy-0.1.4/steammy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 20:54:50.000000 steammy-0.1.4/steammy.egg-info/top_level.txt
```

### Comparing `steammy-0.1.3/LICENSE` & `steammy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `steammy-0.1.3/setup.py` & `steammy-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='steammy',
-    version='0.1.3',
+    version='0.1.4',
     description='A package that helps extract Steam market data as pandas DataFrame for better readabilty and usage.',
     packages=["steammy"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Hungreeee',
     author_email='hungmnguyen13102003@gmail.com',
     license='MIT',
```

### Comparing `steammy-0.1.3/steammy/exceptions.py` & `steammy-0.1.4/steammy/exceptions.py`

 * *Files identical despite different names*

### Comparing `steammy-0.1.3/steammy/request.py` & `steammy-0.1.4/steammy/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 import json
 import pandas as pd
 import warnings
 
-from exceptions import exception
+from steammy.exceptions import exception
 
 warnings.simplefilter(action = "ignore", category = RuntimeWarning)
 
 class Request:
 
   def __init__(self):
     self.headers = {
```

