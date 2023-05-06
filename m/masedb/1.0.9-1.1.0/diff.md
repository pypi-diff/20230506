# Comparing `tmp/masedb-1.0.9.tar.gz` & `tmp/masedb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\masedb-1.0.9.tar", last modified: Sat May  6 02:35:52 2023, max compression
+gzip compressed data, was "dist\masedb-1.1.0.tar", last modified: Sat May  6 02:39:38 2023, max compression
```

## Comparing `masedb-1.0.9.tar` & `masedb-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:52.000000 masedb-1.0.9/
--rw-rw-rw-   0        0        0     2290 2023-05-06 01:50:34.000000 masedb-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     2151 2023-05-06 02:35:52.000000 masedb-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1839 2023-05-06 02:12:56.000000 masedb-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:52.000000 masedb-1.0.9/masedb/
--rw-rw-rw-   0        0        0      783 2023-05-06 02:08:47.000000 masedb-1.0.9/masedb/connect.py
--rw-rw-rw-   0        0        0      703 2023-05-06 02:33:48.000000 masedb-1.0.9/masedb/find.py
--rw-rw-rw-   0        0        0      863 2023-05-06 02:33:31.000000 masedb-1.0.9/masedb/getdata.py
--rw-rw-rw-   0        0        0      762 2023-05-06 02:33:37.000000 masedb-1.0.9/masedb/insert.py
--rw-rw-rw-   0        0        0      835 2023-05-06 02:33:40.000000 masedb-1.0.9/masedb/update.py
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:52.000000 masedb-1.0.9/masedb.egg-info/
--rw-rw-rw-   0        0        0     2151 2023-05-06 02:35:52.000000 masedb-1.0.9/masedb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-06 02:35:52.000000 masedb-1.0.9/masedb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 02:35:52.000000 masedb-1.0.9/masedb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-06 02:35:52.000000 masedb-1.0.9/masedb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 02:35:52.000000 masedb-1.0.9/masedb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 02:35:52.000000 masedb-1.0.9/masedb.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-06 02:35:52.000000 masedb-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2410 2023-05-06 02:35:22.000000 masedb-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:39:38.000000 masedb-1.1.0/
+-rw-rw-rw-   0        0        0     2290 2023-05-06 01:50:34.000000 masedb-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2151 2023-05-06 02:39:38.000000 masedb-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1839 2023-05-06 02:12:56.000000 masedb-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb/
+-rw-rw-rw-   0        0        0      783 2023-05-06 02:08:47.000000 masedb-1.1.0/masedb/connect.py
+-rw-rw-rw-   0        0        0      703 2023-05-06 02:38:54.000000 masedb-1.1.0/masedb/find.py
+-rw-rw-rw-   0        0        0      863 2023-05-06 02:38:42.000000 masedb-1.1.0/masedb/getdata.py
+-rw-rw-rw-   0        0        0      761 2023-05-06 02:38:59.000000 masedb-1.1.0/masedb/insert.py
+-rw-rw-rw-   0        0        0      835 2023-05-06 02:38:35.000000 masedb-1.1.0/masedb/update.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/
+-rw-rw-rw-   0        0        0     2151 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 02:35:52.000000 masedb-1.1.0/masedb.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-06 02:39:38.000000 masedb-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2410 2023-05-06 02:39:27.000000 masedb-1.1.0/setup.py
```

### Comparing `masedb-1.0.9/LICENSE` & `masedb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `masedb-1.0.9/PKG-INFO` & `masedb-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: masedb
-Version: 1.0.9
+Version: 1.1.0
 Summary: Easy mase-db use mongodb, motor asyncio
 Home-page: https://github.com/MaseZev/Mase-DB
 Author: MaseZev
 Author-email: csgomanagement1@gmail.com
 License: mit
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align=center>Mase-DB v1.0.9</h1>
+<h1 align=center>Mase-DB v1.1.0</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
```

### Comparing `masedb-1.0.9/README.md` & `masedb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `masedb-1.0.9/masedb/connect.py` & `masedb-1.1.0/masedb/connect.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.9/masedb/find.py` & `masedb-1.1.0/masedb/find.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.9/masedb/getdata.py` & `masedb-1.1.0/masedb/getdata.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.9/masedb/insert.py` & `masedb-1.1.0/masedb/insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import masedb
-from masedb.connect import connect_to_databaset
+from masedb.connect import connect_to_database
 import motor.motor_asyncio
 import asyncio
 
 async def insert_data(url=None, DatabaseName=None, CollectionName=None, param=None):
 
 	if not url:
```

### Comparing `masedb-1.0.9/masedb/update.py` & `masedb-1.1.0/masedb/update.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.9/masedb.egg-info/PKG-INFO` & `masedb-1.1.0/masedb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: masedb
-Version: 1.0.9
+Version: 1.1.0
 Summary: Easy mase-db use mongodb, motor asyncio
 Home-page: https://github.com/MaseZev/Mase-DB
 Author: MaseZev
 Author-email: csgomanagement1@gmail.com
 License: mit
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align=center>Mase-DB v1.0.9</h1>
+<h1 align=center>Mase-DB v1.1.0</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
```

### Comparing `masedb-1.0.9/setup.py` & `masedb-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import re
 
-readme = '''<h1 align=center>Mase-DB v1.0.9</h1>
+readme = '''<h1 align=center>Mase-DB v1.1.0</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
 
@@ -69,15 +69,15 @@
 
 <br>
 '''
 
 requirements = ["pymongo","dnspython","motor"]
 
 setup(name='masedb',
-      version='1.0.9',
+      version='1.1.0',
       description='Easy mase-db use mongodb, motor asyncio',
       url='https://github.com/MaseZev/Mase-DB',
       packages=['masedb'],
       license='mit',
       author="MaseZev",
       author_email='csgomanagement1@gmail.com',
       long_description=readme,
```

