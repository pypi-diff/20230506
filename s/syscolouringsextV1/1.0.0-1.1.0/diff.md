# Comparing `tmp/syscolouringsextV1-1.0.0.tar.gz` & `tmp/syscolouringsextV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscolouringsextV1-1.0.0.tar", last modified: Sat May  6 21:26:55 2023, max compression
+gzip compressed data, was "syscolouringsextV1-1.1.0.tar", last modified: Sat May  6 21:29:01 2023, max compression
```

## Comparing `syscolouringsextV1-1.0.0.tar` & `syscolouringsextV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 21:26:55.557401 syscolouringsextV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-06 21:26:55.557401 syscolouringsextV1-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 21:26:55.557401 syscolouringsextV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-06 21:26:55.000000 syscolouringsextV1-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 21:26:55.557401 syscolouringsextV1-1.0.0/syscolouringsextV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-06 21:26:55.000000 syscolouringsextV1-1.0.0/syscolouringsextV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 21:26:55.557401 syscolouringsextV1-1.0.0/syscolouringsextV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-06 21:26:55.000000 syscolouringsextV1-1.0.0/syscolouringsextV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-06 21:26:55.000000 syscolouringsextV1-1.0.0/syscolouringsextV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 21:26:55.000000 syscolouringsextV1-1.0.0/syscolouringsextV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-06 21:26:55.000000 syscolouringsextV1-1.0.0/syscolouringsextV1.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 21:29:01.344141 syscolouringsextV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-06 21:29:01.344141 syscolouringsextV1-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 21:29:01.344141 syscolouringsextV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-06 21:29:01.000000 syscolouringsextV1-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 21:29:01.340141 syscolouringsextV1-1.1.0/syscolouringsextV1/
+-rw-r--r--   0 root         (0) root         (0)    72010 2023-05-06 21:29:01.000000 syscolouringsextV1-1.1.0/syscolouringsextV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 21:29:01.340141 syscolouringsextV1-1.1.0/syscolouringsextV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-06 21:29:01.000000 syscolouringsextV1-1.1.0/syscolouringsextV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-06 21:29:01.000000 syscolouringsextV1-1.1.0/syscolouringsextV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 21:29:01.000000 syscolouringsextV1-1.1.0/syscolouringsextV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-06 21:29:01.000000 syscolouringsextV1-1.1.0/syscolouringsextV1.egg-info/top_level.txt
```

