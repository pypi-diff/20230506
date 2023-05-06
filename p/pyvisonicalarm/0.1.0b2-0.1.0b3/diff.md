# Comparing `tmp/pyvisonicalarm-0.1.0b2.tar.gz` & `tmp/pyvisonicalarm-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisonicalarm-0.1.0b2.tar", last modified: Thu May  4 15:20:14 2023, max compression
+gzip compressed data, was "pyvisonicalarm-0.1.0b3.tar", last modified: Sat May  6 12:27:22 2023, max compression
```

## Comparing `pyvisonicalarm-0.1.0b2.tar` & `pyvisonicalarm-0.1.0b3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:20:14.760583 pyvisonicalarm-0.1.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-04 15:20:14.756583 pyvisonicalarm-0.1.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:20:14.756583 pyvisonicalarm-0.1.0b2/pyvisonicalarm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/device_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:20:14.756583 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 15:20:14.000000 pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:20:14.760583 pyvisonicalarm-0.1.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 15:20:01.000000 pyvisonicalarm-0.1.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/pyvisonicalarm/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/device_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 12:27:22.000000 pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 12:27:22.475135 pyvisonicalarm-0.1.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-06 12:27:06.000000 pyvisonicalarm-0.1.0b3/setup.py
```

### Comparing `pyvisonicalarm-0.1.0b2/LICENSE` & `pyvisonicalarm-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b2/PKG-INFO` & `pyvisonicalarm-0.1.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvisonicalarm-0.1.0b2/README.md` & `pyvisonicalarm-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b2/pyvisonicalarm/alarm.py` & `pyvisonicalarm-0.1.0b3/pyvisonicalarm/alarm.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b2/pyvisonicalarm/classes.py` & `pyvisonicalarm-0.1.0b3/pyvisonicalarm/classes.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b2/pyvisonicalarm/const.py` & `pyvisonicalarm-0.1.0b3/pyvisonicalarm/const.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-__VERSION__ = "0.1.0b2"
-
-import enum
-
-
 TEXT_UNKNOWN = "Unknown"
 TEXT_OPEN = "Open"
 TEXT_OPENED = "OPENED"
 TEXT_CLOSED = "Closed"
 TEXT_STATUS_HOME = "HOME"
 TEXT_STATUS_AWAY = "AWAY"
 TEXT_STATUS_DISARM = "DISARM"
```

### Comparing `pyvisonicalarm-0.1.0b2/pyvisonicalarm/core.py` & `pyvisonicalarm-0.1.0b3/pyvisonicalarm/core.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b2/pyvisonicalarm/device_definitions.py` & `pyvisonicalarm-0.1.0b3/pyvisonicalarm/device_definitions.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b2/pyvisonicalarm/devices.py` & `pyvisonicalarm-0.1.0b3/pyvisonicalarm/devices.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from datetime import datetime
 from .classes import BaseClass, title_case
 from .const import TEXT_CLOSED, TEXT_OPEN, TEXT_OPENED, TEXT_UNKNOWN
 
 
 @dataclass
 class Device(BaseClass):
     """Base class definition of a device in the alarm system."""
@@ -91,18 +92,26 @@
 @dataclass
 class MotionDevice(Device):
     """Motion sensor device class definition."""
 
     @property
     def brightness(self) -> int:
         return self._get_nested_key("traits.meteo_info.brightness.value")
+    
+    @property
+    def brightness_last_updated(self) -> datetime:
+        return self._get_nested_key("traits.meteo_info.brightness.date")
 
     @property
     def temperature(self) -> float:
         return self._get_nested_key("traits.meteo_info.temperature.value")
+    
+    @property
+    def temperature_last_updated(self) -> datetime:
+        return self._get_nested_key("traits.meteo_info.temperature.date")
 
 
 @dataclass
 class GenericDevice(Device):
     """Smoke device class definition."""
```

### Comparing `pyvisonicalarm-0.1.0b2/pyvisonicalarm/exceptions.py` & `pyvisonicalarm-0.1.0b3/pyvisonicalarm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvisonicalarm-0.1.0b2/pyvisonicalarm.egg-info/PKG-INFO` & `pyvisonicalarm-0.1.0b3/pyvisonicalarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisonicalarm
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: A simple library for the Visonic Alarm API written in Python 3
 Home-page: https://github.com/msp1974/pyvisonicalarm
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

