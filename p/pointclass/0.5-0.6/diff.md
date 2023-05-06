# Comparing `tmp/pointclass-0.5.tar.gz` & `tmp/pointclass-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointclass-0.5.tar", last modified: Tue Apr 25 16:27:13 2023, max compression
+gzip compressed data, was "pointclass-0.6.tar", last modified: Sat May  6 15:05:06 2023, max compression
```

## Comparing `pointclass-0.5.tar` & `pointclass-0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 16:27:13.770138 pointclass-0.5/
--rw-rw-rw-   0        0        0      177 2023-04-25 16:27:13.766144 pointclass-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.5/licence.txt.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 16:27:13.745335 pointclass-0.5/pointclass/
--rw-rw-rw-   0        0        0      569 2023-04-25 16:26:49.000000 pointclass-0.5/pointclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 16:27:13.765148 pointclass-0.5/pointclass.egg-info/
--rw-rw-rw-   0        0        0      177 2023-04-25 16:27:13.000000 pointclass-0.5/pointclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-04-25 16:27:13.000000 pointclass-0.5/pointclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 16:27:13.000000 pointclass-0.5/pointclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 16:27:13.000000 pointclass-0.5/pointclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 16:27:13.770138 pointclass-0.5/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-04-25 16:27:05.000000 pointclass-0.5/setup1.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:05:06.583535 pointclass-0.6/
+-rw-rw-rw-   0        0        0      177 2023-05-06 15:05:06.581273 pointclass-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.6/licence.txt.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 15:05:06.536934 pointclass-0.6/pointclass/
+-rw-rw-rw-   0        0        0      835 2023-05-06 15:03:57.000000 pointclass-0.6/pointclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:05:06.580275 pointclass-0.6/pointclass.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-05-06 15:05:06.000000 pointclass-0.6/pointclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-05-06 15:05:06.000000 pointclass-0.6/pointclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 15:05:06.000000 pointclass-0.6/pointclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 15:05:06.000000 pointclass-0.6/pointclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 15:05:06.583535 pointclass-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-05-06 15:04:21.000000 pointclass-0.6/setup1.py
```

