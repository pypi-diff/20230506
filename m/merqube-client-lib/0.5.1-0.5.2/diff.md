# Comparing `tmp/merqube_client_lib-0.5.1.tar.gz` & `tmp/merqube_client_lib-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.5.1.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.5.2.tar", max compression
```

## Comparing `merqube_client_lib-0.5.1.tar` & `merqube_client_lib-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/LICENSE
--rw-r--r--   0        0        0      377 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      367 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     3022 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/py.typed
--rw-r--r--   0        0        0        0 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0    12483 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/secapi/client.py
--rw-r--r--   0        0        0    11209 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0      677 2023-05-05 10:49:31.597042 merqube_client_lib-0.5.1/merqube_client_lib/util.py
--rw-r--r--   0        0        0     1713 2023-05-05 10:49:31.601042 merqube_client_lib-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/LICENSE
+-rw-r--r--   0        0        0      377 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      367 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     3022 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0        0 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    12450 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/secapi/client.py
+-rw-r--r--   0        0        0    11209 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1713 2023-05-06 11:49:38.671388 merqube_client_lib-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.2/PKG-INFO
```

### Comparing `merqube_client_lib-0.5.1/LICENSE` & `merqube_client_lib-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.1/merqube_client_lib/logging.py` & `merqube_client_lib-0.5.2/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.1/merqube_client_lib/mocker.py` & `merqube_client_lib-0.5.2/merqube_client_lib/mocker.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.1/merqube_client_lib/secapi/client.py` & `merqube_client_lib-0.5.2/merqube_client_lib/secapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,18 +134,50 @@
         self,
         session: Optional[MerqubeAPISession] = None,
         token: Optional[str] = None,
         **session_kwargs: Any,
     ):
         super().__init__(session=session, token=token, **session_kwargs)
 
-    def get_metrics_for_security(
+    def _get_security_metrics_helper(
         self,
         *,
         sec_type: str,
+        metrics: str | Iterable[str],
+        sec_names: str | Iterable[str] | None = None,
+        sec_ids: str | Iterable[str] | None = None,
+        start_date: str | pd.Timestamp | None = None,
+        end_date: str | pd.Timestamp | None = None,
+        addl_options: AddlSecapiOptions | None = None,
+    ) -> SecAPIRecordsResponse:
+        """
+        if sec_names and sec_ids are both []/None, it gets ALL securities.
+        """
+
+        metrics_list = [metrics] if isinstance(metrics, str) else list(metrics)
+
+        # Join did not work correctly for KeyViews and Tuples are badly behaved, so we'll remap them to lists.
+        sec_names_list = ([sec_names] if isinstance(sec_names, str) else list(sec_names)) if sec_names else []
+        sec_ids_list = ([sec_ids] if isinstance(sec_ids, str) else list(sec_ids)) if sec_ids else []
+
+        query_options = {
+            "metrics": metrics_list,
+            "names": sec_names_list,
+            "ids": sec_ids_list,
+            "start_date": pd.Timestamp(start_date).isoformat() if start_date else start_date,
+            "end_date": pd.Timestamp(end_date).isoformat() if end_date else end_date,
+        }
+        if addl_options:
+            query_options.update(addl_options)
+
+        return self._collection_helper(url=f"/security/{sec_type}", query_options=query_options)
+
+    def get_metrics_for_security(
+        self,
+        sec_type: str,
         sec_id: str | None = None,
         sec_name: str | None = None,
     ) -> list[SecapiMetricDefinition]:
         """
         Get the list of metrics that are currently available for a security
         Can query by id or name
         """
@@ -153,15 +185,14 @@
 
         return self.session.get_collection(
             f"/security/{sec_type}/{sec_id}/metrics" if sec_id else f"/security/{sec_type}/metrics?name={sec_name}"
         )
 
     def get_security_definitions_mapping_table(
         self,
-        *,
         sec_type: str,
         sec_names: str | Iterable[str] | None = None,
         sec_ids: str | Iterable[str] | None = None,
         addl_options: AddlSecapiOptions | None = None,
     ) -> MappingTable:
         """
         Lists defined (and permissioned) securities for a type.
@@ -178,50 +209,16 @@
         rec_data = self._collection_helper(
             url=f"/security/{sec_type}",
             query_options=query_options,
         )
 
         return {c["id"]: c["name"] for c in rec_data} if sec_ids else {c["name"]: c["id"] for c in rec_data}
 
-    def _get_security_metrics_helper(
-        self,
-        *,
-        sec_type: str,
-        metrics: str | Iterable[str],
-        sec_names: str | Iterable[str] | None = None,
-        sec_ids: str | Iterable[str] | None = None,
-        start_date: str | pd.Timestamp | None = None,
-        end_date: str | pd.Timestamp | None = None,
-        addl_options: AddlSecapiOptions | None = None,
-    ) -> SecAPIRecordsResponse:
-        """
-        if sec_names and sec_ids are both []/None, it gets ALL securities.
-        """
-
-        metrics_list = [metrics] if isinstance(metrics, str) else list(metrics)
-
-        # Join did not work correctly for KeyViews and Tuples are badly behaved, so we'll remap them to lists.
-        sec_names_list = ([sec_names] if isinstance(sec_names, str) else list(sec_names)) if sec_names else []
-        sec_ids_list = ([sec_ids] if isinstance(sec_ids, str) else list(sec_ids)) if sec_ids else []
-
-        query_options = {
-            "metrics": metrics_list,
-            "names": sec_names_list,
-            "ids": sec_ids_list,
-            "start_date": pd.Timestamp(start_date).isoformat() if start_date else start_date,
-            "end_date": pd.Timestamp(end_date).isoformat() if end_date else end_date,
-        }
-        if addl_options:
-            query_options.update(addl_options)
-
-        return self._collection_helper(url=f"/security/{sec_type}", query_options=query_options)
-
     def get_security_metrics(
         self,
-        *,
         sec_type: str,
         metrics: str | Iterable[str],  # Secapi doesnt support fetching all metrics yet; cant be None
         sec_names: str | Iterable[str] | None = None,
         sec_ids: str | Iterable[str] | None = None,
         start_date: str | pd.Timestamp | None = None,
         end_date: str | pd.Timestamp | None = None,
         addl_options: AddlSecapiOptions | None = None,
```

### Comparing `merqube_client_lib-0.5.1/merqube_client_lib/session.py` & `merqube_client_lib-0.5.2/merqube_client_lib/session.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.1/merqube_client_lib/util.py` & `merqube_client_lib-0.5.2/merqube_client_lib/util.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.1/pyproject.toml` & `merqube_client_lib-0.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.5.1"
+version = "0.5.2"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
```

### Comparing `merqube_client_lib-0.5.1/PKG-INFO` & `merqube_client_lib-0.5.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.5.1
+Version: 0.5.2
 Summary: MerQube IndexAPI + SecAPI client library
 Home-page: https://github.com/merqube/merqube-client-lib
 License: Apache-2.0
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

