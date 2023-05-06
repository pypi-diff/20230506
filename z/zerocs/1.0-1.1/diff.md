# Comparing `tmp/zerocs-1.0.tar.gz` & `tmp/zerocs-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocs-1.0.tar", last modified: Wed Apr 26 15:18:07 2023, max compression
+gzip compressed data, was "zerocs-1.1.tar", last modified: Sat May  6 12:07:04 2023, max compression
```

## Comparing `zerocs-1.0.tar` & `zerocs-1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/
--rw-r--r--   0 yanping   (1000) yanping   (1000)    18156 2023-04-26 15:18:07.091022 zerocs-1.0/PKG-INFO
--rw-r--r--   0 yanping   (1000) yanping   (1000)       38 2023-04-26 15:18:07.091022 zerocs-1.0/setup.cfg
--rw-r--r--   0 yanping   (1000) yanping   (1000)      867 2023-04-26 15:17:55.000000 zerocs-1.0/setup.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs/
--rw-r--r--   0 yanping   (1000) yanping   (1000)     4765 2023-04-26 13:53:23.000000 zerocs-1.0/zerocs/__init__.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs/base/
--rw-r--r--   0 yanping   (1000) yanping   (1000)      134 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/base/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1845 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/base/_base.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     7208 2023-04-26 13:20:00.000000 zerocs-1.0/zerocs/base/_default_func.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      496 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/base/_function.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     2674 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/base/base_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      529 2023-04-26 13:20:00.000000 zerocs-1.0/zerocs/base/default_func_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      670 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/base/function_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs/fork/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       35 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/fork/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1993 2023-04-22 03:18:59.000000 zerocs-1.0/zerocs/fork/_func.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1115 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/fork/fork_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs/logger/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       41 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/logger/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1860 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/logger/_logger.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      392 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/logger/logger_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     7354 2023-04-26 13:20:00.000000 zerocs-1.0/zerocs/mate.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/network/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       44 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/network/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      425 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/network/_network.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      508 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/network/network_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/rabbitmq/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       47 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/rabbitmq/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1288 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/rabbitmq/_rabbitmq.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1293 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/rabbitmq/rabbitmq_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/script/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       39 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/script/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1460 2023-04-26 13:20:00.000000 zerocs-1.0/zerocs/script/_queue.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      708 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/script/queue_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/snowflakeId/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       55 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/snowflakeId/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     1918 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/snowflakeId/_snowflakeId.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)      469 2023-04-19 11:33:05.000000 zerocs-1.0/zerocs/snowflakeId/snowflakeId.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.091022 zerocs-1.0/zerocs/sqlite/
--rw-r--r--   0 yanping   (1000) yanping   (1000)       42 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/sqlite/__init__.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     5529 2023-04-20 04:53:25.000000 zerocs-1.0/zerocs/sqlite/_sqlite.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)     3577 2023-04-20 03:18:43.000000 zerocs-1.0/zerocs/sqlite/sqlite3_.py
--rw-r--r--   0 yanping   (1000) yanping   (1000)    11296 2023-04-26 13:20:22.000000 zerocs-1.0/zerocs/zerocs_.py
-drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-04-26 15:18:07.087022 zerocs-1.0/zerocs.egg-info/
--rw-r--r--   0 yanping   (1000) yanping   (1000)    18156 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/PKG-INFO
--rw-r--r--   0 yanping   (1000) yanping   (1000)      943 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/SOURCES.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)        1 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/dependency_links.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)       12 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/requires.txt
--rw-r--r--   0 yanping   (1000) yanping   (1000)        7 2023-04-26 15:18:07.000000 zerocs-1.0/zerocs.egg-info/top_level.txt
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    18156 2023-05-06 12:07:04.484085 zerocs-1.1/PKG-INFO
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       38 2023-05-06 12:07:04.484085 zerocs-1.1/setup.cfg
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      867 2023-05-06 12:06:49.000000 zerocs-1.1/setup.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     4765 2023-04-26 13:53:23.000000 zerocs-1.1/zerocs/__init__.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/base/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      134 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/base/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1845 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/base/_base.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     7208 2023-04-26 13:20:00.000000 zerocs-1.1/zerocs/base/_default_func.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      496 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/base/_function.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     2674 2023-04-19 11:33:05.000000 zerocs-1.1/zerocs/base/base_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      529 2023-04-26 13:20:00.000000 zerocs-1.1/zerocs/base/default_func_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      670 2023-04-19 11:33:05.000000 zerocs-1.1/zerocs/base/function_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/fork/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       35 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/fork/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1993 2023-04-22 03:18:59.000000 zerocs-1.1/zerocs/fork/_func.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1115 2023-04-19 11:33:05.000000 zerocs-1.1/zerocs/fork/fork_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/logger/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       41 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/logger/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1860 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/logger/_logger.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      392 2023-04-19 11:33:05.000000 zerocs-1.1/zerocs/logger/logger_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     7354 2023-04-26 13:20:00.000000 zerocs-1.1/zerocs/mate.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/network/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       44 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/network/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      425 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/network/_network.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      508 2023-04-19 11:33:05.000000 zerocs-1.1/zerocs/network/network_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/rabbitmq/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       47 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/rabbitmq/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1288 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/rabbitmq/_rabbitmq.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1293 2023-04-19 11:33:05.000000 zerocs-1.1/zerocs/rabbitmq/rabbitmq_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/script/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       39 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/script/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1460 2023-04-26 13:20:00.000000 zerocs-1.1/zerocs/script/_queue.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      708 2023-04-19 11:33:05.000000 zerocs-1.1/zerocs/script/queue_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/snowflakeId/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       55 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/snowflakeId/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     1918 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/snowflakeId/_snowflakeId.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      469 2023-04-19 11:33:05.000000 zerocs-1.1/zerocs/snowflakeId/snowflakeId.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs/sqlite/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       42 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/sqlite/__init__.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     5529 2023-04-20 04:53:25.000000 zerocs-1.1/zerocs/sqlite/_sqlite.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)     3577 2023-04-20 03:18:43.000000 zerocs-1.1/zerocs/sqlite/sqlite3_.py
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    11546 2023-05-06 12:04:57.000000 zerocs-1.1/zerocs/zerocs_.py
+drwxr-xr-x   0 yanping   (1000) yanping   (1000)        0 2023-05-06 12:07:04.484085 zerocs-1.1/zerocs.egg-info/
+-rw-r--r--   0 yanping   (1000) yanping   (1000)    18156 2023-05-06 12:07:04.000000 zerocs-1.1/zerocs.egg-info/PKG-INFO
+-rw-r--r--   0 yanping   (1000) yanping   (1000)      943 2023-05-06 12:07:04.000000 zerocs-1.1/zerocs.egg-info/SOURCES.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)        1 2023-05-06 12:07:04.000000 zerocs-1.1/zerocs.egg-info/dependency_links.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)       12 2023-05-06 12:07:04.000000 zerocs-1.1/zerocs.egg-info/requires.txt
+-rw-r--r--   0 yanping   (1000) yanping   (1000)        7 2023-05-06 12:07:04.000000 zerocs-1.1/zerocs.egg-info/top_level.txt
```

### Comparing `zerocs-1.0/PKG-INFO` & `zerocs-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocs
-Version: 1.0
+Version: 1.1
 Summary: zerocs
 Home-page: https://github.com/ZYPGITA/zerocs
 Author: YanPing
 Author-email: zyphhxx@foxmail.com
 Maintainer: YanPing
 Maintainer-email: zyphhxx@foxmail.com
 License: MIT License
