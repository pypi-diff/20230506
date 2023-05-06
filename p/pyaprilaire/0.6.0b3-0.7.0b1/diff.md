# Comparing `tmp/pyaprilaire-0.6.0b3.tar.gz` & `tmp/pyaprilaire-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaprilaire-0.6.0b3.tar", last modified: Wed May  3 21:05:55 2023, max compression
+gzip compressed data, was "pyaprilaire-0.7.0b1.tar", last modified: Sat May  6 01:10:08 2023, max compression
```

## Comparing `pyaprilaire-0.6.0b3.tar` & `pyaprilaire-0.7.0b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/pyaprilaire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/socket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/tests/test_socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/pyaprilaire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyaprilaire/socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 01:10:08.000000 pyaprilaire-0.7.0b1/pyaprilaire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:08.677856 pyaprilaire-0.7.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-06 01:09:57.000000 pyaprilaire-0.7.0b1/tests/test_socket_client.py
```

### Comparing `pyaprilaire-0.6.0b3/LICENSE` & `pyaprilaire-0.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b3/PKG-INFO` & `pyaprilaire-0.7.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.6.0b3
+Version: 0.7.0b1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.6.0b3/README.md` & `pyaprilaire-0.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b3/pyaprilaire/client.py` & `pyaprilaire-0.7.0b1/pyaprilaire/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import asyncio
 
 from collections.abc import Callable
 from logging import Logger
 from typing import Any
 
-from .const import Action, FunctionalDomain, QUEUE_FREQUENCY
+from .const import Action, Attribute, FunctionalDomain, QUEUE_FREQUENCY
 from .packet import NackPacket, Packet
 from .socket_client import SocketClient
 
 
 class _AprilaireClientProtocol(asyncio.Protocol):
     """Protocol for interacting with the thermostat over socket connection"""
 
@@ -121,25 +121,25 @@
 
             if isinstance(packet, NackPacket):
                 self.logger.error(
                     "Received NACK for attribute %d", packet.nack_attribute
                 )
                 continue
 
-            if "error" in packet.data:
-                error = packet.data["error"]
+            if Attribute.ERROR in packet.data:
+                error = packet.data[Attribute.ERROR]
 
                 if error != 0:
                     self.logger.error("Thermostat error: %d", error)
 
             if (
                 packet.action == Action.COS
                 and packet.functional_domain == FunctionalDomain.CONTROL
                 and packet.attribute == 1
-                and packet.data.get("mode") == 1
+                and packet.data.get(Attribute.MODE) == 1
             ):
                 self.logger.info("Re-reading control because of COS with mode==1")
 
                 asyncio.ensure_future(self.read_control())
 
                 continue
 
@@ -153,15 +153,15 @@
     def connection_lost(self, exc: Exception | None) -> None:
         """Called when the connection to the socket has been lost"""
         self.logger.info("Aprilaire connection lost")
 
         if self.data_received_callback:
             asyncio.ensure_future(
                 self.data_received_callback(
-                    FunctionalDomain.NONE, 0, {"available": False}
+                    FunctionalDomain.NONE, 0, {Attribute.AVAILABLE: False}
                 )
             )
 
         self.transport = None
 
         if self.reconnect_action:
             asyncio.ensure_future(self.reconnect_action())
@@ -188,34 +188,34 @@
         """Send a request to update the mode"""
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": mode,
-                    "fan_mode": 0,
-                    "heat_setpoint": 0,
-                    "cool_setpoint": 0,
+                    Attribute.MODE: mode,
+                    Attribute.FAN_MODE: 0,
+                    Attribute.HEAT_SETPOINT: 0,
+                    Attribute.COOL_SETPOINT: 0,
                 },
             )
         )
 
     async def update_fan_mode(self, fan_mode: int):
         """Send a request to update the fan mode"""
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": 0,
-                    "fan_mode": fan_mode,
-                    "heat_setpoint": 0,
-                    "cool_setpoint": 0,
+                    Attribute.MODE: 0,
+                    Attribute.FAN_MODE: fan_mode,
+                    Attribute.HEAT_SETPOINT: 0,
+                    Attribute.COOL_SETPOINT: 0,
                 },
             )
         )
 
     async def update_setpoint(self, cool_setpoint: float, heat_setpoint: float):
         """Send a request to update the setpoint"""
 
@@ -224,86 +224,89 @@
 
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": 0,
-                    "fan_mode": 0,
-                    "heat_setpoint": heat_setpoint,
-                    "cool_setpoint": cool_setpoint,
+                    Attribute.MODE: 0,
+                    Attribute.FAN_MODE: 0,
+                    Attribute.HEAT_SETPOINT: heat_setpoint,
+                    Attribute.COOL_SETPOINT: cool_setpoint,
                 },
             )
         )
 
     async def set_hold(self, hold: int):
         """Send a request to set the hold status"""
 
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.SCHEDULING,
                 4,
-                data={"hold": hold},
+                data={Attribute.HOLD: hold},
             )
         )
 
     async def set_dehumidification_setpoint(self, dehumidification_setpoint: int):
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 3,
-                data={"dehumidification_setpoint": dehumidification_setpoint},
+                data={Attribute.DEHUMIDIFICATION_SETPOINT: dehumidification_setpoint},
             )
         )
 
         await self.read_dehumidification_setpoint()
 
     async def set_humidification_setpoint(self, humidification_setpoint: int):
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 4,
-                data={"humidification_setpoint": humidification_setpoint},
+                data={Attribute.HUMIDIFICATION_SETPOINT: humidification_setpoint},
             )
         )
 
         await self.read_humidification_setpoint()
 
     async def set_fresh_air(self, mode: int, event: int):
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 5,
-                data={"fresh_air_mode": mode, "fresh_air_event": event},
+                data={Attribute.FRESH_AIR_MODE: mode, Attribute.FRESH_AIR_EVENT: event},
             )
         )
 
     async def set_air_cleaning(self, mode: int, event: int):
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 6,
-                data={"air_cleaning_mode": mode, "air_cleaning_event": event},
+                data={
+                    Attribute.AIR_CLEANING_MODE: mode,
+                    Attribute.AIR_CLEANING_EVENT: event,
+                },
             )
         )
 
     async def sync(self):
         """Send a request to sync data"""
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.STATUS,
                 2,
