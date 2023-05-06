# Comparing `tmp/masedb-1.1.0.tar.gz` & `tmp/masedb-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\masedb-1.1.0.tar", last modified: Sat May  6 02:39:38 2023, max compression
+gzip compressed data, was "dist\masedb-1.1.4.tar", last modified: Sat May  6 09:35:06 2023, max compression
```

## Comparing `masedb-1.1.0.tar` & `masedb-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 02:39:38.000000 masedb-1.1.0/
--rw-rw-rw-   0        0        0     2290 2023-05-06 01:50:34.000000 masedb-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2151 2023-05-06 02:39:38.000000 masedb-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1839 2023-05-06 02:12:56.000000 masedb-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb/
--rw-rw-rw-   0        0        0      783 2023-05-06 02:08:47.000000 masedb-1.1.0/masedb/connect.py
--rw-rw-rw-   0        0        0      703 2023-05-06 02:38:54.000000 masedb-1.1.0/masedb/find.py
--rw-rw-rw-   0        0        0      863 2023-05-06 02:38:42.000000 masedb-1.1.0/masedb/getdata.py
--rw-rw-rw-   0        0        0      761 2023-05-06 02:38:59.000000 masedb-1.1.0/masedb/insert.py
--rw-rw-rw-   0        0        0      835 2023-05-06 02:38:35.000000 masedb-1.1.0/masedb/update.py
-drwxrwxrwx   0        0        0        0 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/
--rw-rw-rw-   0        0        0     2151 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 02:39:38.000000 masedb-1.1.0/masedb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 02:35:52.000000 masedb-1.1.0/masedb.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-06 02:39:38.000000 masedb-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2410 2023-05-06 02:39:27.000000 masedb-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:35:06.000000 masedb-1.1.4/
+-rw-rw-rw-   0        0        0     2290 2023-05-06 01:50:34.000000 masedb-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3265 2023-05-06 09:35:06.000000 masedb-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2953 2023-05-06 09:34:46.000000 masedb-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 09:35:06.000000 masedb-1.1.4/masedb/
+-rw-rw-rw-   0        0        0      783 2023-05-06 02:08:47.000000 masedb-1.1.4/masedb/connect.py
+-rw-rw-rw-   0        0        0      764 2023-05-06 09:18:16.000000 masedb-1.1.4/masedb/delete.py
+-rw-rw-rw-   0        0        0      268 2023-05-06 08:49:53.000000 masedb-1.1.4/masedb/errors.py
+-rw-rw-rw-   0        0        0      807 2023-05-06 08:51:25.000000 masedb-1.1.4/masedb/find.py
+-rw-rw-rw-   0        0        0      863 2023-05-06 02:38:42.000000 masedb-1.1.4/masedb/getdata.py
+-rw-rw-rw-   0        0        0      797 2023-05-06 08:18:07.000000 masedb-1.1.4/masedb/insert.py
+-rw-rw-rw-   0        0        0      835 2023-05-06 02:38:35.000000 masedb-1.1.4/masedb/update.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:35:06.000000 masedb-1.1.4/masedb.egg-info/
+-rw-rw-rw-   0        0        0     3265 2023-05-06 09:35:04.000000 masedb-1.1.4/masedb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-06 09:35:04.000000 masedb-1.1.4/masedb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 09:35:04.000000 masedb-1.1.4/masedb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-06 09:35:04.000000 masedb-1.1.4/masedb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 09:35:04.000000 masedb-1.1.4/masedb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 02:35:52.000000 masedb-1.1.4/masedb.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-06 09:35:06.000000 masedb-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3524 2023-05-06 09:34:14.000000 masedb-1.1.4/setup.py
```

### Comparing `masedb-1.1.0/LICENSE` & `masedb-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `masedb-1.1.0/PKG-INFO` & `masedb-1.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,24 @@
-Metadata-Version: 2.1
-Name: masedb
-Version: 1.1.0
-Summary: Easy mase-db use mongodb, motor asyncio
-Home-page: https://github.com/MaseZev/Mase-DB
-Author: MaseZev
-Author-email: csgomanagement1@gmail.com
-License: mit
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align=center>Mase-DB v1.1.0</h1>
+<h1 align=center>Mase-DB v1.1.4</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
-##Документация
+## Документация
 
 Документация:
  - Скоро будет!
 
 ## Установка
 ```py
 # ЕСЛИ УСТНОВЛЕН
 pip install --upgrade masedb
 
 # ЕСЛИ НЕ УСТАНОВЛЕН
 python3 -m pip install --upgrade masedb
 ```
-##or
+## or
 ```py
 pip install masedb
 ```
 
 ## Применение
 ### Предпосылки
 Прежде чем приступить к работе, вам понадобится несколько вещей:
@@ -42,38 +30,58 @@
 
 ### Примеры
 ```py
 import masedb
 from masedb.find import find_data
 from masedb.insert import insert_data
 from masedb.update import update_data
