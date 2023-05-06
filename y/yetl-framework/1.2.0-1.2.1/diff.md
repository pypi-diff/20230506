# Comparing `tmp/yetl-framework-1.2.0.tar.gz` & `tmp/yetl-framework-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.2.0.tar", last modified: Sat May  6 19:21:55 2023, max compression
+gzip compressed data, was "yetl-framework-1.2.1.tar", last modified: Sat May  6 20:01:48 2023, max compression
```

## Comparing `yetl-framework-1.2.0.tar` & `yetl-framework-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.369877 yetl-framework-1.2.0/
--rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-06 19:21:55.369877 yetl-framework-1.2.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 19:21:55.369877 yetl-framework-1.2.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.365877 yetl-framework-1.2.0/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      502 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7505 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.365877 yetl-framework-1.2.0/yetl/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      325 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4123 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1551 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.365877 yetl-framework-1.2.0/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.369877 yetl-framework-1.2.0/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 20:01:48.499185 yetl-framework-1.2.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-06 20:01:48.499185 yetl-framework-1.2.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 20:01:48.499185 yetl-framework-1.2.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 20:01:48.495185 yetl-framework-1.2.1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      502 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7497 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 20:01:48.495185 yetl-framework-1.2.1/yetl/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      325 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4123 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1551 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 20:01:48.495185 yetl-framework-1.2.1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 20:00:52.000000 yetl-framework-1.2.1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 20:01:48.499185 yetl-framework-1.2.1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-06 20:01:48.000000 yetl-framework-1.2.1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-06 20:01:48.000000 yetl-framework-1.2.1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 20:01:48.000000 yetl-framework-1.2.1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 20:01:48.000000 yetl-framework-1.2.1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 20:01:48.000000 yetl-framework-1.2.1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 20:01:48.000000 yetl-framework-1.2.1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.2.0/PKG-INFO` & `yetl-framework-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.0
+Version: 1.2.1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.2.0/README.md` & `yetl-framework-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/setup.py` & `yetl-framework-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.2.0",
+    version="1.2.1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.2.0/yetl/_config.py` & `yetl-framework-1.2.1/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/_decorators.py` & `yetl-framework-1.2.1/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/_logging_config.py` & `yetl-framework-1.2.1/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/_project.py` & `yetl-framework-1.2.1/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/_spark_context.py` & `yetl-framework-1.2.1/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/_tables.py` & `yetl-framework-1.2.1/yetl/_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     def _parse_configuration(self):
         push_down_properties = {}
         for stage_name, table_type in self.table_data["tables"].items():
             stage_type = StageType(stage_name)
             for table_type_name, database in table_type.items():
                 table_type = TableType(table_type_name)
                 for database_name, table in database.items():
+                    push_down_properties = {}
                     if PushDownProperties.has_not_value(database_name):
                         for table_name, table_propties in table.items():
                             table_config = {
                                 KeyContants.DATABASE.value: database_name,
                                 KeyContants.TABLE.value: table_name,
                                 KeyContants.STAGE.value: stage_type,
                                 KeyContants.TABLE_TYPE.value: table_type,
@@ -73,15 +74,14 @@
                                 else:
                                     table_config[p] = v
                             stage_config = self.table_data.get(stage_type.value, {})
                             stage_config = stage_config.get(table_type.value, {})
                             table_config = {**stage_config, **table_config}
                             index = f"{stage_name}.{database_name}.{table_name}"
                             self.tables_index[index] = table_config
-                            push_down_properties = {}
                     else:
                         push_down_properties[database_name] = table
 
     table_data: dict = Field(...)
     tables_index: Dict[str, Table] = Field(default={})
     delta_properties: Dict[str, str] = Field(default=None)
```

### Comparing `yetl-framework-1.2.0/yetl/_timeslice.py` & `yetl-framework-1.2.1/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/_utils.py` & `yetl-framework-1.2.1/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/deltalake.py` & `yetl-framework-1.2.1/yetl/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/table/_deltalake.py` & `yetl-framework-1.2.1/yetl/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/table/_factory.py` & `yetl-framework-1.2.1/yetl/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/table/_read.py` & `yetl-framework-1.2.1/yetl/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/table/_table.py` & `yetl-framework-1.2.1/yetl/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.2.1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.2.0/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.2.1/yetl_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.2.0
+Version: 1.2.1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.2.0/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.2.1/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

