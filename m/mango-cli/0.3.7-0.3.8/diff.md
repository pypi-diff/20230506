# Comparing `tmp/mango-cli-0.3.7.tar.gz` & `tmp/mango-cli-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.3.7.tar", last modified: Sat May  6 01:17:49 2023, max compression
+gzip compressed data, was "mango-cli-0.3.8.tar", last modified: Sat May  6 03:47:23 2023, max compression
```

## Comparing `mango-cli-0.3.7.tar` & `mango-cli-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:17:49.612839 mango-cli-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 01:17:49.612839 mango-cli-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 01:17:19.000000 mango-cli-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:17:49.608839 mango-cli-0.3.7/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:17:19.000000 mango-cli-0.3.7/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-06 01:17:19.000000 mango-cli-0.3.7/app/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:17:49.608839 mango-cli-0.3.7/app/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:17:19.000000 mango-cli-0.3.7/app/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-06 01:17:19.000000 mango-cli-0.3.7/app/handlers/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:17:49.612839 mango-cli-0.3.7/app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:17:19.000000 mango-cli-0.3.7/app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-06 01:17:19.000000 mango-cli-0.3.7/app/services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:17:49.612839 mango-cli-0.3.7/mango_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 01:17:49.000000 mango-cli-0.3.7/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-06 01:17:49.000000 mango-cli-0.3.7/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:17:49.000000 mango-cli-0.3.7/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-06 01:17:49.000000 mango-cli-0.3.7/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-06 01:17:49.000000 mango-cli-0.3.7/mango_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 01:17:49.000000 mango-cli-0.3.7/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:17:49.612839 mango-cli-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-06 01:17:19.000000 mango-cli-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 03:47:23.094745 mango-cli-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 03:47:00.000000 mango-cli-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/handlers/download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-06 03:47:00.000000 mango-cli-0.3.8/app/services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:47:23.094745 mango-cli-0.3.8/mango_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-06 03:47:23.000000 mango-cli-0.3.8/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 03:47:22.000000 mango-cli-0.3.8/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:47:23.094745 mango-cli-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-06 03:47:00.000000 mango-cli-0.3.8/setup.py
```

### Comparing `mango-cli-0.3.7/app/handlers/download_data.py` & `mango-cli-0.3.8/app/handlers/download_data.py`

 * *Files identical despite different names*

### Comparing `mango-cli-0.3.7/app/services/data.py` & `mango-cli-0.3.8/app/services/data.py`

 * *Files identical despite different names*

### Comparing `mango-cli-0.3.7/mango_cli.egg-info/requires.txt` & `mango-cli-0.3.8/mango_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mango-cli-0.3.7/setup.py` & `mango-cli-0.3.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     version=version,
     packages=find_packages(),
     author='Mangosoft',
     author_email="wilson.mendoza@mango-soft.com",
     description="Mangosoft CLI",
     py_modules=["app"],
     include_dirs=["app"],
+    includes=["VERSION"],
     install_requires=[requirements],
     entry_points='''
         [console_scripts]
         mango=app.application:cli
     '''
 )
```

