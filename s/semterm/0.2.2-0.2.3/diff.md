# Comparing `tmp/semterm-0.2.2.tar.gz` & `tmp/semterm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semterm-0.2.2.tar", last modified: Thu May  4 05:58:50 2023, max compression
+gzip compressed data, was "semterm-0.2.3.tar", last modified: Sat May  6 06:52:10 2023, max compression
```

## Comparing `semterm-0.2.2.tar` & `semterm-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.199402 semterm-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-04 05:58:27.000000 semterm-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 05:58:27.000000 semterm-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-04 05:58:50.195402 semterm-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-04 05:58:27.000000 semterm-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 05:58:27.000000 semterm-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/UI/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/UI/UserInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/UI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/agent/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/MrklAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/TerminalAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/TerminalAgentExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/TerminalAgentPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/config/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/langchain_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/langchain_extensions/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/langchain_extensions/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/SemanticTerminalManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/SemanticTerminalProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/TerminalOutputParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/TerminalTool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:58:50.199402 semterm-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 05:58:27.000000 semterm-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:52:10.853252 semterm-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-06 06:51:50.000000 semterm-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 06:51:50.000000 semterm-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-06 06:52:10.853252 semterm-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-06 06:51:50.000000 semterm-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 06:51:50.000000 semterm-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:52:10.849252 semterm-0.2.3/semterm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:52:10.849252 semterm-0.2.3/semterm/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/UI/UserInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:52:10.853252 semterm-0.2.3/semterm/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/agent/MrklAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/agent/TerminalAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/agent/TerminalAgentExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/agent/TerminalAgentPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:52:10.853252 semterm-0.2.3/semterm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/config/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:52:10.853252 semterm-0.2.3/semterm/langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/langchain_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/langchain_extensions/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/langchain_extensions/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:52:10.853252 semterm-0.2.3/semterm/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/terminal/SemanticTerminalManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/terminal/SemanticTerminalProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/terminal/TerminalOutputParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/terminal/TerminalTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:51:50.000000 semterm-0.2.3/semterm/terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:52:10.849252 semterm-0.2.3/semterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-06 06:52:10.000000 semterm-0.2.3/semterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-06 06:52:10.000000 semterm-0.2.3/semterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:52:10.000000 semterm-0.2.3/semterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 06:52:10.000000 semterm-0.2.3/semterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 06:52:10.000000 semterm-0.2.3/semterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 06:52:10.000000 semterm-0.2.3/semterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 06:52:10.853252 semterm-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-06 06:51:50.000000 semterm-0.2.3/setup.py
```

### Comparing `semterm-0.2.2/LICENSE` & `semterm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/README.md` & `semterm-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm/agent/MrklAgent.py` & `semterm-0.2.3/semterm/agent/MrklAgent.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm/agent/TerminalAgent.py` & `semterm-0.2.3/semterm/agent/TerminalAgent.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm/agent/TerminalAgentExecutor.py` & `semterm-0.2.3/semterm/agent/TerminalAgentExecutor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from abc import ABC
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Tuple, Union, Optional
 
 from langchain.agents import AgentExecutor
 from langchain.agents.tools import InvalidTool
+from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.schema import AgentAction, AgentFinish
 from langchain.tools import BaseTool
 
 from semterm.langchain_extensions.schema import AgentMistake
 
 
 class TerminalAgentExecutor(AgentExecutor, ABC):
     def _take_next_step(
         self,
         name_to_tool_map: Dict[str, BaseTool],
         color_mapping: Dict[str, str],
         inputs: Dict[str, str],
         intermediate_steps: List[Tuple[AgentAction, str]],
+        run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> Union[
         AgentFinish, List[Tuple[AgentAction, str]], List[Tuple[AgentMistake, str]]
     ]:
         """Take a single step in the thought-action-observation loop.
 
         Override this to take control of how the agent makes and acts on choices.
         """
@@ -31,15 +33,15 @@
             return output
         actions: List[AgentAction]
         if isinstance(output, (AgentAction, AgentMistake)):
             actions = [output]
         else:
             actions = output
         for agent_action in actions:
-            self.callback_manager.on_agent_action(
+            run_manager.on_agent_action(
                 agent_action, verbose=self.verbose, color="green"
             )
             # Otherwise we lookup the tool
             if agent_action.tool in name_to_tool_map:
                 tool = name_to_tool_map[agent_action.tool]
                 return_direct = tool.return_direct
                 color = color_mapping[agent_action.tool]
```

### Comparing `semterm-0.2.2/semterm/agent/TerminalAgentPrompt.py` & `semterm-0.2.3/semterm/agent/TerminalAgentPrompt.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm/langchain_extensions/tools.py` & `semterm-0.2.3/semterm/langchain_extensions/tools.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm/terminal/SemanticTerminalManager.py` & `semterm-0.2.3/semterm/terminal/SemanticTerminalManager.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm/terminal/SemanticTerminalProcess.py` & `semterm-0.2.3/semterm/terminal/SemanticTerminalProcess.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm/terminal/TerminalOutputParser.py` & `semterm-0.2.3/semterm/terminal/TerminalOutputParser.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm/terminal/TerminalTool.py` & `semterm-0.2.3/semterm/terminal/TerminalTool.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/semterm.egg-info/SOURCES.txt` & `semterm-0.2.3/semterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semterm-0.2.2/setup.py` & `semterm-0.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="semterm",
-    version="0.2.2",
+    version="0.2.3",
     description="The Semantic Terminal",
     long_description="The Semantic Terminal",
     author="Lambrou",
     author_email="alexanderlambrou0602@gmail.com",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "semterm = semterm.main:main",
         ],
     },
     install_requires=[
         "langchain",
-        "setuptools",
-        "python-dotenv",
         "tiktoken",
         "pexpect",
         "pydantic",
         "openai",
     ],
 )
```

