# Comparing `tmp/screenshots_pagepixels-1.0.1.tar.gz` & `tmp/screenshots_pagepixels-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenshots_pagepixels-1.0.1.tar", last modified: Sat May  6 20:36:56 2023, max compression
+gzip compressed data, was "screenshots_pagepixels-1.0.3.tar", last modified: Sat May  6 20:50:12 2023, max compression
```

## Comparing `screenshots_pagepixels-1.0.1.tar` & `screenshots_pagepixels-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 20:36:56.917949 screenshots_pagepixels-1.0.1/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1081 2023-05-06 20:04:33.000000 screenshots_pagepixels-1.0.1/LICENSE.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     8614 2023-05-06 20:36:56.917949 screenshots_pagepixels-1.0.1/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7616 2023-05-06 20:09:23.000000 screenshots_pagepixels-1.0.1/README.md
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 20:36:56.913949 screenshots_pagepixels-1.0.1/screenshots_pagepixels.egg-info/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     8614 2023-05-06 20:36:56.000000 screenshots_pagepixels-1.0.1/screenshots_pagepixels.egg-info/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      259 2023-05-06 20:36:56.000000 screenshots_pagepixels-1.0.1/screenshots_pagepixels.egg-info/SOURCES.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        1 2023-05-06 20:36:56.000000 screenshots_pagepixels-1.0.1/screenshots_pagepixels.egg-info/dependency_links.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        9 2023-05-06 20:36:56.000000 screenshots_pagepixels-1.0.1/screenshots_pagepixels.egg-info/requires.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        1 2023-05-06 20:36:56.000000 screenshots_pagepixels-1.0.1/screenshots_pagepixels.egg-info/top_level.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       38 2023-05-06 20:36:56.917949 screenshots_pagepixels-1.0.1/setup.cfg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1284 2023-05-06 20:35:55.000000 screenshots_pagepixels-1.0.1/setup.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1081 2023-05-06 20:04:33.000000 screenshots_pagepixels-1.0.3/LICENSE.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     8614 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/PKG-INFO
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7616 2023-05-06 20:09:23.000000 screenshots_pagepixels-1.0.3/README.md
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/screenshots_pagepixels/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       41 2023-05-06 20:46:43.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2638 2023-05-06 20:24:16.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels/client.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     8614 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/PKG-INFO
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      327 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)        1 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)        9 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/requires.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       23 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/top_level.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       38 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/setup.cfg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1284 2023-05-06 20:49:55.000000 screenshots_pagepixels-1.0.3/setup.py
```

### Comparing `screenshots_pagepixels-1.0.1/LICENSE.txt` & `screenshots_pagepixels-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `screenshots_pagepixels-1.0.1/PKG-INFO` & `screenshots_pagepixels-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenshots_pagepixels
-Version: 1.0.1
+Version: 1.0.3
 Summary: Take immediate screenshots, create scheduled screenshots, take multi-step screenshots (click links, complete forms, login to websites), and get change notifications using the PagePixels Screenshot API python wrapper.
 Home-page: https://github.com/yourusername/screenshots_pagepixels
 Author: PagePixels LLC
 Author-email: support@pagepixels.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `screenshots_pagepixels-1.0.1/README.md` & `screenshots_pagepixels-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `screenshots_pagepixels-1.0.1/screenshots_pagepixels.egg-info/PKG-INFO` & `screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenshots-pagepixels
-Version: 1.0.1
+Version: 1.0.3
 Summary: Take immediate screenshots, create scheduled screenshots, take multi-step screenshots (click links, complete forms, login to websites), and get change notifications using the PagePixels Screenshot API python wrapper.
 Home-page: https://github.com/yourusername/screenshots_pagepixels
 Author: PagePixels LLC
 Author-email: support@pagepixels.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `screenshots_pagepixels-1.0.1/setup.py` & `screenshots_pagepixels-1.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of the README.md file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='screenshots_pagepixels',
-    version='1.0.1',
+    version='1.0.3',
     description='Take immediate screenshots, create scheduled screenshots, take multi-step screenshots (click links, complete forms, login to websites), and get change notifications using the PagePixels Screenshot API python wrapper.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='PagePixels LLC',
     author_email='support@pagepixels.com',
     url='https://github.com/yourusername/screenshots_pagepixels',
     packages=find_packages(),
```

