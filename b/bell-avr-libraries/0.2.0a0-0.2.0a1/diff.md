# Comparing `tmp/bell_avr_libraries-0.2.0a0.tar.gz` & `tmp/bell_avr_libraries-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bell_avr_libraries-0.2.0a0.tar", max compression
+gzip compressed data, was "bell_avr_libraries-0.2.0a1.tar", max compression
```

## Comparing `bell_avr_libraries-0.2.0a0.tar` & `bell_avr_libraries-0.2.0a1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1068 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/LICENSE
--rw-r--r--   0        0        0     7033 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/README.md
--rw-r--r--   0        0        0        0 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/mqtt/__init__.py
--rw-r--r--   0        0        0     5033 2023-03-01 01:05:24.887030 bell_avr_libraries-0.2.0a0/bell/avr/mqtt/client.py
--rw-r--r--   0        0        0    21037 2023-03-01 01:05:24.899030 bell_avr_libraries-0.2.0a0/bell/avr/mqtt/constants.py
--rw-r--r--   0        0        0      538 2023-03-01 01:05:24.895030 bell_avr_libraries-0.2.0a0/bell/avr/mqtt/dispatcher.py
--rw-r--r--   0        0        0    11871 2023-03-01 01:05:24.891029 bell_avr_libraries-0.2.0a0/bell/avr/mqtt/module.py
--rw-r--r--   0        0        0    23185 2023-03-01 01:05:24.883030 bell_avr_libraries-0.2.0a0/bell/avr/mqtt/payloads.py
--rw-r--r--   0        0        0     9905 2023-03-01 01:05:24.895030 bell_avr_libraries-0.2.0a0/bell/avr/mqtt/qt_widget.py
--rw-r--r--   0        0        0     2431 2023-03-01 01:05:24.887030 bell_avr_libraries-0.2.0a0/bell/avr/mqtt/serializer.py
--rw-r--r--   0        0        0        0 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/serial/__init__.py
--rw-r--r--   0        0        0      303 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/serial/client.py
--rw-r--r--   0        0        0     7634 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/serial/pcc.py
--rw-r--r--   0        0        0      825 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/serial/ports.py
--rw-r--r--   0        0        0        0 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/utils/__init__.py
--rw-r--r--   0        0        0     2163 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/utils/decorators.py
--rw-r--r--   0        0        0      723 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/utils/env.py
--rw-r--r--   0        0        0      569 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/utils/testing.py
--rw-r--r--   0        0        0     1063 2023-03-01 01:05:06.703005 bell_avr_libraries-0.2.0a0/bell/avr/utils/timing.py
--rw-r--r--   0        0        0     1584 2023-03-01 01:05:06.707005 bell_avr_libraries-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 bell_avr_libraries-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0     1938 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/README.md
+-rw-r--r--   0        0        0      444 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/__init__.py
+-rw-r--r--   0        0        0      289 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/__init__.py
+-rw-r--r--   0        0        0     5158 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/client.py
+-rw-r--r--   0        0        0    23002 2023-05-06 02:54:35.904636 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/constants.py
+-rw-r--r--   0        0        0      584 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/dispatcher.py
+-rw-r--r--   0        0        0    15050 2023-05-06 02:54:35.900636 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/module.py
+-rw-r--r--   0        0        0    27660 2023-05-06 02:54:35.892636 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/payloads.py
+-rw-r--r--   0        0        0    12127 2023-05-06 02:54:35.908636 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/qt_widget.py
+-rw-r--r--   0        0        0     2534 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/serializer.py
+-rw-r--r--   0        0        0      124 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/serial/__init__.py
+-rw-r--r--   0        0        0      746 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/serial/client.py
+-rw-r--r--   0        0        0    10089 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/serial/pcc.py
+-rw-r--r--   0        0        0      935 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/serial/ports.py
+-rw-r--r--   0        0        0      206 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/__init__.py
+-rw-r--r--   0        0        0     3076 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/decorators.py
+-rw-r--r--   0        0        0     1070 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/env.py
+-rw-r--r--   0        0        0     2890 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/images.py
+-rw-r--r--   0        0        0      726 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/testing.py
+-rw-r--r--   0        0        0     1494 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/timing.py
+-rw-r--r--   0        0        0     1805 2023-05-06 02:54:12.460394 bell_avr_libraries-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3058 1970-01-01 00:00:00.000000 bell_avr_libraries-0.2.0a1/PKG-INFO
```

### Comparing `bell_avr_libraries-0.2.0a0/LICENSE` & `bell_avr_libraries-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/mqtt/client.py` & `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # create the MQTT client
         # Currently using MQTT v3.1.1
         # No reason we can't use v5, just type hinting needs to change
         # for some `on_` functions.
-        self._mqtt_client = paho_mqtt.Client(client_id=f"{self.__class__.__name__}_{uuid.uuid4()}", protocol=paho_mqtt.MQTTv311)
+        self._mqtt_client = paho_mqtt.Client(
+            client_id=f"{self.__class__.__name__}_{uuid.uuid4()}",
+            protocol=paho_mqtt.MQTTv311,
+        )
 
         # set up the on connect and on message handlers
         self._mqtt_client.on_connect = self.on_connect
 
         # dictionary of MQTT topics to callback functions
         # this is intended to be overwritten by the child class
         self.topic_callbacks: _MQTTTopicCallableTypedDict = {}
@@ -35,15 +38,17 @@
 
         # enable verbose logging
         self.enable_verbose_logging: bool = False
 
         # record if we were started with loop forever
         self._looped_forever = False
 
-    def on_connect(self, client: paho_mqtt.Client, userdata: Any, flags: dict, rc: int) -> None:
+    def on_connect(
+        self, client: paho_mqtt.Client, userdata: Any, flags: dict, rc: int
+    ) -> None:
         """
         On connection callback. Subscribes to MQTT topics in the topic map,
         plus any additional `self.subscribe_to` flags.
         """
         logger.debug(f"Connected with result {rc}")
 
         for topic in self.topic_callbacks.keys():
@@ -65,73 +70,83 @@
         rc: int,
     ) -> None:
         """
         Callback when the MQTT client disconnects.
         """
         logger.debug("Disconnected from MQTT server")
 
-    def _connect(self, host: str, port: int) -> None:
+    def connect_(self, host: str, port: int) -> None:
         """
         Connect the MQTT client to the broker. This method cannot be named "connect"
         as this conflicts with the connect methods of Qt Signals.
         """
         if self.enable_verbose_logging:
             logger.info(f"Connecting to MQTT broker at {host}:{port}")
 
         self._mqtt_client.connect(host=host, port=port, keepalive=60)
 
         logger.success("Connected to MQTT broker")
 
         # if an on_message callback has been defined, connect it
         if hasattr(self, "on_message"):
-            self._mqtt_client.on_message = self.on_message # type: ignore
+            self._mqtt_client.on_message = self.on_message  # type: ignore
 
     def stop(self) -> None:
         """
         Stops the MQTT loop and disconnects from the broker.
         """
         if self.enable_verbose_logging:
             logger.info("Disconnecting from MQTT server")
 
         self._mqtt_client.disconnect()
         self._mqtt_client.loop_stop()
 
         if self.enable_verbose_logging:
             logger.info("Disconnected from MQTT server")
 
-    def run(self, host: str = os.getenv("MQTT_HOST", "mqtt"), port: int = get_env_int("MQTT_PORT", 18830) ) -> None:
+    def run(
+        self,
+        host: str = os.getenv("MQTT_HOST", "mqtt"),
+        port: int = get_env_int("MQTT_PORT", 18830),
+    ) -> None:
         """
         Class entrypoint. Connects to the MQTT broker and starts the MQTT loop
         in a blocking manner.
         """
         # connect the MQTT client
-        self._connect(host, port)
+        self.connect_(host, port)
         # run forever
         self._looped_forever = True
         self._mqtt_client.loop_forever()
 
-    def run_non_blocking(self, host: str = os.getenv("MQTT_HOST", "mqtt"), port: int = get_env_int("MQTT_PORT", 18830) ) -> None:
+    def run_non_blocking(
+        self,
+        host: str = os.getenv("MQTT_HOST", "mqtt"),
+        port: int = get_env_int("MQTT_PORT", 18830),
+    ) -> None:
         """
         Class entrypoint. Connects to the MQTT broker and starts the MQTT loop
         in a non-blocking manner.
         """
         # connect the MQTT client
