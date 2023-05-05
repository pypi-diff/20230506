# Comparing `tmp/retroperm-0.0.3.tar.gz` & `tmp/retroperm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retroperm-0.0.3.tar", last modified: Thu Apr 13 11:23:57 2023, max compression
+gzip compressed data, was "retroperm-0.1.0.tar", last modified: Fri May  5 22:05:57 2023, max compression
```

## Comparing `retroperm-0.0.3.tar` & `retroperm-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:23:57.302049 retroperm-0.0.3/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     7647 2023-04-13 09:48:15.000000 retroperm-0.0.3/LICENSE
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-04-13 11:23:57.302049 retroperm-0.0.3/PKG-INFO
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      239 2023-03-30 22:52:41.000000 retroperm-0.0.3/README.md
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      564 2023-04-13 11:23:52.000000 retroperm-0.0.3/pyproject.toml
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:23:57.298049 retroperm-0.0.3/retroperm/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       22 2023-03-30 22:52:41.000000 retroperm-0.0.3/retroperm/__init__.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:23:57.298049 retroperm-0.0.3/retroperm/analysis/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:41.000000 retroperm-0.0.3/retroperm/analysis/__init__.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1676 2023-03-30 22:52:41.000000 retroperm-0.0.3/retroperm/analysis/functions.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      713 2023-03-30 15:19:36.000000 retroperm-0.0.3/retroperm/analysis/permfinder.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     4225 2023-03-28 14:41:57.000000 retroperm-0.0.3/retroperm/analysis/resolver.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1969 2023-04-01 19:20:53.000000 retroperm-0.0.3/retroperm/analysis/utils.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1372 2023-03-24 18:26:08.000000 retroperm-0.0.3/retroperm/analysis/utils_angrmgmt.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     5909 2023-04-13 11:18:32.000000 retroperm-0.0.3/retroperm/project.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:23:57.302049 retroperm-0.0.3/retroperm/rules/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       23 2023-04-11 22:53:49.000000 retroperm-0.0.3/retroperm/rules/__init__.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      614 2023-04-13 10:13:49.000000 retroperm-0.0.3/retroperm/rules/data.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       43 2023-04-11 22:53:49.000000 retroperm-0.0.3/retroperm/rules/default_rules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     2537 2023-04-13 05:40:22.000000 retroperm-0.0.3/retroperm/rules/filesystem_rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      241 2023-04-06 17:49:41.000000 retroperm-0.0.3/retroperm/rules/pathrules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      947 2023-04-12 04:17:48.000000 retroperm-0.0.3/retroperm/rules/rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      754 2023-03-30 17:57:42.000000 retroperm-0.0.3/retroperm/rules/ruleList.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:22.000000 retroperm-0.0.3/retroperm/rules/rules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-30 01:49:39.000000 retroperm-0.0.3/retroperm/setup.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:23:57.298049 retroperm-0.0.3/retroperm.egg-info/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-04-13 11:23:57.000000 retroperm-0.0.3/retroperm.egg-info/PKG-INFO
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      717 2023-04-13 11:23:57.000000 retroperm-0.0.3/retroperm.egg-info/SOURCES.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        1 2023-04-13 11:23:57.000000 retroperm-0.0.3/retroperm.egg-info/dependency_links.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       14 2023-04-13 11:23:57.000000 retroperm-0.0.3/retroperm.egg-info/requires.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       10 2023-04-13 11:23:57.000000 retroperm-0.0.3/retroperm.egg-info/top_level.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      531 2023-04-13 11:23:57.302049 retroperm-0.0.3/setup.cfg
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       37 2023-03-30 22:52:41.000000 retroperm-0.0.3/setup.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-04-13 11:23:57.302049 retroperm-0.0.3/tests/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     2113 2023-04-13 05:45:01.000000 retroperm-0.0.3/tests/test_project.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-05 22:05:57.347803 retroperm-0.1.0/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     7647 2023-04-13 09:48:15.000000 retroperm-0.1.0/LICENSE
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-05-05 22:05:57.347803 retroperm-0.1.0/PKG-INFO
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      239 2023-03-30 22:52:41.000000 retroperm-0.1.0/README.md
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      564 2023-05-05 22:04:22.000000 retroperm-0.1.0/pyproject.toml
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-05 22:05:57.347803 retroperm-0.1.0/retroperm/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       22 2023-03-30 22:52:41.000000 retroperm-0.1.0/retroperm/__init__.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-05 22:05:57.347803 retroperm-0.1.0/retroperm/analysis/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:41.000000 retroperm-0.1.0/retroperm/analysis/__init__.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1676 2023-03-30 22:52:41.000000 retroperm-0.1.0/retroperm/analysis/functions.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      713 2023-03-30 15:19:36.000000 retroperm-0.1.0/retroperm/analysis/permfinder.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     4225 2023-03-28 14:41:57.000000 retroperm-0.1.0/retroperm/analysis/resolver.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1969 2023-04-01 19:20:53.000000 retroperm-0.1.0/retroperm/analysis/utils.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1372 2023-03-24 18:26:08.000000 retroperm-0.1.0/retroperm/analysis/utils_angrmgmt.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     9088 2023-04-26 00:16:19.000000 retroperm-0.1.0/retroperm/project.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-05 22:05:57.347803 retroperm-0.1.0/retroperm/rules/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      182 2023-04-27 19:14:13.000000 retroperm-0.1.0/retroperm/rules/__init__.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      147 2023-04-18 01:01:52.000000 retroperm-0.1.0/retroperm/rules/argument_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      697 2023-04-25 15:27:54.000000 retroperm-0.1.0/retroperm/rules/ban_category_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      995 2023-04-25 15:25:33.000000 retroperm-0.1.0/retroperm/rules/ban_library_function_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     2240 2023-04-25 15:15:54.000000 retroperm-0.1.0/retroperm/rules/data.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       43 2023-04-11 22:53:49.000000 retroperm-0.1.0/retroperm/rules/default_rules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     2737 2023-04-27 20:44:47.000000 retroperm-0.1.0/retroperm/rules/filesystem_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      241 2023-04-06 17:49:41.000000 retroperm-0.1.0/retroperm/rules/pathrules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      571 2023-04-20 18:44:23.000000 retroperm-0.1.0/retroperm/rules/rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      754 2023-03-30 17:57:42.000000 retroperm-0.1.0/retroperm/rules/ruleList.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:22.000000 retroperm-0.1.0/retroperm/rules/rules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-30 01:49:39.000000 retroperm-0.1.0/retroperm/setup.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-05 22:05:57.347803 retroperm-0.1.0/retroperm.egg-info/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-05-05 22:05:57.000000 retroperm-0.1.0/retroperm.egg-info/PKG-INFO
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      832 2023-05-05 22:05:57.000000 retroperm-0.1.0/retroperm.egg-info/SOURCES.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        1 2023-05-05 22:05:57.000000 retroperm-0.1.0/retroperm.egg-info/dependency_links.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       14 2023-05-05 22:05:57.000000 retroperm-0.1.0/retroperm.egg-info/requires.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       10 2023-05-05 22:05:57.000000 retroperm-0.1.0/retroperm.egg-info/top_level.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      531 2023-05-05 22:05:57.347803 retroperm-0.1.0/setup.cfg
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       37 2023-03-30 22:52:41.000000 retroperm-0.1.0/setup.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-05 22:05:57.347803 retroperm-0.1.0/tests/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     5661 2023-04-26 00:20:51.000000 retroperm-0.1.0/tests/test_project.py
```

### Comparing `retroperm-0.0.3/LICENSE` & `retroperm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.3/PKG-INFO` & `retroperm-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retroperm
-Version: 0.0.3
+Version: 0.1.0
 Summary: A retroactive effective binary permission deduction tool
 Home-page: https://github.com/SpiritSeal/retroperm
 Author-email: Saketh Reddy <yssaketh@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SpiritSeal/retroperm
 Project-URL: Bug Tracker, https://github.com/SpiritSeal/retroperm/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `retroperm-0.0.3/pyproject.toml` & `retroperm-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retroperm"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Saketh Reddy", email="yssaketh@gmail.com" },
 ]
 description = "A retroactive effective binary permission deduction tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `retroperm-0.0.3/retroperm/analysis/functions.py` & `retroperm-0.1.0/retroperm/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.3/retroperm/analysis/permfinder.py` & `retroperm-0.1.0/retroperm/analysis/permfinder.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.3/retroperm/analysis/resolver.py` & `retroperm-0.1.0/retroperm/analysis/resolver.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.3/retroperm/analysis/utils.py` & `retroperm-0.1.0/retroperm/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.3/retroperm/analysis/utils_angrmgmt.py` & `retroperm-0.1.0/retroperm/analysis/utils_angrmgmt.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.3/retroperm/project.py` & `retroperm-0.1.0/retroperm/project.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,97 @@
