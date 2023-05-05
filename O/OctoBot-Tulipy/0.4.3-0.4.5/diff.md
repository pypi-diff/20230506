# Comparing `tmp/OctoBot-Tulipy-0.4.3.tar.gz` & `tmp/OctoBot-Tulipy-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Tulipy-0.4.3.tar", last modified: Tue May  2 16:18:37 2023, max compression
+gzip compressed data, was "OctoBot-Tulipy-0.4.5.tar", last modified: Fri May  5 22:25:02 2023, max compression
```

## Comparing `OctoBot-Tulipy-0.4.3.tar` & `OctoBot-Tulipy-0.4.5.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:18:37.980132 OctoBot-Tulipy-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:18:37.980132 OctoBot-Tulipy-0.4.3/OctoBot_Tulipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-02 16:18:37.000000 OctoBot-Tulipy-0.4.3/OctoBot_Tulipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-02 16:18:37.000000 OctoBot-Tulipy-0.4.3/OctoBot_Tulipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:18:37.000000 OctoBot-Tulipy-0.4.3/OctoBot_Tulipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 16:18:37.000000 OctoBot-Tulipy-0.4.3/OctoBot_Tulipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 16:18:37.000000 OctoBot-Tulipy-0.4.3/OctoBot_Tulipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-02 16:18:37.980132 OctoBot-Tulipy-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:18:37.980132 OctoBot-Tulipy-0.4.3/libindicators/
--rw-r--r--   0 runner    (1001) docker     (123)   162241 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/libindicators/tiamalgamation.c
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:18:37.980132 OctoBot-Tulipy-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:18:37.980132 OctoBot-Tulipy-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:18:37.980132 OctoBot-Tulipy-0.4.3/tulipy/
--rw-r--r--   0 runner    (1001) docker     (123)    38448 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/tulipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:18:37.980132 OctoBot-Tulipy-0.4.3/tulipy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-02 16:18:03.000000 OctoBot-Tulipy-0.4.3/tulipy/lib/__init__.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:25:02.772745 OctoBot-Tulipy-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:25:02.768744 OctoBot-Tulipy-0.4.5/OctoBot_Tulipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-05 22:25:02.000000 OctoBot-Tulipy-0.4.5/OctoBot_Tulipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-05 22:25:02.000000 OctoBot-Tulipy-0.4.5/OctoBot_Tulipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:25:02.000000 OctoBot-Tulipy-0.4.5/OctoBot_Tulipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 22:25:02.000000 OctoBot-Tulipy-0.4.5/OctoBot_Tulipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 22:25:02.000000 OctoBot-Tulipy-0.4.5/OctoBot_Tulipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-05 22:25:02.772745 OctoBot-Tulipy-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:25:02.768744 OctoBot-Tulipy-0.4.5/libindicators/
+-rw-r--r--   0 runner    (1001) docker     (123)   162241 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/libindicators/tiamalgamation.c
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:25:02.772745 OctoBot-Tulipy-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:25:02.768744 OctoBot-Tulipy-0.4.5/tulipy/
+-rw-r--r--   0 runner    (1001) docker     (123)    38448 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/tulipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:25:02.772745 OctoBot-Tulipy-0.4.5/tulipy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-05 22:24:47.000000 OctoBot-Tulipy-0.4.5/tulipy/lib/__init__.pyx
```

### Comparing `OctoBot-Tulipy-0.4.3/LICENSE` & `OctoBot-Tulipy-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Tulipy-0.4.3/OctoBot_Tulipy.egg-info/PKG-INFO` & `OctoBot-Tulipy-0.4.5/OctoBot_Tulipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Tulipy
-Version: 0.4.3
+Version: 0.4.5
 Summary: Financial Technical Analysis Indicator Library. Python bindings for https://github.com/TulipCharts/tulipindicators
 Home-page: https://github.com/Drakkar-Software/tulipy
 Author: Drakkar-Software
 License: LGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `OctoBot-Tulipy-0.4.3/PKG-INFO` & `OctoBot-Tulipy-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Tulipy
-Version: 0.4.3
+Version: 0.4.5
 Summary: Financial Technical Analysis Indicator Library. Python bindings for https://github.com/TulipCharts/tulipindicators
 Home-page: https://github.com/Drakkar-Software/tulipy
 Author: Drakkar-Software
 License: LGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `OctoBot-Tulipy-0.4.3/README.md` & `OctoBot-Tulipy-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `OctoBot-Tulipy-0.4.3/libindicators/tiamalgamation.c` & `OctoBot-Tulipy-0.4.5/libindicators/tiamalgamation.c`

 * *Files identical despite different names*

### Comparing `OctoBot-Tulipy-0.4.3/setup.py` & `OctoBot-Tulipy-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 
 setup(
     name='OctoBot-Tulipy',
     description='Financial Technical Analysis Indicator Library. Python bindings for https://github.com/TulipCharts/tulipindicators',
     long_description=long_description,
     long_description_content_type='text/markdown; charset=UTF-8',
-    version='0.4.3',
+    version='0.4.5',
     url='https://github.com/Drakkar-Software/tulipy',
     author='Drakkar-Software',
     license='LGPL-3.0',
     cmdclass={'build_ext': build_ext},
     ext_modules=ext_modules,
     packages=find_packages(exclude=["tests"]),
     install_requires=['numpy >= 1.22.3'],
```

### Comparing `OctoBot-Tulipy-0.4.3/tulipy/__init__.py` & `OctoBot-Tulipy-0.4.5/tulipy/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tulipy-0.4.3/tulipy/lib/__init__.pyx` & `OctoBot-Tulipy-0.4.5/tulipy/lib/__init__.pyx`

 * *Files identical despite different names*