-                data={"synced": 1},
+                data={Attribute.SYNCED: 1},
             )
         )
 
     async def configure_cos(self):
         """Send a request to configure the COS settings"""
         await self._send_packet(
             Packet(
@@ -426,17 +429,17 @@
                 future.set_result(data)
             except asyncio.exceptions.InvalidStateError:
                 pass
 
     def state_changed(self):
         """Send data indicating the state as changed"""
         data = {
-            "connected": self.connected,
-            "stopped": self.stopped,
-            "reconnecting": self.reconnecting,
+            Attribute.CONNECTED: self.connected,
+            Attribute.STOPPED: self.stopped,
+            Attribute.RECONNECTING: self.reconnecting,
         }
 
         self.data_received_callback(data)
 
     async def wait_for_response(
         self, functional_domain: FunctionalDomain, attribute: int, timeout: int = None
     ):
```

### Comparing `pyaprilaire-0.6.0b3/pyaprilaire/mock_server.py` & `pyaprilaire-0.7.0b1/pyaprilaire/mock_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import argparse
 import asyncio
 import logging
 
-from .const import Action, FunctionalDomain, QUEUE_FREQUENCY
+from .const import Action, Attribute, FunctionalDomain, QUEUE_FREQUENCY
 from .packet import Packet
 
 COS_FREQUENCY = 30
 
 
 class CustomFormatter(logging.Formatter):
     """Custom logging formatter"""
@@ -86,203 +86,207 @@
 
         await self.packet_queue.put(
             Packet(
                 Action.READ_RESPONSE,
                 FunctionalDomain.IDENTIFICATION,
                 2,
                 sequence=self._get_sequence(),
-                data={"mac_address": [1, 2, 3, 4, 5, 6]},
+                data={Attribute.MAC_ADDRESS: [1, 2, 3, 4, 5, 6]},
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.CONTROL,
                 1,
                 sequence=self._get_sequence(),
                 data={
-                    "mode": 1,
-                    "fan_mode": self.fan_mode,
-                    "heat_setpoint": self.heat_setpoint,
-                    "cool_setpoint": self.cool_setpoint,
+                    Attribute.MODE: 1,
+                    Attribute.FAN_MODE: self.fan_mode,
+                    Attribute.HEAT_SETPOINT: self.heat_setpoint,
+                    Attribute.COOL_SETPOINT: self.cool_setpoint,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.SENSORS,
                 2,
                 sequence=self._get_sequence(),
                 data={
-                    "indoor_temperature_controlling_sensor_status": 0,
-                    "indoor_temperature_controlling_sensor_value": 25,
-                    "outdoor_temperature_controlling_sensor_status": 0,
-                    "outdoor_temperature_controlling_sensor_value": 25,
-                    "indoor_humidity_controlling_sensor_status": 0,
-                    "indoor_humidity_controlling_sensor_value": 50,
-                    "outdoor_humidity_controlling_sensor_status": 0,
-                    "outdoor_humidity_controlling_sensor_value": 40,
+                    Attribute.INDOOR_TEMPERATURE_CONTROLLING_SENSOR_STATUS: 0,
+                    Attribute.INDOOR_TEMPERATURE_CONTROLLING_SENSOR_VALUE: 25,
+                    Attribute.OUTDOOR_TEMPERATURE_CONTROLLING_SENSOR_STATUS: 0,
+                    Attribute.OUTDOOR_TEMPERATURE_CONTROLLING_SENSOR_VALUE: 25,
+                    Attribute.INDOOR_HUMIDITY_CONTROLLING_SENSOR_STATUS: 0,
+                    Attribute.INDOOR_HUMIDITY_CONTROLLING_SENSOR_VALUE: 50,
+                    Attribute.OUTDOOR_HUMIDITY_CONTROLLING_SENSOR_STATUS: 0,
+                    Attribute.OUTDOOR_HUMIDITY_CONTROLLING_SENSOR_VALUE: 40,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.STATUS,
                 2,
                 sequence=self._get_sequence(),
                 data={
-                    "synced": 1,
+                    Attribute.SYNCED: 1,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.STATUS,
                 7,
                 sequence=self._get_sequence(),
                 data={
-                    "dehumidification_status": self.dehumidification_status,
-                    "humidification_status": self.humidification_status,
-                    "ventilation_status": 2 if self.fresh_air_mode else 0,
-                    "air_cleaning_status": 2 if self.air_cleaning_mode else 0,
+                    Attribute.DEHUMIDIFICATION_STATUS: self.dehumidification_status,
+                    Attribute.HUMIDIFICATION_STATUS: self.humidification_status,
+                    Attribute.VENTILATION_STATUS: 2 if self.fresh_air_mode else 0,
+                    Attribute.AIR_CLEANING_STATUS: 2 if self.air_cleaning_mode else 0,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.CONTROL,
                 7,
                 sequence=self._get_sequence(),
                 data={
-                    "thermostat_modes": 6,
-                    "air_cleaning_available": 1,
-                    "ventilation_available": 1,
-                    "dehumidification_available": 1,
-                    "humidification_available": 2,
+                    Attribute.THERMOSTAT_MODES: 6,
+                    Attribute.AIR_CLEANING_AVAILABLE: 1,
+                    Attribute.VENTILATION_AVAILABLE: 1,
+                    Attribute.DEHUMIDIFICATION_AVAILABLE: 1,
+                    Attribute.HUMIDIFICATION_AVAILABLE: 2,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.SETUP,
                 1,
                 sequence=self._get_sequence(),
-                data={"away_available": 1},
+                data={Attribute.AWAY_AVAILABLE: 1},
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.SCHEDULING,
                 4,
                 sequence=self._get_sequence(),
-                data={"hold": self.hold},
+                data={Attribute.HOLD: self.hold},
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.IDENTIFICATION,
                 1,
                 sequence=self._get_sequence(),
                 data={
-                    "hardware_revision": 66,
-                    "firmware_major_revision": 10,
-                    "firmware_minor_revision": 2,
-                    "protocol_major_revision": 15,
-                    "model_number": 1,
-                    "gainspan_firmware_major_revision": 14,
-                    "gainspan_firmware_minor_revision": 3,
+                    Attribute.HARDWARE_REVISION: 66,
+                    Attribute.FIRMWARE_MAJOR_REVISION: 10,
+                    Attribute.FIRMWARE_MINOR_REVISION: 2,
+                    Attribute.PROTOCOL_MAJOR_REVISION: 15,
+                    Attribute.MODEL_NUMBER: 1,
+                    Attribute.GAINSPAN_FIRMWARE_MAJOR_REVISION: 14,
+                    Attribute.GAINSPAN_FIRMWARE_MINOR_REVISION: 3,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.IDENTIFICATION,
                 4,
                 sequence=self._get_sequence(),
                 data={
-                    "location": self.location,
-                    "name": self.name,
+                    Attribute.LOCATION: self.location,
+                    Attribute.NAME: self.name,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.STATUS,
                 6,
                 sequence=self._get_sequence(),
                 data={
-                    "heating_equipment_status": {2: 2, 4: 7}.get(self.mode, 0),
-                    "cooling_equipment_status": {3: 2, 5: 2}.get(self.mode, 0),
-                    "progressive_recovery": 0,
-                    "fan_status": 1 if self.fan_mode == 1 or self.fan_mode == 2 else 0,
+                    Attribute.HEATING_EQUIPMENT_STATUS: {2: 2, 4: 7}.get(self.mode, 0),
+                    Attribute.COOLING_EQUIPMENT_STATUS: {3: 2, 5: 2}.get(self.mode, 0),
+                    Attribute.PROGRESSIVE_RECOVERY: 0,
+                    Attribute.FAN_STATUS: 1
+                    if self.fan_mode == 1 or self.fan_mode == 2
+                    else 0,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.CONTROL,
                 3,
                 sequence=self._get_sequence(),
-                data={"dehumidification_setpoint": self.dehumidification_setpoint},
+                data={
+                    Attribute.DEHUMIDIFICATION_SETPOINT: self.dehumidification_setpoint
+                },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.CONTROL,
                 4,
                 sequence=self._get_sequence(),
-                data={"humidification_setpoint": self.humidification_setpoint},
+                data={Attribute.HUMIDIFICATION_SETPOINT: self.humidification_setpoint},
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.CONTROL,
                 5,
                 sequence=self._get_sequence(),
                 data={
-                    "fresh_air_mode": self.fresh_air_mode,
-                    "fresh_air_event": self.fresh_air_event,
+                    Attribute.FRESH_AIR_MODE: self.fresh_air_mode,
+                    Attribute.FRESH_AIR_EVENT: self.fresh_air_event,
                 },
             )
         )
 
         await self.packet_queue.put(
             Packet(
                 Action.COS,
                 FunctionalDomain.CONTROL,
                 6,
                 sequence=self._get_sequence(),
                 data={
-                    "air_cleaning_mode": self.air_cleaning_mode,
-                    "air_cleaning_event": self.air_cleaning_event,
+                    Attribute.AIR_CLEANING_MODE: self.air_cleaning_mode,
+                    Attribute.AIR_CLEANING_EVENT: self.air_cleaning_event,
                 },
             )
         )
 
     async def _cos_loop(self):
         """Send the current status (COS) periodically"""
         while self.transport:
@@ -327,311 +331,317 @@
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.CONTROL,
                                 1,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "mode": self.mode,
-                                    "fan_mode": self.fan_mode,
-                                    "heat_setpoint": self.heat_setpoint,
-                                    "cool_setpoint": self.cool_setpoint,
+                                    Attribute.MODE: self.mode,
+                                    Attribute.FAN_MODE: self.fan_mode,
+                                    Attribute.HEAT_SETPOINT: self.heat_setpoint,
+                                    Attribute.COOL_SETPOINT: self.cool_setpoint,
                                 },
                             )
                         )
                     elif packet.attribute == 7:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.CONTROL,
                                 7,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "thermostat_modes": 6,
-                                    "air_cleaning_available": 1,
-                                    "ventilation_available": 1,
-                                    "dehumidification_available": 1,
-                                    "humidification_available": 1,
+                                    Attribute.THERMOSTAT_MODES: 6,
+                                    Attribute.AIR_CLEANING_AVAILABLE: 1,
+                                    Attribute.VENTILATION_AVAILABLE: 1,
+                                    Attribute.DEHUMIDIFICATION_AVAILABLE: 1,
+                                    Attribute.HUMIDIFICATION_AVAILABLE: 1,
                                 },
                             )
                         )
                     elif packet.attribute == 3:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.CONTROL,
                                 3,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "dehumidification_setpoint": self.dehumidification_setpoint
+                                    Attribute.DEHUMIDIFICATION_SETPOINT: self.dehumidification_setpoint
                                 },
                             )
                         )
                     elif packet.attribute == 4:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.CONTROL,
                                 4,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "humidification_setpoint": self.humidification_setpoint
+                                    Attribute.HUMIDIFICATION_SETPOINT: self.humidification_setpoint
                                 },
                             )
                         )
                     elif packet.attribute == 5:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.CONTROL,
                                 5,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "fresh_air_mode": self.fresh_air_mode,
