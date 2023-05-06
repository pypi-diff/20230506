# Comparing `tmp/citizenk-0.1.44.tar.gz` & `tmp/citizenk-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.44.tar", max compression
+gzip compressed data, was "citizenk-0.1.45.tar", max compression
```

## Comparing `citizenk-0.1.44.tar` & `citizenk-0.1.45.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      382 2023-05-01 09:49:27.845822 citizenk-0.1.44/citizenk/__init__.py
--rw-r--r--   0        0        0     8576 2023-05-01 17:21:54.061835 citizenk-0.1.44/citizenk/agent.py
--rw-r--r--   0        0        0    20613 2023-05-01 17:07:14.097178 citizenk-0.1.44/citizenk/citizenk.py
--rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.44/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.44/citizenk/murmur2.py
--rw-r--r--   0        0        0     5132 2023-04-29 16:34:03.441496 citizenk-0.1.44/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.44/citizenk/utils.py
--rw-r--r--   0        0        0     1521 2023-05-01 17:22:39.525375 citizenk-0.1.44/pyproject.toml
--rw-r--r--   0        0        0      863 2023-05-01 17:22:45.176355 citizenk-0.1.44/setup.py
--rw-r--r--   0        0        0     1076 2023-05-01 17:22:45.176615 citizenk-0.1.44/PKG-INFO
+-rw-r--r--   0        0        0      382 2023-05-01 17:44:32.309329 citizenk-0.1.45/citizenk/__init__.py
+-rw-r--r--   0        0        0     8818 2023-05-02 07:11:22.020798 citizenk-0.1.45/citizenk/agent.py
+-rw-r--r--   0        0        0    20655 2023-05-06 18:23:30.532087 citizenk-0.1.45/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20928 2023-04-30 10:29:36.713916 citizenk-0.1.45/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.45/citizenk/murmur2.py
+-rw-r--r--   0        0        0     5453 2023-05-06 18:31:26.831757 citizenk-0.1.45/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.45/citizenk/utils.py
+-rw-r--r--   0        0        0     1521 2023-05-06 18:34:07.359079 citizenk-0.1.45/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-05-06 18:34:11.566828 citizenk-0.1.45/setup.py
+-rw-r--r--   0        0        0     1076 2023-05-06 18:34:11.567078 citizenk-0.1.45/PKG-INFO
```

### Comparing `citizenk-0.1.44/citizenk/agent.py` & `citizenk-0.1.45/citizenk/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
+
 import json
 import logging
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Callable, List, Dict, Optional
+from typing import TYPE_CHECKING, Any, Callable, List
 
 from confluent_kafka import Message as ConfluentMessage
 from fastapi import WebSocket, WebSocketDisconnect
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, ValidationError
 
-from .topic import Topic, TopicDir
-from .utils import annotate_function, CitizenKError
 from .kafka_adapter import KafkaAdapter, KafkaRole
+from .topic import Topic, TopicDir
+from .utils import CitizenKError, annotate_function
 
 if TYPE_CHECKING:
     from .citizenk import CitizenK
 
 logger = logging.getLogger(__name__)
 
 
@@ -34,15 +35,15 @@
     def __init__(
         self,
         app: CitizenK,
         name: str,
         coroutine: Callable,
         topics: list[Topic],
         batch_size: int = 1,
-        return_type: str = "events"
+        return_type: str = "events",
     ):
         self.app = app
         self.name = name
         self.coroutine = coroutine
         self.topics = topics
         for topic in self.topics:
             if topic.topic_dir == TopicDir.OUTPUT:
@@ -77,17 +78,16 @@
                 response_class=JSONResponse,
                 methods=["POST"],
                 endpoint=endpoint,
             )
 
     @staticmethod
     def validate_messages(
-        msgs: List[ConfluentMessage],
-        topics: Dict[str,Topic]
-    ) -> List[KafkaEvent]:
+        msgs: list[ConfluentMessage], topics: dict[str, Topic]
+    ) -> list[KafkaEvent]:
         """Validate the incoming Kafka messages"""
         events = []
         for msg in msgs:
             topic_name = msg.topic()
             topic = topics[topic_name]
             try:
                 value = topic.value_type(**json.loads(msg.value()))
