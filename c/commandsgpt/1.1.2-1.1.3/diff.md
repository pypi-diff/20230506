# Comparing `tmp/commandsgpt-1.1.2.tar.gz` & `tmp/commandsgpt-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.1.2.tar", last modified: Sat May  6 01:01:26 2023, max compression
+gzip compressed data, was "commandsgpt-1.1.3.tar", last modified: Sat May  6 15:21:18 2023, max compression
```

## Comparing `commandsgpt-1.1.2.tar` & `commandsgpt-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/commands_gpt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/commands_gpt/commands_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/instruction_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-06 01:01:26.000000 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-06 01:01:26.000000 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:01:26.000000 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 01:01:26.000000 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:21:18.635806 commandsgpt-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-06 15:21:18.635806 commandsgpt-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:21:18.627806 commandsgpt-1.1.3/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:21:18.631806 commandsgpt-1.1.3/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:21:18.635806 commandsgpt-1.1.3/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/instruction_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/commands_gpt/commands_gpt/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:21:18.635806 commandsgpt-1.1.3/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-06 15:21:18.000000 commandsgpt-1.1.3/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-06 15:21:18.000000 commandsgpt-1.1.3/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:21:18.000000 commandsgpt-1.1.3/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 15:21:18.000000 commandsgpt-1.1.3/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 15:21:07.000000 commandsgpt-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-06 15:21:18.635806 commandsgpt-1.1.3/setup.cfg
```

### Comparing `commandsgpt-1.1.2/LICENSE` & `commandsgpt-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.2/PKG-INFO` & `commandsgpt-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.1.2
+Version: 1.1.3
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `commandsgpt-1.1.2/README.md` & `commandsgpt-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.1.3/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Callable
 
 from ..chat import get_answer_from_model
 from ..config import Config
-from .graphs import Graph, generate_graph_data
+from .graphs import Graph
 
 ESSENTIAL_COMMANDS = {
     "THINK": {
         "description": "Generates a thought in your 'mind' without writing it down yet. This command allows you to create new ideas, reflect, and analyze information. For example, when asked to 'Write a three-paragraph article about Lenz's Law,' you would first use this command to generate the article and then use another to write it.",
         "arguments": {
             "about": {"description": "What to think about. Example: 'Three-paragraph article about Lenz's Law.'", "type": "string"},
         },
```

### Comparing `commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/graphs.py` & `commandsgpt-1.1.3/commands_gpt/commands_gpt/commands/graphs.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 import json
 from typing import Any, Callable
 
 from .. import regex
 from ..static import StaticVar
 from ..config import Config
 
+# status codes
+NOT_REACHED = 0
+NOT_EXECUTED = 1
+EXECUTED = 2
+
 @functools.total_ordering
 class CommandNode:
     def __init__(self, data: list, commands: dict[str, dict], command_name_to_func: dict[str, Callable]):
         self.id = data[0]
         self.previous_command_id = data[1][0] if data[1] else None
         self.dependent_on_data = data[1][1] if data[1] else None
         self.required_value = data[1][2] if data[1] else None
@@ -17,14 +22,17 @@
 
         assert self.command_name in commands, f"Command '{self.command_name}' does not exist."
         assert self.command_name in command_name_to_func, f"Command '{self.command_name}' does not have a function declaration."
 
         self.command = command_name_to_func[self.command_name]
         self.arguments = data[3] if len(data) > 3 else None
 
+        self.status = NOT_REACHED
+        self.data_generated = None
+
     def __eq__(self, other):
         return self.id == other.id
 
     def __lt__(self, other):
         return self.id < other.id
 
     def __str__(self):
@@ -33,85 +41,104 @@
     def execute_command(self, config: Config, graph, arguments: dict[str, Any]):
         print(f"\n\nRunning '{self.command_name}' command with id {self.id}...")
         if config.verbosity >= 2:
             print(f"Using arguments: {arguments}")
         self.data_generated = self.command(config, graph, **arguments)
 
 class Graph:
+    # TODO: Do not call twice set_start_data when initializing a graph (__init__ -> initialize -> build_graph)
+
     def __init__(self, raw_commands_data: StaticVar, commands: dict[str, dict], 
             command_name_to_func: dict[str, Callable]):
-        self.build_graph(raw_commands_data, commands, command_name_to_func)
+        self.set_start_data(raw_commands_data, commands, command_name_to_func)
+        self.initialize()
 
-    def build_graph(self, raw_commands_data: StaticVar, commands: dict[str, dict], 
+    def set_start_data(self, raw_commands_data: StaticVar, commands: dict[str, dict], 
             command_name_to_func: dict[str, Callable]):
         self.raw_commands_data = raw_commands_data
         self.commands = commands
         self.command_name_to_func = command_name_to_func
-        self.commands_data, self.data_references = generate_graph_data(raw_commands_data.val)
+
+    def build_graph(self, raw_commands_data: StaticVar, commands: dict[str, dict], 
+            command_name_to_func: dict[str, Callable]):
+        self.set_start_data(raw_commands_data, commands, command_name_to_func)
+        self.commands_data, self.data_references = generate_graph_build_data(raw_commands_data.val)
         self.build_nodes()
 
     def build_nodes(self):
-        self.nodes: dict[str, CommandNode] = {}
         for command_data in self.commands_data:
             node = CommandNode(command_data, self.commands, self.command_name_to_func)
+            if node.id in self.reached_nodes_ids:
+                # recover results of the node
+                reached_node = self.nodes[node.id]
+                node.status = reached_node.status
+                node.data_generated = reached_node.data_generated
             self.nodes[node.id] = node
 
-    def initialize_graph(self):
-        self.generated_data = {}
+    def initialize(self):
+        self.reached_nodes_ids: list[int] = []
+        self.nodes: dict[str, CommandNode] = {}
+        self.build_graph(self.raw_commands_data, self.commands, self.command_name_to_func)
     
     def inject_node_data(self, node_id: int, data_generated_by_node: dict[str, Any]):
         # inject data generated by the node to the data string
         new_raw_commands_data = StaticVar(regex.inject_node_data(
             self.raw_commands_data.val, node_id, data_generated_by_node,
         ))
 
         # rebuild graph
         self.build_graph(new_raw_commands_data, self.commands, self.command_name_to_func)
     
     def execute_node(self, node_id: int, config: Config):
         node = self.nodes[node_id]
 
-        if node.id in self.generated_data:
-            # already executed
-            return self.generated_data[node.id]
+        if node.status == EXECUTED:
+            return
 
         if node.previous_command_id is not None:
-            previous_node_data_generated = self.execute_node(node.previous_command_id, config)
+            previous_node = self.nodes[node.previous_command_id]
+            if previous_node.status == NOT_EXECUTED:
+                # the previous node was not executed, so this node will not
+                # activate
+                return
+
+            if previous_node.status == NOT_REACHED:
+                self.execute_node(previous_node.id, config)
 
             if node.dependent_on_data:
-                if previous_node_data_generated[node.dependent_on_data] != node.required_value:
-                    return {}
+                if previous_node.data_generated[node.dependent_on_data] != node.required_value:
+                    node.status = NOT_EXECUTED
+                    return
 
         node.execute_command(config, self, node.arguments)
-        self.generated_data[node.id] = node.data_generated
+        self.reached_nodes_ids.append(node.id)
+        node.status = EXECUTED
 
         if node.id in self.data_references:
             self.inject_node_data(node.id, node.data_generated)
 
-        return node.data_generated
-
     def print_graph(self):
         print("\n\n--- Commands graph ---")
         for node in self.nodes.values():
             print(f"\n{node.id}. {node.command_name}")
             if node.previous_command_id:
                 print(f"\n\tExecuted after node «{node.previous_command_id}».")
             if node.dependent_on_data:
                 print(f"\n\t\tResult field '{node.dependent_on_data}' of node «{node.previous_command_id}» must have value «{node.required_value}» in order to execute this node.")
         print("\n--- -------------- ---\n")
 
     def execute_commands(self, config: Config):
-        self.initialize_graph()
+        self.initialize()
         if config.verbosity >= 1:
             self.print_graph()
 
         for node_id in sorted(self.nodes.keys()):
             self.execute_node(node_id, config)
 
-def generate_graph_data(raw_commands_data):
+def generate_graph_build_data(raw_commands_data):
     """
     Parses a commands data string to a JSON to create the graph data
 
     Args:
         raw_commands_data (str): A string containing raw commands data that has not yet been converted to a JSON.
 
     Returns:
@@ -120,15 +147,14 @@
             commands_data: data of the commands (to create a graph).
 
             data_references: data references (data that will be injected).
     """
     data_references = regex.find_data_references_indices(raw_commands_data)
     commands_data = regex.nullify_all_data_references(raw_commands_data)
 
-    # TODO: Fix JSON parsing error that is sometimes raised when newline characters are written.
     try:
         commands_data = json.loads(commands_data, strict=False)
     except Exception as e:
-        print(f"!!! Raw commands data: {raw_commands_data}")
+        print(f"!!! Can't decode raw commands data to JSON: {raw_commands_data}")
         raise e
 
     return commands_data, data_references
```

### Comparing `commandsgpt-1.1.2/commands_gpt/commands_gpt/instruction_recognition.py` & `commandsgpt-1.1.3/commands_gpt/commands_gpt/instruction_recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
             """\n\nDepending on the prompt, you will use different commands and different arguments and relationships between commands. The only way you can see data generated by other commands from a command is by passing them as arguments."""
 
             """\n\nYour response will have this format:"""
             """\n[[command_id, [previous_command_id, dependent_on_data, required_value], "COMMAND_NAME", {"arg1": value1, "arg2": value2, ...}], [...]]"""
             """\nTo reference data generated by a command, use __&i.data__. 'i' is the ID of the command; 'data' is the name of the generated data, and works like a Python value (if it's a list, you can use __&i.data[i]__, __&i.data[i:j]__, etc.; in a dictionary, __&i.data["key"]__, etc.)"""
             """\nThe structure will ultimately be like a graph. The previous_command_id defines after which command the current one will be executed, dependent_on_data is the name of the data generated by the previous command which will be used as a condition (null if it won't be used), and required_value is what value the dependent_on_data must have to execute the current one (or null if it doesn't matter)."""
-            """\nBe concise with the structure."""
+            """\nBe concise but *solid* with the structure."""
+            """\n*Consider that the user might write incorrectly and their inputs might be ambiguous*."""
 
             """\n\nFor example:"""
 
             """\n\nExample 1:"""
             """\nUser prompt: 'Write an article about Lenz's Law, copy it to my clipboard and save it as a file.'"""
             """\nYour response might be: '[[1, [], "%s", {"about": "Article about Lenz's Law"}], [2, [1, null, null], "%s", {"content": "__&1.thought__"}], [3, [2, null, null], "%s", {"content": "__&1.thought__", "file_name": "Article about Lenz's Law"}]]'""" % ("THINK", "WRITE_CLIPBOARD", "WRITE_FILE")
             +
```

### Comparing `commandsgpt-1.1.2/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.1.3/commands_gpt/commands_gpt/regex.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/PKG-INFO` & `commandsgpt-1.1.3/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.1.2
+Version: 1.1.3
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.1.3/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.2/setup.cfg` & `commandsgpt-1.1.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commandsgpt
-version = 1.1.2
+version = 1.1.3
 author = Martín Alexis Martínez Andrade
 author_email = alexis.martinez.contacto@gmail.com
 description = An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/AlexisAndradeDev/CommandsGPT
 project_urls =
```

