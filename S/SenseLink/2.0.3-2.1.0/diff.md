# Comparing `tmp/SenseLink-2.0.3.tar.gz` & `tmp/SenseLink-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SenseLink-2.0.3.tar", last modified: Sun May 29 23:52:09 2022, max compression
+gzip compressed data, was "SenseLink-2.1.0.tar", last modified: Sat May  6 20:20:36 2023, max compression
```

## Comparing `SenseLink-2.0.3.tar` & `SenseLink-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 23:52:09.536194 SenseLink-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-05-29 23:51:44.000000 SenseLink-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10902 2022-05-29 23:52:09.536194 SenseLink-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10408 2022-05-29 23:51:44.000000 SenseLink-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 23:52:09.536194 SenseLink-2.0.3/SenseLink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10902 2022-05-29 23:52:08.000000 SenseLink-2.0.3/SenseLink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-05-29 23:52:09.000000 SenseLink-2.0.3/SenseLink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 23:52:08.000000 SenseLink-2.0.3/SenseLink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-05-29 23:52:09.000000 SenseLink-2.0.3/SenseLink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-29 23:52:09.000000 SenseLink-2.0.3/SenseLink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-29 23:51:44.000000 SenseLink-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 23:52:09.536194 SenseLink-2.0.3/senselink/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 23:52:09.536194 SenseLink-2.0.3/senselink/homeassistant/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/homeassistant/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/homeassistant/ha_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/homeassistant/ha_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 23:52:09.536194 SenseLink-2.0.3/senselink/mqtt/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/mqtt/mqtt_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     7508 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/mqtt/mqtt_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/mqtt/mqtt_listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     5512 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/plug_instance.py
--rw-r--r--   0 runner    (1001) docker     (121)    11675 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/senselink.py
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-05-29 23:51:44.000000 SenseLink-2.0.3/senselink/tplink_encryption.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 23:52:09.536194 SenseLink-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-05-29 23:51:44.000000 SenseLink-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.299939 SenseLink-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-06 20:20:23.000000 SenseLink-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-05-06 20:20:36.299939 SenseLink-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-05-06 20:20:23.000000 SenseLink-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.295939 SenseLink-2.1.0/SenseLink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 20:20:36.000000 SenseLink-2.1.0/SenseLink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 20:20:23.000000 SenseLink-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.295939 SenseLink-2.1.0/senselink/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.295939 SenseLink-2.1.0/senselink/homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/homeassistant/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/homeassistant/ha_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/homeassistant/ha_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:20:36.299939 SenseLink-2.1.0/senselink/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/mqtt/mqtt_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/mqtt/mqtt_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/mqtt/mqtt_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/plug_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/senselink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-06 20:20:23.000000 SenseLink-2.1.0/senselink/tplink_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 20:20:36.299939 SenseLink-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-06 20:20:23.000000 SenseLink-2.1.0/setup.py
```

### Comparing `SenseLink-2.0.3/LICENSE` & `SenseLink-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/PKG-INFO` & `SenseLink-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SenseLink
-Version: 2.0.3
+Version: 2.1.0
 Summary: A tool to create virtual smart plugs and inform a Sense Home Energy Monitor about usage in your home
 Home-page: https://github.com/cbpowell/SenseLink
 Author: Charles Powell
 Author-email: cbpowell@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `SenseLink-2.0.3/README.md` & `SenseLink-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/SenseLink.egg-info/PKG-INFO` & `SenseLink-2.1.0/SenseLink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SenseLink
-Version: 2.0.3
+Version: 2.1.0
 Summary: A tool to create virtual smart plugs and inform a Sense Home Energy Monitor about usage in your home
 Home-page: https://github.com/cbpowell/SenseLink
 Author: Charles Powell
 Author-email: cbpowell@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `SenseLink-2.0.3/SenseLink.egg-info/SOURCES.txt` & `SenseLink-2.1.0/SenseLink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/senselink/__main__.py` & `SenseLink-2.1.0/senselink/__main__.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/senselink/data_source.py` & `SenseLink-2.1.0/senselink/data_source.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/senselink/homeassistant/common.py` & `SenseLink-2.1.0/senselink/homeassistant/common.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/senselink/homeassistant/ha_controller.py` & `SenseLink-2.1.0/senselink/homeassistant/ha_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,37 @@
 
 class HAController:
     ws = None
     event_rq_id = 1
     bulk_rq_id = 2
     data_sources = []
 
