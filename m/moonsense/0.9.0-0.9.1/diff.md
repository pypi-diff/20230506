# Comparing `tmp/moonsense-0.9.0.tar.gz` & `tmp/moonsense-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonsense-0.9.0.tar", last modified: Tue Nov  8 02:08:42 2022, max compression
+gzip compressed data, was "moonsense-0.9.1.tar", last modified: Tue Nov  8 02:11:05 2022, max compression
```

## Comparing `moonsense-0.9.0.tar` & `moonsense-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:08:42.096735 moonsense-0.9.0/
--rw-r--r--   0 bogdan     (501) staff       (20)    11358 2021-10-19 18:59:19.000000 moonsense-0.9.0/LICENSE
--rw-r--r--   0 bogdan     (501) staff       (20)        0 2021-10-19 18:59:19.000000 moonsense-0.9.0/MANIFEST.in
--rw-r--r--   0 bogdan     (501) staff       (20)     2860 2022-11-08 02:08:42.096449 moonsense-0.9.0/PKG-INFO
--rwxr-xr-x   0 bogdan     (501) staff       (20)     2262 2022-10-13 03:11:25.000000 moonsense-0.9.0/README.md
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:08:42.087856 moonsense-0.9.0/moonsense/
--rwxr-xr-x   0 bogdan     (501) staff       (20)      449 2022-11-08 02:08:37.000000 moonsense-0.9.0/moonsense/__init__.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:08:42.089706 moonsense-0.9.0/moonsense/cli/
--rw-r--r--   0 bogdan     (501) staff       (20)     1003 2022-11-08 02:08:37.000000 moonsense-0.9.0/moonsense/cli/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2518 2022-11-08 02:08:37.000000 moonsense-0.9.0/moonsense/cli/download.py
--rwxr-xr-x   0 bogdan     (501) staff       (20)    16421 2022-11-08 02:08:37.000000 moonsense-0.9.0/moonsense/client.py
--rw-r--r--   0 bogdan     (501) staff       (20)     7976 2022-11-08 02:08:37.000000 moonsense-0.9.0/moonsense/download.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:08:42.095430 moonsense-0.9.0/moonsense/models/
--rw-r--r--   0 bogdan     (501) staff       (20)      128 2021-12-21 02:56:44.000000 moonsense-0.9.0/moonsense/models/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)   134755 2022-10-13 21:58:05.000000 moonsense-0.9.0/moonsense/models/bundle_v2_pb2.py
--rw-r--r--   0 bogdan     (501) staff       (20)    14796 2022-10-13 21:58:05.000000 moonsense-0.9.0/moonsense/models/common_v2_pb2.py
--rw-r--r--   0 bogdan     (501) staff       (20)    16667 2022-10-13 21:58:05.000000 moonsense-0.9.0/moonsense/models/control_plane_v2_pb2.py
--rw-r--r--   0 bogdan     (501) staff       (20)    84289 2022-10-13 03:11:47.000000 moonsense-0.9.0/moonsense/models/data_plane_v2_pb2.py
--rw-r--r--   0 bogdan     (501) staff       (20)    17434 2022-10-13 03:11:47.000000 moonsense-0.9.0/moonsense/models/error_reporting_pb2.py
--rw-r--r--   0 bogdan     (501) staff       (20)    13716 2022-11-08 02:08:37.000000 moonsense-0.9.0/moonsense/models/feature_pb2.py
--rw-r--r--   0 bogdan     (501) staff       (20)     5509 2022-10-13 03:11:47.000000 moonsense-0.9.0/moonsense/models/pagination_pb2.py
--rw-r--r--   0 bogdan     (501) staff       (20)   121513 2022-10-13 03:11:47.000000 moonsense-0.9.0/moonsense/models/validate_pb2.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1175 2021-12-21 02:56:44.000000 moonsense-0.9.0/moonsense/pd.py
--rw-r--r--   0 bogdan     (501) staff       (20)      663 2022-11-08 02:08:37.000000 moonsense-0.9.0/moonsense/util.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:08:42.089266 moonsense-0.9.0/moonsense.egg-info/
--rw-r--r--   0 bogdan     (501) staff       (20)     2860 2022-11-08 02:08:42.000000 moonsense-0.9.0/moonsense.egg-info/PKG-INFO
--rw-r--r--   0 bogdan     (501) staff       (20)      704 2022-11-08 02:08:42.000000 moonsense-0.9.0/moonsense.egg-info/SOURCES.txt
--rw-r--r--   0 bogdan     (501) staff       (20)        1 2022-11-08 02:08:42.000000 moonsense-0.9.0/moonsense.egg-info/dependency_links.txt
--rw-r--r--   0 bogdan     (501) staff       (20)       50 2022-11-08 02:08:42.000000 moonsense-0.9.0/moonsense.egg-info/entry_points.txt
--rw-r--r--   0 bogdan     (501) staff       (20)       76 2022-11-08 02:08:42.000000 moonsense-0.9.0/moonsense.egg-info/requires.txt
--rw-r--r--   0 bogdan     (501) staff       (20)       10 2022-11-08 02:08:42.000000 moonsense-0.9.0/moonsense.egg-info/top_level.txt
--rw-r--r--   0 bogdan     (501) staff       (20)       38 2022-11-08 02:08:42.096822 moonsense-0.9.0/setup.cfg
--rwxr-xr-x   0 bogdan     (501) staff       (20)     1602 2022-11-08 02:08:37.000000 moonsense-0.9.0/setup.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:11:05.768103 moonsense-0.9.1/
+-rw-r--r--   0 bogdan     (501) staff       (20)    11358 2021-10-19 18:59:19.000000 moonsense-0.9.1/LICENSE
+-rw-r--r--   0 bogdan     (501) staff       (20)        0 2021-10-19 18:59:19.000000 moonsense-0.9.1/MANIFEST.in
+-rw-r--r--   0 bogdan     (501) staff       (20)     2860 2022-11-08 02:11:05.767853 moonsense-0.9.1/PKG-INFO
+-rwxr-xr-x   0 bogdan     (501) staff       (20)     2262 2022-10-13 03:11:25.000000 moonsense-0.9.1/README.md
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:11:05.759033 moonsense-0.9.1/moonsense/
+-rwxr-xr-x   0 bogdan     (501) staff       (20)      449 2022-11-08 02:08:37.000000 moonsense-0.9.1/moonsense/__init__.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:11:05.761431 moonsense-0.9.1/moonsense/cli/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1003 2022-11-08 02:08:37.000000 moonsense-0.9.1/moonsense/cli/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     2518 2022-11-08 02:08:37.000000 moonsense-0.9.1/moonsense/cli/download.py
+-rwxr-xr-x   0 bogdan     (501) staff       (20)    16355 2022-11-08 02:10:29.000000 moonsense-0.9.1/moonsense/client.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     7976 2022-11-08 02:08:37.000000 moonsense-0.9.1/moonsense/download.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:11:05.766963 moonsense-0.9.1/moonsense/models/
+-rw-r--r--   0 bogdan     (501) staff       (20)      128 2021-12-21 02:56:44.000000 moonsense-0.9.1/moonsense/models/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)   134755 2022-10-13 21:58:05.000000 moonsense-0.9.1/moonsense/models/bundle_v2_pb2.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    14796 2022-10-13 21:58:05.000000 moonsense-0.9.1/moonsense/models/common_v2_pb2.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    16667 2022-10-13 21:58:05.000000 moonsense-0.9.1/moonsense/models/control_plane_v2_pb2.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    84289 2022-10-13 03:11:47.000000 moonsense-0.9.1/moonsense/models/data_plane_v2_pb2.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    17434 2022-10-13 03:11:47.000000 moonsense-0.9.1/moonsense/models/error_reporting_pb2.py
+-rw-r--r--   0 bogdan     (501) staff       (20)    13716 2022-11-08 02:08:37.000000 moonsense-0.9.1/moonsense/models/feature_pb2.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     5509 2022-10-13 03:11:47.000000 moonsense-0.9.1/moonsense/models/pagination_pb2.py
+-rw-r--r--   0 bogdan     (501) staff       (20)   121513 2022-10-13 03:11:47.000000 moonsense-0.9.1/moonsense/models/validate_pb2.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     1175 2021-12-21 02:56:44.000000 moonsense-0.9.1/moonsense/pd.py
+-rw-r--r--   0 bogdan     (501) staff       (20)      663 2022-11-08 02:08:37.000000 moonsense-0.9.1/moonsense/util.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2022-11-08 02:11:05.760764 moonsense-0.9.1/moonsense.egg-info/
+-rw-r--r--   0 bogdan     (501) staff       (20)     2860 2022-11-08 02:11:05.000000 moonsense-0.9.1/moonsense.egg-info/PKG-INFO
+-rw-r--r--   0 bogdan     (501) staff       (20)      704 2022-11-08 02:11:05.000000 moonsense-0.9.1/moonsense.egg-info/SOURCES.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)        1 2022-11-08 02:11:05.000000 moonsense-0.9.1/moonsense.egg-info/dependency_links.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)       50 2022-11-08 02:11:05.000000 moonsense-0.9.1/moonsense.egg-info/entry_points.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)       76 2022-11-08 02:11:05.000000 moonsense-0.9.1/moonsense.egg-info/requires.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)       10 2022-11-08 02:11:05.000000 moonsense-0.9.1/moonsense.egg-info/top_level.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)       38 2022-11-08 02:11:05.768185 moonsense-0.9.1/setup.cfg
+-rwxr-xr-x   0 bogdan     (501) staff       (20)     1602 2022-11-08 02:10:44.000000 moonsense-0.9.1/setup.py
```

### Comparing `moonsense-0.9.0/LICENSE` & `moonsense-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/PKG-INFO` & `moonsense-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonsense
-Version: 0.9.0
+Version: 0.9.1
 Summary: Moonsense Cloud API Client
 Home-page: https://github.com/moonsense/python-sdk.git
 Author: Moonsense Team
 Author-email: support@moonsense.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moonsense-0.9.0/README.md` & `moonsense-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/cli/__init__.py` & `moonsense-0.9.1/moonsense/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/cli/download.py` & `moonsense-0.9.1/moonsense/cli/download.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/client.py` & `moonsense-0.9.1/moonsense/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,25 +140,25 @@
 
             if platforms != None:
                 params.append(("filter[platforms][]", [p.value for p in platforms]))
 
             http_response = requests.get(
                 endpoint, params, **self._headers
             )
