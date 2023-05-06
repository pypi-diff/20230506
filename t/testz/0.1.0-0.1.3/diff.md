# Comparing `tmp/testz-0.1.0.tar.gz` & `tmp/testz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testz-0.1.0.tar", last modified: Sat May  6 16:55:54 2023, max compression
+gzip compressed data, was "testz-0.1.3.tar", last modified: Sat May  6 17:22:18 2023, max compression
```

## Comparing `testz-0.1.0.tar` & `testz-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 16:55:54.319465 testz-0.1.0/
--rw-rw-rw-   0        0        0       52 2023-05-06 16:55:54.318462 testz-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       70 2023-05-03 20:00:39.000000 testz-0.1.0/README.md
--rw-rw-rw-   0        0        0       87 2023-05-06 16:50:32.000000 testz-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 16:55:54.319465 testz-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 16:55:54.288830 testz-0.1.0/testz/
--rw-rw-rw-   0        0        0       34 2023-05-06 16:48:39.000000 testz-0.1.0/testz/__init__.py
--rw-rw-rw-   0        0        0     1289 2023-05-06 16:13:47.000000 testz-0.1.0/testz/cli.py
--rw-rw-rw-   0        0        0      365 2023-05-03 18:30:25.000000 testz-0.1.0/testz/operaciones.py
--rw-rw-rw-   0        0        0      343 2023-05-06 16:41:27.000000 testz-0.1.0/testz/pc.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:55:54.316467 testz-0.1.0/testz/struct/
--rw-rw-rw-   0        0        0      886 2023-05-03 18:02:16.000000 testz-0.1.0/testz/struct/404.py
--rw-rw-rw-   0        0        0     1105 2023-05-03 18:01:12.000000 testz-0.1.0/testz/struct/index.py
--rw-rw-rw-   0        0        0      209 2023-05-03 17:59:59.000000 testz-0.1.0/testz/struct/main.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:55:54.312377 testz-0.1.0/testz.egg-info/
--rw-rw-rw-   0        0        0       52 2023-05-06 16:55:54.000000 testz-0.1.0/testz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-06 16:55:54.000000 testz-0.1.0/testz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 16:55:54.000000 testz-0.1.0/testz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-06 16:55:54.000000 testz-0.1.0/testz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 16:55:54.000000 testz-0.1.0/testz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 17:22:18.207607 testz-0.1.3/
+-rw-rw-rw-   0        0        0      498 2023-05-06 17:22:18.207607 testz-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2023-05-03 20:00:39.000000 testz-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:22:18.209208 testz-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      843 2023-05-06 17:21:33.000000 testz-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:22:18.174540 testz-0.1.3/testz/
+-rw-rw-rw-   0        0        0       34 2023-05-06 16:48:39.000000 testz-0.1.3/testz/__init__.py
+-rw-rw-rw-   0        0        0     1289 2023-05-06 16:13:47.000000 testz-0.1.3/testz/cli.py
+-rw-rw-rw-   0        0        0      365 2023-05-03 18:30:25.000000 testz-0.1.3/testz/operaciones.py
+-rw-rw-rw-   0        0        0      406 2023-05-06 17:21:26.000000 testz-0.1.3/testz/pc.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:22:18.205071 testz-0.1.3/testz.egg-info/
+-rw-rw-rw-   0        0        0      498 2023-05-06 17:22:18.000000 testz-0.1.3/testz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-06 17:22:18.000000 testz-0.1.3/testz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:22:18.000000 testz-0.1.3/testz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-06 17:22:18.000000 testz-0.1.3/testz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 17:22:18.000000 testz-0.1.3/testz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 17:22:18.000000 testz-0.1.3/testz.egg-info/top_level.txt
```

### Comparing `testz-0.1.0/testz/cli.py` & `testz-0.1.3/testz/cli.py`

 * *Files identical despite different names*

