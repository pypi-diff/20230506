# Comparing `tmp/yang-vlp-0.2.15.tar.gz` & `tmp/yang-vlp-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-45krm8_0\yang-vlp-0.2.15.tar", last modified: Fri May  5 07:56:18 2023, max compression
+gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-_qcwp4vf\yang-vlp-0.2.16.tar", last modified: Sat May  6 06:41:29 2023, max compression
```

## Comparing `yang-vlp-0.2.15.tar` & `yang-vlp-0.2.16.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.390613 yang-vlp-0.2.15/
--rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.15/LICENSE
--rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.15/MANIFEST.in
--rw-rw-rw-   0        0        0     2687 2023-05-05 07:56:18.388587 yang-vlp-0.2.15/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-04-27 01:00:56.000000 yang-vlp-0.2.15/README.md
--rw-rw-rw-   0        0        0      639 2023-05-05 07:26:56.000000 yang-vlp-0.2.15/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 07:56:18.391591 yang-vlp-0.2.15/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-05 07:27:01.000000 yang-vlp-0.2.15/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.170583 yang-vlp-0.2.15/vlppy/
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.175588 yang-vlp-0.2.15/vlppy/.vscode/
--rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.15/vlppy/.vscode/settings.json
--rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.15/vlppy/LICENSE.txt
--rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.15/vlppy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.192587 yang-vlp-0.2.15/vlppy/demo/
--rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.15/vlppy/demo/README.md
--rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.15/vlppy/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.208582 yang-vlp-0.2.15/vlppy/demo/__pycache__/
--rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.15/vlppy/demo/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.15/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
--rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.15/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
--rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.15/vlppy/demo/demo_filter.py
--rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.15/vlppy/demo/demo_main.py
--rw-rw-rw-   0        0        0     3188 2023-05-05 07:55:54.000000 yang-vlp-0.2.15/vlppy/demo/vlp_model.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.226582 yang-vlp-0.2.15/vlppy/error/
--rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.15/vlppy/error/__init__.py
--rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.15/vlppy/error/error.py
--rw-rw-rw-   0        0        0      110 2023-05-05 07:27:09.000000 yang-vlp-0.2.15/vlppy/info.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.231585 yang-vlp-0.2.15/vlppy/io/
--rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.15/vlppy/io/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.15/vlppy/io/io.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.243619 yang-vlp-0.2.15/vlppy/model/
--rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.15/vlppy/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.285583 yang-vlp-0.2.15/vlppy/model/__pycache__/
--rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/filter.cpython-39.pyc
--rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/led.cpython-39.pyc
--rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/pd.cpython-39.pyc
--rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/room.cpython-39.pyc
--rw-rw-rw-   0        0        0     6154 2023-05-05 07:26:43.000000 yang-vlp-0.2.15/vlppy/model/led.py
--rw-rw-rw-   0        0        0    17952 2023-05-05 07:54:41.000000 yang-vlp-0.2.15/vlppy/model/pd.py
--rw-rw-rw-   0        0        0    17803 2023-05-05 07:23:46.000000 yang-vlp-0.2.15/vlppy/model/room.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.305587 yang-vlp-0.2.15/vlppy/setting/
--rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.15/vlppy/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.319585 yang-vlp-0.2.15/vlppy/setting/__pycache__/
--rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.15/vlppy/setting/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.15/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
--rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.15/vlppy/setting/json_setting.py
--rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.15/vlppy/setting/settings.json
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.357618 yang-vlp-0.2.15/vlppy/signal/
--rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.15/vlppy/signal/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.15/vlppy/signal/filter.py
--rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.15/vlppy/signal/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.362586 yang-vlp-0.2.15/vlppy/tools/
--rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.15/vlppy/tools/__init__.py
--rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.15/vlppy/tools/decorator.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.368592 yang-vlp-0.2.15/vlppy/vis/
--rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.15/vlppy/vis/__init__.py
--rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.15/vlppy/vis/vis.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.385586 yang-vlp-0.2.15/yang_vlp.egg-info/
--rw-rw-rw-   0        0        0     2687 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.508913 yang-vlp-0.2.16/
+-rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.16/LICENSE
+-rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.16/MANIFEST.in
+-rw-rw-rw-   0        0        0     2687 2023-05-06 06:41:29.507950 yang-vlp-0.2.16/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-04-27 01:00:56.000000 yang-vlp-0.2.16/README.md
+-rw-rw-rw-   0        0        0      639 2023-05-06 06:39:43.000000 yang-vlp-0.2.16/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 06:41:29.509917 yang-vlp-0.2.16/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-06 06:39:38.000000 yang-vlp-0.2.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.332920 yang-vlp-0.2.16/vlppy/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.334911 yang-vlp-0.2.16/vlppy/.vscode/
+-rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.16/vlppy/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.16/vlppy/LICENSE.txt
+-rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.16/vlppy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.349956 yang-vlp-0.2.16/vlppy/demo/
+-rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.16/vlppy/demo/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.16/vlppy/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.356913 yang-vlp-0.2.16/vlppy/demo/__pycache__/
+-rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.16/vlppy/demo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.16/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.16/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.16/vlppy/demo/demo_filter.py
+-rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.16/vlppy/demo/demo_main.py
+-rw-rw-rw-   0        0        0     3188 2023-05-05 07:55:54.000000 yang-vlp-0.2.16/vlppy/demo/vlp_model.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.363916 yang-vlp-0.2.16/vlppy/error/
+-rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.16/vlppy/error/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.16/vlppy/error/error.py
+-rw-rw-rw-   0        0        0      108 2023-05-06 06:40:05.000000 yang-vlp-0.2.16/vlppy/info.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.369947 yang-vlp-0.2.16/vlppy/io/
+-rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.16/vlppy/io/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.16/vlppy/io/io.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.381941 yang-vlp-0.2.16/vlppy/model/
+-rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.16/vlppy/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.424914 yang-vlp-0.2.16/vlppy/model/__pycache__/
+-rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/filter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/led.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/pd.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.16/vlppy/model/__pycache__/room.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6154 2023-05-05 07:26:43.000000 yang-vlp-0.2.16/vlppy/model/led.py
+-rw-rw-rw-   0        0        0    17943 2023-05-05 10:56:03.000000 yang-vlp-0.2.16/vlppy/model/pd.py
+-rw-rw-rw-   0        0        0    17682 2023-05-06 06:38:15.000000 yang-vlp-0.2.16/vlppy/model/room.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.435915 yang-vlp-0.2.16/vlppy/setting/
+-rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.16/vlppy/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.441914 yang-vlp-0.2.16/vlppy/setting/__pycache__/
+-rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.16/vlppy/setting/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.16/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.16/vlppy/setting/json_setting.py
+-rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.16/vlppy/setting/settings.json
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.453929 yang-vlp-0.2.16/vlppy/signal/
+-rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.16/vlppy/signal/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.16/vlppy/signal/filter.py
+-rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.16/vlppy/signal/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.485913 yang-vlp-0.2.16/vlppy/tools/
+-rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.16/vlppy/tools/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.16/vlppy/tools/decorator.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.489941 yang-vlp-0.2.16/vlppy/vis/
+-rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.16/vlppy/vis/__init__.py
+-rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.16/vlppy/vis/vis.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:41:29.505948 yang-vlp-0.2.16/yang_vlp.egg-info/
+-rw-rw-rw-   0        0        0     2687 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 06:41:29.000000 yang-vlp-0.2.16/yang_vlp.egg-info/top_level.txt
```

### Comparing `yang-vlp-0.2.15/LICENSE` & `yang-vlp-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/PKG-INFO` & `yang-vlp-0.2.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.15
+Version: 0.2.16
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `yang-vlp-0.2.15/README.md` & `yang-vlp-0.2.16/README.md`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/pyproject.toml` & `yang-vlp-0.2.16/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yang-vlp"
-version = "0.2.15"
+version = "0.2.16"
 authors = [
   { name="yangwuju", email="1424134319@qq.com" },
 ]
 description = "Construction of visible light positioning model"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `yang-vlp-0.2.15/setup.py` & `yang-vlp-0.2.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = os.path.join(CUR_PATH, 'build')
 if os.path.isdir(path):
     print('INFO del dir ', path) 
     shutil.rmtree(path)
 
 setup(
     name = 'yang-vlp', #应用名
-    version = '0.2.15',  #版本号
+    version = '0.2.16',  #版本号
     description = 'Construction of visible light positioning model', 
     packages = find_packages(),  #包括在安装包内的Python包
     include_package_data = True, #启用清单文件MANIFEST.in,包含数据文件
     # exclude_package_data = {'docs':['1.txt']},  #排除文件
     install_requires = [#自动安装依赖
         'numpy>=1.19.0',
         'matplotlib>=3.5.0',
```

