# Comparing `tmp/analysisbykwok-0.0.24.tar.gz` & `tmp/analysisbykwok-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.24.tar", last modified: Fri May  5 13:37:40 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.25.tar", last modified: Sat May  6 14:26:56 2023, max compression
```

## Comparing `analysisbykwok-0.0.24.tar` & `analysisbykwok-0.0.25.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/
--rw-rw-rw-   0        0        0       62 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/analysisbykwok/
--rw-rw-rw-   0        0        0    17172 2023-05-05 13:35:59.000000 analysisbykwok-0.0.24/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-05 13:33:34.000000 analysisbykwok-0.0.24/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-05 13:37:40.000000 analysisbykwok-0.0.24/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2023-05-05 13:14:17.000000 analysisbykwok-0.0.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 13:37:40.650424 analysisbykwok-0.0.24/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 14:26:56.233025 analysisbykwok-0.0.25/
+-rw-rw-rw-   0        0        0       62 2023-05-06 14:26:56.233025 analysisbykwok-0.0.25/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 14:26:56.217359 analysisbykwok-0.0.25/analysisbykwok/
+-rw-rw-rw-   0        0        0    17172 2023-05-05 13:35:59.000000 analysisbykwok-0.0.25/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-06 14:26:29.000000 analysisbykwok-0.0.25/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:26:56.233025 analysisbykwok-0.0.25/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-05-06 14:26:56.000000 analysisbykwok-0.0.25/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-06 14:26:56.000000 analysisbykwok-0.0.25/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 14:26:56.000000 analysisbykwok-0.0.25/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 14:26:56.000000 analysisbykwok-0.0.25/analysisbykwok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 14:26:56.000000 analysisbykwok-0.0.25/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-05-06 14:26:24.000000 analysisbykwok-0.0.25/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 14:26:56.233025 analysisbykwok-0.0.25/setup.cfg
```

### Comparing `analysisbykwok-0.0.24/analysisbykwok/__init__.py` & `analysisbykwok-0.0.25/analysisbykwok/__init__.py`

 * *Files identical despite different names*

