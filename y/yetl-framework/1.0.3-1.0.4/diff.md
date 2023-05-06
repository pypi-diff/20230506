# Comparing `tmp/yetl-framework-1.0.3.tar.gz` & `tmp/yetl-framework-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.0.3.tar", last modified: Sat May  6 06:50:17 2023, max compression
+gzip compressed data, was "yetl-framework-1.0.4.tar", last modified: Sat May  6 07:48:17 2023, max compression
```

## Comparing `yetl-framework-1.0.3.tar` & `yetl-framework-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 06:50:17.846305 yetl-framework-1.0.3/
--rw-r--r--   0 vsts      (1001) docker     (123)     5817 2023-05-06 06:50:17.846305 yetl-framework-1.0.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5320 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 06:50:17.846305 yetl-framework-1.0.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 06:50:17.846305 yetl-framework-1.0.3/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      503 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3220 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7313 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 06:50:17.846305 yetl-framework-1.0.3/yetl/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      261 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1268 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3425 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4032 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/dataset/_write.py
--rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/dataset/dataset_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7666 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 06:50:17.846305 yetl-framework-1.0.3/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 06:49:25.000000 yetl-framework-1.0.3/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 06:50:17.846305 yetl-framework-1.0.3/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5817 2023-05-06 06:50:17.000000 yetl-framework-1.0.3/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-06 06:50:17.000000 yetl-framework-1.0.3/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 06:50:17.000000 yetl-framework-1.0.3/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 06:50:17.000000 yetl-framework-1.0.3/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 06:50:17.000000 yetl-framework-1.0.3/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 06:50:17.000000 yetl-framework-1.0.3/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5817 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5320 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.815434 yetl-framework-1.0.4/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      504 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3220 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      186 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7313 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/yetl/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1692 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3425 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4032 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4839 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/dataset/dataset_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7666 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-06 07:47:19.000000 yetl-framework-1.0.4/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-06 07:48:17.819434 yetl-framework-1.0.4/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5817 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-06 07:48:17.000000 yetl-framework-1.0.4/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.0.3/PKG-INFO` & `yetl-framework-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.0.3
+Version: 1.0.4
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.0.3/README.md` & `yetl-framework-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/setup.py` & `yetl-framework-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.0.3",
+    version="1.0.4",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.0.3/yetl/_config.py` & `yetl-framework-1.0.4/yetl/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/_decorators.py` & `yetl-framework-1.0.4/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/_logging_config.py` & `yetl-framework-1.0.4/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/_project.py` & `yetl-framework-1.0.4/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/_spark_context.py` & `yetl-framework-1.0.4/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/_tables.py` & `yetl-framework-1.0.4/yetl/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/_timeslice.py` & `yetl-framework-1.0.4/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/_utils.py` & `yetl-framework-1.0.4/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/dataset/_dataset.py` & `yetl-framework-1.0.4/yetl/dataset/_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,36 @@
 from typing import Any, Dict, Union, List
 from .._timeslice import Timeslice
 from .._stage_type import StageType
 from .dataset_type import TableType
 from .._project import Project
 
 
+class ValidationThreshold(BaseModel):
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+
+    invalid_ratio: float = Field(default=None)
+    invalid_rows: int = Field(default=None)
+    max_rows: int = Field(default=None)
+    min_rows: int = Field(default=None)
+
+
 class Table(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     stage: StageType = Field(...)
     database: str = Field(...)
     table: str = Field(...)
     id: Union[str, List[str]] = Field(default=[])
     custom_properties: Dict[str, Any] = Field(default=None)
     table_type: TableType = Field(...)
+    warning_thresholds: ValidationThreshold = Field(default=None)
+    exception_thresholds: ValidationThreshold = Field(default=None)
 
     def _render(self):
         pass
 
 
 class DataSet(BaseModel):
     def __init__(self, **data: Any) -> None:
```

### Comparing `yetl-framework-1.0.3/yetl/dataset/_deltalake.py` & `yetl-framework-1.0.4/yetl/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/dataset/_factory.py` & `yetl-framework-1.0.4/yetl/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/dataset/_read.py` & `yetl-framework-1.0.4/yetl/dataset/_read.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from pydantic import Field, PrivateAttr, BaseModel
+from pydantic import Field, PrivateAttr
 from .._utils import JinjaVariables, render_jinja, get_ddl, load_schema, abs_config_path
 from typing import Any, Dict, List, Union
 from enum import Enum
 import os
 from pyspark.sql.types import StructType
 from pyspark.sql.streaming import StreamingQuery
 from pyspark.sql import DataFrame
@@ -11,30 +11,18 @@
 from ._dataset import DataSet, Table
 
 
 class TriggerType(Enum):
     File = "file"
 
 
-class ValidationThreshold(BaseModel):
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    invalid_ratio: float = Field(default=None)
-    invalid_rows: int = Field(default=None)
-    max_rows: int = Field(default=None)
-    min_rows: int = Field(default=None)
-
-
 class ReadTable(Table):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
-    warning_thresholds: ValidationThreshold = Field(default=None)
-    exception_thresholds: ValidationThreshold = Field(default=None)
     create_table: bool = Field(default=True)
     managed: bool = Field(default=False)
 
 
 class Read(DataSet, ReadTable):
     _OPTION_CF_SCHEMA_HINTS = "cloudFiles.schemaHints"
     _OPTION_CORRUPT_RECORD_NAME = "columnNameOfCorruptRecord"
```

### Comparing `yetl-framework-1.0.3/yetl/deltalake.py` & `yetl-framework-1.0.4/yetl/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.0.4/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.3/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.0.4/yetl_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.0.3
+Version: 1.0.4
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.0.3/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.0.4/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

