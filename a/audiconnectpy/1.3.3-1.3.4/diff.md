# Comparing `tmp/audiconnectpy-1.3.3.tar.gz` & `tmp/audiconnectpy-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.3.tar", last modified: Mon May  1 16:08:33 2023, max compression
+gzip compressed data, was "audiconnectpy-1.3.4.tar", last modified: Sat May  6 10:03:31 2023, max compression
```

## Comparing `audiconnectpy-1.3.3.tar` & `audiconnectpy-1.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22628 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27875 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30451 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 16:08:33.000000 audiconnectpy-1.3.3/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-01 16:08:27.000000 audiconnectpy-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:33.937215 audiconnectpy-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 16:08:09.000000 audiconnectpy-1.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27807 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-06 10:03:29.000000 audiconnectpy-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.3/LICENSE` & `audiconnectpy-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.3/PKG-INFO` & `audiconnectpy-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.3/README.md` & `audiconnectpy-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.3/audiconnectpy/api.py` & `audiconnectpy-1.3.4/audiconnectpy/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import logging
 
 from aiohttp import ClientSession
 
 from .auth import Auth
 from .exceptions import AudiException
+from .helpers import ExtendedDict
 from .models import Globals, Vehicle
 from .services import AudiService
-from .util import ExtendedDict
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AudiConnect:
     """Representation of an Audi Connect Account."""
 
@@ -51,15 +51,15 @@
         """Update data."""
         if not await self.async_login():
             return False
         # Update the state of all vehicles.
         try:
             if len(self._audi_vehicles) == 0:
                 vehicles_response = await self.services.async_get_vehicle_information()
-                for response in vehicles_response.getr("data.userVehicles", {}):
+                for response in vehicles_response.getr("data.userVehicles", []):
                     self._audi_vehicles.append(
                         Vehicle(ExtendedDict(response), self.services)
                     )
             for vehicle in self._audi_vehicles:
                 await self._async_add_or_update_vehicle(vehicle, vinlist)
             return True
         except IOError as exception:
```

### Comparing `audiconnectpy-1.3.3/audiconnectpy/auth.py` & `audiconnectpy-1.3.4/audiconnectpy/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from .exceptions import (
     AudiException,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
 )
-from .util import json_loads
+from .helpers import json_loads
 
 TIMEOUT = 120
 DELAY = 10
 HDR_XAPP_VERSION = "4.13.0"
 HDR_USER_AGENT = "myAudi-Android/4.13.0 (Build 800238275.2210271555) Android/11"
 MARKET_URL = "https://content.app.my.audi.com/service/mobileapp/configurations"
 CLIENT_ID = "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com"
```

### Comparing `audiconnectpy-1.3.3/audiconnectpy/models.py` & `audiconnectpy-1.3.4/audiconnectpy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import logging
 from dataclasses import dataclass
 from datetime import datetime as dt
 from typing import TYPE_CHECKING, Any, Literal
 
 from .exceptions import HttpRequestError, ServiceNotFoundError, TimeoutExceededError
-from .util import ExtendedDict, retry
+from .helpers import ExtendedDict, retry
 
 if TYPE_CHECKING:
     from .services import AudiService
 
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -110,15 +110,15 @@
         "0x030106000D": "tyre_pressure_right_front_tyre_difference",
         "0x030106000E": "tyre_pressure_right_rear_tyre_difference",
         "0x030106000F": "tyre_pressure_spare_tyre_difference",
     }
 
     def __init__(self, data: ExtendedDict, has_pin: bool = False) -> None:
         """Initialize."""
-        self.data: ExtendedDict = data
+        self.data = data
         self.has_pin = has_pin
         self.measure_time = None
         self.send_time = None
         self.send_time_utc = None
         self.measure_mileage = None
         self.send_mileage = None
         self._vehicle_data = self._get_attributes()
@@ -299,18 +299,18 @@
             self.data.getr("charger.settings") is not None
             or self.data.getr("charger.status") is not None
         )
 
     @property
     def attributes(self) -> dict[str, Any]:
         """Attributes properties."""