```

### Comparing `zerocs-1.0/setup.py` & `zerocs-1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zerocs',
-    version='1.0',
+    version='1.1',
     description="zerocs",
     long_description=open('zerocs/README.rst').read(),
     # long_description_content_type='text/plain',
     include_package_data=True,
     author='YanPing',
     author_email='zyphhxx@foxmail.com',
     maintainer='YanPing',
```

### Comparing `zerocs-1.0/zerocs/__init__.py` & `zerocs-1.1/zerocs/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/base/_base.py` & `zerocs-1.1/zerocs/base/_base.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/base/_default_func.py` & `zerocs-1.1/zerocs/base/_default_func.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/base/base_.py` & `zerocs-1.1/zerocs/base/base_.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/base/default_func_.py` & `zerocs-1.1/zerocs/base/default_func_.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/base/function_.py` & `zerocs-1.1/zerocs/base/function_.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/fork/_func.py` & `zerocs-1.1/zerocs/fork/_func.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/fork/fork_.py` & `zerocs-1.1/zerocs/fork/fork_.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/logger/_logger.py` & `zerocs-1.1/zerocs/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/mate.py` & `zerocs-1.1/zerocs/mate.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/rabbitmq/_rabbitmq.py` & `zerocs-1.1/zerocs/rabbitmq/_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/rabbitmq/rabbitmq_.py` & `zerocs-1.1/zerocs/rabbitmq/rabbitmq_.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/script/_queue.py` & `zerocs-1.1/zerocs/script/_queue.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/script/queue_.py` & `zerocs-1.1/zerocs/script/queue_.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/snowflakeId/_snowflakeId.py` & `zerocs-1.1/zerocs/snowflakeId/_snowflakeId.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/sqlite/_sqlite.py` & `zerocs-1.1/zerocs/sqlite/_sqlite.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/sqlite/sqlite3_.py` & `zerocs-1.1/zerocs/sqlite/sqlite3_.py`

 * *Files identical despite different names*

### Comparing `zerocs-1.0/zerocs/zerocs_.py` & `zerocs-1.1/zerocs/zerocs_.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,21 @@
             self._add_service(service, service_id, queue_pid, rpc_pid)
 
     def _get_all_service(self):
         """
         Get All Service
         :return:
         """
-        return self._sqlite_get_all_service()
+        all_service = self._sqlite_get_all_service()
+        _service_list = []
+        for s in all_service:
+            service_name = s['service_name']
+            if service_name not in ['zerocs_service', 'zerocs_config']:
+                _service_list.append(s)
+        return _service_list
 
     def get_snowflake_id(self):
         """
         Obtain IDs, with a maximum of 4000 retrieved per millisecond
         :return:
         """
         return self._get_snowflake_id(datacenter_id=0, worker_id=0, did_wid=-1)
```

### Comparing `zerocs-1.0/zerocs.egg-info/PKG-INFO` & `zerocs-1.1/zerocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocs
-Version: 1.0
+Version: 1.1
 Summary: zerocs
 Home-page: https://github.com/ZYPGITA/zerocs
 Author: YanPing
 Author-email: zyphhxx@foxmail.com
 Maintainer: YanPing
 Maintainer-email: zyphhxx@foxmail.com
 License: MIT License
```

### Comparing `zerocs-1.0/zerocs.egg-info/SOURCES.txt` & `zerocs-1.1/zerocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