-                                    "fresh_air_event": self.fresh_air_event,
+                                    Attribute.FRESH_AIR_MODE: self.fresh_air_mode,
+                                    Attribute.FRESH_AIR_EVENT: self.fresh_air_event,
                                 },
                             )
                         )
                     elif packet.attribute == 6:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.CONTROL,
                                 6,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "air_cleaning_mode": self.air_cleaning_mode,
-                                    "air_cleaning_event": self.air_cleaning_event,
+                                    Attribute.AIR_CLEANING_MODE: self.air_cleaning_mode,
+                                    Attribute.AIR_CLEANING_EVENT: self.air_cleaning_event,
                                 },
                             )
                         )
                 elif packet.functional_domain == FunctionalDomain.SENSORS:
                     if packet.attribute == 2:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.SENSORS,
                                 2,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "indoor_temperature_controlling_sensor_status": 0,
-                                    "indoor_temperature_controlling_sensor_value": 25,
-                                    "outdoor_temperature_controlling_sensor_status": 0,
-                                    "outdoor_temperature_controlling_sensor_value": 25,
-                                    "indoor_humidity_controlling_sensor_status": 0,
-                                    "indoor_humidity_controlling_sensor_value": 50,
-                                    "outdoor_humidity_controlling_sensor_status": 0,
-                                    "outdoor_humidity_controlling_sensor_value": 40,
+                                    Attribute.INDOOR_TEMPERATURE_CONTROLLING_SENSOR_STATUS: 0,
+                                    Attribute.INDOOR_TEMPERATURE_CONTROLLING_SENSOR_VALUE: 25,
+                                    Attribute.OUTDOOR_TEMPERATURE_CONTROLLING_SENSOR_STATUS: 0,
+                                    Attribute.OUTDOOR_TEMPERATURE_CONTROLLING_SENSOR_VALUE: 25,
+                                    Attribute.INDOOR_HUMIDITY_CONTROLLING_SENSOR_STATUS: 0,
+                                    Attribute.INDOOR_HUMIDITY_CONTROLLING_SENSOR_VALUE: 50,
+                                    Attribute.OUTDOOR_HUMIDITY_CONTROLLING_SENSOR_STATUS: 0,
+                                    Attribute.OUTDOOR_HUMIDITY_CONTROLLING_SENSOR_VALUE: 40,
                                 },
                             )
                         )
                 elif packet.functional_domain == FunctionalDomain.SCHEDULING:
                     if packet.attribute == 4:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.SCHEDULING,
                                 4,
                                 sequence=self._get_sequence(),
