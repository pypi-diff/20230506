# Comparing `tmp/crawler_commons-0.0.5.tar.gz` & `tmp/crawler_commons-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawler_commons-0.0.5.tar", last modified: Sat May  6 07:54:50 2023, max compression
+gzip compressed data, was "crawler_commons-0.0.6.tar", last modified: Sat May  6 07:57:22 2023, max compression
```

## Comparing `crawler_commons-0.0.5.tar` & `crawler_commons-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:54:50.939345 crawler_commons-0.0.5/
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.5/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:54:50.939059 crawler_commons-0.0.5/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.5/README.md
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:54:50.937340 crawler_commons-0.0.5/crawapi/
--rw-r--r--   0 nezah      (501) staff       (20)     2634 2023-05-06 07:54:17.000000 crawler_commons-0.0.5/crawapi/__init__.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:54:50.938221 crawler_commons-0.0.5/crawler_commons.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/crawler_commons.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      250 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/crawler_commons.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/crawler_commons.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/crawler_commons.egg-info/top_level.txt
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:54:50.938590 crawler_commons-0.0.5/crawlutils/
--rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.5/crawlutils/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.5/crawlutils/text_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-06 07:54:50.939414 crawler_commons-0.0.5/setup.cfg
--rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:57:22.875394 crawler_commons-0.0.6/
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.6/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:57:22.875200 crawler_commons-0.0.6/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.6/README.md
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:57:22.873460 crawler_commons-0.0.6/crawapi/
+-rw-r--r--   0 nezah      (501) staff       (20)     2634 2023-05-06 07:54:17.000000 crawler_commons-0.0.6/crawapi/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:57:22.874118 crawler_commons-0.0.6/crawler_commons.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/crawler_commons.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      328 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/crawler_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/crawler_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/crawler_commons.egg-info/top_level.txt
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:57:22.874967 crawler_commons-0.0.6/crawlutils/
+-rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.6/crawlutils/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1150 2022-12-27 06:40:36.000000 crawler_commons-0.0.6/crawlutils/date_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1131 2023-05-06 07:52:34.000000 crawler_commons-0.0.6/crawlutils/num_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1007 2023-05-06 07:56:32.000000 crawler_commons-0.0.6/crawlutils/soup_traversal.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.6/crawlutils/text_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-06 07:57:22.875450 crawler_commons-0.0.6/setup.cfg
+-rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/setup.py
```

### Comparing `crawler_commons-0.0.5/LICENSE` & `crawler_commons-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.5/crawapi/__init__.py` & `crawler_commons-0.0.6/crawapi/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.5/crawlutils/__init__.py` & `crawler_commons-0.0.6/crawlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.5/crawlutils/text_utils.py` & `crawler_commons-0.0.6/crawlutils/text_utils.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.5/setup.py` & `crawler_commons-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="crawler_commons",
-    version="0.0.5",
+    version="0.0.6",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="crawler commons",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/crawler_commons",
     packages=setuptools.find_packages(exclude=("test",)),
```

