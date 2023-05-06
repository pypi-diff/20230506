# Comparing `tmp/flatnet-0.1.2.tar.gz` & `tmp/flatnet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatnet-0.1.2.tar", last modified: Fri May  5 22:01:39 2023, max compression
+gzip compressed data, was "flatnet-0.1.3.tar", last modified: Fri May  5 22:15:39 2023, max compression
```

## Comparing `flatnet-0.1.2.tar` & `flatnet-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:16:24.518978 flatnet-0.1.2/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:16:24.518978 flatnet-0.1.2/PKG-INFO
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:16:24.189229 flatnet-0.1.2/flatnet/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.1.2/flatnet/__init__.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    14293 2023-05-06 04:09:02.000000 flatnet-0.1.2/flatnet/train.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:16:24.456012 flatnet-0.1.2/flatnet.egg-info/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/PKG-INFO
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      199 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/SOURCES.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/dependency_links.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      556 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/requires.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/top_level.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-06 04:16:24.518978 flatnet-0.1.2/setup.cfg
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     1198 2023-05-06 04:14:23.000000 flatnet-0.1.2/setup.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:29:20.380452 flatnet-0.1.3/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:29:20.380452 flatnet-0.1.3/PKG-INFO
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:29:19.879272 flatnet-0.1.3/flatnet/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.1.3/flatnet/__init__.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:29:20.301887 flatnet-0.1.3/flatnet/modules/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.1.3/flatnet/modules/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.1.3/flatnet/modules/flatnet_nn.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    14293 2023-05-06 04:09:02.000000 flatnet-0.1.3/flatnet/train.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:29:20.160860 flatnet-0.1.3/flatnet.egg-info/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      257 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      556 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/requires.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/top_level.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-06 04:29:20.380452 flatnet-0.1.3/setup.cfg
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     1202 2023-05-06 04:28:06.000000 flatnet-0.1.3/setup.py
```

### Comparing `flatnet-0.1.2/flatnet/train.py` & `flatnet-0.1.3/flatnet/train.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.2/flatnet.egg-info/requires.txt` & `flatnet-0.1.3/flatnet.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.2/setup.py` & `flatnet-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flatnet',
-    version='0.1.2',
+    version='0.1.3',
     description='FlatNet implementation in PyTorch, from the paper \"Representation Learning via Manifold Flattening and Reconstruction\"',
     author='Michael Psenka',
-    packages=['flatnet'],
+    packages=find_packages(),
     install_requires=[ 
         'cmake>=3.26.3',
         'filelock>=3.12.0',
         'geoopt>=0.5.0',
         'Jinja2>=3.1.2',
         'lit>=16.0.2',
         'MarkupSafe>=2.1.2',
```

