# Comparing `tmp/pyroporn-0.2.2.tar.gz` & `tmp/pyroporn-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroporn-0.2.2.tar", last modified: Sat May  6 07:51:42 2023, max compression
+gzip compressed data, was "pyroporn-0.2.3.tar", last modified: Sat May  6 08:22:05 2023, max compression
```

## Comparing `pyroporn-0.2.2.tar` & `pyroporn-0.2.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.396471 pyroporn-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 07:51:42.396471 pyroporn-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 07:51:31.000000 pyroporn-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/addhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/botcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/genbuttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/getjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/getlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.396471 pyroporn-0.2.2/pyroporn/types/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.396471 pyroporn-0.2.2/pyroporn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 07:51:31.000000 pyroporn-0.2.2/pyroporn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:51:42.392471 pyroporn-0.2.2/pyroporn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 07:51:42.000000 pyroporn-0.2.2/pyroporn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 07:51:42.396471 pyroporn-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-06 07:51:31.000000 pyroporn-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:05.047573 pyroporn-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 08:22:05.047573 pyroporn-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 08:21:53.000000 pyroporn-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:05.043573 pyroporn-0.2.3/pyroporn/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:05.043573 pyroporn-0.2.3/pyroporn/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:05.047573 pyroporn-0.2.3/pyroporn/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/addhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/botcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/genbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/getjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/getlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:05.047573 pyroporn-0.2.3/pyroporn/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:05.047573 pyroporn-0.2.3/pyroporn/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:05.047573 pyroporn-0.2.3/pyroporn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/utilities/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 08:21:53.000000 pyroporn-0.2.3/pyroporn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:05.043573 pyroporn-0.2.3/pyroporn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 08:22:05.000000 pyroporn-0.2.3/pyroporn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-06 08:22:05.000000 pyroporn-0.2.3/pyroporn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:22:05.000000 pyroporn-0.2.3/pyroporn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 08:22:05.000000 pyroporn-0.2.3/pyroporn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 08:22:05.000000 pyroporn-0.2.3/pyroporn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:22:05.047573 pyroporn-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-06 08:21:53.000000 pyroporn-0.2.3/setup.py
```

### Comparing `pyroporn-0.2.2/PKG-INFO` & `pyroporn-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.2.2
+Version: 0.2.3
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.2.2/pyroporn/client.py` & `pyroporn-0.2.3/pyroporn/client.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/config.py` & `pyroporn-0.2.3/pyroporn/config.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/database/bdbDatabase.py` & `pyroporn-0.2.3/pyroporn/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/database/bubDatabase.py` & `pyroporn-0.2.3/pyroporn/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/database/othDatabase.py` & `pyroporn-0.2.3/pyroporn/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/database/papDatabase.py` & `pyroporn-0.2.3/pyroporn/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/database/pmoDatabase.py` & `pyroporn-0.2.3/pyroporn/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/database/pobDatabase.py` & `pyroporn-0.2.3/pyroporn/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/decorators/botcmd.py` & `pyroporn-0.2.3/pyroporn/decorators/botcmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from pyrogram import filters, enums
 
 from pyrogram.errors.exceptions.bad_request_400 import MessageIdInvalid
 
 
 class BotCmd:
+    """
+    ## Available Functions:
+    
+      ``bot_cmd``: Main decorator
+      ``bot_cf``: Decorator to handle custom filters
+    """
+    @classmethod
     def bot_cmd(
         self,
         command: list,
         group: int = 0,
         owner: bool = False,
         private: bool = True
     ):
@@ -38,14 +45,15 @@
                     self.logs.error(e)
                     
             self.addhandler(filterm, wrapper, group)
             return wrapper
         return decorators 
     
     
+    @classmethod
     def bot_cf(self, custom_filters):
         """
         ## Decorator to handle custom filters
 
         ### Arguments:
 
             ``custom_filters``: Custom filters to handle
```

### Comparing `pyroporn-0.2.2/pyroporn/decorators/forcesub.py` & `pyroporn-0.2.3/pyroporn/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/decorators/genbuttons.py` & `pyroporn-0.2.3/pyroporn/decorators/genbuttons.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/decorators/getlink.py` & `pyroporn-0.2.3/pyroporn/decorators/getlink.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/decorators/oncmd.py` & `pyroporn-0.2.3/pyroporn/decorators/oncmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from pyrogram import filters, enums
 
 from pyrogram.errors.exceptions.bad_request_400 import MessageIdInvalid
 
 
 class OnCmd:
+    """
+    ## Available Functions:
+    
+      ``on_cmd``: Main decorator
+      ``on_cf``: Decorator to handle custom filters
+    """
+    @classmethod
     def on_cmd(
         self,
         command: list,
         group: int = 0,
         owner: bool = False,
         private: bool = True
     ):
@@ -38,14 +45,15 @@
                     self.logs.error(e)
                     
             self.addhandler(filterm, wrapper, group)
             return wrapper
         return decorators 
     
     
+    @classmethod
     def on_cf(self, custom_filters):
         """
         ## Decorator to handle custom filters
 
         ### Arguments:
 
             ``custom_filters``: Custom filters to handle
```

### Comparing `pyroporn-0.2.2/pyroporn/methods/content.py` & `pyroporn-0.2.3/pyroporn/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/methods/getfile.py` & `pyroporn-0.2.3/pyroporn/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/methods/message.py` & `pyroporn-0.2.3/pyroporn/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/methods/thumbnail.py` & `pyroporn-0.2.3/pyroporn/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/types/inline.py` & `pyroporn-0.2.3/pyroporn/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/types/inlineBdb.py` & `pyroporn-0.2.3/pyroporn/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/types/inlineBub.py` & `pyroporn-0.2.3/pyroporn/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/types/inlinePob.py` & `pyroporn-0.2.3/pyroporn/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/types/inlineVip.py` & `pyroporn-0.2.3/pyroporn/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/types/text.py` & `pyroporn-0.2.3/pyroporn/types/text.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/utilities/formater.py` & `pyroporn-0.2.3/pyroporn/utilities/formater.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/utilities/logger.py` & `pyroporn-0.2.3/pyroporn/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/utilities/mongo.py` & `pyroporn-0.2.3/pyroporn/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn/utilities/utils.py` & `pyroporn-0.2.3/pyroporn/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/pyroporn.egg-info/PKG-INFO` & `pyroporn-0.2.3/pyroporn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.2.2
+Version: 0.2.3
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.2.2/pyroporn.egg-info/SOURCES.txt` & `pyroporn-0.2.3/pyroporn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.2/setup.py` & `pyroporn-0.2.3/setup.py`

 * *Files identical despite different names*

