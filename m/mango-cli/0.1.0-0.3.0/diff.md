# Comparing `tmp/mango-cli-0.1.0.tar.gz` & `tmp/mango-cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.1.0.tar", last modified: Fri May  5 22:07:35 2023, max compression
+gzip compressed data, was "mango-cli-0.3.0.tar", last modified: Fri May  5 22:35:57 2023, max compression
```

## Comparing `mango-cli-0.1.0.tar` & `mango-cli-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:35.237712 mango-cli-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 22:07:35.237712 mango-cli-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 22:07:13.000000 mango-cli-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:35.237712 mango-cli-0.1.0/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:13.000000 mango-cli-0.1.0/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-05 22:07:13.000000 mango-cli-0.1.0/app/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:35.237712 mango-cli-0.1.0/app/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:13.000000 mango-cli-0.1.0/app/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-05 22:07:13.000000 mango-cli-0.1.0/app/handlers/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:35.237712 mango-cli-0.1.0/app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:13.000000 mango-cli-0.1.0/app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-05 22:07:13.000000 mango-cli-0.1.0/app/services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:35.237712 mango-cli-0.1.0/mango_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 22:07:35.000000 mango-cli-0.1.0/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-05 22:07:35.000000 mango-cli-0.1.0/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:07:35.000000 mango-cli-0.1.0/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 22:07:35.000000 mango-cli-0.1.0/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 22:07:35.000000 mango-cli-0.1.0/mango_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 22:07:35.000000 mango-cli-0.1.0/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:07:35.237712 mango-cli-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 22:07:13.000000 mango-cli-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:35:57.940195 mango-cli-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 22:35:57.940195 mango-cli-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 22:35:29.000000 mango-cli-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:35:57.940195 mango-cli-0.3.0/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:35:29.000000 mango-cli-0.3.0/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-05 22:35:29.000000 mango-cli-0.3.0/app/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:35:57.940195 mango-cli-0.3.0/app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:35:29.000000 mango-cli-0.3.0/app/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-05 22:35:29.000000 mango-cli-0.3.0/app/handlers/download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:35:57.940195 mango-cli-0.3.0/app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:35:29.000000 mango-cli-0.3.0/app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-05 22:35:29.000000 mango-cli-0.3.0/app/services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:35:57.940195 mango-cli-0.3.0/mango_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 22:35:57.000000 mango-cli-0.3.0/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-05 22:35:57.000000 mango-cli-0.3.0/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:35:57.000000 mango-cli-0.3.0/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 22:35:57.000000 mango-cli-0.3.0/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 22:35:57.000000 mango-cli-0.3.0/mango_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 22:35:57.000000 mango-cli-0.3.0/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:35:57.940195 mango-cli-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 22:35:29.000000 mango-cli-0.3.0/setup.py
```

### Comparing `mango-cli-0.1.0/app/handlers/download_data.py` & `mango-cli-0.3.0/app/handlers/download_data.py`

 * *Files identical despite different names*

### Comparing `mango-cli-0.1.0/app/services/data.py` & `mango-cli-0.3.0/app/services/data.py`

 * *Files identical despite different names*

### Comparing `mango-cli-0.1.0/mango_cli.egg-info/requires.txt` & `mango-cli-0.3.0/mango_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mango-cli-0.1.0/setup.py` & `mango-cli-0.3.0/setup.py`

 * *Files identical despite different names*

