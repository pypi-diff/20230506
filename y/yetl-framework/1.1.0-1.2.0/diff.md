# Comparing `tmp/yetl-framework-1.1.0.tar.gz` & `tmp/yetl-framework-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.1.0.tar", last modified: Sat May  6 17:04:38 2023, max compression
+gzip compressed data, was "yetl-framework-1.2.0.tar", last modified: Sat May  6 19:21:55 2023, max compression
```

## Comparing `yetl-framework-1.1.0.tar` & `yetl-framework-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 17:04:38.675783 yetl-framework-1.1.0/
--rw-r--r--   0 vsts      (1001) docker     (123)     5825 2023-05-06 17:04:38.675783 yetl-framework-1.1.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5328 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 17:04:38.675783 yetl-framework-1.1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 17:04:38.675783 yetl-framework-1.1.0/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      502 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7505 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7666 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 17:04:38.675783 yetl-framework-1.1.0/yetl/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      325 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3298 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1551 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 17:04:38.675783 yetl-framework-1.1.0/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 17:03:43.000000 yetl-framework-1.1.0/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 17:04:38.675783 yetl-framework-1.1.0/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5825 2023-05-06 17:04:38.000000 yetl-framework-1.1.0/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-06 17:04:38.000000 yetl-framework-1.1.0/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 17:04:38.000000 yetl-framework-1.1.0/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 17:04:38.000000 yetl-framework-1.1.0/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 17:04:38.000000 yetl-framework-1.1.0/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 17:04:38.000000 yetl-framework-1.1.0/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.369877 yetl-framework-1.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-06 19:21:55.369877 yetl-framework-1.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 19:21:55.369877 yetl-framework-1.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.365877 yetl-framework-1.2.0/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      502 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7505 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7913 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.365877 yetl-framework-1.2.0/yetl/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      325 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4123 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1551 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.365877 yetl-framework-1.2.0/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 19:21:07.000000 yetl-framework-1.2.0/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 19:21:55.369877 yetl-framework-1.2.0/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5741 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      717 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 19:21:55.000000 yetl-framework-1.2.0/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.1.0/PKG-INFO` & `yetl-framework-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.1.0
+Version: 1.2.0
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -135,24 +135,23 @@
       checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
-from yetl import Config, Timeslice, StageType
+from yetl import Config, StageType
 
 pipeline = "auto_load_schema"
 project = "test_project"
-timeslice = Timeslice(day="*", month="*", year="*")
 config = Config(
     project=project, pipeline=pipeline
 )
 table_mapping = config.get_table_mapping(
-    timeslice=timeslice, stage=StageType.raw, table="customers"
+    stage=StageType.raw, table="customers"
 )
 
 print(table_mapping)
 ```
 
 Use even less code and use the decorator pattern:
```

### Comparing `yetl-framework-1.1.0/README.md` & `yetl-framework-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,24 +120,23 @@
       checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
-from yetl import Config, Timeslice, StageType
+from yetl import Config, StageType
 
 pipeline = "auto_load_schema"
 project = "test_project"
-timeslice = Timeslice(day="*", month="*", year="*")
 config = Config(
     project=project, pipeline=pipeline
 )
 table_mapping = config.get_table_mapping(
-    timeslice=timeslice, stage=StageType.raw, table="customers"
+    stage=StageType.raw, table="customers"
 )
 
 print(table_mapping)
 ```
 
 Use even less code and use the decorator pattern:
```

### Comparing `yetl-framework-1.1.0/setup.py` & `yetl-framework-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.1.0",
+    version="1.2.0",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.1.0/yetl/_config.py` & `yetl-framework-1.2.0/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/_decorators.py` & `yetl-framework-1.2.0/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/_logging_config.py` & `yetl-framework-1.2.0/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/_project.py` & `yetl-framework-1.2.0/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/_spark_context.py` & `yetl-framework-1.2.0/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/_tables.py` & `yetl-framework-1.2.0/yetl/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/_timeslice.py` & `yetl-framework-1.2.0/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/_utils.py` & `yetl-framework-1.2.0/yetl/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 class JinjaVariables(Enum):
     DATABASE = "database"
     TABLE = "table"
     CHECKPOINT = "checkpoint"
     FILENAME_DATE_FORMAT = "filename_date_format"
     PATH_DATE_FORMAT = "path_date_format"
     CONTAINER = "container"