-                                data={"hold": self.hold},
+                                data={Attribute.HOLD: self.hold},
                             )
                         )
                 elif packet.functional_domain == FunctionalDomain.IDENTIFICATION:
                     if packet.attribute == 2:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.IDENTIFICATION,
                                 2,
                                 sequence=self._get_sequence(),
-                                data={"mac_address": self.mac_address},
+                                data={Attribute.MAC_ADDRESS: self.mac_address},
                             )
                         )
                     elif packet.attribute == 4 or packet.attribute == 5:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.READ_RESPONSE,
                                 FunctionalDomain.IDENTIFICATION,
                                 4,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "location": self.location,
-                                    "name": self.name,
+                                    Attribute.LOCATION: self.location,
+                                    Attribute.NAME: self.name,
                                 },
                             )
                         )
             elif packet.action == Action.WRITE:
                 if packet.functional_domain == FunctionalDomain.CONTROL:
                     if packet.attribute == 1:
-                        if "mode" in packet.data:
-                            new_mode = packet.data["mode"]
+                        if Attribute.MODE in packet.data:
+                            new_mode = packet.data[Attribute.MODE]
 
                             if new_mode != 0:
                                 self.mode = new_mode
                                 self.hold = 0
 
-                        if "fan_mode" in packet.data:
-                            new_fan_mode = packet.data["fan_mode"]
+                        if Attribute.FAN_MODE in packet.data:
+                            new_fan_mode = packet.data[Attribute.FAN_MODE]
 
                             if new_fan_mode != 0:
                                 self.fan_mode = new_fan_mode
 
-                        if "heat_setpoint" in packet.data:
-                            new_heat_setpoint = packet.data["heat_setpoint"]
+                        if Attribute.HEAT_SETPOINT in packet.data:
+                            new_heat_setpoint = packet.data[Attribute.HEAT_SETPOINT]
 
                             if new_heat_setpoint != 0:
                                 self.heat_setpoint = new_heat_setpoint
                                 self.hold = 1
 
-                        if "cool_setpoint" in packet.data:
-                            new_cool_setpoint = packet.data["cool_setpoint"]
+                        if Attribute.COOL_SETPOINT in packet.data:
+                            new_cool_setpoint = packet.data[Attribute.COOL_SETPOINT]
 
                             if new_cool_setpoint != 0:
                                 self.cool_setpoint = new_cool_setpoint
                                 self.hold = 1
 
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
                                 FunctionalDomain.CONTROL,
                                 1,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "mode": self.mode,
