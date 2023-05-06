# Comparing `tmp/angry-logger-0.1.0.tar.gz` & `tmp/angry_logger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angry-logger-0.1.0.tar", max compression
+gzip compressed data, was "angry_logger-1.0.0.tar", max compression
```

## Comparing `angry-logger-0.1.0.tar` & `angry_logger-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       55 2021-10-13 23:58:58.330765 angry-logger-0.1.0/angry_logger/__init__.py
--rw-r--r--   0        0        0     1502 2021-10-14 00:32:47.429380 angry-logger-0.1.0/angry_logger/_const.py
--rw-r--r--   0        0        0     1806 2021-10-14 00:32:47.455290 angry-logger-0.1.0/angry_logger/logging.py
--rw-r--r--   0        0        0      381 2021-10-13 23:58:48.979337 angry-logger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      563 2021-10-14 00:35:49.961268 angry-logger-0.1.0/setup.py
--rw-r--r--   0        0        0      406 2021-10-14 00:35:49.961458 angry-logger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-05-06 06:29:17.463215 angry_logger-1.0.0/README.md
+-rw-r--r--   0        0        0       50 2023-05-06 06:22:52.569107 angry_logger-1.0.0/angry_logger/__init__.py
+-rw-r--r--   0        0        0     1502 2023-05-06 06:19:33.244907 angry_logger-1.0.0/angry_logger/_const.py
+-rw-r--r--   0        0        0     1796 2023-05-06 06:22:52.576459 angry_logger-1.0.0/angry_logger/logging.py
+-rw-r--r--   0        0        0      551 2023-05-06 06:29:17.463324 angry_logger-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2237 1970-01-01 00:00:00.000000 angry_logger-1.0.0/setup.py
+-rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 angry_logger-1.0.0/PKG-INFO
```

### Comparing `angry-logger-0.1.0/angry_logger/_const.py` & `angry_logger-1.0.0/angry_logger/_const.py`

 * *Files identical despite different names*

### Comparing `angry-logger-0.1.0/angry_logger/logging.py` & `angry_logger-1.0.0/angry_logger/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 import logging as original_logging
 import random
-import re
 from typing import Any
 
 from ._const import *
 
-config = {"potty_mouth": True}
-
-
-def go_to_town(potty_mouth=True):
-    config["potty_mouth"] = potty_mouth
-    my_regular_logger = original_logging.getLogger("regular_logger")
-    my_regular_logger.info("Gosh this is going to be fun.")
-    original_logging.setLoggerClass(_AngryLogger)
-    my_angry_logger = original_logging.getLogger("angry_logger")
-    my_angry_logger.info("You should be all set up now.")
+_config = {"potty_mouth": True}
 
 
 class _AngryLogger(original_logging.Logger):
     @staticmethod
     def clean_up(message: str) -> str:
-        if not config["potty_mouth"]:
+        if not _config["potty_mouth"]:
             for pattern in NAUGHTY_SUBS:
                 message = pattern.sub("*****", message)
         return message
 
     def debug(self, msg: Any, *args: Any, **kwargs: Any) -> None:
         wrapper = random.choice(DEBUG_SUBS)
         wrapper = self.clean_up(wrapper)
@@ -44,7 +34,16 @@
         if random.random() > 0.5:
             first_line = random.choice(ERROR_PRE_LOGS)
             first_line = self.clean_up(first_line)
             super().error(first_line)
         wrapper = random.choice(ERROR_SUBS)
         wrapper = self.clean_up(wrapper)
         super().error(wrapper.format(msg), *args, **kwargs)
+
+
+def start(potty_mouth=True):
+    _config["potty_mouth"] = potty_mouth
+    my_regular_logger = original_logging.getLogger("regular_logger")
+    my_regular_logger.info("Gosh this is going to be fun...")
+    original_logging.setLoggerClass(_AngryLogger)
+    my_angry_logger = original_logging.getLogger("angry_logger")
+    my_angry_logger.info("You should be all set up now.")
```

