# Comparing `tmp/citizenk-0.1.45.tar.gz` & `tmp/citizenk-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.45.tar", max compression
+gzip compressed data, was "citizenk-0.1.46.tar", max compression
```

## Comparing `citizenk-0.1.45.tar` & `citizenk-0.1.46.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      382 2023-05-01 17:44:32.309329 citizenk-0.1.45/citizenk/__init__.py
--rw-r--r--   0        0        0     8818 2023-05-02 07:11:22.020798 citizenk-0.1.45/citizenk/agent.py
--rw-r--r--   0        0        0    20655 2023-05-06 18:23:30.532087 citizenk-0.1.45/citizenk/citizenk.py
--rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.45/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.45/citizenk/murmur2.py
--rw-r--r--   0        0        0     5453 2023-05-06 18:31:26.831757 citizenk-0.1.45/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.45/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-05-06 18:34:07.359079 citizenk-0.1.45/pyproject.toml
--rw-r--r--   0        0        0      863 2023-05-06 18:34:11.566828 citizenk-0.1.45/setup.py
--rw-r--r--   0        0        0     1076 2023-05-06 18:34:11.567078 citizenk-0.1.45/PKG-INFO
+-rw-r--r--   0        0        0      382 2023-05-01 17:44:32.309329 citizenk-0.1.46/citizenk/__init__.py
+-rw-r--r--   0        0        0     8805 2023-05-06 18:47:13.206357 citizenk-0.1.46/citizenk/agent.py
+-rw-r--r--   0        0        0    20655 2023-05-06 18:23:30.532087 citizenk-0.1.46/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.46/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.46/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5453 2023-05-06 18:31:26.831757 citizenk-0.1.46/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.46/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-05-06 18:47:20.808397 citizenk-0.1.46/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-05-06 18:47:38.270075 citizenk-0.1.46/setup.py
+-rw-r--r--   0        0        0     1076 2023-05-06 18:47:38.270341 citizenk-0.1.46/PKG-INFO
```

### Comparing `citizenk-0.1.45/citizenk/agent.py` & `citizenk-0.1.46/citizenk/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         self.consumer = None
 
     def _add_websocket_route(self):
         """Add FastAPI websocket route"""
 
         @self.app.websocket(self.websocket_route)
         async def w(websocket: WebSocket):
-            await websocket.accept(logger=logger)
+            await websocket.accept()
             self.active_websocket_connections.append(websocket)
             self._handle_consumer()
             try:
                 while True:
                     # At the moment there is only support Kafka server --> Websocket client
                     # For clinet --> Kafka use REST API
                     data = await websocket.receive_text()
```

### Comparing `citizenk-0.1.45/citizenk/citizenk.py` & `citizenk-0.1.46/citizenk/citizenk.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.45/citizenk/kafka_adapter.py` & `citizenk-0.1.46/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.45/citizenk/murmur2.py` & `citizenk-0.1.46/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.45/citizenk/topic.py` & `citizenk-0.1.46/citizenk/topic.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.45/pyproject.toml` & `citizenk-0.1.46/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.45"
+version = "0.1.46"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.45/setup.py` & `citizenk-0.1.46/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.45',
+    'version': '0.1.46',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.45/PKG-INFO` & `citizenk-0.1.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.45
+Version: 0.1.46
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

