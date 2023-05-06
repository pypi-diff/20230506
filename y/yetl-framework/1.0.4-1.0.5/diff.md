# Comparing `tmp/yetl-framework-1.0.4.tar.gz` & `tmp/yetl-framework-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.0.4.tar", last modified: Sat May  6 07:48:17 2023, max compression
+gzip compressed data, was "yetl-framework-1.0.5.tar", last modified: Sat May  6 07:53:48 2023, max compression
```

## Comparing `yetl-framework-1.0.4.tar` & `yetl-framework-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/
--rw-r--r--   0 vsts      (1001) docker     (123)     5817 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5320 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.815434 yetl-framework-1.0.4/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      504 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3220 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7313 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/yetl/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1692 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3425 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4032 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4839 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_write.py
--rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/dataset_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7666 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5817 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:53:48.464013 yetl-framework-1.0.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5825 2023-05-06 07:53:48.464013 yetl-framework-1.0.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5328 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 07:53:48.464013 yetl-framework-1.0.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:53:48.464013 yetl-framework-1.0.5/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      504 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3220 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7313 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:53:48.464013 yetl-framework-1.0.5/yetl/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1696 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3437 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4032 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4851 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/dataset/dataset_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7666 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:53:48.464013 yetl-framework-1.0.5/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 07:52:57.000000 yetl-framework-1.0.5/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:53:48.464013 yetl-framework-1.0.5/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5825 2023-05-06 07:53:48.000000 yetl-framework-1.0.5/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-06 07:53:48.000000 yetl-framework-1.0.5/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 07:53:48.000000 yetl-framework-1.0.5/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 07:53:48.000000 yetl-framework-1.0.5/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 07:53:48.000000 yetl-framework-1.0.5/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 07:53:48.000000 yetl-framework-1.0.5/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.0.4/PKG-INFO` & `yetl-framework-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.0.4
+Version: 1.0.5
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -88,15 +88,15 @@
 tables: ./tables.yaml
 
 landing: # this is the landing stage in the deltalake house
   read: # this is the type of spark asset that the pipeline needs to read from
     trigger: customerdetailscomplete-{{filename_date_format}}*.flg
     trigger_type: file
     container: datalake
-    root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
+    location: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
     filename: "{{table}}-{{filename_date_format}}*.csv"
     filename_date_format: "%Y%m%d"
     path_date_format: "%Y%m%d"
     format: cloudFiles
     spark_schema: ../schema/{{table.lower()}}.yaml
     options:
       # autoloader
@@ -125,15 +125,15 @@
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
     create_table: true
     container: datalake
-    root: /mnt/{{container}}/data/raw
+    location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
     options:
       checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
```

### Comparing `yetl-framework-1.0.4/README.md` & `yetl-framework-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 tables: ./tables.yaml
 
 landing: # this is the landing stage in the deltalake house
   read: # this is the type of spark asset that the pipeline needs to read from
     trigger: customerdetailscomplete-{{filename_date_format}}*.flg
     trigger_type: file
     container: datalake
-    root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
+    location: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
     filename: "{{table}}-{{filename_date_format}}*.csv"
     filename_date_format: "%Y%m%d"
     path_date_format: "%Y%m%d"
     format: cloudFiles
     spark_schema: ../schema/{{table.lower()}}.yaml
     options:
       # autoloader
@@ -110,15 +110,15 @@
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
     create_table: true
     container: datalake
-    root: /mnt/{{container}}/data/raw
+    location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
     options:
       checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
```

### Comparing `yetl-framework-1.0.4/setup.py` & `yetl-framework-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.0.4",
+    version="1.0.5",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.0.4/yetl/_config.py` & `yetl-framework-1.0.5/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/_decorators.py` & `yetl-framework-1.0.5/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/_logging_config.py` & `yetl-framework-1.0.5/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/_project.py` & `yetl-framework-1.0.5/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/_spark_context.py` & `yetl-framework-1.0.5/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/_tables.py` & `yetl-framework-1.0.5/yetl/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/_timeslice.py` & `yetl-framework-1.0.5/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/_utils.py` & `yetl-framework-1.0.5/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/dataset/_dataset.py` & `yetl-framework-1.0.5/yetl/dataset/_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
     project: Project = Field(...)
     container: str = Field(...)