### Comparing `yang-vlp-0.2.15/vlppy/LICENSE.txt` & `yang-vlp-0.2.16/vlppy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/demo/__pycache__/demo_main.cpython-39.pyc` & `yang-vlp-0.2.16/vlppy/demo/__pycache__/demo_main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc` & `yang-vlp-0.2.16/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/demo/demo_filter.py` & `yang-vlp-0.2.16/vlppy/demo/demo_filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/demo/demo_main.py` & `yang-vlp-0.2.16/vlppy/demo/demo_main.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/demo/vlp_model.py` & `yang-vlp-0.2.16/vlppy/demo/vlp_model.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/error/error.py` & `yang-vlp-0.2.16/vlppy/error/error.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/io/io.py` & `yang-vlp-0.2.16/vlppy/io/io.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/model/__pycache__/filter.cpython-39.pyc` & `yang-vlp-0.2.16/vlppy/model/__pycache__/filter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/model/__pycache__/led.cpython-39.pyc` & `yang-vlp-0.2.16/vlppy/model/__pycache__/led.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/model/__pycache__/pd.cpython-39.pyc` & `yang-vlp-0.2.16/vlppy/model/__pycache__/pd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/model/__pycache__/room.cpython-39.pyc` & `yang-vlp-0.2.16/vlppy/model/__pycache__/room.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/model/led.py` & `yang-vlp-0.2.16/vlppy/model/led.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/model/pd.py` & `yang-vlp-0.2.16/vlppy/model/pd.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,43 +186,43 @@
         """
         # 对PD坐标张量扩充维度,以便使用广播
         pd_pos = np.expand_dims(self.pos,axis=-2)  # (l*w*h,3) -> (l*w*h,1,3) 
         # print(f"{pd_pos.shape=}")
 
         H0 = 0  #反射（LOS）链路信道增益
         # 遍历每一面反射墙壁参数:(l1*w1,3),(l1*w1,2)
-        for i, (wall_pos, angle) in enumerate(room.get_reflect_wall_args()):
+        for i, (w_pos, angle) in enumerate(room.get_reflect_wall_args()):
             w_alpha, w_beta = np.split(angle,indices_or_sections=2, axis=-1) # (l1*w1,2) -> (l1*w1,1) + (l1*w1,1)
             w_alpha, w_beta = w_alpha.flatten(), w_beta.flatten() # (l1*w1,1) -> (l1*w1)
             # 墙壁反射单元的方向角和倾斜角,角度制转弧度制
             w_alpha_rad, w_beta_rad = np.radians([w_alpha, w_beta]) # (l1*w1)
 
             # 墙壁反射单元法向量
             Nx = np.cos(w_alpha_rad) * np.sin(w_beta_rad)
             Ny = np.sin(w_alpha_rad) * np.sin(w_beta_rad)
             Nz = np.cos(w_beta_rad)
             Nw = np.stack([Nx,Ny,Nz], axis=-1)  # 墙壁反射点法向量 (l1*w1,3)
             Nw = Nw/np.linalg.norm(Nw)  # 墙壁反射点的单位法向量 (l1*w1,3)
 
             # LED -> 墙壁反射单元
             # 发射端
-            Vt_w = wall_pos - led.pos  # LED灯到墙壁反射单元的方向向量 (l1*w1,3)
+            Vt_w = w_pos - led.pos  # LED灯到墙壁反射单元的方向向量 (l1*w1,3)
             d1 = np.linalg.norm(Vt_w, axis=-1) # 求模:LED灯到墙壁反射单元的距离 (l1*w1)
             mark1 = np.all(Vt_w==0, axis=-1) # 异常点处理:判断墙壁反射单元和LED是否重合(方向向量是否为零向量) (l1*w1)
             d1 = np.where(mark1, 1, d1)      # 异常点处理:为使cos_led_t_angle_rad分母不为0,让墙壁反射单元和LED重合时的距离不为0 (l1*w1)
             
             cos_led_t_angle_rad = np.sum(Vt_w*led.Nv, axis=-1) / d1  # LED发射角的余弦值 (l1*w1)
 
             # 接收端
             Vw_t = -Vt_w  # 墙壁反射单元到LED灯的方向向量 (l1,w1,3)
             cos_wall_r_angle_rad = np.sum(Vw_t*Nw, axis=-1) / d1 # 墙壁反射单元入射角 (l1*w1)
 
             # 墙壁反射单元 -> PD
             # 发射端
-            Vw_r = pd_pos - wall_pos # 墙壁反射单元到PD的方向向量  (l*w*h,1,3)-(l1*w1,3) (l*w*h,l1*w1,3)
+            Vw_r = pd_pos - w_pos # 墙壁反射单元到PD的方向向量  (l*w*h,1,3)-(l1*w1,3) (l*w*h,l1*w1,3)
             d2 = np.linalg.norm(Vw_r, axis=-1) # 求模:墙壁反射单元到PD之间的距离 (l*w*h,l1*w1)
 
             mark2 = np.all(Vw_r==0, axis=-1) # 异常点处理:判断墙壁反射单元和参考点是否重合(方向向量是否为零向量) (l*w*h,l1*w1)
             d2 = np.where(mark2, 1, d2)      # 异常点处理:为使cos_wall_t_angle_rad分母不为0,让墙壁反射单元和参考点重合时的距离不为0
 
             cos_wall_t_angle_rad = np.sum(Vw_r*Nw, axis=-1) / d2 # 墙壁反射单元发射角  (l*w*h,l1*w1)
             cos_wall_t_angle_rad = np.where(cos_wall_t_angle_rad>0, cos_wall_t_angle_rad, 0) # 满足墙壁反射入射条件 (l*w*h,l1*w1)
```

### Comparing `yang-vlp-0.2.15/vlppy/model/room.py` & `yang-vlp-0.2.16/vlppy/model/room.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,40 +64,37 @@
         # 不取靠近墙壁的点（符合实际环境）
         if wall in (0,5):    # 地板或天花板
             x = np.arange(gx, self.length-gx+1e-3, gx) 
             y = np.arange(gy, self.width-gy+1e-3, gy) 
             z = 0 if wall == 0 else self.height 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 地板和天花板平面建立二维网格矩阵 
         elif wall in (1,3): #前后墙  
-            x = np.arange(gx, self.length-gx+1e-3, gx) 
+            x = np.arange(0, self.length+1e-3, gx) 
             y = 0 if wall == 1 else self.width 
-            z = np.arange(gz+self.rp_height[0], self.rp_height[1]-gz+1e-3, gz) 
+            z = np.arange(self.rp_height[0], self.rp_height[1]+1e-3, gz) 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 前后墙面建立二维网格矩阵 
         else:  #左右墙
             x = self.length if wall == 2 else 0
-            y = np.arange(gy, self.width-gy+1e-3, gy) 
-            z = np.arange(gz+self.rp_height[0], self.rp_height[1]-gz+1e-3, gz) 
+            y = np.arange(0, self.width+1e-3, gy) 
+            z = np.arange(self.rp_height[0], self.rp_height[1]+1e-3, gz) 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 左右墙面建立二维网格矩阵  
         Xw, Yw, Zw = Xw.flatten(), Yw.flatten(), Zw.flatten() # 打平
         reflect_pos = np.stack([Xw, Yw, Zw], axis=-1)
         return reflect_pos
 
     def _get_reflect_wall_angle(self, shape):
         """获取反射墙壁反射单元(法向量)的方位角和倾斜角
         Return 
             angles = [[alpha0,beta0],[alpha1,beta1],...] (列表元素个数等于反射单元的个数)
                 alpha: 方位角(单位:度) (min,max) = (0°,360°)
                 beta: 倾斜角(单位:度)  (min,max) = (-90°,90°)
         """
-        print(f"{shape=}")
         alpha = np.random.uniform(low=0, high=360, size=shape)
         beta = np.random.uniform(low=-90, high=90, size=shape)
         angles = np.stack([alpha, beta], axis=-1)
-        print(f"{alpha.shape=}")
-        print(f"{angles.shape=}")
         return angles
 
     def _save_reflect_wall_args(self, fp:str, reflect_pos, angles):
         """保存反射墙壁参数(方位角和倾斜角)到excell
         Params 
             fp: 保存路径
             reflect_pos: 墙壁反射单元所在位置
