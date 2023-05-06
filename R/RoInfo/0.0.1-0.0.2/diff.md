# Comparing `tmp/RoInfo-0.0.1.tar.gz` & `tmp/RoInfo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoInfo-0.0.1.tar", last modified: Sat May  6 06:36:06 2023, max compression
+gzip compressed data, was "RoInfo-0.0.2.tar", last modified: Sat May  6 07:13:22 2023, max compression
```

## Comparing `RoInfo-0.0.1.tar` & `RoInfo-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 06:36:06.287871 RoInfo-0.0.1/
--rw-rw-rw-   0        0        0      609 2023-05-06 06:36:06.284869 RoInfo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-06 05:53:11.000000 RoInfo-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 06:36:06.189903 RoInfo-0.0.1/RoInfo/
--rw-rw-rw-   0        0        0       26 2023-05-06 06:14:59.000000 RoInfo-0.0.1/RoInfo/__init__.py
--rw-rw-rw-   0        0        0     5188 2023-05-06 06:09:10.000000 RoInfo-0.0.1/RoInfo/auth.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:36:06.277343 RoInfo-0.0.1/RoInfo.egg-info/
--rw-rw-rw-   0        0        0      609 2023-05-06 06:36:06.000000 RoInfo-0.0.1/RoInfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-06 06:36:06.000000 RoInfo-0.0.1/RoInfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 06:36:06.000000 RoInfo-0.0.1/RoInfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-06 06:36:06.000000 RoInfo-0.0.1/RoInfo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 06:36:06.000000 RoInfo-0.0.1/RoInfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 06:36:06.288875 RoInfo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1004 2023-05-06 05:57:36.000000 RoInfo-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:13:21.999868 RoInfo-0.0.2/
+-rw-rw-rw-   0        0        0      609 2023-05-06 07:13:21.998878 RoInfo-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-06 05:53:11.000000 RoInfo-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 07:13:21.981523 RoInfo-0.0.2/RoInfo/
+-rw-rw-rw-   0        0        0     5188 2023-05-06 06:49:12.000000 RoInfo-0.0.2/RoInfo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:13:21.995544 RoInfo-0.0.2/RoInfo.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:13:22.000870 RoInfo-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-06 06:51:55.000000 RoInfo-0.0.2/setup.py
```

### Comparing `RoInfo-0.0.1/PKG-INFO` & `RoInfo-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoInfo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Roblox API Wrapper for roblox.com
 Home-page: 
 Author: Ryan_shamu
 Author-email: Ryanshamu418@Gmail.com
 Keywords: Roblox,RoInfo,Roblox Web Api,Roblox Python,Roblox For Python,Roblox Api,Roblox Api,Roblox Bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `RoInfo-0.0.1/RoInfo/auth.py` & `RoInfo-0.0.2/RoInfo/__init__.py`

 * *Files identical despite different names*

### Comparing `RoInfo-0.0.1/RoInfo.egg-info/PKG-INFO` & `RoInfo-0.0.2/RoInfo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoInfo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Roblox API Wrapper for roblox.com
 Home-page: 
 Author: Ryan_shamu
 Author-email: Ryanshamu418@Gmail.com
 Keywords: Roblox,RoInfo,Roblox Web Api,Roblox Python,Roblox For Python,Roblox Api,Roblox Api,Roblox Bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `RoInfo-0.0.1/setup.py` & `RoInfo-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A Roblox API Wrapper for roblox.com'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="RoInfo",
     version=VERSION,
     author="Ryan_shamu",
     author_email="Ryanshamu418@Gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     packages=find_packages(),
-    install_requires=["websocket-client","numpy","requests","bs4"],
+    install_requires=["websocket-client","numpy","requests","bs4", "re"],
     keywords=['Roblox', 'RoInfo', 'Roblox Web Api', 'Roblox Python', 'Roblox For Python', 'Roblox Api', 'Roblox Api', 'Roblox Bot'],
     url='',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