-from typing import Dict, List
+from typing import Dict, List, Set
 import angr
 from .analysis.utils import get_arg_locations
 from .analysis.utils_angrmgmt import string_at_addr
+from .rules.argument_rule import ArgumentRule
+from .rules.ban_category_rule import BanCategoryRule
+from .rules.ban_library_function_rule import BanLibraryFunctionRule
 from .rules.data import important_func_args
 from .rules import Rule, default_rules
 import pyvex
+from sortedcollections import OrderedSet
 
 import logging
 
 logging.getLogger('angr.analyses.reaching_definitions').setLevel(logging.FATAL)
 logging.getLogger('angr.project').setLevel(logging.FATAL)
 logging.getLogger('cle.loader').setLevel(logging.FATAL)
 
 
 class RetropermProject:
 
     def __init__(self, binary_path):
         self.binary_path = binary_path
         self.proj = angr.Project(binary_path, auto_load_libs=False)
         self.cfg = self.proj.analyses.CFGFast.prep()()
-        self.ccca = self.proj.analyses[angr.analyses.CompleteCallingConventionsAnalysis].prep()()
-        self.resolved_data: Dict[angr.SimProcedure, ResolvedFunctionObject] = {}
-        self.rules = set()
+        try:
+            self.ccca = self.proj.analyses[angr.analyses.CompleteCallingConventionsAnalysis].prep()()
+        except:
+            self.ccca = None
+        self.rules = OrderedSet()
+        self.resolved_function_data: Dict[angr.SimProcedure, ResolvedFunctionObject] = {}
         self.resolved_function_data = None
