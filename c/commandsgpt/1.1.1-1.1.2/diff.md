# Comparing `tmp/commandsgpt-1.1.1.tar.gz` & `tmp/commandsgpt-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.1.1.tar", last modified: Fri May  5 16:28:45 2023, max compression
+gzip compressed data, was "commandsgpt-1.1.2.tar", last modified: Sat May  6 01:01:26 2023, max compression
```

## Comparing `commandsgpt-1.1.1.tar` & `commandsgpt-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.793868 commandsgpt-1.1.1/commands_gpt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/commands_gpt/commands_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/instruction_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-05 16:28:45.000000 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-05 16:28:45.000000 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:28:45.000000 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 16:28:45.000000 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/instruction_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/commands_gpt/commands_gpt/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-06 01:01:26.000000 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-06 01:01:26.000000 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:01:26.000000 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 01:01:26.000000 commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 01:01:14.000000 commandsgpt-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-06 01:01:26.352602 commandsgpt-1.1.2/setup.cfg
```

### Comparing `commandsgpt-1.1.1/LICENSE` & `commandsgpt-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.1/PKG-INFO` & `commandsgpt-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.1.1
+Version: 1.1.2
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `commandsgpt-1.1.1/README.md` & `commandsgpt-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/graphs.py` & `commandsgpt-1.1.2/commands_gpt/commands_gpt/commands/graphs.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.1/commands_gpt/commands_gpt/instruction_recognition.py` & `commandsgpt-1.1.2/commands_gpt/commands_gpt/instruction_recognition.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.1/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.1.2/commands_gpt/commands_gpt/regex.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,26 +13,36 @@
     if isinstance(data, (list, tuple)):
         return data[int(index)]
     elif isinstance(data, dict):
         return data[index]
     else:
         raise AssertionError(f"Could not get data for {data_name}. Indexes for type {type(data)} are not supported.")
 
+def fix_for_json(value_as_str: str):
+    # Replace newlines with escaped newlines
+    value_as_str = value_as_str.replace(r"\n", "\\n")
+
+    # Escape double quotes inside the string
+    value_as_str = value_as_str.replace('"', '\\"')
+    return value_as_str
+
 def replace_generated_data_by_node(match_obj, generated_data_by_node: Dict[str, Any]) -> str:
     # Get the data name from the matched object
     data_name = match_obj.group(1)
 
     # Check if the data name has an index/key
     if '[' in data_name and ']' in data_name:
         value = get_indexed_data(data_name, generated_data_by_node)
     else:
         value = generated_data_by_node[data_name]
 
-    # Replace newlines with escaped newlines
-    return str(value).replace(r"\n", "\\n")
+    value_as_str = str(value)
+    value_as_str = fix_for_json(value_as_str)
+
+    return value_as_str
 
 def inject_node_data(raw_commands_data: str, node_id, generated_data_by_node: dict[str, Any]):
     pattern = rf"__&{node_id}\.(\w+)__"
     return re.sub(pattern, lambda m: replace_generated_data_by_node(m, generated_data_by_node), raw_commands_data)
 
 def nullify_all_data_references(raw_commands_data: str):
     """Replaces all __&i.data__ by null."""
```

### Comparing `commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/PKG-INFO` & `commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.1.1
+Version: 1.1.2
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.1.2/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.1/setup.cfg` & `commandsgpt-1.1.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commandsgpt
-version = 1.1.1
+version = 1.1.2
 author = Martín Alexis Martínez Andrade
 author_email = alexis.martinez.contacto@gmail.com
 description = An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/AlexisAndradeDev/CommandsGPT
 project_urls =
```

