# Comparing `tmp/masedb-1.0.7.tar.gz` & `tmp/masedb-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\masedb-1.0.7.tar", last modified: Sat May  6 02:25:05 2023, max compression
+gzip compressed data, was "dist\masedb-1.0.8.tar", last modified: Sat May  6 02:29:54 2023, max compression
```

## Comparing `masedb-1.0.7.tar` & `masedb-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 02:25:05.000000 masedb-1.0.7/
--rw-rw-rw-   0        0        0     2290 2023-05-06 01:50:34.000000 masedb-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     2151 2023-05-06 02:25:05.000000 masedb-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1839 2023-05-06 02:12:56.000000 masedb-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 02:25:05.000000 masedb-1.0.7/masedb/
--rw-rw-rw-   0        0        0      783 2023-05-06 02:08:47.000000 masedb-1.0.7/masedb/connect.py
--rw-rw-rw-   0        0        0      678 2023-05-06 02:11:06.000000 masedb-1.0.7/masedb/find.py
--rw-rw-rw-   0        0        0      838 2023-05-06 02:11:03.000000 masedb-1.0.7/masedb/getdata.py
--rw-rw-rw-   0        0        0      736 2023-05-06 02:12:10.000000 masedb-1.0.7/masedb/insert.py
--rw-rw-rw-   0        0        0      810 2023-05-06 02:12:07.000000 masedb-1.0.7/masedb/update.py
-drwxrwxrwx   0        0        0        0 2023-05-06 02:25:05.000000 masedb-1.0.7/masedb.egg-info/
--rw-rw-rw-   0        0        0     2151 2023-05-06 02:25:05.000000 masedb-1.0.7/masedb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-06 02:25:05.000000 masedb-1.0.7/masedb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 02:25:05.000000 masedb-1.0.7/masedb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-06 02:25:05.000000 masedb-1.0.7/masedb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 02:25:05.000000 masedb-1.0.7/masedb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 02:23:41.000000 masedb-1.0.7/masedb.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-06 02:25:05.000000 masedb-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2410 2023-05-06 02:24:59.000000 masedb-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:29:54.000000 masedb-1.0.8/
+-rw-rw-rw-   0        0        0     2290 2023-05-06 01:50:34.000000 masedb-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2151 2023-05-06 02:29:54.000000 masedb-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1839 2023-05-06 02:12:56.000000 masedb-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 02:29:54.000000 masedb-1.0.8/masedb/
+-rw-rw-rw-   0        0        0      783 2023-05-06 02:08:47.000000 masedb-1.0.8/masedb/connect.py
+-rw-rw-rw-   0        0        0      678 2023-05-06 02:11:06.000000 masedb-1.0.8/masedb/find.py
+-rw-rw-rw-   0        0        0      838 2023-05-06 02:11:03.000000 masedb-1.0.8/masedb/getdata.py
+-rw-rw-rw-   0        0        0      736 2023-05-06 02:12:10.000000 masedb-1.0.8/masedb/insert.py
+-rw-rw-rw-   0        0        0      810 2023-05-06 02:12:07.000000 masedb-1.0.8/masedb/update.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:29:54.000000 masedb-1.0.8/masedb.egg-info/
+-rw-rw-rw-   0        0        0     2151 2023-05-06 02:29:54.000000 masedb-1.0.8/masedb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-06 02:29:54.000000 masedb-1.0.8/masedb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 02:29:54.000000 masedb-1.0.8/masedb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-06 02:29:54.000000 masedb-1.0.8/masedb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 02:29:54.000000 masedb-1.0.8/masedb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 02:23:41.000000 masedb-1.0.8/masedb.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-06 02:29:54.000000 masedb-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2410 2023-05-06 02:29:26.000000 masedb-1.0.8/setup.py
```

### Comparing `masedb-1.0.7/LICENSE` & `masedb-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `masedb-1.0.7/PKG-INFO` & `masedb-1.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: masedb
-Version: 1.0.7
-Summary: Easy mase-db use mongodb, motor asyncio
-Home-page: https://github.com/MaseZev/Mase-DB
-Author: MaseZev
-Author-email: csgomanagement1@gmail.com
-License: mit
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align=center>Mase-DB v1.0.3</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
```

### Comparing `masedb-1.0.7/README.md` & `masedb-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-<h1 align=center>Mase-DB v1.0.3</h1>
+Metadata-Version: 2.1
+Name: masedb
+Version: 1.0.8
+Summary: Easy mase-db use mongodb, motor asyncio
+Home-page: https://github.com/MaseZev/Mase-DB
+Author: MaseZev
+Author-email: csgomanagement1@gmail.com
+License: mit
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align=center>Mase-DB v1.0.8</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
```

### Comparing `masedb-1.0.7/masedb/connect.py` & `masedb-1.0.8/masedb/connect.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.7/masedb/find.py` & `masedb-1.0.8/masedb/find.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.7/masedb/getdata.py` & `masedb-1.0.8/masedb/getdata.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.7/masedb/insert.py` & `masedb-1.0.8/masedb/insert.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.7/masedb/update.py` & `masedb-1.0.8/masedb/update.py`

 * *Files identical despite different names*

### Comparing `masedb-1.0.7/masedb.egg-info/PKG-INFO` & `masedb-1.0.8/masedb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: masedb
-Version: 1.0.7
+Version: 1.0.8
 Summary: Easy mase-db use mongodb, motor asyncio
 Home-page: https://github.com/MaseZev/Mase-DB
 Author: MaseZev
 Author-email: csgomanagement1@gmail.com
 License: mit
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align=center>Mase-DB v1.0.3</h1>
+<h1 align=center>Mase-DB v1.0.8</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
```

### Comparing `masedb-1.0.7/setup.py` & `masedb-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import re
 
-readme = '''<h1 align=center>Mase-DB v1.0.3</h1>
+readme = '''<h1 align=center>Mase-DB v1.0.8</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
 
@@ -69,15 +69,15 @@
 
 <br>
 '''
 
 requirements = ["pymongo","dnspython","motor"]
 
 setup(name='masedb',
-      version='1.0.7',
+      version='1.0.8',
       description='Easy mase-db use mongodb, motor asyncio',
       url='https://github.com/MaseZev/Mase-DB',
       packages=['masedb'],
       license='mit',
       author="MaseZev",
       author_email='csgomanagement1@gmail.com',
       long_description=readme,
```

