# Comparing `tmp/renault-api-lite-0.8.1.tar.gz` & `tmp/renault-api-lite-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renault-api-lite-0.8.1.tar", last modified: Mon Dec 26 13:18:59 2022, max compression
+gzip compressed data, was "renault-api-lite-0.8.2.tar", last modified: Sat May  6 11:14:06 2023, max compression
```

## Comparing `renault-api-lite-0.8.1.tar` & `renault-api-lite-0.8.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:18:59.609406 renault-api-lite-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-26 13:18:43.000000 renault-api-lite-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2022-12-26 13:18:59.609406 renault-api-lite-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2022-12-26 13:18:43.000000 renault-api-lite-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:18:59.609406 renault-api-lite-0.8.1/renault/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-26 13:18:43.000000 renault-api-lite-0.8.1/renault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-26 13:18:43.000000 renault-api-lite-0.8.1/renault/excpetion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20415 2022-12-26 13:18:43.000000 renault-api-lite-0.8.1/renault/renault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 13:18:59.609406 renault-api-lite-0.8.1/renault_api_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2022-12-26 13:18:59.000000 renault-api-lite-0.8.1/renault_api_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2022-12-26 13:18:59.000000 renault-api-lite-0.8.1/renault_api_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-26 13:18:59.000000 renault-api-lite-0.8.1/renault_api_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-26 13:18:59.000000 renault-api-lite-0.8.1/renault_api_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-26 13:18:59.000000 renault-api-lite-0.8.1/renault_api_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-26 13:18:59.609406 renault-api-lite-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2022-12-26 13:18:43.000000 renault-api-lite-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:14:06.264905 renault-api-lite-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-06 11:13:55.000000 renault-api-lite-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-06 11:14:06.264905 renault-api-lite-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-06 11:13:55.000000 renault-api-lite-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:14:06.264905 renault-api-lite-0.8.2/renault/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:13:55.000000 renault-api-lite-0.8.2/renault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-06 11:13:55.000000 renault-api-lite-0.8.2/renault/excpetion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-05-06 11:13:55.000000 renault-api-lite-0.8.2/renault/renault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:14:06.264905 renault-api-lite-0.8.2/renault_api_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-06 11:14:06.000000 renault-api-lite-0.8.2/renault_api_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-06 11:14:06.000000 renault-api-lite-0.8.2/renault_api_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 11:14:06.000000 renault-api-lite-0.8.2/renault_api_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 11:14:06.000000 renault-api-lite-0.8.2/renault_api_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 11:14:06.000000 renault-api-lite-0.8.2/renault_api_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 11:14:06.264905 renault-api-lite-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-06 11:13:55.000000 renault-api-lite-0.8.2/setup.py
```

### Comparing `renault-api-lite-0.8.1/LICENSE` & `renault-api-lite-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `renault-api-lite-0.8.1/PKG-INFO` & `renault-api-lite-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renault-api-lite
-Version: 0.8.1
+Version: 0.8.2
 Summary: Lightweight Python API for querying status info for a variety of Renault vehicle models
 Home-page: https://github.com/bkogler/renault-api-lite
 Author: Bernhard Kogler
 Author-email: bernhard.kogler@supersonnig.org
 License: MIT
 Keywords: Renault Z.E. ZOE Twingo Megane Kangoo Electric vehicle EV status API
 Classifier: Development Status :: 5 - Production/Stable
@@ -54,15 +54,15 @@
 {
     "battery_status_data": {
         "timestamp": "2022-08-145T07:24:12Z",
         "battery_level": 90,
         "battery_temperature": 25,
         "battery_autonomy": 207,
         "battery_capacity": 0,
-        "battery_available_energy": 10,
+        "battery_available_energy": 20,
         "plug_status": 0,
         "charging_status": -1.1,
         "charging_remaining_rime": 10,
         "charging_instantaneous_power": 0.0
     }
 }
 ````
@@ -85,15 +85,15 @@
 {
     "battery_status_data": {
         "timestamp": "2022-08-145T07:24:12Z",
         "battery_level": 90,
         "battery_temperature": 25,
         "battery_autonomy": 207,
         "battery_capacity": 0,
-        "battery_available_energy": 10,
+        "battery_available_energy": 20,
         "plug_status": 0,
         "charging_status": -1.1,
         "charging_remaining_rime": 10,
         "charging_instantaneous_power": 0.0
     },
     "cockpit_data": {
         "fuel_autonomy": null,
@@ -106,10 +106,12 @@
 # Disclaimer
 This project is not affiliated with, endorsed by, or connected to Renault. I accept no responsibility for any consequences, intended or accidental, as a result of interacting with Renault's API using this project.
 
 # Credits
 This project is based on [hacf-fr's renault-api](https://github.com/hacf-fr/renault-api) for Python
 
 # Links
-[renault-api-lite repository](https://github.com/bkogler/renault-api-lite)
+[renault-api-lite GitHub repository](https://github.com/bkogler/renault-api-lite)
+
+[renault-api-lite on PyPi](https://pypi.org/project/renault-api-lite/)
 
 [hacf-fr's renault-api](https://github.com/hacf-fr/renault-api)
```

