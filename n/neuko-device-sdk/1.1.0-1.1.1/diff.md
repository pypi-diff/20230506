# Comparing `tmp/neuko-device-sdk-1.1.0.tar.gz` & `tmp/neuko-device-sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuko-device-sdk-1.1.0.tar", last modified: Mon Nov 28 09:17:43 2022, max compression
+gzip compressed data, was "neuko-device-sdk-1.1.1.tar", last modified: Sat May  6 07:07:33 2023, max compression
```

## Comparing `neuko-device-sdk-1.1.0.tar` & `neuko-device-sdk-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,56 @@
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.710749 neuko-device-sdk-1.1.0/
--rw-r--r--   0 popoimaevi   (501) staff       (20)     1073 2022-02-09 06:51:49.000000 neuko-device-sdk-1.1.0/LICENSE
--rw-r--r--   0 popoimaevi   (501) staff       (20)     7748 2022-11-28 09:17:43.710969 neuko-device-sdk-1.1.0/PKG-INFO
--rw-r--r--   0 popoimaevi   (501) staff       (20)     6981 2022-11-28 09:17:36.000000 neuko-device-sdk-1.1.0/README.md
--rw-r--r--   0 popoimaevi   (501) staff       (20)       76 2022-11-28 09:17:43.711915 neuko-device-sdk-1.1.0/setup.cfg
--rw-r--r--   0 popoimaevi   (501) staff       (20)     1448 2022-11-28 09:17:36.000000 neuko-device-sdk-1.1.0/setup.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     1449 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/setupdev.py
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.685592 neuko-device-sdk-1.1.0/src/
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.688689 neuko-device-sdk-1.1.0/src/neuko/
--rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/__init__.py
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.692498 neuko-device-sdk-1.1.0/src/neuko/connection/
--rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/connection/__init__.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     2435 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/connection/certificateManagement.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     3369 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/src/neuko/connection/certificateStore.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     6192 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/src/neuko/connection/connectionManagement.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     2833 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/connection/connectionStore.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     1821 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/connection/model.py
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.697784 neuko-device-sdk-1.1.0/src/neuko/device/
--rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/device/__init__.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)    40025 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/src/neuko/device/device.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     2137 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/device/deviceManagement.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     5770 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/src/neuko/device/identifierStore.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     2005 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/device/model.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)    13093 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/src/neuko/device/telemetricState.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     7393 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/src/neuko/device/telemetricWorker.py
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.702181 neuko-device-sdk-1.1.0/src/neuko/iot/
--rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/iot/__init__.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     5041 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/iot/bootstrap.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)    14338 2022-04-27 03:44:53.000000 neuko-device-sdk-1.1.0/src/neuko/iot/iot.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)      745 2022-04-26 04:06:04.000000 neuko-device-sdk-1.1.0/src/neuko/iot/model.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)    18294 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/src/neuko/iot/neuko.py
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.703635 neuko-device-sdk-1.1.0/src/neuko/lifecycle/
--rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/lifecycle/__init__.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)     4768 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.0/src/neuko/lifecycle/connectionStateMachine.py
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.706150 neuko-device-sdk-1.1.0/src/neuko/utility/
--rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/utility/__init__.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)      539 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/utility/logger.py
--rw-r--r--   0 popoimaevi   (501) staff       (20)      111 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.0/src/neuko/utility/utils.py
-drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2022-11-28 09:17:43.710205 neuko-device-sdk-1.1.0/src/neuko_device_sdk.egg-info/
--rw-r--r--   0 popoimaevi   (501) staff       (20)     7748 2022-11-28 09:17:43.000000 neuko-device-sdk-1.1.0/src/neuko_device_sdk.egg-info/PKG-INFO
--rw-r--r--   0 popoimaevi   (501) staff       (20)     1035 2022-11-28 09:17:43.000000 neuko-device-sdk-1.1.0/src/neuko_device_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 popoimaevi   (501) staff       (20)        1 2022-11-28 09:17:43.000000 neuko-device-sdk-1.1.0/src/neuko_device_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 popoimaevi   (501) staff       (20)       67 2022-11-28 09:17:43.000000 neuko-device-sdk-1.1.0/src/neuko_device_sdk.egg-info/requires.txt
--rw-r--r--   0 popoimaevi   (501) staff       (20)        6 2022-11-28 09:17:43.000000 neuko-device-sdk-1.1.0/src/neuko_device_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.556115 neuko-device-sdk-1.1.1/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     1073 2022-02-09 06:51:49.000000 neuko-device-sdk-1.1.1/LICENSE
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     7748 2023-05-06 07:07:33.556349 neuko-device-sdk-1.1.1/PKG-INFO
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     6981 2023-05-06 07:07:27.000000 neuko-device-sdk-1.1.1/README.md
+-rw-r--r--   0 popoimaevi   (501) staff       (20)       76 2023-05-06 07:07:33.557195 neuko-device-sdk-1.1.1/setup.cfg
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     1448 2023-05-06 07:07:27.000000 neuko-device-sdk-1.1.1/setup.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     1448 2023-05-06 07:04:14.000000 neuko-device-sdk-1.1.1/setupdev.py
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.531387 neuko-device-sdk-1.1.1/src/
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.533472 neuko-device-sdk-1.1.1/src/neuko/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/__init__.py
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.536261 neuko-device-sdk-1.1.1/src/neuko/connection/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/connection/__init__.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     2435 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/connection/certificateManagement.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     3369 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/src/neuko/connection/certificateStore.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     6192 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/src/neuko/connection/connectionManagement.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     2833 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/connection/connectionStore.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     1821 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/connection/model.py
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.540417 neuko-device-sdk-1.1.1/src/neuko/device/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/device/__init__.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)    40025 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/src/neuko/device/device.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     2137 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/device/deviceManagement.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     5770 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/src/neuko/device/identifierStore.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     2005 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/device/model.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)    13093 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/src/neuko/device/telemetricState.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     7393 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/src/neuko/device/telemetricWorker.py
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.543380 neuko-device-sdk-1.1.1/src/neuko/iot/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/iot/__init__.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     5041 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/iot/bootstrap.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)    14338 2022-04-27 03:44:53.000000 neuko-device-sdk-1.1.1/src/neuko/iot/iot.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)      745 2022-04-26 04:06:04.000000 neuko-device-sdk-1.1.1/src/neuko/iot/model.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)    18373 2023-05-06 07:04:14.000000 neuko-device-sdk-1.1.1/src/neuko/iot/neuko.py
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.544371 neuko-device-sdk-1.1.1/src/neuko/lifecycle/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/lifecycle/__init__.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     4768 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/src/neuko/lifecycle/connectionStateMachine.py
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.546166 neuko-device-sdk-1.1.1/src/neuko/utility/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)        0 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/utility/__init__.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)      539 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/utility/logger.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)      111 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/src/neuko/utility/utils.py
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.549049 neuko-device-sdk-1.1.1/src/neuko_device_sdk.egg-info/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     7748 2023-05-06 07:07:33.000000 neuko-device-sdk-1.1.1/src/neuko_device_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     1377 2023-05-06 07:07:33.000000 neuko-device-sdk-1.1.1/src/neuko_device_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 popoimaevi   (501) staff       (20)        1 2023-05-06 07:07:33.000000 neuko-device-sdk-1.1.1/src/neuko_device_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 popoimaevi   (501) staff       (20)       67 2023-05-06 07:07:33.000000 neuko-device-sdk-1.1.1/src/neuko_device_sdk.egg-info/requires.txt
+-rw-r--r--   0 popoimaevi   (501) staff       (20)        6 2023-05-06 07:07:33.000000 neuko-device-sdk-1.1.1/src/neuko_device_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 popoimaevi   (501) staff       (20)        0 2023-05-06 07:07:33.555576 neuko-device-sdk-1.1.1/tests/
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     5278 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/tests/test_01_identifierStore.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     4138 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/tests/test_02_deviceManagement.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     2206 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/tests/test_03_certificateStore.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     4898 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/tests/test_04_certificateManagement.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)      706 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/tests/test_05_connectionStore.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     6831 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/tests/test_06_connectionManagement.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)     4021 2022-03-14 04:06:47.000000 neuko-device-sdk-1.1.1/tests/test_07_worker.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)    13693 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/tests/test_08_telemetricState.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)    12636 2022-11-28 09:17:03.000000 neuko-device-sdk-1.1.1/tests/test_09_bootstrap.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)    14716 2023-05-06 07:04:14.000000 neuko-device-sdk-1.1.1/tests/test_10_neuko.py
+-rw-r--r--   0 popoimaevi   (501) staff       (20)    17860 2023-05-06 07:04:14.000000 neuko-device-sdk-1.1.1/tests/test_11_device.py
```

### Comparing `neuko-device-sdk-1.1.0/LICENSE` & `neuko-device-sdk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/PKG-INFO` & `neuko-device-sdk-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuko-device-sdk
-Version: 1.1.0
+Version: 1.1.1
 Summary: Neuko device SDK for Python hardware
 Author: neuko.io
 Author-email: hello@neuko.io
 License: MIT
 Keywords: iot,device,thing,cloud,mqtt,development,neuko
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `neuko-device-sdk-1.1.0/README.md` & `neuko-device-sdk-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/setup.py` & `neuko-device-sdk-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = long_description.replace("\r","")
 except(IOError, ImportError):
     long_description = open('README.md').read()
 
 
 setup(
     name='neuko-device-sdk',
-    version='1.1.0',
+    version='1.1.1',
     license='MIT',
     description="Neuko device SDK for Python hardware",
     long_description= long_description,
     long_description_content_type="text/markdown",
     author="neuko.io",
     author_email='hello@neuko.io',
     packages=find_packages('src'),
```

