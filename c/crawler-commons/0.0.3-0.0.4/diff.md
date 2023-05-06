# Comparing `tmp/crawler_commons-0.0.3.tar.gz` & `tmp/crawler_commons-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawler_commons-0.0.3.tar", last modified: Sat May  6 07:39:55 2023, max compression
+gzip compressed data, was "crawler_commons-0.0.4.tar", last modified: Sat May  6 07:43:01 2023, max compression
```

## Comparing `crawler_commons-0.0.3.tar` & `crawler_commons-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:39:55.330787 crawler_commons-0.0.3/
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.3/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:39:55.330556 crawler_commons-0.0.3/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.3/README.md
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:39:55.329080 crawler_commons-0.0.3/crawapi/
--rw-r--r--   0 nezah      (501) staff       (20)     2460 2023-05-06 07:35:34.000000 crawler_commons-0.0.3/crawapi/__init__.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:39:55.329941 crawler_commons-0.0.3/crawler_commons.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:39:55.000000 crawler_commons-0.0.3/crawler_commons.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      250 2023-05-06 07:39:55.000000 crawler_commons-0.0.3/crawler_commons.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-06 07:39:55.000000 crawler_commons-0.0.3/crawler_commons.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-06 07:39:55.000000 crawler_commons-0.0.3/crawler_commons.egg-info/top_level.txt
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:39:55.330312 crawler_commons-0.0.3/crawlutils/
--rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.3/crawlutils/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.3/crawlutils/text_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-06 07:39:55.330846 crawler_commons-0.0.3/setup.cfg
--rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-06 07:37:36.000000 crawler_commons-0.0.3/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:43:01.564264 crawler_commons-0.0.4/
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.4/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:43:01.564069 crawler_commons-0.0.4/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.4/README.md
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:43:01.562845 crawler_commons-0.0.4/crawapi/
+-rw-r--r--   0 nezah      (501) staff       (20)     2541 2023-05-06 07:42:57.000000 crawler_commons-0.0.4/crawapi/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:43:01.563509 crawler_commons-0.0.4/crawler_commons.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:43:01.000000 crawler_commons-0.0.4/crawler_commons.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      250 2023-05-06 07:43:01.000000 crawler_commons-0.0.4/crawler_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-06 07:43:01.000000 crawler_commons-0.0.4/crawler_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-06 07:43:01.000000 crawler_commons-0.0.4/crawler_commons.egg-info/top_level.txt
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:43:01.563846 crawler_commons-0.0.4/crawlutils/
+-rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.4/crawlutils/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.4/crawlutils/text_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-06 07:43:01.564319 crawler_commons-0.0.4/setup.cfg
+-rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-06 07:42:57.000000 crawler_commons-0.0.4/setup.py
```

### Comparing `crawler_commons-0.0.3/LICENSE` & `crawler_commons-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.3/crawapi/__init__.py` & `crawler_commons-0.0.4/crawapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import logging
 from typing import Dict
 
 import requests
 from bs4 import BeautifulSoup
-from cache import AdtCache
+from cache import AdtCache, MemoryCache
 
 from crawlutils.text_utils import make_num_include_zo, make_num
 
 logger = logging.getLogger("naverweb")
 
 naver_url = "https://finance.naver.com/item/main.nhn"
 
 
 class NaverWeb:
-    def __init__(self, cache: AdtCache):
+    def __init__(self, cache: AdtCache = None):
+        if cache is None:
+            cache = MemoryCache()
+
         self.cache: AdtCache = cache
 
     def get_stock_info(self, code) -> Dict[str, int]:
         """
         :param code:
         :return:
          - market_cap : 시가총액
```

### Comparing `crawler_commons-0.0.3/crawlutils/__init__.py` & `crawler_commons-0.0.4/crawlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.3/crawlutils/text_utils.py` & `crawler_commons-0.0.4/crawlutils/text_utils.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.3/setup.py` & `crawler_commons-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="crawler_commons",
-    version="0.0.3",
+    version="0.0.4",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="crawler commons",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/crawler_commons",
     packages=setuptools.find_packages(exclude=("test",)),
```

