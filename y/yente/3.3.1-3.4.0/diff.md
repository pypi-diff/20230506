# Comparing `tmp/yente-3.3.1.tar.gz` & `tmp/yente-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.3.1.tar", last modified: Tue Apr 25 13:00:19 2023, max compression
+gzip compressed data, was "yente-3.4.0.tar", last modified: Sat May  6 20:02:57 2023, max compression
```

## Comparing `yente-3.3.1.tar` & `yente-3.4.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.890479 yente-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 12:58:23.000000 yente-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 12:58:23.000000 yente-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-25 13:00:19.890479 yente-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-25 12:58:23.000000 yente-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:00:19.890479 yente-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-25 12:58:23.000000 yente-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.882479 yente-3.3.1/yente/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:23.000000 yente-3.3.1/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-25 12:58:23.000000 yente-3.3.1/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-25 12:58:23.000000 yente-3.3.1/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.886479 yente-3.3.1/yente/data/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-25 12:58:23.000000 yente-3.3.1/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-25 12:58:23.000000 yente-3.3.1/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 12:58:23.000000 yente-3.3.1/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.886479 yente-3.3.1/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-25 12:58:23.000000 yente-3.3.1/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.890479 yente-3.3.1/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-25 12:58:23.000000 yente-3.3.1/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 12:58:23.000000 yente-3.3.1/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.890479 yente-3.3.1/yente/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-25 12:58:23.000000 yente-3.3.1/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 12:58:23.000000 yente-3.3.1/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-25 12:58:23.000000 yente-3.3.1/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-25 12:58:23.000000 yente-3.3.1/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:00:19.886479 yente-3.3.1/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:58:36.000000 yente-3.3.1/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 13:00:19.000000 yente-3.3.1/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:57.002739 yente-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 20:00:22.000000 yente-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-06 20:00:22.000000 yente-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-06 20:02:57.002739 yente-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-06 20:00:22.000000 yente-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 20:02:57.002739 yente-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-06 20:00:22.000000 yente-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:56.990738 yente-3.4.0/yente/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:22.000000 yente-3.4.0/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-06 20:00:22.000000 yente-3.4.0/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-06 20:00:22.000000 yente-3.4.0/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:56.998739 yente-3.4.0/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-06 20:00:22.000000 yente-3.4.0/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-06 20:00:22.000000 yente-3.4.0/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-06 20:00:22.000000 yente-3.4.0/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:56.998739 yente-3.4.0/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-06 20:00:22.000000 yente-3.4.0/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:57.002739 yente-3.4.0/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-06 20:00:22.000000 yente-3.4.0/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 20:00:22.000000 yente-3.4.0/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:57.002739 yente-3.4.0/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-06 20:00:22.000000 yente-3.4.0/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-06 20:00:22.000000 yente-3.4.0/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-06 20:00:22.000000 yente-3.4.0/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-06 20:00:22.000000 yente-3.4.0/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:02:56.998739 yente-3.4.0/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:00:35.000000 yente-3.4.0/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 20:02:56.000000 yente-3.4.0/yente.egg-info/top_level.txt
```

### Comparing `yente-3.3.1/LICENSE` & `yente-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/PKG-INFO` & `yente-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.3.1
+Version: 3.4.0
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.3.1/README.md` & `yente-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/setup.py` & `yente-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,41 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.3.1",
+    version="3.4.0",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
     namespace_packages=[],
     install_requires=[
         "followthemoney==3.3.0",
-        "nomenklatura==2.9.5",
-        "asyncstdlib==3.10.6",
+        "nomenklatura==2.11.0",
+        "asyncstdlib==3.10.7",
         "aiocron==1.8",
         "aiocsv==1.2.4",
         "aiofiles==23.1.0",
-        "types-aiofiles==23.1.0.1",
+        "types-aiofiles==23.1.0.2",
         "aiohttp[speedups]==3.8.4",
         "elasticsearch[async]==8.7.0",
         "fastapi==0.95.1",
-        "uvicorn[standard]==0.21.1",
+        "uvicorn[standard]==0.22.0",
         "python-multipart==0.0.6",
         "email-validator==2.0.0.post2",
         "structlog==23.1.0",
         "pyicu==2.11",
-        "orjson==3.8.10",
+        "jellyfish==0.11.2",
+        "orjson==3.8.11",
         "text-unidecode==1.3",
         "click==8.0.4",
         "normality==2.4.0",
         "languagecodes==1.1.1",
         "countrynames==1.14.3",
         "fingerprints==1.1.0",
         "pantomime==0.6.0",
```

### Comparing `yente-3.3.1/yente/app.py` & `yente-3.4.0/yente/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from fastapi import Request, Response
 from starlette.middleware.base import RequestResponseEndpoint
 from fastapi.responses import JSONResponse
 from structlog.contextvars import clear_contextvars, bind_contextvars
 
 from yente import settings
 from yente.logs import get_logger
-from yente.routers import reconcile, search, admin
+from yente.routers import reconcile, search, match, admin
 
 log = get_logger("yente")
 
 
 async def request_middleware(
     request: Request, call_next: RequestResponseEndpoint
 ) -> Response:
@@ -65,13 +65,14 @@
         version=settings.VERSION,
         contact=settings.CONTACT,
         openapi_tags=settings.TAGS,
         redoc_url="/",
     )
     app.middleware("http")(request_middleware)
     app.include_router(search.router)