-    def __init__(self, url, auth_token):
+    def __init__(self, url, auth_token, max_ws_message_size=None):
         self.url = url
         self.auth_token = auth_token
+        self.max_ws_message = max_ws_message_size
 
     async def connect(self):
         # Create task
         await self.client_handler()
 
     async def client_handler(self):
         logging.info(f"Starting websocket client to URL: {self.url}")
         try:
-            async with websockets.connect(self.url) as websocket:
+            if self.max_ws_message is not None:
+                max_ws_param = int(self.max_ws_message)
+                if max_ws_param > 0:
+                    ws_args = {"uri": self.url, "max_size": max_ws_param}
+                else:
+                    # Interpret 0 as None/No limit
+                    ws_args = ws_args = {"uri": self.url, "max_size": None}
+            else:
+                ws_args = {"uri": self.url}
+
+            async with websockets.connect(**ws_args) as websocket:
                 self.ws = websocket
                 # Wait for incoming message from server
                 while True:
                     try:
                         message = await websocket.recv()
                         logging.debug(f"Received message: {message}")
                         await self.on_message(websocket, message)
```

### Comparing `SenseLink-2.0.3/senselink/homeassistant/ha_data_source.py` & `SenseLink-2.1.0/senselink/homeassistant/ha_data_source.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/senselink/mqtt/mqtt_controller.py` & `SenseLink-2.1.0/senselink/mqtt/mqtt_controller.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/senselink/mqtt/mqtt_data_source.py` & `SenseLink-2.1.0/senselink/mqtt/mqtt_data_source.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/senselink/plug_instance.py` & `SenseLink-2.1.0/senselink/plug_instance.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/senselink/senselink.py` & `SenseLink-2.1.0/senselink/senselink.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,20 +118,20 @@
 
 class SenseLink:
     transport = None
     protocol = None
     should_respond = True
     has_aggregate = False
 
-    def __init__(self, config, port=9999):
+    def __init__(self, config=None, port=9999):
         self.config = config
         self.port = port
         self.target = None
         self.server_task = None
-        self._instances = {}
+        self.instances = {}
         self._agg_instances = {}
         self.tasks = set()
 
     def create_instances(self):
         config = yaml.load(self.config, Loader=yaml.FullLoader)
         logging.debug(f"Configuration loaded: {config}")
         sources = config.get('sources')
@@ -169,15 +169,16 @@
             elif source_id.lower() == HASS_KEY:
                 # Configure this HASS Data source
                 hass = source[HASS_KEY]
                 if hass is None:
                     logging.error(f"Configuration error for Source {source_id}")
                 url = hass['url']
                 auth_token = hass['auth_token']
-                hass_controller = HAController(url, auth_token)
+                max_message_size = hass.get('max_message_size') or None
+                hass_controller = HAController(url, auth_token, max_ws_message_size=max_message_size)
 
                 # Generate plug instances
                 plugs = hass[PLUGS_KEY]
                 logging.info("Generating HASS instances")
                 instances = PlugInstance.configure_plugs(plugs, HASource, hass_controller)
                 self.add_instances(instances)
 
@@ -191,24 +192,24 @@
                 mqtt_conf = source[MQTT_KEY]
                 if mqtt_conf is None:
                     logging.error(f"Configuration error for Source {source_id}")
                 host = mqtt_conf['host']
                 port = mqtt_conf.get('port') or 1883
                 username = mqtt_conf.get('username') or None
                 password = mqtt_conf.get('password') or None
-                mqtt_controller = MQTTController(host, port, username, password)
+                mqtt_cont = MQTTController(host, port, username, password)
 
                 # Generate plug instances
                 plugs = mqtt_conf[PLUGS_KEY]
                 logging.info("Generating MQTT instances")
