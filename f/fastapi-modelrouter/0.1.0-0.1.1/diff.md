# Comparing `tmp/fastapi-modelrouter-0.1.0.tar.gz` & `tmp/fastapi-modelrouter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-modelrouter-0.1.0.tar", last modified: Thu May  4 18:37:10 2023, max compression
+gzip compressed data, was "fastapi-modelrouter-0.1.1.tar", last modified: Sat May  6 21:18:24 2023, max compression
```

## Comparing `fastapi-modelrouter-0.1.0.tar` & `fastapi-modelrouter-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 18:37:10.060375 fastapi-modelrouter-0.1.0/
--rw-rw-r--   0 windt     (1000) windt     (1000)     1065 2023-05-02 17:18:03.000000 fastapi-modelrouter-0.1.0/LICENSE
--rw-rw-r--   0 windt     (1000) windt     (1000)     2204 2023-05-04 18:37:10.060375 fastapi-modelrouter-0.1.0/PKG-INFO
--rw-rw-r--   0 windt     (1000) windt     (1000)     1384 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.0/README.md
--rw-rw-r--   0 windt     (1000) windt     (1000)      103 2023-05-04 18:37:10.060375 fastapi-modelrouter-0.1.0/setup.cfg
--rw-rw-r--   0 windt     (1000) windt     (1000)     1497 2023-05-04 18:37:02.000000 fastapi-modelrouter-0.1.0/setup.py
-drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 18:37:10.056375 fastapi-modelrouter-0.1.0/src/
-drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 18:37:10.056375 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/
--rw-rw-r--   0 windt     (1000) windt     (1000)     2204 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/PKG-INFO
--rw-rw-r--   0 windt     (1000) windt     (1000)      366 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/SOURCES.txt
--rw-rw-r--   0 windt     (1000) windt     (1000)        1 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/dependency_links.txt
--rw-rw-r--   0 windt     (1000) windt     (1000)       19 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/requires.txt
--rw-rw-r--   0 windt     (1000) windt     (1000)       12 2023-05-04 18:37:10.000000 fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/top_level.txt
-drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-04 18:37:10.060375 fastapi-modelrouter-0.1.0/src/modelrouter/
--rw-rw-r--   0 windt     (1000) windt     (1000)      141 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.0/src/modelrouter/__init__.py
--rw-rw-r--   0 windt     (1000) windt     (1000)     2061 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.0/src/modelrouter/model_to_pydantic.py
--rw-rw-r--   0 windt     (1000) windt     (1000)     9725 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.0/src/modelrouter/modelrouter.py
+drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-06 21:18:24.966723 fastapi-modelrouter-0.1.1/
+-rw-rw-r--   0 windt     (1000) windt     (1000)     1065 2023-05-02 17:18:03.000000 fastapi-modelrouter-0.1.1/LICENSE
+-rw-rw-r--   0 windt     (1000) windt     (1000)     2225 2023-05-06 21:18:24.966723 fastapi-modelrouter-0.1.1/PKG-INFO
+-rw-rw-r--   0 windt     (1000) windt     (1000)     1405 2023-05-04 20:27:04.000000 fastapi-modelrouter-0.1.1/README.md
+-rw-rw-r--   0 windt     (1000) windt     (1000)      103 2023-05-06 21:18:24.966723 fastapi-modelrouter-0.1.1/setup.cfg
+-rw-rw-r--   0 windt     (1000) windt     (1000)     1497 2023-05-06 21:12:50.000000 fastapi-modelrouter-0.1.1/setup.py
+drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-06 21:18:24.962723 fastapi-modelrouter-0.1.1/src/
+drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-06 21:18:24.962723 fastapi-modelrouter-0.1.1/src/fastapi_modelrouter.egg-info/
+-rw-rw-r--   0 windt     (1000) windt     (1000)     2225 2023-05-06 21:18:24.000000 fastapi-modelrouter-0.1.1/src/fastapi_modelrouter.egg-info/PKG-INFO
+-rw-rw-r--   0 windt     (1000) windt     (1000)      366 2023-05-06 21:18:24.000000 fastapi-modelrouter-0.1.1/src/fastapi_modelrouter.egg-info/SOURCES.txt
+-rw-rw-r--   0 windt     (1000) windt     (1000)        1 2023-05-06 21:18:24.000000 fastapi-modelrouter-0.1.1/src/fastapi_modelrouter.egg-info/dependency_links.txt
+-rw-rw-r--   0 windt     (1000) windt     (1000)       19 2023-05-06 21:18:24.000000 fastapi-modelrouter-0.1.1/src/fastapi_modelrouter.egg-info/requires.txt
+-rw-rw-r--   0 windt     (1000) windt     (1000)       12 2023-05-06 21:18:24.000000 fastapi-modelrouter-0.1.1/src/fastapi_modelrouter.egg-info/top_level.txt
+drwxrwxr-x   0 windt     (1000) windt     (1000)        0 2023-05-06 21:18:24.966723 fastapi-modelrouter-0.1.1/src/modelrouter/
+-rw-rw-r--   0 windt     (1000) windt     (1000)      141 2023-05-04 18:30:10.000000 fastapi-modelrouter-0.1.1/src/modelrouter/__init__.py
+-rw-rw-r--   0 windt     (1000) windt     (1000)     2353 2023-05-06 18:47:55.000000 fastapi-modelrouter-0.1.1/src/modelrouter/model_to_pydantic.py
+-rw-rw-r--   0 windt     (1000) windt     (1000)     9737 2023-05-06 21:12:16.000000 fastapi-modelrouter-0.1.1/src/modelrouter/modelrouter.py
```

### Comparing `fastapi-modelrouter-0.1.0/LICENSE` & `fastapi-modelrouter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-modelrouter-0.1.0/PKG-INFO` & `fastapi-modelrouter-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-modelrouter
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI Router that creates CRUD routes for SqlAlchemy models
 Home-page: https://github.com/UweWindt/fastapi-modelrouter
 Author: Uwe Windt
 Author-email: uwe.windt@windisoft.de
 License: MIT
 Keywords: fastapi router sqlalchemy development
 Classifier: Development Status :: 3 - Alpha
