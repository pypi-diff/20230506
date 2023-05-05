# Comparing `tmp/py_clob_client-0.6.0.tar.gz` & `tmp/py_clob_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_clob_client-0.6.0.tar", last modified: Wed Apr 19 16:51:51 2023, max compression
+gzip compressed data, was "py_clob_client-0.7.0.tar", last modified: Fri May  5 23:14:19 2023, max compression
```

## Comparing `py_clob_client-0.6.0.tar` & `py_clob_client-0.7.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.999919 py_clob_client-0.6.0/
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1067 2022-05-27 21:15:08.000000 py_clob_client-0.6.0/LICENSE
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-04-19 16:51:50.999780 py_clob_client-0.6.0/PKG-INFO
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2304 2023-02-01 18:41:38.000000 py_clob_client-0.6.0/README.md
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.994408 py_clob_client-0.6.0/py_clob_client/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.6.0/py_clob_client/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    15509 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/client.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2467 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/clob_types.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      453 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/constants.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      674 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/endpoints.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      871 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/exceptions.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.995353 py_clob_client-0.6.0/py_clob_client/headers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/headers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1473 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/headers/headers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.995634 py_clob_client-0.6.0/py_clob_client/http_helpers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.6.0/py_clob_client/http_helpers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     3850 2023-03-31 18:04:55.000000 py_clob_client-0.6.0/py_clob_client/http_helpers/helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.996471 py_clob_client-0.6.0/py_clob_client/order_builder/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/order_builder/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     3995 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/order_builder/builder.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)       26 2023-01-26 15:15:34.000000 py_clob_client-0.6.0/py_clob_client/order_builder/constants.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      629 2023-01-27 20:18:52.000000 py_clob_client-0.6.0/py_clob_client/order_builder/helpers.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      583 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/signer.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.997275 py_clob_client-0.6.0/py_clob_client/signing/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.6.0/py_clob_client/signing/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      795 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/signing/eip712.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      708 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/signing/hmac.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      186 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/py_clob_client/signing/model.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1040 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/py_clob_client/utilities.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.995148 py_clob_client-0.6.0/py_clob_client.egg-info/
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/PKG-INFO
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1247 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/SOURCES.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)        1 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/dependency_links.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       36 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/requires.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       21 2023-04-19 16:51:50.000000 py_clob_client-0.6.0/py_clob_client.egg-info/top_level.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       38 2023-04-19 16:51:50.999966 py_clob_client-0.6.0/setup.cfg
--rw-r--r--   0 poly-rodr   (505) staff       (20)      963 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/setup.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.997751 py_clob_client-0.6.0/tests/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/__init__.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.998068 py_clob_client-0.6.0/tests/headers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/headers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     3256 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/headers/test_headers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.998319 py_clob_client-0.6.0/tests/http_helpers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/http_helpers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2384 2023-03-31 18:04:55.000000 py_clob_client-0.6.0/tests/http_helpers/test_helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.998900 py_clob_client-0.6.0/tests/order_builder/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/order_builder/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    30909 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/tests/order_builder/test_builder.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      274 2023-01-27 20:18:52.000000 py_clob_client-0.6.0/tests/order_builder/test_helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-04-19 16:51:50.999564 py_clob_client-0.6.0/tests/signing/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/signing/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      757 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/signing/test_eip712.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      536 2022-09-23 20:43:25.000000 py_clob_client-0.6.0/tests/signing/test_hmac.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1172 2023-04-12 18:14:06.000000 py_clob_client-0.6.0/tests/test_client.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    33747 2023-04-19 16:44:09.000000 py_clob_client-0.6.0/tests/test_utilities.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.806583 py_clob_client-0.7.0/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1067 2022-05-27 21:15:08.000000 py_clob_client-0.7.0/LICENSE
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-05-05 23:14:19.806450 py_clob_client-0.7.0/PKG-INFO
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2304 2023-02-01 18:41:38.000000 py_clob_client-0.7.0/README.md
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.802968 py_clob_client-0.7.0/py_clob_client/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.7.0/py_clob_client/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    16135 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/py_clob_client/client.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2531 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/py_clob_client/clob_types.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      453 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/constants.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      713 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/py_clob_client/endpoints.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      871 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/exceptions.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.803665 py_clob_client-0.7.0/py_clob_client/headers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/headers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1473 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/headers/headers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.803844 py_clob_client-0.7.0/py_clob_client/http_helpers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.7.0/py_clob_client/http_helpers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     4213 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/py_clob_client/http_helpers/helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.804451 py_clob_client-0.7.0/py_clob_client/order_builder/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/order_builder/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     3995 2023-04-19 16:44:09.000000 py_clob_client-0.7.0/py_clob_client/order_builder/builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       26 2023-01-26 15:15:34.000000 py_clob_client-0.7.0/py_clob_client/order_builder/constants.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      629 2023-01-27 20:18:52.000000 py_clob_client-0.7.0/py_clob_client/order_builder/helpers.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      583 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/signer.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.804951 py_clob_client-0.7.0/py_clob_client/signing/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.7.0/py_clob_client/signing/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      795 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/signing/eip712.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      708 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/signing/hmac.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      186 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/signing/model.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1040 2023-04-19 16:44:09.000000 py_clob_client-0.7.0/py_clob_client/utilities.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.803469 py_clob_client-0.7.0/py_clob_client.egg-info/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/PKG-INFO
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1226 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/SOURCES.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        1 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/dependency_links.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       36 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/requires.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       21 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/top_level.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       38 2023-05-05 23:14:19.806636 py_clob_client-0.7.0/setup.cfg
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      963 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/setup.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.805189 py_clob_client-0.7.0/tests/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/__init__.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.805465 py_clob_client-0.7.0/tests/headers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/headers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     3256 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/headers/test_headers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.805677 py_clob_client-0.7.0/tests/http_helpers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/http_helpers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2759 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/tests/http_helpers/test_helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.805997 py_clob_client-0.7.0/tests/order_builder/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/order_builder/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    30909 2023-04-19 16:44:09.000000 py_clob_client-0.7.0/tests/order_builder/test_builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      274 2023-01-27 20:18:52.000000 py_clob_client-0.7.0/tests/order_builder/test_helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.806292 py_clob_client-0.7.0/tests/signing/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/signing/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      757 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/signing/test_eip712.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      536 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/signing/test_hmac.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    33747 2023-04-19 16:44:09.000000 py_clob_client-0.7.0/tests/test_utilities.py
```

### Comparing `py_clob_client-0.6.0/LICENSE` & `py_clob_client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/PKG-INFO` & `py_clob_client-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_clob_client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python client for the Polymarket CLOB
 Home-page: https://github.com/Polymarket/py-clob-client
 Author: Polymarket Engineering
 Author-email: engineering@polymarket.com
 Maintainer: Polymarket Engineering
 Maintainer-email: engineering@polymarket.com
 Project-URL: Bug Tracker, https://github.com/Polymarket/py-clob-client/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py_clob_client Version: 0.6.0 Summary: Python