-                instances = PlugInstance.configure_plugs(plugs, MQTTSource, mqtt_controller)
+                instances = PlugInstance.configure_plugs(plugs, MQTTSource, mqtt_cont)
                 self.add_instances(instances)
 
                 # Start controller
-                mqtt_task = mqtt_controller.connect()
+                mqtt_task = mqtt_cont.connect()
                 self.tasks.add(mqtt_task)
 
             # Aggregate-type Plugs
             elif source_id.lower() == AGG_KEY:
                 # Only one aggregate key allowed
                 if self.has_aggregate:
                     # Already defined, ignore this one
@@ -230,15 +231,15 @@
             for inst in instances.values():
                 # Grab data source for this instance
                 ag_ds = inst.data_source
                 # So that we can get the element IDs (i.e. plug_id's)
                 element_ids = ag_ds.element_ids
                 # Use those element_ids to get actual instances from global instance dict
                 elements = []
-                for plug in self._instances.values():
+                for plug in self.instances.values():
                     if plug.identifier in element_ids:
                         # Check if this plug is already in another aggregate
                         if plug.in_aggregate:
                             logging.warning(f"""Configuration adds plug {plug.identifier} to more than one Aggregate"""
                                             f""" plug. Usage in Aggregate {inst.identifier} will be ignored.""")
                             continue
                         # We want this plug
@@ -246,39 +247,49 @@
                         plug.in_aggregate = True
                 # Pass these elements (top-level plugs) back to Aggregate data source
                 ag_ds.elements = elements
             # Add these aggregate plugs to the instance list
             self.add_instances(instances)
 
     def add_instances(self, instances):
-        # Check for duplicated MAC
-        union_macs = [val for val in instances.keys() if val in self._instances.keys()]
-        if any(union_macs):
-            # Assertion error - can't use the same MAC twice!
-            raise AssertionError(
-                f"Configuration Error: Two plugs configured with the same MAC address! ({union_macs})")
+        if instances is PlugInstance:
+            # Single plug
+            p_i = instances
+            self.instances.update({p_i.identifier: p_i})
+        elif all(isinstance(p, PlugInstance) for p in instances):
+            # List of plugs, convert to dict and add to storage
+            new_instances = {p_i.identifier: p_i for p_i in instances}
+            self.instances = {**self.instances, **new_instances}
+        else:
+            # Assume Dict of plugs
+            # Check for duplicated MAC
+            union_macs = [val for val in instances.keys() if val in self.instances.keys()]
+            if any(union_macs):
+                # Assertion error - can't use the same MAC twice!
+                raise AssertionError(
+                    f"Configuration Error: Two plugs configured with the same MAC address! ({union_macs})")
 
-        # Add to global instances
-        self._instances = {**self._instances, **instances}
+            # Add to global instances
+            self.instances = {**self.instances, **instances}
 
     def plug_for_mac(self, mac):
-        return self._instances[mac]
+        return self.instances[mac]
 
     def print_instance_wattages(self):
-        for inst in self._instances:
+        for inst in self.instances:
             logging.info(f"Plug {inst.identifier} power: {inst.power}")
 
     async def start(self):
         self.tasks.add(self.server_start())
         await asyncio.gather(*self.tasks)
 
     async def server_start(self):
         loop = asyncio.get_running_loop()
         finished = loop.create_future()
-        protocol = SenseLinkProtocol(self._instances, finished)
+        protocol = SenseLinkProtocol(self.instances, finished)
         protocol.should_respond = self.should_respond
         protocol.target = self.target
 
         logging.info("Starting UDP server")
         try:
             self.transport, self.protocol = await loop.create_datagram_endpoint(
                 lambda: protocol,
```

### Comparing `SenseLink-2.0.3/senselink/tplink_encryption.py` & `SenseLink-2.1.0/senselink/tplink_encryption.py`

 * *Files identical despite different names*

### Comparing `SenseLink-2.0.3/setup.py` & `SenseLink-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SenseLink',
-    version='2.0.3',
+    version='2.1.0',
     description='A tool to create virtual smart plugs and inform a Sense Home Energy Monitor about usage in your home',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/cbpowell/SenseLink',
     author='Charles Powell',
     author_email='cbpowell@gmail.com',
     license='MIT',
```

