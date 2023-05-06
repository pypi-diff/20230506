# Comparing `tmp/wikihowapi_pk-0.0.4.tar.gz` & `tmp/wikihowapi_pk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikihowapi_pk-0.0.4.tar", last modified: Sat May  6 13:54:04 2023, max compression
+gzip compressed data, was "wikihowapi_pk-0.0.5.tar", last modified: Sat May  6 13:57:56 2023, max compression
```

## Comparing `wikihowapi_pk-0.0.4.tar` & `wikihowapi_pk-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:54:04.153714 wikihowapi_pk-0.0.4/
--rw-r--r--   0 piko       (501) staff       (20)     1101 2023-05-03 09:56:00.000000 wikihowapi_pk-0.0.4/LICENSE
--rw-r--r--   0 piko       (501) staff       (20)     9276 2023-05-06 13:54:04.153475 wikihowapi_pk-0.0.4/PKG-INFO
--rw-r--r--   0 piko       (501) staff       (20)     8758 2023-05-06 13:52:37.000000 wikihowapi_pk-0.0.4/README.md
--rw-r--r--   0 piko       (501) staff       (20)       38 2023-05-06 13:54:04.153764 wikihowapi_pk-0.0.4/setup.cfg
--rw-r--r--   0 piko       (501) staff       (20)      791 2023-05-06 13:49:01.000000 wikihowapi_pk-0.0.4/setup.py
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:54:04.152094 wikihowapi_pk-0.0.4/tests/
--rw-r--r--   0 piko       (501) staff       (20)      984 2023-05-06 13:02:39.000000 wikihowapi_pk-0.0.4/tests/test.py
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:54:04.152446 wikihowapi_pk-0.0.4/wikihowapi_pk/
--rw-r--r--   0 piko       (501) staff       (20)    28292 2023-05-06 13:48:18.000000 wikihowapi_pk-0.0.4/wikihowapi_pk/__init__.py
--rw-r--r--   0 piko       (501) staff       (20)      194 2023-05-03 09:37:40.000000 wikihowapi_pk-0.0.4/wikihowapi_pk/exceptions.py
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:54:04.153232 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/
--rw-r--r--   0 piko       (501) staff       (20)     9276 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/PKG-INFO
--rw-r--r--   0 piko       (501) staff       (20)      278 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/SOURCES.txt
--rw-r--r--   0 piko       (501) staff       (20)        1 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/dependency_links.txt
--rw-r--r--   0 piko       (501) staff       (20)        9 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/requires.txt
--rw-r--r--   0 piko       (501) staff       (20)       14 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/top_level.txt
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:57:56.416785 wikihowapi_pk-0.0.5/
+-rw-r--r--   0 piko       (501) staff       (20)     1101 2023-05-03 09:56:00.000000 wikihowapi_pk-0.0.5/LICENSE
+-rw-r--r--   0 piko       (501) staff       (20)     9276 2023-05-06 13:57:56.416530 wikihowapi_pk-0.0.5/PKG-INFO
+-rw-r--r--   0 piko       (501) staff       (20)     8758 2023-05-06 13:52:37.000000 wikihowapi_pk-0.0.5/README.md
+-rw-r--r--   0 piko       (501) staff       (20)       38 2023-05-06 13:57:56.416840 wikihowapi_pk-0.0.5/setup.cfg
+-rw-r--r--   0 piko       (501) staff       (20)      791 2023-05-06 13:57:40.000000 wikihowapi_pk-0.0.5/setup.py
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:57:56.415136 wikihowapi_pk-0.0.5/tests/
+-rw-r--r--   0 piko       (501) staff       (20)      984 2023-05-06 13:02:39.000000 wikihowapi_pk-0.0.5/tests/test.py
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:57:56.415492 wikihowapi_pk-0.0.5/wikihowapi_pk/
+-rw-r--r--   0 piko       (501) staff       (20)    28290 2023-05-06 13:57:52.000000 wikihowapi_pk-0.0.5/wikihowapi_pk/__init__.py
+-rw-r--r--   0 piko       (501) staff       (20)      194 2023-05-03 09:37:40.000000 wikihowapi_pk-0.0.5/wikihowapi_pk/exceptions.py
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:57:56.416286 wikihowapi_pk-0.0.5/wikihowapi_pk.egg-info/
+-rw-r--r--   0 piko       (501) staff       (20)     9276 2023-05-06 13:57:56.000000 wikihowapi_pk-0.0.5/wikihowapi_pk.egg-info/PKG-INFO
+-rw-r--r--   0 piko       (501) staff       (20)      278 2023-05-06 13:57:56.000000 wikihowapi_pk-0.0.5/wikihowapi_pk.egg-info/SOURCES.txt
+-rw-r--r--   0 piko       (501) staff       (20)        1 2023-05-06 13:57:56.000000 wikihowapi_pk-0.0.5/wikihowapi_pk.egg-info/dependency_links.txt
+-rw-r--r--   0 piko       (501) staff       (20)        9 2023-05-06 13:57:56.000000 wikihowapi_pk-0.0.5/wikihowapi_pk.egg-info/requires.txt
+-rw-r--r--   0 piko       (501) staff       (20)       14 2023-05-06 13:57:56.000000 wikihowapi_pk-0.0.5/wikihowapi_pk.egg-info/top_level.txt
```

### Comparing `wikihowapi_pk-0.0.4/LICENSE` & `wikihowapi_pk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wikihowapi_pk-0.0.4/PKG-INFO` & `wikihowapi_pk-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikihowapi_pk
-Version: 0.0.4
+Version: 0.0.5
 Summary: API to extract more data from wikiHow
 Home-page: https://github.com/p1k0pan/AdaptiveStoryFinder.git
 Author: p1k0pan
 Author-email: pan.jingheng1998@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wikihowapi_pk-0.0.4/README.md` & `wikihowapi_pk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wikihowapi_pk-0.0.4/setup.py` & `wikihowapi_pk-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='wikihowapi_pk',
