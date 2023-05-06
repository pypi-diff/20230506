# Comparing `tmp/bell_avr_libraries-0.2.0a1.tar.gz` & `tmp/bell_avr_libraries-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bell_avr_libraries-0.2.0a1.tar", max compression
+gzip compressed data, was "bell_avr_libraries-0.2.0a2.tar", max compression
```

## Comparing `bell_avr_libraries-0.2.0a1.tar` & `bell_avr_libraries-0.2.0a2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/LICENSE
--rw-r--r--   0        0        0     1938 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/README.md
--rw-r--r--   0        0        0      444 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/__init__.py
--rw-r--r--   0        0        0      289 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/__init__.py
--rw-r--r--   0        0        0     5158 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/client.py
--rw-r--r--   0        0        0    23002 2023-05-06 02:54:35.904636 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/constants.py
--rw-r--r--   0        0        0      584 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/dispatcher.py
--rw-r--r--   0        0        0    15050 2023-05-06 02:54:35.900636 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/module.py
--rw-r--r--   0        0        0    27660 2023-05-06 02:54:35.892636 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/payloads.py
--rw-r--r--   0        0        0    12127 2023-05-06 02:54:35.908636 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/qt_widget.py
--rw-r--r--   0        0        0     2534 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/mqtt/serializer.py
--rw-r--r--   0        0        0      124 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/serial/__init__.py
--rw-r--r--   0        0        0      746 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/serial/client.py
--rw-r--r--   0        0        0    10089 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/serial/pcc.py
--rw-r--r--   0        0        0      935 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/serial/ports.py
--rw-r--r--   0        0        0      206 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/__init__.py
--rw-r--r--   0        0        0     3076 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/decorators.py
--rw-r--r--   0        0        0     1070 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/env.py
--rw-r--r--   0        0        0     2890 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/images.py
--rw-r--r--   0        0        0      726 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/testing.py
--rw-r--r--   0        0        0     1494 2023-05-06 02:54:12.456395 bell_avr_libraries-0.2.0a1/bell/avr/utils/timing.py
--rw-r--r--   0        0        0     1805 2023-05-06 02:54:12.460394 bell_avr_libraries-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     3058 1970-01-01 00:00:00.000000 bell_avr_libraries-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0     1938 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/README.md
+-rw-r--r--   0        0        0      444 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/__init__.py
+-rw-r--r--   0        0        0      289 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/__init__.py
+-rw-r--r--   0        0        0     8330 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/client.py
+-rw-r--r--   0        0        0    23046 2023-05-06 14:31:47.295250 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/constants.py
+-rw-r--r--   0        0        0      588 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/dispatcher.py
+-rw-r--r--   0        0        0    15050 2023-05-06 14:31:47.287250 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/module.py
+-rw-r--r--   0        0        0    28762 2023-05-06 14:31:47.275250 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/payloads.py
+-rw-r--r--   0        0        0    12127 2023-05-06 14:31:47.303250 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/qt_widget.py
+-rw-r--r--   0        0        0     2534 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/mqtt/serializer.py
+-rw-r--r--   0        0        0      124 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/serial/__init__.py
+-rw-r--r--   0        0        0      746 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/serial/client.py
+-rw-r--r--   0        0        0    10089 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/serial/pcc.py
+-rw-r--r--   0        0        0      935 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/serial/ports.py
+-rw-r--r--   0        0        0      206 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/__init__.py
+-rw-r--r--   0        0        0     3076 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/decorators.py
+-rw-r--r--   0        0        0     1070 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/env.py
+-rw-r--r--   0        0        0     2890 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/images.py
+-rw-r--r--   0        0        0      726 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/testing.py
+-rw-r--r--   0        0        0     1494 2023-05-06 14:31:27.043231 bell_avr_libraries-0.2.0a2/bell/avr/utils/timing.py
+-rw-r--r--   0        0        0     1805 2023-05-06 14:31:27.047232 bell_avr_libraries-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3058 1970-01-01 00:00:00.000000 bell_avr_libraries-0.2.0a2/PKG-INFO
```

### Comparing `bell_avr_libraries-0.2.0a1/LICENSE` & `bell_avr_libraries-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/README.md` & `bell_avr_libraries-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/constants.py` & `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,9 +544,9 @@
     "avr/autonomous/enable": AVREmptyMessage,
     "avr/autonomous/disable": AVREmptyMessage,
     "avr/autonomous/building/enable": AVRAutonomousBuildingEnable,
     "avr/autonomous/building/disable": AVRAutonomousBuildingDisable,
 }
 """
 Complete dictionary with topics as keys, and the associated payload class type
-as values.
+as values. This is used in `bell.avr.mqtt.serializer`.
 """