@@ -125,93 +125,96 @@
             result = await self.coroutine(**arguments)
             return result
         return None
 
     def __str__(self) -> str:
         return self.name
 
+
 class WebSocketAgent(Agent):
     def __init__(
         self,
         app: CitizenK,
         name: str,
         coroutine: Callable,
         topics: list[Topic],
         batch_size: int = 1,
         return_type: str = "events",
-        websocket_route: Optional[str] = None,
+        websocket_route: str | None = None,
     ):
         Agent.__init__(
             self,
             app=app,
             name=name,
             coroutine=coroutine,
             topics=topics,
             batch_size=batch_size,
-            return_type=return_type
+            return_type=return_type,
         )
         self.websocket_route = websocket_route
         if websocket_route:
             self._add_websocket_route()
         self.active_websocket_connections: list[WebSocket] = []
         self.consumer = None
 
     def _add_websocket_route(self):
-        """ Add FastAPI websocket route"""
+        """Add FastAPI websocket route"""
+
         @self.app.websocket(self.websocket_route)
         async def w(websocket: WebSocket):
-            await websocket.accept()
+            await websocket.accept(logger=logger)
             self.active_websocket_connections.append(websocket)
             self._handle_consumer()
             try:
                 while True:
+                    # At the moment there is only support Kafka server --> Websocket client
+                    # For clinet --> Kafka use REST API
                     data = await websocket.receive_text()
                     logger.info("Received data from we socket %s: ignoring", data)
             except WebSocketDisconnect:
                 self.active_websocket_connections.remove(websocket)
                 self._handle_consumer()
 
     def info(self) -> dict[str, Any]:
         return {
             "name": self.name,
             "cycles": self.cycles,
-            "connections": len(self.active_websocket_connections)
+            "connections": len(self.active_websocket_connections),
         }
 
     def _handle_consumer(self):
         if len(self.active_websocket_connections) > 0 and self.consumer is None:
             # Start consumer once there is at least one connection
             # No consumer group, by default consumes from all partitions latest
-            self.consumer = KafkaAdapter(self.app.kafka_config,KafkaRole.CONSUMER)
+            # TODO: support initial offset = latest - timedelta
+            self.consumer = KafkaAdapter(self.app.kafka_config, KafkaRole.CONSUMER)
             self.consumer.start_consumer(topics=self.topic_names)
-            logger.debug("Started agent %s consumer",self.name)
+            logger.debug("Started agent %s consumer", self.name)
         if len(self.active_websocket_connections) == 0 and self.consumer is not None:
             # Close consumer if there are no live connections...
             self.consumer.close()
             self.consumer = None
-            logger.debug("Closed agent %s consumer",self.name)
+            logger.debug("Closed agent %s consumer", self.name)
 
     async def consume(self):
         if self.consumer is not None:
-            msgs = self.consumer.consume(
-                num_messages=self.batch_size, timeout=0.1
-            )
+            msgs = self.consumer.consume(num_messages=self.batch_size, timeout=0.1)
             if len(msgs) > 0:
-                logger.debug("Agent %s consumed %s messages",self.name,len(msgs))
-                events = Agent.validate_messages(msgs, {t.name:t for t in self.topics})
+                logger.debug("Agent %s consumed %s messages", self.name, len(msgs))
+                events = Agent.validate_messages(msgs, {t.name: t for t in self.topics})
                 await self.process(events)
                 return True
         return False
 
-    def close(self):
+    async def close(self):
         if self.consumer is not None:
             self.consumer.close()
             self.consumer = None
         for connection in self.active_websocket_connections:
-            connection.close()
+            await connection.close()
 
     def _generate_apis(self):
         for topic in self.topics:
 
             async def endpoint(values: int):
                 result = await self.coroutine(values=values)
                 await self.websocket_broadcast_result(result)