-        self._connect(host, port)
+        self.connect_(host, port)
         # run in background
         self._mqtt_client.loop_start()
 
-    def _publish(self, topic: str, payload: Union[str, bytes], force_write: bool = False) -> None:
+    def _publish(
+        self, topic: str, payload: Union[str, bytes], force_write: bool = False
+    ) -> None:
         """
         Raw publish function that expects a topic and a payload as a string or bytes.
         """
         if self.enable_verbose_logging:
             logger.debug(f"Publishing message to {topic}: {payload}")
 
         self._mqtt_client.publish(topic, payload)
 
         # https://github.com/eclipse/paho.mqtt.python/blob/9782ab81fe7ee3a05e74c7f3e1d03d5611ea4be4/src/paho/mqtt/client.py#L1563
         # pre-emptively write network data while still in a callback, bypassing
         # the thread mutex.
         # can only be used if run with .loop_forever()
         # https://www.bellavrforum.org/t/sending-messages-to-pcc-from-sandbox/311/8
         if self._looped_forever or force_write:
-            self._mqtt_client.loop_write()
+            self._mqtt_client.loop_write()
```

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/mqtt/constants.py` & `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,20 @@
     _AVRVIOAttitudeEulerRadiansCallable,
     AVRVIOAttitudeQuaternion,
     _AVRVIOAttitudeQuaternionCallable,
     AVRVIOHeading,
     _AVRVIOHeadingCallable,
     AVRVIOConfidence,
     _AVRVIOConfidenceCallable,
+    AVRVIOImageCapture,
+    _AVRVIOImageCaptureCallable,
+    AVRVIOImageRequest,
+    _AVRVIOImageRequestCallable,
+    AVRVIOImageStreamEnable,
+    _AVRVIOImageStreamEnableCallable,
     AVRAprilTagsVehiclePosition,
     _AVRAprilTagsVehiclePositionCallable,
     AVRAprilTagsRaw,
     _AVRAprilTagsRawCallable,
     AVRAprilTagsVisible,
     _AVRAprilTagsVisibleCallable,
     AVRAprilTagsStatus,
@@ -88,16 +94,14 @@
     _AVRThermalReadingCallable,
     AVRAutonomousBuildingEnable,
     _AVRAutonomousBuildingEnableCallable,
     AVRAutonomousBuildingDisable,
     _AVRAutonomousBuildingDisableCallable,
 )
 
-
-
 MQTTTopics = [
     "avr/pcm/color/set",
     "avr/pcm/color/timed",
     "avr/pcm/laser/fire",
     "avr/pcm/laser/on",
     "avr/pcm/laser/off",
     "avr/pcm/servo/open",
@@ -131,14 +135,18 @@
     "avr/vio/resync",
     "avr/vio/position/local",
     "avr/vio/velocity",
     "avr/vio/attitude/euler/radians",
     "avr/vio/attitude/quaternion",
     "avr/vio/heading",
     "avr/vio/confidence",
+    "avr/vio/image/capture",
+    "avr/vio/image/request",
+    "avr/vio/image/stream/enable",
+    "avr/vio/image/stream/disable",
     "avr/apriltags/vehicle_position",
     "avr/apriltags/raw",
     "avr/apriltags/visible",
     "avr/apriltags/status",
     "avr/status/led/pcm",
     "avr/status/led/vio",
     "avr/status/led/apriltags",
@@ -147,15 +155,15 @@
     "avr/thermal/reading",
     "avr/autonomous/enable",
     "avr/autonomous/disable",
     "avr/autonomous/building/enable",
     "avr/autonomous/building/disable",
 ]
 """
-List of all MQTT topics
+List of all MQTT topics as strings. This is in no particular order.
 """
 
 MQTTPayloads = [
     AVRPCMColorSet,
     AVRPCMColorTimed,
     AVREmptyMessage,
     AVRPCMServo,
@@ -187,24 +195,28 @@
     AVRVIOResync,
     AVRVIOPositionLocal,
     AVRVIOVelocity,
     AVRVIOAttitudeEulerRadians,
     AVRVIOAttitudeQuaternion,
     AVRVIOHeading,
     AVRVIOConfidence,
+    AVRVIOImageCapture,
+    AVRVIOImageRequest,
+    AVRVIOImageStreamEnable,
     AVRAprilTagsVehiclePosition,
     AVRAprilTagsRaw,
     AVRAprilTagsVisible,
     AVRAprilTagsStatus,
     AVRThermalReading,
     AVRAutonomousBuildingEnable,
     AVRAutonomousBuildingDisable,
 ]
 """
-List of all MQTT payload classes
+List of all MQTT payload classes. This is in no particular order.
+There are no duplicates.
 """
 
 _MQTTTopicCallableTypedDict = TypedDict(
     "_MQTTTopicCallableTypedDict",
     {
         "avr/pcm/color/set": _AVRPCMColorSetCallable,
         "avr/pcm/color/timed": _AVRPCMColorTimedCallable,
@@ -242,14 +254,18 @@
         "avr/vio/resync": _AVRVIOResyncCallable,
         "avr/vio/position/local": _AVRVIOPositionLocalCallable,
         "avr/vio/velocity": _AVRVIOVelocityCallable,
         "avr/vio/attitude/euler/radians": _AVRVIOAttitudeEulerRadiansCallable,
         "avr/vio/attitude/quaternion": _AVRVIOAttitudeQuaternionCallable,
         "avr/vio/heading": _AVRVIOHeadingCallable,
         "avr/vio/confidence": _AVRVIOConfidenceCallable,
+        "avr/vio/image/capture": _AVRVIOImageCaptureCallable,
+        "avr/vio/image/request": _AVRVIOImageRequestCallable,
+        "avr/vio/image/stream/enable": _AVRVIOImageStreamEnableCallable,
+        "avr/vio/image/stream/disable": _AVREmptyMessageCallable,
         "avr/apriltags/vehicle_position": _AVRAprilTagsVehiclePositionCallable,
         "avr/apriltags/raw": _AVRAprilTagsRawCallable,
         "avr/apriltags/visible": _AVRAprilTagsVisibleCallable,
         "avr/apriltags/status": _AVRAprilTagsStatusCallable,
         "avr/status/led/pcm": _AVREmptyMessageCallable,
         "avr/status/led/vio": _AVREmptyMessageCallable,
         "avr/status/led/apriltags": _AVREmptyMessageCallable,
@@ -260,15 +276,16 @@
         "avr/autonomous/disable": _AVREmptyMessageCallable,
         "avr/autonomous/building/enable": _AVRAutonomousBuildingEnableCallable,
         "avr/autonomous/building/disable": _AVRAutonomousBuildingDisableCallable,
     },
     total=False
 )
 """
-TypedDict of topics to callback function signature
+TypedDict of topics as keys, and function signatures that accept the corresponding
+payload class as values.
 """
 
 MQTTTopicCallable: _MQTTTopicCallableTypedDict = {
     "avr/pcm/color/set": _AVRPCMColorSetCallable,
     "avr/pcm/color/timed": _AVRPCMColorTimedCallable,
     "avr/pcm/laser/fire": _AVREmptyMessageCallable,
     "avr/pcm/laser/on": _AVREmptyMessageCallable,
@@ -304,14 +321,18 @@
     "avr/vio/resync": _AVRVIOResyncCallable,
     "avr/vio/position/local": _AVRVIOPositionLocalCallable,
     "avr/vio/velocity": _AVRVIOVelocityCallable,
     "avr/vio/attitude/euler/radians": _AVRVIOAttitudeEulerRadiansCallable,
     "avr/vio/attitude/quaternion": _AVRVIOAttitudeQuaternionCallable,
     "avr/vio/heading": _AVRVIOHeadingCallable,
     "avr/vio/confidence": _AVRVIOConfidenceCallable,
+    "avr/vio/image/capture": _AVRVIOImageCaptureCallable,
+    "avr/vio/image/request": _AVRVIOImageRequestCallable,
+    "avr/vio/image/stream/enable": _AVRVIOImageStreamEnableCallable,
+    "avr/vio/image/stream/disable": _AVREmptyMessageCallable,
     "avr/apriltags/vehicle_position": _AVRAprilTagsVehiclePositionCallable,
     "avr/apriltags/raw": _AVRAprilTagsRawCallable,
     "avr/apriltags/visible": _AVRAprilTagsVisibleCallable,
     "avr/apriltags/status": _AVRAprilTagsStatusCallable,
     "avr/status/led/pcm": _AVREmptyMessageCallable,
     "avr/status/led/vio": _AVREmptyMessageCallable,
     "avr/status/led/apriltags": _AVREmptyMessageCallable,
@@ -320,15 +341,17 @@
     "avr/thermal/reading": _AVRThermalReadingCallable,
     "avr/autonomous/enable": _AVREmptyMessageCallable,
     "avr/autonomous/disable": _AVREmptyMessageCallable,
     "avr/autonomous/building/enable": _AVRAutonomousBuildingEnableCallable,
     "avr/autonomous/building/disable": _AVRAutonomousBuildingDisableCallable,
 }
 """
-Complete dictionary of topics to callback function signature
+Complete dictionary of topics as keys, and function signatures that
+accept the corresponding payload class as values.
+This is used for `bell.avr.mqtt.module.MQTTModule.topic_callbacks`.
 """
 
 _MQTTTopicPayloadTypedDict = TypedDict(
     "_MQTTTopicPayloadTypedDict",
     {
         "avr/pcm/color/set": AVRPCMColorSet,
         "avr/pcm/color/timed": AVRPCMColorTimed,
@@ -366,14 +389,18 @@
         "avr/vio/resync": AVRVIOResync,
         "avr/vio/position/local": AVRVIOPositionLocal,
         "avr/vio/velocity": AVRVIOVelocity,
         "avr/vio/attitude/euler/radians": AVRVIOAttitudeEulerRadians,
         "avr/vio/attitude/quaternion": AVRVIOAttitudeQuaternion,
         "avr/vio/heading": AVRVIOHeading,
         "avr/vio/confidence": AVRVIOConfidence,
+        "avr/vio/image/capture": AVRVIOImageCapture,
+        "avr/vio/image/request": AVRVIOImageRequest,
+        "avr/vio/image/stream/enable": AVRVIOImageStreamEnable,
+        "avr/vio/image/stream/disable": AVREmptyMessage,
         "avr/apriltags/vehicle_position": AVRAprilTagsVehiclePosition,
         "avr/apriltags/raw": AVRAprilTagsRaw,
         "avr/apriltags/visible": AVRAprilTagsVisible,
         "avr/apriltags/status": AVRAprilTagsStatus,
         "avr/status/led/pcm": AVREmptyMessage,
         "avr/status/led/vio": AVREmptyMessage,
         "avr/status/led/apriltags": AVREmptyMessage,
@@ -384,15 +411,15 @@
         "avr/autonomous/disable": AVREmptyMessage,
         "avr/autonomous/building/enable": AVRAutonomousBuildingEnable,
         "avr/autonomous/building/disable": AVRAutonomousBuildingDisable,
     },
     total=False
 )
 """
-TypedDict of topics to associated payloads
+TypedDict with topics as keys, and the associated payload class as values.
 """
 
 _MQTTTopicPayloadTypeTypedDict = TypedDict(
     "_MQTTTopicPayloadTypeTypedDict",
     {
         "avr/pcm/color/set": Type[AVRPCMColorSet],
         "avr/pcm/color/timed": Type[AVRPCMColorTimed],
@@ -430,14 +457,18 @@
         "avr/vio/resync": Type[AVRVIOResync],
         "avr/vio/position/local": Type[AVRVIOPositionLocal],
         "avr/vio/velocity": Type[AVRVIOVelocity],
         "avr/vio/attitude/euler/radians": Type[AVRVIOAttitudeEulerRadians],
         "avr/vio/attitude/quaternion": Type[AVRVIOAttitudeQuaternion],
         "avr/vio/heading": Type[AVRVIOHeading],
         "avr/vio/confidence": Type[AVRVIOConfidence],
+        "avr/vio/image/capture": Type[AVRVIOImageCapture],
+        "avr/vio/image/request": Type[AVRVIOImageRequest],
+        "avr/vio/image/stream/enable": Type[AVRVIOImageStreamEnable],
+        "avr/vio/image/stream/disable": Type[AVREmptyMessage],
         "avr/apriltags/vehicle_position": Type[AVRAprilTagsVehiclePosition],
         "avr/apriltags/raw": Type[AVRAprilTagsRaw],
         "avr/apriltags/visible": Type[AVRAprilTagsVisible],
         "avr/apriltags/status": Type[AVRAprilTagsStatus],
         "avr/status/led/pcm": Type[AVREmptyMessage],
         "avr/status/led/vio": Type[AVREmptyMessage],
         "avr/status/led/apriltags": Type[AVREmptyMessage],
@@ -448,15 +479,15 @@
         "avr/autonomous/disable": Type[AVREmptyMessage],
         "avr/autonomous/building/enable": Type[AVRAutonomousBuildingEnable],
         "avr/autonomous/building/disable": Type[AVRAutonomousBuildingDisable],
     },
     total=False
 )
 """
-TypedDict of topics to associated payloads types
+TypedDict with topics as keys, and the associated payload class type as values.
 """
 
 MQTTTopicPayload: _MQTTTopicPayloadTypeTypedDict = {
     "avr/pcm/color/set": AVRPCMColorSet,
     "avr/pcm/color/timed": AVRPCMColorTimed,
     "avr/pcm/laser/fire": AVREmptyMessage,
     "avr/pcm/laser/on": AVREmptyMessage,
@@ -492,14 +523,18 @@
     "avr/vio/resync": AVRVIOResync,
     "avr/vio/position/local": AVRVIOPositionLocal,
     "avr/vio/velocity": AVRVIOVelocity,
     "avr/vio/attitude/euler/radians": AVRVIOAttitudeEulerRadians,
     "avr/vio/attitude/quaternion": AVRVIOAttitudeQuaternion,
     "avr/vio/heading": AVRVIOHeading,
     "avr/vio/confidence": AVRVIOConfidence,
+    "avr/vio/image/capture": AVRVIOImageCapture,
+    "avr/vio/image/request": AVRVIOImageRequest,
+    "avr/vio/image/stream/enable": AVRVIOImageStreamEnable,
+    "avr/vio/image/stream/disable": AVREmptyMessage,
     "avr/apriltags/vehicle_position": AVRAprilTagsVehiclePosition,
     "avr/apriltags/raw": AVRAprilTagsRaw,
     "avr/apriltags/visible": AVRAprilTagsVisible,
     "avr/apriltags/status": AVRAprilTagsStatus,
     "avr/status/led/pcm": AVREmptyMessage,
     "avr/status/led/vio": AVREmptyMessage,
     "avr/status/led/apriltags": AVREmptyMessage,
@@ -508,9 +543,10 @@
     "avr/thermal/reading": AVRThermalReading,
     "avr/autonomous/enable": AVREmptyMessage,
     "avr/autonomous/disable": AVREmptyMessage,
     "avr/autonomous/building/enable": AVRAutonomousBuildingEnable,
     "avr/autonomous/building/disable": AVRAutonomousBuildingDisable,
 }
 """
-Actual dictionary of topics to associated payload types
+Complete dictionary with topics as keys, and the associated payload class type
+as values.
 """
```

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/mqtt/dispatcher.py` & `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/dispatcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import Any
 
 from bell.avr.mqtt.constants import _MQTTTopicCallableTypedDict
 from bell.avr.mqtt.payloads import AVREmptyMessage
 