+    app.include_router(match.router)
     app.include_router(reconcile.router)
     app.include_router(admin.router)
 
     app.add_exception_handler(ApiError, api_error_handler)
     app.add_exception_handler(TransportError, transport_error_handler)
     return app
```

### Comparing `yente-3.3.1/yente/cli.py` & `yente-3.4.0/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/data/common.py` & `yente-3.4.0/yente/data/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from datetime import datetime
 from typing import Dict, List, Union, Optional
 from pydantic import BaseModel, Field
-from nomenklatura.matching.types import FeatureDocs
-from nomenklatura.matching.types import MatchingResult
+from nomenklatura.matching.types import MatchingResult, FeatureDocs
 
 from yente import settings
 from yente.data.entity import Entity
 
 EntityProperties = Dict[str, List[Union[str, "EntityResponse"]]]
 
 
@@ -31,16 +30,16 @@
             id=entity.id,
             caption=entity.caption,
             schema=entity.schema.name,
             properties=dict(entity.properties),
             datasets=list(entity.datasets),
             referents=list(entity.referents),
             target=entity.target,
-            first_seen=entity.first_seen,
-            last_seen=entity.last_seen,
+            first_seen=entity._first_seen or entity.first_seen,
+            last_seen=entity._last_seen or entity.last_seen,
         )
 
 
 EntityResponse.update_forward_refs()
 
 
 class ScoredEntityResponse(EntityResponse):
@@ -56,16 +55,16 @@
             id=entity.id,
             caption=entity.caption,
             schema=entity.schema.name,
             properties=entity.properties,
             datasets=list(entity.datasets),
             referents=list(entity.referents),
             target=entity.target,
-            first_seen=entity.first_seen,
-            last_seen=entity.last_seen,
+            first_seen=entity._first_seen or entity.first_seen,
+            last_seen=entity._last_seen or entity.last_seen,
             score=result["score"],
             match=result["score"] >= threshold,
             features=result["features"],
         )
 
 
 class StatusResponse(BaseModel):
@@ -133,7 +132,17 @@
     entities_url: Optional[str]
     version: str
     children: List[str]
 
 
 class DataCatalogModel(BaseModel):
     datasets: List[DatasetModel]
+
+
+class Algorithm(BaseModel):
+    name: str
+    description: Optional[str]
+    features: FeatureDocs
+
+
+class AlgorithmResponse(BaseModel):
+    algorithms: List[Algorithm]
```

### Comparing `yente-3.3.1/yente/data/dataset.py` & `yente-3.4.0/yente/data/dataset.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/data/entity.py` & `yente-3.4.0/yente/data/entity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, TYPE_CHECKING
+from typing import Any, Dict, Optional, TYPE_CHECKING
 from followthemoney import model
 from followthemoney.model import Model
 from followthemoney.types import registry
 from followthemoney.helpers import combine_names
 from nomenklatura.entity import CompositeEntity
 
 from yente.logs import get_logger
