# Comparing `tmp/notion-vzhd1701-fork-0.0.36.tar.gz` & `tmp/notion_vzhd1701_fork-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-vzhd1701-fork-0.0.36.tar", max compression
+gzip compressed data, was "notion_vzhd1701_fork-0.0.37.tar", max compression
```

## Comparing `notion-vzhd1701-fork-0.0.36.tar` & `notion_vzhd1701_fork-0.0.37.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1058 2022-12-06 07:51:46.453574 notion-vzhd1701-fork-0.0.36/LICENSE
--rw-r--r--   0        0        0        0 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/__init__.py
--rw-r--r--   0        0        0    24687 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/block.py
--rw-r--r--   0        0        0    16173 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/client.py
--rw-r--r--   0        0        0    27115 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/collection.py
--rw-r--r--   0        0        0      108 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/logger.py
--rw-r--r--   0        0        0     3693 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/maps.py
--rw-r--r--   0        0        0     9350 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/markdown.py
--rw-r--r--   0        0        0     8200 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/monitor.py
--rw-r--r--   0        0        0      997 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/operations.py
--rw-r--r--   0        0        0     4480 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/records.py
--rw-r--r--   0        0        0      290 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/settings.py
--rw-r--r--   0        0        0     9398 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/smoke_test.py
--rw-r--r--   0        0        0     1636 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/space.py
--rw-r--r--   0        0        0    14955 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/store.py
--rw-r--r--   0        0        0     1258 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/user.py
--rw-r--r--   0        0        0     2851 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/utils.py
--rw-r--r--   0        0        0     2225 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/notion/utils_ssl.py
--rw-r--r--   0        0        0      641 2022-12-06 07:51:46.457574 notion-vzhd1701-fork-0.0.36/pyproject.toml
--rw-r--r--   0        0        0      900 2022-12-06 07:51:57.204806 notion-vzhd1701-fork-0.0.36/setup.py
--rw-r--r--   0        0        0     1075 2022-12-06 07:51:57.205096 notion-vzhd1701-fork-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-05-06 07:12:08.027606 notion_vzhd1701_fork-0.0.37/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/__init__.py
+-rw-r--r--   0        0        0    24687 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/block.py
+-rw-r--r--   0        0        0    16173 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/client.py
+-rw-r--r--   0        0        0    27115 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/collection.py
+-rw-r--r--   0        0        0      108 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/logger.py
+-rw-r--r--   0        0        0     3693 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/maps.py
+-rw-r--r--   0        0        0     9350 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/markdown.py
+-rw-r--r--   0        0        0     8200 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/monitor.py
+-rw-r--r--   0        0        0      997 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/operations.py
+-rw-r--r--   0        0        0     4480 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/records.py
+-rw-r--r--   0        0        0      290 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/settings.py
+-rw-r--r--   0        0        0     9398 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/smoke_test.py
+-rw-r--r--   0        0        0     1636 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/space.py
+-rw-r--r--   0        0        0    14955 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/store.py
+-rw-r--r--   0        0        0     1258 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/user.py
+-rw-r--r--   0        0        0     2851 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/utils.py
+-rw-r--r--   0        0        0     2279 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/notion/utils_ssl.py
+-rw-r--r--   0        0        0      641 2023-05-06 07:12:08.031607 notion_vzhd1701_fork-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 notion_vzhd1701_fork-0.0.37/PKG-INFO
```

### Comparing `notion-vzhd1701-fork-0.0.36/LICENSE` & `notion_vzhd1701_fork-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/block.py` & `notion_vzhd1701_fork-0.0.37/notion/block.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/client.py` & `notion_vzhd1701_fork-0.0.37/notion/client.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/collection.py` & `notion_vzhd1701_fork-0.0.37/notion/collection.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/maps.py` & `notion_vzhd1701_fork-0.0.37/notion/maps.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/markdown.py` & `notion_vzhd1701_fork-0.0.37/notion/markdown.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/monitor.py` & `notion_vzhd1701_fork-0.0.37/notion/monitor.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/operations.py` & `notion_vzhd1701_fork-0.0.37/notion/operations.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/records.py` & `notion_vzhd1701_fork-0.0.37/notion/records.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/smoke_test.py` & `notion_vzhd1701_fork-0.0.37/notion/smoke_test.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/space.py` & `notion_vzhd1701_fork-0.0.37/notion/space.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/store.py` & `notion_vzhd1701_fork-0.0.37/notion/store.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/user.py` & `notion_vzhd1701_fork-0.0.37/notion/user.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/utils.py` & `notion_vzhd1701_fork-0.0.37/notion/utils.py`

 * *Files identical despite different names*

### Comparing `notion-vzhd1701-fork-0.0.36/notion/utils_ssl.py` & `notion_vzhd1701_fork-0.0.37/notion/utils_ssl.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     needed to avoid cloudflare bot detector that returns 403 on some requests
     this makes the requests library have the same TLS fingerprint as httpx
     in the future cloudflare may ban this signature also
     in that case we can use different cipher suite to alter TLS signature even further
     https://stackoverflow.com/questions/64967706/python-requests-https-code-403-without-but-code-200-when-using-burpsuite
     """
 
-    context = create_urllib3_context()
+    CIPHERS = ('DEFAULT:@SECLEVEL=2')
+
+    context = create_urllib3_context(ciphers=CIPHERS)
     set_minimum_tls_version_1_2(context)
     context.options &= ~ssl.OP_NO_TICKET
 
     return context
 
 
 class HTTPAdapterTLS(HTTPAdapter):
```

### Comparing `notion-vzhd1701-fork-0.0.36/pyproject.toml` & `notion_vzhd1701_fork-0.0.37/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "notion-vzhd1701-fork"
-version = "0.0.36"
+version = "0.0.37"
 description = "Fork of https://github.com/jamalex/notion-py"
 authors = ["Jamie Alexandre <jamalex@gmail.com>"]
 maintainers = ["vzhd1701 <vzhd1701@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/vzhd1701/notion-py"
 packages = [
     { include = "notion" },
```

### Comparing `notion-vzhd1701-fork-0.0.36/PKG-INFO` & `notion_vzhd1701_fork-0.0.37/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: notion-vzhd1701-fork
-Version: 0.0.36
+Version: 0.0.37
 Summary: Fork of https://github.com/jamalex/notion-py
 Home-page: https://github.com/vzhd1701/notion-py
 License: MIT
 Author: Jamie Alexandre
 Author-email: jamalex@gmail.com
 Maintainer: vzhd1701
 Maintainer-email: vzhd1701@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: commonmark (>=0.9.1,<0.10.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
```

