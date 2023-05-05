# Comparing `tmp/valo_api-1.7.0.tar.gz` & `tmp/valo_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valo_api-1.7.0.tar", max compression
+gzip compressed data, was "valo_api-2.0.0.tar", max compression
```

## Comparing `valo_api-1.7.0.tar` & `valo_api-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,33 @@
--rw-r--r--   0        0        0     1074 2023-04-19 19:00:01.506382 valo_api-1.7.0/LICENSE
--rw-r--r--   0        0        0     2451 2023-04-19 19:00:01.506382 valo_api-1.7.0/README.md
--rw-r--r--   0        0        0     3115 2023-04-19 19:00:01.510382 valo_api-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      388 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/__init__.py
--rw-r--r--   0        0        0      793 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/config.py
--rw-r--r--   0        0        0     7593 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/__init__.py
--rw-r--r--   0        0        0     8990 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/account_details.py
--rw-r--r--   0        0        0     3369 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/content.py
--rw-r--r--   0        0        0     3508 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/crosshair.py
--rw-r--r--   0        0        0    11005 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/leaderboard.py
--rw-r--r--   0        0        0    14178 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/lifetime_matches.py
--rw-r--r--   0        0        0     3787 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/match_details.py
--rw-r--r--   0        0        0    14140 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/match_history.py
--rw-r--r--   0        0        0    17609 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/mmr_details.py
--rw-r--r--   0        0        0     9551 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/mmr_history.py
--rw-r--r--   0        0        0     8985 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/raw.py
--rw-r--r--   0        0        0     3961 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/status.py
--rw-r--r--   0        0        0     4828 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/store_featured.py
--rw-r--r--   0        0        0     4659 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/store_offers.py
--rw-r--r--   0        0        0     3578 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/version_info.py
--rw-r--r--   0        0        0     3782 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints/website.py
--rw-r--r--   0        0        0     1407 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/endpoints_config.py
--rw-r--r--   0        0        0        0 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/exceptions/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/exceptions/rate_limit.py
--rw-r--r--   0        0        0     2069 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/exceptions/valo_api_exception.py
--rw-r--r--   0        0        0        0 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/__init__.py
--rw-r--r--   0        0        0      410 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/account_details.py
--rw-r--r--   0        0        0      541 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/competitive_updates_raw.py
--rw-r--r--   0        0        0      858 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/content.py
--rw-r--r--   0        0        0      371 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/error_response.py
--rw-r--r--   0        0        0      917 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/leaderboard.py
--rw-r--r--   0        0        0     1175 2023-04-19 19:00:01.646381 valo_api-1.7.0/valo_api/responses/lifetime_match.py
--rw-r--r--   0        0        0     5550 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/match_details_raw.py
--rw-r--r--   0        0        0     5996 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/match_history.py
--rw-r--r--   0        0        0      299 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/match_history_raw.py
--rw-r--r--   0        0        0     1317 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/mmr_details.py
--rw-r--r--   0        0        0      628 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/mmr_history.py
--rw-r--r--   0        0        0     1306 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/mmr_raw.py
--rw-r--r--   0        0        0      817 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/status.py
--rw-r--r--   0        0        0     1093 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/store_featured.py
--rw-r--r--   0        0        0      853 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/store_offers.py
--rw-r--r--   0        0        0      157 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/version_info.py
--rw-r--r--   0        0        0      236 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/responses/website.py
--rw-r--r--   0        0        0        0 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/utils/__init__.py
--rw-r--r--   0        0        0      216 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/utils/dict_struct.py
--rw-r--r--   0        0        0     3821 2023-04-19 19:00:01.650381 valo_api-1.7.0/valo_api/utils/fetch_endpoint.py
--rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 valo_api-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-05 22:41:41.516197 valo_api-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2451 2023-05-05 22:41:41.516197 valo_api-2.0.0/README.md
+-rw-r--r--   0        0        0     3115 2023-05-05 22:41:41.520197 valo_api-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/config.py
+-rw-r--r--   0        0        0     3905 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/endpoint.py
+-rw-r--r--   0        0        0      405 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/endpoints/__init__.py
+-rw-r--r--   0        0        0    10241 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/endpoints_config.py
+-rw-r--r--   0        0        0        0 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/exceptions/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/exceptions/rate_limit.py
+-rw-r--r--   0        0        0     2069 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/exceptions/valo_api_exception.py
+-rw-r--r--   0        0        0        0 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/account_details.py
+-rw-r--r--   0        0        0      541 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/competitive_updates_raw.py
+-rw-r--r--   0        0        0      858 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/content.py
+-rw-r--r--   0        0        0      371 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/error_response.py
+-rw-r--r--   0        0        0      917 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/leaderboard.py
+-rw-r--r--   0        0        0     1169 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/lifetime_match.py
+-rw-r--r--   0        0        0     5550 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/match_details_raw.py
+-rw-r--r--   0        0        0     5996 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/match_history.py
+-rw-r--r--   0        0        0      299 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/match_history_raw.py
+-rw-r--r--   0        0        0     1317 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/mmr_details.py
+-rw-r--r--   0        0        0      628 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/mmr_history.py
+-rw-r--r--   0        0        0     1306 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/mmr_raw.py
+-rw-r--r--   0        0        0      817 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/status.py
+-rw-r--r--   0        0        0     1093 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/store_featured.py
+-rw-r--r--   0        0        0      853 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/store_offers.py
+-rw-r--r--   0        0        0      157 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/version_info.py
+-rw-r--r--   0        0        0      236 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/website.py
+-rw-r--r--   0        0        0        0 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/utils/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/utils/dict_struct.py
+-rw-r--r--   0        0        0     3821 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/utils/fetch_endpoint.py
+-rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 valo_api-2.0.0/PKG-INFO
```

### Comparing `valo_api-1.7.0/LICENSE` & `valo_api-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/README.md` & `valo_api-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/pyproject.toml` & `valo_api-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "valo_api"
-version = "1.7.0"
+version = "2.0.0"
 description = "Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api"
 readme = "README.md"
 authors = ["Manuel Raimann <raimannma@outlook.de>"]
 license = "MIT"
 repository = "https://github.com/raimannma/ValorantAPI"
 homepage = "https://github.com/raimannma/ValorantAPI"
 