@@ -15,18 +15,24 @@
 
 class Entity(CompositeEntity):
     """Entity for sanctions list entries and adjacent objects."""
 
     def __init__(self, model: Model, data: Dict[str, Any], cleaned: bool = True):
         super().__init__(model, data, cleaned=cleaned)
         self.target: bool = data.get("target", False)
+        self._first_seen: Optional[str] = data.get("first_seen", None)
+        self._last_seen: Optional[str] = data.get("last_seen", None)
 
     def to_dict(self) -> Dict[str, Any]:
         data = super().to_dict()
         data["target"] = self.target
+        if data.get("first_seen") is None:
+            data["first_seen"] = self._first_seen
+        if data.get("last_seen") is None:
+            data["last_seen"] = self._last_seen
         return data
 
     @classmethod
     def from_example(cls, example: "EntityExample") -> "Entity":
         data = {"id": example.id, "schema": example.schema_}
         obj = cls(model, data)
         for prop_name, values in example.properties.items():
```

### Comparing `yente-3.3.1/yente/data/freebase.py` & `yente-3.4.0/yente/data/freebase.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/data/loader.py` & `yente-3.4.0/yente/data/loader.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/data/manifest.py` & `yente-3.4.0/yente/data/manifest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import asyncio
 from typing import List, Optional, Dict, Any
 from pydantic import BaseModel
+from nomenklatura.dataset import DataCatalog
 
 from yente import settings
 from yente.data.loader import load_yaml_url
+from yente.data.dataset import Dataset
 
 
 class CatalogManifest(BaseModel):
     """OpenSanctions is not one dataset but a whole collection, so this
     side-loads it into the yente dataset archive."""
 
     url: str
@@ -41,7 +44,23 @@
     async def load(cls) -> "Manifest":
         data = await load_yaml_url(settings.MANIFEST)
         manifest = cls.parse_obj(data)
         for catalog in manifest.catalogs:
             await catalog.fetch(manifest)
         # TODO: load remote metadata from a `metadata_url` on each dataset?
         return manifest
+
+
+class Catalog(DataCatalog[Dataset]):
+    """A collection of datasets, loaded from a manifest."""
+
+    instance: Optional["Catalog"] = None
+    lock = asyncio.Lock()
+
+    @classmethod
+    async def load(cls) -> "Catalog":
+        async with cls.lock:
+            instance = cls(Dataset, {})
+            manifest = await Manifest.load()
+            for dmf in manifest.datasets:
+                instance.make_dataset(dmf)
+            return instance
```

### Comparing `yente-3.3.1/yente/logs.py` & `yente-3.4.0/yente/logs.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/resources/favicon.ico` & `yente-3.4.0/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/routers/admin.py` & `yente-3.4.0/yente/routers/admin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import aiocron  # type: ignore
+from typing import List
 from fastapi import APIRouter, Query
 from fastapi import HTTPException
+from normality import collapse_spaces
 from starlette.responses import FileResponse
+from nomenklatura.matching import ALGORITHMS
 
 from yente import settings
 from yente.logs import get_logger
 from yente.data import get_catalog, refresh_catalog
 from yente.data.common import ErrorResponse, StatusResponse
-from yente.data.common import DataCatalogModel
+from yente.data.common import DataCatalogModel, AlgorithmResponse, Algorithm
 from yente.search.search import get_index_status
 from yente.search.indexer import update_index, update_index_threaded
 from yente.search.base import close_es
 
 log = get_logger(__name__)
 router = APIRouter()
 
