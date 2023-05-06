# Comparing `tmp/aiofauna-0.1.1.tar.gz` & `tmp/aiofauna-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.1.1.tar", max compression
+gzip compressed data, was "aiofauna-0.1.2.tar", max compression
```

## Comparing `aiofauna-0.1.1.tar` & `aiofauna-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3619 2023-05-05 14:04:33.858503 aiofauna-0.1.1/aiofauna/__init__.py
--rw-r--r--   0        0        0    17190 2023-05-05 14:01:54.151818 aiofauna-0.1.1/aiofauna/api.py
--rw-r--r--   0        0        0      819 2023-05-06 04:21:31.770848 aiofauna-0.1.1/aiofauna/cli.py
--rw-r--r--   0        0        0     4014 2023-05-05 14:00:20.387576 aiofauna-0.1.1/aiofauna/client.py
--rw-r--r--   0        0        0      529 2023-05-05 14:00:19.927579 aiofauna-0.1.1/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8161 2023-05-05 14:00:19.463582 aiofauna-0.1.1/aiofauna/errors.py
--rw-r--r--   0        0        0     6673 2023-05-05 14:00:19.003585 aiofauna-0.1.1/aiofauna/json.py
--rw-r--r--   0        0        0     5861 2023-05-05 14:00:18.547588 aiofauna-0.1.1/aiofauna/objects.py
--rw-r--r--   0        0        0    14407 2023-05-06 04:23:16.333568 aiofauna-0.1.1/aiofauna/odm.py
--rw-r--r--   0        0        0     2760 2023-05-05 14:00:17.607594 aiofauna-0.1.1/aiofauna/page.py
--rw-r--r--   0        0        0    41588 2023-05-05 14:00:16.947598 aiofauna-0.1.1/aiofauna/query.py
--rw-r--r--   0        0        0      515 2023-05-06 04:25:08.136315 aiofauna-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      859 2023-05-06 04:25:11.799493 aiofauna-0.1.1/setup.py
--rw-r--r--   0        0        0      677 2023-05-06 04:25:11.800346 aiofauna-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3619 2023-05-05 14:04:33.858503 aiofauna-0.1.2/aiofauna/__init__.py
+-rw-r--r--   0        0        0    17190 2023-05-05 14:01:54.151818 aiofauna-0.1.2/aiofauna/api.py
+-rw-r--r--   0        0        0      819 2023-05-06 04:21:31.770848 aiofauna-0.1.2/aiofauna/cli.py
+-rw-r--r--   0        0        0     4014 2023-05-05 14:00:20.387576 aiofauna-0.1.2/aiofauna/client.py
+-rw-r--r--   0        0        0      529 2023-05-05 14:00:19.927579 aiofauna-0.1.2/aiofauna/deprecated.py
+-rw-r--r--   0        0        0     8161 2023-05-05 14:00:19.463582 aiofauna-0.1.2/aiofauna/errors.py
+-rw-r--r--   0        0        0     6673 2023-05-05 14:00:19.003585 aiofauna-0.1.2/aiofauna/json.py
+-rw-r--r--   0        0        0     5861 2023-05-05 14:00:18.547588 aiofauna-0.1.2/aiofauna/objects.py
+-rw-r--r--   0        0        0    14595 2023-05-06 08:00:24.709545 aiofauna-0.1.2/aiofauna/odm.py
+-rw-r--r--   0        0        0     2760 2023-05-05 14:00:17.607594 aiofauna-0.1.2/aiofauna/page.py
+-rw-r--r--   0        0        0    41588 2023-05-05 14:00:16.947598 aiofauna-0.1.2/aiofauna/query.py
+-rw-r--r--   0        0        0      515 2023-05-06 08:02:13.509398 aiofauna-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-05-06 08:02:46.814771 aiofauna-0.1.2/setup.py
+-rw-r--r--   0        0        0      677 2023-05-06 08:02:46.815555 aiofauna-0.1.2/PKG-INFO
```

### Comparing `aiofauna-0.1.1/aiofauna/__init__.py` & `aiofauna-0.1.2/aiofauna/__init__.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/api.py` & `aiofauna-0.1.2/aiofauna/api.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/cli.py` & `aiofauna-0.1.2/aiofauna/cli.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/client.py` & `aiofauna-0.1.2/aiofauna/client.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/deprecated.py` & `aiofauna-0.1.2/aiofauna/deprecated.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/errors.py` & `aiofauna-0.1.2/aiofauna/errors.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/json.py` & `aiofauna-0.1.2/aiofauna/json.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/objects.py` & `aiofauna-0.1.2/aiofauna/objects.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/odm.py` & `aiofauna-0.1.2/aiofauna/odm.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import asyncio
 
 
 from typing import List, Optional, Any, Callable, Union
 
 try:
-    import query as q
+    import query as q # type: ignore
 except ImportError:
     from . import query as q
 
 from .errors import AioFaunaException
 
 
 from .json import JSONModel  # pylint: disable=no-name-in-module
@@ -249,15 +249,15 @@
                     "ts": data["ts"] / 1000,
                 }
             )
 
         except AioFaunaException as exc:
             logging.error(exc)
 
-            return await ExceptionModel(message=str(exc), status="error").create()
+            raise ValueError(f"{field} {value} not found")
 
     @classmethod
     async def find_many(cls, field: str, value: Any) -> List[AsyncFaunaModel]:
         """
 
 
         Finds documents in FaunaDB by a field.
@@ -360,15 +360,15 @@
                     "ts": data["ts"] / 1000,
                 }
             )
 
         except AioFaunaException as exc:
             logging.error(exc)
 
-            return await ExceptionModel(message=str(exc), status="error").create()
+            raise ValueError(f"{ref} not found")
 
     @classmethod
     async def find_all(cls, limit: int, offset: int) -> List[AsyncFaunaModel]:
         """
 
 
         Finds all documents of the model in FaunaDB.
@@ -507,16 +507,20 @@
 
             An instance of the model if created successfully, None otherwise.
         """
 
         try:
             for field in self.__fields__.values():
                 if field.field_info.extra.get("unique"):
-                    if await self.__class__.find_unique(field.name, getattr(self, field.name)):
-                        raise ValueError(f"{field.name} must be unique")
+                    instance = await self.find_unique(field.name, getattr(self, field.name))
+                    if instance is None:
+                        continue
+                    else:
+                        await instance.__class__.q()(q.create(q.collection(self.__class__.__name__.lower()), {"data": self.dict()})) # type: ignore
+                        return instance # type: ignore
             self.__class__.q()(q.create(q.collection(self.__class__.__name__.lower()), {"data": self.dict()}))
             return self
         
         except AioFaunaException as exc:
             
             logging.error(exc)
```

### Comparing `aiofauna-0.1.1/aiofauna/page.py` & `aiofauna-0.1.2/aiofauna/page.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/aiofauna/query.py` & `aiofauna-0.1.2/aiofauna/query.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.1/pyproject.toml` & `aiofauna-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiofauna"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Oscar Bahamonde <oscar.bahamonde.dev@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = {extras = ["dotenv"], version = "^1.10.7"}
 aiohttp = "^3.8.4"
```

### Comparing `aiofauna-0.1.1/setup.py` & `aiofauna-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pydantic[dotenv]>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['dev = aiofauna.cli:dev']}
 
 setup_kwargs = {
     'name': 'aiofauna',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': None,
     'author': 'Oscar Bahamonde',
     'author_email': 'oscar.bahamonde.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `aiofauna-0.1.1/PKG-INFO` & `aiofauna-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofauna
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde.dev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