-                                    "fan_mode": self.fan_mode,
-                                    "heat_setpoint": self.heat_setpoint,
-                                    "cool_setpoint": self.cool_setpoint,
+                                    Attribute.MODE: self.mode,
+                                    Attribute.FAN_MODE: self.fan_mode,
+                                    Attribute.HEAT_SETPOINT: self.heat_setpoint,
+                                    Attribute.COOL_SETPOINT: self.cool_setpoint,
                                 },
                             )
                         )
 
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
                                 FunctionalDomain.STATUS,
                                 6,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "heating_equipment_status": {2: 2, 4: 7}.get(
-                                        self.mode, 0
-                                    ),
-                                    "cooling_equipment_status": {3: 2, 5: 2}.get(
-                                        self.mode, 0
-                                    ),
-                                    "progressive_recovery": 0,
-                                    "fan_status": 1
+                                    Attribute.HEATING_EQUIPMENT_STATUS: {
+                                        2: 2,
+                                        4: 7,
+                                    }.get(self.mode, 0),
+                                    Attribute.COOLING_EQUIPMENT_STATUS: {
+                                        3: 2,
+                                        5: 2,
+                                    }.get(self.mode, 0),
+                                    Attribute.PROGRESSIVE_RECOVERY: 0,
+                                    Attribute.FAN_STATUS: 1
                                     if self.fan_mode == 1 or self.fan_mode == 2
                                     else 0,
                                 },
                             )
                         )
 
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
                                 FunctionalDomain.SCHEDULING,
                                 4,
                                 sequence=self._get_sequence(),
-                                data={"hold": self.hold},
+                                data={Attribute.HOLD: self.hold},
                             )
                         )
                     elif packet.attribute == 3:
                         self.dehumidification_setpoint = packet.data[
-                            "dehumidification_setpoint"
+                            Attribute.DEHUMIDIFICATION_SETPOINT
                         ]
                         self.dehumidification_status = 2
                     elif packet.attribute == 4:
                         self.humidification_setpoint = packet.data[
-                            "humidification_setpoint"
+                            Attribute.HUMIDIFICATION_SETPOINT
                         ]
                         self.humidification_status = 2
                     elif packet.attribute == 5:
-                        self.fresh_air_mode = packet.data["fresh_air_mode"]
-                        self.fresh_air_event = packet.data["fresh_air_event"]
+                        self.fresh_air_mode = packet.data[Attribute.FRESH_AIR_MODE]
+                        self.fresh_air_event = packet.data[Attribute.FRESH_AIR_EVENT]
 
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
                                 FunctionalDomain.CONTROL,
                                 5,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "fresh_air_mode": self.fresh_air_mode,
-                                    "fresh_air_event": self.fresh_air_event,
+                                    Attribute.FRESH_AIR_MODE: self.fresh_air_mode,
+                                    Attribute.FRESH_AIR_EVENT: self.fresh_air_event,
                                 },
                             )
                         )
 
                     if packet.attribute in [3, 4, 5]:
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
                                 FunctionalDomain.STATUS,
                                 7,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "dehumidification_status": self.dehumidification_status,
-                                    "humidification_status": self.humidification_status,
-                                    "ventilation_status": 2
+                                    Attribute.DEHUMIDIFICATION_STATUS: self.dehumidification_status,
+                                    Attribute.HUMIDIFICATION_STATUS: self.humidification_status,
+                                    Attribute.VENTILATION_STATUS: 2
                                     if self.fresh_air_mode
                                     else 0,
-                                    "air_cleaning_status": 2
+                                    Attribute.AIR_CLEANING_STATUS: 2
                                     if self.air_cleaning_mode
                                     else 0,
                                 },
                             )
                         )
                     elif packet.attribute == 6:
-                        self.air_cleaning_mode = packet.data["air_cleaning_mode"]
-                        self.air_cleaning_event = packet.data["air_cleaning_event"]
+                        self.air_cleaning_mode = packet.data[
+                            Attribute.AIR_CLEANING_MODE
+                        ]
+                        self.air_cleaning_event = packet.data[
+                            Attribute.AIR_CLEANING_EVENT
+                        ]
 
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
                                 FunctionalDomain.CONTROL,
                                 6,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "air_cleaning_mode": self.air_cleaning_mode,
-                                    "air_cleaning_event": self.air_cleaning_event,
+                                    Attribute.AIR_CLEANING_MODE: self.air_cleaning_mode,
+                                    Attribute.AIR_CLEANING_EVENT: self.air_cleaning_event,
                                 },
                             )
                         )
 
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
                                 FunctionalDomain.STATUS,
                                 7,
                                 sequence=self._get_sequence(),
                                 data={
-                                    "dehumidification_status": 2,
-                                    "humidification_status": 2,
-                                    "ventilation_status": 2
+                                    Attribute.DEHUMIDIFICATION_STATUS: 2,
+                                    Attribute.HUMIDIFICATION_STATUS: 2,
+                                    Attribute.VENTILATION_STATUS: 2
                                     if self.fresh_air_mode
                                     else 0,
-                                    "air_cleaning_status": 2
+                                    Attribute.AIR_CLEANING_STATUS: 2
                                     if self.air_cleaning_mode
                                     else 0,
                                 },
                             )
                         )
 
                 elif packet.functional_domain == FunctionalDomain.SCHEDULING:
                     if packet.attribute == 4:
-                        if "hold" in packet.data:
-                            self.hold = packet.data["hold"]
+                        if Attribute.HOLD in packet.data:
+                            self.hold = packet.data[Attribute.HOLD]
 
                         self.packet_queue.put_nowait(
                             Packet(
                                 Action.COS,
                                 FunctionalDomain.SCHEDULING,
                                 4,
                                 sequence=self._get_sequence(),
-                                data={"hold": self.hold},
+                                data={Attribute.HOLD: self.hold},
                             )
                         )
                 elif packet.functional_domain == FunctionalDomain.STATUS:
                     if packet.attribute == 2:
                         asyncio.ensure_future(self._send_status())
 
     def connection_lost(self, exc: Exception | None) -> None:
```

### Comparing `pyaprilaire-0.6.0b3/pyaprilaire/socket_client.py` & `pyaprilaire-0.7.0b1/pyaprilaire/socket_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b3/pyaprilaire.egg-info/PKG-INFO` & `pyaprilaire-0.7.0b1/pyaprilaire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.6.0b3
+Version: 0.7.0b1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.6.0b3/pyproject.toml` & `pyaprilaire-0.7.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaprilaire"
-version = "0.6.0b3"
+version = "0.7.0b1"
 readme = "README.md"
 dependencies = [
     "crc >= 4"
 ]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "coverage"]
 
 [tool.bumpver]
-current_version = "0.6.0b3"
+current_version = "0.7.0b1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyaprilaire-0.6.0b3/tests/test_client.py` & `pyaprilaire-0.7.0b1/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyaprilaire.client import _AprilaireClientProtocol, AprilaireClient
-from pyaprilaire.const import Action, FunctionalDomain
+from pyaprilaire.const import Action, Attribute, FunctionalDomain
 from pyaprilaire.packet import Packet
 
 import asyncio
 import logging
 
 import unittest
 from unittest.mock import patch, AsyncMock, Mock
@@ -60,18 +60,18 @@
         (functional_domain, attribute, data) = self.data_received_mock.call_args[0]
 
         self.assertEqual(functional_domain, FunctionalDomain.CONTROL)
         self.assertEqual(attribute, 1)
         self.assertDictEqual(
             data,
             {
-                "mode": 1,
-                "fan_mode": 2,
-                "heat_setpoint": 10,
-                "cool_setpoint": 20,
+                Attribute.MODE: 1,
+                Attribute.FAN_MODE: 2,
+                Attribute.HEAT_SETPOINT: 10,
+                Attribute.COOL_SETPOINT: 20,
             },
         )
 
     def test_data_received_nack(self):
         with self.assertLogs(self.logger, level="ERROR") as cm:
             self.protocol.data_received(bytes([1, 1, 0, 2, 6, 1, 0]))
 
@@ -140,18 +140,18 @@
         self.protocol.packet_queue.put_nowait = Mock()
 
         original_packet = Packet(
             Action.WRITE,
             FunctionalDomain.CONTROL,
             1,
             data={
-                "mode": 1,
-                "fan_mode": 0,
-                "heat_setpoint": 0,
-                "cool_setpoint": 0,
+                Attribute.MODE: 1,
+                Attribute.FAN_MODE: 0,
+                Attribute.HEAT_SETPOINT: 0,
+                Attribute.COOL_SETPOINT: 0,
             },
         )
 
         await self.protocol._send_packet(original_packet)
 
         self.assertEqual(self.protocol.packet_queue.put.call_count, 1)
 
@@ -190,80 +190,80 @@
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": 1,
-                    "fan_mode": 0,
-                    "heat_setpoint": 0,
-                    "cool_setpoint": 0,
+                    Attribute.MODE: 1,
+                    Attribute.FAN_MODE: 0,
+                    Attribute.HEAT_SETPOINT: 0,
+                    Attribute.COOL_SETPOINT: 0,
                 },
             )
         )
 
     async def test_update_fan_mode(self):
         await self.protocol.update_fan_mode(1)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": 0,
-                    "fan_mode": 1,
-                    "heat_setpoint": 0,
-                    "cool_setpoint": 0,
+                    Attribute.MODE: 0,
+                    Attribute.FAN_MODE: 1,
+                    Attribute.HEAT_SETPOINT: 0,
+                    Attribute.COOL_SETPOINT: 0,
                 },
             )
         )
 
     async def test_update_setpoint(self):
         await self.protocol.update_setpoint(10, 20)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": 0,
-                    "fan_mode": 0,
-                    "heat_setpoint": 20,
-                    "cool_setpoint": 10,
+                    Attribute.MODE: 0,
+                    Attribute.FAN_MODE: 0,
+                    Attribute.HEAT_SETPOINT: 20,
+                    Attribute.COOL_SETPOINT: 10,
                 },
             )
         )
 
     async def test_set_hold(self):
         await self.protocol.set_hold(1)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.SCHEDULING,
                 4,
                 data={
-                    "hold": 1,
+                    Attribute.HOLD: 1,
                 },
             )
         )
 
     async def test_sync(self):
         await self.protocol.sync()
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.STATUS,
                 2,
                 data={
-                    "synced": 1,
+                    Attribute.SYNCED: 1,
                 },
             )
         )
 
     async def test_configure_cos(self):
         pass
 
@@ -389,15 +389,19 @@
         self.client.reconnecting = True
 
         self.client.state_changed()
 
         self.assertEqual(self.data_received_mock.call_count, 1)
         self.assertEqual(
             self.data_received_mock.call_args[0][0],
-            {"connected": True, "stopped": True, "reconnecting": True},
+            {
+                Attribute.CONNECTED: True,
+                Attribute.STOPPED: True,
+                Attribute.RECONNECTING: True,
+            },
         )
 
     def assertPacketQueueContains(self, packet: Packet):
         queue_items = list(self.client.protocol.packet_queue._queue)
 
         self.assertEqual(any(qp == packet for qp in queue_items), True)
 
