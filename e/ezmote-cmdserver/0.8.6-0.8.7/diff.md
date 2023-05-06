# Comparing `tmp/ezmote-cmdserver-0.8.6.tar.gz` & `tmp/ezmote-cmdserver-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmote-cmdserver-0.8.6.tar", last modified: Sat May  6 08:38:45 2023, max compression
+gzip compressed data, was "ezmote-cmdserver-0.8.7.tar", last modified: Sat May  6 15:38:23 2023, max compression
```

## Comparing `ezmote-cmdserver-0.8.6.tar` & `ezmote-cmdserver-0.8.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:38:45.956577 ezmote-cmdserver-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 08:38:45.956577 ezmote-cmdserver-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:38:45.956577 ezmote-cmdserver-0.8.6/cmdserver/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 08:38:08.000000 ezmote-cmdserver-0.8.6/cmdserver/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:38:45.956577 ezmote-cmdserver-0.8.6/cmdserver/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/pj.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/playingnow.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/tivo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/tivos.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/apis/wake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/commandcontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/debounce.py
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/infoprovider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/jvc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25365 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/jvccommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/pjcontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/tivocontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)    69607 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/cmdserver/zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:38:45.956577 ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 08:38:45.000000 ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-06 08:38:45.000000 ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:38:45.000000 ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 08:38:45.000000 ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:38:45.000000 ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-06 08:38:45.000000 ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 08:38:45.000000 ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:38:45.956577 ezmote-cmdserver-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-06 08:38:07.000000 ezmote-cmdserver-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:23.824129 ezmote-cmdserver-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 15:38:23.824129 ezmote-cmdserver-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:23.820129 ezmote-cmdserver-0.8.7/cmdserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:23.820129 ezmote-cmdserver-0.8.7/cmdserver/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/pj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/playingnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/tivo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/tivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/apis/wake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/commandcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/infoprovider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/jvc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25365 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/jvccommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/pjcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/tivocontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69607 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/cmdserver/zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:38:23.824129 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 15:38:23.000000 ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 15:38:23.824129 ezmote-cmdserver-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-06 15:37:48.000000 ezmote-cmdserver-0.8.7/setup.py
```

### Comparing `ezmote-cmdserver-0.8.6/LICENSE` & `ezmote-cmdserver-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/PKG-INFO` & `ezmote-cmdserver-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmote-cmdserver
-Version: 0.8.6
+Version: 0.8.7
 Summary: A small webapp which can be used for web based home cinema automation
 Home-page: http://github.com/3ll3d00d/cmdserver
 Author: Matt Khan
 Author-email: mattkhan+cmdserver@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ezmote-cmdserver-0.8.6/README.md` & `ezmote-cmdserver-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/apis/command.py` & `ezmote-cmdserver-0.8.7/cmdserver/apis/command.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/apis/info.py` & `ezmote-cmdserver-0.8.7/cmdserver/apis/info.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/apis/pj.py` & `ezmote-cmdserver-0.8.7/cmdserver/apis/pj.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/apis/tivo.py` & `ezmote-cmdserver-0.8.7/cmdserver/apis/tivo.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/apis/tivos.py` & `ezmote-cmdserver-0.8.7/cmdserver/apis/tivos.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/apis/wake.py` & `ezmote-cmdserver-0.8.7/cmdserver/apis/wake.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/commandcontroller.py` & `ezmote-cmdserver-0.8.7/cmdserver/commandcontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/config.py` & `ezmote-cmdserver-0.8.7/cmdserver/config.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/debounce.py` & `ezmote-cmdserver-0.8.7/cmdserver/debounce.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/infoprovider.py` & `ezmote-cmdserver-0.8.7/cmdserver/infoprovider.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 is_default = value.get('defaultPlayingNowId', False)
                 if is_default is True:
                     self.__default_playing_now_id = value['playingNowId']
         self.__by_playing_now_id = {value['playingNowId']: value['title']
                                     for key, value in config.commands.items() if 'playingNowId' in value}
         self.__ms: MediaServer = MediaServer('localhost', config.mcws.get('user', None), config.mcws.get('pass', None))
         # make sure all calls in pymcws have a timeout not just connection checks