+        self.called_symbols: Set[str] | None = None
+        self.resolved_project_data: Dict[str, object] = {}
+        # self.resolved_project_data: ResolvedProjectData = None
 
     def get_printable_value(self, reg_arg_type: angr.sim_type.SimTypeReg, value: int) -> str or int:
         if reg_arg_type.__class__ == angr.sim_type.SimTypePointer:
             str_val = string_at_addr(self.cfg, value, self.proj)
             # Strip double quotes
             return str_val[1:-1]
         else:
             return value
 
-    def resolve_abusable_functions(self):
+    def create_called_symbols_list(self) -> Set[str]:
+        proj = self.proj
+        cfg = self.cfg
 
-        resolved_data: Dict[angr.SimProcedure, ResolvedFunctionObject] = {}
+        called_symbols = OrderedSet()
+        # for symbol in proj.loader.main_object.symbols:
+        #     if proj.is_symbol_hooked(symbol.name):
+        #         called_symbols.append(symbol.name)
+        for func in cfg.kb.functions.values():
+            for block in func.blocks:
+                if block.size == 0:
+                    continue
+                vex_block: pyvex.block.IRSB = block.vex
+                cur_addr = vex_block.addr
+                if vex_block.jumpkind != 'Ijk_Call' or len(vex_block.next.constants) == 0:
+                    continue
+                call_target = vex_block.next.constants[0].value
+                called_symbols.add(cfg.kb.functions.function(addr=call_target))
+        self.called_symbols = called_symbols
+        return called_symbols
 
+    def resolve_defined_simproc_args(self):
         proj = self.proj
         cfg = self.cfg
         ccca = self.ccca
 
+        resolved_function_data: Dict[angr.SimProcedure, ResolvedFunctionObject] = {}
         running_resolved_functions: Dict[angr.sim_procedure.SimProcedure: Dict[int, Dict[str, str | int]]] = {}
 
         for func in cfg.kb.functions.values():
             for block in func.blocks:
                 if block.size == 0:
                     continue
                 vex_block: pyvex.block.IRSB = block.vex
                 cur_addr = vex_block.addr
                 if vex_block.jumpkind != 'Ijk_Call' or len(vex_block.next.constants) == 0:
                     continue
                 call_target = vex_block.next.constants[0].value
+                # TODO: Transport this to below
                 call_target_symbol = cfg.kb.functions.function(addr=call_target)
                 if call_target_symbol is None or not proj.is_symbol_hooked(call_target_symbol.name):
                     continue
                 simproc = proj.symbol_hooked_by(call_target_symbol.name)
+                # TODO: Remove after doing something about the way the things are stored in the lookup table
+                # TODO: / create new extended "pass" Simprocs to catch the new targets (see logbook 04-13-23)
+                # print(call_target_symbol.name, simproc)
                 if not simproc or simproc.__class__ not in important_func_args:
                     continue
 
                 important_arg_nums = important_func_args[simproc.__class__]
 
                 target_arg_locations = [arg.reg_name for arg in get_arg_locations(ccca.kb.functions[call_target])]
                 important_args = [target_arg_locations[arg_num] for arg_num in important_arg_nums]