-from config import url
+from masedb.delete import delete_data
 import asyncio
 
-#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName)
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
+
+#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 #await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 #await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name': 'mark'}, param2={'$set':{'let': 10}})
+#await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
+
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
+
+#     Название базы данных и колекции
 
 DatabaseName = 'pondb2'
 CollectionName = 'poncoll2'
 
+# Сыллка отт монгодб для подключения
+
+url = ''
+
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def test():
 
-	db = await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName)
+	db = await find_data(url=url, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 	print(db)
-	try: 
-		cash = db['cash']
-	except:
-		await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 19})
-		cash = 'Успешное занесение'
 
-	print(cash)
+	if not db:
+		print('занесение')
+
+		return await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name':'mark'})
+
+	try: cash = db['cash']
+	except: cash = None
 
+	await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
 
+	if not cash:
+		print('update data')
+		return await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name':'mark'}, param2={'$set':{'cash': 10}})
+
+	print(cash)
 
 asyncio.run(test())
 
+
 ```
 
 
-<br>
+<br>
```

### Comparing `masedb-1.1.0/README.md` & `masedb-1.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-<h1 align=center>Mase-DB v1.0.3</h1>
+Metadata-Version: 2.1
+Name: masedb
+Version: 1.1.4
+Summary: Easy mase-db use mongodb, motor asyncio
+Home-page: https://github.com/MaseZev/Mase-DB
+Author: MaseZev
+Author-email: csgomanagement1@gmail.com
+License: mit
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align=center>Mase-DB v1.1.4</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
 
@@ -30,38 +42,58 @@
 
 ### Примеры
 ```py
 import masedb
 from masedb.find import find_data
 from masedb.insert import insert_data
 from masedb.update import update_data
-from config import url
+from masedb.delete import delete_data
 import asyncio
 
-#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName)
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
+
+#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 #await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 #await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name': 'mark'}, param2={'$set':{'let': 10}})
+#await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
+
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
+
+#     Название базы данных и колекции
 
 DatabaseName = 'pondb2'
 CollectionName = 'poncoll2'
 
+# Сыллка отт монгодб для подключения
+
+url = ''
+
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def test():
 
-	db = await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName)
+	db = await find_data(url=url, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 	print(db)
-	try: 
-		cash = db['cash']
-	except:
-		await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 19})
-		cash = 'Успешное занесение'
 
-	print(cash)
+	if not db:
+		print('занесение')
+
+		return await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name':'mark'})
+
+	try: cash = db['cash']
+	except: cash = None
 
+	await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
 
+	if not cash:
+		print('update data')
+		return await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name':'mark'}, param2={'$set':{'cash': 10}})
+
+	print(cash)
 
 asyncio.run(test())
 
+
 ```
 
 
 <br>
```

### Comparing `masedb-1.1.0/masedb/connect.py` & `masedb-1.1.4/masedb/connect.py`

 * *Files identical despite different names*

### Comparing `masedb-1.1.0/masedb/find.py` & `masedb-1.1.4/masedb/delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import masedb
 from masedb.connect import connect_to_database
 import motor.motor_asyncio
 import asyncio
 
-async def find_data(url=None, DatabaseName=None, CollectionName=None):
+async def delete_data(url=None, DatabaseName=None, CollectionName=None, param=None):
 
 	if not url:
 
 		return print('[Mase-DB] Не указана ссылка-uri монго дб')
 
 	if not DatabaseName:
 
 		return print('[Mase-DB] Не указано название базы данных монго дб')
 
 	if not CollectionName:
 
 		return print('[Mase-DB] Не указано название колекции монго дб')
 
+	if not param:
+
+		return print('not param1')
+
+
 	db = await connect_to_database(url=url, DatabaseName=DatabaseName, CollectionName=CollectionName)
 
-	info = await db.find_one()
+	await db.delete_one(param)
 
-	return info
+	return
```

### Comparing `masedb-1.1.0/masedb/getdata.py` & `masedb-1.1.4/masedb/getdata.py`

 * *Files identical despite different names*

### Comparing `masedb-1.1.0/masedb/insert.py` & `masedb-1.1.4/masedb/find.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import masedb
 from masedb.connect import connect_to_database
 import motor.motor_asyncio
 import asyncio
 
-async def insert_data(url=None, DatabaseName=None, CollectionName=None, param=None):
+async def find_data(url=None, DatabaseName=None, CollectionName=None, param=None):
 
 	if not url:
+		print('[Mase-DB] Не указана ссылка-uri монго дб')
 
-		return print('[Mase-DB] Не указана ссылка-uri монго дб')
+		return False
 
 	if not DatabaseName:
