# Comparing `tmp/pyroporn-0.2.6.tar.gz` & `tmp/pyroporn-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroporn-0.2.6.tar", last modified: Sat May  6 08:52:22 2023, max compression
+gzip compressed data, was "pyroporn-0.2.7.tar", last modified: Sat May  6 08:55:48 2023, max compression
```

## Comparing `pyroporn-0.2.6.tar` & `pyroporn-0.2.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:52:22.340856 pyroporn-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 08:52:22.340856 pyroporn-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 08:52:10.000000 pyroporn-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:52:22.336856 pyroporn-0.2.6/pyroporn/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:52:22.340856 pyroporn-0.2.6/pyroporn/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:52:22.340856 pyroporn-0.2.6/pyroporn/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/decorators/genbuttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/decorators/getjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/decorators/getlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:52:22.340856 pyroporn-0.2.6/pyroporn/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:52:22.340856 pyroporn-0.2.6/pyroporn/types/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:52:22.340856 pyroporn-0.2.6/pyroporn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/utilities/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 08:52:10.000000 pyroporn-0.2.6/pyroporn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:52:22.336856 pyroporn-0.2.6/pyroporn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 08:52:22.000000 pyroporn-0.2.6/pyroporn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-06 08:52:22.000000 pyroporn-0.2.6/pyroporn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:52:22.000000 pyroporn-0.2.6/pyroporn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 08:52:22.000000 pyroporn-0.2.6/pyroporn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 08:52:22.000000 pyroporn-0.2.6/pyroporn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:52:22.340856 pyroporn-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-06 08:52:10.000000 pyroporn-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:55:48.709432 pyroporn-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 08:55:48.709432 pyroporn-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 08:55:31.000000 pyroporn-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:55:48.701432 pyroporn-0.2.7/pyroporn/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:55:48.705433 pyroporn-0.2.7/pyroporn/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:55:48.705433 pyroporn-0.2.7/pyroporn/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/decorators/genbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/decorators/getjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/decorators/getlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:55:48.705433 pyroporn-0.2.7/pyroporn/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:55:48.709432 pyroporn-0.2.7/pyroporn/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:55:48.709432 pyroporn-0.2.7/pyroporn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/utilities/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 08:55:31.000000 pyroporn-0.2.7/pyroporn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:55:48.701432 pyroporn-0.2.7/pyroporn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 08:55:48.000000 pyroporn-0.2.7/pyroporn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-06 08:55:48.000000 pyroporn-0.2.7/pyroporn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:55:48.000000 pyroporn-0.2.7/pyroporn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 08:55:48.000000 pyroporn-0.2.7/pyroporn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 08:55:48.000000 pyroporn-0.2.7/pyroporn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:55:48.709432 pyroporn-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-06 08:55:31.000000 pyroporn-0.2.7/setup.py
```

### Comparing `pyroporn-0.2.6/PKG-INFO` & `pyroporn-0.2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.2.6
+Version: 0.2.7
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.2.6/pyroporn/client.py` & `pyroporn-0.2.7/pyroporn/client.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/config.py` & `pyroporn-0.2.7/pyroporn/config.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/database/bdbDatabase.py` & `pyroporn-0.2.7/pyroporn/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/database/bubDatabase.py` & `pyroporn-0.2.7/pyroporn/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/database/othDatabase.py` & `pyroporn-0.2.7/pyroporn/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/database/papDatabase.py` & `pyroporn-0.2.7/pyroporn/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/database/pmoDatabase.py` & `pyroporn-0.2.7/pyroporn/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/database/pobDatabase.py` & `pyroporn-0.2.7/pyroporn/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/decorators/forcesub.py` & `pyroporn-0.2.7/pyroporn/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/decorators/genbuttons.py` & `pyroporn-0.2.7/pyroporn/decorators/genbuttons.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/decorators/getlink.py` & `pyroporn-0.2.7/pyroporn/decorators/getlink.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/decorators/oncmd.py` & `pyroporn-0.2.7/pyroporn/decorators/oncmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyrogram import filters, enums
-
+from pyrogram.handlers import MessageHandler
 from pyrogram.errors.exceptions.bad_request_400 import MessageIdInvalid
 
 
 class OnCmd:
     """
     ## Available Functions:
     
@@ -80,8 +80,8 @@
 
         ### Arguments:
 
             ``function``: Callback function
             ``filterm``: Filters
             ``cmdgrp``: Command Group
         """
-        self.add_handler(MessageHandler(function, filterm), cmdgrp)
+        self.add_handler(MessageHandler(function, filterm), cmdgrp)
```

### Comparing `pyroporn-0.2.6/pyroporn/methods/content.py` & `pyroporn-0.2.7/pyroporn/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/methods/getfile.py` & `pyroporn-0.2.7/pyroporn/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/methods/message.py` & `pyroporn-0.2.7/pyroporn/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/methods/thumbnail.py` & `pyroporn-0.2.7/pyroporn/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/types/inline.py` & `pyroporn-0.2.7/pyroporn/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/types/inlineBdb.py` & `pyroporn-0.2.7/pyroporn/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/types/inlineBub.py` & `pyroporn-0.2.7/pyroporn/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/types/inlinePob.py` & `pyroporn-0.2.7/pyroporn/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/types/inlineVip.py` & `pyroporn-0.2.7/pyroporn/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/types/text.py` & `pyroporn-0.2.7/pyroporn/types/text.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/utilities/formater.py` & `pyroporn-0.2.7/pyroporn/utilities/formater.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/utilities/logger.py` & `pyroporn-0.2.7/pyroporn/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/utilities/mongo.py` & `pyroporn-0.2.7/pyroporn/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn/utilities/utils.py` & `pyroporn-0.2.7/pyroporn/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/pyroporn.egg-info/PKG-INFO` & `pyroporn-0.2.7/pyroporn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.2.6
+Version: 0.2.7
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.2.6/pyroporn.egg-info/SOURCES.txt` & `pyroporn-0.2.7/pyroporn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.6/setup.py` & `pyroporn-0.2.7/setup.py`

 * *Files identical despite different names*

