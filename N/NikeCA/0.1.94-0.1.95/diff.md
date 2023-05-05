# Comparing `tmp/NikeCA-0.1.94.tar.gz` & `tmp/NikeCA-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.94.tar", last modified: Fri May  5 21:54:58 2023, max compression
+gzip compressed data, was "NikeCA-0.1.95.tar", last modified: Fri May  5 22:41:47 2023, max compression
```

## Comparing `NikeCA-0.1.94.tar` & `NikeCA-0.1.95.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:54:58.522671 NikeCA-0.1.94/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.94/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-05 21:54:58.522407 NikeCA-0.1.94/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.94/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-05 21:54:58.522753 NikeCA-0.1.94/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-05 21:54:38.000000 NikeCA-0.1.94/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:54:58.517064 NikeCA-0.1.94/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:54:58.518141 NikeCA-0.1.94/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3966 2023-05-04 22:56:58.000000 NikeCA-0.1.94/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:54:58.518926 NikeCA-0.1.94/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:54:58.520275 NikeCA-0.1.94/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6139 2023-05-05 21:54:19.000000 NikeCA-0.1.94/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 21:54:58.522029 NikeCA-0.1.94/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-05 21:54:58.000000 NikeCA-0.1.94/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-05 21:54:58.000000 NikeCA-0.1.94/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-05 21:54:58.000000 NikeCA-0.1.94/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-05 21:54:58.000000 NikeCA-0.1.94/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-05 21:54:58.000000 NikeCA-0.1.94/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23789 2023-05-05 04:24:30.000000 NikeCA-0.1.94/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.94/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.94/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.94/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 22:41:47.226207 NikeCA-0.1.95/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.95/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-05 22:41:47.225862 NikeCA-0.1.95/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.95/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-05 22:41:47.226288 NikeCA-0.1.95/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-05 22:41:39.000000 NikeCA-0.1.95/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 22:41:47.219871 NikeCA-0.1.95/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 22:41:47.220868 NikeCA-0.1.95/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3966 2023-05-04 22:56:58.000000 NikeCA-0.1.95/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 22:41:47.221878 NikeCA-0.1.95/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 22:41:47.223394 NikeCA-0.1.95/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6125 2023-05-05 22:38:40.000000 NikeCA-0.1.95/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-05 22:41:47.225263 NikeCA-0.1.95/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-05 22:41:47.000000 NikeCA-0.1.95/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-05 22:41:47.000000 NikeCA-0.1.95/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-05 22:41:47.000000 NikeCA-0.1.95/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-05 22:41:47.000000 NikeCA-0.1.95/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-05 22:41:47.000000 NikeCA-0.1.95/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    24039 2023-05-05 22:40:39.000000 NikeCA-0.1.95/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.95/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.95/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.95/src/__init__.py
```

### Comparing `NikeCA-0.1.94/LICENSE` & `NikeCA-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/PKG-INFO` & `NikeCA-0.1.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.94
+Version: 0.1.95
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.94/README.md` & `NikeCA-0.1.95/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/setup.py` & `NikeCA-0.1.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.94',
+	version='0.1.95',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.94/src/Dashboards/Dashboards.py` & `NikeCA-0.1.95/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.95/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.95/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.95/src/Dashboards/Telemetry/Telemetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 from ProductUsage import ProductUsage
 
 
-class Telemetry(ProductUsage):
+class Telemetry:
 
     ProductUsage = ProductUsage
 
     def telemetry_product_viewed(self
                        , username: str
                        , warehouse: str
                        , database: str
```

### Comparing `NikeCA-0.1.94/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.95/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.94
+Version: 0.1.95
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.94/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.95/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.95/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/NikeQA.py` & `NikeCA-0.1.95/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/NikeSF.py` & `NikeCA-0.1.95/src/NikeSF.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pandas as pd
 
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
 from Dashboards.Dashboards import Dashboards
-from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
-from Dashboards.Telemetry.Telemetry import Telemetry
-from Dashboards.Telemetry.ProductUsage import ProductUsage
+# from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
+# from Dashboards.Telemetry.Telemetry import Telemetry
 
 
-class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery):#, InclusionExclusion):
+class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery):
+    # , InclusionExclusion):
 
     Dashboards = Dashboards
-    Telemetry = Telemetry
-    ProductUsage = ProductUsage
+    Dashboards.Telemetry = Dashboards.Telemetry
+    Dashboards.Telemetry.ProductUsage = Dashboards.Telemetry.ProductUsage
+    Dashboards.InclusionExclusion = Dashboards.InclusionExclusion
 
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
@@ -571,18 +572,18 @@
         if database is None:
             database = self.__database
         if role is None:
             role = self.__role
         if polars is False:
             polars = self.__polars
 
-        return InclusionExclusion.pos_data_quality_review(self, username=username, warehouse=warehouse,
-                                                          database=database, role=role, columns=columns,
-                                                          filters=filters, order_by=order_by, polars=polars,
-                                                          start_date=start_date, end_date=end_date)
+        return Dashboards.InclusionExclusion.pos_data_quality_review(self, username=username, warehouse=warehouse,
+                                                                     database=database, role=role, columns=columns,
+                                                                     filters=filters, order_by=order_by, polars=polars,
+                                                                     start_date=start_date, end_date=end_date)
 
     def summary(self
                 , username: str = None
                 , warehouse: str = None
                 , database: str = None
                 , role: str = None
                 , columns=None
@@ -600,17 +601,17 @@
         if database is None:
             database = self.__database
         if role is None:
             role = self.__role
         if polars is False:
             polars = self.__polars
 
-        return InclusionExclusion.summary(self, username=username, warehouse=warehouse, database=database, role=role,
-                                          columns=columns, filters=filters, order_by=order_by, polars=polars,
-                                          start_date=start_date, end_date=end_date)
+        return Dashboards.InclusionExclusion.summary(self, username=username, warehouse=warehouse, database=database,
+                                                     role=role, columns=columns, filters=filters, order_by=order_by,
+                                                     polars=polars, start_date=start_date, end_date=end_date)
 
     def home_summary(self
                      , username: str = None
                      , warehouse: str = None
                      , database: str = None
                      , role: str = None
                      , columns=None
@@ -628,11 +629,13 @@
         if database is None:
             database = self.__database
         if role is None:
             role = self.__role
         if polars is False:
             polars = self.__polars
 
-        return InclusionExclusion.home_summary(self, username=username, warehouse=warehouse, database=database,
-                                               role=role, columns=columns, filters=filters, order_by=order_by,
-                                               polars=polars, start_date=start_date, end_date=end_date)
+        return Dashboards.InclusionExclusion.home_summary(self, username=username, warehouse=warehouse,
+                                                          database=database, role=role, columns=columns,
+                                                          filters=filters, order_by=order_by, polars=polars,
+                                                          start_date=start_date, end_date=end_date)
+
```

### Comparing `NikeCA-0.1.94/src/_BuildSearchQuery.py` & `NikeCA-0.1.95/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/_GitHub.py` & `NikeCA-0.1.95/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/_QA.py` & `NikeCA-0.1.95/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/_SearchFiles.py` & `NikeCA-0.1.95/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/_SnowflakeData.py` & `NikeCA-0.1.95/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/_SnowflakeDependencies.py` & `NikeCA-0.1.95/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.94/src/_SnowflakePull.py` & `NikeCA-0.1.95/src/_SnowflakePull.py`

 * *Files identical despite different names*