@@ -85,14 +88,34 @@
     The manifest is the configuration file of the yente service. It specifies what
     data sources are included, and how often they should be loaded.
     """
     catalog = await get_catalog()
     return DataCatalogModel.parse_obj(catalog.to_dict())
 
 
+@router.get(
+    "/algorithms",
+    tags=["System information"],
+    response_model=AlgorithmResponse,
+)
+async def algorithms() -> AlgorithmResponse:
+    """Return a list of the supported matching/scoring algorithms used by the matching endpoing.
+
+    See also the [scoring documentation](https://www.opensanctions.org/docs/api/scoring/)."""
+    algorithms: List[Algorithm] = []
+    for algo in ALGORITHMS:
+        desc = Algorithm(
+            name=algo.NAME,
+            description=collapse_spaces(algo.__doc__),
+            features=algo.explain(),
+        )
+        algorithms.append(desc)
+    return AlgorithmResponse(algorithms=algorithms)
+
+
 @router.post(
     "/updatez",
     summary="Force an index update",
     tags=["System information"],
     response_model=StatusResponse,
     responses={403: {"model": ErrorResponse, "description": "Authorization error."}},
 )
```

### Comparing `yente-3.3.1/yente/routers/reconcile.py` & `yente-3.4.0/yente/routers/reconcile.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from urllib.parse import urljoin
 from typing import Any, Coroutine, Dict, List, Tuple
 from fastapi import APIRouter, Query, Form
 from fastapi import Request, Response
 from fastapi import HTTPException
 from followthemoney import model
 from followthemoney.types import registry
+from nomenklatura.matching import get_algorithm
 
 from yente import settings
 from yente.data.common import ErrorResponse, EntityExample
 from yente.logs import get_logger
 from yente.data.entity import Entity
 from yente.data.dataset import Dataset
 from yente.data.freebase import (
@@ -160,16 +161,19 @@
             properties[prop.name] = []
         properties[prop.name].append(p.get("v"))
 
     example = EntityExample(id=None, schema=schema, properties=dict(properties))
     proxy = Entity.from_example(example)
     query = entity_query(dataset, proxy)
     resp = await search_entities(query, limit=limit, offset=offset)
+    algorithm = get_algorithm(settings.DEFAULT_ALGORITHM)
+    if algorithm is None:
+        raise HTTPException(400, detail=f"Unknown algorithm: {algorithm}")
     entities = result_entities(resp)
-    scoreds = [s for s in score_results(proxy, entities, limit=limit)]
+    scoreds = [s for s in score_results(algorithm, proxy, entities, limit=limit)]
     results = [FreebaseScoredEntity.from_scored(s) for s in scoreds]
     log.info(
         f"/reconcile/{dataset.name}",
         action="reconcile",
         schema=proxy.schema.name,
         results=result_total(resp).value,
     )
```

### Comparing `yente-3.3.1/yente/routers/util.py` & `yente-3.4.0/yente/routers/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/scoring.py` & `yente-3.4.0/yente/scoring.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-from typing import Iterable, List, Optional
-from nomenklatura.matching import compare_scored
+from typing import Iterable, List, Optional, Type
+from nomenklatura.matching.types import ScoringAlgorithm
 
 from yente import settings
 from yente.data.entity import Entity
 from yente.data.common import ScoredEntityResponse
 
 
 def score_results(
+    algorithm: Type[ScoringAlgorithm],
     entity: Entity,
     results: Iterable[Entity],
     threshold: float = settings.SCORE_THRESHOLD,
     cutoff: float = 0.0,
     limit: Optional[int] = None,
 ) -> List[ScoredEntityResponse]:
     scored: List[ScoredEntityResponse] = []
     matches = 0
     for proxy in results:
-        scoring = compare_scored(entity, proxy)
+        scoring = algorithm.compare(entity, proxy)
         result = ScoredEntityResponse.from_entity_result(proxy, scoring, threshold)
         if result.score <= cutoff:
             continue
         if result.match:
             matches += 1
         scored.append(result)
 
     scored = sorted(scored, key=lambda r: r.score, reverse=True)
     if limit is not None:
         scored = scored[:limit]
-
-    # If multiple entities meet the match threshold, it's ambiguous
-    # and we bail out:
-    if matches > 1:
-        for result in scored:
-            result.match = False
-
     return scored
```

### Comparing `yente-3.3.1/yente/search/base.py` & `yente-3.4.0/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/search/indexer.py` & `yente-3.4.0/yente/search/indexer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import asyncio
 import threading
+from normality import WS
 from typing import Any, AsyncGenerator, Dict, List
 from elasticsearch import AsyncElasticsearch
 from elasticsearch.helpers import async_bulk, BulkIndexError
 from elasticsearch.exceptions import BadRequestError
 from followthemoney import model
 from followthemoney.types.date import DateType
 from followthemoney.types.name import NameType
+from nomenklatura.util import fingerprint_name
 
 from yente import settings
 from yente.logs import get_logger
 from yente.data.entity import Entity
 from yente.data.dataset import Dataset
 from yente.data import get_catalog
 from yente.data.loader import load_json_lines
 from yente.search.base import get_es, close_es, index_semaphore
 from yente.search.mapping import make_entity_mapping
 from yente.search.mapping import INDEX_SETTINGS
-from yente.data.util import expand_dates, expand_names
+from yente.search.mapping import NAMES_FIELD, SOUNDEX_FIELD, NAME_PART_FIELD
+from yente.data.util import expand_dates, soundex_names
 
 log = get_logger(__name__)
 
 
 async def iter_entity_docs(
     dataset: Dataset, index: str
 ) -> AsyncGenerator[Dict[str, Any], None]:
@@ -40,50 +43,60 @@
             entity.datasets.add(dataset.name)
         if dataset.ns is not None:
             entity = dataset.ns.apply(entity)
 
         texts = entity.pop("indexText")
         doc = entity.to_full_dict(matchable=True)
         doc["text"] = texts
+        names = doc.pop(NameType.group, [])
+        expanded_names = set(names)
+        name_parts = set()
+        for name in names:
+            fp = fingerprint_name(name)
+            if fp is not None:
+                expanded_names.add(fp)
+                name_parts.update(fp.split(WS))
+        doc[NAMES_FIELD] = list(expanded_names)
+        doc[NAME_PART_FIELD] = list(name_parts)
+        doc[SOUNDEX_FIELD] = soundex_names(names)
         doc[DateType.group] = expand_dates(doc.pop(DateType.group, []))
-        doc[NameType.group] = expand_names(doc.pop(NameType.group, []))
         entity_id = doc.pop("id")
         yield {"_index": index, "_id": entity_id, "_source": doc}
 
 
 async def index_entities_rate_limit(
     es: AsyncElasticsearch, dataset: Dataset, force: bool
-) -> None:
+) -> bool:
     async with index_semaphore:
-        await index_entities(es, dataset, force=force)
+        return await index_entities(es, dataset, force=force)
 
 
-async def index_entities(es: AsyncElasticsearch, dataset: Dataset, force: bool) -> None:
+async def index_entities(es: AsyncElasticsearch, dataset: Dataset, force: bool) -> bool:
     """Index entities in a particular dataset, with versioning of the index."""
     if not dataset.load:
         log.debug("Dataset is not loadable", dataset=dataset.name)
-        return
+        return False
     if dataset.entities_url is None:
         log.warning("Cannot identify resource with FtM entities", dataset=dataset.name)
-        return
+        return False
 
     # Versioning defaults to the software version instead of a data update date:
     version = f"{settings.INDEX_VERSION}{dataset.version}"
     log.info(
         "Indexing entities",
         dataset=dataset.name,
         url=dataset.entities_url,
         version=version,
     )
     dataset_prefix = f"{settings.ENTITY_INDEX}-{dataset.name}"
     next_index = f"{dataset_prefix}-{version}"
     exists = await es.indices.exists(index=next_index)
     if exists.body and not force:
         log.info("Index is up to date.", index=next_index)
-        return
+        return False
 
     # await es.indices.delete(index=next_index)
     log.info("Create index", index=next_index)
     try:
         schemata = list(model.schemata.values())
         mapping = make_entity_mapping(schemata)
         await es.indices.create(
@@ -111,46 +124,52 @@
         log.exception(
             "Indexing error: %r" % exc,
             dataset=dataset.name,
             index=next_index,
             entities_url=dataset.entities_url,
         )
         await es.indices.delete(index=next_index)
-        return
+        return False
 
     await es.indices.refresh(index=next_index)
     res = await es.indices.put_alias(index=next_index, name=settings.ENTITY_INDEX)
     if res.meta.status != 200:
         log.error("Failed to alias next index", index=next_index)
-        return
+        return False
 
     log.info("Index is now aliased to: %s" % settings.ENTITY_INDEX, index=next_index)
     indices: Any = await es.cat.indices(format="json")
     current: List[str] = [s.get("index") for s in indices]
     current = [c for c in current if c.startswith(f"{dataset_prefix}-")]
     if len(current) == 0:
         log.error("No index was created", index=next_index)
-        return
+        return False
     for index in current:
         if index != next_index:
             log.info("Delete other index", index=index)
             await es.indices.delete(index=index)
 
+    return True
+
 
-async def update_index(force: bool = False) -> None:
+async def update_index(force: bool = False) -> bool:
+    """Reindex all datasets if there is a new version of their data contenst available,
+    return boolean to indicate if the index was changed for any of them."""
     es_ = await get_es()
     es = es_.options(request_timeout=300)
     try:
         catalog = await get_catalog()
         log.info("Index update check")
         indexers = []
         for dataset in catalog.datasets:
             indexers.append(index_entities_rate_limit(es, dataset, force))
-        await asyncio.gather(*indexers)
-        log.info("Index update complete.")
+        results = await asyncio.gather(*indexers)
+        changed = True in results
+        log.info("Index update complete.", changed=changed)
+        return changed
     finally:
         await es.close()
         await close_es()
 
 
 def update_index_threaded(force: bool = False) -> None:
     async def update_in_thread() -> None:
```

### Comparing `yente-3.3.1/yente/search/mapping.py` & `yente-3.4.0/yente/search/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, Iterable, List, Optional, Union
 from followthemoney import model
 from followthemoney.schema import Schema
 from followthemoney.types import registry
 from followthemoney.types.common import PropertyType
+from followthemoney.types.name import NameType
 
 from yente import settings
 
 MappingProperty = Dict[str, Union[List[str], str]]
 
 DATE_FORMAT = "yyyy-MM-dd'T'HH||yyyy-MM-dd'T'HH:mm||yyyy-MM-dd'T'HH:mm:ss||yyyy-MM-dd||yyyy-MM||yyyy||strict_date_optional_time"
 TEXT_TYPES = (registry.name, registry.address)
@@ -27,14 +28,17 @@
     },
     "index": {
         "refresh_interval": "5s",
         "auto_expand_replicas": "0-all",
         "number_of_shards": settings.ES_SHARDS,
     },
 }