```

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/dispatcher.py` & `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def dispatch_message(
     topic_callbacks: _MQTTTopicCallableTypedDict, topic: str, payload: Any
 ) -> None:
     """
     Given a dictionary of topics and callbacks,
-    this executes appropriate callback with the correct arguments.
+    this executes the appropriate callback with the correct arguments.
     """
     if topic not in topic_callbacks:
         return
 
     # execute callback
     if isinstance(payload, AVREmptyMessage):
         topic_callbacks[topic]()
```

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/module.py` & `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/module.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/payloads.py` & `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/payloads.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 
 """
 These are Python classes for MQTT message payloads.
 As AVR exclusively uses JSON, these are all [Pydantic](https://docs.pydantic.dev/)
 classes that have all of the required fields for a message.
 
 This is a Python implementation of the AVR [AsyncAPI definition](../mqtt/asyncapi).
+
 Example:
 
 ```python
 from bell.avr.mqtt.payloads import AVRPCMColorSet
 
 payload = AVRPCMColorSet(wrgb=(128, 232, 142, 0))```
+Some of the Python documentation does not get generated correctly,
+please refer to the above AsyncAPI definition, or the "View Source" dropdowns
+on the right side.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Literal, Optional, Protocol, Tuple, Type, Union, overload
 
 from pydantic import BaseModel as PydanticBaseModel
@@ -43,16 +47,19 @@
 
 
 class BaseModel(PydanticBaseModel):
     class Config:
         'For [Pydantic configuration](https://docs.pydantic.dev/latest/usage/model_config/), please ignore.'
         extra = Extra.forbid
 
-
 class AVREmptyMessage(BaseModel):
+    """
+    This is an empty class to be used with topics with no payload. When data is sent on a topic that expects `AVREmptyMessage`, an empty string, or an empty dict (`{}`) are both acceptable.
+    """
+
     pass
 
 class AVRPCMColorSetWrgbItem(BaseModel):
     __root__: int = Field(..., ge=0, le=255)
 
     def __int__(self) -> int:
         return self.__root__
@@ -168,28 +175,36 @@
 class AVRFCMFlightMode(BaseModel):
     flight_mode: Literal["UNKNOWN", "READY", "TAKEOFF", "HOLD", "MISSION", "RETURN_TO_LAUNCH", "LAND", "OFFBOARD", "FOLLOW_ME", "MANUAL", "ALTCTL", "POSCTL", "ACRO", "STABILIZED", "RATTITUDE"]
     """
     Active flight mode
     """
 
 class AVRFCMPositionLocal(BaseModel):
+    """
+    The local position of the drone.
+    """
+
     n: float
     """
     X position in a North/East/Down coordinate system in meters.
     """
     e: float
     """
     Y position in a North/East/Down coordinate system in meters.
     """
     d: float
     """
     Z position in a North/East/Down coordinate system in meters.
     """
 
 class AVRFCMPositionGlobal(BaseModel):
+    """
+    The global position of the drone.
+    """
+
     lat: float = Field(..., ge=-90, le=90)
     """
     Latitude in degrees.
     """
     lon: float = Field(..., ge=-180, le=180)
     """
     Longitude in degrees.
