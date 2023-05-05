# Comparing `tmp/bigraph-schema-0.0.6.tar.gz` & `tmp/bigraph-schema-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigraph-schema-0.0.6.tar", last modified: Mon Apr 24 01:31:22 2023, max compression
+gzip compressed data, was "bigraph-schema-0.0.7.tar", last modified: Fri May  5 23:02:52 2023, max compression
```

## Comparing `bigraph-schema-0.0.6.tar` & `bigraph-schema-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      378 2023-04-24 01:31:10.000000 bigraph-schema-0.0.6/README.md
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/bigraph_schema/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      106 2023-04-19 21:19:48.000000 bigraph-schema-0.0.6/bigraph_schema/__init__.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.6/bigraph_schema/parse.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      919 2023-04-20 03:53:50.000000 bigraph-schema-0.0.6/bigraph_schema/protocol.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18353 2023-04-24 01:15:10.000000 bigraph-schema-0.0.6/bigraph_schema/registry.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    19757 2023-04-24 01:30:22.000000 bigraph-schema-0.0.6/bigraph_schema/schema.py
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/bigraph_schema.egg-info/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      337 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       25 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/requires.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/top_level.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/setup.cfg
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1327 2023-04-24 01:30:56.000000 bigraph-schema-0.0.6/setup.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      378 2023-04-24 01:31:10.000000 bigraph-schema-0.0.7/README.md
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/bigraph_schema/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      106 2023-04-19 21:19:48.000000 bigraph-schema-0.0.7/bigraph_schema/__init__.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.7/bigraph_schema/parse.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      919 2023-04-20 03:53:50.000000 bigraph-schema-0.0.7/bigraph_schema/protocol.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18894 2023-05-05 23:00:46.000000 bigraph-schema-0.0.7/bigraph_schema/registry.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    19757 2023-05-05 23:00:52.000000 bigraph-schema-0.0.7/bigraph_schema/schema.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/bigraph_schema.egg-info/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      337 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       25 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/requires.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-05-05 23:02:52.000000 bigraph-schema-0.0.7/bigraph_schema.egg-info/top_level.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-05-05 23:02:52.869993 bigraph-schema-0.0.7/setup.cfg
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1327 2023-05-05 23:02:36.000000 bigraph-schema-0.0.7/setup.py
```

### Comparing `bigraph-schema-0.0.6/PKG-INFO` & `bigraph-schema-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.6
+Version: 0.0.7
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.6/bigraph_schema/parse.py` & `bigraph-schema-0.0.7/bigraph_schema/parse.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.6/bigraph_schema/protocol.py` & `bigraph-schema-0.0.7/bigraph_schema/protocol.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.6/bigraph_schema/registry.py` & `bigraph-schema-0.0.7/bigraph_schema/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,17 +205,16 @@
 
 
     def substitute_type(self, schema):
         if isinstance(schema, str):
             schema = self.access(schema)
         elif '_type' in schema:
             type_key = schema['_type']
-            type_schema = self.access(type_key)
-            type_schema = copy.deepcopy(type_schema)
-            schema.update(type_schema)
+            type_schema = copy.deepcopy(self.access(type_key))
+            schema = deep_merge(type_schema, schema)
 
         return schema
 
 
     def expand_schema(self, schema):
         # make this only show the types at the leaves
 
@@ -233,15 +232,15 @@
 
     def generate_default(self, schema):
         default = None
 
         if isinstance(schema, str):
             schema = self.access(schema)
         elif '_type' in schema:
-            schema = self.access(schema['_type'])
+            schema = self.substitute_type(schema)
 
         if '_default' in schema:
             if not '_deserialize' in schema:
                 raise Exception(
                     f'asking for default for {type_key} but no deserialize in {schema}')
             deserialize = deserialize_registry.access(
                 schema['_deserialize'])
@@ -386,29 +385,40 @@
     return result
 
 
 def replace(old_value, new_value):
     return new_value
 
 
+# TODO: make these work
+def serialize_dict(value):
+    return value
+
+
+def deserialize_dict(value):
+    return value
+
+
 # validate the function registered is of the right type?
 apply_registry.register('accumulate', accumulate)
 apply_registry.register('concatenate', concatenate)
 apply_registry.register('replace', replace)
 apply_registry.register('merge', deep_merge)
 divide_registry.register('divide_float', divide_float)
 divide_registry.register('divide_int', divide_int)
 divide_registry.register('divide_longest', divide_longest)
 divide_registry.register('divide_list', divide_list)
 divide_registry.register('divide_dict', divide_dict)
 serialize_registry.register('str', str)
+serialize_registry.register('serialize_dict', serialize_dict)
 deserialize_registry.register('float', float)
 deserialize_registry.register('int', int)
 deserialize_registry.register('str', str)
 deserialize_registry.register('eval', eval)
+deserialize_registry.register('deserialize_dict', deserialize_dict)
 
 # if super type is re-registered, propagate changes to subtypes (?)
 
 # remove shape types
 type_library = {
     # abstract number type
     'number': {
@@ -459,14 +469,24 @@
         '_serialize': 'str',
         '_deserialize': 'eval',
         '_divide': 'divide_dict',
         '_type_parameters': ['A'],
         '_description': 'mapping from str to some type (or nested dicts)'
     },
 
+    'dict': {
+        '_default': '{}',
+        '_apply': 'merge',
+        '_serialize': 'serialize_dict',
+        '_deserialize': 'deserialize_dict',
+        '_divide': 'divide_dict',
+        '_type_parameters': ['key', 'value'],
+        '_description': 'mapping from keys of any type to values of any type'
+    },
+
     'edge': {
         'wires': {
             '_type': 'hash[list[string]]'
         },
     },
 
     # 'process': {
```

### Comparing `bigraph-schema-0.0.6/bigraph_schema/schema.py` & `bigraph-schema-0.0.7/bigraph_schema/schema.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.6/bigraph_schema.egg-info/PKG-INFO` & `bigraph-schema-0.0.7/bigraph_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.6
+Version: 0.0.7
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigraph-schema-0.0.6/setup.py` & `bigraph-schema-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
 
 
 setup(
```