@@ -427,138 +431,138 @@
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": 1,
-                    "fan_mode": 0,
-                    "heat_setpoint": 0,
-                    "cool_setpoint": 0,
+                    Attribute.MODE: 1,
+                    Attribute.FAN_MODE: 0,
+                    Attribute.HEAT_SETPOINT: 0,
+                    Attribute.COOL_SETPOINT: 0,
                 },
             )
         )
 
     async def test_update_fan_mode(self):
         await self.client.update_fan_mode(1)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": 0,
-                    "fan_mode": 1,
-                    "heat_setpoint": 0,
-                    "cool_setpoint": 0,
+                    Attribute.MODE: 0,
+                    Attribute.FAN_MODE: 1,
+                    Attribute.HEAT_SETPOINT: 0,
+                    Attribute.COOL_SETPOINT: 0,
                 },
             )
         )
 
     async def test_update_setpoint(self):
         await self.client.update_setpoint(10, 20)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
-                    "mode": 0,
-                    "fan_mode": 0,
-                    "heat_setpoint": 20,
-                    "cool_setpoint": 10,
+                    Attribute.MODE: 0,
+                    Attribute.FAN_MODE: 0,
+                    Attribute.HEAT_SETPOINT: 20,
+                    Attribute.COOL_SETPOINT: 10,
                 },
             )
         )
 
     async def test_set_hold(self):
         await self.client.set_hold(1)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.SCHEDULING,
                 4,
                 data={
-                    "hold": 1,
+                    Attribute.HOLD: 1,
                 },
             )
         )
 
     async def test_set_dehumidification_setpoint(self):
         await self.client.set_dehumidification_setpoint(50)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 3,
                 data={
-                    "dehumidification_setpoint": 50,
+                    Attribute.DEHUMIDIFICATION_SETPOINT: 50,
                 },
             )
         )
 
     async def test_set_humidification_setpoint(self):
         await self.client.set_humidification_setpoint(50)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 4,
                 data={
-                    "humidification_setpoint": 50,
+                    Attribute.HUMIDIFICATION_SETPOINT: 50,
                 },
             )
         )
 
     async def test_set_fresh_air(self):
         await self.client.set_fresh_air(1, 3)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 5,
                 data={
-                    "fresh_air_mode": 1,
-                    "fresh_air_event": 3,
+                    Attribute.FRESH_AIR_MODE: 1,
+                    Attribute.FRESH_AIR_EVENT: 3,
                 },
             )
         )
 
     async def test_set_air_cleaning(self):
         await self.client.set_air_cleaning(1, 3)
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 6,
                 data={
-                    "air_cleaning_mode": 1,
-                    "air_cleaning_event": 3,
+                    Attribute.AIR_CLEANING_MODE: 1,
+                    Attribute.AIR_CLEANING_EVENT: 3,
                 },
             )
         )
 
     async def test_sync(self):
         await self.client.sync()
 
         self.assertPacketQueueContains(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.STATUS,
                 2,
                 data={
-                    "synced": 1,
+                    Attribute.SYNCED: 1,
                 },
             )
         )
 
     async def test_configure_cos(self):
         pass
```

### Comparing `pyaprilaire-0.6.0b3/tests/test_packet.py` & `pyaprilaire-0.7.0b1/tests/test_packet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyaprilaire.const import Action, FunctionalDomain
+from pyaprilaire.const import Action, Attribute, FunctionalDomain
 from pyaprilaire.packet import NackPacket, Packet
 
 import unittest
 
 
 class Test_Packet(unittest.TestCase):
     def test_invalid_action(self):