@@ -252,14 +267,18 @@
     """
     fix_type: Literal["NO_GPS", "NO_FIX", "FIX_2D", "FIX_3D", "FIX_DGPS", "RTK_FLOAT", "RTK_FIXED"]
     """
     GPS fix type
     """
 
 class AVRFusionPositionLocal(BaseModel):
+    """
+    The local position of the drone.
+    """
+
     n: float
     """
     X position in a North/East/Down coordinate system in meters.
     """
     e: float
     """
     Y position in a North/East/Down coordinate system in meters.
@@ -280,14 +299,18 @@
     """
     Vd: float
     """
     Z velocity in a North/East/Down coordinate system in meters per second.
     """
 
 class AVRFusionPositionGlobal(BaseModel):
+    """
+    The global position of the drone.
+    """
+
     lat: float = Field(..., ge=-90, le=90)
     """
     Latitude in degrees.
     """
     lon: float = Field(..., ge=-180, le=180)
     """
     Longitude in degrees.
@@ -408,14 +431,18 @@
     """
     heading: int
     """
     Custom heading field. This is the heading in degrees * 100.
     """
 
 class AVRVIOResync(BaseModel):
+    """
+    Position *difference* of the drone, from where the drone thinks it is, to where it really is.
+    """
+
     hdg: float
     """
     Heading in degrees.
     """
     n: float
     """
     X position in a North/East/Down coordinate system in meters.
@@ -426,14 +453,18 @@
     """
     d: float
     """
     Z position in a North/East/Down coordinate system in meters.
     """
 
 class AVRVIOPositionLocal(BaseModel):
+    """
+    Local position of the drone.
+    """
+
     n: float
     """
     X position in a North/East/Down coordinate system in meters.
     """
     e: float
     """
     Y position in a North/East/Down coordinate system in meters.
@@ -573,14 +604,18 @@
     """
     frequency: float = Field(..., gt=0, le=5)
     """
     At what rate should new images be sent (frames per second).
     """
 
 class AVRAprilTagsVehiclePosition(BaseModel):
+    """
+    Position of the drone relative to the world origin in world frame.
+    """
+
     tag_id: int = Field(..., ge=0)
     """
     AprilTag ID.
     """
     x: float
     """
     X position in a North/East/Down coordinate system in centimeters.
@@ -634,28 +669,36 @@
         return _convert_type(v, tuple, float)
 
 
 class AVRAprilTagsRaw(BaseModel):
     apriltags: List[AVRAprilTagsRawApriltags]
 
 class AVRAprilTagsVisibleApriltagsAbsolutePosition(BaseModel):
+    """
+    The position of the drone in world frame in centimeters. If the tag has no truth data, this will not be present in the output.
+    """
+
     x: float
     """
     X position in a North/East/Down coordinate system in centimeters.
     """
     y: float
     """
     Y position in a North/East/Down coordinate system in centimeters.
     """
     z: float
     """
     Z position in a North/East/Down coordinate system in centimeters.
     """
 
 class AVRAprilTagsVisibleApriltagsRelativePosition(BaseModel):
