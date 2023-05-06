# Comparing `tmp/kynaylibs-3.0.0.tar.gz` & `tmp/kynaylibs-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-3.0.0.tar", last modified: Sat May  6 10:00:58 2023, max compression
+gzip compressed data, was "kynaylibs-7.0.1.tar", last modified: Sat May  6 10:24:55 2023, max compression
```

## Comparing `kynaylibs-3.0.0.tar` & `kynaylibs-7.0.1.tar`

### file list

```diff
@@ -1,12 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:00:58.442190 kynaylibs-3.0.0/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-06 09:59:38.000000 kynaylibs-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:00:58.442190 kynaylibs-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-06 09:59:38.000000 kynaylibs-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:00:58.442190 kynaylibs-3.0.0/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:00:58.000000 kynaylibs-3.0.0/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-06 10:00:58.000000 kynaylibs-3.0.0/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 10:00:58.000000 kynaylibs-3.0.0/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-06 10:00:58.000000 kynaylibs-3.0.0/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 10:00:58.000000 kynaylibs-3.0.0/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 10:00:58.442190 kynaylibs-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1576 2023-05-06 10:00:46.000000 kynaylibs-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:24:55.422133 kynaylibs-7.0.1/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:24:55.422133 kynaylibs-7.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:24:55.422133 kynaylibs-7.0.1/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-06 10:24:44.000000 kynaylibs-7.0.1/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:24:55.422133 kynaylibs-7.0.1/kynaylibs/core/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/ai.py
+-rw-r--r--   0 root         (0) root         (0)    15600 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/cos_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:24:55.422133 kynaylibs-7.0.1/kynaylibs/core/db/
+-rw-r--r--   0 root         (0) root         (0)     9321 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/db/pmpermit.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/filter.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/func.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/inline.py
+-rw-r--r--   0 root         (0) root         (0)    17800 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/lgs.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/core/what.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:24:55.422133 kynaylibs-7.0.1/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-06 09:59:38.000000 kynaylibs-7.0.1/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:24:55.422133 kynaylibs-7.0.1/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:24:55.000000 kynaylibs-7.0.1/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      572 2023-05-06 10:24:55.000000 kynaylibs-7.0.1/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 10:24:55.000000 kynaylibs-7.0.1/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-06 10:24:55.000000 kynaylibs-7.0.1/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-06 10:24:55.000000 kynaylibs-7.0.1/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 10:24:55.422133 kynaylibs-7.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-05-06 10:24:44.000000 kynaylibs-7.0.1/setup.py
```

### Comparing `kynaylibs-3.0.0/LICENSE` & `kynaylibs-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-3.0.0/PKG-INFO` & `kynaylibs-7.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 3.0.0
+Version: 7.0.1
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-3.0.0/README.md` & `kynaylibs-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-3.0.0/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-7.0.1/kynaylibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 3.0.0
+Version: 7.0.1
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-3.0.0/setup.py` & `kynaylibs-7.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
+from sys import argv
 
 import setuptools
 
-requirements = ["pyrogram", "pymongo", "python-decouple", "python-dotenv", "pyaes", "tgcrypto", "uvloop", "aiohttp", "wget"]
+with open("requirements.txt", encoding="utf-8") as r:
+    requirements = [i.strip() for i in r]
 
-with open("kynaylibs/version.py", "rt", encoding="utf8") as x:
+with open("kynaylibs/__init__.py", "rt", encoding="utf8") as x:
     version = re.search(r'__version__ = "(.*?)"', x.read()).group(1)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 name = "kynaylibs"
 author = "naya1503"
```