@@ -147,66 +147,66 @@
         )
 
         packet = packets[0]
 
         self.assertDictEqual(
             packet.data,
             {
-                "mode": 1,
-                "fan_mode": 2,
-                "heat_setpoint": 10,
-                "cool_setpoint": 20,
+                Attribute.MODE: 1,
+                Attribute.FAN_MODE: 2,
+                Attribute.HEAT_SETPOINT: 10,
+                Attribute.COOL_SETPOINT: 20,
             },
         )
 
     def test_scheduling_4_parse(self):
         packets: list[Packet] = list(
             Packet.parse([1, 1, 0, 13, 3, 3, 4, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 42])
         )
 
         packet = packets[0]
 
         self.assertDictEqual(
             packet.data,
             {
-                "hold": 1,
+                Attribute.HOLD: 1,
             },
         )
 
     def test_sensor_2_parse(self):
         packets: list[Packet] = list(
             Packet.parse([1, 1, 0, 11, 3, 5, 2, 1, 10, 2, 20, 3, 50, 4, 60, 12])
         )
 
         packet = packets[0]
 
         self.assertDictEqual(
             packet.data,
             {
-                "indoor_temperature_controlling_sensor_status": 1,
-                "indoor_temperature_controlling_sensor_value": 10,
-                "outdoor_temperature_controlling_sensor_status": 2,
-                "outdoor_temperature_controlling_sensor_value": 20,
-                "indoor_humidity_controlling_sensor_status": 3,
-                "indoor_humidity_controlling_sensor_value": 50,
-                "outdoor_humidity_controlling_sensor_status": 4,
-                "outdoor_humidity_controlling_sensor_value": 60,
+                Attribute.INDOOR_TEMPERATURE_CONTROLLING_SENSOR_STATUS: 1,
+                Attribute.INDOOR_TEMPERATURE_CONTROLLING_SENSOR_VALUE: 10,
+                Attribute.OUTDOOR_TEMPERATURE_CONTROLLING_SENSOR_STATUS: 2,
+                Attribute.OUTDOOR_TEMPERATURE_CONTROLLING_SENSOR_VALUE: 20,
+                Attribute.INDOOR_HUMIDITY_CONTROLLING_SENSOR_STATUS: 3,
+                Attribute.INDOOR_HUMIDITY_CONTROLLING_SENSOR_VALUE: 50,
+                Attribute.OUTDOOR_HUMIDITY_CONTROLLING_SENSOR_STATUS: 4,
+                Attribute.OUTDOOR_HUMIDITY_CONTROLLING_SENSOR_VALUE: 60,
             },
         )
 
     def test_identification_2_parse(self):
         packets: list[Packet] = list(
             Packet.parse([1, 1, 0, 9, 3, 8, 2, 1, 2, 3, 4, 5, 6, 176])
         )
 
         packet = packets[0]
 
         self.assertDictEqual(
             packet.data,
-            {"mac_address": "1:2:3:4:5:6"},
+            {Attribute.MAC_ADDRESS: "1:2:3:4:5:6"},
         )
 
     def test_identification_4_parse(self):
         packets: list[Packet] = list(
             Packet.parse(
                 [
                     1,
@@ -245,15 +245,15 @@
             )
         )
 
         packet = packets[0]
 
         self.assertDictEqual(
             packet.data,
-            {"location": "12345", "name": "Test Name"},
+            {Attribute.LOCATION: "12345", Attribute.NAME: "Test Name"},
         )
 
     def test_decode_temperature(self):
         temperature = Packet._decode_temperature(0x15)
 
         self.assertEqual(temperature, 21)
 
@@ -372,32 +372,32 @@
         serialized = Packet(
             Action.READ_RESPONSE,
             FunctionalDomain.CONTROL,
             1,
             1,
             1,
             data={
-                "mode": 1,
-                "fan_mode": 2,
-                "heat_setpoint": 10,
-                "cool_setpoint": 20,
+                Attribute.MODE: 1,
+                Attribute.FAN_MODE: 2,
+                Attribute.HEAT_SETPOINT: 10,
+                Attribute.COOL_SETPOINT: 20,
             },
         ).serialize()
 
         self.assertSequenceEqual(serialized, [1, 1, 0, 7, 3, 2, 1, 1, 2, 10, 20, 107])
 
     def test_scheduling_4_serialize(self):
         serialized = Packet(
             Action.READ_RESPONSE,
             FunctionalDomain.SCHEDULING,
             4,
             1,
             1,
             data={
-                "hold": 1,
+                Attribute.HOLD: 1,
             },
         ).serialize()
 
         self.assertSequenceEqual(
             serialized, [1, 1, 0, 13, 3, 3, 4, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 55]
         )
 
@@ -405,51 +405,51 @@
         serialized = Packet(
             Action.READ_RESPONSE,
             FunctionalDomain.SENSORS,
             2,
             1,
             1,
             data={
-                "indoor_temperature_controlling_sensor_status": 1,
-                "indoor_temperature_controlling_sensor_value": 10,
-                "outdoor_temperature_controlling_sensor_status": 2,
-                "outdoor_temperature_controlling_sensor_value": 20,
-                "indoor_humidity_controlling_sensor_status": 3,
-                "indoor_humidity_controlling_sensor_value": 50,
-                "outdoor_humidity_controlling_sensor_status": 4,
-                "outdoor_humidity_controlling_sensor_value": 60,
+                Attribute.INDOOR_TEMPERATURE_CONTROLLING_SENSOR_STATUS: 1,
+                Attribute.INDOOR_TEMPERATURE_CONTROLLING_SENSOR_VALUE: 10,
+                Attribute.OUTDOOR_TEMPERATURE_CONTROLLING_SENSOR_STATUS: 2,
+                Attribute.OUTDOOR_TEMPERATURE_CONTROLLING_SENSOR_VALUE: 20,
+                Attribute.INDOOR_HUMIDITY_CONTROLLING_SENSOR_STATUS: 3,
+                Attribute.INDOOR_HUMIDITY_CONTROLLING_SENSOR_VALUE: 50,
+                Attribute.OUTDOOR_HUMIDITY_CONTROLLING_SENSOR_STATUS: 4,
+                Attribute.OUTDOOR_HUMIDITY_CONTROLLING_SENSOR_VALUE: 60,
             },
         ).serialize()
 
         self.assertSequenceEqual(
             serialized, [1, 1, 0, 11, 3, 5, 2, 1, 10, 2, 20, 3, 50, 4, 60, 12]
         )
 
     def test_identification_2_serialize(self):
         serialized = Packet(
             Action.READ_RESPONSE,
             FunctionalDomain.IDENTIFICATION,
             2,
             1,
             1,
-            data={"mac_address": [1, 2, 3, 4, 5, 6]},
+            data={Attribute.MAC_ADDRESS: [1, 2, 3, 4, 5, 6]},
         ).serialize()
 
         self.assertSequenceEqual(
             serialized, [1, 1, 0, 9, 3, 8, 2, 1, 2, 3, 4, 5, 6, 176]
         )
 
     def test_identification_4_serialize(self):
         serialized = Packet(
             Action.READ_RESPONSE,
             FunctionalDomain.IDENTIFICATION,
             4,
             1,
             1,
-            data={"location": "12345", "name": "Test Name"},
+            data={Attribute.LOCATION: "12345", Attribute.NAME: "Test Name"},
         ).serialize()
 
         self.assertSequenceEqual(
             serialized,
             [
                 1,
                 1,
```

### Comparing `pyaprilaire-0.6.0b3/tests/test_socket_client.py` & `pyaprilaire-0.7.0b1/tests/test_socket_client.py`

 * *Files identical despite different names*

