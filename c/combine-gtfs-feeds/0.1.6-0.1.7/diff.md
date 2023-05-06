# Comparing `tmp/combine_gtfs_feeds-0.1.6.tar.gz` & `tmp/combine_gtfs_feeds-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combine_gtfs_feeds-0.1.6.tar", last modified: Sat May  6 03:19:53 2023, max compression
+gzip compressed data, was "combine_gtfs_feeds-0.1.7.tar", last modified: Sat May  6 03:38:46 2023, max compression
```

## Comparing `combine_gtfs_feeds-0.1.6.tar` & `combine_gtfs_feeds-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:19:53.803478 combine_gtfs_feeds-0.1.6/
--rw-rw-rw-   0        0        0     1106 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      775 2023-05-06 03:19:53.803478 combine_gtfs_feeds-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-02-04 22:54:46.000000 combine_gtfs_feeds-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 03:19:53.653037 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/
--rw-rw-rw-   0        0        0       55 2022-06-19 21:37:15.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:19:53.796680 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/
--rw-rw-rw-   0        0        0       79 2023-02-05 03:16:30.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/__init__.py
--rw-rw-rw-   0        0        0      937 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/cli.py
--rw-rw-rw-   0        0        0     7284 2023-02-06 23:13:16.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/gtfs_schema.py
--rw-rw-rw-   0        0        0     1115 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/log_controller.py
--rw-rw-rw-   0        0        0      424 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/main.py
--rw-rw-rw-   0        0        0    25166 2023-03-22 22:32:23.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/run.py
--rw-rw-rw-   0        0        0      186 2023-02-06 17:58:18.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/test.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:19:53.687933 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/
--rw-rw-rw-   0        0        0      775 2023-05-06 03:19:51.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-06 03:19:52.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:19:52.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-06 03:19:52.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-06-19 21:38:13.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2023-05-06 03:19:52.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-06 03:19:52.000000 combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 03:19:53.803478 combine_gtfs_feeds-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-05-06 03:16:00.000000 combine_gtfs_feeds-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:38:46.500077 combine_gtfs_feeds-0.1.7/
+-rw-rw-rw-   0        0        0     1106 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      775 2023-05-06 03:38:46.500077 combine_gtfs_feeds-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-02-04 22:54:46.000000 combine_gtfs_feeds-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 03:38:46.379407 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/
+-rw-rw-rw-   0        0        0       55 2022-06-19 21:37:15.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:38:46.495252 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/
+-rw-rw-rw-   0        0        0       79 2023-02-05 03:16:30.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/__init__.py
+-rw-rw-rw-   0        0        0      937 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/cli.py
+-rw-rw-rw-   0        0        0     7284 2023-02-06 23:13:16.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/gtfs_schema.py
+-rw-rw-rw-   0        0        0     1115 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/log_controller.py
+-rw-rw-rw-   0        0        0      424 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/main.py
+-rw-rw-rw-   0        0        0    25166 2023-03-22 22:32:23.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/run.py
+-rw-rw-rw-   0        0        0      186 2023-02-06 17:58:18.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/test.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:38:46.437540 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-06 03:38:46.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-06-19 21:38:13.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 03:38:46.500077 combine_gtfs_feeds-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-05-06 03:38:21.000000 combine_gtfs_feeds-0.1.7/setup.py
```

### Comparing `combine_gtfs_feeds-0.1.6/LICENSE` & `combine_gtfs_feeds-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.6/PKG-INFO` & `combine_gtfs_feeds-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combine_gtfs_feeds
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package to combine GTFS feeds.
 Home-page: https://github.com/psrc/combine_gtfs_feeds
 Author: psrc staff
 Author-email: scoe@psrc.org
 License: MIT
 Keywords: GTFS
 Platform: UNKNOWN
```

### Comparing `combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/cli.py` & `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/cli.py`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/gtfs_schema.py` & `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/gtfs_schema.py`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/log_controller.py` & `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/log_controller.py`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.6/combine_gtfs_feeds/cli/run.py` & `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/run.py`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/PKG-INFO` & `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combine-gtfs-feeds
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package to combine GTFS feeds.
 Home-page: https://github.com/psrc/combine_gtfs_feeds
 Author: psrc staff
 Author-email: scoe@psrc.org
 License: MIT
 Keywords: GTFS
 Platform: UNKNOWN
```

### Comparing `combine_gtfs_feeds-0.1.6/combine_gtfs_feeds.egg-info/SOURCES.txt` & `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.6/setup.py` & `combine_gtfs_feeds-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     to combine multiple gtfs feeds into a single feed/dataset. \
     The main purpose of combine_gtfs_tools is to be able work \
     from one GTFS feed when performing transit service analysis \
     for a particular geographic location."
 
 setup(
     name="combine_gtfs_feeds",
-    version="0.1.6",
+    version="0.1.7",
     author="psrc staff",
     author_email="scoe@psrc.org",
     url="https://github.com/psrc/combine_gtfs_feeds",
     description="Package to combine GTFS feeds.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