+
 def dispatch_message(
     topic_callbacks: _MQTTTopicCallableTypedDict, topic: str, payload: Any
-):
+) -> None:
     """
-    Dispatch a message to the appropriate callback with the correct arguments.
+    Given a dictionary of topics and callbacks,
+    this executes appropriate callback with the correct arguments.
     """
     if topic not in topic_callbacks:
         return
 
     # execute callback
     if isinstance(payload, AVREmptyMessage):
         topic_callbacks[topic]()
     else:
-        topic_callbacks[topic](payload)
+        topic_callbacks[topic](payload)
```

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/mqtt/module.py` & `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/module.py`

 * *Files 26% similar despite different names*

```diff
@@ -45,40 +45,94 @@
     AVRVIOResync,
     AVRVIOPositionLocal,
     AVRVIOVelocity,
     AVRVIOAttitudeEulerRadians,
     AVRVIOAttitudeQuaternion,
     AVRVIOHeading,
     AVRVIOConfidence,
+    AVRVIOImageCapture,
+    AVRVIOImageRequest,
+    AVRVIOImageStreamEnable,
     AVRAprilTagsVehiclePosition,
     AVRAprilTagsRaw,
     AVRAprilTagsVisible,
     AVRAprilTagsStatus,
     AVRThermalReading,
     AVRAutonomousBuildingEnable,
     AVRAutonomousBuildingDisable,
 )
 from bell.avr.mqtt.serializer import deserialize_payload, serialize_payload
 
 
 class MQTTModule(MQTTClient):
     """
-    Generic MQTT Module class that should be inherited by other modules.
-    The `topic_callbacks` attribute should be a dictionary of topics to functions
-    that will be called with a payload.
+    This is a boilerplate module for AVR that makes it very easy to send
+    and receive MQTT messages and do something with them.
+
+    Here is an example of a module that changes the LED color every 5 seconds:
+    ```python
+    import random
+    import time
+
+    from bell.avr.mqtt.module import MQTTModule
+    from bell.avr.mqtt.payloads import AVRPCMColorSet
+
+
+    class Sandbox(MQTTModule):
+        def update_led(self) -> None:
+            wrgb = tuple(random.randint(0, 255) for _ in range(4))
+            self.send_message("avr/pcm/color/set", AVRPCMColorSet(wrgb=wrgb))
+
+        def run(self) -> None:
+            super().run_non_blocking()
+
+            while True:
+                time.sleep(5)
+                self.update_led()
+
+
+    if __name__ == "__main__":
+        box = Sandbox()
+        box.run()
+    ```
+
+    For a fully commented code example, see
+    [AVR-VMC-Sandbox-Module](https://github.com/bellflight/AVR-VMC-Sandbox-Module).
+
+    See `bell.avr.mqtt.client.MQTTClient.topic_callbacks` for more information on how to set up callbacks.
+
+    Additionally, the `message_cache` attribute is a dictionary that holds
+    a copy of the last payload sent by that module on a given topic. The keys are the
+    topic strings, and the values are the topic payloads.
     """
     def __init__(self):
         super().__init__()
 
-        # maintain a cache of the last message sent on a topic by this client
         self.message_cache: _MQTTTopicPayloadTypedDict = {}
+        """
+        The `message_cache` attribute is a dictionary that holds
+        a copy of the last payload sent by *that* module on a given topic.
+        The keys are the topic strings, and the values are the topic payloads.
+        This can be useful for doing operations based on the last known state
+        of a topic.
+
+        Example from the Fusion module:
+
+        ```python
+        if "avr/fusion/heading" in self.message_cache:
+            heading = int(self.message_cache["avr/fusion/heading"].hdg * 100)
+        else:
+            logger.debug("Waiting for avr/fusion/attitude/heading to be populated")
+            return
+        ```
+        """
 
     def on_message(self, client: paho_mqtt.Client, userdata: Any, msg: paho_mqtt.MQTTMessage) -> None:
         """
-        Process and dispatch an incoming message.
+        Process and dispatch an incoming message. This is called automatically.
         """
         payload = deserialize_payload(msg.topic, msg.payload)
 
         if self.enable_verbose_logging:
             logger.debug(f"Recieved {msg.topic}: {msg.payload}")
 
         dispatch_message(self.topic_callbacks, msg.topic, payload)
@@ -160,14 +214,22 @@
     @overload
     def send_message(self, topic: Literal["avr/vio/attitude/quaternion"], payload: Union[AVRVIOAttitudeQuaternion, dict], force_write: bool = False) -> None: ...
     @overload
     def send_message(self, topic: Literal["avr/vio/heading"], payload: Union[AVRVIOHeading, dict], force_write: bool = False) -> None: ...
     @overload
     def send_message(self, topic: Literal["avr/vio/confidence"], payload: Union[AVRVIOConfidence, dict], force_write: bool = False) -> None: ...
     @overload
+    def send_message(self, topic: Literal["avr/vio/image/capture"], payload: Union[AVRVIOImageCapture, dict], force_write: bool = False) -> None: ...
+    @overload
+    def send_message(self, topic: Literal["avr/vio/image/request"], payload: Union[AVRVIOImageRequest, dict], force_write: bool = False) -> None: ...
+    @overload
+    def send_message(self, topic: Literal["avr/vio/image/stream/enable"], payload: Union[AVRVIOImageStreamEnable, dict], force_write: bool = False) -> None: ...
+    @overload
+    def send_message(self, topic: Literal["avr/vio/image/stream/disable"], payload: Union[AVREmptyMessage, dict, None] = None, force_write: bool = False) -> None: ...
+    @overload
     def send_message(self, topic: Literal["avr/apriltags/vehicle_position"], payload: Union[AVRAprilTagsVehiclePosition, dict], force_write: bool = False) -> None: ...
     @overload
     def send_message(self, topic: Literal["avr/apriltags/raw"], payload: Union[AVRAprilTagsRaw, dict], force_write: bool = False) -> None: ...
     @overload
     def send_message(self, topic: Literal["avr/apriltags/visible"], payload: Union[AVRAprilTagsVisible, dict], force_write: bool = False) -> None: ...
     @overload
     def send_message(self, topic: Literal["avr/apriltags/status"], payload: Union[AVRAprilTagsStatus, dict], force_write: bool = False) -> None: ...
@@ -190,14 +252,38 @@
     @overload
     def send_message(self, topic: Literal["avr/autonomous/building/enable"], payload: Union[AVRAutonomousBuildingEnable, dict], force_write: bool = False) -> None: ...
     @overload
     def send_message(self, topic: Literal["avr/autonomous/building/disable"], payload: Union[AVRAutonomousBuildingDisable, dict], force_write: bool = False) -> None: ...
 
     def send_message(self, topic: str, payload: Union[pydantic.BaseModel, dict, None] = None, force_write: bool = False) -> None:
         """
-        Sends a message to the MQTT broker. Enabling `force_write` will
+        Sends a message to the MQTT broker. This expects a topic to send the message
+        on, and the payload for the message. The payload can either be a class
+        or a dictionary.
+
+        Example:
+
+        ```python
+        from bell.avr.mqtt.payloads import AVRPCMServoAbsolute
+
+        ...
+
+        # Python class
+        self.send_message("avr/pcm/servo/absolute", AVRPCMServoAbsolute(servo=2, position=100))
+
+        # Python dicts
+        self.send_message("avr/pcm/servo/absolute", {"servo": 2, "position": 100})
+        ```
+
+        Using Python classes are highly recommended as this performs
+        extra validation checks.
+
+        For `send_message` to work, either `run` or `run_non_blocking` must have
+        already been called.
+
+        Enabling `force_write` will
         forcefully send the message, bypassing threading mutex. Only use this
         if you know what you're doing.
         """
         str_payload = serialize_payload(topic, payload)
         self._publish(topic, str_payload, force_write)
         self.message_cache[topic] = copy.deepcopy(payload)
```

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/mqtt/payloads.py` & `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/payloads.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,54 @@
 # This file is automatically @generated. DO NOT EDIT!
 # fmt: off
 
