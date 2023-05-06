# Comparing `tmp/steammy-0.1.0.tar.gz` & `tmp/steammy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steammy-0.1.0.tar", last modified: Sat May  6 18:10:36 2023, max compression
+gzip compressed data, was "steammy-0.1.1.tar", last modified: Sat May  6 18:45:09 2023, max compression
```

## Comparing `steammy-0.1.0.tar` & `steammy-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:10:36.280943 steammy-0.1.0/
--rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steammy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      249 2023-05-06 18:10:36.279947 steammy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       47 2023-05-06 18:02:42.000000 steammy-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 18:10:36.280943 steammy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      285 2023-05-06 18:07:06.000000 steammy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:10:36.268440 steammy-0.1.0/steammy/
--rw-rw-rw-   0        0        0       28 2023-05-06 17:33:14.000000 steammy-0.1.0/steammy/__init__.py
--rw-rw-rw-   0        0        0      543 2023-05-05 21:51:45.000000 steammy-0.1.0/steammy/exceptions.py
--rw-rw-rw-   0        0        0    10444 2023-05-06 17:57:23.000000 steammy-0.1.0/steammy/request.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:10:36.279947 steammy-0.1.0/steammy.egg-info/
--rw-rw-rw-   0        0        0      249 2023-05-06 18:10:36.000000 steammy-0.1.0/steammy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-06 18:10:36.000000 steammy-0.1.0/steammy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:10:36.000000 steammy-0.1.0/steammy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-06 18:10:36.000000 steammy-0.1.0/steammy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:10:36.000000 steammy-0.1.0/steammy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 18:45:09.606210 steammy-0.1.1/
+-rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steammy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      451 2023-05-06 18:45:09.606210 steammy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2023-05-06 18:02:42.000000 steammy-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 18:45:09.607208 steammy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      587 2023-05-06 18:45:05.000000 steammy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:45:09.595640 steammy-0.1.1/steammy/
+-rw-rw-rw-   0        0        0       28 2023-05-06 17:33:14.000000 steammy-0.1.1/steammy/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-05 21:51:45.000000 steammy-0.1.1/steammy/exceptions.py
+-rw-rw-rw-   0        0        0    10444 2023-05-06 17:57:23.000000 steammy-0.1.1/steammy/request.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:45:09.605214 steammy-0.1.1/steammy.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-05-06 18:45:09.000000 steammy-0.1.1/steammy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-06 18:45:09.000000 steammy-0.1.1/steammy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:45:09.000000 steammy-0.1.1/steammy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 18:45:09.000000 steammy-0.1.1/steammy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:45:09.000000 steammy-0.1.1/steammy.egg-info/top_level.txt
```

### Comparing `steammy-0.1.0/LICENSE` & `steammy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `steammy-0.1.0/steammy/exceptions.py` & `steammy-0.1.1/steammy/exceptions.py`

 * *Files identical despite different names*

### Comparing `steammy-0.1.0/steammy/request.py` & `steammy-0.1.1/steammy/request.py`

 * *Files identical despite different names*

