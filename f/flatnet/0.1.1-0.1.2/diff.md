# Comparing `tmp/flatnet-0.1.1.tar.gz` & `tmp/flatnet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatnet-0.1.1.tar", last modified: Fri May  5 21:55:11 2023, max compression
+gzip compressed data, was "flatnet-0.1.2.tar", last modified: Fri May  5 22:01:39 2023, max compression
```

## Comparing `flatnet-0.1.1.tar` & `flatnet-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,13 @@
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:25.978708 flatnet-0.1.1/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:10:25.963083 flatnet-0.1.1/PKG-INFO
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3012 2023-05-06 03:53:34.000000 flatnet-0.1.1/README.md
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:24.519713 flatnet-0.1.1/flatnet/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.1.1/flatnet/__init__.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:24.958895 flatnet-0.1.1/flatnet/modules/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.1.1/flatnet/modules/__init__.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.1.1/flatnet/modules/flatnet_nn.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    14293 2023-05-06 04:09:02.000000 flatnet-0.1.1/flatnet/train.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:24.818928 flatnet-0.1.1/flatnet.egg-info/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:10:23.000000 flatnet-0.1.1/flatnet.egg-info/PKG-INFO
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      668 2023-05-06 04:10:24.000000 flatnet-0.1.1/flatnet.egg-info/SOURCES.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-06 04:10:23.000000 flatnet-0.1.1/flatnet.egg-info/dependency_links.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      556 2023-05-06 04:10:23.000000 flatnet-0.1.1/flatnet.egg-info/requires.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       21 2023-05-06 04:10:23.000000 flatnet-0.1.1/flatnet.egg-info/top_level.txt
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:25.178467 flatnet-0.1.1/models/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/__init__.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      410 2022-11-18 19:19:10.000000 flatnet-0.1.1/models/operators.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      520 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:25.664951 flatnet-0.1.1/models/umap_scripts/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/__init__.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    36015 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/distances.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    34501 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/layouts.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    17347 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/sparse.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    12988 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/spectral.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)   136753 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/umap.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     6896 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/utils.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     8208 2022-11-21 18:44:42.000000 flatnet-0.1.1/models/vae.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-06 04:10:25.978708 flatnet-0.1.1/setup.cfg
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     1202 2023-05-06 04:08:32.000000 flatnet-0.1.1/setup.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:25.921306 flatnet-0.1.1/tools/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:39.000000 flatnet-0.1.1/tools/__init__.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      608 2022-11-04 18:24:19.000000 flatnet-0.1.1/tools/gp_manifold_generator.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3433 2023-01-22 00:04:53.000000 flatnet-0.1.1/tools/manifold_generator.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3241 2022-10-28 03:06:50.000000 flatnet-0.1.1/tools/randman.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-03-31 21:46:28.000000 flatnet-0.1.1/tools/test_geodesics.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:16:24.518978 flatnet-0.1.2/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:16:24.518978 flatnet-0.1.2/PKG-INFO
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:16:24.189229 flatnet-0.1.2/flatnet/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.1.2/flatnet/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    14293 2023-05-06 04:09:02.000000 flatnet-0.1.2/flatnet/train.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:16:24.456012 flatnet-0.1.2/flatnet.egg-info/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      199 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      556 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/requires.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-06 04:16:23.000000 flatnet-0.1.2/flatnet.egg-info/top_level.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-06 04:16:24.518978 flatnet-0.1.2/setup.cfg
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     1198 2023-05-06 04:14:23.000000 flatnet-0.1.2/setup.py
```

### Comparing `flatnet-0.1.1/flatnet/train.py` & `flatnet-0.1.2/flatnet/train.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.1/flatnet.egg-info/requires.txt` & `flatnet-0.1.2/flatnet.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.1/setup.py` & `flatnet-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flatnet',
-    version='0.1.1',
+    version='0.1.2',
     description='FlatNet implementation in PyTorch, from the paper \"Representation Learning via Manifold Flattening and Reconstruction\"',
     author='Michael Psenka',
-    packages=find_packages(),
+    packages=['flatnet'],
     install_requires=[ 
         'cmake>=3.26.3',
         'filelock>=3.12.0',
         'geoopt>=0.5.0',
         'Jinja2>=3.1.2',
         'lit>=16.0.2',
         'MarkupSafe>=2.1.2',
```

