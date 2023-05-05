# Comparing `tmp/graphql-api-1.3.2.tar.gz` & `tmp/graphql-api-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.3.2.tar", last modified: Fri May  5 12:27:33 2023, max compression
+gzip compressed data, was "graphql-api-1.3.3.tar", last modified: Fri May  5 22:59:55 2023, max compression
```

## Comparing `graphql-api-1.3.2.tar` & `graphql-api-1.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:27:33.984700 graphql-api-1.3.2/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-05 12:27:24.000000 graphql-api-1.3.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-05 12:27:24.000000 graphql-api-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 12:27:33.984700 graphql-api-1.3.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-05 12:27:24.000000 graphql-api-1.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-05 12:27:33.000000 graphql-api-1.3.2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:27:33.979700 graphql-api-1.3.2/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3382 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    23879 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    32840 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     3372 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5612 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:27:33.980700 graphql-api-1.3.2/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-05 12:27:33.984700 graphql-api-1.3.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-05 12:27:24.000000 graphql-api-1.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:27:33.983700 graphql-api-1.3.2/tests/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5129 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_custom_types.py
--rwxrwxrwx   0 root         (0) root         (0)     5183 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_docstrings.py
--rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_error.py
--rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_filtering.py
--rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_graphql.py
--rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_relay.py
--rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:59:55.191846 graphql-api-1.3.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-05 22:59:45.000000 graphql-api-1.3.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-05 22:59:45.000000 graphql-api-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 22:59:55.191846 graphql-api-1.3.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-05 22:59:45.000000 graphql-api-1.3.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-05 22:59:54.000000 graphql-api-1.3.3/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:59:55.186845 graphql-api-1.3.3/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3382 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    23879 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     3372 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5612 2023-05-05 22:59:45.000000 graphql-api-1.3.3/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:59:55.188845 graphql-api-1.3.3/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 22:59:55.000000 graphql-api-1.3.3/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-05 22:59:55.000000 graphql-api-1.3.3/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 22:59:55.000000 graphql-api-1.3.3/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-05 22:59:55.000000 graphql-api-1.3.3/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 22:59:55.000000 graphql-api-1.3.3/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-05 22:59:55.192845 graphql-api-1.3.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-05 22:59:45.000000 graphql-api-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:59:55.191846 graphql-api-1.3.3/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5129 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_custom_types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5183 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-05 22:59:45.000000 graphql-api-1.3.3/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.3.2/LICENSE` & `graphql-api-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/PKG-INFO` & `graphql-api-1.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.2
+Version: 1.3.3
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.2/graphql-api-v1.3.2.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.3/graphql-api-v1.3.3.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.2/README.md` & `graphql-api-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/api.py` & `graphql-api-1.3.3/graphql_api/api.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/context.py` & `graphql-api-1.3.3/graphql_api/context.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.3/graphql_api/dataclass_mapping.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/error.py` & `graphql-api-1.3.3/graphql_api/error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/executor.py` & `graphql-api-1.3.3/graphql_api/executor.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/mapper.py` & `graphql-api-1.3.3/graphql_api/mapper.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/middleware.py` & `graphql-api-1.3.3/graphql_api/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/reduce.py` & `graphql-api-1.3.3/graphql_api/reduce.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/relay.py` & `graphql-api-1.3.3/graphql_api/relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/remote.py` & `graphql-api-1.3.3/graphql_api/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,19 +183,19 @@
                     http_timeout=self.http_timeout,
                     verify=self.verify,
                 )
             )
         except RequestException as e:
             import sys
 
-            err_msg = f"{e}, remote service '{self.name}' is unavailable."
+            err_msg = f"{e}, remote service '{self.name}' is unavailable '{self.url}'."
             raise type(e)(err_msg).with_traceback(sys.exc_info()[2])
 
         except ValueError as e:
-            raise ValueError(f"{e}, from remote service '{self.name}'.")
+            raise ValueError(f"{e}, from remote service '{self.name}' at '{self.url}'.")
 
         return ExecutionResult(data=json_.get("data"), errors=json_.get("errors"))
 
 
 class GraphQLMappers:
     def __init__(
         self, query_mapper: GraphQLTypeMapper, mutable_mapper: GraphQLTypeMapper
```

### Comparing `graphql-api-1.3.2/graphql_api/types.py` & `graphql-api-1.3.3/graphql_api/types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api/utils.py` & `graphql-api-1.3.3/graphql_api/utils.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.3/graphql_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.2
+Version: 1.3.3
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.2/graphql-api-v1.3.2.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.3/graphql-api-v1.3.3.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.2/graphql_api.egg-info/SOURCES.txt` & `graphql-api-1.3.3/graphql_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/setup.py` & `graphql-api-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_custom_types.py` & `graphql-api-1.3.3/tests/test_custom_types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_docstrings.py` & `graphql-api-1.3.3/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_error.py` & `graphql-api-1.3.3/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_filtering.py` & `graphql-api-1.3.3/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_graphql.py` & `graphql-api-1.3.3/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_relay.py` & `graphql-api-1.3.3/tests/test_relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_remote.py` & `graphql-api-1.3.3/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_schema.py` & `graphql-api-1.3.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.2/tests/test_subscriptions.py` & `graphql-api-1.3.3/tests/test_subscriptions.py`

 * *Files identical despite different names*

