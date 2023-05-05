# Comparing `tmp/lib-pybroker-1.1.7.tar.gz` & `tmp/lib-pybroker-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-pybroker-1.1.7.tar", last modified: Mon May  1 20:41:31 2023, max compression
+gzip compressed data, was "lib-pybroker-1.1.8.tar", last modified: Fri May  5 23:09:48 2023, max compression
```

## Comparing `lib-pybroker-1.1.7.tar` & `lib-pybroker-1.1.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.981930 lib-pybroker-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-01 20:41:31.981930 lib-pybroker-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-01 20:41:31.981930 lib-pybroker-1.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.973930 lib-pybroker-1.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.973930 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.977930 lib-pybroker-1.1.7/src/pybroker/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    58375 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/vect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.981930 lib-pybroker-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    76914 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.595905 lib-pybroker-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-05 23:09:48.595905 lib-pybroker-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-05 23:09:48.595905 lib-pybroker-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.583904 lib-pybroker-1.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.587904 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 23:09:48.000000 lib-pybroker-1.1.8/src/lib_pybroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.591904 lib-pybroker-1.1.8/src/pybroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58375 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/src/pybroker/vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:09:48.595905 lib-pybroker-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76914 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-05 23:09:37.000000 lib-pybroker-1.1.8/tests/test_vect.py
```

### Comparing `lib-pybroker-1.1.7/LICENSE` & `lib-pybroker-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/PKG-INFO` & `lib-pybroker-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.7
+Version: 1.1.8
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.7/README.md` & `lib-pybroker-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/setup.cfg` & `lib-pybroker-1.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/lib_pybroker.egg-info/PKG-INFO` & `lib-pybroker-1.1.8/src/lib_pybroker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.7
+Version: 1.1.8
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.7/src/lib_pybroker.egg-info/SOURCES.txt` & `lib-pybroker-1.1.8/src/lib_pybroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/__init__.py` & `lib-pybroker-1.1.8/src/pybroker/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,8 +43,12 @@
     param,
     register_columns,
     unregister_columns,
 )
 from .strategy import Strategy, TestResult
 from .vect import cross, highv, lowv, sumv
 
-__version__ = "1.1.7"
+# Temporary fix for regression in Numba 0.57.0
+# https://github.com/numba/numba/issues/8940
+from numba.np.unsafe import ndarray
+
+__version__ = "1.1.8"
```

### Comparing `lib-pybroker-1.1.7/src/pybroker/cache.py` & `lib-pybroker-1.1.8/src/pybroker/cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/common.py` & `lib-pybroker-1.1.8/src/pybroker/common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/config.py` & `lib-pybroker-1.1.8/src/pybroker/config.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/context.py` & `lib-pybroker-1.1.8/src/pybroker/context.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/data.py` & `lib-pybroker-1.1.8/src/pybroker/data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/eval.py` & `lib-pybroker-1.1.8/src/pybroker/eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/indicator.py` & `lib-pybroker-1.1.8/src/pybroker/indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/log.py` & `lib-pybroker-1.1.8/src/pybroker/log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/model.py` & `lib-pybroker-1.1.8/src/pybroker/model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/portfolio.py` & `lib-pybroker-1.1.8/src/pybroker/portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/scope.py` & `lib-pybroker-1.1.8/src/pybroker/scope.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/strategy.py` & `lib-pybroker-1.1.8/src/pybroker/strategy.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/src/pybroker/vect.py` & `lib-pybroker-1.1.8/src/pybroker/vect.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_cache.py` & `lib-pybroker-1.1.8/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_common.py` & `lib-pybroker-1.1.8/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_context.py` & `lib-pybroker-1.1.8/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_data.py` & `lib-pybroker-1.1.8/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_eval.py` & `lib-pybroker-1.1.8/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_indicator.py` & `lib-pybroker-1.1.8/tests/test_indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_log.py` & `lib-pybroker-1.1.8/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_model.py` & `lib-pybroker-1.1.8/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_portfolio.py` & `lib-pybroker-1.1.8/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_scope.py` & `lib-pybroker-1.1.8/tests/test_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,31 +405,32 @@
                 "predict function. Please pass a predict_fn to "
                 "pybroker.model()."
             ),
         ):
             pred_scope.fetch("SPY", MODEL_NAME)
 
     def test_fetch_when_input_data_empty_then_error(self, col_scope):
+        model_name = "no_input_data"
         ind_scope = IndicatorScope({}, [])
         input_scope = ModelInputScope(col_scope, ind_scope)
-        pybroker.model(MODEL_NAME, lambda sym, train, test: {})
-        model = TrainedModel(name=MODEL_NAME, instance={}, predict_fn=None)
+        pybroker.model(model_name, lambda sym, train, test: {})
+        model = TrainedModel(name=model_name, instance={}, predict_fn=None)
         pred_scope = PredictionScope(
-            models={ModelSymbol(MODEL_NAME, "SPY"): model},
+            models={ModelSymbol(model_name, "SPY"): model},
             input_scope=input_scope,
         )
         with pytest.raises(
             ValueError,
             match=re.escape(
-                f"No input data found for model {MODEL_NAME!r}. Consider "
+                f"No input data found for model {model_name!r}. Consider "
                 "passing input_data_fn to pybroker#model() if custom columns "
                 "were registered."
             ),
         ):
-            pred_scope.fetch("SPY", MODEL_NAME)
+            pred_scope.fetch("SPY", model_name)
 
 
 class TestPriceScope:
     @pytest.mark.parametrize(
         "price, expected_price",
         [
             (50, 50),
```

### Comparing `lib-pybroker-1.1.7/tests/test_strategy.py` & `lib-pybroker-1.1.8/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.7/tests/test_vect.py` & `lib-pybroker-1.1.8/tests/test_vect.py`

 * *Files identical despite different names*

