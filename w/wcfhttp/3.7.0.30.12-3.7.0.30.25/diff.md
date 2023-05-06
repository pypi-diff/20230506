# Comparing `tmp/wcfhttp-3.7.0.30.12.tar.gz` & `tmp/wcfhttp-3.7.0.30.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-3.7.0.30.12.tar", last modified: Sat May  6 13:08:57 2023, max compression
+gzip compressed data, was "wcfhttp-3.7.0.30.25.tar", last modified: Sat May  6 15:35:16 2023, max compression
```

## Comparing `wcfhttp-3.7.0.30.12.tar` & `wcfhttp-3.7.0.30.25.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 13:08:57.087969 wcfhttp-3.7.0.30.12/
--rw-r--r--   0 chuck      (501) staff       (20)       44 2023-05-05 15:29:35.000000 wcfhttp-3.7.0.30.12/MANIFEST.in
--rw-r--r--   0 chuck      (501) staff       (20)     1272 2023-05-06 13:08:57.087586 wcfhttp-3.7.0.30.12/PKG-INFO
--rw-r--r--   0 chuck      (501) staff       (20)       38 2023-05-06 13:08:57.088109 wcfhttp-3.7.0.30.12/setup.cfg
--rw-r--r--   0 chuck      (501) staff       (20)     1389 2023-05-06 07:14:27.000000 wcfhttp-3.7.0.30.12/setup.py
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 13:08:57.084234 wcfhttp-3.7.0.30.12/wcfhttp/
--rw-r--r--   0 chuck      (501) staff       (20)       67 2023-05-06 06:41:48.000000 wcfhttp-3.7.0.30.12/wcfhttp/__init__.py
--rw-r--r--   0 chuck      (501) staff       (20)     3439 2023-05-06 13:08:35.000000 wcfhttp-3.7.0.30.12/wcfhttp/core.py
--rw-r--r--   0 chuck      (501) staff       (20)     1740 2023-05-06 10:36:26.000000 wcfhttp-3.7.0.30.12/wcfhttp/main.py
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 13:08:57.087017 wcfhttp-3.7.0.30.12/wcfhttp.egg-info/
--rw-r--r--   0 chuck      (501) staff       (20)     1272 2023-05-06 13:08:57.000000 wcfhttp-3.7.0.30.12/wcfhttp.egg-info/PKG-INFO
--rw-r--r--   0 chuck      (501) staff       (20)      260 2023-05-06 13:08:57.000000 wcfhttp-3.7.0.30.12/wcfhttp.egg-info/SOURCES.txt
--rw-r--r--   0 chuck      (501) staff       (20)        1 2023-05-06 13:08:57.000000 wcfhttp-3.7.0.30.12/wcfhttp.egg-info/dependency_links.txt
--rw-r--r--   0 chuck      (501) staff       (20)       46 2023-05-06 13:08:57.000000 wcfhttp-3.7.0.30.12/wcfhttp.egg-info/entry_points.txt
--rw-r--r--   0 chuck      (501) staff       (20)       58 2023-05-06 13:08:57.000000 wcfhttp-3.7.0.30.12/wcfhttp.egg-info/requires.txt
--rw-r--r--   0 chuck      (501) staff       (20)        8 2023-05-06 13:08:57.000000 wcfhttp-3.7.0.30.12/wcfhttp.egg-info/top_level.txt
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 15:35:16.112958 wcfhttp-3.7.0.30.25/
+-rw-r--r--   0 chuck      (501) staff       (20)       44 2023-05-05 15:29:35.000000 wcfhttp-3.7.0.30.25/MANIFEST.in
+-rw-r--r--   0 chuck      (501) staff       (20)     1290 2023-05-06 15:35:16.112553 wcfhttp-3.7.0.30.25/PKG-INFO
+-rw-r--r--   0 chuck      (501) staff       (20)       38 2023-05-06 15:35:16.113096 wcfhttp-3.7.0.30.25/setup.cfg
+-rw-r--r--   0 chuck      (501) staff       (20)     1389 2023-05-06 07:14:27.000000 wcfhttp-3.7.0.30.25/setup.py
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 15:35:16.108041 wcfhttp-3.7.0.30.25/wcfhttp/
+-rw-r--r--   0 chuck      (501) staff       (20)       67 2023-05-06 06:41:48.000000 wcfhttp-3.7.0.30.25/wcfhttp/__init__.py
+-rw-r--r--   0 chuck      (501) staff       (20)    11045 2023-05-06 15:09:26.000000 wcfhttp-3.7.0.30.25/wcfhttp/core.py
+-rw-r--r--   0 chuck      (501) staff       (20)     1740 2023-05-06 10:36:26.000000 wcfhttp-3.7.0.30.25/wcfhttp/main.py
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 15:35:16.111999 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/
+-rw-r--r--   0 chuck      (501) staff       (20)     1290 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/PKG-INFO
+-rw-r--r--   0 chuck      (501) staff       (20)      260 2023-05-06 15:35:16.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/SOURCES.txt
+-rw-r--r--   0 chuck      (501) staff       (20)        1 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/dependency_links.txt
+-rw-r--r--   0 chuck      (501) staff       (20)       46 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/entry_points.txt
+-rw-r--r--   0 chuck      (501) staff       (20)       58 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/requires.txt
+-rw-r--r--   0 chuck      (501) staff       (20)        8 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-3.7.0.30.12/PKG-INFO` & `wcfhttp-3.7.0.30.25/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 3.7.0.30.12
+Version: 3.7.0.30.25
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WeChatFerry HTTP 客户端
 [![PyPi](https://img.shields.io/pypi/v/wcfhttp.svg)](https://pypi.python.org/pypi/wcfhttp)
 
-基于 [wcferry](https://pypi.org/project/wcferry/) 封装。
+基于 [wcferry](https://pypi.org/project/wcferry/) 封装的 HTTP 客户端。
 
 ## 快速开始
 ### 安装
 ```sh
 pip install --upgrade wcfhttp
 ```
```

### Comparing `wcfhttp-3.7.0.30.12/setup.py` & `wcfhttp-3.7.0.30.25/setup.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-3.7.0.30.12/wcfhttp/main.py` & `wcfhttp-3.7.0.30.25/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-3.7.0.30.12/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-3.7.0.30.25/wcfhttp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 3.7.0.30.12
+Version: 3.7.0.30.25
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WeChatFerry HTTP 客户端
 [![PyPi](https://img.shields.io/pypi/v/wcfhttp.svg)](https://pypi.python.org/pypi/wcfhttp)
 
-基于 [wcferry](https://pypi.org/project/wcferry/) 封装。
+基于 [wcferry](https://pypi.org/project/wcferry/) 封装的 HTTP 客户端。
 
 ## 快速开始
 ### 安装
 ```sh
 pip install --upgrade wcfhttp
 ```
```

