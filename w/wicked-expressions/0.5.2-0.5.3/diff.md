# Comparing `tmp/wicked_expressions-0.5.2.tar.gz` & `tmp/wicked_expressions-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.5.2.tar", max compression
+gzip compressed data, was "wicked_expressions-0.5.3.tar", max compression
```

## Comparing `wicked_expressions-0.5.2.tar` & `wicked_expressions-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-04-20 20:02:14.128563 wicked_expressions-0.5.2/LICENSE
--rw-r--r--   0        0        0     2119 2023-04-20 20:02:14.128563 wicked_expressions-0.5.2/README.md
--rw-r--r--   0        0        0     1219 2023-04-20 20:03:24.614335 wicked_expressions-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-20 20:03:24.594334 wicked_expressions-0.5.2/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      783 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     7975 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      304 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     8309 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/datastash.bolt
--rw-r--r--   0        0        0     1924 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      341 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8524 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0     3127 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1220 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     5701 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-04-20 20:02:14.136563 wicked_expressions-0.5.2/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-06 20:43:54.704532 wicked_expressions-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2119 2023-05-06 20:43:54.704532 wicked_expressions-0.5.3/README.md
+-rw-r--r--   0        0        0     1219 2023-05-06 20:45:43.303906 wicked_expressions-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-05-06 20:45:43.279905 wicked_expressions-0.5.3/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      783 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     7975 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     8309 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/datastash.bolt
+-rw-r--r--   0        0        0     1850 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      341 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8524 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      596 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1221 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     5253 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-05-06 20:43:54.712532 wicked_expressions-0.5.3/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.5.3/PKG-INFO
```

### Comparing `wicked_expressions-0.5.2/LICENSE` & `wicked_expressions-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.2/README.md` & `wicked_expressions-0.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     - bolt
     - wicked_expressions
 
 pipeline:
     - mecha
 ```
 
-Once you've required `bolt` and `wicked-expressions`, you are able to import the python package's `api` module directly inside your bolt scripts.
+Once you've required `bolt` and `wicked_expressions`, you are able to import the python package's `api` module directly inside your bolt scripts.
 
 ```py
 from wicked_expressions:api import Scoreboard, Data
 ```
 
 Now you're free to use the API objects. Create simple and complex expressions, compare storages with scores, scores with scores, check if scores exist and more.
```

### Comparing `wicked_expressions-0.5.2/pyproject.toml` & `wicked_expressions-0.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.5.2"
+version = "0.5.3"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/comparison.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/datastash.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/datastash.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/internal_api.bolt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any
 import bolt_expressions.node as be_node
 import bolt_expressions.api as be_api
 
 from ./config import Config
+from ./safe_load import safe_load
 import ./sources as sources
 
 
 class Scoreboard(be_api.Scoreboard):
     def objective(self, name: str, criteria: str = 'dummy', prefixed=True, display_name=None):
         if prefixed:
             name = self._expr.opts.objective_prefix + name
@@ -17,21 +18,18 @@
         if name not in self.added_objectives:
             self.added_objectives.add(name)
             self.create_objective(name, criteria, display_name)
 
         return Score(self, name)
 
     def create_objective(self, objective_id: str, criteria: str, display_name: str | dict):
-        setup_path = f"{Config.ROOT_LOCAL}/scoreboard_setup"
-
         if isinstance(display_name, str):
             display_name = display_name
 
-        merge function_tag minecraft:load {"values": [setup_path]}
-        append function setup_path:
+        with safe_load('scoreboard_setup', append=True):
             if display_name is None:
                 scoreboard objectives add objective_id criteria
             else:
                 scoreboard objectives add objective_id criteria display_name
 
 class Score(be_api.Score):
     def __getitem__(self, scoreholder: str | list[str]) -> sources.ScoreSource | list[sources.ScoreSource]:
```

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/sources.bolt`

 * *Files 0% similar despite different names*

```diff
@@ -98,16 +98,7 @@
 def is_comparison_case() -> bool:
     """Determines whether a comparison dunder method call was intended to compare."""
 
     frame = inspect.getouterframes(inspect.currentframe(), 2)[2]
     output = re.compile(r"sources.|optimizer.").search(frame.filename) == None
     # print([' ', '+'][output], frame.filename)
     return output
-
-
-
-
-
-
-
-
-
```

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/var.bolt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List
 
 
 class Var:
     is_static = False
 
     def __new__(self, type_annotation):
-        if type_annotation == Bool:
+        if type_annotation == Bool: 
             return sources.BoolSource.create(is_static=self.is_static)
         elif type_annotation == Byte:
             return sources.ByteSource.create(is_static=self.is_static)
         elif type_annotation == Short:
             return sources.ShortSource.create(is_static=self.is_static)
         elif type_annotation == Int:
             return sources.IntSource.create(is_static=self.is_static)