-        self.__ms.session.request = functools.partial(self.__ms.session.request, timeout=2)
+        self.__ms.session.request = functools.partial(self.__ms.session.request, timeout=10)
         self.__ms_mac: str = config.mcws.get('mac', '')
         self.__ms.port = int(config.mcws.get('port', 52199))
         self.__ms.local_ip_list = config.mcws.get('ip', '127.0.0.1')
         self.__ms.local_ip = self.__ms.local_ip_list
         self.__token = None
         self.__current_state = {}
         self.__refresh_task = task.LoopingCall(self.refresh)
@@ -60,27 +60,82 @@
             content = transform_unstructured_response(response)
             self.__token = content['Token']
         return self.__token
 
     def refresh(self) -> Deferred:
         return threads.deferToThread(self.__async_refresh)
 
+    def __extract_video_layout(self, file_key: Optional[str]) -> Optional[str]:
+        if file_key:
+            # default (no options set)
+            #        (1:1)(11:AspectRatio)(30:(1:4)(1:0)(1:0)(1:0)(1:1)(1:0))
+            # 1.6    (1:1)(11:AspectRatio)(35:(1:4)(1:0)(1:0)(6:196613)(1:1)(1:0))
+            # 1.78   (1:1)(11:AspectRatio)(35:(1:4)(1:0)(1:0)(6:589840)(1:1)(1:0))
+            # 1.85   (1:1)(11:AspectRatio)(36:(1:4)(1:0)(1:0)(7:1310757)(1:1)(1:0))
+            # 2.35   (1:1)(11:AspectRatio)(36:(1:4)(1:0)(1:0)(7:1310767)(1:1)(1:0))
+            # 2.40   (1:1)(11:AspectRatio)(35:(1:4)(1:0)(1:0)(6:327692)(1:1)(1:0))
+            # options are stored in this section : (1:0)(1:0)(6:327692)(1:1)(1:0)
+            #  * 0 = preserve AR, 1 = stretch, 2 = crop
+            #  * AR override
+            #  * 0 = none, 196613 = 1.66, 589840 = 1.78, 1310757 = 1.85, 1310767 = 2.35, 327692 = 2.4
+            #  * 1 = crop edges to sides of screen, 0 = off
+            #  * 1 = crop edges, 0 = off
+            resp = self.__ms.send_request('Files/GetInfo', {'Action': 'json', 'Keys': file_key, 'Fields': 'Playback Info'})
+            resp.raise_for_status()
+            results = resp.json()
+            if results:
+                playback_info = results[0].get('Playback Info')
+                if playback_info:
+                    ar_text = '(11:AspectRatio)'
+                    try:
+                        video_layout = playback_info[playback_info.index(ar_text) + len(ar_text):]
+                        import re
+                        tokens: List[str] = [x for x in re.split(r'[()]', video_layout) if x]
+                        if len(tokens) >= 7 and tokens[1] == '1:4':
+                            if tokens[4] == '1:0':
+                                return None
+                            elif tokens[4] == '6:196613':
+                                return '1.6'
+                            elif tokens[4] == '6:589840':
+                                return '1.78'
+                            elif tokens[4] == '7:1310757':
+                                return '1.85'
+                            elif tokens[4] == '7:1310767':
+                                return '2.35'
+                            elif tokens[4] == '6:327692':
+                                return '2.40'
+                    except:
+                        logger.info(f'Unable to parse file_key {file_key}, playback info is {playback_info}')
+                        pass
+        return None
+
     def __async_refresh(self):
         try:
             zones, active_zone = get_zones(self.__ms)
             playback_info = pymcws.playback.info(self.__ms, active_zone)
