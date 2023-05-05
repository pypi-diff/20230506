# Comparing `tmp/causalforge-0.0.7.tar.gz` & `tmp/causalforge-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalforge-0.0.7.tar", last modified: Tue May  2 00:17:13 2023, max compression
+gzip compressed data, was "causalforge-0.0.8.tar", last modified: Fri May  5 23:30:22 2023, max compression
```

## Comparing `causalforge-0.0.7.tar` & `causalforge-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-02 00:17:13.008997 causalforge-0.0.7/
--rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.7/LICENSE
--rw-r--r--   0 AG62216    (501) staff       (20)     2942 2023-05-02 00:17:13.009132 causalforge-0.0.7/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)     2491 2023-05-01 23:55:39.000000 causalforge-0.0.7/README.md
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-02 00:17:13.004813 causalforge-0.0.7/causalforge/
--rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-05-02 00:16:22.000000 causalforge-0.0.7/causalforge/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-02 00:17:13.008553 causalforge-0.0.7/causalforge/tests/
--rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.7/causalforge/tests/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-02 00:17:13.007871 causalforge-0.0.7/causalforge.egg-info/
--rw-r--r--   0 AG62216    (501) staff       (20)     2942 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/SOURCES.txt
--rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/dependency_links.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      128 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/requires.txt
--rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/top_level.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-02 00:17:13.009783 causalforge-0.0.7/setup.cfg
--rw-r--r--   0 AG62216    (501) staff       (20)     1659 2023-04-26 23:15:59.000000 causalforge-0.0.7/setup.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-05 23:30:22.797928 causalforge-0.0.8/
+-rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.8/LICENSE
+-rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-05 23:30:22.798164 causalforge-0.0.8/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)     2580 2023-05-04 08:14:33.000000 causalforge-0.0.8/README.md
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-05 23:30:22.787429 causalforge-0.0.8/causalforge/
+-rw-r--r--   0 AG62216    (501) staff       (20)      146 2023-05-05 23:29:22.000000 causalforge-0.0.8/causalforge/__init__.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     3801 2023-05-03 23:40:50.000000 causalforge-0.0.8/causalforge/data_loader.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     3285 2023-05-05 22:52:33.000000 causalforge-0.0.8/causalforge/metrics.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     2870 2023-05-04 17:12:50.000000 causalforge-0.0.8/causalforge/model.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-05 23:30:22.796688 causalforge-0.0.8/causalforge/models/
+-rw-r--r--   0 AG62216    (501) staff       (20)       85 2023-05-04 00:28:37.000000 causalforge-0.0.8/causalforge/models/__init__.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     7439 2023-05-05 22:30:35.000000 causalforge-0.0.8/causalforge/models/dragonnet.py
+-rw-r--r--   0 AG62216    (501) staff       (20)     5911 2023-05-04 01:22:14.000000 causalforge-0.0.8/causalforge/models/utils.py
+-rw-r--r--   0 AG62216    (501) staff       (20)      519 2023-05-05 04:55:01.000000 causalforge-0.0.8/causalforge/utils.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-05 23:30:22.793061 causalforge-0.0.8/causalforge.egg-info/
+-rw-r--r--   0 AG62216    (501) staff       (20)     3032 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)      417 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/SOURCES.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/dependency_links.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      137 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/requires.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-05 23:30:22.000000 causalforge-0.0.8/causalforge.egg-info/top_level.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-05 23:30:22.799226 causalforge-0.0.8/setup.cfg
+-rw-r--r--   0 AG62216    (501) staff       (20)     1660 2023-05-02 00:20:37.000000 causalforge-0.0.8/setup.py
```

### Comparing `causalforge-0.0.7/LICENSE` & `causalforge-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.7/PKG-INFO` & `causalforge-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-Metadata-Version: 2.1
-Name: causalforge
-Version: 0.0.7
-Summary: Python Package for Causal Inference
-Home-page: https://github.com/anthem-ai/causalflow
-Author: Gino Tesei, Jey Kottalam
-Author-email: 
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalforge/main/logo.png">
 
-<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png?token=GHSAT0AAAAAAB6UCMRK6JN5QVPWHF2GO3XSZCQL25A">
-
-# CausalFlow
+# CausalForge
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 
 CausalForge is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
-from experimental or observational data.
+from experimental or observational data. Methods have been redesigned for production. [Check out the documentation.](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 
 <details>
   <summary> <H3>Installing Python Package</H3>  </summary>
 
 We recommend to create a proper enviroment with tensorflow and pytorch 
 installed. For example, for a local Mac enviroment without GPUs:
```

### Comparing `causalforge-0.0.7/setup.py` & `causalforge-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     name="causalforge",
     version=causalforge.__version__,
     author="Gino Tesei, Jey Kottalam",
     author_email="",
     description="Python Package for Causal Inference",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/anthem-ai/causalflow",
+    url="https://github.com/anthem-ai/causalforge",
     packages=packages,
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
```

