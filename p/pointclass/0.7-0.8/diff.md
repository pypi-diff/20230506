# Comparing `tmp/pointclass-0.7.tar.gz` & `tmp/pointclass-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointclass-0.7.tar", last modified: Sat May  6 15:17:22 2023, max compression
+gzip compressed data, was "pointclass-0.8.tar", last modified: Sat May  6 15:57:02 2023, max compression
```

## Comparing `pointclass-0.7.tar` & `pointclass-0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 15:17:22.724060 pointclass-0.7/
--rw-rw-rw-   0        0        0      177 2023-05-06 15:17:22.723063 pointclass-0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.7/licence.txt.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 15:17:22.708809 pointclass-0.7/pointclass/
--rw-rw-rw-   0        0        0      835 2023-05-06 15:17:06.000000 pointclass-0.7/pointclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 15:17:22.722067 pointclass-0.7/pointclass.egg-info/
--rw-rw-rw-   0        0        0      177 2023-05-06 15:17:22.000000 pointclass-0.7/pointclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-05-06 15:17:22.000000 pointclass-0.7/pointclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 15:17:22.000000 pointclass-0.7/pointclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 15:17:22.000000 pointclass-0.7/pointclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 15:17:22.724060 pointclass-0.7/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-05-06 15:17:16.000000 pointclass-0.7/setup1.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:57:02.547562 pointclass-0.8/
+-rw-rw-rw-   0        0        0      177 2023-05-06 15:57:02.546566 pointclass-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.8/licence.txt.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 15:57:02.527501 pointclass-0.8/pointclass/
+-rw-rw-rw-   0        0        0      973 2023-05-06 15:56:17.000000 pointclass-0.8/pointclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:57:02.545568 pointclass-0.8/pointclass.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-05-06 15:57:02.000000 pointclass-0.8/pointclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-05-06 15:57:02.000000 pointclass-0.8/pointclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 15:57:02.000000 pointclass-0.8/pointclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 15:57:02.000000 pointclass-0.8/pointclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 15:57:02.547562 pointclass-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-05-06 15:56:25.000000 pointclass-0.8/setup1.py
```