@@ -68,66 +101,88 @@
                 for stmt in vex_block.statements:
                     if not isinstance(stmt, pyvex.stmt.Put):
                         continue
                     stmt: pyvex.stmt.Put
                     reg = proj.arch.register_names[stmt.offset]
                     if reg in important_args:
                         arg_num = important_args.index(reg)
+                        if not hasattr(stmt.data, "con"):
+                            continue
+                        # try:
                         ora[arg_num] = self.get_printable_value(simproc.prototype.args[arg_num], stmt.data.con.value)
+                        # except:
+                        #     print('FAILED ON', stmt)
+                        #     exit(1)
 
                 final_resolved_block = {}
                 for count, value in enumerate(ora):
                     final_resolved_block[important_arg_nums[count]] = value
 
                 if simproc not in running_resolved_functions:
                     running_resolved_functions[simproc] = {}
                 running_resolved_functions[simproc][cur_addr] = final_resolved_block
 
         for key, value in running_resolved_functions.items():
             key: angr.sim_procedure.SimProcedure
-            resolved_data[key.display_name] = ResolvedFunctionObject(key, value)
-        self.resolved_data = resolved_data
-        return resolved_data
+            resolved_function_data[key.display_name] = ResolvedFunctionObject(key, value)
+        self.resolved_function_data = resolved_function_data
+        return resolved_function_data
+
+    def resolve_abusable_functions(self):
+
+        self.resolved_project_data['resolved_function_data'] = self.resolve_defined_simproc_args()
+        self.resolved_project_data['active_symbols'] = self.create_called_symbols_list()
+        return self.resolved_project_data
 
     # Rule Stuff
     def init_rules(self, rule_list: List[Rule], override_default=False):
         # Add the rules to the self.rules
-        self.rules = set(rule_list if override_default else (rule_list and default_rules))
+        self.rules = OrderedSet(rule_list if override_default else (rule_list and default_rules))
 
     def load_rules(self, rule_list: List[Rule]):
         # Add the rules to the self.rules
         self.rules |= rule_list
 
     def validate_rule(self, rule: Rule) -> str:
-        output: Dict[str, bool] = rule.validate_batch(self.resolved_data)
-        fails = []
-        for key, value in output.items():
-            if not value:
-                fails.append(key)
-        if fails:
-            return f'Failed on {fails}'
+
+        if isinstance(rule, ArgumentRule):
+            output: Dict[str, bool] = rule.validate(self.resolved_project_data)
+            fails = []
+            for key, value in output.items():
+                if not value:
+                    fails.append(key)
+            if fails:
+                return f'Failed on {fails}'
+            else:
+                return 'Passed'
+        elif isinstance(rule, BanLibraryFunctionRule):
+            return 'Passed' if rule.validate(self.resolved_project_data) else 'Failed'
+        elif isinstance(rule, BanCategoryRule):
+            return f'Failed on {rule.validate(self.resolved_project_data)}' if rule.validate(self.resolved_project_data) else 'Passed'
+        elif isinstance(rule, Rule):
+            raise NotImplementedError
         else:
-            return 'Passed'
+            raise ValueError('Rule not recognized')
 
     def validate_rules(self, rule_list=None):
         if not rule_list:
             if not self.rules:
                 raise ValueError('No rules to validate')
             rule_list = self.rules
         output = {}
-        for rule in self.rules:
+        for rule in rule_list:
             output[rule] = self.validate_rule(rule)
 
         return output
 
 
 class ResolvedFunctionObject:
 
     def generate_argument_categories(self):
-        argument_types = set()
+        argument_types = OrderedSet()
         for key, value in self.args_by_location.items():
             for arg_type, arg_value in value.items():
                 argument_types.add(arg_type)
             return argument_types
 
     def __init__(self, resolved_function_simproc: angr.sim_procedure.SimProcedure,
                  args_by_location: Dict[int, Dict[str, str]]):
@@ -136,7 +191,24 @@
         # print(self.args_by_location)
         self.argument_types = self.generate_argument_categories()
 
     def __repr__(self):
         # Example: {'open': <ResolvedFunction: open@[0xdeadbeef, 0xcafebabe, ...]>}
         list_of_addresses = [hex(addr) for addr in list(self.args_by_location.keys())]
         return f"<ResolvedFunction: {self.resolved_function_simproc}@{list_of_addresses}>"