-        settings = ExtendedDict(self.data.getr("charger.settings", {}))
-        status = ExtendedDict(self.data.getr("charger.status", {}))
-        charging = ExtendedDict(status.get("chargingStatusData", {}))
-        cruising = ExtendedDict(status.get("cruisingRangeStatusData", {}))
+        settings = self.data.getr("charger.settings", {})
+        status = self.data.getr("charger.status", {})
+        charging = status.get("chargingStatusData", {})
+        cruising = status.get("cruisingRangeStatusData", {})
         attrs = {
             "max_charge_current": settings.getr("maxChargeCurrent.content"),
             "charging_state": charging.getr("chargingState.content"),
             "actual_charge_rate": charging.getr("actualChargeRate.content"),
             "actual_charge_rate_unit": charging.getr("chargeRateUnit.content"),
             "charging_power": charging.getr("chargingPower.content"),
             "charging_mode": charging.getr("chargingMode.content"),
@@ -344,16 +344,16 @@
             or self.data.getr("climater.status") is not None
         )
 
     @property
     def attributes(self) -> dict[str, Any]:
         """Attributes properties."""
         attrs = {}
-        settings = ExtendedDict(self.data.getr("climater.settings"))
-        status = ExtendedDict(self.data.getr("climater.status"))
+        settings = self.data.getr("climater.settings")
+        status = self.data.getr("climater.status")
         attrs = {
             "climatisation_state": status.getr(
                 "climatisationStatusData.climatisationState.content"
             ),
             "outdoor_temperature": status.getr(
                 "temperatureStatusData.outdoorTemperature.content"
             ),
@@ -499,19 +499,19 @@
             "overallMileage": overall_mileage,
         }
 
 
 class Vehicle:
     """Vehicle class."""
 
-    def __init__(self, data: Any, audi_service: AudiService) -> None:
+    def __init__(self, data: ExtendedDict, audi_service: AudiService) -> None:
         """Initialize."""
         self._audi_service = audi_service
-        self.vin = data.get("vin")
-        self.csid = data.get("csid")
+        self.vin: str = data.get("vin", "")
+        self.csid: str = data.get("csid", "")
         self.model = data.getr("vehicle.media.longName", "")
         self.model_year = data.getr("vehicle.core.modelYear")
         if (nickname := data.get("nickname")) is not None and len(nickname) > 0:
             self.title = nickname
         else:
             self.title = data.getr("vehicle.media.shortName", self.vin)
```

### Comparing `audiconnectpy-1.3.3/audiconnectpy/services.py` & `audiconnectpy-1.3.4/audiconnectpy/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import logging
 from datetime import datetime, timedelta
 from hashlib import sha512
 from typing import Any, Literal
 
 from .auth import Auth
 from .exceptions import AudiException, HttpRequestError, TimeoutExceededError
+from .helpers import ExtendedDict, to_byte_array
 from .models import (
     ChargerDataResponse,
     ClimaterDataResponse,
     DestinationDataResponse,
     HistoryDataResponse,
     PositionDataResponse,
     PreheaterDataResponse,
     TripDataResponse,
     UsersDataResponse,
     VehicleDataResponse,
 )
-from .util import ExtendedDict, to_byte_array
 
 MAX_RESPONSE_ATTEMPTS = 10
 REQUEST_STATUS_SLEEP = 10
 
 SUCCEEDED = "succeeded"
 FAILED = "failed"
 REQUEST_SUCCESSFUL = "request_successful"
```

### Comparing `audiconnectpy-1.3.3/audiconnectpy/util.py` & `audiconnectpy-1.3.4/audiconnectpy/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,22 @@
 
 
 class ExtendedDict(dict[Any, Any]):
     """Extend dictionnary class."""
 
     def getr(self, keys: str, default: Any = None) -> Any:
         """Get recursive attribut."""
-        return reduce(
+        reduce_value: Any = reduce(
             lambda d, key: d.get(key, default) if isinstance(d, dict) else default,
             keys.split("."),
             self,
         )
+        if isinstance(reduce_value, dict):
+            return ExtendedDict(reduce_value)
+        return reduce_value
 
 
 def to_byte_array(hex_string: str) -> list[int]:
     """Return byte array."""
     result = []
     for i in range(0, len(hex_string), 2):
         result.append(int(hex_string[i : i + 2], 16))
```

### Comparing `audiconnectpy-1.3.3/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.3.4/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.3/pyproject.toml` & `audiconnectpy-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.3/setup.py` & `audiconnectpy-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.3",
+    version="1.3.4",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

