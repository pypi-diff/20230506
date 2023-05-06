# Comparing `tmp/obfuscater-1.0.0.tar.gz` & `tmp/obfuscater-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obfuscater-1.0.0.tar", last modified: Sat May  6 07:16:42 2023, max compression
+gzip compressed data, was "obfuscater-2.0.0.tar", last modified: Sat May  6 07:35:00 2023, max compression
```

## Comparing `obfuscater-1.0.0.tar` & `obfuscater-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:16:42.492667 obfuscater-1.0.0/
--rw-rw-rw-   0        0        0      291 2023-05-06 07:16:42.492667 obfuscater-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 07:16:42.489255 obfuscater-1.0.0/obfuscater/
--rw-rw-rw-   0        0        0    73455 2023-05-06 07:14:57.000000 obfuscater-1.0.0/obfuscater/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:16:42.491667 obfuscater-1.0.0/obfuscater.egg-info/
--rw-rw-rw-   0        0        0      291 2023-05-06 07:16:42.000000 obfuscater-1.0.0/obfuscater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-06 07:16:42.000000 obfuscater-1.0.0/obfuscater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:16:42.000000 obfuscater-1.0.0/obfuscater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 07:16:42.000000 obfuscater-1.0.0/obfuscater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 07:16:42.493648 obfuscater-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-05-06 07:16:09.000000 obfuscater-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:35:00.745525 obfuscater-2.0.0/
+-rw-rw-rw-   0        0        0      291 2023-05-06 07:35:00.745525 obfuscater-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 07:35:00.740528 obfuscater-2.0.0/obfuscater/
+-rw-rw-rw-   0        0        0    73455 2023-05-06 07:14:57.000000 obfuscater-2.0.0/obfuscater/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-05-06 07:23:29.000000 obfuscater-2.0.0/obfuscater/run.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:35:00.744524 obfuscater-2.0.0/obfuscater.egg-info/
+-rw-rw-rw-   0        0        0      291 2023-05-06 07:35:00.000000 obfuscater-2.0.0/obfuscater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-05-06 07:35:00.000000 obfuscater-2.0.0/obfuscater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:35:00.000000 obfuscater-2.0.0/obfuscater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 07:35:00.000000 obfuscater-2.0.0/obfuscater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:35:00.746523 obfuscater-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0    74016 2023-05-06 07:34:12.000000 obfuscater-2.0.0/setup.py
```

### Comparing `obfuscater-1.0.0/obfuscater/__init__.py` & `obfuscater-2.0.0/obfuscater/__init__.py`

 * *Files identical despite different names*