@@ -228,22 +231,23 @@
                 path=f"{self.app.api_router_prefix}/agent/{self.name}/{topic.name}",
                 response_class=JSONResponse,
                 methods=["POST"],
                 endpoint=endpoint,
             )
 
     async def websocket_broadcast_result(self, result: str):
-        """ Broadcast the agent result to all clients"""
+        """Broadcast the agent result to all clients"""
         if result is None:
             return
+        # Todo, consider using websocket.broadcast
         for connection in list(self.active_websocket_connections):
             try:
                 await connection.send_text(result)
             except WebSocketDisconnect:
                 logger.info("Websocket connection disconnected")
                 self.active_websocket_connections.remove(connection)
 
     async def process(self, events: list[KafkaEvent]):
-        """ Process incoming events"""
-        result = await Agent.process(self,events)
+        """Process incoming events"""
+        result = await Agent.process(self, events)
         await self.websocket_broadcast_result(result)
         return result
```

### Comparing `citizenk-0.1.44/citizenk/citizenk.py` & `citizenk-0.1.45/citizenk/citizenk.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,42 +98,40 @@
             return {}
 
         @self.get(f"{self.api_router_prefix}/info", response_class=JSONResponse)
         def get_service_info():
             """Get the service info"""
             hosts = {}
             assignments = {}
-            lag = {}
+            lags = {}
             if self.consumer is not None:
                 hosts = self.consumer.get_group_members()
                 assignments = self.consumer.assigned_partitions
-                lag = self.consumer.get_group_lag()
+                lags = self.consumer.get_group_lag()
             return {
                 "started": self._started,
                 "app": {
                     "name": self.app_name,
                     "title": self.title,
                     "description": self.description,
                     "version": self.version,
                 },
                 "host": socket.gethostbyname(socket.gethostname()),
                 "topics": {
                     "in": [
-                        t.info()
+                        t.info(lags, assignments)
                         for t in self.topics.values()
                         if t.topic_dir != TopicDir.OUTPUT
                     ],
                     "out": [
                         t.info()
                         for t in self.topics.values()
                         if t.topic_dir != TopicDir.INPUT
                     ],
                 },
-                "lag": lag,
-                "assignments": assignments,
                 "agents": [a.info() for a in self.agents.values()],
                 "websocket_agents": [a.info() for a in self.websocket_agents.values()],
                 "hosts": {f"{tp[0]}-{tp[1]}": h for tp, h in hosts.items()},
             }
 
     def is_sink(self) -> bool:
         return self.app_type == AppType.SINK
@@ -218,20 +216,20 @@
 
         # Check that all topics exist in broker
         broker = self.producer if self.consumer is None else self.consumer
         broker_topics = broker.get_all_broker_topics()
         for topic_name, topic in self.topics.items():
             if topic_name not in broker_topics:
                 raise CitizenKError(f"Can't find topic {topic_name} in broker")
-            # Set num partitions and replicas in topic. Might be usefull...
+            # Set num partitions and replicas in topic. Might be useful...
             topic.partition_count = len(broker_topics[topic_name].partitions)
             topic.replica_count = len(broker_topics[topic_name].partitions[0].replicas)
 
         # Start Main consumer loop if there is any consumer
