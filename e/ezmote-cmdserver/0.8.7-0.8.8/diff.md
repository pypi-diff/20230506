# Comparing `tmp/ezmote-cmdserver-0.8.7.tar.gz` & `tmp/ezmote-cmdserver-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmote-cmdserver-0.8.7.tar", last modified: Sat May  6 15:38:23 2023, max compression
+gzip compressed data, was "ezmote-cmdserver-0.8.8.tar", last modified: Sat May  6 15:52:57 2023, max compression
```

## Comparing `ezmote-cmdserver-0.8.7.tar` & `ezmote-cmdserver-0.8.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:23.824129 ezmote-cmdserver-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 15:38:23.824129 ezmote-cmdserver-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:23.820129 ezmote-cmdserver-0.8.7/cmdserver/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:23.820129 ezmote-cmdserver-0.8.7/cmdserver/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/pj.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/playingnow.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/tivo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/tivos.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/wake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/commandcontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/debounce.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/infoprovider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/jvc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25365 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/jvccommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/pjcontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/tivocontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)    69607 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:23.824129 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 15:38:23.824129 ezmote-cmdserver-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:52:57.854184 ezmote-cmdserver-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 15:52:57.854184 ezmote-cmdserver-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:52:57.850184 ezmote-cmdserver-0.8.8/cmdserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:52:57.854184 ezmote-cmdserver-0.8.8/cmdserver/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/pj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/playingnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/tivo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/tivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/apis/wake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/commandcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/infoprovider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/jvc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25365 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/jvccommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/pjcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/tivocontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69607 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/cmdserver/zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:52:57.854184 ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 15:52:57.000000 ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-06 15:52:57.000000 ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:52:57.000000 ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 15:52:57.000000 ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:52:57.000000 ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-06 15:52:57.000000 ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 15:52:57.000000 ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 15:52:57.854184 ezmote-cmdserver-0.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-06 15:52:24.000000 ezmote-cmdserver-0.8.8/setup.py
```

### Comparing `ezmote-cmdserver-0.8.7/LICENSE` & `ezmote-cmdserver-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/PKG-INFO` & `ezmote-cmdserver-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmote-cmdserver
-Version: 0.8.7
+Version: 0.8.8
 Summary: A small webapp which can be used for web based home cinema automation
 Home-page: http://github.com/3ll3d00d/cmdserver
 Author: Matt Khan
 Author-email: mattkhan+cmdserver@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ezmote-cmdserver-0.8.7/README.md` & `ezmote-cmdserver-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/apis/command.py` & `ezmote-cmdserver-0.8.8/cmdserver/apis/command.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/apis/info.py` & `ezmote-cmdserver-0.8.8/cmdserver/apis/info.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/apis/pj.py` & `ezmote-cmdserver-0.8.8/cmdserver/apis/pj.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/apis/tivo.py` & `ezmote-cmdserver-0.8.8/cmdserver/apis/tivo.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/apis/tivos.py` & `ezmote-cmdserver-0.8.8/cmdserver/apis/tivos.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/apis/wake.py` & `ezmote-cmdserver-0.8.8/cmdserver/apis/wake.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/commandcontroller.py` & `ezmote-cmdserver-0.8.8/cmdserver/commandcontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/config.py` & `ezmote-cmdserver-0.8.8/cmdserver/config.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/debounce.py` & `ezmote-cmdserver-0.8.8/cmdserver/debounce.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/infoprovider.py` & `ezmote-cmdserver-0.8.8/cmdserver/infoprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 is_default = value.get('defaultPlayingNowId', False)
                 if is_default is True:
                     self.__default_playing_now_id = value['playingNowId']
         self.__by_playing_now_id = {value['playingNowId']: value['title']
                                     for key, value in config.commands.items() if 'playingNowId' in value}
         self.__ms: MediaServer = MediaServer('localhost', config.mcws.get('user', None), config.mcws.get('pass', None))
         # make sure all calls in pymcws have a timeout not just connection checks
-        self.__ms.session.request = functools.partial(self.__ms.session.request, timeout=10)
+        self.__ms.session.request = functools.partial(self.__ms.session.request, timeout=2.5)
         self.__ms_mac: str = config.mcws.get('mac', '')
         self.__ms.port = int(config.mcws.get('port', 52199))
         self.__ms.local_ip_list = config.mcws.get('ip', '127.0.0.1')
         self.__ms.local_ip = self.__ms.local_ip_list
         self.__token = None
         self.__current_state = {}
         self.__refresh_task = task.LoopingCall(self.refresh)
```

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/jvc.py` & `ezmote-cmdserver-0.8.8/cmdserver/jvc.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/jvccommands.py` & `ezmote-cmdserver-0.8.8/cmdserver/jvccommands.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/main.py` & `ezmote-cmdserver-0.8.8/cmdserver/main.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/pjcontroller.py` & `ezmote-cmdserver-0.8.8/cmdserver/pjcontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/tivocontroller.py` & `ezmote-cmdserver-0.8.8/cmdserver/tivocontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/ws.py` & `ezmote-cmdserver-0.8.8/cmdserver/ws.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/cmdserver/zeroconf.py` & `ezmote-cmdserver-0.8.8/cmdserver/zeroconf.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/PKG-INFO` & `ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmote-cmdserver
-Version: 0.8.7
+Version: 0.8.8
 Summary: A small webapp which can be used for web based home cinema automation
 Home-page: http://github.com/3ll3d00d/cmdserver
 Author: Matt Khan
 Author-email: mattkhan+cmdserver@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/SOURCES.txt` & `ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/requires.txt` & `ezmote-cmdserver-0.8.8/ezmote_cmdserver.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.7/setup.py` & `ezmote-cmdserver-0.8.8/setup.py`

 * *Files identical despite different names*