+"""
+These are Python classes for MQTT message payloads.
+As AVR exclusively uses JSON, these are all [Pydantic](https://docs.pydantic.dev/)
+classes that have all of the required fields for a message.
+
+This is a Python implementation of the AVR [AsyncAPI definition](../mqtt/asyncapi).
+Example:
+
+```python
+from bell.avr.mqtt.payloads import AVRPCMColorSet
+
+payload = AVRPCMColorSet(wrgb=(128, 232, 142, 0))```
+"""
+
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, List, Literal, Optional, Protocol, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, List, Literal, Optional, Protocol, Tuple, Type, Union, overload
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import Extra, Field, conlist, validator
 
 
-def _convert_type(iter: Union[list, tuple], convert_to: Union[Type[int], Type[float]]) -> Union[tuple, int, float]:
-    if isinstance(iter, (tuple, list)):
-        return tuple(_convert_type(x, convert_to) for x in iter)
+@overload
+def _convert_type(iter_in: Union[list, tuple], iter_out: Type[list], items_convert_to: Type[int]) -> List[int]: ...
+
+@overload
+def _convert_type(iter_in: Union[list, tuple], iter_out: Type[list], items_convert_to: Type[float]) -> List[float]: ...
+
+@overload
+def _convert_type(iter_in: Union[list, tuple], iter_out: Type[tuple], items_convert_to: Type[int]) -> Tuple[int, ...]: ...
+
+@overload
+def _convert_type(iter_in: Union[list, tuple], iter_out: Type[tuple], items_convert_to: Type[float]) -> Tuple[float, ...]: ...
+
+def _convert_type(iter_in: Union[list, tuple], iter_out: Union[Type[list], Type[tuple]], items_convert_to: Union[Type[int], Type[float]]) -> Union[tuple, list, int, float]:
+    if isinstance(iter_in, (tuple, list)):
+        return iter_out(_convert_type(x, iter_out, items_convert_to) for x in iter_in)
     else:
-        return convert_to(iter)
+        return items_convert_to(iter_in)
 
 
 class BaseModel(PydanticBaseModel):
     class Config:
+        'For [Pydantic configuration](https://docs.pydantic.dev/latest/usage/model_config/), please ignore.'
         extra = Extra.forbid
 
 
 class AVREmptyMessage(BaseModel):
     pass
 
 class AVRPCMColorSetWrgbItem(BaseModel):
@@ -36,16 +63,16 @@
         wrgb: Tuple[int, int, int, int]
     else:
         wrgb: conlist(AVRPCMColorSetWrgbItem, min_items=4, max_items=4)
     """
     Color values for the white, red, green, and blue channels, respectively.
     """
     @validator('wrgb')
-    def validate_wrgb(cls, v):
-        return _convert_type(v, int)
+    def _validate_wrgb(cls, v) -> tuple:
+        return _convert_type(v, tuple, int)
 
 
 class AVRPCMColorTimedWrgbItem(BaseModel):
     __root__: int = Field(..., ge=0, le=255)
 
     def __int__(self) -> int:
         return self.__root__
@@ -56,16 +83,16 @@
         wrgb: Tuple[int, int, int, int]
     else:
         wrgb: conlist(AVRPCMColorTimedWrgbItem, min_items=4, max_items=4)
     """
     Color values for the white, red, green, and blue channels, respectively.
     """
     @validator('wrgb')
-    def validate_wrgb(cls, v):
-        return _convert_type(v, int)
+    def _validate_wrgb(cls, v) -> tuple:
+        return _convert_type(v, tuple, int)
 
     time: float = Field(default=0.5, ge=0)
     """
     Number of seconds the color should be set for. Default is 0.5.
     """
 
 class AVRPCMServo(BaseModel):
@@ -470,14 +497,89 @@
 
 class AVRVIOConfidence(BaseModel):
     tracking: float = Field(..., ge=0, le=100)
     """
     Tracking confidence percentage. Higher number is better.
     """
 
+class AVRVIOImageCaptureShapeItem(BaseModel):
+    __root__: int = Field(..., ge=1)
+
+    def __int__(self) -> int:
+        return self.__root__
+
+
+class AVRVIOImageCapture(BaseModel):
+    data: str
+    """
+    Base64 encoded data of the image. To reconstruct this as a numpy array,
+use `bell.avr.utils.images.deserialize_image` and an `bell.avr.utils.images.ImageData` class.
+Alternatively, manually reconstructing the image is as follows:
+
+```python
+import base64
+import zlib
+import numpy as np
+
+image_bytes = base64.b64decode(image_data.encode("utf-8"))
+
+if compressed:
+    image_bytes = zlib.decompress(image_bytes)
+
+image_byte_array = bytearray(image_bytes)
+image_array = np.array(image_byte_array)
+
+original_array = np.reshape(image_array, shape)
+```
+
+    """
+    side: Literal["left", "right"]
+    """
+    Which side of the camera to capture an image from
+    """
+    if TYPE_CHECKING:
+        shape: List[int]
+    else:
+        shape: List[AVRVIOImageCaptureShapeItem]
+    """
+    The shape of the image data. For example: [1270, 480, 4] would be a 1270x480 image with 4 channels per pixel.
+    """
+    @validator('shape')
+    def _validate_shape(cls, v) -> list:
+        return _convert_type(v, list, int)
+
+    compressed: bool
+    """
+    Whether or not the image data is zlib compressed.
+    """
+
+class AVRVIOImageRequest(BaseModel):
+    side: Literal["left", "right"]
+    """
+    Which side of the camera to capture an image from
+    """
+    compressed: bool = Field(default=False)
+    """
+    Whether or not the image data should be zlib compressed.
+    """
+
+class AVRVIOImageStreamEnable(BaseModel):
+    side: Literal["left", "right"]
+    """
+    Which side of the camera to capture an image from
+    """
+    compressed: bool = Field(default=False)
+    """
+    Whether or not the image data should be zlib compressed.
+    """
+    frequency: float = Field(..., gt=0, le=5)
+    """
+    At what rate should new images be sent (frames per second).
+    """
+
 class AVRAprilTagsVehiclePosition(BaseModel):
     tag_id: int = Field(..., ge=0)
     """
     AprilTag ID.
     """
     x: float
     """
@@ -524,16 +626,16 @@
         rotation: Tuple[Tuple[float, float, float], Tuple[float, float, float], Tuple[float, float, float]]
     else:
         rotation: conlist(conlist(AVRAprilTagsRawApriltagsRotationItem, min_items=3, max_items=3), min_items=3, max_items=3)
     """
     3x3 rotation matrix.
     """
     @validator('rotation')
-    def validate_rotation(cls, v):
-        return _convert_type(v, float)
+    def _validate_rotation(cls, v) -> tuple:
+        return _convert_type(v, tuple, float)
 
 
 class AVRAprilTagsRaw(BaseModel):
     apriltags: List[AVRAprilTagsRawApriltags]
 
 class AVRAprilTagsVisibleApriltagsAbsolutePosition(BaseModel):
     x: float
@@ -598,336 +700,387 @@
 
 class AVRAprilTagsStatus(BaseModel):
     frames_per_second: int = Field(..., ge=0)
     """
     Number of frames of video data processed in the last second
     """
 
+class AVRThermalReadingShapeItem(BaseModel):
+    __root__: int = Field(..., ge=1)
+
+    def __int__(self) -> int:
+        return self.__root__
+
+
 class AVRThermalReading(BaseModel):
     data: str
     """
