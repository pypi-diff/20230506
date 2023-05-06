# Comparing `tmp/operbot-172.tar.gz` & `tmp/operbot-180.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operbot-172.tar", last modified: Tue Apr 25 10:55:22 2023, max compression
+gzip compressed data, was "operbot-180.tar", last modified: Sat May  6 14:52:38 2023, max compression
```

## Comparing `operbot-172.tar` & `operbot-180.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-25 10:55:22.805705 operbot-172/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-04-25 07:12:36.000000 operbot-172/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2846 2023-04-25 07:12:36.000000 operbot-172/bin/operbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)      968 2023-04-25 10:41:31.000000 operbot-172/bin/operbotcmd
--rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-04-25 07:12:36.000000 operbot-172/bin/operbotctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1149 2023-04-25 07:12:36.000000 operbot-172/bin/operbotd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-04-25 07:12:36.000000 operbot-172/files/operbot.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/operbot/
--rw-r--r--   0 bart      (1000) bart      (1001)      147 2023-04-25 08:55:43.000000 operbot-172/operbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2834 2023-04-25 08:58:33.000000 operbot-172/operbot/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-25 07:15:29.000000 operbot-172/operbot/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6077 2023-04-25 07:15:29.000000 operbot-172/operbot/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1965 2023-04-25 07:15:29.000000 operbot-172/operbot/loggers.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/operbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)    17599 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      918 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7792 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1022 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1091 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2657 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/usr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5596 2023-04-25 07:15:29.000000 operbot-172/operbot/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4661 2023-04-25 07:15:29.000000 operbot-172/operbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)      211 2023-04-25 07:19:01.000000 operbot-172/operbot/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-25 07:15:29.000000 operbot-172/operbot/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1916 2023-04-25 07:15:29.000000 operbot-172/operbot/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-25 07:15:29.000000 operbot-172/operbot/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/operbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-25 10:55:22.000000 operbot-172/operbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      817 2023-04-25 10:55:22.000000 operbot-172/operbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-25 10:55:22.000000 operbot-172/operbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-25 10:55:22.000000 operbot-172/operbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-25 10:55:22.805705 operbot-172/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-25 10:42:46.000000 operbot-172/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-25 07:12:36.000000 operbot-172/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-25 07:12:36.000000 operbot-172/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-25 07:12:36.000000 operbot-172/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-04-25 07:12:36.000000 operbot-172/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-04-25 07:12:36.000000 operbot-172/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-05-06 14:52:38.229128 operbot-180/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-05-06 13:50:40.000000 operbot-180/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.225128 operbot-180/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     3306 2023-05-06 13:50:40.000000 operbot-180/bin/operbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1717 2023-05-06 14:51:56.000000 operbot-180/bin/operbotcmd
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-05-06 13:50:40.000000 operbot-180/bin/operbotctl
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2456 2023-05-06 13:50:40.000000 operbot-180/bin/operbotd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.225128 operbot-180/files/
+-rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-05-06 13:50:40.000000 operbot-180/files/operbot.service
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/operbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)      801 2023-05-06 13:50:40.000000 operbot-180/operbot/classes.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      621 2023-05-06 13:50:40.000000 operbot-180/operbot/clients.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1168 2023-05-06 13:50:40.000000 operbot-180/operbot/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1072 2023-05-06 13:50:40.000000 operbot-180/operbot/command.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      763 2023-05-06 13:50:40.000000 operbot-180/operbot/decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      529 2023-05-06 13:50:40.000000 operbot-180/operbot/default.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1153 2023-05-06 13:50:40.000000 operbot-180/operbot/encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      581 2023-05-06 13:50:40.000000 operbot-180/operbot/errored.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1843 2023-05-06 13:50:40.000000 operbot-180/operbot/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      983 2023-05-06 13:50:40.000000 operbot-180/operbot/listens.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2010 2023-05-06 13:50:40.000000 operbot-180/operbot/loggers.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2304 2023-05-06 13:50:40.000000 operbot-180/operbot/message.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/operbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      309 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      456 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      553 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    20619 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      810 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7968 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      392 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1012 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1146 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      371 2023-05-06 13:50:40.000000 operbot-180/operbot/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3565 2023-05-06 13:50:40.000000 operbot-180/operbot/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4364 2023-05-06 13:50:40.000000 operbot-180/operbot/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      386 2023-05-06 13:50:40.000000 operbot-180/operbot/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      460 2023-05-06 13:50:40.000000 operbot-180/operbot/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2191 2023-05-06 13:50:40.000000 operbot-180/operbot/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      296 2023-05-06 13:50:40.000000 operbot-180/operbot/skipper.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1961 2023-05-06 13:50:40.000000 operbot-180/operbot/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1251 2023-05-06 13:50:40.000000 operbot-180/operbot/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/operbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-05-06 14:52:38.000000 operbot-180/operbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      935 2023-05-06 14:52:38.000000 operbot-180/operbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-05-06 14:52:38.000000 operbot-180/operbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-05-06 14:52:38.000000 operbot-180/operbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-05-06 14:52:38.229128 operbot-180/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-05-06 13:50:40.000000 operbot-180/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-06 14:52:38.229128 operbot-180/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      715 2023-05-06 14:21:03.000000 operbot-180/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      382 2023-05-06 14:51:12.000000 operbot-180/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-05-06 13:50:40.000000 operbot-180/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-05-06 13:50:40.000000 operbot-180/test/test_objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-05-06 13:50:40.000000 operbot-180/test/test_storage.py
```

### Comparing `operbot-172/PKG-INFO` & `operbot-180/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 172
+Version: 180
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `operbot-172/README.rst` & `operbot-180/README.rst`

 * *Files identical despite different names*