+
+
+# TODO: Implement this in order to make the code more readable and easier to work with
+# class ResolvedProjectData:
+#     def __init__(self, rfo: ResolvedFunctionObject = None, called_symbols: List[str] = None):
+#         self.resolved_function_data: Dict[angr.SimProcedure, ResolvedFunctionObject] = {}
+#         self.active_symbols: List[str] = []
+
+
+
+
+
+
+
+
+
+
```

### Comparing `retroperm-0.0.3/retroperm/rules/filesystem_rule.py` & `retroperm-0.1.0/retroperm/rules/filesystem_rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 from typing import Dict
-from .rule import Rule
+# from .rule import Rule
+from .argument_rule import ArgumentRule
 from pathlib2 import Path
 import pathlib2 as pathlib
 
 from ..project import ResolvedFunctionObject
 
 
-class FilesystemRule(Rule):
+class FilesystemRule(ArgumentRule):
     """
     Filesystem rules.
     """
 
     def __init__(self,
                  location: str | Path,
                  arg_cat: str,  # argument_category
                  is_whitelist: bool,
                  is_dir: bool):
-        super().__init__()
-        self.arg_cat = arg_cat
+        super().__init__(arg_cat)
         self.location = location
         self.is_whitelist = is_whitelist
         self.is_dir = is_dir
 
     def __repr__(self):
         # return f'FilesystemRule({self.location=}, {self.arg_cat=}, {self.is_whitelist=}, {self.is_dir=})'
         # I just want location and whitelist status
         # return f'FilesystemRule(\'{self.location}\' is {"whitelisted" if self.is_whitelist else "blacklisted"})'
         # Format as "Whitelist: /etc/passwd"
         return f'{"Whitelist" if self.is_whitelist else "Blacklist"} {self.location}'
 
-    def validate_batch(self, resolved_data: Dict[str, ResolvedFunctionObject]) -> Dict:
+    # def validate(self, resolved_data: Dict[str, ResolvedFunctionObject]) -> Dict:
+    def validate(self, resolved_project_data: Dict[str, object]) -> Dict:
         """
         Validate the rule against the resolved data.
         """
+        resolved_function_data = resolved_project_data['resolved_function_data']
         output: dict[str, bool] = {}
-        for key, rfo in resolved_data.items():
-            if self.validate(rfo):
-                # Redundant for now, but will be useful later
+        for key, rfo in resolved_function_data.items():
+            if self.validate_rfo(rfo):
+                # Redundant for now, but will maybe be useful later
                 output[key] = True
                 # print(f'Rule {self} passed on {key}!')
             else:
                 output[key] = False
                 # print(f'Rule {self} failed on {key}!')
         return output
 
-    def validate(self, rfo: ResolvedFunctionObject) -> bool:
+    def validate_rfo(self, rfo: ResolvedFunctionObject) -> bool:
         """
         Validate the rule against a single resolved function.
         """
         for addr, res_args in rfo.args_by_location.items():
             if self.arg_cat not in res_args:
                 continue
             if self.arg_cat is 'filename':
```

### Comparing `retroperm-0.0.3/retroperm/rules/ruleList.py` & `retroperm-0.1.0/retroperm/rules/ruleList.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.0.3/retroperm.egg-info/PKG-INFO` & `retroperm-0.1.0/retroperm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retroperm
-Version: 0.0.3
+Version: 0.1.0
 Summary: A retroactive effective binary permission deduction tool
 Home-page: https://github.com/SpiritSeal/retroperm
 Author-email: Saketh Reddy <yssaketh@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SpiritSeal/retroperm
 Project-URL: Bug Tracker, https://github.com/SpiritSeal/retroperm/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `retroperm-0.0.3/retroperm.egg-info/SOURCES.txt` & `retroperm-0.1.0/retroperm.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 retroperm/analysis/__init__.py
 retroperm/analysis/functions.py
 retroperm/analysis/permfinder.py
 retroperm/analysis/resolver.py
 retroperm/analysis/utils.py
 retroperm/analysis/utils_angrmgmt.py
 retroperm/rules/__init__.py
+retroperm/rules/argument_rule.py
+retroperm/rules/ban_category_rule.py
+retroperm/rules/ban_library_function_rule.py
 retroperm/rules/data.py
 retroperm/rules/default_rules.py
 retroperm/rules/filesystem_rule.py
 retroperm/rules/pathrules.py
 retroperm/rules/rule.py
 retroperm/rules/ruleList.py
 retroperm/rules/rules.py
```

### Comparing `retroperm-0.0.3/setup.cfg` & `retroperm-0.1.0/setup.cfg`

 * *Files identical despite different names*

