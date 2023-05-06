# Comparing `tmp/valo_api-2.0.0.tar.gz` & `tmp/valo_api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valo_api-2.0.0.tar", max compression
+gzip compressed data, was "valo_api-2.0.1.tar", max compression
```

## Comparing `valo_api-2.0.0.tar` & `valo_api-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1074 2023-05-05 22:41:41.516197 valo_api-2.0.0/LICENSE
--rw-r--r--   0        0        0     2451 2023-05-05 22:41:41.516197 valo_api-2.0.0/README.md
--rw-r--r--   0        0        0     3115 2023-05-05 22:41:41.520197 valo_api-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      388 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/__init__.py
--rw-r--r--   0        0        0      793 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/config.py
--rw-r--r--   0        0        0     3905 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/endpoint.py
--rw-r--r--   0        0        0      405 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/endpoints/__init__.py
--rw-r--r--   0        0        0    10241 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/endpoints_config.py
--rw-r--r--   0        0        0        0 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/exceptions/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/exceptions/rate_limit.py
--rw-r--r--   0        0        0     2069 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/exceptions/valo_api_exception.py
--rw-r--r--   0        0        0        0 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/__init__.py
--rw-r--r--   0        0        0      410 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/account_details.py
--rw-r--r--   0        0        0      541 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/competitive_updates_raw.py
--rw-r--r--   0        0        0      858 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/content.py
--rw-r--r--   0        0        0      371 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/error_response.py
--rw-r--r--   0        0        0      917 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/leaderboard.py
--rw-r--r--   0        0        0     1169 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/lifetime_match.py
--rw-r--r--   0        0        0     5550 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/match_details_raw.py
--rw-r--r--   0        0        0     5996 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/match_history.py
--rw-r--r--   0        0        0      299 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/match_history_raw.py
--rw-r--r--   0        0        0     1317 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/mmr_details.py
--rw-r--r--   0        0        0      628 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/mmr_history.py
--rw-r--r--   0        0        0     1306 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/mmr_raw.py
--rw-r--r--   0        0        0      817 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/status.py
--rw-r--r--   0        0        0     1093 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/store_featured.py
--rw-r--r--   0        0        0      853 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/store_offers.py
--rw-r--r--   0        0        0      157 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/version_info.py
--rw-r--r--   0        0        0      236 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/responses/website.py
--rw-r--r--   0        0        0        0 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/utils/__init__.py
--rw-r--r--   0        0        0      216 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/utils/dict_struct.py
--rw-r--r--   0        0        0     3821 2023-05-05 22:41:41.660198 valo_api-2.0.0/valo_api/utils/fetch_endpoint.py
--rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 valo_api-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-06 21:37:12.170305 valo_api-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2451 2023-05-06 21:37:12.170305 valo_api-2.0.1/README.md
+-rw-r--r--   0        0        0     3115 2023-05-06 21:37:12.174305 valo_api-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-05-06 21:37:12.306307 valo_api-2.0.1/valo_api/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-06 21:37:12.306307 valo_api-2.0.1/valo_api/config.py
+-rw-r--r--   0        0        0     5217 2023-05-06 21:37:12.306307 valo_api-2.0.1/valo_api/endpoint.py
+-rw-r--r--   0        0        0      405 2023-05-06 21:37:12.306307 valo_api-2.0.1/valo_api/endpoints/__init__.py
+-rw-r--r--   0        0        0    10241 2023-05-06 21:37:12.306307 valo_api-2.0.1/valo_api/endpoints_config.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:37:12.306307 valo_api-2.0.1/valo_api/exceptions/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/exceptions/rate_limit.py
+-rw-r--r--   0        0        0     2069 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/exceptions/valo_api_exception.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/account_details.py
+-rw-r--r--   0        0        0      541 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/competitive_updates_raw.py
+-rw-r--r--   0        0        0      858 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/content.py
+-rw-r--r--   0        0        0      371 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/error_response.py
+-rw-r--r--   0        0        0      917 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/leaderboard.py
+-rw-r--r--   0        0        0     1169 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/lifetime_match.py
+-rw-r--r--   0        0        0     5550 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/match_details_raw.py
+-rw-r--r--   0        0        0     5996 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/match_history.py
+-rw-r--r--   0        0        0      299 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/match_history_raw.py
+-rw-r--r--   0        0        0     1317 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/mmr_details.py
+-rw-r--r--   0        0        0      628 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/mmr_history.py
+-rw-r--r--   0        0        0     1306 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/mmr_raw.py
+-rw-r--r--   0        0        0      817 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/status.py
+-rw-r--r--   0        0        0     1093 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/store_featured.py
+-rw-r--r--   0        0        0      853 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/store_offers.py
+-rw-r--r--   0        0        0      157 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/version_info.py
+-rw-r--r--   0        0        0      236 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/responses/website.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/utils/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/utils/dict_struct.py
+-rw-r--r--   0        0        0     3821 2023-05-06 21:37:12.310307 valo_api-2.0.1/valo_api/utils/fetch_endpoint.py
+-rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 valo_api-2.0.1/PKG-INFO
```

### Comparing `valo_api-2.0.0/LICENSE` & `valo_api-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/README.md` & `valo_api-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/pyproject.toml` & `valo_api-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "valo_api"
-version = "2.0.0"
+version = "2.0.1"
 description = "Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api"
 readme = "README.md"
 authors = ["Manuel Raimann <raimannma@outlook.de>"]
 license = "MIT"
 repository = "https://github.com/raimannma/ValorantAPI"
 homepage = "https://github.com/raimannma/ValorantAPI"
