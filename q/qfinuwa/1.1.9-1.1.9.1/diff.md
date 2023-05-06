# Comparing `tmp/qfinuwa-1.1.9.tar.gz` & `tmp/qfinuwa-1.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfinuwa-1.1.9.tar", last modified: Sat May  6 08:47:15 2023, max compression
+gzip compressed data, was "qfinuwa-1.1.9.1.tar", last modified: Sat May  6 09:42:16 2023, max compression
```

## Comparing `qfinuwa-1.1.9.tar` & `qfinuwa-1.1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:47:15.119421 qfinuwa-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-06 08:47:15.119421 qfinuwa-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-06 08:47:15.119421 qfinuwa-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:47:15.115421 qfinuwa-1.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:47:15.119421 qfinuwa-1.1.9/src/qfinuwa/
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/API.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/backtester.py
--rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:47:15.119421 qfinuwa-1.1.9/src/qfinuwa/opt/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/opt/_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/opt/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/opt/_stockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-06 08:47:00.000000 qfinuwa-1.1.9/src/qfinuwa/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:47:15.119421 qfinuwa-1.1.9/src/qfinuwa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-06 08:47:15.000000 qfinuwa-1.1.9/src/qfinuwa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-06 08:47:15.000000 qfinuwa-1.1.9/src/qfinuwa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:47:15.000000 qfinuwa-1.1.9/src/qfinuwa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-06 08:47:15.000000 qfinuwa-1.1.9/src/qfinuwa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 08:47:15.000000 qfinuwa-1.1.9/src/qfinuwa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.637391 qfinuwa-1.1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/src/qfinuwa/
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/backtester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/src/qfinuwa/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/opt/_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/opt/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/opt/_stockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/top_level.txt
```

### Comparing `qfinuwa-1.1.9/LICENSE.txt` & `qfinuwa-1.1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/PKG-INFO` & `qfinuwa-1.1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfinuwa
-Version: 1.1.9
+Version: 1.1.9.1
 Summary: Framework for backtesting quantitative trading algorithims.
 Home-page: https://github.com/QFinUWA/algo-backtester/issues
 Author: Isaac Bergl
 Author-email: tberg644@gmail.com
 Project-URL: Bug Tracker, https://github.com/QFinUWA/algo-backtester/issues
 Project-URL: repository, https://github.com/QFinUWA/algo-backtester
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qfinuwa-1.1.9/README.md` & `qfinuwa-1.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/setup.cfg` & `qfinuwa-1.1.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QFinUWA
-version = 1.1.9
+version = 1.1.9.1
 author = Isaac Bergl
 author_email = tberg644@gmail.com
 description = A backtesting framework for quantitative finance for QFIN UWA.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/QFinUWA/algo-backtester/issues
 project_urls =
```

### Comparing `qfinuwa-1.1.9/src/qfinuwa/API.py` & `qfinuwa-1.1.9.1/src/qfinuwa/API.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/src/qfinuwa/backtester.py` & `qfinuwa-1.1.9.1/src/qfinuwa/backtester.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/src/qfinuwa/indicators.py` & `qfinuwa-1.1.9.1/src/qfinuwa/indicators.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/src/qfinuwa/opt/_portfolio.py` & `qfinuwa-1.1.9.1/src/qfinuwa/opt/_portfolio.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
     #---------------[Public Methods]-----------------#
 
     def order(self, stock: str, quantity: Union[int, float]) -> bool:
         
         if abs(self._delta[stock] + quantity) > self._delta_limits[stock]:
             return False 
+        
+        if quantity == 0:
+            return False
 
         self._delta[stock] += quantity
         price = quantity*self._curr_prices[stock]
         self._fees_paid[stock] += abs(self._fee*price)
         self._capital[stock] -= price
         self._trades.append((self._i, stock, quantity))
         return True
```

### Comparing `qfinuwa-1.1.9/src/qfinuwa/opt/_result.py` & `qfinuwa-1.1.9.1/src/qfinuwa/opt/_result.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/src/qfinuwa/opt/_stockdata.py` & `qfinuwa-1.1.9.1/src/qfinuwa/opt/_stockdata.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/src/qfinuwa/plotting.py` & `qfinuwa-1.1.9.1/src/qfinuwa/plotting.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/src/qfinuwa/strategy.py` & `qfinuwa-1.1.9.1/src/qfinuwa/strategy.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9/src/qfinuwa.egg-info/PKG-INFO` & `qfinuwa-1.1.9.1/src/qfinuwa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfinuwa
-Version: 1.1.9
+Version: 1.1.9.1
 Summary: Framework for backtesting quantitative trading algorithims.
 Home-page: https://github.com/QFinUWA/algo-backtester/issues
 Author: Isaac Bergl
 Author-email: tberg644@gmail.com
 Project-URL: Bug Tracker, https://github.com/QFinUWA/algo-backtester/issues
 Project-URL: repository, https://github.com/QFinUWA/algo-backtester
 Classifier: Programming Language :: Python :: 3
```

