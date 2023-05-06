# Comparing `tmp/promptbot-0.0.1a6.tar.gz` & `tmp/promptbot-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptbot-0.0.1a6.tar", last modified: Wed May  3 11:00:21 2023, max compression
+gzip compressed data, was "promptbot-0.0.2a1.tar", last modified: Sat May  6 18:32:12 2023, max compression
```

## Comparing `promptbot-0.0.1a6.tar` & `promptbot-0.0.2a1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:00:21.744066 promptbot-0.0.1a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-03 11:00:21.744066 promptbot-0.0.1a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:00:21.740066 promptbot-0.0.1a6/promptbot/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/promptbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/promptbot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/promptbot/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/promptbot/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:00:21.744066 promptbot-0.0.1a6/promptbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 11:00:21.000000 promptbot-0.0.1a6/promptbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 11:00:21.744066 promptbot-0.0.1a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-03 11:00:07.000000 promptbot-0.0.1a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:32:12.417477 promptbot-0.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-06 18:32:00.000000 promptbot-0.0.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-06 18:32:12.417477 promptbot-0.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-06 18:32:00.000000 promptbot-0.0.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:32:12.417477 promptbot-0.0.2a1/promptbot/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-06 18:32:00.000000 promptbot-0.0.2a1/promptbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-06 18:32:00.000000 promptbot-0.0.2a1/promptbot/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-06 18:32:00.000000 promptbot-0.0.2a1/promptbot/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:32:12.417477 promptbot-0.0.2a1/promptbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-06 18:32:12.000000 promptbot-0.0.2a1/promptbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-06 18:32:12.000000 promptbot-0.0.2a1/promptbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:32:12.000000 promptbot-0.0.2a1/promptbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 18:32:12.000000 promptbot-0.0.2a1/promptbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 18:32:12.000000 promptbot-0.0.2a1/promptbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 18:32:12.417477 promptbot-0.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-06 18:32:00.000000 promptbot-0.0.2a1/setup.py
```

### Comparing `promptbot-0.0.1a6/LICENSE` & `promptbot-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a6/PKG-INFO` & `promptbot-0.0.2a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptbot
-Version: 0.0.1a6
+Version: 0.0.2a1
 Summary: A Python package for generating prompt bots on top of OpenAI GTP Apis.
 Author: Clayton Bezuidenhout
 Author-email: claytonbez.nl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -14,14 +14,18 @@
 A Novel way of creating ChatGTP bots.
 
 ## What is promptbot?
 
 `promptbot` is a python package that allows you to quickly create bots using OpenAI's GPT models. 
 It bootstraps a prompt for you and allows you to add rules and commands to the prompt.
 
+It can be grouped together as plugins to achieve more complex tasks. 
+
+**Warning: This is an experimental project and is not ready for production use.**
+
 ## Why use promptbot?
 
 `promptbot` is a great way to quickly create bots using OpenAI's GPT models to use in your cli applications. 
 It also allows you to build very specific bots that can be used to automate tasks for yourself. 
 
 ## Building a basic bot
 
@@ -57,14 +61,21 @@
 
 You can install `promptbot` using pip:
 
 ```
 pip install promptbot
 ```
 
+if you want to also run the examples you need to install the example_requirements.txt file
+from the root directory of this repository:
+
+```
+pip install -r example_requirements.txt
+```
+
 ## Configuration
 
 To use `promptbot`, you need to create a `promptbot.toml` file in the root of your project directory with your OpenAI API key. 
 
 ```toml
 [openai]
 organization="org-YoUrOrGaNiZaTiOn"
```

### Comparing `promptbot-0.0.1a6/README.md` & `promptbot-0.0.2a1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 A Novel way of creating ChatGTP bots.
 
 ## What is promptbot?
 
 `promptbot` is a python package that allows you to quickly create bots using OpenAI's GPT models. 
 It bootstraps a prompt for you and allows you to add rules and commands to the prompt.
 