```

### Comparing `valo_api-2.0.0/valo_api/config.py` & `valo_api-2.0.1/valo_api/config.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/endpoint.py` & `valo_api-2.0.1/valo_api/endpoint.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,27 +5,33 @@
     Generic,
     Iterable,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
+    get_args,
 )
 
 import io
 from dataclasses import dataclass
 
 import msgspec
 from PIL import Image
 from requests import Response
 
 from valo_api.exceptions.valo_api_exception import ValoAPIException
 from valo_api.responses.error_response import ErrorResponse
 from valo_api.utils.dict_struct import DictStruct
-from valo_api.utils.fetch_endpoint import fetch_endpoint, fetch_endpoint_async
+from valo_api.utils.fetch_endpoint import fetch_endpoint
+
+try:
+    from valo_api.utils.fetch_endpoint import fetch_endpoint_async
+except ImportError:
+    pass
 
 R = TypeVar("R")
 
 
 def response_type(api_type: R):
     class APIResponse(DictStruct):
         status: int
@@ -46,19 +52,24 @@
     data_response: bool = True
 
     def endpoint_wrappers(
         self,
     ) -> Iterable[Tuple[str, Callable[..., Union[R, Awaitable[R]]]]]:
         for version in self.versions:
             yield f"{self.f_name}_{version}", self._get_endpoint_wrapper(version)
-            yield f"{self.f_name}_{version}_async", self._get_endpoint_wrapper(
-                version, True
-            )
+            if "fetch_endpoint_async" in globals():
+                yield f"{self.f_name}_{version}_async", self._get_endpoint_wrapper(
+                    version, True
+                )
         yield self.f_name, self._get_endpoint_wrapper()
-        yield f"{self.f_name}_async", self._get_endpoint_wrapper(async_function=True)
+
+        if "fetch_endpoint_async" in globals():
+            yield f"{self.f_name}_async", self._get_endpoint_wrapper(
+                async_function=True
+            )
 
     def _get_endpoint_wrapper(
         self, version: Optional[str] = None, async_function: bool = False
     ) -> Union[Callable[..., Union[R, Awaitable[R]]]]:
         if async_function:
 
             async def wrapper(**kwargs) -> R:
@@ -71,16 +82,38 @@
 
             def wrapper(**kwargs) -> R:
                 kwargs["version"] = kwargs.get("version", version)
                 for k in self.kwargs.keys():
                     kwargs[k] = kwargs.get(k, "")
                 return self._get_endpoint(**kwargs)
 
+        doc_title = f"{self.f_name} ({version})" if version else self.f_name
+        doc_title = doc_title.replace("_", " ").title() + " from the API."
+        doc_args = "\n\nArgs:\n"
+        if self.kwargs:
+            for k, v in self.kwargs.items():
+                args = ", ".join(
+                    [a.__name__ for a in get_args(v) if a.__name__ != "NoneType"]
+                )
+                if len(args) > 0:
+                    args = f"[{args}]"
+                doc_args += f"    {k}: {v.__name__}{args}\n"
+        returns = self.recursive_typing_get_args(self.return_type)
+        doc_return = f"\n\nReturns:\n    {returns}: API Fetch Result\n"
+        doc_raise = "\n\nRaises:\n    ValoAPIException: If the API returns an error."
+        wrapper.__doc__ = doc_title + doc_args + doc_return + doc_raise
+
         return wrapper
 
+    def recursive_typing_get_args(self, type_: Type) -> str:
+        args = get_args(type_)
+        if not args or len(args) == 0:
+            return f"{type_.__name__}"
+        return ", ".join({self.recursive_typing_get_args(arg) for arg in args})
+
     def build_query_args(self, **kwargs):
         formatted_query_args = (
             {k: v.format(**kwargs) for k, v in self.query_args.items() if v}
             if self.query_args
             else None
         )
         if formatted_query_args is None:
```

### Comparing `valo_api-2.0.0/valo_api/endpoints_config.py` & `valo_api-2.0.1/valo_api/endpoints_config.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/exceptions/rate_limit.py` & `valo_api-2.0.1/valo_api/exceptions/rate_limit.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/exceptions/valo_api_exception.py` & `valo_api-2.0.1/valo_api/exceptions/valo_api_exception.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/competitive_updates_raw.py` & `valo_api-2.0.1/valo_api/responses/competitive_updates_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/content.py` & `valo_api-2.0.1/valo_api/responses/content.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/leaderboard.py` & `valo_api-2.0.1/valo_api/responses/leaderboard.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/lifetime_match.py` & `valo_api-2.0.1/valo_api/responses/lifetime_match.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/match_details_raw.py` & `valo_api-2.0.1/valo_api/responses/match_details_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/match_history.py` & `valo_api-2.0.1/valo_api/responses/match_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/mmr_details.py` & `valo_api-2.0.1/valo_api/responses/mmr_details.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/mmr_history.py` & `valo_api-2.0.1/valo_api/responses/mmr_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/mmr_raw.py` & `valo_api-2.0.1/valo_api/responses/mmr_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/status.py` & `valo_api-2.0.1/valo_api/responses/status.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/store_featured.py` & `valo_api-2.0.1/valo_api/responses/store_featured.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/responses/store_offers.py` & `valo_api-2.0.1/valo_api/responses/store_offers.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/valo_api/utils/fetch_endpoint.py` & `valo_api-2.0.1/valo_api/utils/fetch_endpoint.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.0/PKG-INFO` & `valo_api-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valo-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api
 Home-page: https://github.com/raimannma/ValorantAPI
 License: MIT
 Author: Manuel Raimann
 Author-email: raimannma@outlook.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

