# Comparing `tmp/ezmote-cmdserver-0.8.4.tar.gz` & `tmp/ezmote-cmdserver-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmote-cmdserver-0.8.4.tar", last modified: Sat May  6 08:11:43 2023, max compression
+gzip compressed data, was "ezmote-cmdserver-0.8.5.tar", last modified: Sat May  6 08:27:12 2023, max compression
```

## Comparing `ezmote-cmdserver-0.8.4.tar` & `ezmote-cmdserver-0.8.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:11:43.585117 ezmote-cmdserver-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 08:11:43.585117 ezmote-cmdserver-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:11:43.581117 ezmote-cmdserver-0.8.4/cmdserver/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:11:43.585117 ezmote-cmdserver-0.8.4/cmdserver/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/pj.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/playingnow.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/tivo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/tivos.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/apis/wake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/commandcontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/debounce.py
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/infoprovider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/jvc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25365 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/jvccommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/pjcontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/tivocontroller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)    69607 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/cmdserver/zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:11:43.585117 ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 08:11:43.000000 ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-06 08:11:43.000000 ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:11:43.000000 ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 08:11:43.000000 ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:11:43.000000 ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-06 08:11:43.000000 ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 08:11:43.000000 ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:11:43.585117 ezmote-cmdserver-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-06 08:11:07.000000 ezmote-cmdserver-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:27:12.746675 ezmote-cmdserver-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 08:27:12.746675 ezmote-cmdserver-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:27:12.746675 ezmote-cmdserver-0.8.5/cmdserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 08:26:37.000000 ezmote-cmdserver-0.8.5/cmdserver/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:27:12.746675 ezmote-cmdserver-0.8.5/cmdserver/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/pj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/playingnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/tivo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/tivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/apis/wake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/commandcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/infoprovider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/jvc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25365 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/jvccommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/pjcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/tivocontroller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69607 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/cmdserver/zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:27:12.746675 ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-06 08:27:12.000000 ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-06 08:27:12.000000 ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:27:12.000000 ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 08:27:12.000000 ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:27:12.000000 ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-06 08:27:12.000000 ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 08:27:12.000000 ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:27:12.746675 ezmote-cmdserver-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-06 08:26:36.000000 ezmote-cmdserver-0.8.5/setup.py
```

### Comparing `ezmote-cmdserver-0.8.4/LICENSE` & `ezmote-cmdserver-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/PKG-INFO` & `ezmote-cmdserver-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmote-cmdserver
-Version: 0.8.4
+Version: 0.8.5
 Summary: A small webapp which can be used for web based home cinema automation
 Home-page: http://github.com/3ll3d00d/cmdserver
 Author: Matt Khan
 Author-email: mattkhan+cmdserver@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ezmote-cmdserver-0.8.4/README.md` & `ezmote-cmdserver-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/apis/command.py` & `ezmote-cmdserver-0.8.5/cmdserver/apis/command.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/apis/info.py` & `ezmote-cmdserver-0.8.5/cmdserver/apis/info.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/apis/pj.py` & `ezmote-cmdserver-0.8.5/cmdserver/apis/pj.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/apis/tivo.py` & `ezmote-cmdserver-0.8.5/cmdserver/apis/tivo.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/apis/tivos.py` & `ezmote-cmdserver-0.8.5/cmdserver/apis/tivos.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/apis/wake.py` & `ezmote-cmdserver-0.8.5/cmdserver/apis/wake.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/commandcontroller.py` & `ezmote-cmdserver-0.8.5/cmdserver/commandcontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/config.py` & `ezmote-cmdserver-0.8.5/cmdserver/config.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/debounce.py` & `ezmote-cmdserver-0.8.5/cmdserver/debounce.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/infoprovider.py` & `ezmote-cmdserver-0.8.5/cmdserver/infoprovider.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/jvc.py` & `ezmote-cmdserver-0.8.5/cmdserver/jvc.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/jvccommands.py` & `ezmote-cmdserver-0.8.5/cmdserver/jvccommands.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/main.py` & `ezmote-cmdserver-0.8.5/cmdserver/main.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/pjcontroller.py` & `ezmote-cmdserver-0.8.5/cmdserver/pjcontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/tivocontroller.py` & `ezmote-cmdserver-0.8.5/cmdserver/tivocontroller.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/ws.py` & `ezmote-cmdserver-0.8.5/cmdserver/ws.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/cmdserver/zeroconf.py` & `ezmote-cmdserver-0.8.5/cmdserver/zeroconf.py`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/PKG-INFO` & `ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmote-cmdserver
-Version: 0.8.4
+Version: 0.8.5
 Summary: A small webapp which can be used for web based home cinema automation
 Home-page: http://github.com/3ll3d00d/cmdserver
 Author: Matt Khan
 Author-email: mattkhan+cmdserver@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/SOURCES.txt` & `ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/ezmote_cmdserver.egg-info/requires.txt` & `ezmote-cmdserver-0.8.5/ezmote_cmdserver.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ezmote-cmdserver-0.8.4/setup.py` & `ezmote-cmdserver-0.8.5/setup.py`

 * *Files identical despite different names*

