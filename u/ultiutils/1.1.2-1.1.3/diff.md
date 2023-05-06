# Comparing `tmp/ultiutils-1.1.2.tar.gz` & `tmp/ultiutils-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultiutils-1.1.2.tar", last modified: Fri Apr 21 22:54:29 2023, max compression
+gzip compressed data, was "ultiutils-1.1.3.tar", last modified: Sat May  6 14:11:27 2023, max compression
```

## Comparing `ultiutils-1.1.2.tar` & `ultiutils-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 22:54:29.667918 ultiutils-1.1.2/
--rw-r--r--   0 runner    (1000) runner    (1000)      485 2023-04-21 22:54:29.667918 ultiutils-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2021-07-22 16:01:49.000000 ultiutils-1.1.2/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      306 2021-07-24 20:39:36.000000 ultiutils-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-21 22:54:29.667918 ultiutils-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1591 2021-07-24 20:08:38.000000 ultiutils-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 22:54:29.663917 ultiutils-1.1.2/ultiutils/
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2021-07-24 20:39:17.000000 ultiutils-1.1.2/ultiutils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3710 2021-07-23 01:39:59.000000 ultiutils-1.1.2/ultiutils/ultimain.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 22:54:29.667918 ultiutils-1.1.2/ultiutils.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      485 2023-04-21 22:54:29.000000 ultiutils-1.1.2/ultiutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      241 2023-04-21 22:54:29.000000 ultiutils-1.1.2/ultiutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-21 22:54:29.000000 ultiutils-1.1.2/ultiutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-04-21 22:54:29.000000 ultiutils-1.1.2/ultiutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-04-21 22:54:29.000000 ultiutils-1.1.2/ultiutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 14:11:27.641884 ultiutils-1.1.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)      485 2023-05-06 14:11:27.641884 ultiutils-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2021-07-22 16:01:49.000000 ultiutils-1.1.3/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      306 2021-07-24 20:39:36.000000 ultiutils-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-06 14:11:27.641884 ultiutils-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1591 2021-07-24 20:08:38.000000 ultiutils-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 14:11:27.641884 ultiutils-1.1.3/ultiutils/
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2021-07-24 20:39:17.000000 ultiutils-1.1.3/ultiutils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3710 2021-07-23 01:39:59.000000 ultiutils-1.1.3/ultiutils/ultimain.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 14:11:27.641884 ultiutils-1.1.3/ultiutils.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      485 2023-05-06 14:11:27.000000 ultiutils-1.1.3/ultiutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      241 2023-05-06 14:11:27.000000 ultiutils-1.1.3/ultiutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 14:11:27.000000 ultiutils-1.1.3/ultiutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-05-06 14:11:27.000000 ultiutils-1.1.3/ultiutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-05-06 14:11:27.000000 ultiutils-1.1.3/ultiutils.egg-info/top_level.txt
```

### Comparing `ultiutils-1.1.2/setup.py` & `ultiutils-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `ultiutils-1.1.2/ultiutils/ultimain.py` & `ultiutils-1.1.3/ultiutils/ultimain.py`

 * *Files identical despite different names*

