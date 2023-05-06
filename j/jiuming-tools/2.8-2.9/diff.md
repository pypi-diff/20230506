# Comparing `tmp/jiuming-tools-2.8.tar.gz` & `tmp/jiuming-tools-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiuming-tools-2.8.tar", last modified: Mon Jan 17 05:58:18 2022, max compression
+gzip compressed data, was "jiuming-tools-2.9.tar", last modified: Mon Jan 17 06:04:06 2022, max compression
```

## Comparing `jiuming-tools-2.8.tar` & `jiuming-tools-2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.317750 jiuming-tools-2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-17 05:58:18.317750 jiuming-tools-2.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     1606 2022-01-17 05:56:15.000000 jiuming-tools-2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.313750 jiuming-tools-2.8/jiuming_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-17 05:58:18.000000 jiuming-tools-2.8/jiuming_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-01-17 05:58:18.000000 jiuming-tools-2.8/jiuming_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-17 05:58:18.000000 jiuming-tools-2.8/jiuming_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-17 05:58:18.000000 jiuming-tools-2.8/jiuming_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-17 05:58:18.000000 jiuming-tools-2.8/jiuming_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-01-17 05:58:18.000000 jiuming-tools-2.8/jiuming_tools.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-01-17 05:56:15.000000 jiuming-tools-2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-17 05:58:18.317750 jiuming-tools-2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      879 2022-01-17 05:56:15.000000 jiuming-tools-2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.313750 jiuming-tools-2.8/src/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.313750 jiuming-tools-2.8/src/cmd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/cmd/cmd_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.313750 jiuming-tools-2.8/src/config/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/config/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4486 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/config/config_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2102 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/config/global_config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/config/server_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.313750 jiuming-tools-2.8/src/local/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/local/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3136 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/local/http_server.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1525 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/local/net_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4324 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/local/pc_info.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2207 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/local/pc_test.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12293 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/ming.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.313750 jiuming-tools-2.8/src/script/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/script/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4940 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/script/script_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/script/script_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.313750 jiuming-tools-2.8/src/server/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/server/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10208 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/server/server_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/server/server_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:58:18.317750 jiuming-tools-2.8/src/utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      235 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/utils/iputils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      571 2022-01-17 05:56:15.000000 jiuming-tools-2.8/src/utils/timeUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-17 06:04:06.487512 jiuming-tools-2.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1606 2022-01-17 06:02:36.000000 jiuming-tools-2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/jiuming_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-17 06:04:06.000000 jiuming-tools-2.9/jiuming_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-01-17 06:04:06.000000 jiuming-tools-2.9/jiuming_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-17 06:04:06.000000 jiuming-tools-2.9/jiuming_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-17 06:04:06.000000 jiuming-tools-2.9/jiuming_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-17 06:04:06.000000 jiuming-tools-2.9/jiuming_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-01-17 06:04:06.000000 jiuming-tools-2.9/jiuming_tools.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-01-17 06:02:36.000000 jiuming-tools-2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-17 06:04:06.487512 jiuming-tools-2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      879 2022-01-17 06:02:36.000000 jiuming-tools-2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/src/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/src/cmd/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/cmd/cmd_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/src/config/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/config/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4486 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/config/config_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2102 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/config/global_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/config/server_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/src/local/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/local/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3136 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/local/http_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1525 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/local/net_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4324 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/local/pc_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2207 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/local/pc_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12293 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/ming.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/src/script/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/script/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4940 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/script/script_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/script/script_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/src/server/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/server/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10208 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/server/server_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/server/server_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:04:06.487512 jiuming-tools-2.9/src/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      235 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/utils/iputils.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      571 2022-01-17 06:02:36.000000 jiuming-tools-2.9/src/utils/timeUtils.py
```

### Comparing `jiuming-tools-2.8/README.md` & `jiuming-tools-2.9/README.md`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/jiuming_tools.egg-info/SOURCES.txt` & `jiuming-tools-2.9/jiuming_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/setup.py` & `jiuming-tools-2.9/setup.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/cmd/cmd_manager.py` & `jiuming-tools-2.9/src/cmd/cmd_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import click
 from lxml import etree
 from requests_cache import CachedSession
 
 def search(name):
+    # 处理空格
+    name = name.strip()
     # 增加缓存处理
     session = CachedSession('jiuming-tools_http_cache', backend='filesystem', use_cache_dir=True)
     response = session.get("http://linux.51yip.com/search/{}".format(name))
     response.encoding = 'utf-8'
     if response.status_code != 200:
         click.echo(response.text)  # 以文本形式打印网页源码
         if response.status_code == 404:
```

### Comparing `jiuming-tools-2.8/src/config/config_manager.py` & `jiuming-tools-2.9/src/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/config/global_config.py` & `jiuming-tools-2.9/src/config/global_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 
 # 版本号  setup.py  ming.py 引用  每次发布 版本+1
-ming_global_version = 2.8
+ming_global_version = 2.9
 
 
 def getVersion():
     return ming_global_version
 
 
 class ToolsDependency:
```

### Comparing `jiuming-tools-2.8/src/local/http_server.py` & `jiuming-tools-2.9/src/local/http_server.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/local/net_manager.py` & `jiuming-tools-2.9/src/local/net_manager.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/local/pc_info.py` & `jiuming-tools-2.9/src/local/pc_info.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/local/pc_test.py` & `jiuming-tools-2.9/src/local/pc_test.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/ming.py` & `jiuming-tools-2.9/src/ming.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/script/script_manager.py` & `jiuming-tools-2.9/src/script/script_manager.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/script/script_store.py` & `jiuming-tools-2.9/src/script/script_store.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/server/server_config.py` & `jiuming-tools-2.9/src/server/server_config.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/server/server_store.py` & `jiuming-tools-2.9/src/server/server_store.py`

 * *Files identical despite different names*

### Comparing `jiuming-tools-2.8/src/utils/timeUtils.py` & `jiuming-tools-2.9/src/utils/timeUtils.py`

 * *Files identical despite different names*