### Comparing `operbot-172/operbot/clocked.py` & `operbot-180/operbot/utility.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,25 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
-'clocked'
-
-
-import threading
-import time
-
-
-from .objects import Object
-from .threads import launch
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 def __dir__():
     return (
-            'Repeater',
-            'Timer',
-            'elapsed'
+            'elapsed',
+            'spl'
            )
 
 
 __all__ = __dir__()
 
 
-class Timer:
-
-    def __init__(self, sleep, func, *args, thrname=None):
-        super().__init__()
-        self.args = args
-        self.func = func
-        self.sleep = sleep
-        self.name = thrname or str(self.func).split()[2]
-        self.state = Object
-        self.timer = None
-
-    def run(self):
-        self.state.latest = time.time()
-        launch(self.func, *self.args)
-
-    def start(self):
-        timer = threading.Timer(self.sleep, self.run)
-        timer.name = self.name
-        timer.daemon = True
-        timer.sleep = self.sleep
-        timer.state = self.state
-        timer.state.starttime = time.time()
-        timer.state.latest = time.time()
-        timer.func = self.func
-        timer.start()
-        self.timer = timer
-        return timer
-
-    def stop(self):
-        if self.timer:
-            self.timer.cancel()
-
-
-class Repeater(Timer):
-
-    def run(self):
-        thr = launch(self.start)
-        super().run()
-        return thr
-
-
 def elapsed(seconds, short=True):
     txt = ""
     nsec = float(seconds)
     if nsec < 1:
         return f"{nsec:.2f}s"
     year = 365*24*60*60
     week = 7*24*60*60
@@ -98,7 +49,15 @@
         txt += "%sh" % hours
     if minutes:
         txt += "%sm" % minutes
     if sec:
         txt += "%ss" % sec
     txt = txt.strip()
     return txt
+
+
+def spl(txt):
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
```

### Comparing `operbot-172/operbot/loggers.py` & `operbot-180/operbot/loggers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0903,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
-"logging"
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import logging
 import logging.handlers
 import os
 
 
-from .handler import spl
 from .persist import Persist, cdir, touch
 from .runtime import Cfg
