# Comparing `tmp/kynaylibs-7.0.2.tar.gz` & `tmp/kynaylibs-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-7.0.2.tar", last modified: Sat May  6 10:35:57 2023, max compression
+gzip compressed data, was "kynaylibs-7.0.3.tar", last modified: Sat May  6 10:41:57 2023, max compression
```

## Comparing `kynaylibs-7.0.2.tar` & `kynaylibs-7.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:35:57.832837 kynaylibs-7.0.2/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:35:57.832837 kynaylibs-7.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:35:57.828837 kynaylibs-7.0.2/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-06 10:35:46.000000 kynaylibs-7.0.2/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:35:57.832837 kynaylibs-7.0.2/kynaylibs/core/
--rw-r--r--   0 root         (0) root         (0)      426 2023-05-06 10:35:46.000000 kynaylibs-7.0.2/kynaylibs/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/ai.py
--rw-r--r--   0 root         (0) root         (0)    15600 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/constants.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/cos_cmd.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:35:57.832837 kynaylibs-7.0.2/kynaylibs/core/db/
--rw-r--r--   0 root         (0) root         (0)     9321 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/db/pmpermit.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/filter.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/func.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/inline.py
--rw-r--r--   0 root         (0) root         (0)    17800 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/lgs.py
--rw-r--r--   0 root         (0) root         (0)     2611 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/core/what.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:35:57.832837 kynaylibs-7.0.2/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1275 2023-05-06 10:35:46.000000 kynaylibs-7.0.2/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-06 09:59:38.000000 kynaylibs-7.0.2/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:35:57.828837 kynaylibs-7.0.2/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:35:57.000000 kynaylibs-7.0.2/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-06 10:35:57.000000 kynaylibs-7.0.2/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 10:35:57.000000 kynaylibs-7.0.2/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-06 10:35:57.000000 kynaylibs-7.0.2/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-06 10:35:57.000000 kynaylibs-7.0.2/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 10:35:57.832837 kynaylibs-7.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-06 10:24:44.000000 kynaylibs-7.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.654969 kynaylibs-7.0.3/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-06 10:41:44.000000 kynaylibs-7.0.3/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.654969 kynaylibs-7.0.3/kynaylibs/core/
+-rw-r--r--   0 root         (0) root         (0)      426 2023-05-06 10:35:46.000000 kynaylibs-7.0.3/kynaylibs/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/ai.py
+-rw-r--r--   0 root         (0) root         (0)    15600 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/cos_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/kynaylibs/core/db/
+-rw-r--r--   0 root         (0) root         (0)     9282 2023-05-06 10:41:44.000000 kynaylibs-7.0.3/kynaylibs/core/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/db/pmpermit.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/filter.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/func.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/inline.py
+-rw-r--r--   0 root         (0) root         (0)    17800 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/lgs.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/core/what.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-05-06 10:35:46.000000 kynaylibs-7.0.3/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-06 09:59:38.000000 kynaylibs-7.0.3/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:41:57.654969 kynaylibs-7.0.3/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      572 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-06 10:41:57.000000 kynaylibs-7.0.3/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 10:41:57.658970 kynaylibs-7.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-05-06 10:24:44.000000 kynaylibs-7.0.3/setup.py
```

### Comparing `kynaylibs-7.0.2/LICENSE` & `kynaylibs-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/PKG-INFO` & `kynaylibs-7.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.0.2
+Version: 7.0.3
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.0.2/README.md` & `kynaylibs-7.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/ai.py` & `kynaylibs-7.0.3/kynaylibs/core/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/constants.py` & `kynaylibs-7.0.3/kynaylibs/core/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/cos_cmd.py` & `kynaylibs-7.0.3/kynaylibs/core/cos_cmd.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/db/__init__.py` & `kynaylibs-7.0.3/kynaylibs/core/db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from datetime import datetime, timedelta
 import pymongo.errors
 from platform import python_version as py
 from pyrogram import __version__ as pyro
 from ubotlibs.ubot.utils import *
 from Ubot.modules.basic import ADMINS
 from dateutil.relativedelta import relativedelta
-from ubotlibs.ubot.database import cli
 import asyncio
 import requests
 import asyncio
 from Ubot import *
 
 from motor.motor_asyncio import AsyncIOMotorClient as MongoCli
 from config import *
```

### Comparing `kynaylibs-7.0.2/kynaylibs/core/db/pmpermit.py` & `kynaylibs-7.0.3/kynaylibs/core/db/pmpermit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/filter.py` & `kynaylibs-7.0.3/kynaylibs/core/filter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/func.py` & `kynaylibs-7.0.3/kynaylibs/core/func.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/inline.py` & `kynaylibs-7.0.3/kynaylibs/core/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/lgs.py` & `kynaylibs-7.0.3/kynaylibs/core/lgs.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/core/what.py` & `kynaylibs-7.0.3/kynaylibs/core/what.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs/nan/__init__.py` & `kynaylibs-7.0.3/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-7.0.3/kynaylibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.0.2
+Version: 7.0.3
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.0.2/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-7.0.3/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.2/setup.py` & `kynaylibs-7.0.3/setup.py`

 * *Files identical despite different names*