```

### Comparing `wicked_expressions-0.5.2/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.5.3/wicked_expressions/modules/var_sources.bolt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import base64
 import inspect
 import nbtlib
 
 from ./sources import ScoreSource, DataSource
 from ./utils import logger, defer
 from ./config import Config
+from ./safe_load import safe_load
 
 
 class BaseVar:
     _var_type = ''
     _location_index = -1
     _static_cache = {}
 
@@ -38,64 +39,48 @@
 
     @staticmethod
     def _get_frame_context() -> tuple:
         frame = inspect.getouterframes(inspect.currentframe(), 2)[4]
         path = frame.filename[len(str(ctx.directory)):]
         return (frame.lineno, path)
 
-    @defer
-    @staticmethod
-    def flush_variables_setup():
-        BoolSource._flush_on_load()
-        ByteSource._flush_on_load()
-        ShortSource._flush_on_load()
-        IntSource._flush_on_load()
-        LongSource._flush_on_load()
-        FloatSource._flush_on_load()
-        DoubleSource._flush_on_load()
-        StringSource._flush_on_load()
-        ListSource._flush_on_load()
-
-
 class VarScoreSource(ScoreSource, BaseVar):
     @classmethod
     def create(cls, is_static: bool):
         location_index = cls._evaluate_location_index(is_static)
-        return cls(f"${ctx.project_id}#{cls._var_type}${location_index}", Config.SCOREBOARD_ROOT)
+        full_location = f"${ctx.project_id}#{cls._var_type}${location_index}"
+        
+        cls._setup_flushing(full_location)
+        return cls(full_location, Config.SCOREBOARD_ROOT)
 
     @classmethod
-    def _flush_on_load(cls):
-        mcfunc_path = f"{Config.ROOT_LOCAL}/runtime_var_flush_score"
-
-        for index in range(cls._location_index+1):
-            merge function_tag minecraft:load {"values": [mcfunc_path]}
-            append function mcfunc_path:
-                scoreboard players reset f"${ctx.project_id}#{cls._var_type}${index}" Config.SCOREBOARD_ROOT
+    def _setup_flushing(cls, full_location):
+        with safe_load(f"flush_variable/{cls._var_type}", append=True):
+            scoreboard players reset full_location Config.SCOREBOARD_ROOT
 
 class VarStorageSource(DataSource, BaseVar):
     @classmethod
     def create(cls, is_static: bool):
         location_index = cls._evaluate_location_index(is_static)
+        cls._setup_flushing(location_index)
         return cls('storage', Config.STORAGE_ROOT)[ctx.project_id]['data'][cls._var_type][location_index]
 
     @classmethod
-    def _flush_on_load(cls):
-        mcfunc_path = f"{Config.ROOT_LOCAL}/runtime_var_flush_storage"
+    def _setup_flushing(cls, location_index):
+        slot_block_size = 64
+
+        if not location_index % slot_block_size:
+            slot_block = []
+            full_location = f"{ctx.project_id}.data.{cls._var_type}"
 
-        if cls._location_index < 0:
-            return 0
+            for n in range(slot_block_size):
+                slot_block.append(cls._default_slot_value)
 
-        fresh_slots = []
-        for n in range(cls._location_index+1):
-            fresh_slots.append(cls._default_slot_value)
-
-        merge function_tag minecraft:load {"values": [mcfunc_path]}
-        append function mcfunc_path:
-            nbt_path = f"{ctx.project_id}.data.{cls._var_type}"
-            data modify storage Config.STORAGE_ROOT nbt_path set value fresh_slots
+            with safe_load(f"flush_variable/{cls._var_type}", append=True):
+                data modify storage Config.STORAGE_ROOT full_location append value slot_block
 
 class BoolSource(VarScoreSource):
     _var_type = 'bool'
 
     def _rebind(self, score, value):
         if not isinstance(value, ExpressionNode):
             value = int(value)
```

### Comparing `wicked_expressions-0.5.2/PKG-INFO` & `wicked_expressions-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.5.2
+Version: 0.5.3
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -66,15 +66,15 @@
     - bolt
     - wicked_expressions
 
 pipeline:
     - mecha
 ```
 
-Once you've required `bolt` and `wicked-expressions`, you are able to import the python package's `api` module directly inside your bolt scripts.
+Once you've required `bolt` and `wicked_expressions`, you are able to import the python package's `api` module directly inside your bolt scripts.
 
 ```py
 from wicked_expressions:api import Scoreboard, Data
 ```
 
 Now you're free to use the API objects. Create simple and complex expressions, compare storages with scores, scores with scores, check if scores exist and more.
```

