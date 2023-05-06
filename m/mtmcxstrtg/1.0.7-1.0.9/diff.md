# Comparing `tmp/mtmcxstrtg-1.0.7.tar.gz` & `tmp/mtmcxstrtg-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmcxstrtg-1.0.7.tar", last modified: Tue May  2 14:14:11 2023, max compression
+gzip compressed data, was "mtmcxstrtg-1.0.9.tar", last modified: Sat May  6 03:35:06 2023, max compression
```

## Comparing `mtmcxstrtg-1.0.7.tar` & `mtmcxstrtg-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:14:11.357772 mtmcxstrtg-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-02 14:14:11.357772 mtmcxstrtg-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:14:11.357772 mtmcxstrtg-1.0.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/scripts/run.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 14:14:11.357772 mtmcxstrtg-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:14:11.353772 mtmcxstrtg-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:14:11.357772 mtmcxstrtg-1.0.7/src/mtmcxstrtg/
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:14:11.357772 mtmcxstrtg-1.0.7/src/mtmcxstrtg/strategy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-05-02 14:14:03.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 14:14:11.357772 mtmcxstrtg-1.0.7/src/mtmcxstrtg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-02 14:14:11.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-05-02 14:14:11.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 14:14:11.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 14:14:11.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-02 14:14:11.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-02 14:14:11.000000 mtmcxstrtg-1.0.7/src/mtmcxstrtg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 03:35:06.421004 mtmcxstrtg-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-06 03:35:06.421004 mtmcxstrtg-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 03:35:06.417004 mtmcxstrtg-1.0.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/scripts/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-06 03:35:06.421004 mtmcxstrtg-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 03:35:06.417004 mtmcxstrtg-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 03:35:06.421004 mtmcxstrtg-1.0.9/src/mtmcxstrtg/
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 03:35:06.421004 mtmcxstrtg-1.0.9/src/mtmcxstrtg/strategy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-05-06 03:34:56.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 03:35:06.421004 mtmcxstrtg-1.0.9/src/mtmcxstrtg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-06 03:35:06.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-05-06 03:35:06.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 03:35:06.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 03:35:06.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-06 03:35:06.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-06 03:35:06.000000 mtmcxstrtg-1.0.9/src/mtmcxstrtg.egg-info/top_level.txt
```

### Comparing `mtmcxstrtg-1.0.7/PKG-INFO` & `mtmcxstrtg-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmcxstrtg
-Version: 1.0.7
+Version: 1.0.9
 Summary: imutum_cryptocurrency_strategy
 Home-page: https://github.com/imutum/imutum_cryptocurrency_strategy
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmcxstrtg-1.0.7/scripts/run.py` & `mtmcxstrtg-1.0.9/scripts/run.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.7/setup.py` & `mtmcxstrtg-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = "imutum_cryptocurrency_strategy"
 abbreviation_name = "mtmcxstrtg"  # 缩写
 description = ""
-version = "1.0.7"
+version = "1.0.9"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
```

### Comparing `mtmcxstrtg-1.0.7/src/mtmcxstrtg/account.py` & `mtmcxstrtg-1.0.9/src/mtmcxstrtg/account.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.7/src/mtmcxstrtg/flow.py` & `mtmcxstrtg-1.0.9/src/mtmcxstrtg/flow.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.7/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py` & `mtmcxstrtg-1.0.9/src/mtmcxstrtg/strategy/cta_deviation_signal_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,8 +79,8 @@
     # 保存amount dict, 记录了本次交易的信息
     # 如果本次交易没有平仓，那么保留上次的交易价格
     next_price = last_price if (envs["quote_coins"] * next_quantity > 0) else envs["price_current"]
     write_amount(amount_path, {"quantity": next_quantity, "price": next_price, "asset": next_amount})
 
 
 if __name__ == '__main__':
-    main_func("cta_.yaml")
+    main_func("test.yaml")
```

### Comparing `mtmcxstrtg-1.0.7/src/mtmcxstrtg/util.py` & `mtmcxstrtg-1.0.9/src/mtmcxstrtg/util.py`

 * *Files identical despite different names*

### Comparing `mtmcxstrtg-1.0.7/src/mtmcxstrtg.egg-info/PKG-INFO` & `mtmcxstrtg-1.0.9/src/mtmcxstrtg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmcxstrtg
-Version: 1.0.7
+Version: 1.0.9
 Summary: imutum_cryptocurrency_strategy
 Home-page: https://github.com/imutum/imutum_cryptocurrency_strategy
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

