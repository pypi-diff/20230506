# Comparing `tmp/screenshots_pagepixels-1.0.3.tar.gz` & `tmp/screenshots_pagepixels-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenshots_pagepixels-1.0.3.tar", last modified: Sat May  6 20:50:12 2023, max compression
+gzip compressed data, was "screenshots_pagepixels-1.0.4.tar", last modified: Sat May  6 21:33:04 2023, max compression
```

## Comparing `screenshots_pagepixels-1.0.3.tar` & `screenshots_pagepixels-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1081 2023-05-06 20:04:33.000000 screenshots_pagepixels-1.0.3/LICENSE.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     8614 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7616 2023-05-06 20:09:23.000000 screenshots_pagepixels-1.0.3/README.md
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/screenshots_pagepixels/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       41 2023-05-06 20:46:43.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2638 2023-05-06 20:24:16.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels/client.py
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     8614 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      327 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/SOURCES.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        1 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/dependency_links.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        9 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/requires.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       23 2023-05-06 20:50:12.000000 screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/top_level.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       38 2023-05-06 20:50:12.909757 screenshots_pagepixels-1.0.3/setup.cfg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1284 2023-05-06 20:49:55.000000 screenshots_pagepixels-1.0.3/setup.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 21:33:04.300935 screenshots_pagepixels-1.0.4/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1081 2023-05-06 20:04:33.000000 screenshots_pagepixels-1.0.4/LICENSE.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     8582 2023-05-06 21:33:04.300935 screenshots_pagepixels-1.0.4/PKG-INFO
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7616 2023-05-06 20:09:23.000000 screenshots_pagepixels-1.0.4/README.md
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 21:33:04.300935 screenshots_pagepixels-1.0.4/screenshots_pagepixels/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       41 2023-05-06 20:46:43.000000 screenshots_pagepixels-1.0.4/screenshots_pagepixels/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2638 2023-05-06 20:24:16.000000 screenshots_pagepixels-1.0.4/screenshots_pagepixels/client.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-05-06 21:33:04.300935 screenshots_pagepixels-1.0.4/screenshots_pagepixels.egg-info/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     8582 2023-05-06 21:33:03.000000 screenshots_pagepixels-1.0.4/screenshots_pagepixels.egg-info/PKG-INFO
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      327 2023-05-06 21:33:04.000000 screenshots_pagepixels-1.0.4/screenshots_pagepixels.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)        1 2023-05-06 21:33:03.000000 screenshots_pagepixels-1.0.4/screenshots_pagepixels.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)        9 2023-05-06 21:33:04.000000 screenshots_pagepixels-1.0.4/screenshots_pagepixels.egg-info/requires.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       23 2023-05-06 21:33:04.000000 screenshots_pagepixels-1.0.4/screenshots_pagepixels.egg-info/top_level.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       38 2023-05-06 21:33:04.300935 screenshots_pagepixels-1.0.4/setup.cfg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1252 2023-05-06 21:32:48.000000 screenshots_pagepixels-1.0.4/setup.py
```

### Comparing `screenshots_pagepixels-1.0.3/LICENSE.txt` & `screenshots_pagepixels-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `screenshots_pagepixels-1.0.3/PKG-INFO` & `screenshots_pagepixels-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: screenshots_pagepixels
-Version: 1.0.3
+Version: 1.0.4
 Summary: Take immediate screenshots, create scheduled screenshots, take multi-step screenshots (click links, complete forms, login to websites), and get change notifications using the PagePixels Screenshot API python wrapper.
-Home-page: https://github.com/yourusername/screenshots_pagepixels
+Home-page: https://pagepixels.com
 Author: PagePixels LLC
 Author-email: support@pagepixels.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `screenshots_pagepixels-1.0.3/README.md` & `screenshots_pagepixels-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `screenshots_pagepixels-1.0.3/screenshots_pagepixels/client.py` & `screenshots_pagepixels-1.0.4/screenshots_pagepixels/client.py`

 * *Files identical despite different names*

### Comparing `screenshots_pagepixels-1.0.3/screenshots_pagepixels.egg-info/PKG-INFO` & `screenshots_pagepixels-1.0.4/screenshots_pagepixels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: screenshots-pagepixels
-Version: 1.0.3
+Version: 1.0.4
 Summary: Take immediate screenshots, create scheduled screenshots, take multi-step screenshots (click links, complete forms, login to websites), and get change notifications using the PagePixels Screenshot API python wrapper.
-Home-page: https://github.com/yourusername/screenshots_pagepixels
+Home-page: https://pagepixels.com
 Author: PagePixels LLC
 Author-email: support@pagepixels.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `screenshots_pagepixels-1.0.3/setup.py` & `screenshots_pagepixels-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 # Read the contents of the README.md file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='screenshots_pagepixels',
-    version='1.0.3',
+    version='1.0.4',
     description='Take immediate screenshots, create scheduled screenshots, take multi-step screenshots (click links, complete forms, login to websites), and get change notifications using the PagePixels Screenshot API python wrapper.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='PagePixels LLC',
     author_email='support@pagepixels.com',
-    url='https://github.com/yourusername/screenshots_pagepixels',
+    url='https://pagepixels.com',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