-    The raw data from the thermal camera are integer values from an 8x8 grid of pixels. This data is then converted into a `bytearray` and base64 encoded. Any example of how to unpack this data:
+    Base64 encoded data of the image. To reconstruct this as a numpy array,
+use `bell.avr.utils.images.deserialize_image` and an `bell.avr.utils.images.ImageData` class.
+Alternatively, manually reconstructing the image is as follows:
 
 ```python
 import base64
-import json
+import zlib
+import numpy as np
+
+image_bytes = base64.b64decode(image_data.encode("utf-8"))
 
-data = json.loads(payload)["data"]
-base64_decoded = data.encode("utf-8")
-as_bytes = base64.b64decode(base64_decoded)
-pixel_ints = list(bytearray(as_bytes))
+if compressed:
+    image_bytes = zlib.decompress(image_bytes)
+
+image_byte_array = bytearray(image_bytes)
+image_array = np.array(image_byte_array)
+
+original_array = np.reshape(image_array, shape)
 ```
 
     """
+    if TYPE_CHECKING:
+        shape: List[int]
+    else:
+        shape: List[AVRThermalReadingShapeItem]
+    """
+    The shape of the image data. For example: [1270, 480, 4] would be a 1270x480 image with 4 channels per pixel.
+    """
+    @validator('shape')
+    def _validate_shape(cls, v) -> list:
+        return _convert_type(v, list, int)
+
+    compressed: bool
+    """
+    Whether or not the image data is zlib compressed.
+    """
 
 class AVRAutonomousBuildingEnable(BaseModel):
     building: int = Field(..., ge=0, le=15)
     """
     Building ID. This is 0-indexed.
     """
 
 class AVRAutonomousBuildingDisable(BaseModel):
     building: int = Field(..., ge=0, le=15)
     """
     Building ID. This is 0-indexed.
     """
 
-class _AVRFCMPositionGlobalCallable(Protocol):
+class _AVRVIOAttitudeEulerRadiansCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionGlobal) -> Any:
+    def __call__(self, payload: AVRVIOAttitudeEulerRadians) -> Any:
         ...
 
-class _AVRVIOAttitudeQuaternionCallable(Protocol):
+class _AVREmptyMessageCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOAttitudeQuaternion) -> Any:
+    def __call__(self) -> Any:
         ...
 
-class _AVRPCMColorSetCallable(Protocol):
+class _AVRFusionCourseCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMColorSet) -> Any:
+    def __call__(self, payload: AVRFusionCourse) -> Any:
         ...
 
-class _AVRVIOResyncCallable(Protocol):
+class _AVRFCMPositionGlobalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOResync) -> Any:
+    def __call__(self, payload: AVRFCMPositionGlobal) -> Any:
         ...
 
-class _AVRFCMAttitudeEulerDegreesCallable(Protocol):
+class _AVRFusionPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMAttitudeEulerDegrees) -> Any:
+    def __call__(self, payload: AVRFusionPositionLocal) -> Any:
         ...
 
-class _AVRFCMAirborneCallable(Protocol):
+class _AVRVIOResyncCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMAirborne) -> Any:
+    def __call__(self, payload: AVRVIOResync) -> Any:
         ...
 
-class _AVRAutonomousBuildingDisableCallable(Protocol):
+class _AVRPCMServoPercentCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAutonomousBuildingDisable) -> Any:
+    def __call__(self, payload: AVRPCMServoPercent) -> Any:
         ...
 
-class _AVRPCMServoAbsoluteCallable(Protocol):
+class _AVRAprilTagsVisibleCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoAbsolute) -> Any:
+    def __call__(self, payload: AVRAprilTagsVisible) -> Any:
         ...
 
-class _AVRFCMPositionLocalCallable(Protocol):
+class _AVRVIOImageStreamEnableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionLocal) -> Any:
+    def __call__(self, payload: AVRVIOImageStreamEnable) -> Any:
         ...
 
-class _AVRFusionGroundspeedCallable(Protocol):
+class _AVRAprilTagsVehiclePositionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionGroundspeed) -> Any:
+    def __call__(self, payload: AVRAprilTagsVehiclePosition) -> Any:
         ...
 
-class _AVRFusionAttitudeEulerRadiansCallable(Protocol):
+class _AVRFusionHeadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionAttitudeEulerRadians) -> Any:
+    def __call__(self, payload: AVRFusionHeading) -> Any:
         ...
 
-class _AVRVIOHeadingCallable(Protocol):
+class _AVRFusionHILGPSMessageCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOHeading) -> Any:
+    def __call__(self, payload: AVRFusionHILGPSMessage) -> Any:
         ...
 
-class _AVRFusionHILGPSMessageCallable(Protocol):
+class _AVRPCMServoAbsoluteCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionHILGPSMessage) -> Any:
+    def __call__(self, payload: AVRPCMServoAbsolute) -> Any:
         ...
 
-class _AVRFCMBatteryCallable(Protocol):
+class _AVRFusionVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMBattery) -> Any:
+    def __call__(self, payload: AVRFusionVelocity) -> Any:
         ...
 
-class _AVRFCMFlightModeCallable(Protocol):
+class _AVRPCMServoCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMFlightMode) -> Any:
+    def __call__(self, payload: AVRPCMServo) -> Any:
         ...
 
-class _AVRFCMGPSInfoCallable(Protocol):
+class _AVRFCMVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMGPSInfo) -> Any:
+    def __call__(self, payload: AVRFCMVelocity) -> Any:
         ...
 
-class _AVRFusionAttitudeQuaternionCallable(Protocol):
+class _AVRVIOImageRequestCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionAttitudeQuaternion) -> Any:
+    def __call__(self, payload: AVRVIOImageRequest) -> Any:
         ...
 
-class _AVRAprilTagsVehiclePositionCallable(Protocol):
+class _AVRPCMColorSetCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsVehiclePosition) -> Any:
+    def __call__(self, payload: AVRPCMColorSet) -> Any:
         ...
 
-class _AVRFCMHILGPSStatsCallable(Protocol):
+class _AVRFusionAttitudeEulerRadiansCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMHILGPSStats) -> Any:
+    def __call__(self, payload: AVRFusionAttitudeEulerRadians) -> Any:
         ...
 
-class _AVRVIOAttitudeEulerRadiansCallable(Protocol):
+class _AVRFusionAttitudeQuaternionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOAttitudeEulerRadians) -> Any:
+    def __call__(self, payload: AVRFusionAttitudeQuaternion) -> Any:
         ...
 
-class _AVRAutonomousBuildingEnableCallable(Protocol):
+class _AVRVIOImageCaptureCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAutonomousBuildingEnable) -> Any:
+    def __call__(self, payload: AVRVIOImageCapture) -> Any:
         ...
 
-class _AVREmptyMessageCallable(Protocol):
+class _AVRFCMAirborneCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self) -> Any:
+    def __call__(self, payload: AVRFCMAirborne) -> Any:
         ...
 
-class _AVRThermalReadingCallable(Protocol):
+class _AVRFCMFlightModeCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRThermalReading) -> Any:
+    def __call__(self, payload: AVRFCMFlightMode) -> Any:
+        ...
+
+class _AVRFusionClimbRateCallable(Protocol):
+    """
+    Class used only for type-hinting MQTT callbacks.
+    """
+    def __call__(self, payload: AVRFusionClimbRate) -> Any:
         ...
 
 class _AVRAprilTagsStatusCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
     def __call__(self, payload: AVRAprilTagsStatus) -> Any:
         ...
 
-class _AVRFusionCourseCallable(Protocol):
+class _AVRVIOHeadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionCourse) -> Any:
+    def __call__(self, payload: AVRVIOHeading) -> Any:
         ...
 
-class _AVRFusionClimbRateCallable(Protocol):
+class _AVRFCMBatteryCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionClimbRate) -> Any:
+    def __call__(self, payload: AVRFCMBattery) -> Any:
         ...
 
-class _AVRFusionPositionLocalCallable(Protocol):
+class _AVRFusionPositionGlobalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionPositionLocal) -> Any:
+    def __call__(self, payload: AVRFusionPositionGlobal) -> Any:
         ...
 
-class _AVRFusionVelocityCallable(Protocol):
+class _AVRPCMServoPWMCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionVelocity) -> Any:
+    def __call__(self, payload: AVRPCMServoPWM) -> Any:
         ...
 
-class _AVRFCMArmedCallable(Protocol):
+class _AVRVIOVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMArmed) -> Any:
+    def __call__(self, payload: AVRVIOVelocity) -> Any:
         ...
 
-class _AVRFusionHeadingCallable(Protocol):
+class _AVRPCMColorTimedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionHeading) -> Any:
+    def __call__(self, payload: AVRPCMColorTimed) -> Any:
         ...
 
-class _AVRVIOPositionLocalCallable(Protocol):
+class _AVRAutonomousBuildingDisableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOPositionLocal) -> Any:
+    def __call__(self, payload: AVRAutonomousBuildingDisable) -> Any:
         ...
 
 class _AVRFCMLandedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
     def __call__(self, payload: AVRFCMLanded) -> Any:
         ...
 
-class _AVRPCMColorTimedCallable(Protocol):
+class _AVRFCMPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMColorTimed) -> Any:
+    def __call__(self, payload: AVRFCMPositionLocal) -> Any:
         ...
 
-class _AVRPCMServoPWMCallable(Protocol):
+class _AVRFCMArmedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoPWM) -> Any:
+    def __call__(self, payload: AVRFCMArmed) -> Any:
         ...
 
-class _AVRVIOConfidenceCallable(Protocol):
+class _AVRFCMHILGPSStatsCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOConfidence) -> Any:
+    def __call__(self, payload: AVRFCMHILGPSStats) -> Any:
         ...
 
-class _AVRPCMServoCallable(Protocol):
+class _AVRVIOAttitudeQuaternionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServo) -> Any:
+    def __call__(self, payload: AVRVIOAttitudeQuaternion) -> Any:
         ...
 
-class _AVRFCMPositionHomeCallable(Protocol):
+class _AVRVIOPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionHome) -> Any:
+    def __call__(self, payload: AVRVIOPositionLocal) -> Any:
         ...
 
-class _AVRFCMVelocityCallable(Protocol):
+class _AVRFCMGPSInfoCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMVelocity) -> Any:
+    def __call__(self, payload: AVRFCMGPSInfo) -> Any:
         ...
 
-class _AVRVIOVelocityCallable(Protocol):
+class _AVRAprilTagsRawCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOVelocity) -> Any:
+    def __call__(self, payload: AVRAprilTagsRaw) -> Any:
         ...
 
-class _AVRAprilTagsVisibleCallable(Protocol):
+class _AVRVIOConfidenceCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsVisible) -> Any:
+    def __call__(self, payload: AVRVIOConfidence) -> Any:
         ...
 
-class _AVRFusionPositionGlobalCallable(Protocol):
+class _AVRThermalReadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionPositionGlobal) -> Any:
+    def __call__(self, payload: AVRThermalReading) -> Any:
         ...
 
-class _AVRPCMServoPercentCallable(Protocol):
+class _AVRFCMPositionHomeCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoPercent) -> Any:
+    def __call__(self, payload: AVRFCMPositionHome) -> Any:
         ...
 
-class _AVRAprilTagsRawCallable(Protocol):
+class _AVRFusionGroundspeedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsRaw) -> Any:
+    def __call__(self, payload: AVRFusionGroundspeed) -> Any:
+        ...
+
+class _AVRFCMAttitudeEulerDegreesCallable(Protocol):
+    """
+    Class used only for type-hinting MQTT callbacks.
+    """
+    def __call__(self, payload: AVRFCMAttitudeEulerDegrees) -> Any:
+        ...
+
+class _AVRAutonomousBuildingEnableCallable(Protocol):
+    """
+    Class used only for type-hinting MQTT callbacks.
+    """
+    def __call__(self, payload: AVRAutonomousBuildingEnable) -> Any:
         ...
```

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/mqtt/serializer.py` & `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/serializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+"""
+Using these functions ensure consistent serialization and deserialization of
+MQTT payloads.
+"""
+
 import json
 from typing import Any
 
 import pydantic
 
 from bell.avr.mqtt.constants import MQTTTopicPayload
 from bell.avr.mqtt.payloads import AVREmptyMessage
 
 
 def deserialize_payload(topic: str, payload: bytes) -> Any:
     """