+Metadata-Version: 2.1 Name: py_clob_client Version: 0.7.0 Summary: Python
 client for the Polymarket CLOB Home-page: https://github.com/Polymarket/py-
 clob-client Author: Polymarket Engineering Author-email:
 engineering@polymarket.com Maintainer: Polymarket Engineering Maintainer-email:
 engineering@polymarket.com Project-URL: Bug Tracker, https://github.com/
 Polymarket/py-clob-client/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.9.10 Description-Content-Type:
```

### Comparing `py_clob_client-0.6.0/README.md` & `py_clob_client-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client/client.py` & `py_clob_client-0.7.0/py_clob_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,35 +25,38 @@
     TIME,
     TRADES,
     GET_TRADE_NOTIFICATIONS,
     DROP_TRADE_NOTIFICATIONS,
     GET_BALANCE_ALLOWANCE,
     IS_ORDER_SCORING,
     GET_TICK_SIZE,
+    ARE_ORDERS_SCORING,
 )
 from .clob_types import (
     ApiCreds,
     FilterParams,
     OrderArgs,
     RequestArgs,
     TradeNotificationParams,
     OrderBookSummary,
     BalanceAllowanceParams,
     OrderScoringParams,
     TickSize,
+    OrdersScoringParams,
 )
 from .exceptions import PolyException
 from .http_helpers.helpers import (
     add_query_params,
     delete,
     get,
     post,
     add_trade_notifications_query_params,
     add_balance_allowance_params_to_url,
     add_order_scoring_params_to_url,
+    add_orders_scoring_params_to_url,
 )
 from py_order_utils.config import get_contract_config
 from .constants import L0, L1, L1_AUTH_UNAVAILABLE, L2, L2_AUTH_UNAVAILABLE
 from .utilities import (
     parse_raw_orderbook_summary,
     generate_orderbook_summary_hash,
     order_to_json,
@@ -460,7 +463,20 @@
         self.assert_level_2_auth()
         request_args = RequestArgs(method="GET", request_path=IS_ORDER_SCORING)
         headers = create_level_2_headers(self.signer, self.creds, request_args)
         url = add_order_scoring_params_to_url(
             "{}{}".format(self.host, IS_ORDER_SCORING), params
         )
         return get(url, headers=headers)
+
+    def are_orders_scoring(self, params: OrdersScoringParams):
+        """
+        Check if the orders are currently scoring
+        Requires Level 2 authentication
+        """
+        self.assert_level_2_auth()
+        request_args = RequestArgs(method="GET", request_path=ARE_ORDERS_SCORING)
+        headers = create_level_2_headers(self.signer, self.creds, request_args)
+        url = add_orders_scoring_params_to_url(
+            "{}{}".format(self.host, ARE_ORDERS_SCORING), params
+        )
+        return get(url, headers=headers)
```

### Comparing `py_clob_client-0.6.0/py_clob_client/clob_types.py` & `py_clob_client-0.7.0/py_clob_client/clob_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,14 +131,19 @@
 
 
 @dataclass
 class OrderScoringParams:
     orderId: str
 
 
+@dataclass
+class OrdersScoringParams:
+    orderIds: list[str]
+
+
 TickSize = Literal["0.1", "0.01", "0.001", "0.0001"]
 
 
 @dataclass
 class RoundConfig:
     price: float
     size: float
```

### Comparing `py_clob_client-0.6.0/py_clob_client/endpoints.py` & `py_clob_client-0.7.0/py_clob_client/endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 MID_POINT = "/midpoint"
 PRICE = "/price"
 GET_LAST_TRADE_PRICE = "/last-trade-price"
 GET_TRADE_NOTIFICATIONS = "/trade-notifications"
 DROP_TRADE_NOTIFICATIONS = "/drop-trade-notifications"
 GET_BALANCE_ALLOWANCE = "/balance-allowance"
 IS_ORDER_SCORING = "/order-scoring"
+ARE_ORDERS_SCORING = "/orders-scoring"
 GET_TICK_SIZE = "/tick-size"
```

### Comparing `py_clob_client-0.6.0/py_clob_client/exceptions.py` & `py_clob_client-0.7.0/py_clob_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client/headers/headers.py` & `py_clob_client-0.7.0/py_clob_client/headers/headers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client/http_helpers/helpers.py` & `py_clob_client-0.7.0/py_clob_client/http_helpers/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 
 from py_clob_client.clob_types import (
     FilterParams,
     TradeNotificationParams,
     BalanceAllowanceParams,
     OrderScoringParams,
+    OrdersScoringParams,
 )
 
 from ..exceptions import PolyApiException
 
 GET = "GET"
 POST = "POST"
 DELETE = "DELETE"
@@ -131,7 +132,21 @@
     """
     url = base_url
     if params:
         url = url + "?"
         if params.orderId:
             url = build_query_params(url, "order_id", params.orderId)
     return url
+
+
+def add_orders_scoring_params_to_url(
+    base_url: str, params: OrdersScoringParams = None
+) -> str:
+    """
+    Adds query parameters to a url
+    """
+    url = base_url
+    if params:
+        url = url + "?"
+        if params.orderIds:
+            url = build_query_params(url, "order_ids", ",".join(params.orderIds))
+    return url
```

### Comparing `py_clob_client-0.6.0/py_clob_client/order_builder/builder.py` & `py_clob_client-0.7.0/py_clob_client/order_builder/builder.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client/order_builder/helpers.py` & `py_clob_client-0.7.0/py_clob_client/order_builder/helpers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client/signer.py` & `py_clob_client-0.7.0/py_clob_client/signer.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client/signing/eip712.py` & `py_clob_client-0.7.0/py_clob_client/signing/eip712.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client/signing/hmac.py` & `py_clob_client-0.7.0/py_clob_client/signing/hmac.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client/utilities.py` & `py_clob_client-0.7.0/py_clob_client/utilities.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/py_clob_client.egg-info/PKG-INFO` & `py_clob_client-0.7.0/py_clob_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-clob-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python client for the Polymarket CLOB
 Home-page: https://github.com/Polymarket/py-clob-client
 Author: Polymarket Engineering
 Author-email: engineering@polymarket.com
 Maintainer: Polymarket Engineering
 Maintainer-email: engineering@polymarket.com
 Project-URL: Bug Tracker, https://github.com/Polymarket/py-clob-client/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-clob-client Version: 0.6.0 Summary: Python
+Metadata-Version: 2.1 Name: py-clob-client Version: 0.7.0 Summary: Python
 client for the Polymarket CLOB Home-page: https://github.com/Polymarket/py-
 clob-client Author: Polymarket Engineering Author-email:
 engineering@polymarket.com Maintainer: Polymarket Engineering Maintainer-email:
 engineering@polymarket.com Project-URL: Bug Tracker, https://github.com/
 Polymarket/py-clob-client/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.9.10 Description-Content-Type:
```

### Comparing `py_clob_client-0.6.0/py_clob_client.egg-info/SOURCES.txt` & `py_clob_client-0.7.0/py_clob_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 py_clob_client/order_builder/constants.py
 py_clob_client/order_builder/helpers.py
 py_clob_client/signing/__init__.py
 py_clob_client/signing/eip712.py
 py_clob_client/signing/hmac.py
 py_clob_client/signing/model.py
 tests/__init__.py
-tests/test_client.py
 tests/test_utilities.py
 tests/headers/__init__.py
 tests/headers/test_headers.py
 tests/http_helpers/__init__.py
 tests/http_helpers/test_helpers.py
 tests/order_builder/__init__.py
 tests/order_builder/test_builder.py
```

### Comparing `py_clob_client-0.6.0/setup.py` & `py_clob_client-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_clob_client",
-    version="0.6.0",
+    version="0.7.0",
     author="Polymarket Engineering",
     author_email="engineering@polymarket.com",
     maintainer="Polymarket Engineering",
     maintainer_email="engineering@polymarket.com",
     description="Python client for the Polymarket CLOB",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `py_clob_client-0.6.0/tests/headers/test_headers.py` & `py_clob_client-0.7.0/tests/headers/test_headers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/tests/http_helpers/test_helpers.py` & `py_clob_client-0.7.0/tests/http_helpers/test_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from unittest import TestCase
 from py_clob_client.clob_types import (
     FilterParams,
     TradeNotificationParams,
     BalanceAllowanceParams,
     AssetType,
     OrderScoringParams,
+    OrdersScoringParams,
 )
 
 from py_clob_client.http_helpers.helpers import (
     build_query_params,
     add_query_params,
     add_trade_notifications_query_params,
     add_balance_allowance_params_to_url,
     add_order_scoring_params_to_url,
+    add_orders_scoring_params_to_url,
 )
 
 
 class TestHelpers(TestCase):
     def test_build_query_params(self):
         # last is ?
         url = build_query_params("http://tracker?", "q1", "a")
@@ -64,7 +66,15 @@
     def test_add_order_scoring_params_to_url(self):
         url = add_order_scoring_params_to_url(
             "http://tracker",
             OrderScoringParams(orderId="0x0123abc"),
         )
         self.assertIsNotNone(url)
         self.assertEqual(url, "http://tracker?order_id=0x0123abc")
+
+    def test_add_orders_scoring_params_to_urll(self):
+        url = add_orders_scoring_params_to_url(
+            "http://tracker",
+            OrdersScoringParams(orderIds=["0x0", "0x1", "0x2"]),
+        )
+        self.assertIsNotNone(url)
+        self.assertEqual(url, "http://tracker?order_ids=0x0,0x1,0x2")
```

### Comparing `py_clob_client-0.6.0/tests/order_builder/test_builder.py` & `py_clob_client-0.7.0/tests/order_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/tests/signing/test_eip712.py` & `py_clob_client-0.7.0/tests/signing/test_eip712.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/tests/signing/test_hmac.py` & `py_clob_client-0.7.0/tests/signing/test_hmac.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.6.0/tests/test_utilities.py` & `py_clob_client-0.7.0/tests/test_utilities.py`

 * *Files identical despite different names*