+            zones_data = {}
+            for z in zones:
+                if z == active_zone:
+                    zd, pn = self.__zone_to_dict(z, playback_info)
+                    vl = ''
+                    if pn and pn.get('status', None) != 'Stopped':
+                        vl = self.__extract_video_layout(pn.get('fileKey', None))
+                    pn['videoLayout'] = vl
+                else:
+                    zd = self.__zone_to_dict(z, None)
+                zones_data[z.id] = zd
             self.__current_state = {
                 'config': {
                     'host': self.__ms.local_ip,
                     'port': self.__ms.port,
                     'token': self.__get_token(),
                     'ssl': False,
                     'alive': True
                 },
-                'zones': {z.id: self.__zone_to_dict(z, playback_info if z == active_zone else None) for z in zones},
+                'zones': zones_data
             }
             active_command = self.get_active_command(self.__current_state['zones'].get(active_zone.id, None))
             self.__current_state['playingCommand'] = {'active': active_command}
             self.__ws_server.broadcast(json.dumps(self.__current_state, ensure_ascii=False))
         except ConnectTimeout as e:
             logger.warning(f"Unable to connect, MC probably sleeping {e.request.method} {e.request.url}")
             self.__broadcast_down()
@@ -117,30 +172,32 @@
             return True
         else:
             return False
 
     @staticmethod
     def __zone_to_dict(zone: Zone, playback_info):
         zd = {'name': zone.name, 'id': zone.id, 'active': playback_info is not None}
+        pn = None
         if playback_info:
             InfoProvider.__extract_volume(playback_info, zd)
-            zd['playingNow'] = {
+            pn = {
                 'artist': playback_info.get('Artist', ''),
                 'album': playback_info.get('Album', ''),
                 'status': InfoProvider.__extract_status(playback_info),
                 'fileKey': playback_info.get('FileKey', ''),
                 'positionMillis': float(playback_info.get('PositionMS', 0)),
                 'durationMillis': float(playback_info.get('DurationMS', 0)),
                 'positionDisplay': playback_info.get('PlayingNowPositionDisplay', ''),
                 'imageURL': playback_info.get('ImageURL', ''),
                 'name': playback_info.get('Name', ''),
                 'externalSource': playback_info.get('Name', '') == 'Ipc'
             }
             zd['volumeRatio'] = float(playback_info.get('Volume', 0))
-        return zd
+        zd['playingNow'] = pn
+        return zd, pn
 
     @staticmethod
     def __extract_volume(playback_info: dict, zd: dict):
         volume_display = playback_info.get('VolumeDisplay', None)
         if not volume_display or volume_display == 'Muted':
             zd['muted'] = True
             zd['volumedb'] = -100.0
```

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/jvc.py` & `ezmote-cmdserver-0.8.7/cmdserver/jvc.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/jvccommands.py` & `ezmote-cmdserver-0.8.7/cmdserver/jvccommands.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/main.py` & `ezmote-cmdserver-0.8.7/cmdserver/main.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/pjcontroller.py` & `ezmote-cmdserver-0.8.7/cmdserver/pjcontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/tivocontroller.py` & `ezmote-cmdserver-0.8.7/cmdserver/tivocontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/ws.py` & `ezmote-cmdserver-0.8.7/cmdserver/ws.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/cmdserver/zeroconf.py` & `ezmote-cmdserver-0.8.7/cmdserver/zeroconf.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/PKG-INFO` & `ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmote-cmdserver
-Version: 0.8.6
+Version: 0.8.7
 Summary: A small webapp which can be used for web based home cinema automation
 Home-page: http://github.com/3ll3d00d/cmdserver
 Author: Matt Khan
 Author-email: mattkhan+cmdserver@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/SOURCES.txt` & `ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/ezmote_cmdserver.egg-info/requires.txt` & `ezmote-cmdserver-0.8.7/ezmote_cmdserver.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.6/setup.py` & `ezmote-cmdserver-0.8.7/setup.py`

 * *Files identical despite different names*