-    root: str = Field(...)
+    location: str = Field(...)
     path: str = Field(default=None)
     options: dict = Field(...)
     timeslice: Timeslice = Field(...)
     checkpoint: str = Field(default=None)
     config_path: str = Field(...)
 
     def _render(self):
```

### Comparing `yetl-framework-1.0.4/yetl/dataset/_deltalake.py` & `yetl-framework-1.0.5/yetl/dataset/_deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,23 @@
         self._replacements = {
             JinjaVariables.TABLE: self.table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
         }
 
-        self.root = render_jinja(self.root, self._replacements)
+        self.location = render_jinja(self.location, self._replacements)
         self.path = render_jinja(self.path, self._replacements)
         self.database = render_jinja(self.database, self._replacements)
         self.table = render_jinja(self.table, self._replacements)
         if self.options:
             for option, value in self.options.items():
                 self.options[option] = render_jinja(value, self._replacements)
 
-        self.location = os.path.join(self.root, self.path)
+        self.location = os.path.join(self.location, self.path)
         if not is_databricks():
             self.location = f"{self.config_path}/../data{self.location}"
             self.location = os.path.abspath(self.location)
 
     def create_delta_table(self):
         database_table = f"`{self.database}`.`{self.table}`"
         self._logger.info(f"Creating delta lake table {database_table}")
```

### Comparing `yetl-framework-1.0.4/yetl/dataset/_factory.py` & `yetl-framework-1.0.5/yetl/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/dataset/_read.py` & `yetl-framework-1.0.5/yetl/dataset/_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     _OPTION_CF_SCHEMA_HINTS = "cloudFiles.schemaHints"
     _OPTION_CORRUPT_RECORD_NAME = "columnNameOfCorruptRecord"
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._render()
-        self.path = os.path.join(self.root, self.filename)
+        self.path = os.path.join(self.location, self.filename)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
     trigger: str = Field(default=None)
     trigger_type: TriggerType = Field(default=None)
     filename: str = Field(...)
     filename_date_format: str = Field(...)
@@ -56,15 +56,15 @@
             ),
             JinjaVariables.TABLE: self.table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
         }
 
-        self.root = render_jinja(self.root, self._replacements)
+        self.location = render_jinja(self.location, self._replacements)
         self.filename = render_jinja(self.filename, self._replacements)
         self.database = render_jinja(self.database, self._replacements)
         self.table = render_jinja(self.table, self._replacements)
         self.trigger = render_jinja(self.trigger, self._replacements)
 
         if self.options:
             for option, value in self.options.items():
```

### Comparing `yetl-framework-1.0.4/yetl/deltalake.py` & `yetl-framework-1.0.5/yetl/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.0.5/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.4/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.0.5/yetl_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.0.4
+Version: 1.0.5
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -88,15 +88,15 @@
 tables: ./tables.yaml
 
 landing: # this is the landing stage in the deltalake house
   read: # this is the type of spark asset that the pipeline needs to read from
     trigger: customerdetailscomplete-{{filename_date_format}}*.flg
     trigger_type: file
     container: datalake
-    root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
+    location: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
     filename: "{{table}}-{{filename_date_format}}*.csv"
     filename_date_format: "%Y%m%d"
     path_date_format: "%Y%m%d"
     format: cloudFiles
     spark_schema: ../schema/{{table.lower()}}.yaml
     options:
       # autoloader
@@ -125,15 +125,15 @@
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
     managed: false
     create_table: true
     container: datalake
-    root: /mnt/{{container}}/data/raw
+    location: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
     options:
       checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
```

### Comparing `yetl-framework-1.0.4/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.0.5/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