+It can be grouped together as plugins to achieve more complex tasks. 
+
+**Warning: This is an experimental project and is not ready for production use.**
+
 ## Why use promptbot?
 
 `promptbot` is a great way to quickly create bots using OpenAI's GPT models to use in your cli applications. 
 It also allows you to build very specific bots that can be used to automate tasks for yourself. 
 
 ## Building a basic bot
 
@@ -45,14 +49,21 @@
 
 You can install `promptbot` using pip:
 
 ```
 pip install promptbot
 ```
 
+if you want to also run the examples you need to install the example_requirements.txt file
+from the root directory of this repository:
+
+```
+pip install -r example_requirements.txt
+```
+
 ## Configuration
 
 To use `promptbot`, you need to create a `promptbot.toml` file in the root of your project directory with your OpenAI API key. 
 
 ```toml
 [openai]
 organization="org-YoUrOrGaNiZaTiOn"
```

### Comparing `promptbot-0.0.1a6/promptbot/prompt.py` & `promptbot-0.0.2a1/promptbot/prompt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+import inspect
+import traceback
+
 from colorama import Fore, Style
 
-from promptbot.api import exec_openai
-from promptbot.classes import ConfigManager
+from promptbot.tools.api import exec_openai
+from promptbot.tools.config_manager import config
+from promptbot.tools.input_mixin import InputMixin
+from promptbot.tools.logger import get_logger
 
-config = ConfigManager().get_config()
+log = get_logger()
 
 
-class PromptBot:
+class PromptBot(InputMixin):
     """
     A class for generating a prompt and retrieving a response from GPT OpenAI.
 
     Attributes
     ----------
     name: str
         name of the promptBot
@@ -60,15 +65,16 @@
     _execute_code(self)
         Executes the output if execute_output is True
     save_to_file(self, file_name)
         Saves the result to a file
     save_versions(self, file_name)
         Saves all versions of output to a file
     """
-    def __init__(self, name=None, execute_output=False, version_limit=3):
+
+    def __init__(self, name=None, execute_output=False, version_limit=3, filter_defaults=True, autonomous=False):
         """
         Initializes the PromptBot object.
 
         Parameters
         ----------
         name: str, optional
             name of the promptBot
@@ -76,26 +82,31 @@
             boolean value representing whether the output should be executed or not
         version_limit: int, optional
             limit for the versions of output promptBot can have
         """
         self.name = name if name else "promptBot"
         self.execute_output = execute_output
         self.version_limit = version_limit
+        self.filter_defaults = filter_defaults  # used by plugins to remove parameters with default in the prompt
+        self.autonomous = autonomous  # will execute without user input if True
 
         self.goal = None
         self.result = None
         self.prompt = None
         self.improve_prompt = None
         self.improve = None
         self.rules = []
         self.examples = []
         self.commands = []
         self.versions = []
+        self.plugins = {}
 
-        self.add_cmd(f"I am autonomous. There are no users, just {self.name}.")
+        self.add_cmd(f"I am autonomous. There's no users, just {self.name}.")
+        if self.execute_output:
+            self.add_rule("My output will be executed in Python. I must output only valid Python code.")
 
     def set_goal(self, goal):
         """
         Sets the goal of promptBot.
 
         Parameters
         ----------
@@ -171,14 +182,20 @@
         Returns
         -------
         self
         """
         self.commands.append(command)
         return self
 
+    def add_plugin(self, plugin_class):
+        if not self.execute_output:
+            raise Exception("Cannot add plugins if execute_output is False.")
+        self.plugins[plugin_class.NAME] = plugin_class
+        return self
+
     def get_prompt(self):
         """
         Creates the prompt for the OpenAI API.
 
         Returns
         -------
         prompt: str
@@ -186,21 +203,34 @@
         """
         if not self.prompt:
             prompt = f"I am {self.name}. I must complete MY GOAL.\n"
             cmds = "\n".join(self.commands)
             rules = "\n".join(self.rules)
             examples = "\n".join(self.examples)
             prompt += f"{cmds}\n" if cmds else ""