@@ -25,26 +25,27 @@
 
 ### Features
 
 - Generates direct from SqlAlchemy Models CRUD routes
 - no need to write Pydantic Basemodels
 - keep SqlAlchemy Models and routes in sync
 - Simple to Use
-- Composite primary key
+- Supports composite primary keys
+- Supports queryparams
 
 
 ## Installation
 ```
 pip install fastapi-modelrouter
 ```
 
 ## Basic Usage
 ```
 from fastapi import FastAPI
-from modelrouter.modelrouter import ModelRouter
+from modelrouter import ModelRouter
 
 # setup Sqlalchemy Database
 from sqlalchemy import create_engine, Column, String, Integer
 from sqlalchemy.orm import sessionmaker, declarative_base
 
 sqlalchemy_database_url = "sqlite:///:memory"
```

### Comparing `fastapi-modelrouter-0.1.0/README.md` & `fastapi-modelrouter-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 
 ### Features
 
 - Generates direct from SqlAlchemy Models CRUD routes
 - no need to write Pydantic Basemodels
 - keep SqlAlchemy Models and routes in sync
 - Simple to Use
-- Composite primary key
+- Supports composite primary keys
+- Supports queryparams
 
 
 ## Installation
 ```
 pip install fastapi-modelrouter
 ```
 
 ## Basic Usage
 ```
 from fastapi import FastAPI
-from modelrouter.modelrouter import ModelRouter
+from modelrouter import ModelRouter
 
 # setup Sqlalchemy Database
 from sqlalchemy import create_engine, Column, String, Integer
 from sqlalchemy.orm import sessionmaker, declarative_base
 
 sqlalchemy_database_url = "sqlite:///:memory"
```

### Comparing `fastapi-modelrouter-0.1.0/setup.py` & `fastapi-modelrouter-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fastapi-modelrouter',
-    version='0.1.0',
+    version='0.1.1',
     license='MIT',
     description='FastAPI Router that creates CRUD routes for SqlAlchemy models',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Uwe Windt",
     author_email='uwe.windt@windisoft.de',
     packages=find_packages('src'),
