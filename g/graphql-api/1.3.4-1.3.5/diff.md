# Comparing `tmp/graphql-api-1.3.4.tar.gz` & `tmp/graphql-api-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.3.4.tar", last modified: Fri May  5 23:11:38 2023, max compression
+gzip compressed data, was "graphql-api-1.3.5.tar", last modified: Sat May  6 01:37:09 2023, max compression
```

## Comparing `graphql-api-1.3.4.tar` & `graphql-api-1.3.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 23:11:38.222506 graphql-api-1.3.4/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-05 23:11:28.000000 graphql-api-1.3.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-05 23:11:28.000000 graphql-api-1.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 23:11:38.222506 graphql-api-1.3.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-05 23:11:28.000000 graphql-api-1.3.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-05 23:11:37.000000 graphql-api-1.3.4/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 23:11:38.217506 graphql-api-1.3.4/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3382 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    23879 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     3372 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5674 2023-05-05 23:11:28.000000 graphql-api-1.3.4/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 23:11:38.218506 graphql-api-1.3.4/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 23:11:38.000000 graphql-api-1.3.4/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-05 23:11:38.000000 graphql-api-1.3.4/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 23:11:38.000000 graphql-api-1.3.4/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-05 23:11:38.000000 graphql-api-1.3.4/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 23:11:38.000000 graphql-api-1.3.4/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-05 23:11:38.223506 graphql-api-1.3.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-05 23:11:28.000000 graphql-api-1.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 23:11:38.222506 graphql-api-1.3.4/tests/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5129 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_custom_types.py
--rwxrwxrwx   0 root         (0) root         (0)     5183 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_docstrings.py
--rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_error.py
--rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_filtering.py
--rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_graphql.py
--rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_relay.py
--rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-05 23:11:28.000000 graphql-api-1.3.4/tests/test_subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:37:09.025891 graphql-api-1.3.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-06 01:36:58.000000 graphql-api-1.3.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-06 01:36:58.000000 graphql-api-1.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-06 01:37:09.025891 graphql-api-1.3.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-06 01:36:58.000000 graphql-api-1.3.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-06 01:37:08.000000 graphql-api-1.3.5/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:37:09.019890 graphql-api-1.3.5/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3422 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    24042 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    32869 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     3372 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5896 2023-05-06 01:36:58.000000 graphql-api-1.3.5/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:37:09.021890 graphql-api-1.3.5/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-06 01:37:08.000000 graphql-api-1.3.5/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-06 01:37:09.025891 graphql-api-1.3.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-06 01:36:58.000000 graphql-api-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:37:09.024891 graphql-api-1.3.5/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5129 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_custom_types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5183 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-06 01:36:58.000000 graphql-api-1.3.5/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.3.4/LICENSE` & `graphql-api-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/PKG-INFO` & `graphql-api-1.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.4
+Version: 1.3.5
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.4/graphql-api-v1.3.4.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.5/graphql-api-v1.3.5.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.4/README.md` & `graphql-api-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/api.py` & `graphql-api-1.3.5/graphql_api/api.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/context.py` & `graphql-api-1.3.5/graphql_api/context.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.5/graphql_api/dataclass_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     GraphQLType,
     GraphQLObjectType,
     GraphQLField,
     GraphQLInputField,
     GraphQLNonNull,
 )
 
-from graphql_api.utils import to_camel_case
+from graphql_api.utils import to_camel_case, to_camel_case_text
 
 
 def type_is_dataclass(_class: Type):
     try:
         from dataclasses import is_dataclass
     except ImportError:
         return False
@@ -68,15 +68,15 @@
 
                     return resolver
 
                 description = None
 
                 for docstring_param in docstrings.params:
                     if docstring_param.arg_name == prop_name:
-                        description = docstring_param.description
+                        description = to_camel_case_text(docstring_param.description)
 
                 type_: GraphQLType = local_mapper.map(type_=field_type)
 
                 nullable = False
 
                 if typing_inspect.is_union_type(field_type):
                     union_args = typing_inspect.get_args(field_type, evaluate=True)
```

### Comparing `graphql-api-1.3.4/graphql_api/error.py` & `graphql-api-1.3.5/graphql_api/error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/executor.py` & `graphql-api-1.3.5/graphql_api/executor.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/mapper.py` & `graphql-api-1.3.5/graphql_api/mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,20 @@
     GraphQLUUID,
     GraphQLDateTime,
     GraphQLJSON,
     JsonType,
     GraphQLMappedEnumType,
 )
 
