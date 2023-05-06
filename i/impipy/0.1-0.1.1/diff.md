# Comparing `tmp/impipy-0.1.tar.gz` & `tmp/impipy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impipy-0.1.tar", last modified: Fri May  5 22:26:17 2023, max compression
+gzip compressed data, was "impipy-0.1.1.tar", last modified: Sat May  6 13:26:32 2023, max compression
```

## Comparing `impipy-0.1.tar` & `impipy-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 22:26:17.727179 impipy-0.1/
--rw-rw-rw-   0        0        0      239 2023-05-05 22:26:17.724200 impipy-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 22:26:17.719412 impipy-0.1/impipy.egg-info/
--rw-rw-rw-   0        0        0      239 2023-05-05 22:26:17.000000 impipy-0.1/impipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-05 22:26:17.000000 impipy-0.1/impipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 22:26:17.000000 impipy-0.1/impipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-05 22:26:17.000000 impipy-0.1/impipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 22:26:17.000000 impipy-0.1/impipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 22:26:17.727179 impipy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-05-05 22:24:26.000000 impipy-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:26:32.242216 impipy-0.1.1/
+-rw-rw-rw-   0        0        0      299 2023-05-06 13:26:32.225170 impipy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-05-06 13:22:50.000000 impipy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 13:26:32.157675 impipy-0.1.1/impipy/
+-rw-rw-rw-   0        0        0       91 2023-05-06 11:55:10.000000 impipy-0.1.1/impipy/__init__.py
+-rw-rw-rw-   0        0        0    27372 2023-05-05 22:01:35.000000 impipy-0.1.1/impipy/importance.py
+-rw-rw-rw-   0        0        0     8077 2023-05-05 21:58:18.000000 impipy-0.1.1/impipy/tree_importance.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:26:32.217121 impipy-0.1.1/impipy.egg-info/
+-rw-rw-rw-   0        0        0      299 2023-05-06 13:26:31.000000 impipy-0.1.1/impipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-06 13:26:31.000000 impipy-0.1.1/impipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 13:26:31.000000 impipy-0.1.1/impipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-05-06 13:26:31.000000 impipy-0.1.1/impipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 13:26:31.000000 impipy-0.1.1/impipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 13:26:32.243197 impipy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-05-06 13:25:52.000000 impipy-0.1.1/setup.py
```

