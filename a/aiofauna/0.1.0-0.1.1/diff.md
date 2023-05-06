# Comparing `tmp/aiofauna-0.1.0.tar.gz` & `tmp/aiofauna-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.1.0.tar", max compression
+gzip compressed data, was "aiofauna-0.1.1.tar", max compression
```

## Comparing `aiofauna-0.1.0.tar` & `aiofauna-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,14 @@
--rw-r--r--   0        0        0     1113 2023-05-01 08:40:13.385351 aiofauna-0.1.0/LICENSE
--rw-r--r--   0        0        0     3069 2023-05-05 11:52:01.285112 aiofauna-0.1.0/README.md
--rw-r--r--   0        0        0     4075 2023-05-02 01:57:27.857521 aiofauna-0.1.0/aiofauna/__init__.py
--rw-r--r--   0        0        0    17190 2023-05-04 02:13:14.898858 aiofauna-0.1.0/aiofauna/api.py
--rw-r--r--   0        0        0    15131 2023-05-02 01:57:28.093559 aiofauna-0.1.0/aiofauna/application.py
--rw-r--r--   0        0        0     4337 2023-05-02 01:57:27.909530 aiofauna-0.1.0/aiofauna/asgi.py
--rw-r--r--   0        0        0      220 2023-05-02 01:57:13.298647 aiofauna-0.1.0/aiofauna/cli.py
--rw-r--r--   0        0        0     4014 2023-05-02 03:44:15.825940 aiofauna-0.1.0/aiofauna/client.py
--rw-r--r--   0        0        0     3678 2023-05-02 03:44:16.169933 aiofauna-0.1.0/aiofauna/datastructures.py
--rw-r--r--   0        0        0      529 2023-05-02 03:44:16.533925 aiofauna-0.1.0/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8161 2023-05-02 03:44:16.889918 aiofauna-0.1.0/aiofauna/errors.py
--rw-r--r--   0        0        0     2978 2023-05-02 03:44:17.217911 aiofauna-0.1.0/aiofauna/helpers.py
--rw-r--r--   0        0        0     6673 2023-05-02 03:44:17.525905 aiofauna-0.1.0/aiofauna/json.py
--rw-r--r--   0        0        0     5861 2023-05-02 03:44:17.853898 aiofauna-0.1.0/aiofauna/objects.py
--rw-r--r--   0        0        0    14824 2023-05-05 12:09:47.607251 aiofauna-0.1.0/aiofauna/odm.py
--rw-r--r--   0        0        0     2760 2023-05-02 03:44:15.489947 aiofauna-0.1.0/aiofauna/page.py
--rw-r--r--   0        0        0    41588 2023-05-02 03:44:15.141955 aiofauna-0.1.0/aiofauna/query.py
--rw-r--r--   0        0        0      829 2023-05-05 11:52:16.905014 aiofauna-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3988 2023-05-05 12:11:56.329063 aiofauna-0.1.0/setup.py
--rw-r--r--   0        0        0     4116 2023-05-05 12:11:56.329635 aiofauna-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3619 2023-05-05 14:04:33.858503 aiofauna-0.1.1/aiofauna/__init__.py
+-rw-r--r--   0        0        0    17190 2023-05-05 14:01:54.151818 aiofauna-0.1.1/aiofauna/api.py
+-rw-r--r--   0        0        0      819 2023-05-06 04:21:31.770848 aiofauna-0.1.1/aiofauna/cli.py
+-rw-r--r--   0        0        0     4014 2023-05-05 14:00:20.387576 aiofauna-0.1.1/aiofauna/client.py
+-rw-r--r--   0        0        0      529 2023-05-05 14:00:19.927579 aiofauna-0.1.1/aiofauna/deprecated.py
+-rw-r--r--   0        0        0     8161 2023-05-05 14:00:19.463582 aiofauna-0.1.1/aiofauna/errors.py
+-rw-r--r--   0        0        0     6673 2023-05-05 14:00:19.003585 aiofauna-0.1.1/aiofauna/json.py
+-rw-r--r--   0        0        0     5861 2023-05-05 14:00:18.547588 aiofauna-0.1.1/aiofauna/objects.py
+-rw-r--r--   0        0        0    14407 2023-05-06 04:23:16.333568 aiofauna-0.1.1/aiofauna/odm.py
+-rw-r--r--   0        0        0     2760 2023-05-05 14:00:17.607594 aiofauna-0.1.1/aiofauna/page.py
+-rw-r--r--   0        0        0    41588 2023-05-05 14:00:16.947598 aiofauna-0.1.1/aiofauna/query.py
+-rw-r--r--   0        0        0      515 2023-05-06 04:25:08.136315 aiofauna-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-05-06 04:25:11.799493 aiofauna-0.1.1/setup.py
+-rw-r--r--   0        0        0      677 2023-05-06 04:25:11.800346 aiofauna-0.1.1/PKG-INFO
```

### Comparing `aiofauna-0.1.0/aiofauna/__init__.py` & `aiofauna-0.1.1/aiofauna/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,81 @@
-"""
----
-title: AioFauna
----
-
-# AioFauna
- 
- 🚀 Introducing aiofauna: A full-stack framework for FaunaDB, industry performant with a seamless user experience! 🔥 Take your Backend Development to the next level dramatically improving productivity, performance and development experience.
-
-🌟 Features:
-
-✅ Inspired by FastAPI: DX (Developer Experience) first. Based on Pydantic, Aiohttp, and FaunaDB. CORS support, query and path parameters, request body parsing, most of the features you love from FastAPI are available in aiofauna.
-
-✅ Blazingly Fast!: Industry performant http server while having the fastest python based http client allowing exceptional integrations with third party APIs, forget about installing dozens of SDKs.
-
-✅ Async/await coroutines: Leverage the power of async programming for enhanced performance and responsiveness. 
-
-✅ Automatic Swagger UI generation: Automatic documentation and manual testing UI following industry standard without further effort!.
-
-✅ Live reload and SSE (Server-Sent Events) support: Stream data in real-time to your clients and experience effortless development with live reload.
-
-✅ Pydantic-based Document Object Mapper (DOM): Define and validate your data models with ease. Summarize complex FQL expressions into pythonic, fully typed asynchronous methods for all CRUD operations.
-
-✅ Auto-provisioning: Automatic management of indexes, unique indexes, and collections.
-
-✅ Full JSON communication: Custom encoders to ensure seamless data exchange between your application and FaunaDB backend.
-
-✅ ASGI compliant: provides an ASGI adapter, allowing broader integration with _asgi_ servers like `uvicorn`, `tornado` or `daphne`.
-
-💡 With aiofauna, you can build fast, scalable, and reliable applications using the power of FaunaDB and modern asynchronous Python with its out of the box aiohttp based web framework. Say goodbye to the hassle of manually managing indexes and collections and hello to a seamless data driven development experience with FaunaModel.
-
-🌐 aiofauna is independent and allows native interaction with external services like Docker API, GCP API, AWS API among others, implementing a lightweight stack with aiohttp server capabilities and fauna backend (to be enhanced soon).
-
-📚 Check out the aiofauna library, and start building your next-gen applications today! 🚀
-#Python #FaunaDB #Async #Pydantic #aiofauna
-
-⚙️ If you are using a synchronous framework check out [Faudantic](https://github.com/obahamonde/faudantic) for a similar experience with FaunaDB and Pydantic.
-
-📚 [Documentation](https://aiofauna.smartpro.solutions)
-
-📦 [PyPi](https://pypi.org/project/aiofauna/)
-
-📦 [GitHub](https://github.com/obahamonde/aiofauna)
-
-📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Stream data in real-time to your clients)
-
-"""
-
-__version__ = (0, 0, 35)
-__author__ = "obahamonde"
-__license__ = "MIT"
-
-import json
-from datetime import datetime
-from typing import Any, AsyncGenerator, Callable, Dict, List, Optional, Union
-from uuid import UUID, uuid4
-
-import asyncio
-import aiohttp_cors
-
-from pydantic import (
-    BaseModel,
-    BaseConfig,
-    BaseSettings,
-    Field,
-)  # pylint: disable=no-name-in-module
-
-from aiohttp.web import (
-    Application,
-    AppRunner,
-    Request,
-    Response,
-    RouteDef,
-    TCPSite,
-    json_response,
-)
-from aiohttp.web_middlewares import middleware
-from aiohttp_sse import sse_response
-from .client import ClientSession, AsyncFaunaClient as FaunaClient
-from .errors import AioFaunaException as FaunaException
-from . import query as q
-from .json import (
-    FaunaJSONEncoder as JSONEncoder,
-    to_json as dumps,
-    parse_json_or_none as loads,
-)
-from .odm import AsyncFaunaModel as FaunaModel
-from .application import App
-from .helpers import (
-    jsonify,
-    redirect,
-    render_template,
-    make_response,
-    upload_files,
-)
-from .asgi import aioasgi
-from .datastructures import Graph
-from .api import Api
+"""
+---
+title: AioFauna
+---
+
+# AioFauna
+ 
+ 🚀 Introducing aiofauna: A full-stack framework for FaunaDB, industry performant with a seamless user experience! 🔥 Take your Backend Development to the next level dramatically improving productivity, performance and development experience.
+
+🌟 Features:
+
+✅ Inspired by FastAPI: DX (Developer Experience) first. Based on Pydantic, Aiohttp, and FaunaDB. CORS support, query and path parameters, request body parsing, most of the features you love from FastAPI are available in aiofauna.
+
+✅ Blazingly Fast!: Industry performant http server while having the fastest python based http client allowing exceptional integrations with third party APIs, forget about installing dozens of SDKs.
+
+✅ Async/await coroutines: Leverage the power of async programming for enhanced performance and responsiveness. 
+
+✅ Automatic Swagger UI generation: Automatic documentation and manual testing UI following industry standard without further effort!.
+
+✅ Live reload and SSE (Server-Sent Events) support: Stream data in real-time to your clients and experience effortless development with live reload.
+
+✅ Pydantic-based Document Object Mapper (DOM): Define and validate your data models with ease. Summarize complex FQL expressions into pythonic, fully typed asynchronous methods for all CRUD operations.
+
+✅ Auto-provisioning: Automatic management of indexes, unique indexes, and collections.
+
+✅ Full JSON communication: Custom encoders to ensure seamless data exchange between your application and FaunaDB backend.
+
+💡 With aiofauna, you can build fast, scalable, and reliable applications using the power of FaunaDB and modern asynchronous Python with its out of the box aiohttp based web framework. Say goodbye to the hassle of manually managing indexes and collections and hello to a seamless data driven development experience with FaunaModel.
+
+🌐 aiofauna is independent and allows native interaction with external services like Docker API, GCP API, AWS API among others, implementing a lightweight stack with aiohttp server capabilities and fauna backend (to be enhanced soon).
+
+📚 Check out the aiofauna library, and start building your next-gen applications today! 🚀
+#Python #FaunaDB #Async #Pydantic #aiofauna
+
+⚙️ If you are using a synchronous framework check out [Faudantic](https://github.com/obahamonde/faudantic) for a similar experience with FaunaDB and Pydantic.
+
+📚 [Documentation](https://aiofauna.smartpro.solutions)
+
+📦 [PyPi](https://pypi.org/project/aiofauna/)
+
+📦 [GitHub](https://github.com/obahamonde/aiofauna)
+
+📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Stream data in real-time to your clients)
+
+"""
+
+__version__ = (0, 1, 0)
+__author__ = "obahamonde"
+__license__ = "MIT"
+
+import json
+from datetime import datetime
+from typing import Any, AsyncGenerator, Callable, Dict, List, Optional, Union
+from uuid import UUID, uuid4
+
+import asyncio
+import aiohttp_cors
+
+from pydantic import BaseModel,BaseConfig, BaseSettings, Field  # pylint: disable=no-name-in-module
+
+from aiohttp.web import (
+    Application,
+    AppRunner,
+    Request,
+    Response,
+    RouteDef,
+    TCPSite,
+    json_response,
+)
+from aiohttp.web_middlewares import middleware
+from aiohttp_sse import sse_response
+from .client import ClientSession, AsyncFaunaClient as FaunaClient
+from .errors import AioFaunaException as FaunaException
+from . import query as q
+from .json import (
+    FaunaJSONEncoder as JSONEncoder,
+    to_json as dumps,
+    parse_json_or_none as loads,
+)
+from .odm import AsyncFaunaModel as FaunaModel
+from .api import Api
```

### Comparing `aiofauna-0.1.0/aiofauna/api.py` & `aiofauna-0.1.1/aiofauna/api.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.0/aiofauna/client.py` & `aiofauna-0.1.1/aiofauna/client.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.0/aiofauna/deprecated.py` & `aiofauna-0.1.1/aiofauna/deprecated.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.0/aiofauna/errors.py` & `aiofauna-0.1.1/aiofauna/errors.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.0/aiofauna/json.py` & `aiofauna-0.1.1/aiofauna/json.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.0/aiofauna/objects.py` & `aiofauna-0.1.1/aiofauna/objects.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.0/aiofauna/odm.py` & `aiofauna-0.1.1/aiofauna/odm.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,30 +508,23 @@
             An instance of the model if created successfully, None otherwise.
         """
 
         try:
             for field in self.__fields__.values():
                 if field.field_info.extra.get("unique"):
                     if await self.__class__.find_unique(field.name, getattr(self, field.name)):
-                        raise Exception(
-                            f"Document with {field.name} {getattr(self, field.name)} already exists"
-                        ) 
-                return self.__class__(
-                    **{
-                        **(await self.__class__.q()(q.create(q.collection(self.__class__.__name__.lower()), {"data": self.dict()}))),
-                        "ref": self.ref,
-                        "ts": self.ts,
-                    }
-                )
-                
-
+                        raise ValueError(f"{field.name} must be unique")
+            self.__class__.q()(q.create(q.collection(self.__class__.__name__.lower()), {"data": self.dict()}))
+            return self
+        
         except AioFaunaException as exc:
+            
             logging.error(exc)
-
-            return await ExceptionModel(message=str(exc), status="error").create()
+            
+            raise ValueError(exc)
 
     @classmethod
     async def query(cls, query: str) -> List[AsyncFaunaModel]:
         """
 
 
         Queries FaunaDB using a string query and returns a list of instances of the model.
@@ -609,12 +602,7 @@
             An instance of the model if saved successfully, None otherwise.
         """
 
         if isinstance(self.ref, str) and len(self.ref) == 18:
             return await self.update(self.ref, kwargs=self.dict())
         return await self.create()
 
-
-class ExceptionModel(AsyncFaunaModel):
-    message: Optional[str]
-    status: Optional[str]
-
```

### Comparing `aiofauna-0.1.0/aiofauna/page.py` & `aiofauna-0.1.1/aiofauna/page.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.0/aiofauna/query.py` & `aiofauna-0.1.1/aiofauna/query.py`

 * *Files identical despite different names*