-from graphql_api.utils import to_camel_case, to_snake_case, to_input_value
+from graphql_api.utils import (
+    to_camel_case,
+    to_snake_case,
+    to_input_value,
+    to_camel_case_text,
+)
 from graphql_api.exception import GraphQLBaseException
 from graphql_api.dataclass_mapping import type_is_dataclass, type_from_dataclass
 
 """
 class AnyObject:
 
 
@@ -112,15 +117,15 @@
         self.schema = schema
 
     def types(self) -> Set[GraphQLType]:
         return set(self.registry.values())
 
     def map_to_field(self, function_type: Callable, name="", key="") -> GraphQLField:
         type_hints = typing.get_type_hints(function_type)
-        description = inspect.getdoc(function_type)
+        description = to_camel_case_text(inspect.getdoc(function_type))
 
         return_type = type_hints.pop("return", None)
 
         if not return_type:
             raise GraphQLTypeMapInvalid(
                 f"Field '{name}.{key}' with function ({function_type}) did "
                 f"not specify a valid return type."
@@ -289,15 +294,15 @@
 
     # noinspection PyMethodMayBeStatic
     def map_to_enum(self, type_: Type[enum.Enum]) -> GraphQLEnumType:
         enum_type = type_
         name = f"{type_.__name__}Enum"
         # Enums don't include a suffix as they are immutable
 
-        description = inspect.getdoc(enum_type)
+        description = to_camel_case_text(inspect.getdoc(enum_type))
 
         enum_type = GraphQLMappedEnumType(
             name=name, values=enum_type, description=description
         )
 
         enum_type.enum_type = type_
 
@@ -354,15 +359,15 @@
         for subclass in subclasses:
             if not is_abstract(subclass, self.schema):
                 self.map(subclass)
 
         class_funcs = get_class_funcs(class_type, self.schema, self.as_mutable)
 
         interface_name = f"{name}{self.suffix}Interface"
-        description = inspect.getdoc(class_type)
+        description = to_camel_case_text(inspect.getdoc(class_type))
 
         def local_resolve_type():
             local_self = self
 
             # noinspection PyUnusedLocal
             def resolve_type(value, info, _type):
                 value = local_self.map(type(value))
@@ -405,15 +410,17 @@
             func = creator
 
         else:
             creator = class_type
             # noinspection PyTypeChecker
             func = class_type.__init__
 
-        description = inspect.getdoc(func) or inspect.getdoc(class_type)
+        description = to_camel_case_text(
+            inspect.getdoc(func) or inspect.getdoc(class_type)
+        )
 
         try:
             type_hints = typing.get_type_hints(func)
         except Exception as err:
             raise TypeError(
                 f"Unable to build input type '{name}' for '{class_type}', "
                 f"check the '{class_type}.__init__' method or the "
@@ -477,15 +484,15 @@
             fields=local_fields(),
             out_type=local_container_type(),
             description=description,
         )
 
     def map_to_object(self, class_type: Type) -> GraphQLType:
         name = f"{class_type.__name__}{self.suffix}"
-        description = inspect.getdoc(class_type)
+        description = to_camel_case_text(inspect.getdoc(class_type))
 
         class_funcs = get_class_funcs(class_type, self.schema, self.as_mutable)
 
         for key, func in class_funcs:
             func_meta = get_value(func, self.schema, "meta")
             func_meta["type"] = get_value(func, self.schema, "type")
```

### Comparing `graphql-api-1.3.4/graphql_api/middleware.py` & `graphql-api-1.3.5/graphql_api/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/reduce.py` & `graphql-api-1.3.5/graphql_api/reduce.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/relay.py` & `graphql-api-1.3.5/graphql_api/relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/remote.py` & `graphql-api-1.3.5/graphql_api/remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/types.py` & `graphql-api-1.3.5/graphql_api/types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/graphql_api/utils.py` & `graphql-api-1.3.5/graphql_api/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,23 @@
 # From this response in Stackoverflow
 # http://stackoverflow.com/a/1176023/1072990
 def to_snake_case(name):
     s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
     return re.sub("([a-z0-9])([A-Z])", r"\1_\2", s1).lower()
 
 
+def to_camel_case_text(text: str):
+    if not text:
+        return text
+    for word in text.split():
+        if "_" in word and word.islower():
+            text = text.replace(word, to_camel_case(word))
+    return text
+
+
 def to_input_value(value):
     from graphql_api.mapper import is_scalar
 
     if value is None:
         return None
 
     python_type = type(value)
```

### Comparing `graphql-api-1.3.4/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.5/graphql_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.4
+Version: 1.3.5
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.4/graphql-api-v1.3.4.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.5/graphql-api-v1.3.5.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.4/graphql_api.egg-info/SOURCES.txt` & `graphql-api-1.3.5/graphql_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/setup.py` & `graphql-api-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_custom_types.py` & `graphql-api-1.3.5/tests/test_custom_types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_docstrings.py` & `graphql-api-1.3.5/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_error.py` & `graphql-api-1.3.5/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_filtering.py` & `graphql-api-1.3.5/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_graphql.py` & `graphql-api-1.3.5/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_relay.py` & `graphql-api-1.3.5/tests/test_relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_remote.py` & `graphql-api-1.3.5/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_schema.py` & `graphql-api-1.3.5/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.4/tests/test_subscriptions.py` & `graphql-api-1.3.5/tests/test_subscriptions.py`

 * *Files identical despite different names*

