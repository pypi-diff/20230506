# Comparing `tmp/multicallable-5.0.0.tar.gz` & `tmp/multicallable-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/hassan/Documents/codes/deusfinance/multicallable/dist/tmprbl27g9d/multicallable-5.0.0.tar", last modified: Tue Apr  4 14:05:35 2023, max compression
+gzip compressed data, was "/home/hassan/Documents/codes/deusfinance/multicallable/dist/tmp88kvdulz/multicallable-5.0.1.tar", last modified: Sat May  6 14:24:34 2023, max compression
```

## Comparing `multicallable-5.0.0.tar` & `multicallable-5.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-04 14:05:35.000000 multicallable-5.0.0/
--rw-r--r--   0 hassan    (1000) hassan    (1000)     1074 2023-01-24 14:27:32.000000 multicallable-5.0.0/LICENCE
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4131 2023-04-04 14:05:35.000000 multicallable-5.0.0/PKG-INFO
--rw-r--r--   0 hassan    (1000) hassan    (1000)     3582 2023-02-28 12:46:08.000000 multicallable-5.0.0/README.md
--rw-r--r--   0 hassan    (1000) hassan    (1000)      103 2022-12-05 11:39:52.000000 multicallable-5.0.0/pyproject.toml
--rw-r--r--   0 hassan    (1000) hassan    (1000)      674 2023-04-04 14:05:35.000000 multicallable-5.0.0/setup.cfg
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-04 14:05:35.000000 multicallable-5.0.0/src/
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-04 14:05:35.000000 multicallable-5.0.0/src/multicallable/
--rw-r--r--   0 hassan    (1000) hassan    (1000)      424 2023-04-04 14:02:41.000000 multicallable-5.0.0/src/multicallable/__init__.py
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-04 14:05:35.000000 multicallable-5.0.0/src/multicallable/multicall/
--rw-r--r--   0 hassan    (1000) hassan    (1000)      117 2023-04-04 13:25:46.000000 multicallable-5.0.0/src/multicallable/multicall/__init__.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     6785 2022-12-15 11:24:06.000000 multicallable-5.0.0/src/multicallable/multicall/constants.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4886 2023-04-04 14:00:44.000000 multicallable-5.0.0/src/multicallable/multicall/multicall.py
--rw-r--r--   0 hassan    (1000) hassan    (1000)     3990 2023-04-04 13:53:09.000000 multicallable-5.0.0/src/multicallable/multicallable.py
-drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-04-04 14:05:35.000000 multicallable-5.0.0/src/multicallable.egg-info/
--rw-r--r--   0 hassan    (1000) hassan    (1000)     4131 2023-04-04 14:05:35.000000 multicallable-5.0.0/src/multicallable.egg-info/PKG-INFO
--rw-r--r--   0 hassan    (1000) hassan    (1000)      393 2023-04-04 14:05:35.000000 multicallable-5.0.0/src/multicallable.egg-info/SOURCES.txt
--rw-r--r--   0 hassan    (1000) hassan    (1000)        1 2023-04-04 14:05:35.000000 multicallable-5.0.0/src/multicallable.egg-info/dependency_links.txt
--rw-r--r--   0 hassan    (1000) hassan    (1000)       14 2023-04-04 14:05:35.000000 multicallable-5.0.0/src/multicallable.egg-info/top_level.txt
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     1074 2023-01-24 14:27:32.000000 multicallable-5.0.1/LICENCE
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     4131 2023-05-06 14:24:34.000000 multicallable-5.0.1/PKG-INFO
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     3582 2023-02-28 12:46:08.000000 multicallable-5.0.1/README.md
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      103 2022-12-05 11:39:52.000000 multicallable-5.0.1/pyproject.toml
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      674 2023-05-06 14:24:34.000000 multicallable-5.0.1/setup.cfg
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      424 2023-05-06 14:22:17.000000 multicallable-5.0.1/src/multicallable/__init__.py
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable/multicall/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      117 2023-04-04 13:25:46.000000 multicallable-5.0.1/src/multicallable/multicall/__init__.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     7362 2023-05-06 14:21:30.000000 multicallable-5.0.1/src/multicallable/multicall/constants.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     4886 2023-04-04 14:00:44.000000 multicallable-5.0.1/src/multicallable/multicall/multicall.py
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     3990 2023-04-04 13:53:09.000000 multicallable-5.0.1/src/multicallable/multicallable.py
+drwxr-xr-x   0 hassan    (1000) hassan    (1000)        0 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/
+-rw-r--r--   0 hassan    (1000) hassan    (1000)     4131 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/PKG-INFO
+-rw-r--r--   0 hassan    (1000) hassan    (1000)      393 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/SOURCES.txt
+-rw-r--r--   0 hassan    (1000) hassan    (1000)        1 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/dependency_links.txt
+-rw-r--r--   0 hassan    (1000) hassan    (1000)       14 2023-05-06 14:24:34.000000 multicallable-5.0.1/src/multicallable.egg-info/top_level.txt
```

### Comparing `multicallable-5.0.0/LICENCE` & `multicallable-5.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `multicallable-5.0.0/PKG-INFO` & `multicallable-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicallable
-Version: 5.0.0
+Version: 5.0.1
 Summary: Easy way to work with Multicall package
 Home-page: https://github.com/deusfinance/multicallable
 Author: Hassan Abbasi, Mojtaba Farokhi
 Author-email: hassan.abbp@gmail.com
 Project-URL: Bug Tracker, https://github.com/deusfinance/multicallable/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multicallable-5.0.0/README.md` & `multicallable-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `multicallable-5.0.0/setup.cfg` & `multicallable-5.0.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multicallable