+		print('[Mase-DB] Не указано название базы данных монго дб')
 
-		return print('[Mase-DB] Не указано название базы данных монго дб')
+		return False
 
 	if not CollectionName:
 
-		return print('[Mase-DB] Не указано название колекции монго дб')
+		print('[Mase-DB] Не указано название колекции монго дб')
+
+		return False
 
 	if not param:
 
-		return print('not param')
+		print('not param')
+		return False
 
 	db = await connect_to_database(url=url, DatabaseName=DatabaseName, CollectionName=CollectionName)
 
-	await db.insert_one(param)
+	info = await db.find_one(param)
 
-	return
+	return info
```

### Comparing `masedb-1.1.0/masedb/update.py` & `masedb-1.1.4/masedb/update.py`

 * *Files identical despite different names*

### Comparing `masedb-1.1.0/masedb.egg-info/PKG-INFO` & `masedb-1.1.4/masedb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: masedb
-Version: 1.1.0
+Version: 1.1.4
 Summary: Easy mase-db use mongodb, motor asyncio
 Home-page: https://github.com/MaseZev/Mase-DB
 Author: MaseZev
 Author-email: csgomanagement1@gmail.com
 License: mit
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align=center>Mase-DB v1.1.0</h1>
+<h1 align=center>Mase-DB v1.1.4</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
 
@@ -42,38 +42,58 @@
 
 ### Примеры
 ```py
 import masedb
 from masedb.find import find_data
 from masedb.insert import insert_data
 from masedb.update import update_data
-from config import url
+from masedb.delete import delete_data
 import asyncio
 
-#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName)
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
+
+#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 #await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 #await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name': 'mark'}, param2={'$set':{'let': 10}})
+#await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
+
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
+
+#     Название базы данных и колекции
 
 DatabaseName = 'pondb2'
 CollectionName = 'poncoll2'
 
+# Сыллка отт монгодб для подключения
+
+url = ''
+
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def test():
 
-	db = await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName)
+	db = await find_data(url=url, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 	print(db)
-	try: 
-		cash = db['cash']
-	except:
-		await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 19})
-		cash = 'Успешное занесение'
 
-	print(cash)
+	if not db:
+		print('занесение')
 
+		return await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name':'mark'})
 
+	try: cash = db['cash']
+	except: cash = None
+
+	await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
+
+	if not cash:
+		print('update data')
+		return await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name':'mark'}, param2={'$set':{'cash': 10}})
+
+	print(cash)
 
 asyncio.run(test())
 
+
 ```
 
 
 <br>
```

### Comparing `masedb-1.1.0/setup.py` & `masedb-1.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import re
 
-readme = '''<h1 align=center>Mase-DB v1.1.0</h1>
+readme = '''<h1 align=center>Mase-DB v1.1.4</h1>
 <p align=center>Легкое использование базы данных монгодб.</p>
 
 ##Документация
 
 Документация:
  - Скоро будет!
 
@@ -33,51 +33,71 @@
 
 ### Примеры
 ```py
 import masedb
 from masedb.find import find_data
 from masedb.insert import insert_data
 from masedb.update import update_data
-from config import url
+from masedb.delete import delete_data
 import asyncio
 
-#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName)
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
+
+#await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 #await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 #await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name': 'mark'}, param2={'$set':{'let': 10}})
+#await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
+
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
+
+#     Название базы данных и колекции
 
 DatabaseName = 'pondb2'
 CollectionName = 'poncoll2'
 
+# Сыллка отт монгодб для подключения
+
+url = ''
+
+#--------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def test():
 
-	db = await find_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName)
+	db = await find_data(url=url, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name': 'mark'})
 	print(db)
-	try: 
-		cash = db['cash']
-	except:
-		await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 19})
-		cash = 'Успешное занесение'
 
-	print(cash)
+	if not db:
+		print('занесение')
 
+		return await insert_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'name':'mark'})
 
+	try: cash = db['cash']
+	except: cash = None
+
+	await delete_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param={'cash': 10})
+
+	if not cash:
+		print('update data')
+		return await update_data(url=url.uri, DatabaseName=DatabaseName, CollectionName=CollectionName, param1={'name':'mark'}, param2={'$set':{'cash': 10}})
+
+	print(cash)
 
 asyncio.run(test())
 
+
 ```
 
 
 <br>
 '''
 
 requirements = ["pymongo","dnspython","motor"]
 
 setup(name='masedb',
-      version='1.1.0',
+      version='1.1.4',
       description='Easy mase-db use mongodb, motor asyncio',
       url='https://github.com/MaseZev/Mase-DB',
       packages=['masedb'],
       license='mit',
       author="MaseZev",
       author_email='csgomanagement1@gmail.com',
       long_description=readme,
```