+from .utility import spl
 
 
 LEVELS = {'debug': logging.DEBUG,
           'info': logging.INFO,
           'warning': logging.WARNING,
           'warn': logging.WARNING,
           'error': logging.ERROR,
```

### Comparing `operbot-172/operbot/modules/irc.py` & `operbot-180/operbot/modules/irc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,90 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0902,R0903,W0613,E1101,R0912,R0904,R0915
-# pylint: disable=E0402,E0401
+# pylint: disable=C,I,R,W,E0402,E1101
 
 
-'internet relay chat'
+"""internet relay chat
+
+IRC
+
+::
+
+ $ operbot cfg server=<server> channel=<channel> nick=<nick>
+
+ (*) default channel/server is #opb on localhost
+
+
+SASL
+
+::
+
+ $ operbot pwd <nickservnick> <nickservpass>
+ $ operbot cfg password=<outputfrompwd>
+
+
+USERS
+
+as default the user's userhost is not checked when a user types a command in a
+channel. To enable userhost checking enable users with the ``cfg`` command::
+
+ $ operbot cfg users=True
+
+
+To add a user to the bot use the met command::
+
+ $ operbot  met <userhost>
+
+to delete a user use the del command with a substring of the userhost::
+
+ $ operbot del <substring>
+
+"""
+
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
+
 
 
 import base64
 import os
 import queue
 import random
 import socket
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from ..handler import Client, Command, Error, Event, Listens
-from ..loggers import Logging
-from ..objects import Default, Object, edit, keys, prt
-from ..persist import Class, last, write
-from ..runtime import Cfg
-from ..threads import launch
-
-
-from .usr import Users
+from operbot.classes import Classes
+from operbot.clients import Client
+from operbot.command import Command
+from operbot.default import Default
+from operbot.errored import Errors
+from operbot.message import Message
+from operbot.listens import Listens
+from operbot.loggers import Logging
+from operbot.objects import Object, copy, edit, keys, prt, update
+from operbot.persist import find, fntime, last, write
+from operbot.runtime import Cfg
+from operbot.threads import launch
+from operbot.utility import elapsed
 
 
 def __dir__():
     return (
             'Config',
             'IRC',
+            'NoUser',
+            'Users',
+            'User',
             'cfg',
+            'dlt',
+            'met'
             'mre',
             'pwd',
             'start'
            )
 
 
 saylock = _thread.allocate_lock()
@@ -83,15 +130,15 @@
         self.server = Config.server
         self.servermodes = Config.servermodes
         self.sleep = Config.sleep
         self.username = Config.username
         self.users = Config.users
 
 
-Class.add(Config)
+Classes.add(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
     def __init__(self):
         super().__init__()
         self.break_long_words = False
@@ -278,15 +325,15 @@
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
                ) as ex:
-            Error.errors.append(ex)
+            Errors.errors.append(ex)
 
     def docommand(self, evt):
         evt.orig = repr(self)
         Command.handle(evt)
 
     def doconnect(self, server, nck, port=6667):
         while 1:
@@ -307,15 +354,15 @@
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.command('PRIVMSG', channel, txt)
 
     def error(self, event):
         self.state.nrerror += 1
         self.state.errors.append(event.txt)
-        self.stop()
+        #self.stop()
 
     def event(self, txt):
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.command('PONG', evt.txt or '')
@@ -394,15 +441,15 @@
             )
             self.command('NOTICE', event.channel, txt)
 
     def parsing(self, txt):
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
-        obj = Event()
+        obj = Message()
         obj.rawstr = rawstr
         obj.command = ''
         obj.arguments = []
         arguments = rawstr.split()
         if arguments:
             obj.origin = arguments[0]
         else:
@@ -463,30 +510,31 @@
             except (
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Error.errors.append(ex)
-                self.stop()
+                Errors.errors.append(ex)
+                #self.stop()
                 return self.event(str(ex))
         return self.event(self.buffer.pop(0))
 
     def privmsg(self, event):
         if event.txt:
             if event.txt[0] in [self.cfg.control, '!']:
                 event.txt = event.txt[1:]
             elif event.txt.startswith('%s:' % self.cfg.nick):
                 event.txt = event.txt[len(self.cfg.nick)+1:]
             else:
                 return
             if self.cfg.users and not Users.allowed(event.origin, 'USER'):
                 return
-            msg = Event(event)
+            msg = Message()
+            copy(msg, event)
             msg.type = 'command'
             msg.parse(event.txt)
             self.handle(msg)
 
     def quit(self, event):
         if event.orig and event.orig in self.zelf:
             self.stop()
@@ -504,15 +552,15 @@
                 self.sock.send(txt)
             except (
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Error.errors.append(ex)
+                Errors.errors.append(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
         try:
@@ -561,14 +609,79 @@
         Logging.debug("stopping")
         Listens.remove(self)
         Client.stop(self)
         Output.stop(self)
         self.disconnect()
 
 
+class NoUser(Exception):
+
+    pass
+
+
+class Users(Object):
+
+    @staticmethod
+    def allowed(origin, perm):
+        perm = perm.upper()
+        user = Users.get_user(origin)
+        val = False
+        if user and perm in user.perms:
+            val = True
+        return val
+
+    @staticmethod
+    def delete(origin, perm):
+        res = False
+        for user in Users.get_users(origin):
+            try:
+                user.perms.remove(perm)
+                write(user)
+                res = True
+            except ValueError:
+                pass
+        return res
+
+    @staticmethod
+    def get_users(origin=''):
+        selector = {'user': origin}
+        return find('user', selector)
+
+    @staticmethod
+    def get_user(origin):
+        users = list(Users.get_users(origin))
+        res = None
+        if len(users) > 0:
+            res = users[-1]
+        return res
+
+    @staticmethod
+    def perm(origin, permission):
+        user = Users.get_user(origin)
+        if not user:
+            raise NoUser(origin)
+        if permission.upper() not in user.perms:
+            user.perms.append(permission.upper())
+            write(user)
+        return user
+
+
+class User(Object):
+
+    def __init__(self, val=None):
+        Object.__init__(self)
+        self.user = ''
+        self.perms = []
+        if val:
+            update(self, val)
+
+
+Classes.add(User)
+
+
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
         event.reply(prt(
                         config,
                         keys(config),
@@ -576,14 +689,42 @@
                        )
     else:
         edit(config, event.sets)
         write(config)
         event.reply('ok')
 
 
+def dlt(event):
+    if not event.args:
+        event.reply('dlt <username>')
+        return
+    selector = {'user': event.args[0]}
+    for obj in find('user', selector):
+        obj.__deleted__ = True
+        write(obj)
+        event.reply('ok')
+        break
+
+
+def met(event):
+    if not event.args:
+        nmr = 0
+        for obj in find('user'):
+            lap = elapsed(time.time() - fntime(obj.__fnm__))
+            event.reply(f'{nmr} {obj.user} {obj.perms} {lap}s')
+            nmr += 1
+        if not nmr:
+            event.reply('no user')
+        return
+    user = User()
+    user.user = event.rest
+    user.perms = ['USER']
+    write(user)
+    event.reply('ok')
+
 def mre(event):
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = event.bot()
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
```

### Comparing `operbot-172/operbot/modules/log.py` & `operbot-180/operbot/modules/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0903,E0402
-
-
-'log'
+# pylint: disable=C,I,R,W,E0402
 
 
 import time
 
 
-from ..clocked import elapsed
-from ..persist import Class, find, fntime, write
-from ..objects import Object
+from operbot.classes import Classes
+from operbot.persist import find, fntime, write
+from operbot.objects import Object
+from operbot.utility import elapsed
 
 
 def __dir__():
     return (
             'Log',
             'log',
            )
@@ -23,26 +21,23 @@
 class Log(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
-Class.add(Log)
+Classes.add(Log)
 
 
 def log(event):
     if not event.rest:
         nmr = 0
         for obj in find('log'):
-            event.reply('%s %s %s' % (
-                                      nmr,
-                                      obj.txt,
-                                      elapsed(time.time() - fntime(obj.__oid__)))
-                                     )
+            lap = elapsed(time.time() - fntime(obj.__oid__))
+            event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
     write(obj)
```

### Comparing `operbot-172/operbot/modules/rss.py` & `operbot-180/operbot/modules/rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0903,E1101,E0402
+# pylint: disable=C,I,R,W,E0402,E1101
 
 
-'rich site syndicate'
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import html.parser
 import re
 import threading
 import time
 import urllib
@@ -14,21 +15,22 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from ..clocked import Repeater, elapsed
-from ..handler import Listens, spl
-from ..objects import Object, prt, update
-from ..persist import Class, find, fntime, last, write
-from ..runtime import Cfg
-from ..threads import launch, threaded
-
+from operbot.classes import Classes
+from operbot.listens import Listens
+from operbot.objects import Object, prt, update
+from operbot.persist import find, fntime, last, write
+from operbot.repeats import Repeater
+from operbot.runtime import Cfg
+from operbot.threads import launch, threaded
+from operbot.utility import elapsed, spl
 
 def __dir__():
     return (
         'Feed',
         'Fetcher',
         'Repeater',
         'Rss',
@@ -63,25 +65,25 @@
     def __init__(self):
         super().__init__()
         self.display_list = 'title,link,author'
         self.name = ''
         self.rss = ''
 
 
-Class.add(Rss)
+Classes.add(Rss)
 
 
 class Seen(Object):
 
     def __init__(self):
         super().__init__()
         self.urls = []
 
 
-Class.add(Seen)
+Classes.add(Seen)
 
 
 class Fetcher(Object):
 
     dosave = False
     seen = Seen()
 
@@ -209,29 +211,30 @@
         ('submit', 'submit'),
         ('url', url),
     ]
     postdata = urlencode(postarray, quote_via=quote_plus)
     req = Request('http://tinyurl.com/create.php',
                   data=bytes(postdata, 'UTF-8'))
     req.add_header('User-agent', useragent(url))
-    for txt in urlopen(req).readlines():
-        line = txt.decode('UTF-8').strip()
-        i = re.search('data-clipboard-text="(.*?)"', line, re.M)
-        if i:
-            return i.groups()
+    with urlopen(req) as htm:
+        for txt in htm.readlines():
+            line = txt.decode('UTF-8').strip()
+            i = re.search('data-clipboard-text="(.*?)"', line, re.M)
+            if i:
+                return i.groups()
     return []
 
 
 def geturl(url):
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
-    req.add_header('User-agent', useragent('OPERBOT - operator bot'))
-    response = urllib.request.urlopen(req)
-    response.data = response.read()
-    return response
+    req.add_header('User-agent', useragent(Cfg.name.upper()))
+    with urllib.request.urlopen(req) as response:
+        response.data = response.read()
+        return response
 
 
 def striphtml(text):
     clean = re.compile('<.*?>')
     return re.sub(clean, '', text)
```

### Comparing `operbot-172/operbot/modules/thr.py` & `operbot-180/operbot/modules/thr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0114,C0115,C0116,E1101,E0402
+# pylint: disable=C,I,R,W,E0402,E1101
 
 
-"list running threads."
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import threading
 import time
 
 
-from ..clocked import elapsed
-from ..objects import Object, update
+from operbot.objects import Object, update
+from operbot.utility import elapsed
 
 
 def __dir__():
     return (
             'thr',
            )
 
@@ -37,12 +38,13 @@
         elif getattr(obj, 'starttime', None):
             uptime = int(time.time() - obj.starttime)
         else:
             uptime = int(time.time() - starttime)
         result.append((uptime, thread.name))
     res = []
     for uptime, txt in sorted(result, key=lambda x: x[0]):
-        res.append('%s/%s' % (txt, elapsed(uptime)))
+        lap = elapsed(uptime)
+        res.append(f'{txt}/{lap}')
     if res:
         event.reply(' '.join(res))
     else:
         event.reply('no threads')
```

### Comparing `operbot-172/operbot/objects.py` & `operbot-180/operbot/objects.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,65 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0112,C0115,C0116,R0903,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
-"a clean namespace"
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import datetime
-import json
 import os
 import uuid
-import _thread
-
-
-from json import JSONDecoder, JSONEncoder
 
 
 def __dir__():
     return (
-            'Default',
             'Object',
-            'dumps',
             'edit',
             'items',
             'keys',
             'kind',
-            'loads',
             'prt',
             'search',
             'update',
             'values',
            )
 
 
 __all__ = __dir__()
 
 
-lock = _thread.allocate_lock()
-
-
 class Object:
 
     __slots__ = ('__dict__', '__oid__')
 
     def __init__(self, *args, **kwargs):
         self.__oid__ = ident(self)
-        if args:
-            val = args[0]
-            if isinstance(val, list):
-                update(self, dict(val))
-            elif isinstance(val, zip):
-                update(self, dict(val))
-            elif isinstance(val, dict):
-                update(self, val)
-            elif isinstance(val, Object):
-                update(self, vars(val))
-        if kwargs:
-            self.__dict__.update(kwargs)
 
     def __iter__(self):
         return iter(self.__dict__)
 
     def __len__(self):
         return len(self.__dict__)
 
     def __str__(self):
         return str(self.__dict__)
 
 
+def copy(obj, val):
+    if isinstance(val, list):
+        update(obj, dict(val))
+    elif isinstance(val, zip):
+        update(obj, dict(val))
+    elif isinstance(val, dict):
+        update(obj, val)
+    elif isinstance(val, Object):
+        update(obj, vars(val))
+
+
 def edit(obj, setter, skip=False):
     try:
         setter = vars(setter)
     except (TypeError, ValueError):
         pass
     if not setter:
         setter = {}
@@ -98,15 +87,15 @@
     return count
 
 
 def ident(obj):
     return os.path.join(
                         kind(obj),
                         str(uuid.uuid4().hex),
-                        os.sep.join(str(datetime.datetime.now()).split()),
+                        os.sep.join(str(datetime.datetime.now()).split())
                        )
 
 
 def items(obj) -> []:
     if isinstance(obj, type({})):
         return obj.items()
     return obj.__dict__.items()
@@ -172,81 +161,7 @@
 def update(obj, data) -> None:
     for key, value in items(data):
         setattr(obj, key, value)
 
 
 def values(obj) -> []:
     return obj.__dict__.values()
-
-
-class Default(Object):
-
-    __slots__ = ("__default__",)
-
-    def __init__(self, *args, **kwargs):
-        Object.__init__(self, *args, **kwargs)
-        self.__default__ = ""
-
-    def __getattr__(self, key):
-        return self.__dict__.get(key, self.__default__)
-
-
-class ObjectDecoder(JSONDecoder):
-
-    errors = []
-
-    def __init__(self):
-        ""
-        JSONDecoder.__init__(self)
-
-    def decode(self, s, _w=None) -> Object:
-        ""
-        val = JSONDecoder.decode(self, s)
-        if not val:
-            val = {}
-        return Object(val)
-
-    def raw_decode(self, s, idx=0) -> (int, Object):
-        ""
-        return JSONDecoder.raw_decode(self, s, idx)
-
-
-def loads(string, *args, **kw) -> Object:
-    return json.loads(string, *args, cls=ObjectDecoder, **kw)
-
-
-class ObjectEncoder(JSONEncoder):
-
-    def __init__(self, *args, **kw):
-        ""
-        JSONEncoder.__init__(self, *args, **kw)
-
-    def default(self, o) -> str:
-        ""
-        if isinstance(o, dict):
-            return o.items()
-        if isinstance(o, Object):
-            return vars(o)
-        if isinstance(o, list):
-            return iter(o)
-        if isinstance(o,
-                      (type(str), type(True), type(False),
-                       type(int), type(float))
-                     ):
-            return str(o)
-        try:
-            return JSONEncoder.default(self, o)
-        except TypeError:
-            return str(o)
-
-    def encode(self, o) -> str:
-        ""
-        return JSONEncoder.encode(self, o)
-
-    def iterencode(self, o, _one_shot=False) -> str:
-        ""
-        return JSONEncoder.iterencode(self, o, _one_shot)
-
-
-def dumps(*args, **kw) -> str:
-    kw["cls"] = ObjectEncoder
-    return json.dumps(*args, **kw)
```

### Comparing `operbot-172/operbot/persist.py` & `operbot-180/operbot/persist.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Tihs file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0903,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
-"persistence"
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import json
 import os
 import pathlib
 import time
 import _thread
 
 
-from .objects import Default, Object, ObjectDecoder, ObjectEncoder
-from .objects import kind, search, update
+from .classes import Classes
+from .decoder import ObjectDecoder
+from .encoder import ObjectEncoder
+from .errored import NoClassError
+from .objects import Object, kind, search, update
+from .runtime import Cfg
 
 
 def __dir__():
     return (
             'Persist',
             'cdir',
             'last',
@@ -30,51 +35,26 @@
 
 __all__ = __dir__()
 
 
 disklock = _thread.allocate_lock()
 
 
-class NoClassError(Exception):
-
-    "class is not registered"
-
-
-class Class:
-
-    cls = Default()
-
-    @staticmethod
-    def add(clz):
-        setattr(Class.cls, "%s.%s" % (clz.__module__, clz.__name__), clz)
-
-    @staticmethod
-    def get(cmd):
-        return getattr(Class.cls, cmd, None)
-
-    @staticmethod
-    def match(mtc):
-        mtc = mtc.lower()
-        for clz in Class.cls:
-            if mtc == clz.split(".")[-1].lower():
-                yield clz
-
-    @staticmethod
-    def remove(cmd):
-        del Class.cls[cmd]
-
-
 class Persist(Object):
 
-    workdir = ""
+    workdir = Cfg.wd
 
     @staticmethod
     def logdir():
         return os.path.join(Persist.workdir, "logs")
 
+    @staticmethod
+    def storedir():
+        return os.path.join(Persist.workdir, "store")
+
 
 def cdir(pth) -> None:
     if not pth.endswith(os.sep):
         pth = os.path.dirname(pth)
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
 
@@ -84,41 +64,105 @@
     return json.dump(*args, **kw)
 
 
 def files() -> []:
     return os.listdir(os.path.join(Persist.workdir, "store"))
 
 
+def find(mtc, selector=None) -> []:
+    if selector is None:
+        selector = {}
+    for fnm in fns(mtc):
+        obj = hook(fnm)
+        if '__deleted__' in obj:
+            continue
+        if selector and not search(obj, selector):
+            continue
+        yield obj
+
+
+def fnclass(pth):
+    try:
+        *_rest, mpth = pth.split("store")
+        splitted = mpth.split(os.sep)
+        return splitted[0]
+    except ValueError:
+        pass
+    return None
+
+
 def fns(mtc) -> []:
     assert Persist.workdir
     dname = ''
     lst = mtc.lower().split(".")[-1]
     for rootdir, dirs, _files in os.walk(Persist.workdir, topdown=False):
         if dirs:
             dname = sorted(dirs)[-1]
             if dname.count('-') == 2:
                 ddd = os.path.join(rootdir, dname)
                 fls = sorted(os.listdir(ddd))
                 if fls:
                     path2 = os.path.join(ddd, fls[-1])
-                    spl = strip(path2).split(os.sep)[0]
+                    spl = strip(path2).split(os.sep, maxsplit=1)[0]
                     if lst in spl.lower().split(".")[-1]:
                         yield strip(path2)
 
 
+def fntime(daystr):
+    daystr = daystr.replace('_', ':')
+    datestr = ' '.join(daystr.split(os.sep)[-2:])
+    if '.' in datestr:
+        datestr, rest = datestr.rsplit('.', 1)
+    else:
+        rest = ''
+    tme = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
+    if rest:
+        tme += float('.' + rest)
+    else:
+        tme = 0
+    return tme
+
+
 def hook(otp) -> Object:
     clz = fnclass(otp)
-    cls = Class.get(clz)
+    cls = Classes.get(clz)
     if cls:
         obj = cls()
         read(obj, otp)
         return obj
     raise NoClassError(clz)
 
 
+def last(obj, selector=None) -> None:
+    if selector is None:
+        selector = {}
+    result = sorted(
+                    find(kind(obj), selector),
+                    key=lambda x: fntime(x.__oid__)
+                   )
+    if result:
+        inp = result[-1]
+        update(obj, inp)
+        obj.__oid__ = inp.__oid__
+    return obj.__oid__
+
+
+def match(mtc, selector=None) -> []:
+    if selector is None:
+        selector = {}
+    for tpe in Classes.match(mtc):
+        for fnm in fns(tpe):
+            obj = hook(fnm)
+            if '__deleted__' in obj:
+                continue
+            if selector and not search(obj, selector):
+                continue
+            yield obj
+
+
 def load(fpt, *args, **kw) -> Object:
     return json.load(fpt, *args, cls=ObjectDecoder, **kw)
 
 
 def path(pth) -> str:
     return os.path.join(Persist.workdir, 'store', pth)
 
@@ -149,72 +193,7 @@
 def write(obj) -> str:
     pth = path(obj.__oid__)
     cdir(pth)
     with disklock:
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile)
     return strip(pth)
-
-
-def find(mtc, selector=None) -> []:
-    if selector is None:
-        selector = {}
-    for fnm in fns(mtc):
-        obj = hook(fnm)
-        if '__deleted__' in obj:
-            continue
-        if selector and not search(obj, selector):
-            continue
-        yield obj
-
-
-def last(obj, selector=None) -> None:
-    if selector is None:
-        selector = {}
-    result = sorted(
-                    find(kind(obj), selector),
-                    key=lambda x: fntime(x.__oid__)
-                   )
-    if result:
-        inp = result[-1]
-        update(obj, inp)
-        obj.__oid__ = inp.__oid__
-    return obj.__oid__
-
-
-def match(mtc, selector=None) -> []:
-    if selector is None:
-        selector = {}
-    for tpe in Class.match(mtc):
-        print(tpe)
-        for fnm in fns(tpe):
-            obj = hook(fnm)
-            if '__deleted__' in obj:
-                continue
-            if selector and not search(obj, selector):
-                continue
-            yield obj
-
-
-def fnclass(pth):
-    try:
-        *_rest, mpth = pth.split("store")
-        splitted = mpth.split(os.sep)
-        return splitted[0]
-    except ValueError:
-        pass
-    return None
-
-
-def fntime(daystr):
-    daystr = daystr.replace('_', ':')
-    datestr = ' '.join(daystr.split(os.sep)[-2:])
-    if '.' in datestr:
-        datestr, rest = datestr.rsplit('.', 1)
-    else:
-        rest = ''
-    tme = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
-    if rest:
-        tme += float('.' + rest)
-    else:
-        tme = 0
-    return tme
```

### Comparing `operbot-172/operbot/scanner.py` & `operbot-180/operbot/scanner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0116,E0401,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
-"introspection"
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import importlib
 import importlib.util
 import inspect
 import os
 
 
-from .handler import Command, spl
+from .command import Command
+from .threads import launch
+from .utility import spl
 
 
 def __dir__():
     return (
             'importer',
             'initer',
             'scan',
@@ -49,14 +52,21 @@
 def starter(mname, path=None):
     mod = doimport(mname, path)
     if "start" in dir(mod):
         mod.start()
     return mod
 
 
+def threader(mname, path=None):
+    mod = doimport(mname, path)
+    if "start" in dir(mod):
+        mod._thr = launch(mod.start)
+    return mod
+
+
 def listmods(path):
     return sorted([x[:-3] for x in os.listdir(path) if not x.startswith("__")])
 
 
 def scan(mod):
     for key, cmd in inspect.getmembers(mod, inspect.isfunction):
         if key.startswith("cb"):
@@ -81,11 +91,12 @@
     if not os.path.exists(pth):
         return res
     for fnm in os.listdir(pth):
         if fnm.endswith("~") or fnm.startswith("__"):
             continue
         if not doall and not include(fnm, mods):
             continue
-        mname = "%s.%s" % (pname, fnm.split(os.sep)[-1][:-3])
+        mnm = fnm.split(os.sep)[-1][:-3]
+        mname = f"{pname}.{mnm}"
         path2 = os.path.join(pth, fnm)
         res.append(func(mname, path2))
     return res
```

### Comparing `operbot-172/operbot/threads.py` & `operbot-180/operbot/threads.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,W0613,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
-'threads'
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import queue
 import time
 import types
```

### Comparing `operbot-172/operbot.egg-info/PKG-INFO` & `operbot-180/operbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 172
+Version: 180
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `operbot-172/setup.py` & `operbot-180/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 continue
             upl.append(d)
     return upl
 
 
 setup(
     name="operbot",
-    version="172",
+    version="180",
     author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/operbot",
     description="operator bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
```

### Comparing `operbot-172/test/test_decoder.py` & `operbot-180/test/test_decoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 "decoder tests"
 
 
 import unittest
 
 
-from operbot.objects import Object, dumps, loads
+from operbot.objects import Object
+from operbot.decoder import loads
+from operbot.encoder import dumps
 
 
 class TestDecoder(unittest.TestCase):
 
     def test_loads(self):
         obj = Object()
         obj.test = "bla"
```

### Comparing `operbot-172/test/test_inherit.py` & `operbot-180/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `operbot-172/test/test_objects.py` & `operbot-180/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `operbot-172/test/test_storage.py` & `operbot-180/test/test_storage.py`

 * *Files identical despite different names*

