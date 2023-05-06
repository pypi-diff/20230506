# Comparing `tmp/aliyun-python-sdk-nlp-automl-0.0.8.tar.gz` & `tmp/aliyun-python-sdk-nlp-automl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-nlp-automl-0.0.8.tar", last modified: Tue Sep  8 03:27:55 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-nlp-automl-0.0.9.tar", last modified: Mon Dec 28 07:46:01 2020, max compression
```

## Comparing `aliyun-python-sdk-nlp-automl-0.0.8.tar` & `aliyun-python-sdk-nlp-automl-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1572 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyun_python_sdk_nlp_automl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1572 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyun_python_sdk_nlp_automl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      840 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyun_python_sdk_nlp_automl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyun_python_sdk_nlp_automl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyun_python_sdk_nlp_automl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyun_python_sdk_nlp_automl.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/
--rw-r--r--   0 root         (0) root         (0)       21 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/
--rw-r--r--   0 root         (0) root         (0)     2764 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/CreateAsyncPredictRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/GetAsyncPredictRequest.py
--rw-r--r--   0 root         (0) root         (0)     2084 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/GetPredictResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1652 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/RunContactReviewRequest.py
--rw-r--r--   0 root         (0) root         (0)     1864 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/RunPreTrainServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1978 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/RunSmartCallServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-09-08 03:27:55.000000 aliyun-python-sdk-nlp-automl-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2487 2020-09-08 03:27:54.000000 aliyun-python-sdk-nlp-automl-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1572 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyun_python_sdk_nlp_automl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1572 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyun_python_sdk_nlp_automl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1924 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyun_python_sdk_nlp_automl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyun_python_sdk_nlp_automl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyun_python_sdk_nlp_automl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyun_python_sdk_nlp_automl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/
+-rw-r--r--   0 root         (0) root         (0)       21 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/
+-rw-r--r--   0 root         (0) root         (0)     1970 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/AddMTInterveneWordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/AddMtIntervenePackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/BindIntervenePackageAndModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1580 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/GetPredictDocRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/InvokeActionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/PredictMTModelByDocRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/PredictMTModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20190701/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/
+-rw-r--r--   0 root         (0) root         (0)     2764 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/CreateAsyncPredictRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/CreateDatasetRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/CreateDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/CreateModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/CreateProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/DeleteModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/DeployModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/GetAsyncPredictRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/GetModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/GetPredictResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/ListDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/ListModelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/RunContactReviewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/RunPreTrainServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/RunSmartCallServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2020-12-28 07:46:01.000000 aliyun-python-sdk-nlp-automl-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2487 2020-12-28 07:46:00.000000 aliyun-python-sdk-nlp-automl-0.0.9/setup.py
```

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/PKG-INFO` & `aliyun-python-sdk-nlp-automl-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-nlp-automl
-Version: 0.0.8
+Version: 0.0.9
 Summary: The nlp-automl module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-nlp-automl
```

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/README.rst` & `aliyun-python-sdk-nlp-automl-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/aliyun_python_sdk_nlp_automl.egg-info/PKG-INFO` & `aliyun-python-sdk-nlp-automl-0.0.9/aliyun_python_sdk_nlp_automl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-nlp-automl
-Version: 0.0.8
+Version: 0.0.9
 Summary: The nlp-automl module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-nlp-automl
```

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/endpoint.py` & `aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/CreateAsyncPredictRequest.py` & `aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/CreateAsyncPredictRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/GetAsyncPredictRequest.py` & `aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/GetAsyncPredictRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/GetPredictResultRequest.py` & `aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/GetPredictResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/RunContactReviewRequest.py` & `aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/RunContactReviewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/RunPreTrainServiceRequest.py` & `aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/RunPreTrainServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/aliyunsdknlp_automl/request/v20191111/RunSmartCallServiceRequest.py` & `aliyun-python-sdk-nlp-automl-0.0.9/aliyunsdknlp_automl/request/v20191111/RunSmartCallServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlp-automl-0.0.8/setup.py` & `aliyun-python-sdk-nlp-automl-0.0.9/setup.py`

 * *Files identical despite different names*

