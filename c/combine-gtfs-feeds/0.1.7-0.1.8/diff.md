# Comparing `tmp/combine_gtfs_feeds-0.1.7.tar.gz` & `tmp/combine_gtfs_feeds-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combine_gtfs_feeds-0.1.7.tar", last modified: Sat May  6 03:38:46 2023, max compression
+gzip compressed data, was "combine_gtfs_feeds-0.1.8.tar", last modified: Sat May  6 15:14:02 2023, max compression
```

## Comparing `combine_gtfs_feeds-0.1.7.tar` & `combine_gtfs_feeds-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:38:46.500077 combine_gtfs_feeds-0.1.7/
--rw-rw-rw-   0        0        0     1106 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      775 2023-05-06 03:38:46.500077 combine_gtfs_feeds-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-02-04 22:54:46.000000 combine_gtfs_feeds-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 03:38:46.379407 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/
--rw-rw-rw-   0        0        0       55 2022-06-19 21:37:15.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:38:46.495252 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/
--rw-rw-rw-   0        0        0       79 2023-02-05 03:16:30.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/__init__.py
--rw-rw-rw-   0        0        0      937 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/cli.py
--rw-rw-rw-   0        0        0     7284 2023-02-06 23:13:16.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/gtfs_schema.py
--rw-rw-rw-   0        0        0     1115 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/log_controller.py
--rw-rw-rw-   0        0        0      424 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/main.py
--rw-rw-rw-   0        0        0    25166 2023-03-22 22:32:23.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/run.py
--rw-rw-rw-   0        0        0      186 2023-02-06 17:58:18.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/test.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:38:46.437540 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/
--rw-rw-rw-   0        0        0      775 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-06 03:38:46.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-06-19 21:38:13.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-06 03:38:45.000000 combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 03:38:46.500077 combine_gtfs_feeds-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-05-06 03:38:21.000000 combine_gtfs_feeds-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:14:02.326697 combine_gtfs_feeds-0.1.8/
+-rw-rw-rw-   0        0        0     1106 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      775 2023-05-06 15:14:02.324994 combine_gtfs_feeds-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-02-04 22:54:46.000000 combine_gtfs_feeds-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 15:14:02.249740 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/
+-rw-rw-rw-   0        0        0       55 2022-06-19 21:37:15.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:14:02.318162 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/
+-rw-rw-rw-   0        0        0       79 2023-02-05 03:16:30.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/__init__.py
+-rw-rw-rw-   0        0        0      937 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/cli.py
+-rw-rw-rw-   0        0        0     7294 2023-05-06 04:42:10.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/gtfs_schema.py
+-rw-rw-rw-   0        0        0     1115 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/log_controller.py
+-rw-rw-rw-   0        0        0      424 2022-06-19 21:33:26.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/main.py
+-rw-rw-rw-   0        0        0    25166 2023-03-22 22:32:23.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/run.py
+-rw-rw-rw-   0        0        0      186 2023-02-06 17:58:18.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/test.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:14:02.281104 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-05-06 15:14:01.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-06 15:14:02.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 15:14:01.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-06 15:14:01.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-06-19 21:38:13.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2023-05-06 15:14:01.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-06 15:14:01.000000 combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 15:14:02.328497 combine_gtfs_feeds-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-05-06 15:12:56.000000 combine_gtfs_feeds-0.1.8/setup.py
```

### Comparing `combine_gtfs_feeds-0.1.7/LICENSE` & `combine_gtfs_feeds-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.7/PKG-INFO` & `combine_gtfs_feeds-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combine_gtfs_feeds
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package to combine GTFS feeds.
 Home-page: https://github.com/psrc/combine_gtfs_feeds
 Author: psrc staff
 Author-email: scoe@psrc.org
 License: MIT
 Keywords: GTFS
 Platform: UNKNOWN
```

### Comparing `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/cli.py` & `combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/cli.py`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/gtfs_schema.py` & `combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/gtfs_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     class Stops(pa.SchemaModel):
         stop_id: Series[str] = pa.Field(coerce=True)
         stop_code: Optional[Series[str]] = pa.Field(coerce=True, nullable=True)
         stop_name: Series[str] = pa.Field(coerce=True)
         stop_desc: Optional[Series[str]] = pa.Field(coerce=True, nullable=True)
         stop_lat: Series[float64] = pa.Field(coerce=True, nullable=True)
         stop_lon: Series[float64] = pa.Field(coerce=True, nullable=True)
-        zone_id: Series[str] = pa.Field(coerce=True, nullable=True)
+        zone_id: Optional[Series[str]] = pa.Field(coerce=True, nullable=True)
         stop_url: Optional[Series[str]] = pa.Field(coerce=True, nullable=True)
         location_type: Optional[Series[pd.Int64Dtype]] = pa.Field(
             coerce=True, nullable=True, isin=[0, 1, 2, 3, 4]
         )
         parent_station: Optional[Series[str]] = pa.Field(coerce=True, nullable=True)
         stop_timezone: Optional[Series[str]] = pa.Field(coerce=True, nullable=True)
         wheelchair_boarding: Optional[Series[pd.Int64Dtype]] = pa.Field(
```

### Comparing `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/log_controller.py` & `combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/log_controller.py`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds/cli/run.py` & `combine_gtfs_feeds-0.1.8/combine_gtfs_feeds/cli/run.py`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/PKG-INFO` & `combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combine-gtfs-feeds
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package to combine GTFS feeds.
 Home-page: https://github.com/psrc/combine_gtfs_feeds
 Author: psrc staff
 Author-email: scoe@psrc.org
 License: MIT
 Keywords: GTFS
 Platform: UNKNOWN
```

### Comparing `combine_gtfs_feeds-0.1.7/combine_gtfs_feeds.egg-info/SOURCES.txt` & `combine_gtfs_feeds-0.1.8/combine_gtfs_feeds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `combine_gtfs_feeds-0.1.7/setup.py` & `combine_gtfs_feeds-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     to combine multiple gtfs feeds into a single feed/dataset. \
     The main purpose of combine_gtfs_tools is to be able work \
     from one GTFS feed when performing transit service analysis \
     for a particular geographic location."
 
 setup(
     name="combine_gtfs_feeds",
-    version="0.1.7",
+    version="0.1.8",
     author="psrc staff",
     author_email="scoe@psrc.org",
     url="https://github.com/psrc/combine_gtfs_feeds",
     description="Package to combine GTFS feeds.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