### Comparing `renault-api-lite-0.8.1/README.md` & `renault-api-lite-0.8.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 {
     "battery_status_data": {
         "timestamp": "2022-08-145T07:24:12Z",
         "battery_level": 90,
         "battery_temperature": 25,
         "battery_autonomy": 207,
         "battery_capacity": 0,
-        "battery_available_energy": 10,
+        "battery_available_energy": 20,
         "plug_status": 0,
         "charging_status": -1.1,
         "charging_remaining_rime": 10,
         "charging_instantaneous_power": 0.0
     }
 }
 ````
@@ -68,15 +68,15 @@
 {
     "battery_status_data": {
         "timestamp": "2022-08-145T07:24:12Z",
         "battery_level": 90,
         "battery_temperature": 25,
         "battery_autonomy": 207,
         "battery_capacity": 0,
-        "battery_available_energy": 10,
+        "battery_available_energy": 20,
         "plug_status": 0,
         "charging_status": -1.1,
         "charging_remaining_rime": 10,
         "charging_instantaneous_power": 0.0
     },
     "cockpit_data": {
         "fuel_autonomy": null,
@@ -89,10 +89,12 @@
 # Disclaimer
 This project is not affiliated with, endorsed by, or connected to Renault. I accept no responsibility for any consequences, intended or accidental, as a result of interacting with Renault's API using this project.
 
 # Credits
 This project is based on [hacf-fr's renault-api](https://github.com/hacf-fr/renault-api) for Python
 
 # Links
-[renault-api-lite repository](https://github.com/bkogler/renault-api-lite)
+[renault-api-lite GitHub repository](https://github.com/bkogler/renault-api-lite)
+
+[renault-api-lite on PyPi](https://pypi.org/project/renault-api-lite/)
 
 [hacf-fr's renault-api](https://github.com/hacf-fr/renault-api)
```

### Comparing `renault-api-lite-0.8.1/renault/renault.py` & `renault-api-lite-0.8.2/renault/renault.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,18 +275,19 @@
     def __initialize_backend(self) -> None:
         """
         Internal method that brings preparations in place for underlying renault-api client (backend) and its async
         context
 
         :return:
         """
+        # save event loop for further usage with later async calls
         self.__async_loop = asyncio.get_event_loop_policy().get_event_loop()
-        self.__aiohttp_client_session = aiohttp.ClientSession(
-            timeout=ClientTimeout(total=self.__timeout),
-            loop=self.__async_loop)
+
+        # prepare AIOHTTP client session (automatically uses the asyncio event loop of the current thread)
+        self.__aiohttp_client_session = aiohttp.ClientSession(timeout=ClientTimeout(total=self.__timeout))
 
         self.__renault_client = RenaultClient(websession=self.__aiohttp_client_session, locale=self.__account_locale)
 
     def __run_async(self, coroutine: Coroutine) -> Any:
         """
         Internal method to run a coroutine using the instance's async context
 
@@ -445,22 +446,14 @@
             vehicle_list.append({
                 "model": model,
                 "vin": vin
             })
 
         return vehicle_list
 
-    def __del__(self) -> None:
-        """
-        Housekeeping: Close open http client session
-        :return:
-        """
-        if not self.__async_loop.is_closed() and self.__aiohttp_client_session:
-            self.__run_async(self.__aiohttp_client_session.close())
-
     def get_status(self, status_type: StatusType | Tuple[StatusType, ...] = STATUS_MINIMUM) \
             -> OrderedDict[str, Any]:
         """
         Retrieves and returns vehicle status
 
         :param status_type: Single StatusType element or tuple of StatusType elements to request from backend.
             Several predefined Tuples are available as class variable.
```

### Comparing `renault-api-lite-0.8.1/renault_api_lite.egg-info/PKG-INFO` & `renault-api-lite-0.8.2/renault_api_lite.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renault-api-lite
-Version: 0.8.1
+Version: 0.8.2
 Summary: Lightweight Python API for querying status info for a variety of Renault vehicle models
 Home-page: https://github.com/bkogler/renault-api-lite
 Author: Bernhard Kogler
 Author-email: bernhard.kogler@supersonnig.org
 License: MIT
 Keywords: Renault Z.E. ZOE Twingo Megane Kangoo Electric vehicle EV status API
 Classifier: Development Status :: 5 - Production/Stable
@@ -54,15 +54,15 @@
 {
     "battery_status_data": {
         "timestamp": "2022-08-145T07:24:12Z",
         "battery_level": 90,
         "battery_temperature": 25,
         "battery_autonomy": 207,
         "battery_capacity": 0,
-        "battery_available_energy": 10,
+        "battery_available_energy": 20,
         "plug_status": 0,
         "charging_status": -1.1,
         "charging_remaining_rime": 10,
         "charging_instantaneous_power": 0.0
     }
 }
 ````
@@ -85,15 +85,15 @@
 {
     "battery_status_data": {
         "timestamp": "2022-08-145T07:24:12Z",
         "battery_level": 90,
         "battery_temperature": 25,
         "battery_autonomy": 207,
         "battery_capacity": 0,
-        "battery_available_energy": 10,
+        "battery_available_energy": 20,
         "plug_status": 0,
         "charging_status": -1.1,
         "charging_remaining_rime": 10,
         "charging_instantaneous_power": 0.0
     },
     "cockpit_data": {
         "fuel_autonomy": null,
@@ -106,10 +106,12 @@
 # Disclaimer
 This project is not affiliated with, endorsed by, or connected to Renault. I accept no responsibility for any consequences, intended or accidental, as a result of interacting with Renault's API using this project.
 
 # Credits
 This project is based on [hacf-fr's renault-api](https://github.com/hacf-fr/renault-api) for Python
 
 # Links
-[renault-api-lite repository](https://github.com/bkogler/renault-api-lite)
+[renault-api-lite GitHub repository](https://github.com/bkogler/renault-api-lite)
+
+[renault-api-lite on PyPi](https://pypi.org/project/renault-api-lite/)
 
 [hacf-fr's renault-api](https://github.com/hacf-fr/renault-api)
```

### Comparing `renault-api-lite-0.8.1/setup.py` & `renault-api-lite-0.8.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='renault-api-lite',
-    version='0.8.1',
+    version='0.8.2',
     packages=['renault'],
     url='https://github.com/bkogler/renault-api-lite',
     license='MIT',
     author='Bernhard Kogler',
     author_email='bernhard.kogler@supersonnig.org',
     description='Lightweight Python API for querying status info for a variety of Renault vehicle models',
     long_description=long_description,
@@ -21,10 +21,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords="Renault Z.E. ZOE Twingo Megane Kangoo Electric vehicle EV status API",
     python_requires='>=3.10',
     install_requires=[
-        'renault-api>=0.1.11'
+        'renault-api>=0.1.13'
     ]
 )
```