### Comparing `neuko-device-sdk-1.1.0/setupdev.py` & `neuko-device-sdk-1.1.1/setupdev.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = long_description.replace("\r","")
 except(IOError, ImportError):
     long_description = open('README.md').read()
 
 
 setup(
     name='neuko-device-sdk',
-    version='1.0.22',
+    version='1.1.1',
     license='MIT',
     description="Neuko device SDK for Python hardware",
     long_description= long_description,
     long_description_content_type="text/markdown",
     author="neuko.io",
     author_email='hello@neuko.io',
     packages=find_packages('src'),
```

### Comparing `neuko-device-sdk-1.1.0/src/neuko/connection/certificateManagement.py` & `neuko-device-sdk-1.1.1/src/neuko/connection/certificateManagement.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/connection/certificateStore.py` & `neuko-device-sdk-1.1.1/src/neuko/connection/certificateStore.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/connection/connectionManagement.py` & `neuko-device-sdk-1.1.1/src/neuko/connection/connectionManagement.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/connection/connectionStore.py` & `neuko-device-sdk-1.1.1/src/neuko/connection/connectionStore.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/connection/model.py` & `neuko-device-sdk-1.1.1/src/neuko/connection/model.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/device/device.py` & `neuko-device-sdk-1.1.1/src/neuko/device/device.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/device/deviceManagement.py` & `neuko-device-sdk-1.1.1/src/neuko/device/deviceManagement.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/device/identifierStore.py` & `neuko-device-sdk-1.1.1/src/neuko/device/identifierStore.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/device/model.py` & `neuko-device-sdk-1.1.1/src/neuko/device/model.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/device/telemetricState.py` & `neuko-device-sdk-1.1.1/src/neuko/device/telemetricState.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/device/telemetricWorker.py` & `neuko-device-sdk-1.1.1/src/neuko/device/telemetricWorker.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/iot/bootstrap.py` & `neuko-device-sdk-1.1.1/src/neuko/iot/bootstrap.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/iot/iot.py` & `neuko-device-sdk-1.1.1/src/neuko/iot/iot.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/iot/model.py` & `neuko-device-sdk-1.1.1/src/neuko/iot/model.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/iot/neuko.py` & `neuko-device-sdk-1.1.1/src/neuko/iot/neuko.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import paho.mqtt.client as Mqtt
 import aiohttp
 import uuid
 import json
 import asyncio
 import inspect
 import threading
-from datetime import datetime
+from datetime import datetime, timezone
 from paho.mqtt.client import MQTTMessage
 from .iot import IoT
 from .model import AwsUpdateDelta, UpdateDelta
 from ..utility.logger import Logger
 from ..connection.model import ConfigurationProtocol, Certificate
 from ..device.deviceManagement import DeviceManagement
 from ..connection.certificateManagement import CertificateManagement
@@ -299,25 +299,25 @@
             logger.error(ex)
             raise Exception(ex)
 
     async def timestreamStorage(self, stateName: str, state: object) -> None:
         try:
             # init var
             deviceId = DeviceManagement.resolveDeviceUniqueId(self._deviceIdentifier)
-            now = datetime.now()
+            now = datetime.now(timezone.utc).isoformat(timespec='milliseconds').replace('+00:00', 'Z')
             payload = {
                 'device_id': deviceId,
                 'state_name': stateName,
-                'timestamp': now.isoformat(),
+                'timestamp': now,
                 'data': state
             }
             logger.debug(f'timestreamStorage: payload = {payload}')
 
             await self.publish(
-                f'{AWS_PREFIX}/{RULES_PREFIX}/{TIMESTREAMRULE}',
+                f'{AWS_PREFIX}/{RULES_PREFIX}/{TIMESTREAMRULE}/{deviceId}',
                 json.dumps(payload)
             )
         except Exception as ex:
             logger.error(ex)
             raise Exception(ex)
 
     async def onTelemetricStateChangedRequest(self, context, listener) -> None:
```

### Comparing `neuko-device-sdk-1.1.0/src/neuko/lifecycle/connectionStateMachine.py` & `neuko-device-sdk-1.1.1/src/neuko/lifecycle/connectionStateMachine.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko/utility/logger.py` & `neuko-device-sdk-1.1.1/src/neuko/utility/logger.py`

 * *Files identical despite different names*

### Comparing `neuko-device-sdk-1.1.0/src/neuko_device_sdk.egg-info/PKG-INFO` & `neuko-device-sdk-1.1.1/src/neuko_device_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuko-device-sdk
-Version: 1.1.0
+Version: 1.1.1
 Summary: Neuko device SDK for Python hardware
 Author: neuko.io
 Author-email: hello@neuko.io
 License: MIT
 Keywords: iot,device,thing,cloud,mqtt,development,neuko
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