+NAMES_FIELD = NameType.group or "names"
+NAME_PART_FIELD = "name_parts"
+SOUNDEX_FIELD = "soundex"
 
 
 def make_field(
     type_: str, copy_to: Optional[List[str]] = None, format: Optional[str] = None
 ) -> MappingProperty:
     spec: MappingProperty = {"type": type_}
     if type_ == "keyword":
@@ -82,14 +86,16 @@
     mapping = {
         "schema": make_keyword(),
         "caption": make_field("keyword"),
         "datasets": make_keyword(),
         "referents": make_keyword(),
         "target": make_field("boolean"),
         "text": make_field("text"),
+        SOUNDEX_FIELD: make_keyword(),
+        NAME_PART_FIELD: make_keyword(),
         "last_seen": make_field("date", format=DATE_FORMAT),
         "first_seen": make_field("date", format=DATE_FORMAT),
         "properties": {"dynamic": "strict", "properties": prop_mapping},
     }
 
     for t in registry.groups.values():
         if t.group is None:
```

### Comparing `yente-3.3.1/yente/search/nested.py` & `yente-3.4.0/yente/search/nested.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente/search/queries.py` & `yente-3.4.0/yente/search/queries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from typing import Any, Dict, Generator, List, Tuple, Union, Optional
 from followthemoney.schema import Schema
 from followthemoney.proxy import EntityProxy
 from followthemoney.types import registry
