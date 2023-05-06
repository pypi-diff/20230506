# Comparing `tmp/jsonschema_gentypes-2.2.2.tar.gz` & `tmp/jsonschema_gentypes-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_gentypes-2.2.2.tar", max compression
+gzip compressed data, was "jsonschema_gentypes-2.2.3.tar", max compression
```

## Comparing `jsonschema_gentypes-2.2.2.tar` & `jsonschema_gentypes-2.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1304 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/LICENSE
--rw-r--r--   0        0        0     3358 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/README.md
--rw-r--r--   0        0        0    21740 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/__init__.py
--rw-r--r--   0        0        0    17327 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/api.py
--rw-r--r--   0        0        0    12980 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_04.py
--rw-r--r--   0        0        0     2574 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_06.py
--rw-r--r--   0        0        0      149 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_07.py
--rw-r--r--   0        0        0     3042 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_2019_09.py
--rw-r--r--   0        0        0     4339 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_2020_12.py
--rw-r--r--   0        0        0    15368 2023-05-06 13:18:40.997998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/cli.py
--rw-r--r--   0        0        0     2538 2023-05-06 13:19:36.710131 jsonschema_gentypes-2.2.2/jsonschema_gentypes/configuration.py
--rw-r--r--   0        0        0     4982 2023-05-06 13:19:39.126134 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_04.py
--rw-r--r--   0        0        0     5251 2023-05-06 13:19:41.306135 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_06.py
--rw-r--r--   0        0        0     5481 2023-05-06 13:19:43.506136 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_07.py
--rw-r--r--   0        0        0     1698 2023-05-06 13:19:45.690137 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09.py
--rw-r--r--   0        0        0     1596 2023-05-06 13:19:51.822139 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
--rw-r--r--   0        0        0      384 2023-05-06 13:19:57.986143 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
--rw-r--r--   0        0        0     1260 2023-05-06 13:19:47.730137 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
--rw-r--r--   0        0        0      296 2023-05-06 13:19:55.950142 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
--rw-r--r--   0        0        0      973 2023-05-06 13:19:49.766138 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
--rw-r--r--   0        0        0     3019 2023-05-06 13:19:53.918140 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
--rw-r--r--   0        0        0     2569 2023-05-06 13:20:00.278145 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12.py
--rw-r--r--   0        0        0     1691 2023-05-06 13:20:06.506147 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
--rw-r--r--   0        0        0      384 2023-05-06 13:20:10.638146 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
--rw-r--r--   0        0        0      859 2023-05-06 13:20:02.334147 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
--rw-r--r--   0        0        0      973 2023-05-06 13:20:04.378147 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
--rw-r--r--   0        0        0     3019 2023-05-06 13:20:08.618147 jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
--rw-r--r--   0        0        0        0 2023-05-06 13:18:41.001998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/py.typed
--rw-r--r--   0        0        0     6112 2023-05-06 13:18:41.001998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/resolver.py
--rw-r--r--   0        0        0     3067 2023-05-06 13:18:41.001998 jsonschema_gentypes-2.2.2/jsonschema_gentypes/schema.json
--rw-r--r--   0        0        0     2514 2023-05-06 13:21:22.290182 jsonschema_gentypes-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/LICENSE
+-rw-r--r--   0        0        0     3358 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/README.md
+-rw-r--r--   0        0        0    21740 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/__init__.py
+-rw-r--r--   0        0        0    17333 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/api.py
+-rw-r--r--   0        0        0    12980 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_04.py
+-rw-r--r--   0        0        0     2574 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_06.py
+-rw-r--r--   0        0        0      149 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_07.py
+-rw-r--r--   0        0        0     3042 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_2019_09.py
+-rw-r--r--   0        0        0     4339 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_2020_12.py
+-rw-r--r--   0        0        0    15368 2023-05-06 13:39:20.564776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/cli.py
+-rw-r--r--   0        0        0     2538 2023-05-06 13:40:52.097660 jsonschema_gentypes-2.2.3/jsonschema_gentypes/configuration.py
+-rw-r--r--   0        0        0     4982 2023-05-06 13:40:54.561687 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_04.py
+-rw-r--r--   0        0        0     5251 2023-05-06 13:40:56.769708 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_06.py
+-rw-r--r--   0        0        0     5481 2023-05-06 13:40:58.977725 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_07.py
+-rw-r--r--   0        0        0     1698 2023-05-06 13:41:01.137741 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09.py
+-rw-r--r--   0        0        0     1596 2023-05-06 13:41:07.353795 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
+-rw-r--r--   0        0        0      384 2023-05-06 13:41:13.589856 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
+-rw-r--r--   0        0        0     1260 2023-05-06 13:41:03.213757 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
+-rw-r--r--   0        0        0      296 2023-05-06 13:41:11.533836 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
+-rw-r--r--   0        0        0      973 2023-05-06 13:41:05.269775 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
+-rw-r--r--   0        0        0     3019 2023-05-06 13:41:09.489816 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
+-rw-r--r--   0        0        0     2569 2023-05-06 13:41:15.853877 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12.py
+-rw-r--r--   0        0        0     1691 2023-05-06 13:41:22.145938 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
+-rw-r--r--   0        0        0      384 2023-05-06 13:41:26.293978 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
+-rw-r--r--   0        0        0      859 2023-05-06 13:41:17.917897 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
+-rw-r--r--   0        0        0      973 2023-05-06 13:41:20.033918 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
+-rw-r--r--   0        0        0     3019 2023-05-06 13:41:24.265958 jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
+-rw-r--r--   0        0        0        0 2023-05-06 13:39:20.568776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/py.typed
+-rw-r--r--   0        0        0     6112 2023-05-06 13:39:20.568776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/resolver.py
+-rw-r--r--   0        0        0     3067 2023-05-06 13:39:20.568776 jsonschema_gentypes-2.2.3/jsonschema_gentypes/schema.json
+-rw-r--r--   0        0        0     2514 2023-05-06 13:42:41.322701 jsonschema_gentypes-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.2.3/PKG-INFO
```

### Comparing `jsonschema_gentypes-2.2.2/LICENSE` & `jsonschema_gentypes-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/README.md` & `jsonschema_gentypes-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/__init__.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/api.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,21 +134,21 @@
             schema,
         )
 
         root = self.root is None
         if root:
             self.root = TypeProxy()
         if schema is True:
-            type_ = NativeType("Any")
+            type_: Type = NativeType("Any")
             if root:
                 assert self.root is not None
                 self.root.set_type(type_)
             return type_
         if schema is False:
-            type_ = NativeType("None")
+            type_ = BuiltinType("None")
             if root:
                 assert self.root is not None
                 self.root.set_type(type_)
             return type_
         assert not isinstance(schema, bool)
 
         proxy = TypeProxy()
@@ -395,15 +395,15 @@
                 return type_
             elif "enum" in schema:
                 return self.enum(schema_validation, proposed_name)
             elif "default" in schema:
                 return self.default(schema_meta_data, proposed_name)
 
         if schema_type is None:
-            type_ = BuiltinType("Any")
+            type_ = NativeType("Any")
             type_.set_comments(["WARNING: we get an schema without any type"])
             return type_
         assert isinstance(schema_type, str), (
             f"Expected to find a supported schema type, got {schema_type}" f"\nDuring parsing of {schema}"
         )
 
         return self._get_type(schema, schema_type, proposed_name)
```

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_04.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_04.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_06.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_06.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_2019_09.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_2019_09.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/api_draft_2020_12.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/api_draft_2020_12.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/cli.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/cli.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/configuration.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/configuration.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_04.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_04.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_06.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_06.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_07.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_07.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_core.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_core.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/resolver.py` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/resolver.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/jsonschema_gentypes/schema.json` & `jsonschema_gentypes-2.2.3/jsonschema_gentypes/schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.2.2/pyproject.toml` & `jsonschema_gentypes-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 strict = true
 
 [tool.poetry]
 name = "jsonschema-gentypes"
-version = "2.2.2"
+version = "2.2.3"
 description = "Tool to generate Python types based on TypedDict from a JSON Schema"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 repository = "https://github.com/camptocamp/jsonschema-gentypes"
 license = "BSD-2-Clause"
 keywords = ["jsonschema", "types"]
 packages = [{ include = "jsonschema_gentypes" }]
```

### Comparing `jsonschema_gentypes-2.2.2/PKG-INFO` & `jsonschema_gentypes-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-gentypes
-Version: 2.2.2
+Version: 2.2.3
 Summary: Tool to generate Python types based on TypedDict from a JSON Schema
 Home-page: https://github.com/camptocamp/jsonschema-gentypes
 License: BSD-2-Clause
 Keywords: jsonschema,types
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4
```