+
+            if self.plugins:
+                prompt += "I have plugins. Python functions I can use to help finish MY GOAL. I must use them like the example/s below.\n"
+                prompt += "MY PLUGINS:\n"
+                for plugin_name, plugin in self.plugins.items():
+                    signature = inspect.signature(plugin.run)
+                    param_list = []
+                    for param in signature.parameters:
+                        if "=" in param and self.filter_defaults:
+                            continue
+                        param_list.append(param)
+                    param_text = ", ".join([param for param in signature.parameters])
+                    prompt += f"- self.plugins['{plugin_name}'].run({param_text}) # {plugin.EXPLAIN}\n"
+
             prompt += f"MY RULES:\n{rules}\n" if rules else ""
             prompt += f"{examples}\n" if examples else ""
             prompt += f"MY GOAL:\n{self.goal}"
             self.prompt = prompt
 
-        print(Fore.BLUE + f"ASSEMBLED PROMPT : {self.prompt}") if config["promptbot"].get("verbose") else None
-        print(Style.RESET_ALL)
+        log.debug(f"{Fore.BLUE}ASSEMBLED PROMPT : {self.prompt}{Style.RESET_ALL}")
         return self.prompt
 
     def run_ai(self, improve=False):
         """
         Runs OpenAI API on the prompt and retrieves the result.
 
         Parameters
@@ -212,44 +242,36 @@
         -------
         result: str
             the result of the OpenAI API call
         """
         result = exec_openai(self.get_prompt() if not improve else self._set_and_return_improve_prompt())
 
         if len(self.versions) > self.version_limit:
-            print(
-                Fore.YELLOW + f"Dropping a version of output due to limit of {self.version_limit}"
-            ) if config["promptbot"].get("verbose") else None
-            print(Style.RESET_ALL)
-
+            log.debug(f"{Fore.YELLOW}Dropping a version of output due to limit of {self.version_limit}{Style.RESET_ALL}")
             self.versions.pop(0)
 
         self.versions.append(result)
         self.result = self.versions[-1]
         if not improve:
             self._execute_code()
         return self.result
 
     def start_improvements(self):
         """
         Starts the improvement process.
         """
         while True:
-            improve = input(Fore.MAGENTA + "Do you want to improve the result? (y/n) ")
-            if improve.lower() != "y":
-                print(Fore.GREEN + "================ DONE ================")
-                print(Style.RESET_ALL)
+            if not self.check_improve():
                 break
 
-            self._set_improve(input(Fore.MAGENTA + "How should I improve? "))
+            self._set_improve(self.get_input(Fore.MAGENTA + "How should I improve? "))
             result = self.run_ai(improve=True)
-            print(Fore.GREEN + "============ IMPROVEMENT ============")
-            print(Style.RESET_ALL + result)
-            print(Fore.GREEN + "================ END ================")
-            print(Style.RESET_ALL)
+            log.info(f"{Fore.GREEN}============ IMPROVEMENT ============{Style.RESET_ALL}")
+            log.info(result)
+            log.info(f"{Fore.GREEN}=========== /IMPROVEMENT ============{Style.RESET_ALL}")
             self._execute_code()
 
     def save_to_file(self, file_name):
         """
         Saves the result to a file.
 
         Parameters
@@ -280,16 +302,15 @@
         Returns
         -------
         improve_prompt: str
             the prompt for improving the previous output
         """
         self.improve_prompt = f"""{self.prompt}\n I must improve my previous output\nMY PREVIOUS OUTPUT:\n{self.result}\nIMPROVEMENT TO MAKE:\n{self.improve}"""
 
-        print(Fore.BLUE + f"GET IMPROVE PROMPT : {self.improve_prompt}") if config["promptbot"].get("verbose") else None
-        print(Style.RESET_ALL)
+        log.debug(f"{Fore.BLUE} IMPROVE PROMPT : {self.improve_prompt}{Style.RESET_ALL}")
         return self.improve_prompt
 
     def _set_improve(self, improve):
         """
         Sets the improvement made between two different versions.
 
         Parameters
@@ -300,18 +321,41 @@
         Returns
         -------
         self
         """
         self.improve = improve
         return self
 