-    version='0.0.4',
+    version='0.0.5',
     description='API to extract more data from wikiHow',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/p1k0pan/AdaptiveStoryFinder.git',
     author='p1k0pan',
     author_email='pan.jingheng1998@gmail.com',
     license='MIT',
```

### Comparing `wikihowapi_pk-0.0.4/tests/test.py` & `wikihowapi_pk-0.0.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `wikihowapi_pk-0.0.4/wikihowapi_pk/__init__.py` & `wikihowapi_pk-0.0.5/wikihowapi_pk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 wikihowAPI_pk
 
 API to extract data from wikiHow.
 """
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 __author__ = 'Aniket Sharma, Ashok Arora, p1k0pan'
 __credits__ = 'Aniket Sharma & Ashok Arora & p1k0pan'
 
 from bs4 import BeautifulSoup
 import urllib.request
 from wikihowapi_pk.exceptions import *
 from datetime import datetime
@@ -824,15 +824,15 @@
             views = result_data.find('li', {'class': 'sr_view'}).text.strip()
             update = result_data.find('li', {'class': 'sr_updated'}).text
             update = update[:8].lstrip()+" "+update[8:].strip()
             sp_verif = result_data.find('li', {'class': 'sp_verif'})
             if sp_verif:
                 sp_verif = sp_verif.text.strip()
             else:
-                sp_verif = None
+                sp_verif = ""
 
 
 
             result_dict["url"]=url
             result_dict["img_url"]=img_rul
             result_dict["title"]=title
             result_dict["update"] = update
```

### Comparing `wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/PKG-INFO` & `wikihowapi_pk-0.0.5/wikihowapi_pk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikihowapi-pk
-Version: 0.0.4
+Version: 0.0.5
 Summary: API to extract more data from wikiHow
 Home-page: https://github.com/p1k0pan/AdaptiveStoryFinder.git
 Author: p1k0pan
 Author-email: pan.jingheng1998@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