-from followthemoney.types.name import NameType
+from nomenklatura.util import name_words
 
 from yente.logs import get_logger
 from yente.data.dataset import Dataset
-from yente.data.util import tokenize_names, pick_names
-from yente.search.mapping import TEXT_TYPES
+from yente.data.util import pick_names, soundex_names
+from yente.search.mapping import TEXT_TYPES, NAMES_FIELD, SOUNDEX_FIELD, NAME_PART_FIELD
 
 log = get_logger(__name__)
 FilterDict = Dict[str, Union[bool, str, List[str]]]
 Clause = Dict[str, Any]
 
-NAMES_FIELD = NameType.group or "names"
-
 
 def filter_query(
     shoulds: List[Clause],
     dataset: Optional[Dataset] = None,
     schema: Optional[Schema] = None,
     filters: FilterDict = {},
 ) -> Clause:
@@ -38,29 +36,31 @@
             continue
         values = [v for v in values if len(v)]
         if len(values):
             filterqs.append({"terms": {field: values}})
     return {"bool": {"filter": filterqs, "should": shoulds, "minimum_should_match": 1}}
 
 
-def names_query(entity: EntityProxy, field: str = NAMES_FIELD) -> List[Clause]:
+def names_query(entity: EntityProxy) -> List[Clause]:
     names = entity.get_type_values(registry.name, matchable=True)
     shoulds = []
     for name in pick_names(names, limit=5):
         match = {
-            field: {
+            NAMES_FIELD: {
                 "query": name,
                 "fuzziness": "AUTO",
                 "minimum_should_match": "70%",
                 "boost": 3.0,
             }
         }
         shoulds.append({"match": match})
-    for token in tokenize_names(names):
-        shoulds.append({"term": {field: {"value": token}}})
+    for token in name_words(names):
+        shoulds.append({"term": {NAME_PART_FIELD: {"value": token}}})
+    for phoneme in soundex_names(names):
+        shoulds.append({"term": {SOUNDEX_FIELD: {"value": phoneme}}})
     return shoulds
 
 
 def entity_query(dataset: Dataset, entity: EntityProxy) -> Clause:
     shoulds: List[Clause] = []
     for prop, value in entity.itervalues():
         if prop.type == registry.name or not prop.matchable:
```

### Comparing `yente-3.3.1/yente/search/search.py` & `yente-3.4.0/yente/search/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 
 
 def result_entity(data: Dict[str, Any]) -> Optional[Entity]:
     source: Optional[Dict[str, Any]] = data.get("_source")
     if source is None or source.get("schema") is None:
         return None
     source["id"] = data.get("_id")
-    return Entity.from_dict(model, source)
+    entity = Entity.from_dict(model, source)
+    entity.datasets = set(source["datasets"])
+    return entity
 
 
 def result_total(result: ObjectApiResponse[Any]) -> TotalSpec:
     total: Dict[str, Any] = result.get("hits", {}).get("total")
     return TotalSpec(value=total["value"], relation=total["relation"])
```

### Comparing `yente-3.3.1/yente/settings.py` & `yente-3.4.0/yente/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def env_str(name: str, default: Optional[str] = None) -> Optional[str]:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.3.1"
+VERSION = "3.4.0"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE") or "yente"
 DESCRIPTION = """
@@ -29,27 +29,27 @@
 `yente` is the open source basis for the OpenSanctions SaaS API. Its matching
 and entity retrieval functionality is identical to the hosted API, but it does
 not include functionality for metered accounting of API requests.
 
 In this service, there is support for the following operations:
 
 * A simple text-based search for interactive applications (``/search``),
-* A query-by-example endpoint for KYC-style tasks (``/match``),
+* A query-by-example endpoint for screening tasks (``/match``),
 * Support for getting graph data for a particular entity (``/entities``),
 * Support for the OpenRefine Reconciliation API (``/reconcile``).
 
 The API uses JSON for data transfer and does not support authentication or access
 control.
 
 Further reading:
 
 * [Self-hosted OpenSanctions](https://www.opensanctions.org/docs/self-hosted/)
 * [Install and deployment](https://github.com/opensanctions/yente/blob/main/README.md)
 * Intro to the [entity data model](https://www.opensanctions.org/docs/entities/)
-* Tutorial: [Using the matching API to do KYC-style checks](https://www.opensanctions.org/articles/2022-02-01-matching-api/)
+* Tutorial: [Using the matching API to do screening checks](https://www.opensanctions.org/docs/api/matching/)
 * [Data dictionary](https://opensanctions.org/reference/)
 """
 
 TAGS: List[Dict[str, Any]] = [
     {
         "name": "Matching",
         "description": "Endpoints for conducting a user-facing entity search or "
@@ -91,14 +91,15 @@
 
 MANIFEST_DEFAULT_PATH = Path(__file__).parent.parent / "manifests/default.yml"
 MANIFEST = env_str("YENTE_MANIFEST") or str(MANIFEST_DEFAULT_PATH)
 CRON: Optional[Cron] = None
 CRONTAB = env_str("YENTE_CRONTAB", "*/30 * * * *")
 AUTO_REINDEX = as_bool(env_str("YENTE_AUTO_REINDEX", "true"))
 STREAM_LOAD = as_bool(env_str("YENTE_STREAM_LOAD", "true"))
+DEFAULT_ALGORITHM = env_str("YENTE_DEFAULT_ALGORITHM") or "regression-v1"
 
 DATA_PATH = Path(env_str("YENTE_DATA_PATH") or "/tmp")
 RESOURCES_PATH = Path(__file__).parent.joinpath("resources")
 
 BASE_SCHEMA = "Thing"
 PORT = int(env_str("YENTE_PORT") or env_str("PORT") or "8000")
 UPDATE_TOKEN = env_str("YENTE_UPDATE_TOKEN", "unsafe-default")
@@ -123,14 +124,14 @@
 ES_USERNAME = env_str("YENTE_ELASTICSEARCH_USERNAME")
 ES_PASSWORD = env_str("YENTE_ELASTICSEARCH_PASSWORD")
 ES_CLOUD_ID = env_str("YENTE_ELASTICSEARCH_CLOUD_ID")
 ES_SNIFF = as_bool(env_str("YENTE_ELASTICSEARCH_SNIFF") or "false")
 ES_INDEX = env_str("YENTE_ELASTICSEARCH_INDEX", "yente")
 ES_SHARDS = int(env_str("YENTE_ELASTICSEARCH_SHARDS") or "1")
 ENTITY_INDEX = f"{ES_INDEX}-entities"
-INDEX_VERSION = "002"
+INDEX_VERSION = "003"
 
 LOG_JSON = as_bool(env_str("YENTE_LOG_JSON", "false"))
 LOG_LEVEL = logging.DEBUG if DEBUG else logging.INFO
 
 # Used to pad out first_seen, last_seen on static collections
 RUN_TIME = datetime.utcnow().isoformat()[:19]
```

### Comparing `yente-3.3.1/yente/util.py` & `yente-3.4.0/yente/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.3.1/yente.egg-info/PKG-INFO` & `yente-3.4.0/yente.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.3.1
+Version: 3.4.0
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.3.1/yente.egg-info/SOURCES.txt` & `yente-3.4.0/yente.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 yente/data/freebase.py
 yente/data/loader.py
 yente/data/manifest.py
 yente/data/util.py
 yente/resources/favicon.ico
 yente/routers/__init__.py
 yente/routers/admin.py
+yente/routers/match.py
 yente/routers/reconcile.py
 yente/routers/search.py
 yente/routers/util.py
 yente/search/__init__.py
 yente/search/base.py
 yente/search/indexer.py
 yente/search/mapping.py
```

### Comparing `yente-3.3.1/yente.egg-info/requires.txt` & `yente-3.4.0/yente.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 followthemoney==3.3.0
-nomenklatura==2.9.5
-asyncstdlib==3.10.6
+nomenklatura==2.11.0
+asyncstdlib==3.10.7
 aiocron==1.8
 aiocsv==1.2.4
 aiofiles==23.1.0
-types-aiofiles==23.1.0.1
+types-aiofiles==23.1.0.2
 aiohttp[speedups]==3.8.4
 elasticsearch[async]==8.7.0
 fastapi==0.95.1
-uvicorn[standard]==0.21.1
+uvicorn[standard]==0.22.0
 python-multipart==0.0.6
 email-validator==2.0.0.post2
 structlog==23.1.0
 pyicu==2.11
-orjson==3.8.10
+jellyfish==0.11.2
+orjson==3.8.11
 text-unidecode==1.3
 click==8.0.4
 normality==2.4.0
 languagecodes==1.1.1
 countrynames==1.14.3
 fingerprints==1.1.0
 pantomime==0.6.0
```