+    DELTA_PROPERTIES = "delta_properties"
+    LOCATION = "location"
 
 
 def is_databricks():
     return "DATABRICKS_RUNTIME_VERSION" in os.environ
 
 
 def check_version(data: dict):
@@ -127,14 +129,23 @@
                 problem = f"{e.problem}."
 
             raise Exception(f"Invalid yaml format in {path}. {problem} {location}")
     _logger.debug(data)
     return data
 
 
+def load_text(path: str):
+    _logger = logging.getLogger(__name__)
+    _logger.info(f"Loading text file {path}")
+    with open(path, "r", encoding=_ENCODING) as f:
+        data = f.read()
+    _logger.debug(data)
+    return data
+
+
 def get_ddl(spark_schema: StructType, header: bool = True):
     _logger = logging.getLogger(__name__)
     _logger.debug(f"Converting spark schema to ddl with header={str(header)}")
     if header:
         ddl = [f"{f.name} {f.dataType.simpleString()}" for f in spark_schema.fields]
         _logger.debug(ddl)
     else:
```

### Comparing `yetl-framework-1.1.0/yetl/deltalake.py` & `yetl-framework-1.2.0/yetl/deltalake.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from pyspark.sql import DataFrame
 import logging
 from pyspark.sql.types import StructType, StructField
 import jinja2
-from typing import List
+from typing import List, Union, Dict
 from ._spark_context import get_spark_context
 from pydantic import BaseModel, Field
 from typing import Any
 from ._project import Project
 from pyspark.sql import SparkSession
 
 
@@ -38,43 +38,48 @@
             self.spark.sql(f"SHOW TABLES in {database};")
             .where(f"tableName='{table}' AND !isTemporary")
             .count()
             == 1
         )
         return table_exists
 
+    def get_delta_properties_sql(self, delta_properties: Dict[str, Union[str, bool]]):
+        sql_properties = [
+            f"{k.lower()} = {v.lower()}" for k, v in delta_properties.items()
+        ]
+        sql_properties = ", ".join(sql_properties)
+        return sql_properties
+
     def create_table(
         self,
         database: str,
         table: str,
         path: str = None,
         delta_properties: List[str] = None,
         sql: str = None,
     ):
         _logger.debug(f"Creating table if not exists {database}.{table} at {path}")
 
         if not sql:
             sql = f"CREATE TABLE IF NOT EXISTS `{database}`.`{table}`"
 
-        # add in the delta properties if there are any
-        sql_properties = ""
-        if delta_properties:
-            sql_properties = [
-                f"{k.lower()} = {v.lower()}" for k, v in delta_properties.items()
-            ]
-            sql_properties = ", ".join(sql_properties)
-            sql_properties = f"TBLPROPERTIES({sql_properties})"
-
-        sql_path = ""
-        if path:
-            sql_path = f"USING DELTA LOCATION '{path}'"
+            # add in the delta properties if there are any
+            sql_properties = ""
+            if delta_properties:
+                sql_properties = self.get_delta_properties_sql(delta_properties)
+                sql_properties = f"TBLPROPERTIES({sql_properties})"
+
+            sql_path = ""
+            if path:
+                sql_path = f"USING DELTA LOCATION '{path}'"
 
-            sql = f"{sql}\n{sql_path}\n{sql_properties};"
+                sql = f"{sql}\n{sql_path}\n{sql_properties};"
 
         _logger.debug(f"{sql}")
+        print(sql)
         self.spark.sql(sql)
 
         return sql
 
     def create_database(self, database: str):
         _logger.debug(f"Creating database if not exists `{database}`")
         sql = f"CREATE DATABASE IF NOT EXISTS {database}"
```

### Comparing `yetl-framework-1.1.0/yetl/table/_deltalake.py` & `yetl-framework-1.2.0/yetl/table/_deltalake.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import logging
 from pydantic import Field, PrivateAttr
