# Comparing `tmp/jsepp-0.1.1.tar.gz` & `tmp/jsepp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsepp-0.1.1.tar", last modified: Mon Apr 17 07:59:55 2023, max compression
+gzip compressed data, was "jsepp-0.1.2.tar", last modified: Sat May  6 04:55:07 2023, max compression
```

## Comparing `jsepp-0.1.1.tar` & `jsepp-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:59:55.827626 jsepp-0.1.1/
--rw-rw-rw-   0        0        0      610 2023-04-17 07:59:55.826629 jsepp-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-12 02:46:41.000000 jsepp-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 07:59:55.793237 jsepp-0.1.1/jsepp/
--rw-rw-rw-   0        0        0       14 2023-04-12 06:01:14.000000 jsepp-0.1.1/jsepp/__init__.py
--rw-rw-rw-   0        0        0     2049 2023-04-17 07:54:59.000000 jsepp-0.1.1/jsepp/dbutils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:59:55.826629 jsepp-0.1.1/jsepp.egg-info/
--rw-rw-rw-   0        0        0      610 2023-04-17 07:59:55.000000 jsepp-0.1.1/jsepp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-17 07:59:55.000000 jsepp-0.1.1/jsepp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:59:55.000000 jsepp-0.1.1/jsepp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-17 07:59:55.000000 jsepp-0.1.1/jsepp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 07:59:55.000000 jsepp-0.1.1/jsepp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 07:59:55.827626 jsepp-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      429 2023-04-17 07:55:55.000000 jsepp-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:55:07.973894 jsepp-0.1.2/
+-rw-rw-rw-   0        0        0      610 2023-05-06 04:55:07.973894 jsepp-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-12 02:46:41.000000 jsepp-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 04:55:07.968909 jsepp-0.1.2/jsepp/
+-rw-rw-rw-   0        0        0       14 2023-04-12 06:01:14.000000 jsepp-0.1.2/jsepp/__init__.py
+-rw-rw-rw-   0        0        0     3114 2023-05-06 04:46:06.000000 jsepp-0.1.2/jsepp/data.py
+-rw-rw-rw-   0        0        0     2049 2023-04-17 07:54:59.000000 jsepp-0.1.2/jsepp/dbutils.py
+-rw-rw-rw-   0        0        0      571 2023-05-06 04:45:51.000000 jsepp-0.1.2/jsepp/ml.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:55:07.972897 jsepp-0.1.2/jsepp.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 04:55:07.000000 jsepp-0.1.2/jsepp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 04:55:07.973894 jsepp-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      529 2023-05-06 04:53:47.000000 jsepp-0.1.2/setup.py
```

### Comparing `jsepp-0.1.1/PKG-INFO` & `jsepp-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsepp
-Version: 0.1.1
+Version: 0.1.2
 Summary: a package for general environmental data processing
 Author: Hansen Zhao
 Author-email: zhaohs12@163.com
 
 ## JSEPP
 ### dbutils
 #### MySQLConn
```

### Comparing `jsepp-0.1.1/jsepp/dbutils.py` & `jsepp-0.1.2/jsepp/dbutils.py`

 * *Files identical despite different names*

### Comparing `jsepp-0.1.1/jsepp.egg-info/PKG-INFO` & `jsepp-0.1.2/jsepp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsepp
-Version: 0.1.1
+Version: 0.1.2
 Summary: a package for general environmental data processing
 Author: Hansen Zhao
 Author-email: zhaohs12@163.com
 
 ## JSEPP
 ### dbutils
 #### MySQLConn
```