-    Deserializes an MQTT payload bytestring into a pydantic model. If the topic is
-    not know, serialized JSON will be returned.
+    Deserializes an MQTT payload bytes into a pydantic model. If the topic is
+    not known, deserialized JSON will be returned.
 
-    A ValueError will be raised if the payload is not valid JSON.
+    A `ValueError` will be raised if the payload is not valid JSON.
 
-    Additionally, a ValueError will be raised if the given topic is known
+    Additionally, a `ValueError` will be raised if the given topic is known
     and the payload does not match the required schema.
     """
 
     # so json.loads doesn't choke on an empty string
     if payload in {None, "", b""}:
         payload = b"{}"
 
@@ -36,20 +41,20 @@
     # whatever the user gave us
     return payload
 
 
 def serialize_payload(topic: str, payload: Any) -> str:
     """
     Serializes a payload into a string we can send over MQTT. If the topic is
-    not know, serialized JSON will be returned.
+    not known, serialized JSON will be returned.
 
-    A ValueError will be raised if the payload is a string or byte string
+    A `ValueError` will be raised if the payload is a string or bytes
     and is not valid JSON.
 
-    Additionally, a ValueError will be raised if the given topic is known
+    Additionally, a `ValueError` will be raised if the given topic is known
     and the payload does not match the required schema.
     """
 
     # if no payload given, use empty message
     if payload in [None, "", b"", {}]:
         payload = AVREmptyMessage()
 
@@ -71,8 +76,8 @@
             payload = MQTTTopicPayload[topic](**payload)
 
     # convert pydantic models to json
     if isinstance(payload, pydantic.BaseModel):
         return payload.json()
 
     # convert any other data type to json
-    return json.dumps(payload)
+    return json.dumps(payload)
```

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/serial/pcc.py` & `bell_avr_libraries-0.2.0a1/bell/avr/serial/pcc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,46 @@
 import ctypes
 from struct import pack
 from typing import Any, List, Literal, Optional, Tuple, Union
 
-from loguru import logger
-
 import serial
+from loguru import logger
 
 
 class PeripheralControlComputer:
+    """
+    The `PeripheralControlComputer` class sends serial messages
+    to the AVR peripheral control computer, via easy-to-use class methods.
+
+    The class must be initialized with a
+    [`pyserial`](https://pypi.org/project/pyserial/)
+    [`serial.Serial`](https://pythonhosted.org/pyserial/pyserial_api.html#serial.Serial)
+    or `bell.avr.serial.client.SerialLoop` class instance.
+
+    Example:
+
+    ```python
+    import bell.avr.serial.client
+    import bell.avr.serial.pcc
+    import threading
+
+    client = bell.avr.serial.client.SerialLoop()
+    client.port = port
+    client.baudrate = baudrate
+    client.open()
+
+    pcc = bell.avr.serial.pcc.PeripheralControlComputer(client)
+
+    client_thread = threading.Thread(target=client.run)
+    client_thread.start()
+
+    pcc.set_servo_max(0, 100)
+    ```
+    """
+
     def __init__(self, ser: serial.Serial) -> None:
         self.ser = ser
 
         self.PREAMBLE = (0x24, 0x50)
 
         self.HEADER_OUTGOING = (*self.PREAMBLE, 0x3C)
         self.HEADER_INCOMING = (*self.PREAMBLE, 0x3E)
@@ -30,14 +59,18 @@
             "RESET_AVR_PERIPH",
             "CHECK_SERVO_CONTROLLER",
         ]
 
         self.shutdown: bool = False
 
     def set_base_color(self, wrgb: Tuple[int, int, int, int]) -> None:
+        """
+        Set the color of the LED strip. Expects a tuple of 4 integers between
+        0 and 255, inclusive. This is in the White, Red, Green, Blue format.
+        """
         command = self.commands.index("SET_BASE_COLOR")
         wrgb_l = list(wrgb)
 
         # wrgb + code = 5
         if len(wrgb_l) != 4:
             wrgb_l = [0, 0, 0, 0]
 
@@ -47,38 +80,51 @@
 
         data = self._construct_payload(command, 1 + len(wrgb_l), wrgb_l)
 
         logger.debug(f"Setting base color: {data}")
         self.ser.write(data)
 
     def set_temp_color(
-        self, wrgb: Tuple[int, int, int, int], time: float = 0.5
+        self, wrgb: Tuple[int, int, int, int], duration: float = 0.5
     ) -> None:
+        """
+        Set the color of the LED strip for a specific duration.
+        Expects a tuple of 4 integers between
+        0 and 255, inclusive. This is in the White, Red, Green, Blue format.
+
+        Duration defaults to 0.5 seconds if not given.
+        """
+
         command = self.commands.index("SET_TEMP_COLOR")
         wrgb_l = list(wrgb)
 
         # wrgb + code = 5
         if len(wrgb_l) != 4:
             wrgb_l = [0, 0, 0, 0]
 
         for i, color in enumerate(wrgb_l):
             if not isinstance(color, int) or color > 255 or color < 0:
                 wrgb_l[i] = 0
 
-        time_bytes = self.list_pack("<f", time)
+        time_bytes = self._list_pack("<f", duration)
         data = self._construct_payload(
             command, 1 + len(wrgb) + len(wrgb_l), wrgb_l + time_bytes
         )
 
         logger.debug(f"Setting temp color: {data}")
         self.ser.write(data)
 
     def set_servo_open_close(
         self, servo: int, action: Literal["open", "close"]
     ) -> None:
+        """
+        Opens or closes a servo. Expects the 0-indexed servo ID and the
+        action to perform.
+        """
+
         valid_command = False
 
         command = self.commands.index("SET_SERVO_OPEN_CLOSE")
         data = []
 
         # 128 is inflection point, over 128 == open; under 128 == close
 
@@ -96,14 +142,19 @@
         length = 3
         data = self._construct_payload(command, length, data)
 
         logger.debug(f"Setting servo open/close: {data}")
         self.ser.write(data)
 
     def set_servo_min(self, servo: int, minimum: float) -> None:
+        """
+        Sets the minimum pulse width of a servo. Expects the 0-indexed servo ID and
+        the minimum pulse width between 0 and 1000 non-inclusive.
+        """
+
         valid_command = False
 
         command = self.commands.index("SET_SERVO_MIN")
         data = []
 
         if isinstance(minimum, (float, int)) and minimum < 1000 and minimum > 0:
             valid_command = True
@@ -115,14 +166,19 @@
         length = 3
         data = self._construct_payload(command, length, data)
 
         logger.debug(f"Setting servo min: {data}")
         self.ser.write(data)
 
     def set_servo_max(self, servo: int, maximum: float) -> None:
+        """
+        Sets the maximum pulse width of a servo. Expects the 0-indexed servo ID and
+        the maximum pulse width between 0 and 1000 non-inclusive.
+        """
+
         valid_command = False
 
         command = self.commands.index("SET_SERVO_MAX")
         data = []
 
         if isinstance(maximum, (float, int)) and maximum < 1000 and maximum > 0:
             valid_command = True
@@ -134,14 +190,19 @@
         length = 3
         data = self._construct_payload(command, length, data)
 
         logger.debug(f"Setting servo max: {data}")
         self.ser.write(data)
 
     def set_servo_pct(self, servo: int, pct: int) -> None:
+        """
+        Sets the percentage open of a servo. Expects the 0-indexed servo ID and
+        the percentage open between 0 and 100 inclusive.
+        """
+
         valid_command = False
 
         command = self.commands.index("SET_SERVO_PCT")
         data = []
 
         if isinstance(pct, (float, int)) and pct <= 100 and pct >= 0:
             valid_command = True
@@ -153,14 +214,19 @@
         length = 3
         data = self._construct_payload(command, length, data)
 
         logger.debug(f"Setting servo percent: {data}")
         self.ser.write(data)
 
     def set_servo_abs(self, servo: int, absolute: int) -> None:
+        """
+        Sets the absolute position of a servo. Expects the 0-indexed servo ID and
+        the absolute position.
+        """
+
         valid_command = False
 
         command = self.commands.index("SET_SERVO_ABS")
         data = []
 
         if isinstance(absolute, int):
             uint16_absolute = ctypes.c_uint16(absolute).value
@@ -175,32 +241,43 @@
         length = 4
         data = self._construct_payload(command, length, data)
 
         logger.debug(f"Setting servo absolute: {data}")
         self.ser.write(data)
 
     def fire_laser(self) -> None:
+        """
+        Fires the laser for a 0.25 second pulse. Has a cooldown of 0.5 seconds.
+        """
+
         command = self.commands.index("FIRE_LASER")
 
         length = 1
         data = self._construct_payload(command, length)
 
         logger.debug(f"Setting the laser on: {data}")
         self.ser.write(data)
 
     def set_laser_on(self) -> None:
+        """
+        Turns laser on for 0.1 second every 0.5 seconds.
+        """
+
         command = self.commands.index("SET_LASER_ON")
 
         length = 1
         data = self._construct_payload(command, length)
 
         logger.debug(f"Setting the laser on: {data}")
         self.ser.write(data)
 
     def set_laser_off(self) -> None:
+        """
+        Turns the laser off. Does not prevent `fire_laser`.
+        """
         command = self.commands.index("SET_LASER_OFF")
 
         length = 1
         data = self._construct_payload(command, length)
 
         logger.debug(f"Setting the laser off: {data}")
         self.ser.write(data)
@@ -215,14 +292,17 @@
     #     self.ser.write(data)
 
     #     self.ser.close()
     #     time.sleep(5)
     #     self.ser.open()
 
     def check_servo_controller(self) -> None:
+        """
+        Checks the servo controller.
+        """
         command = self.commands.index("CHECK_SERVO_CONTROLLER")
 
         length = 1
         data = self._construct_payload(command, length)
 
         logger.debug(f"Checking servo controller: {data}")
         self.ser.write(data)
@@ -242,28 +322,32 @@
             ("<B", [code]),
             ("<%dB" % len(data), data),
         )
 
         for section in new_data:
             payload += pack(section[0], *section[1])
 
-        crc = self.calc_crc(payload, len(payload))
+        crc = self._calc_crc(payload, len(payload))
 
         payload += pack("<B", crc)
 
         return payload
 
-    def list_pack(self, bit_format: Union[str, bytes], value: Any) -> List[int]:
+    def _list_pack(self, bit_format: Union[str, bytes], value: Any) -> List[int]:
         return list(pack(bit_format, value))
 
-    def crc8_dvb_s2(self, crc: int, a: int) -> int:
+    def _crc8_dvb_s2(self, crc: int, a: int) -> int:
         # https://stackoverflow.com/a/52997726
         crc ^= a
         for _ in range(8):
             crc = ((crc << 1) ^ 0xD5) % 256 if crc & 0x80 else (crc << 1) % 256
         return crc
 
-    def calc_crc(self, string: bytes, length: int) -> int:
+    def _calc_crc(self, string: bytes, length: int) -> int:
+        """
+        Calculates the crc for an input.
+        """
+
         crc = 0
         for i in range(length):
-            crc = self.crc8_dvb_s2(crc, string[i])
+            crc = self._crc8_dvb_s2(crc, string[i])
         return crc
```

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/utils/testing.py` & `bell_avr_libraries-0.2.0a1/bell/avr/utils/testing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from functools import wraps
 from typing import Any, Callable
 
 
 def dont_run_forever(*args, **kwargs) -> Callable:
     """
-    Decorator to overwrite the `run_forever` decorator when writing tests.
+    Decorator to overwrite the `bell.avr.utils.decorators.run_forever` decorator when writing tests.
     Use like so:
 
     ```python
+    # pip install pytest-mock
+
     from bell.avr.utils.testing import dont_run_forever
-    mocker.patch("bell.avr.utils.decorators.run_forever", dont_run_forever)
+    from pytest_mock.plugin import MockerFixture
+
+    def test_function(mocker: MockerFixture):
+        mocker.patch("bell.avr.utils.decorators.run_forever", dont_run_forever)
     ```
     """
 
     def decorator(f: Callable) -> Callable:
         @wraps(f)
         def wrapper(*args, **kwargs) -> Any:
             return f(*args, **kwargs)
```

### Comparing `bell_avr_libraries-0.2.0a0/bell/avr/utils/timing.py` & `bell_avr_libraries-0.2.0a1/bell/avr/utils/timing.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,28 @@
 
 def rate_limit(
     fun: Callable, period: Optional[float] = None, frequency: Optional[float] = None
 ) -> None:
     """
     Run the given callable every `period` seconds, or `frequency` times per second.
     Either `period` or `frequency` must be set.
+
+    Example:
+
+    ```python
+    for _ in range(10):
+        # add() will only run twice
+        timing.rate_limit(add, period=5)
+        time.sleep(1)
+    ```
+
+    This works by tracking calls to the `rate_limit` function from a line number
+    within a file, so multiple calls to `rate_limit` say within a loop
+    with the same callable and period will be treated separately. This allows
+    for dynamic frequency manipulation.
     """
     if frequency is not None:
         period = 1 / frequency
 
     assert period is not None
 
     # in order to allow dynamic rate limits, record things based on the
```

### Comparing `bell_avr_libraries-0.2.0a0/pyproject.toml` & `bell_avr_libraries-0.2.0a1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
     name = "bell-avr-libraries"
-    version = "0.2.0a0"
+    version = "0.2.0a1"
     description = "Common Python libraries used by parts of Bell AVR"
     license = "MIT"
     readme = "README.md"
-    homepage = "https://github.com/bellflight/AVR-Python-Libraries"
+    homepage = "https://roboticseducation.org/bell-advanced-vertical-robotics/"
+    repository = "https://github.com/bellflight/AVR-Python-Libraries"
+    documentation = "https://bellflight.github.io/AVR-Python-Libraries"
     authors = [
         "Chris Padilla <cpadilla@bellflight.com>",
         "Nathan Vaughn <nvaughn51@gmail.com>",
     ]
     packages = [{ include = "bell/avr" }]
     exclude = [
         "bell/**/*.j2",
@@ -17,36 +19,38 @@
         "bell/**/*.yml",
         "bell/**/.gitignore",
     ]
     include = ["bell/**/*.pyi", "bell/**/*.py"]
 
 [tool.poetry.dependencies]
     python             = ">=3.8,<3.12"
-    loguru             = "^0.6.0"
+    loguru             = ">=0.6,<0.8"
     pydantic           = "^1.10.2"
     paho-mqtt          = "^1.6.1"
+    numpy              = "^1.24.3"
     pyserial           = { version = "^3.5", optional = true }
     pyside6-essentials = { version = "^6.4.2", optional = true }
 
 [tool.poetry.extras]
     serial = ["pyserial"]
     qt     = ["pyside6-essentials"]
 
 [tool.poetry.group.dev.dependencies]
     # testing
     pytest       = "^7.2.0"
     pytest-xdist = "^3.0.2"
     pytest-mock  = "^3.10.0"
     pytest-cov   = "^4.0.0"
-    pre-commit   = "^2.21.0"
+    pre-commit   = ">=2.21,<4.0"
     # building template
     Jinja2  = "^3.1.2"
     jsonref = "^1.0.1"
     pyyaml  = "^6.0"
     tomli   = { version = "^2.0.1", python = "<3.11" }
+    pdoc    = "^13.1.1"
 
 [tool.pyright]
     typeCheckingMode = "basic"
     venvPath         = "."
     venv             = ".venv"
 
 [tool.ruff]
```