-version = 5.0.0
+version = 5.0.1
 author = Hassan Abbasi, Mojtaba Farokhi
 author_email = hassan.abbp@gmail.com
 description = Easy way to work with Multicall package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/deusfinance/multicallable
 project_urls =
```

### Comparing `multicallable-5.0.0/src/multicallable/multicall/constants.py` & `multicallable-5.0.1/src/multicallable/multicall/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,20 @@
     1285: 'moonriver',
     1284: 'moonbeam',
     25: 'cronos',
     288: 'boba',
     100: 'gnosis',
     42220: 'celo',
     1088: 'metis',
+    42170: 'arbitrum-nova',
+    97: 'bsc-testnet',
+    80001: 'mumbai',  # Polygon testnet
+    4002: 'fantom-testnet',
+    421613: 'arbitrum-goerli',
+    43113: 'fuji',  # Avalanche testnet
     3: 'ropsten',
     42: 'kovan',
     4: 'rinkeby',
     5: 'goerli',
 }
 
 MULTICALL_ADDRESS = {
@@ -32,12 +38,18 @@
     'moonriver': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'moonbeam': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'cronos': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'boba': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'gnosis': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'celo': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'metis': '0xcA11bde05977b3631167028862bE2a173976CA11',
+    'arbitrum-nova': '0xcA11bde05977b3631167028862bE2a173976CA11',
+    'bsc-testnet': '0xcA11bde05977b3631167028862bE2a173976CA11',
+    'mumbai': '0xcA11bde05977b3631167028862bE2a173976CA11',
+    'fantom-testnet': '0xcA11bde05977b3631167028862bE2a173976CA11',
+    'arbitrum-goerli': '0xcA11bde05977b3631167028862bE2a173976CA11',
+    'fuji': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'ropsten': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'kovan': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'rinkeby': '0xcA11bde05977b3631167028862bE2a173976CA11',
     'goerli': '0xcA11bde05977b3631167028862bE2a173976CA11',
 }
```

### Comparing `multicallable-5.0.0/src/multicallable/multicall/multicall.py` & `multicallable-5.0.1/src/multicallable/multicall/multicall.py`

 * *Files identical despite different names*

### Comparing `multicallable-5.0.0/src/multicallable/multicallable.py` & `multicallable-5.0.1/src/multicallable/multicallable.py`

 * *Files identical despite different names*

### Comparing `multicallable-5.0.0/src/multicallable.egg-info/PKG-INFO` & `multicallable-5.0.1/src/multicallable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicallable
-Version: 5.0.0
+Version: 5.0.1
 Summary: Easy way to work with Multicall package
 Home-page: https://github.com/deusfinance/multicallable
 Author: Hassan Abbasi, Mojtaba Farokhi
 Author-email: hassan.abbp@gmail.com
 Project-URL: Bug Tracker, https://github.com/deusfinance/multicallable/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