-        # Normal gobal consumer (with group)
+        # Normal global consumer (with group)
         # Websocket consumers (no group)
         if self.consumer is not None or len(self.websocket_agents) > 0:
 
             if self.agents_in_thread:
                 # Start in a thread
                 self.background_loop = asyncio.new_event_loop()
                 self.background_thread = threading.Thread(
@@ -260,15 +258,14 @@
         for agent in self.websocket_agents.values():
             agent.close()
         if self.main_consumer_loop_task is not None:
             self.main_consumer_loop_task.cancel()
         if self.background_loop is not None:
             self.background_loop.stop()
 
-
     def background_consumer_thread(self, loop: asyncio.BaseEventLoop):
         logger.debug("CitizenK background consumer thread started...")
         asyncio.set_event_loop(loop)
         try:
             loop.run_forever()
         except asyncio.CancelledError as e:
             logger.error("Background consumer loop cancelled %s", e)
@@ -295,15 +292,15 @@
     async def _main_consumer_loop(self):
         """Main Kafka consumer loop which invokes the process agents"""
         logger.debug("CitizenK main processing loop started...")
         while True:
             # Check if consumer was deleted
             if self.consumer is None and len(self.consumer_topics) > 0:
                 break
-            
+
             try:
                 start_time = time.time()
                 processed = False
                 # Consume from global consumer
                 if self.consumer is not None:
                     msgs = self.consumer.consume(
                         num_messages=self.total_batch_size, timeout=0.1
@@ -339,15 +336,14 @@
                     # Wait a bit until messages arrive
                     logger.debug("No kafka events, sleeping")
                     await asyncio.sleep(1)
 
             except Exception as e:
                 logger.exception("Exception in main loop: %s", str(e))
                 await asyncio.sleep(3)
-            
 
     def topic(
         self,
         name: str,
         value_type: BaseModel,
         topic_dir: TopicDir = TopicDir.INPUT,
         subject_name: Optional[str] = None,
@@ -400,15 +396,21 @@
                 raise CitizenKError("Agents can only accept values and events")
             if websocket_route is None:
                 self.agents[agent_name] = Agent(
                     self, agent_name, f, topics, batch_size, return_type
                 )
             else:
                 self.websocket_agents[agent_name] = WebSocketAgent(
-                    self, agent_name, f, topics, batch_size, return_type, websocket_route
+                    self,
+                    agent_name,
+                    f,
+                    topics,
+                    batch_size,
+                    return_type,
+                    websocket_route,
                 )
 
             logger.debug("Adding agent %s %s", agent_name, topics)
             return wrapper
 
         return decorator
```

### Comparing `citizenk-0.1.44/citizenk/kafka_adapter.py` & `citizenk-0.1.45/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.44/citizenk/murmur2.py` & `citizenk-0.1.45/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.44/citizenk/topic.py` & `citizenk-0.1.45/citizenk/topic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any, Callable, Dict, List
 
 from confluent_kafka.schema_registry import Schema, SchemaRegistryClient
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, ValidationError
 
 from .utils import CitizenKError, annotate_function
 
@@ -45,29 +45,34 @@
         self.subject_name = (
             f"{name}-value".lower() if subject_name is None else subject_name
         )
         self.schema_id = None
         self.partitioner = partitioner
         self.partition_count = None
         self.replica_count = None
-
         if self.app.auto_generate_apis:
             self._generate_apis()
 
         # Register topic schema
         self.manage_schema()
 
-    def info(self):
-        return {
+    def info(self, lags: Dict[str,int]={}, assignments: Dict[str,List[int]]={}):
+        topic_info = {
             "name": self.name,
+            "dir": self.topic_dir.name,
             "value": self.value_type.__name__,
             "subject": self.subject_name,
             "partitions": self.partition_count,
-            "replicas": self.replica_count,
+            "replicas": self.replica_count
         }
+        if self.name in lags:
+            topic_info["lag"] = lags[self.name]
+        if self.name in assignments:
+            topic_info["assignments"] = assignments[self.name]
+        return topic_info
 
     def _generate_apis(self):
         if self.topic_dir in [TopicDir.OUTPUT, TopicDir.BIDIR]:
 
             def f(value: int, key: str = ""):
                 self.send(value, key)
                 return value
```

### Comparing `citizenk-0.1.44/pyproject.toml` & `citizenk-0.1.45/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.44"
+version = "0.1.45"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
```

### Comparing `citizenk-0.1.44/setup.py` & `citizenk-0.1.45/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.44',
+    'version': '0.1.45',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.44/PKG-INFO` & `citizenk-0.1.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.44
+Version: 0.1.45
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