-from .._utils import JinjaVariables, render_jinja, is_databricks
+from .._utils import (
+    JinjaVariables,
+    render_jinja,
+    is_databricks,
+    abs_config_path,
+    load_text,
+)
 from typing import Any, Dict, Union, List
 from .._timeslice import Timeslice
 import os
 from .._stage_type import StageType
 from ._table import Table
 from ..deltalake import DeltaLakeFn
 
@@ -16,17 +22,18 @@
 #     pass
 
 
 class DeltaLake(Table):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
-        self._render()
         self._spark = DeltaLakeFn(project=self.project)
-        self.create_delta_table()
+        self._render()
+        if self.create_table:
+            self.create_delta_table()
 
     @classmethod
     def in_allowed_stages(cls, stage: StageType):
         return stage in (stage.raw, stage.base, stage.curated)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
@@ -41,47 +48,67 @@
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
     checkpoint_location: str = Field(default=None)
     stage: StageType = Field(...)
     managed: bool = Field(default=False)
     create_table: bool = Field(default=True)
+    sql: str = Field(default=None)
+
+    def _load_sql(self, path: str):
+        path = abs_config_path(self.config_path, path)
+        sql = load_text(path)
+        return sql
 
     def _render(self):
         self._replacements = {
             JinjaVariables.TABLE: self.table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
         }
-
-        self.location = render_jinja(self.location, self._replacements)
-        self.path = render_jinja(self.path, self._replacements)
+        if self.delta_properties:
+            delta_properties_sql = self._spark.get_delta_properties_sql(
+                self.delta_properties
+            )
+            self._replacements[JinjaVariables.DELTA_PROPERTIES] = delta_properties_sql
         self.database = render_jinja(self.database, self._replacements)
         self.table = render_jinja(self.table, self._replacements)
-        if self.options:
-            for option, value in self.options.items():
-                self.options[option] = render_jinja(value, self._replacements)
-
+        self.location = render_jinja(self.location, self._replacements)
+        self.path = render_jinja(self.path, self._replacements)
         self.location = os.path.join(self.location, self.path)
         if not is_databricks():
             self.location = f"{self.config_path}/../data{self.location}"
             self.location = os.path.abspath(self.location)
+        self._replacements[JinjaVariables.LOCATION] = self.location
+
+        if self.options:
+            for option, value in self.options.items():
+                self.options[option] = render_jinja(value, self._replacements)
+
+        if self.sql:
+            # render the path
+            self.sql = render_jinja(self.sql, self._replacements)
+            # load the file
+            self.sql = self._load_sql(self.sql)
+            # render the SQL
+            self.sql = render_jinja(self.sql, self._replacements)
 
+    # TODO: Create or alter table
     def create_delta_table(self):
-        database_table = f"`{self.database}`.`{self.table}`"
-        self._logger.info(f"Creating delta lake table {database_table}")
         self._spark.create_database(self.database)
 
         if self.managed:
             self._spark.create_table(
                 database=self.database,
                 table=self.table,
                 delta_properties=self.delta_properties,
+                sql=self.sql,
             )
         else:
             self._spark.create_table(
                 database=self.database,
                 table=self.table,
                 delta_properties=self.delta_properties,
                 path=self.location,
+                sql=self.sql,
             )
```

### Comparing `yetl-framework-1.1.0/yetl/table/_factory.py` & `yetl-framework-1.2.0/yetl/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/table/_read.py` & `yetl-framework-1.2.0/yetl/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/table/_table.py` & `yetl-framework-1.2.0/yetl/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.2.0/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.1.0/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.2.0/yetl_framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.1.0
+Version: 1.2.0
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
@@ -135,24 +135,23 @@
       checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
-from yetl import Config, Timeslice, StageType
+from yetl import Config, StageType
 
 pipeline = "auto_load_schema"
 project = "test_project"
-timeslice = Timeslice(day="*", month="*", year="*")
 config = Config(
     project=project, pipeline=pipeline
 )
 table_mapping = config.get_table_mapping(
-    timeslice=timeslice, stage=StageType.raw, table="customers"
+    stage=StageType.raw, table="customers"
 )
 
 print(table_mapping)
 ```
 
 Use even less code and use the decorator pattern:
```

### Comparing `yetl-framework-1.1.0/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.2.0/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

