# Comparing `tmp/luckyun-nacos-0.1.0.tar.gz` & `tmp/luckyun-nacos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luckyun-nacos-0.1.0.tar", last modified: Fri Apr 28 01:34:40 2023, max compression
+gzip compressed data, was "luckyun-nacos-0.2.0.tar", last modified: Sat May  6 06:35:53 2023, max compression
```

## Comparing `luckyun-nacos-0.1.0.tar` & `luckyun-nacos-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 peiyandong   (501) staff       (20)        0 2023-04-28 01:34:40.824171 luckyun-nacos-0.1.0/
--rw-r--r--   0 peiyandong   (501) staff       (20)      483 2023-04-28 01:34:40.824045 luckyun-nacos-0.1.0/PKG-INFO
--rw-r--r--   0 peiyandong   (501) staff       (20)       16 2023-04-27 03:20:09.000000 luckyun-nacos-0.1.0/README.md
-drwxr-xr-x   0 peiyandong   (501) staff       (20)        0 2023-04-28 01:34:40.822889 luckyun-nacos-0.1.0/luckyun_nacos/
--rw-r--r--   0 peiyandong   (501) staff       (20)       26 2023-04-25 09:38:04.000000 luckyun-nacos-0.1.0/luckyun_nacos/__init__.py
--rw-r--r--   0 peiyandong   (501) staff       (20)     1882 2023-04-28 00:52:15.000000 luckyun-nacos-0.1.0/luckyun_nacos/client.py
-drwxr-xr-x   0 peiyandong   (501) staff       (20)        0 2023-04-28 01:34:40.823567 luckyun-nacos-0.1.0/luckyun_nacos.egg-info/
--rw-r--r--   0 peiyandong   (501) staff       (20)      483 2023-04-28 01:34:40.000000 luckyun-nacos-0.1.0/luckyun_nacos.egg-info/PKG-INFO
--rw-r--r--   0 peiyandong   (501) staff       (20)      291 2023-04-28 01:34:40.000000 luckyun-nacos-0.1.0/luckyun_nacos.egg-info/SOURCES.txt
--rw-r--r--   0 peiyandong   (501) staff       (20)        1 2023-04-28 01:34:40.000000 luckyun-nacos-0.1.0/luckyun_nacos.egg-info/dependency_links.txt
--rw-r--r--   0 peiyandong   (501) staff       (20)      169 2023-04-28 01:34:40.000000 luckyun-nacos-0.1.0/luckyun_nacos.egg-info/requires.txt
--rw-r--r--   0 peiyandong   (501) staff       (20)       20 2023-04-28 01:34:40.000000 luckyun-nacos-0.1.0/luckyun_nacos.egg-info/top_level.txt
--rw-r--r--   0 peiyandong   (501) staff       (20)       38 2023-04-28 01:34:40.824205 luckyun-nacos-0.1.0/setup.cfg
--rw-r--r--   0 peiyandong   (501) staff       (20)      702 2023-04-28 01:33:00.000000 luckyun-nacos-0.1.0/setup.py
-drwxr-xr-x   0 peiyandong   (501) staff       (20)        0 2023-04-28 01:34:40.823844 luckyun-nacos-0.1.0/tests/
--rw-r--r--   0 peiyandong   (501) staff       (20)        0 2023-04-25 09:34:32.000000 luckyun-nacos-0.1.0/tests/__init__.py
--rw-r--r--   0 peiyandong   (501) staff       (20)      947 2023-04-27 09:59:20.000000 luckyun-nacos-0.1.0/tests/test_client.py
+drwxr-xr-x   0 peiyandong   (501) staff       (20)        0 2023-05-06 06:35:53.311261 luckyun-nacos-0.2.0/
+-rw-r--r--   0 peiyandong   (501) staff       (20)      483 2023-05-06 06:35:53.311138 luckyun-nacos-0.2.0/PKG-INFO
+-rw-r--r--   0 peiyandong   (501) staff       (20)      743 2023-05-06 06:03:33.000000 luckyun-nacos-0.2.0/README.md
+drwxr-xr-x   0 peiyandong   (501) staff       (20)        0 2023-05-06 06:35:53.309713 luckyun-nacos-0.2.0/luckyun_nacos/
+-rw-r--r--   0 peiyandong   (501) staff       (20)       26 2023-04-25 09:38:04.000000 luckyun-nacos-0.2.0/luckyun_nacos/__init__.py
+-rw-r--r--   0 peiyandong   (501) staff       (20)     1957 2023-05-04 09:43:12.000000 luckyun-nacos-0.2.0/luckyun_nacos/client.py
+drwxr-xr-x   0 peiyandong   (501) staff       (20)        0 2023-05-06 06:35:53.310620 luckyun-nacos-0.2.0/luckyun_nacos.egg-info/
+-rw-r--r--   0 peiyandong   (501) staff       (20)      483 2023-05-06 06:35:53.000000 luckyun-nacos-0.2.0/luckyun_nacos.egg-info/PKG-INFO
+-rw-r--r--   0 peiyandong   (501) staff       (20)      291 2023-05-06 06:35:53.000000 luckyun-nacos-0.2.0/luckyun_nacos.egg-info/SOURCES.txt
+-rw-r--r--   0 peiyandong   (501) staff       (20)        1 2023-05-06 06:35:53.000000 luckyun-nacos-0.2.0/luckyun_nacos.egg-info/dependency_links.txt
+-rw-r--r--   0 peiyandong   (501) staff       (20)      191 2023-05-06 06:35:53.000000 luckyun-nacos-0.2.0/luckyun_nacos.egg-info/requires.txt
+-rw-r--r--   0 peiyandong   (501) staff       (20)       20 2023-05-06 06:35:53.000000 luckyun-nacos-0.2.0/luckyun_nacos.egg-info/top_level.txt
+-rw-r--r--   0 peiyandong   (501) staff       (20)       38 2023-05-06 06:35:53.311309 luckyun-nacos-0.2.0/setup.cfg
+-rw-r--r--   0 peiyandong   (501) staff       (20)      702 2023-05-06 05:47:51.000000 luckyun-nacos-0.2.0/setup.py
+drwxr-xr-x   0 peiyandong   (501) staff       (20)        0 2023-05-06 06:35:53.310816 luckyun-nacos-0.2.0/tests/
+-rw-r--r--   0 peiyandong   (501) staff       (20)        0 2023-04-25 09:34:32.000000 luckyun-nacos-0.2.0/tests/__init__.py
+-rw-r--r--   0 peiyandong   (501) staff       (20)     1120 2023-05-04 09:33:56.000000 luckyun-nacos-0.2.0/tests/test_client.py
```

### Comparing `luckyun-nacos-0.1.0/luckyun_nacos/client.py` & `luckyun-nacos-0.2.0/luckyun_nacos/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import nacos
 import asyncio
 import threading
 import yaml
+from luckyun_logger import get_logger
+
+logger = get_logger(__name__)
 
 class Client():
     def __init__(self, server_addresses, service_name=None, service_ip=None, service_port: int = None, heartbeat_rate = 15, endpoint=None, namespace=None, ak=None, sk=None, username=None, password=None):
 
         self.service_name = service_name
         self.service_ip = service_ip
         self.service_port = service_port
@@ -32,15 +35,15 @@
     async def remove_instance(self):
         self.client.remove_naming_instance(
             self.service_name, self.service_ip, self.service_port)
 
     async def task_nacos_heartbeat(self):
         while True:
             await asyncio.sleep(self.heartbeat_rate)
-            print("send_heartbeat")
+            logger.info("send_heartbeat")
             self.client.send_heartbeat(
                 self.service_name, self.service_ip, self.service_port)
 
     async def run_nacos_heartbeat(self):
         task = asyncio.create_task(self.task_nacos_heartbeat())
         await task
```

### Comparing `luckyun-nacos-0.1.0/setup.py` & `luckyun-nacos-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='luckyun-nacos',
-    version='0.1.0',
+    version='0.2.0',
     description='Nacos client',
     author='lucksoft',
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