@@ -130,16 +127,16 @@
             reflect_pos,angles 反射单元坐标和反射单元角度(方向角和倾斜角)(单位:度)
         """
         wall_args = pd.read_excel(fp).to_numpy()
         xw, yw, zw, alpha, beta = np.split(wall_args,indices_or_sections=5,axis=-1)
         # 加载npz文件
         # with np.load(fp) as f:
         #     xw,yw,zw,alpha,beta = f['xw'],f['yw'],f['zw'],f['alpha'],f['beta']
-        # xw, yw, zw = xw.flatten(), yw.flatten(), zw.flatten() # 打平操作
-        # alpha, beta = alpha.flatten(), beta.flatten()
+        xw, yw, zw = xw.flatten(), yw.flatten(), zw.flatten() # 打平操作
+        alpha, beta = alpha.flatten(), beta.flatten()
         reflect_pos = np.stack([xw, yw, zw], axis=-1)
         angles = np.stack([alpha, beta], axis=-1)
         return reflect_pos, angles
 
     def set_regular_wall(self):
         """设置为规制墙壁 (更新墙壁参数)
         """
```

### Comparing `yang-vlp-0.2.15/vlppy/setting/__pycache__/json_setting.cpython-39.pyc` & `yang-vlp-0.2.16/vlppy/setting/__pycache__/json_setting.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/setting/json_setting.py` & `yang-vlp-0.2.16/vlppy/setting/json_setting.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/setting/settings.json` & `yang-vlp-0.2.16/vlppy/setting/settings.json`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/signal/filter.py` & `yang-vlp-0.2.16/vlppy/signal/filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/signal/plot.py` & `yang-vlp-0.2.16/vlppy/signal/plot.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/vlppy/vis/vis.py` & `yang-vlp-0.2.16/vlppy/vis/vis.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.15/yang_vlp.egg-info/PKG-INFO` & `yang-vlp-0.2.16/yang_vlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.15
+Version: 0.2.16
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `yang-vlp-0.2.15/yang_vlp.egg-info/SOURCES.txt` & `yang-vlp-0.2.16/yang_vlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

