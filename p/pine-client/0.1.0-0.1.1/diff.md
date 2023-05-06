# Comparing `tmp/pine_client-0.1.0.tar.gz` & `tmp/pine_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pine_client-0.1.0.tar", max compression
+gzip compressed data, was "pine_client-0.1.1.tar", max compression
```

## Comparing `pine_client-0.1.0.tar` & `pine_client-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       95 2023-05-05 13:04:36.000000 pine_client-0.1.0/README.md
--rw-r--r--   0        0        0       60 2023-05-05 13:04:36.000000 pine_client-0.1.0/pine_client/__init__.py
--rw-r--r--   0        0        0    32255 2023-05-05 13:04:36.000000 pine_client-0.1.0/pine_client/client.py
--rw-r--r--   0        0        0     2669 2023-05-05 13:04:36.000000 pine_client-0.1.0/pine_client/utils.py
--rw-r--r--   0        0        0      505 2023-05-05 13:04:50.000000 pine_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 pine_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       95 2023-05-06 16:01:56.000000 pine_client-0.1.1/README.md
+-rw-r--r--   0        0        0       60 2023-05-06 16:01:56.000000 pine_client-0.1.1/pine_client/__init__.py
+-rw-r--r--   0        0        0    32326 2023-05-06 16:01:56.000000 pine_client-0.1.1/pine_client/client.py
+-rw-r--r--   0        0        0     2669 2023-05-06 16:01:56.000000 pine_client-0.1.1/pine_client/utils.py
+-rw-r--r--   0        0        0      505 2023-05-06 16:02:11.000000 pine_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 pine_client-0.1.1/PKG-INFO
```

### Comparing `pine_client-0.1.0/pine_client/client.py` & `pine_client-0.1.1/pine_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -781,14 +781,18 @@
                     "Invalid response received, the 'd' property is missing."
                 )
             if singular:
                 if len(data_d) > 1:
                     raise Exception(
                         "Returned multiple results when only one was expected."
                     )
+
+                if len(data_d) == 0:
+                    return None
+
                 return data_d[0]
             return data_d
 
         return transform_get_result_fn
 
     def get(self, params: Params) -> Any:
         result = self.request({**params, "method": "GET"})
```

### Comparing `pine_client-0.1.0/pine_client/utils.py` & `pine_client-0.1.1/pine_client/utils.py`

 * *Files identical despite different names*

### Comparing `pine_client-0.1.0/PKG-INFO` & `pine_client-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pine-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: This module provides the core layer for python interface for the pinejs API
 Author: Balena
 Author-email: info@balena.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