```

### Comparing `fastapi-modelrouter-0.1.0/src/fastapi_modelrouter.egg-info/PKG-INFO` & `fastapi-modelrouter-0.1.1/src/fastapi_modelrouter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-modelrouter
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI Router that creates CRUD routes for SqlAlchemy models
 Home-page: https://github.com/UweWindt/fastapi-modelrouter
 Author: Uwe Windt
 Author-email: uwe.windt@windisoft.de
 License: MIT
 Keywords: fastapi router sqlalchemy development
 Classifier: Development Status :: 3 - Alpha
@@ -25,26 +25,27 @@
 
 ### Features
 
 - Generates direct from SqlAlchemy Models CRUD routes
 - no need to write Pydantic Basemodels
 - keep SqlAlchemy Models and routes in sync
 - Simple to Use
-- Composite primary key
+- Supports composite primary keys
+- Supports queryparams
 
 
 ## Installation
 ```
 pip install fastapi-modelrouter
 ```
 
 ## Basic Usage
 ```
 from fastapi import FastAPI
-from modelrouter.modelrouter import ModelRouter
+from modelrouter import ModelRouter
 
 # setup Sqlalchemy Database
 from sqlalchemy import create_engine, Column, String, Integer
 from sqlalchemy.orm import sessionmaker, declarative_base
 
 sqlalchemy_database_url = "sqlite:///:memory"
```

### Comparing `fastapi-modelrouter-0.1.0/src/modelrouter/model_to_pydantic.py` & `fastapi-modelrouter-0.1.1/src/modelrouter/model_to_pydantic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Container, Optional, Type, Any
 
 from pydantic import BaseConfig, BaseModel, create_model
+from pydantic.fields import FieldInfo
 from sqlalchemy.inspection import inspect
 
 
 class OrmConfig(BaseConfig):
     orm_mode = True
 
 
@@ -50,11 +51,16 @@
         elif hasattr(column.type, "python_type"):
             python_type = column.type.python_type
         assert python_type, f"Could not infer python_type for {column}"
         default = None
         if not force_optional:
             if column.default is None and not column.nullable:
                 default = ...
-        fields[column.name] = (python_type, default)
+            # else:
+            #     default = column.default
+        if hasattr(column.type, "length") and column.type.length:
+            fields[column.name] = (python_type, FieldInfo(max_length=column.type.length, default=default))
+        else:
+            fields[column.name] = (python_type, default)
     basemodel_name = name if name != '' else model.__name__
     basemodel: Type[BaseModel] = create_model(basemodel_name, __config__=OrmConfig, **fields)  # type: ignore
     return basemodel
```

### Comparing `fastapi-modelrouter-0.1.0/src/modelrouter/modelrouter.py` & `fastapi-modelrouter-0.1.1/src/modelrouter/modelrouter.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,20 @@
         self.db_model: Type[Model] = db_model
         self.db: CALLABLE_SESSION = db
         self.schema: Type[BaseModel] = model_to_pydantic(db_model)
         self.queryparams_schema: Type[BaseModel] = model_to_pydantic(db_model,
                                                                      name=db_model.__name__ + 'queryParams',
                                                                      force_optional=True)
         self.create_schema: Type[BaseModel] = model_to_pydantic(db_model,
-                                                                name=db_model.__name__ + 'Create')
+                                                                name=db_model.__name__ + '_Create')
         self.pk_schema: Type[BaseModel] = model_to_pydantic(db_model,
-                                                            name=db_model.__name__ + 'Pk',
+                                                            name=db_model.__name__ + '_Primary_Key',
                                                             only_pk=True)
         self.nonpk_schema: Type[BaseModel] = model_to_pydantic(db_model,
-                                                               name=db_model.__name__ + 'body',
+                                                               name=db_model.__name__ + '_Body',
                                                                exclude_pk=True)
 
         prefix = prefix if prefix != "" else "/" + db_model.__name__.lower()
         print(prefix)
         super().__init__(prefix=prefix, tags=tags, **kwargs)
 
         if get_all_route:
```

