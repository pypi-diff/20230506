# Comparing `tmp/pymailauth-1.2.tar.gz` & `tmp/pymailauth-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymailauth-1.2.tar", last modified: Sat May  6 06:55:33 2023, max compression
+gzip compressed data, was "pymailauth-1.2.1.tar", last modified: Sat May  6 06:57:41 2023, max compression
```

## Comparing `pymailauth-1.2.tar` & `pymailauth-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2023-05-06 06:55:33.259135 pymailauth-1.2/
--rw-rw-r--   0 ankit     (1000) ankit     (1000)      407 2023-05-06 06:55:33.259135 pymailauth-1.2/PKG-INFO
-drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2023-05-06 06:55:33.259135 pymailauth-1.2/pymailauth/
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       29 2023-05-06 06:43:56.000000 pymailauth-1.2/pymailauth/__init__.py
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       56 2023-05-06 06:43:56.000000 pymailauth-1.2/pymailauth/consts.py
--rw-rw-r--   0 ankit     (1000) ankit     (1000)     3339 2023-05-06 06:43:56.000000 pymailauth-1.2/pymailauth/service.py
-drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2023-05-06 06:55:33.259135 pymailauth-1.2/pymailauth.egg-info/
--rw-rw-r--   0 ankit     (1000) ankit     (1000)      407 2023-05-06 06:55:33.000000 pymailauth-1.2/pymailauth.egg-info/PKG-INFO
--rw-rw-r--   0 ankit     (1000) ankit     (1000)      276 2023-05-06 06:55:33.000000 pymailauth-1.2/pymailauth.egg-info/SOURCES.txt
--rw-rw-r--   0 ankit     (1000) ankit     (1000)        1 2023-05-06 06:55:33.000000 pymailauth-1.2/pymailauth.egg-info/dependency_links.txt
--rw-rw-r--   0 ankit     (1000) ankit     (1000)        1 2023-05-06 06:33:01.000000 pymailauth-1.2/pymailauth.egg-info/not-zip-safe
--rw-rw-r--   0 ankit     (1000) ankit     (1000)      109 2023-05-06 06:55:33.000000 pymailauth-1.2/pymailauth.egg-info/requires.txt
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       11 2023-05-06 06:55:33.000000 pymailauth-1.2/pymailauth.egg-info/top_level.txt
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       38 2023-05-06 06:55:33.259135 pymailauth-1.2/setup.cfg
--rw-rw-r--   0 ankit     (1000) ankit     (1000)      808 2023-05-06 06:54:49.000000 pymailauth-1.2/setup.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2023-05-06 06:57:41.928746 pymailauth-1.2.1/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      408 2023-05-06 06:57:41.924746 pymailauth-1.2.1/PKG-INFO
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2023-05-06 06:57:41.924746 pymailauth-1.2.1/pymailauth/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       29 2023-05-06 06:43:56.000000 pymailauth-1.2.1/pymailauth/__init__.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       56 2023-05-06 06:43:56.000000 pymailauth-1.2.1/pymailauth/consts.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     3339 2023-05-06 06:43:56.000000 pymailauth-1.2.1/pymailauth/service.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2023-05-06 06:57:41.924746 pymailauth-1.2.1/pymailauth.egg-info/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      408 2023-05-06 06:57:41.000000 pymailauth-1.2.1/pymailauth.egg-info/PKG-INFO
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      276 2023-05-06 06:57:41.000000 pymailauth-1.2.1/pymailauth.egg-info/SOURCES.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        1 2023-05-06 06:57:41.000000 pymailauth-1.2.1/pymailauth.egg-info/dependency_links.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        1 2023-05-06 06:33:01.000000 pymailauth-1.2.1/pymailauth.egg-info/not-zip-safe
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      109 2023-05-06 06:57:41.000000 pymailauth-1.2.1/pymailauth.egg-info/requires.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       11 2023-05-06 06:57:41.000000 pymailauth-1.2.1/pymailauth.egg-info/top_level.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       38 2023-05-06 06:57:41.928746 pymailauth-1.2.1/setup.cfg
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      809 2023-05-06 06:56:44.000000 pymailauth-1.2.1/setup.py
```

### Comparing `pymailauth-1.2/pymailauth/service.py` & `pymailauth-1.2.1/pymailauth/service.py`

 * *Files identical despite different names*

### Comparing `pymailauth-1.2/setup.py` & `pymailauth-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 pymailauth is a python library which simplifies email setup
 for gmail. It is based on google oauth.
 Please refer readme for more details
 """
 
 setup(
     name="pymailauth",
-    version="1.2",
-    description="Python mail service for GMail",
+    version="1.2.1",
+    description="Python mail client for GMail",
     long_description=desc,
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     author="Ankit Kumar Pandey",
     author_email="itsankitkp@gmail.com",
     url="https://github.com/itsankitkp/pymailauth",
```

