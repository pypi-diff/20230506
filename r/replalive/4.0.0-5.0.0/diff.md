# Comparing `tmp/replalive-4.0.0.tar.gz` & `tmp/replalive-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replalive-4.0.0.tar", last modified: Sat May  6 15:34:25 2023, max compression
+gzip compressed data, was "replalive-5.0.0.tar", last modified: Sat May  6 15:37:51 2023, max compression
```

## Comparing `replalive-4.0.0.tar` & `replalive-5.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 15:34:25.146693 replalive-4.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)      718 2023-05-06 15:34:25.146693 replalive-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      578 2023-05-06 15:34:11.000000 replalive-4.0.0/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 replalive-4.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 15:34:25.146693 replalive-4.0.0/replalive.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      718 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      197 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 15:34:25.000000 replalive-4.0.0/replalive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-06 15:34:25.146693 replalive-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      405 2023-05-06 15:34:18.000000 replalive-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 15:37:51.430326 replalive-5.0.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)      878 2023-05-06 15:37:51.426325 replalive-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      739 2023-05-06 15:37:28.000000 replalive-5.0.0/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 replalive-5.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-06 15:37:51.426325 replalive-5.0.0/replalive.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      878 2023-05-06 15:37:51.000000 replalive-5.0.0/replalive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      197 2023-05-06 15:37:51.000000 replalive-5.0.0/replalive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 15:37:51.000000 replalive-5.0.0/replalive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-05-06 15:37:51.000000 replalive-5.0.0/replalive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-06 15:37:51.000000 replalive-5.0.0/replalive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-06 15:37:51.430326 replalive-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      405 2023-05-06 15:37:48.000000 replalive-5.0.0/setup.py
```

