# Comparing `tmp/NikeCA-0.1.96b0.tar.gz` & `tmp/NikeCA-0.1.96rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.96b0.tar", last modified: Fri May  5 23:50:02 2023, max compression
+gzip compressed data, was "NikeCA-0.1.96rc0.tar", last modified: Fri May  5 23:57:06 2023, max compression
```

## Comparing `NikeCA-0.1.96b0.tar` & `NikeCA-0.1.96rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:50:02.409203 NikeCA-0.1.96b0/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.96b0/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18014 2023-05-05 23:50:02.408749 NikeCA-0.1.96b0/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.96b0/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-05 23:50:02.409315 NikeCA-0.1.96b0/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-05-05 23:49:33.000000 NikeCA-0.1.96b0/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:50:02.402233 NikeCA-0.1.96b0/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:50:02.403890 NikeCA-0.1.96b0/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3966 2023-05-04 22:56:58.000000 NikeCA-0.1.96b0/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:50:02.404777 NikeCA-0.1.96b0/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:50:02.406200 NikeCA-0.1.96b0/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6179 2023-05-05 23:41:19.000000 NikeCA-0.1.96b0/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:50:02.408153 NikeCA-0.1.96b0/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18014 2023-05-05 23:50:02.000000 NikeCA-0.1.96b0/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-05 23:50:02.000000 NikeCA-0.1.96b0/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-05 23:50:02.000000 NikeCA-0.1.96b0/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-05 23:50:02.000000 NikeCA-0.1.96b0/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-05 23:50:02.000000 NikeCA-0.1.96b0/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    24409 2023-05-05 23:49:18.000000 NikeCA-0.1.96b0/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.96b0/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.96b0/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.96b0/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:57:06.216230 NikeCA-0.1.96rc0/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.96rc0/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18015 2023-05-05 23:57:06.215839 NikeCA-0.1.96rc0/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.96rc0/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-05 23:57:06.216454 NikeCA-0.1.96rc0/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-05-05 23:57:02.000000 NikeCA-0.1.96rc0/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:57:06.208007 NikeCA-0.1.96rc0/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:57:06.209568 NikeCA-0.1.96rc0/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3966 2023-05-04 22:56:58.000000 NikeCA-0.1.96rc0/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:57:06.210821 NikeCA-0.1.96rc0/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:57:06.212550 NikeCA-0.1.96rc0/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6190 2023-05-05 23:56:48.000000 NikeCA-0.1.96rc0/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 23:57:06.215242 NikeCA-0.1.96rc0/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18015 2023-05-05 23:57:06.000000 NikeCA-0.1.96rc0/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-05 23:57:06.000000 NikeCA-0.1.96rc0/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-05 23:57:06.000000 NikeCA-0.1.96rc0/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-05 23:57:06.000000 NikeCA-0.1.96rc0/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-05 23:57:06.000000 NikeCA-0.1.96rc0/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    24409 2023-05-05 23:49:18.000000 NikeCA-0.1.96rc0/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.96rc0/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.96rc0/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.96rc0/src/__init__.py
```

### Comparing `NikeCA-0.1.96b0/LICENSE` & `NikeCA-0.1.96rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/PKG-INFO` & `NikeCA-0.1.96rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.96b0
+Version: 0.1.96rc0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.96b0/README.md` & `NikeCA-0.1.96rc0/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/setup.py` & `NikeCA-0.1.96rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.96b',
+	version='0.1.96c',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.96b0/src/Dashboards/Dashboards.py` & `NikeCA-0.1.96rc0/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.96rc0/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.96rc0/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.96rc0/src/Dashboards/Telemetry/Telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                        , filters: list | None = None
                        , order_by: list | None = None
                        , polars: bool = False
                        , start_date: str = '1900-01-01'
                        , end_date: str = '9999-12-31'
                        ):
 
-        from NikeCA import Snowflake
+        from src.NikeCA import Snowflake
         import polars as pl
         import configparser
 
         config = configparser.ConfigParser()
         config.read('pip.ini')
 
         b = config['telemetry_product_usage'].get('col_b')
@@ -69,15 +69,15 @@
             """
 
         df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
                                     role=role).snowflake_pull(query=query, polars=polars))
 
         print(query)
 
-        return
+        return df
 
     def telemetry_get_base_query(self
                        , filters: list | None = None
                        , start_date: str = '1900-01-01'
                        , end_date: str = '9999-12-31'
                        ):
 
@@ -170,15 +170,15 @@
         FROM (
             {self.telemetry_get_base_query(start_date=start_date, end_date=end_date, filters=filters)}   
         )
         ORDER BY
             {order_by}
     """
 
-        from NikeCA import Snowflake
+        from src.NikeCA import Snowflake
         import polars as pl
 
         df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
                                     role=role).snowflake_pull(query=query, polars=polars))
 
         print(query)
```

### Comparing `NikeCA-0.1.96b0/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.96rc0/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.96b0
+Version: 0.1.96rc0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.96b0/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.96rc0/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.96rc0/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/NikeQA.py` & `NikeCA-0.1.96rc0/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/NikeSF.py` & `NikeCA-0.1.96rc0/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/_BuildSearchQuery.py` & `NikeCA-0.1.96rc0/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/_GitHub.py` & `NikeCA-0.1.96rc0/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/_QA.py` & `NikeCA-0.1.96rc0/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/_SearchFiles.py` & `NikeCA-0.1.96rc0/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/_SnowflakeData.py` & `NikeCA-0.1.96rc0/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/_SnowflakeDependencies.py` & `NikeCA-0.1.96rc0/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.96b0/src/_SnowflakePull.py` & `NikeCA-0.1.96rc0/src/_SnowflakePull.py`

 * *Files identical despite different names*

