# Comparing `tmp/wcfhttp-3.7.0.30.0.tar.gz` & `tmp/wcfhttp-3.7.0.30.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-3.7.0.30.0.tar", last modified: Sat May  6 12:56:19 2023, max compression
+gzip compressed data, was "wcfhttp-3.7.0.30.11.tar", last modified: Sat May  6 13:06:04 2023, max compression
```

## Comparing `wcfhttp-3.7.0.30.0.tar` & `wcfhttp-3.7.0.30.11.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 12:56:19.460453 wcfhttp-3.7.0.30.0/
--rw-r--r--   0 chuck      (501) staff       (20)       44 2023-05-05 15:29:35.000000 wcfhttp-3.7.0.30.0/MANIFEST.in
--rw-r--r--   0 chuck      (501) staff       (20)     1517 2023-05-06 12:56:19.460055 wcfhttp-3.7.0.30.0/PKG-INFO
--rw-r--r--   0 chuck      (501) staff       (20)       38 2023-05-06 12:56:19.460597 wcfhttp-3.7.0.30.0/setup.cfg
--rw-r--r--   0 chuck      (501) staff       (20)     1389 2023-05-06 07:14:27.000000 wcfhttp-3.7.0.30.0/setup.py
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 12:56:19.456479 wcfhttp-3.7.0.30.0/wcfhttp/
--rw-r--r--   0 chuck      (501) staff       (20)       67 2023-05-06 06:41:48.000000 wcfhttp-3.7.0.30.0/wcfhttp/__init__.py
--rw-r--r--   0 chuck      (501) staff       (20)     3438 2023-05-06 12:56:11.000000 wcfhttp-3.7.0.30.0/wcfhttp/core.py
--rw-r--r--   0 chuck      (501) staff       (20)     1740 2023-05-06 10:36:26.000000 wcfhttp-3.7.0.30.0/wcfhttp/main.py
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 12:56:19.459491 wcfhttp-3.7.0.30.0/wcfhttp.egg-info/
--rw-r--r--   0 chuck      (501) staff       (20)     1517 2023-05-06 12:56:19.000000 wcfhttp-3.7.0.30.0/wcfhttp.egg-info/PKG-INFO
--rw-r--r--   0 chuck      (501) staff       (20)      260 2023-05-06 12:56:19.000000 wcfhttp-3.7.0.30.0/wcfhttp.egg-info/SOURCES.txt
--rw-r--r--   0 chuck      (501) staff       (20)        1 2023-05-06 12:56:19.000000 wcfhttp-3.7.0.30.0/wcfhttp.egg-info/dependency_links.txt
--rw-r--r--   0 chuck      (501) staff       (20)       46 2023-05-06 12:56:19.000000 wcfhttp-3.7.0.30.0/wcfhttp.egg-info/entry_points.txt
--rw-r--r--   0 chuck      (501) staff       (20)       57 2023-05-06 12:56:19.000000 wcfhttp-3.7.0.30.0/wcfhttp.egg-info/requires.txt
--rw-r--r--   0 chuck      (501) staff       (20)        8 2023-05-06 12:56:19.000000 wcfhttp-3.7.0.30.0/wcfhttp.egg-info/top_level.txt
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 13:06:04.358344 wcfhttp-3.7.0.30.11/
+-rw-r--r--   0 chuck      (501) staff       (20)       44 2023-05-05 15:29:35.000000 wcfhttp-3.7.0.30.11/MANIFEST.in
+-rw-r--r--   0 chuck      (501) staff       (20)     1364 2023-05-06 13:06:04.357941 wcfhttp-3.7.0.30.11/PKG-INFO
+-rw-r--r--   0 chuck      (501) staff       (20)       38 2023-05-06 13:06:04.358484 wcfhttp-3.7.0.30.11/setup.cfg
+-rw-r--r--   0 chuck      (501) staff       (20)     1389 2023-05-06 07:14:27.000000 wcfhttp-3.7.0.30.11/setup.py
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 13:06:04.353831 wcfhttp-3.7.0.30.11/wcfhttp/
+-rw-r--r--   0 chuck      (501) staff       (20)       67 2023-05-06 06:41:48.000000 wcfhttp-3.7.0.30.11/wcfhttp/__init__.py
+-rw-r--r--   0 chuck      (501) staff       (20)     3439 2023-05-06 13:05:57.000000 wcfhttp-3.7.0.30.11/wcfhttp/core.py
+-rw-r--r--   0 chuck      (501) staff       (20)     1740 2023-05-06 10:36:26.000000 wcfhttp-3.7.0.30.11/wcfhttp/main.py
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 13:06:04.357268 wcfhttp-3.7.0.30.11/wcfhttp.egg-info/
+-rw-r--r--   0 chuck      (501) staff       (20)     1364 2023-05-06 13:06:04.000000 wcfhttp-3.7.0.30.11/wcfhttp.egg-info/PKG-INFO
+-rw-r--r--   0 chuck      (501) staff       (20)      260 2023-05-06 13:06:04.000000 wcfhttp-3.7.0.30.11/wcfhttp.egg-info/SOURCES.txt
+-rw-r--r--   0 chuck      (501) staff       (20)        1 2023-05-06 13:06:04.000000 wcfhttp-3.7.0.30.11/wcfhttp.egg-info/dependency_links.txt
+-rw-r--r--   0 chuck      (501) staff       (20)       46 2023-05-06 13:06:04.000000 wcfhttp-3.7.0.30.11/wcfhttp.egg-info/entry_points.txt
+-rw-r--r--   0 chuck      (501) staff       (20)       58 2023-05-06 13:06:04.000000 wcfhttp-3.7.0.30.11/wcfhttp.egg-info/requires.txt
+-rw-r--r--   0 chuck      (501) staff       (20)        8 2023-05-06 13:06:04.000000 wcfhttp-3.7.0.30.11/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-3.7.0.30.0/PKG-INFO` & `wcfhttp-3.7.0.30.11/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 3.7.0.30.0
+Version: 3.7.0.30.11
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -14,15 +14,15 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WeChatFerry HTTP 客户端
-[![PyPi](https://img.shields.io/pypi/v/wcferry.svg)](https://pypi.python.org/pypi/wcferry) [![Downloads](https://static.pepy.tech/badge/wcferry)](https://pypi.python.org/pypi/wcferry) [![Documentation Status](https://readthedocs.org/projects/wechatferry/badge/?version=latest)](https://wechatferry.readthedocs.io/zh/latest/?badge=latest)
+[![PyPi](https://img.shields.io/pypi/v/wcfhttp.svg)](https://pypi.python.org/pypi/wcfhttp) [![Downloads](https://static.pepy.tech/badge/wcfhttp)](https://pypi.python.org/pypi/wcfhttp)
 
 基于 [wcferry](https://pypi.org/project/wcferry/) 封装。
 
 ## 快速开始
 ### 安装
 ```sh
 pip install --upgrade wcfhttp
```

### Comparing `wcfhttp-3.7.0.30.0/setup.py` & `wcfhttp-3.7.0.30.11/setup.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-3.7.0.30.0/wcfhttp/core.py` & `wcfhttp-3.7.0.30.11/wcfhttp/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any
 
 import requests
 from fastapi import Body, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "3.7.0.30.0"
+__version__ = "3.7.0.30.11"
 
 
 class Msg(BaseModel):
     id: str
     type: int
     xml: str
     sender: str
```

### Comparing `wcfhttp-3.7.0.30.0/wcfhttp/main.py` & `wcfhttp-3.7.0.30.11/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-3.7.0.30.0/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-3.7.0.30.11/wcfhttp.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 3.7.0.30.0
+Version: 3.7.0.30.11
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -14,15 +14,15 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WeChatFerry HTTP 客户端
-[![PyPi](https://img.shields.io/pypi/v/wcferry.svg)](https://pypi.python.org/pypi/wcferry) [![Downloads](https://static.pepy.tech/badge/wcferry)](https://pypi.python.org/pypi/wcferry) [![Documentation Status](https://readthedocs.org/projects/wechatferry/badge/?version=latest)](https://wechatferry.readthedocs.io/zh/latest/?badge=latest)
+[![PyPi](https://img.shields.io/pypi/v/wcfhttp.svg)](https://pypi.python.org/pypi/wcfhttp) [![Downloads](https://static.pepy.tech/badge/wcfhttp)](https://pypi.python.org/pypi/wcfhttp)
 
 基于 [wcferry](https://pypi.org/project/wcferry/) 封装。
 
 ## 快速开始
 ### 安装
 ```sh
 pip install --upgrade wcfhttp
```