@@ -59,15 +59,15 @@
 sphinxcontrib-serializinghtml = "^1.1.5"
 sphinx-rtd-theme = "^1.1.1"
 sphinx-autodoc-typehints = "^1.19.5"
 autodocsumm = "^0.2.8"
 responses = ">=0.22,<0.24"
 pytest-parallel = "^0.1.1"
 pytest-split = "^0.8.0"
-tomlkit = "<0.11.8"
+tomlkit = "<0.11.9"
 colorama = "^0.4.6"
 aioresponses = "^0.7.4"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 
 [tool.poetry.extras]
 async = [
     "aiohttp",
```

### Comparing `valo_api-1.7.0/valo_api/config.py` & `valo_api-2.0.0/valo_api/config.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/exceptions/rate_limit.py` & `valo_api-2.0.0/valo_api/exceptions/rate_limit.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/exceptions/valo_api_exception.py` & `valo_api-2.0.0/valo_api/exceptions/valo_api_exception.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/competitive_updates_raw.py` & `valo_api-2.0.0/valo_api/responses/competitive_updates_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/content.py` & `valo_api-2.0.0/valo_api/responses/content.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/leaderboard.py` & `valo_api-2.0.0/valo_api/responses/leaderboard.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/lifetime_match.py` & `valo_api-2.0.0/valo_api/responses/lifetime_match.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import Optional
 
 from valo_api.utils.dict_struct import DictStruct
 
 
 class LifetimeMatchMapV1(DictStruct):
     id: str
     name: str
```

### Comparing `valo_api-1.7.0/valo_api/responses/match_details_raw.py` & `valo_api-2.0.0/valo_api/responses/match_details_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/match_history.py` & `valo_api-2.0.0/valo_api/responses/match_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/mmr_details.py` & `valo_api-2.0.0/valo_api/responses/mmr_details.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/mmr_history.py` & `valo_api-2.0.0/valo_api/responses/mmr_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/mmr_raw.py` & `valo_api-2.0.0/valo_api/responses/mmr_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/status.py` & `valo_api-2.0.0/valo_api/responses/status.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/store_featured.py` & `valo_api-2.0.0/valo_api/responses/store_featured.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/responses/store_offers.py` & `valo_api-2.0.0/valo_api/responses/store_offers.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/valo_api/utils/fetch_endpoint.py` & `valo_api-2.0.0/valo_api/utils/fetch_endpoint.py`

 * *Files identical despite different names*

### Comparing `valo_api-1.7.0/PKG-INFO` & `valo_api-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valo-api
-Version: 1.7.0
+Version: 2.0.0
 Summary: Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api
 Home-page: https://github.com/raimannma/ValorantAPI
 License: MIT
 Author: Manuel Raimann
 Author-email: raimannma@outlook.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