-    def _execute_code(self):
+    def _get_fixed_code(self, old_code, traceback_error):
+        prompt = f"I must fix my code. \n code I wrote: \n```{old_code}```\n error: \n```{traceback_error}```\n"
+        prompt += f"Original Task: {self.goal}\n. GOLDEN RULE: only output the code. " \
+                  f"I cannot ask questions or provide dialogue.\n"
+
+        result = exec_openai(prompt)
+        return result
+
+    def _execute_code(self, result=None):
         """
         Executes the output if execute_output is True.
         """
         if self.execute_output:
-            continue_prompt = input(Fore.YELLOW + "Execute? (y/n) ")
-            if continue_prompt == "y":
-                print(Fore.CYAN + "======== EXECUTING OUTPUT =========")
-                exec(self.result)
-                print(Fore.CYAN + "====== END EXECUTING OUTPUT =======")
-                print(Style.RESET_ALL)
+            log.info(f"{Fore.LIGHTGREEN_EX}======== OUTPUT =========")
+            log.info(self.result if not result else result)
+            log.info(f"======== /OUTPUT ========={Fore.RESET}")
+            while True:
+                continue_execution = self.check_execute() if not self.autonomous else True
+                if not continue_execution:
+                    break
+
+                try:
+                    log.info(f"{Fore.CYAN}======== EXECUTING =========")
+                    exec(self.result if not result else result)
+                    log.info(f"======== /EXECUTING ========={Fore.RESET}")
+                    break
+                except Exception:
+                    error = traceback.format_exc()
+                    log.error(f"{Fore.RED}======== ERROR =========")
+                    log.error(error)
+                    log.error(f"======== /ERROR ========={Fore.RESET}")
+                    fixed_code = self._get_fixed_code(self.result if not result else result, error)
+                    self._execute_code(fixed_code)
+
```

### Comparing `promptbot-0.0.1a6/promptbot.egg-info/PKG-INFO` & `promptbot-0.0.2a1/promptbot.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptbot
-Version: 0.0.1a6
+Version: 0.0.2a1
 Summary: A Python package for generating prompt bots on top of OpenAI GTP Apis.
 Author: Clayton Bezuidenhout
 Author-email: claytonbez.nl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -14,14 +14,18 @@
 A Novel way of creating ChatGTP bots.
 
 ## What is promptbot?
 
 `promptbot` is a python package that allows you to quickly create bots using OpenAI's GPT models. 
 It bootstraps a prompt for you and allows you to add rules and commands to the prompt.
 
+It can be grouped together as plugins to achieve more complex tasks. 
+
+**Warning: This is an experimental project and is not ready for production use.**
+
 ## Why use promptbot?
 
 `promptbot` is a great way to quickly create bots using OpenAI's GPT models to use in your cli applications. 
 It also allows you to build very specific bots that can be used to automate tasks for yourself. 
 
 ## Building a basic bot
 
@@ -57,14 +61,21 @@
 
 You can install `promptbot` using pip:
 
 ```
 pip install promptbot
 ```
 
+if you want to also run the examples you need to install the example_requirements.txt file
+from the root directory of this repository:
+
+```
+pip install -r example_requirements.txt
+```
+
 ## Configuration
 
 To use `promptbot`, you need to create a `promptbot.toml` file in the root of your project directory with your OpenAI API key. 
 
 ```toml
 [openai]
 organization="org-YoUrOrGaNiZaTiOn"
```

### Comparing `promptbot-0.0.1a6/setup.py` & `promptbot-0.0.2a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 cwd = os.path.dirname(__file__)
 requirements = open(os.path.join(cwd, 'requirements.txt')).read()
 readme = open(os.path.join(cwd, 'README.md')).read()
 
 setup(
     name='promptbot',
-    version='0.0.1-alpha.6',
+    version='0.0.2-alpha.1',
     author='Clayton Bezuidenhout',
     author_email='claytonbez.nl@gmail.com',
     description='A Python package for generating prompt bots on top of OpenAI GTP Apis.',
     long_description=f"""{readme}""",
     long_description_content_type='text/markdown',
     packages=['promptbot'],
     install_requires=requirements,
```