-            print(params)
+
             if http_response.status_code != 200:
                 raise RuntimeError(
                     f"unable to list sessions. status code: {http_response.status_code}"
                 )
 
             response = json_format.Parse(
                 http_response.text, SessionListResponse(), ignore_unknown_fields=True)
             if len(response.sessions) == 0:
                 return  # no more sessions
-            print(len(response.sessions))
+
             for session in response.sessions:
                 yield session
 
             if response.pagination.next_page is not None and response.pagination.next_page > 0:
                 page = response.pagination.current_page + 1
             else:
                 break
```

### Comparing `moonsense-0.9.0/moonsense/download.py` & `moonsense-0.9.1/moonsense/download.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/models/bundle_v2_pb2.py` & `moonsense-0.9.1/moonsense/models/bundle_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/models/common_v2_pb2.py` & `moonsense-0.9.1/moonsense/models/common_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/models/control_plane_v2_pb2.py` & `moonsense-0.9.1/moonsense/models/control_plane_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/models/data_plane_v2_pb2.py` & `moonsense-0.9.1/moonsense/models/data_plane_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/models/error_reporting_pb2.py` & `moonsense-0.9.1/moonsense/models/error_reporting_pb2.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/models/feature_pb2.py` & `moonsense-0.9.1/moonsense/models/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/models/pagination_pb2.py` & `moonsense-0.9.1/moonsense/models/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/models/validate_pb2.py` & `moonsense-0.9.1/moonsense/models/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/pd.py` & `moonsense-0.9.1/moonsense/pd.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense/util.py` & `moonsense-0.9.1/moonsense/util.py`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/moonsense.egg-info/PKG-INFO` & `moonsense-0.9.1/moonsense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonsense
-Version: 0.9.0
+Version: 0.9.1
 Summary: Moonsense Cloud API Client
 Home-page: https://github.com/moonsense/python-sdk.git
 Author: Moonsense Team
 Author-email: support@moonsense.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moonsense-0.9.0/moonsense.egg-info/SOURCES.txt` & `moonsense-0.9.1/moonsense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moonsense-0.9.0/setup.py` & `moonsense-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="moonsense",
-    version="0.9.0",
+    version="0.9.1",
     packages=find_packages(exclude=["tests*"]),
     description="Moonsense Cloud API Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': ['moonsense=moonsense.cli:main'],
     },
```