+    """
+    The relative position of the drone relative to the AprilTag in world frame in centimeters.
+    """
+
     x: float
     """
     X position in a North/East/Down coordinate system in centimeters.
     """
     y: float
     """
     Y position in a North/East/Down coordinate system in centimeters.
@@ -759,328 +802,328 @@
 
 class AVRAutonomousBuildingDisable(BaseModel):
     building: int = Field(..., ge=0, le=15)
     """
     Building ID. This is 0-indexed.
     """
 
-class _AVRVIOAttitudeEulerRadiansCallable(Protocol):
+class _AVRPCMColorSetCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOAttitudeEulerRadians) -> Any:
+    def __call__(self, payload: AVRPCMColorSet) -> Any:
         ...
 
-class _AVREmptyMessageCallable(Protocol):
+class _AVRFCMPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self) -> Any:
+    def __call__(self, payload: AVRFCMPositionLocal) -> Any:
         ...
 
-class _AVRFusionCourseCallable(Protocol):
+class _AVRFCMLandedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionCourse) -> Any:
+    def __call__(self, payload: AVRFCMLanded) -> Any:
         ...
 
-class _AVRFCMPositionGlobalCallable(Protocol):
+class _AVRPCMServoPercentCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionGlobal) -> Any:
+    def __call__(self, payload: AVRPCMServoPercent) -> Any:
         ...
 
-class _AVRFusionPositionLocalCallable(Protocol):
+class _AVRFusionGroundspeedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionPositionLocal) -> Any:
+    def __call__(self, payload: AVRFusionGroundspeed) -> Any:
         ...
 
-class _AVRVIOResyncCallable(Protocol):
+class _AVRFCMFlightModeCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOResync) -> Any:
+    def __call__(self, payload: AVRFCMFlightMode) -> Any:
         ...
 
-class _AVRPCMServoPercentCallable(Protocol):
+class _AVRFusionPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoPercent) -> Any:
+    def __call__(self, payload: AVRFusionPositionLocal) -> Any:
         ...
 
-class _AVRAprilTagsVisibleCallable(Protocol):
+class _AVRFusionHeadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsVisible) -> Any:
+    def __call__(self, payload: AVRFusionHeading) -> Any:
         ...
 
-class _AVRVIOImageStreamEnableCallable(Protocol):
+class _AVRFCMPositionHomeCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageStreamEnable) -> Any:
+    def __call__(self, payload: AVRFCMPositionHome) -> Any:
         ...
 
-class _AVRAprilTagsVehiclePositionCallable(Protocol):
+class _AVRFCMGPSInfoCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsVehiclePosition) -> Any:
+    def __call__(self, payload: AVRFCMGPSInfo) -> Any:
         ...
 
-class _AVRFusionHeadingCallable(Protocol):
+class _AVRFCMAttitudeEulerDegreesCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionHeading) -> Any:
+    def __call__(self, payload: AVRFCMAttitudeEulerDegrees) -> Any:
         ...
 
-class _AVRFusionHILGPSMessageCallable(Protocol):
+class _AVRFusionClimbRateCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionHILGPSMessage) -> Any:
+    def __call__(self, payload: AVRFusionClimbRate) -> Any:
         ...
 
-class _AVRPCMServoAbsoluteCallable(Protocol):
+class _AVRFCMHILGPSStatsCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoAbsolute) -> Any:
+    def __call__(self, payload: AVRFCMHILGPSStats) -> Any:
         ...
 
-class _AVRFusionVelocityCallable(Protocol):
+class _AVRAprilTagsRawCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionVelocity) -> Any:
+    def __call__(self, payload: AVRAprilTagsRaw) -> Any:
         ...
 
-class _AVRPCMServoCallable(Protocol):
+class _AVRAprilTagsVisibleCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServo) -> Any:
+    def __call__(self, payload: AVRAprilTagsVisible) -> Any:
         ...
 
-class _AVRFCMVelocityCallable(Protocol):
+class _AVRVIOHeadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMVelocity) -> Any:
+    def __call__(self, payload: AVRVIOHeading) -> Any:
         ...
 
-class _AVRVIOImageRequestCallable(Protocol):
+class _AVRVIOAttitudeEulerRadiansCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageRequest) -> Any:
+    def __call__(self, payload: AVRVIOAttitudeEulerRadians) -> Any:
         ...
 
-class _AVRPCMColorSetCallable(Protocol):
+class _AVRFusionVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMColorSet) -> Any:
+    def __call__(self, payload: AVRFusionVelocity) -> Any:
         ...
 
-class _AVRFusionAttitudeEulerRadiansCallable(Protocol):
+class _AVRVIOAttitudeQuaternionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionAttitudeEulerRadians) -> Any:
+    def __call__(self, payload: AVRVIOAttitudeQuaternion) -> Any:
         ...
 
-class _AVRFusionAttitudeQuaternionCallable(Protocol):
+class _AVRAutonomousBuildingEnableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionAttitudeQuaternion) -> Any:
+    def __call__(self, payload: AVRAutonomousBuildingEnable) -> Any:
         ...
 
-class _AVRVIOImageCaptureCallable(Protocol):
+class _AVRVIOResyncCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageCapture) -> Any:
+    def __call__(self, payload: AVRVIOResync) -> Any:
         ...
 
-class _AVRFCMAirborneCallable(Protocol):
+class _AVRVIOImageStreamEnableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMAirborne) -> Any:
+    def __call__(self, payload: AVRVIOImageStreamEnable) -> Any:
         ...
 
-class _AVRFCMFlightModeCallable(Protocol):
+class _AVRFCMVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMFlightMode) -> Any:
+    def __call__(self, payload: AVRFCMVelocity) -> Any:
         ...
 
-class _AVRFusionClimbRateCallable(Protocol):
+class _AVRFCMPositionGlobalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionClimbRate) -> Any:
+    def __call__(self, payload: AVRFCMPositionGlobal) -> Any:
         ...
 
-class _AVRAprilTagsStatusCallable(Protocol):
+class _AVRVIOImageRequestCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsStatus) -> Any:
+    def __call__(self, payload: AVRVIOImageRequest) -> Any:
         ...
 
-class _AVRVIOHeadingCallable(Protocol):
+class _AVRFCMArmedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOHeading) -> Any:
+    def __call__(self, payload: AVRFCMArmed) -> Any:
         ...
 
-class _AVRFCMBatteryCallable(Protocol):
+class _AVRAprilTagsStatusCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMBattery) -> Any:
+    def __call__(self, payload: AVRAprilTagsStatus) -> Any:
         ...
 
-class _AVRFusionPositionGlobalCallable(Protocol):
+class _AVRPCMColorTimedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionPositionGlobal) -> Any:
+    def __call__(self, payload: AVRPCMColorTimed) -> Any:
         ...
 
-class _AVRPCMServoPWMCallable(Protocol):
+class _AVRFusionHILGPSMessageCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoPWM) -> Any:
+    def __call__(self, payload: AVRFusionHILGPSMessage) -> Any:
         ...
 
-class _AVRVIOVelocityCallable(Protocol):
+class _AVRAutonomousBuildingDisableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOVelocity) -> Any:
+    def __call__(self, payload: AVRAutonomousBuildingDisable) -> Any:
         ...
 
-class _AVRPCMColorTimedCallable(Protocol):
+class _AVRFusionCourseCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMColorTimed) -> Any:
+    def __call__(self, payload: AVRFusionCourse) -> Any:
         ...
 
-class _AVRAutonomousBuildingDisableCallable(Protocol):
+class _AVRFusionAttitudeQuaternionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAutonomousBuildingDisable) -> Any:
+    def __call__(self, payload: AVRFusionAttitudeQuaternion) -> Any:
         ...
 
-class _AVRFCMLandedCallable(Protocol):
+class _AVRVIOConfidenceCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMLanded) -> Any:
+    def __call__(self, payload: AVRVIOConfidence) -> Any:
         ...
 
-class _AVRFCMPositionLocalCallable(Protocol):
+class _AVRPCMServoAbsoluteCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionLocal) -> Any:
+    def __call__(self, payload: AVRPCMServoAbsolute) -> Any:
         ...
 
-class _AVRFCMArmedCallable(Protocol):
+class _AVRAprilTagsVehiclePositionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMArmed) -> Any:
+    def __call__(self, payload: AVRAprilTagsVehiclePosition) -> Any:
         ...
 
-class _AVRFCMHILGPSStatsCallable(Protocol):
+class _AVRVIOImageCaptureCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMHILGPSStats) -> Any:
+    def __call__(self, payload: AVRVIOImageCapture) -> Any:
         ...
 
-class _AVRVIOAttitudeQuaternionCallable(Protocol):
+class _AVRFusionPositionGlobalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOAttitudeQuaternion) -> Any:
+    def __call__(self, payload: AVRFusionPositionGlobal) -> Any:
         ...
 
 class _AVRVIOPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
     def __call__(self, payload: AVRVIOPositionLocal) -> Any:
         ...
 
-class _AVRFCMGPSInfoCallable(Protocol):
+class _AVRThermalReadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMGPSInfo) -> Any:
+    def __call__(self, payload: AVRThermalReading) -> Any:
         ...
 
-class _AVRAprilTagsRawCallable(Protocol):
+class _AVRFCMAirborneCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsRaw) -> Any:
+    def __call__(self, payload: AVRFCMAirborne) -> Any:
         ...
 
-class _AVRVIOConfidenceCallable(Protocol):
+class _AVRFCMBatteryCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOConfidence) -> Any:
+    def __call__(self, payload: AVRFCMBattery) -> Any:
         ...
 
-class _AVRThermalReadingCallable(Protocol):
+class _AVRPCMServoCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRThermalReading) -> Any:
+    def __call__(self, payload: AVRPCMServo) -> Any:
         ...
 
-class _AVRFCMPositionHomeCallable(Protocol):
+class _AVRVIOVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionHome) -> Any:
+    def __call__(self, payload: AVRVIOVelocity) -> Any:
         ...
 
-class _AVRFusionGroundspeedCallable(Protocol):
+class _AVREmptyMessageCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionGroundspeed) -> Any:
+    def __call__(self) -> Any:
         ...
 
-class _AVRFCMAttitudeEulerDegreesCallable(Protocol):
+class _AVRPCMServoPWMCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMAttitudeEulerDegrees) -> Any:
+    def __call__(self, payload: AVRPCMServoPWM) -> Any:
         ...
 
-class _AVRAutonomousBuildingEnableCallable(Protocol):
+class _AVRFusionAttitudeEulerRadiansCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAutonomousBuildingEnable) -> Any:
+    def __call__(self, payload: AVRFusionAttitudeEulerRadians) -> Any:
         ...
```

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/qt_widget.py` & `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/qt_widget.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/mqtt/serializer.py` & `bell_avr_libraries-0.2.0a2/bell/avr/mqtt/serializer.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/serial/client.py` & `bell_avr_libraries-0.2.0a2/bell/avr/serial/client.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/serial/pcc.py` & `bell_avr_libraries-0.2.0a2/bell/avr/serial/pcc.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/serial/ports.py` & `bell_avr_libraries-0.2.0a2/bell/avr/serial/ports.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/utils/decorators.py` & `bell_avr_libraries-0.2.0a2/bell/avr/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/utils/env.py` & `bell_avr_libraries-0.2.0a2/bell/avr/utils/env.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/utils/images.py` & `bell_avr_libraries-0.2.0a2/bell/avr/utils/images.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/utils/testing.py` & `bell_avr_libraries-0.2.0a2/bell/avr/utils/testing.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/bell/avr/utils/timing.py` & `bell_avr_libraries-0.2.0a2/bell/avr/utils/timing.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a1/pyproject.toml` & `bell_avr_libraries-0.2.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "bell-avr-libraries"
-    version = "0.2.0a1"
+    version = "0.2.0a2"
     description = "Common Python libraries used by parts of Bell AVR"
     license = "MIT"
     readme = "README.md"
     homepage = "https://roboticseducation.org/bell-advanced-vertical-robotics/"
     repository = "https://github.com/bellflight/AVR-Python-Libraries"
     documentation = "https://bellflight.github.io/AVR-Python-Libraries"
     authors = [
```

### Comparing `bell_avr_libraries-0.2.0a1/PKG-INFO` & `bell_avr_libraries-0.2.0a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bell-avr-libraries
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Common Python libraries used by parts of Bell AVR
 Home-page: https://roboticseducation.org/bell-advanced-vertical-robotics/
 License: MIT
 Author: Chris Padilla
 Author-email: cpadilla@bellflight.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

