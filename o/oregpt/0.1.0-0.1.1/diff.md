# Comparing `tmp/oregpt-0.1.0.tar.gz` & `tmp/oregpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oregpt-0.1.0.tar", max compression
+gzip compressed data, was "oregpt-0.1.1.tar", max compression
```

## Comparing `oregpt-0.1.0.tar` & `oregpt-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2023-05-02 02:51:46.385578 oregpt-0.1.0/LICENSE
--rw-r--r--   0        0        0     1742 2023-05-05 01:47:58.064901 oregpt-0.1.0/README.md
--rw-r--r--   0        0        0     2261 2023-05-05 01:26:45.664901 oregpt-0.1.0/oregpt/chat_bot.py
--rw-r--r--   0        0        0     2236 2023-05-05 01:26:45.664901 oregpt-0.1.0/oregpt/main.py
--rw-r--r--   0        0        0     1003 2023-05-05 01:26:45.664901 oregpt-0.1.0/oregpt/stdinout.py
--rw-r--r--   0        0        0     1819 2023-05-05 01:26:45.664901 oregpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2614 1970-01-01 00:00:00.000000 oregpt-0.1.0/setup.py
--rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 oregpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-02 02:51:46.385578 oregpt-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2037 2023-05-06 07:13:10.385157 oregpt-0.1.1/README.md
+-rw-r--r--   0        0        0     2302 2023-05-06 07:12:20.995157 oregpt-0.1.1/oregpt/chat_bot.py
+-rw-r--r--   0        0        0     2072 2023-05-06 07:12:20.995157 oregpt-0.1.1/oregpt/main.py
+-rw-r--r--   0        0        0     2232 2023-05-06 07:12:20.995157 oregpt-0.1.1/oregpt/stdinout.py
+-rw-r--r--   0        0        0     1819 2023-05-06 07:12:43.525157 oregpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 oregpt-0.1.1/setup.py
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 oregpt-0.1.1/PKG-INFO
```

### Comparing `oregpt-0.1.0/LICENSE` & `oregpt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oregpt-0.1.0/README.md` & `oregpt-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # oregpt
-A tiny GPT CLI tool.
-You can chat with the GPT model developped by OpenAI and save the conversation as json.
-
 ![workflow](https://github.com/shinichi-takayanagi/oregpt/actions/workflows/main.yml/badge.svg)
 [![license](https://img.shields.io/github/license/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/blob/master/LICENSE)
 [![release](https://img.shields.io/github/release/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/releases/latest)
 [![python-version](https://img.shields.io/pypi/pyversions/oregpt.svg)](https://pypi.org/project/oregpt/)
 [![pypi](https://img.shields.io/pypi/v/oregpt?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oregpt)
 
-![oregpt](https://user-images.githubusercontent.com/24406372/236361796-4a38af2b-b7b6-48e3-8ab6-dcba0be1532f.gif)
+A tiny GPT CLI tool.
+You can chat with the GPT model developped by OpenAI and save the conversation as json.
+
+![oregpt](https://user-images.githubusercontent.com/24406372/236609166-0f2385b1-fd9e-4810-b80d-c19c44d13411.gif)
 
 ## Installation
 ### Get your own OpenAI API Key
 Assuming you have an environment variable with key named `OPENAI_API_KEY`.
 If you don't have a OpenAI API key [visit here](https://platform.openai.com/account/api-keys), generate one and add it as an environment variable
 
 ```bash
@@ -30,20 +30,30 @@
 ## Usage
 Once you have installed oregpt, you can run it by typing:
 ```bash
 $ oregpt
 ```
 
 ## Configuration
-You can specify the place of conversation `log` , style (color etc) and the model provided by OpenAI in `~/.oregpt/config.yml`
-```
+You can specify the place of conversation `log`,
+[style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)
+and
+[the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)
+in `~/.oregpt/config.yml`
+```yaml
 ❯ cat ~/.oregpt/config.yml
 log: /tmp/oregpt/
 openai:
     model: gpt-3.5-turbo
 # You can also specify OpenAI's API key here
 #     api_key: <your-api-key>
-style:
-    user: "#00BEFE"
-    assistant: "#87CEEB"
-    system: "#cc0000"
+character:
+    user:
+        name: Me
+        style: "#00BEFE"
+    assistant:
+        name: AI
+        style: "#87CEEB"
+    system:
+        name: System
+        style: "#cc0000"
 ```
```

### Comparing `oregpt-0.1.0/oregpt/chat_bot.py` & `oregpt-0.1.1/oregpt/chat_bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,24 +27,25 @@
         # https://community.openai.com/t/the-system-role-how-it-influences-the-chat-behavior/87353
         # https://learn.microsoft.com/ja-jp/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions#system-role
         # self._log = [{"role": "system", "content": f"You are a chat bot."}]
         self._log: list[dict[str, str]] = []
 
     def respond(self, message: str) -> str:
         self._log.append({"role": "user", "content": message})
-        # API Reference: https://platform.openai.com/docs/api-reference/completions/create
-        response = openai.ChatCompletion.create(
-            model=self._model,
-            messages=self._log,
-            max_tokens=1024,
-            temperature=0,
-            stream=True,
-        )
+        with self._std_in_out.print_assistant_thinking():
+            # API Reference: https://platform.openai.com/docs/api-reference/completions/create
+            response = openai.ChatCompletion.create(
+                model=self._model,
+                messages=self._log,
+                max_tokens=1024,
+                temperature=0,
+                stream=True,
+            )
+
         content = ""
-        self._std_in_out.print_assistant_prefix()
         for chunk in response:
             chunked_content = chunk["choices"][0]["delta"].get("content", "")
             self._std_in_out.print_assistant(chunked_content)
             content += chunked_content
         self._std_in_out.print_assistant("\n")
         self._log.append({"role": "assistant", "content": content})
         return content
```

### Comparing `oregpt-0.1.0/oregpt/main.py` & `oregpt-0.1.1/oregpt/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,46 +28,38 @@
     if value := os.getenv("OPENAI_API_KEY"):
         openai.api_key = value
         return
 
     raise LookupError("OpenAI's API key was not found in config.yml and environment variables")
 
 
-def make_std_in_out(config: dict[str, Any]) -> StdInOut:
-    return StdInOut(
-        Style.from_dict(
-            {
-                "": config["user"],  # Default color which is used for "input" should be the same with user
-                "user": config["user"],
-                "assistant": config["assistant"],
-                "system": config["system"],
-            }
-        ),
-        lambda: "To exit, type q, quit or exit",
-    )
-
-
-def main() -> None:
+def main() -> int:
     config = load_config()
     initialize_open_ai_key(config["openai"])
-    std_in_out = make_std_in_out(config["style"])
+    std_in_out = StdInOut(config["character"], lambda: "To exit, type q, quit, exit, or Ctrl + C")
     bot = ChatBot(config["openai"]["model"], std_in_out)
 
-    while True:
-        text = std_in_out.input().lower()
-        match text:
-            case "exit" | "quit" | "q":
-                break
-            case "clear":
-                bot.clear()
-                std_in_out.print_system("Clear all conversation history")
-            case "history":
-                std_in_out.print_system(str(bot.log))
-            case "save":
-                file_name = bot.save(config["log"])
-                std_in_out.print_system(f"Save all conversation history in {file_name}")
-            case _:
-                bot.respond(text)
+    try:
+        while True:
+            message = std_in_out.input().lower()
+            match message:
+                case "exit" | "quit" | "q":
+                    break
+                case "clear":
+                    bot.clear()
+                    std_in_out.print_system("Clear all conversation history")
+                case "history":
+                    std_in_out.print_system(str(bot.log))
+                case "save":
+                    file_name = bot.save(config["log"])
+                    std_in_out.print_system(f"Save all conversation history in {file_name}")
+                case _:
+                    bot.respond(message)
+    except KeyboardInterrupt:
+        return 0
+    except Exception as e:
+        raise Exception(f"Something happened: {str(e)}") from e
+    return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `oregpt-0.1.0/pyproject.toml` & `oregpt-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oregpt"
-version = "0.1.0"
+version = "0.1.1"
 description = "A tiny GPT CLI tool"
 authors = ["Shinichi Takayanagi <shinichi.takayanagi@gmail.com>"]
 homepage = "https://github.com/shinichi-takayanagi/oregpt"
 repository = "https://github.com/shinichi-takayanagi/oregpt"
 license = "MIT"
 readme = "README.md"
 keywords = ["gpt-chatbot", "gpt-cli", "openai-cli"]
```

### Comparing `oregpt-0.1.0/setup.py` & `oregpt-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['openai>=0.27.6,<0.28.0', 'prompt-toolkit>=3.0.38,<4.0.0', 'pyyaml>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['oregpt = oregpt.main:main']}
 
 setup_kwargs = {
     'name': 'oregpt',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A tiny GPT CLI tool',
-    'long_description': '# oregpt\nA tiny GPT CLI tool.\nYou can chat with the GPT model developped by OpenAI and save the conversation as json.\n\n![workflow](https://github.com/shinichi-takayanagi/oregpt/actions/workflows/main.yml/badge.svg)\n[![license](https://img.shields.io/github/license/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/blob/master/LICENSE)\n[![release](https://img.shields.io/github/release/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/releases/latest)\n[![python-version](https://img.shields.io/pypi/pyversions/oregpt.svg)](https://pypi.org/project/oregpt/)\n[![pypi](https://img.shields.io/pypi/v/oregpt?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oregpt)\n\n![oregpt](https://user-images.githubusercontent.com/24406372/236361796-4a38af2b-b7b6-48e3-8ab6-dcba0be1532f.gif)\n\n## Installation\n### Get your own OpenAI API Key\nAssuming you have an environment variable with key named `OPENAI_API_KEY`.\nIf you don\'t have a OpenAI API key [visit here](https://platform.openai.com/account/api-keys), generate one and add it as an environment variable\n\n```bash\nexport OPENAI_API_KEY=<YOUR-OPENAI-API-KEY>\n\n```\n\n### Instal from PyPI\nYou can install the package using pip:\n\n```bash\n$ pip install oregpt\n```\n\n## Usage\nOnce you have installed oregpt, you can run it by typing:\n```bash\n$ oregpt\n```\n\n## Configuration\nYou can specify the place of conversation `log` , style (color etc) and the model provided by OpenAI in `~/.oregpt/config.yml`\n```\n❯ cat ~/.oregpt/config.yml\nlog: /tmp/oregpt/\nopenai:\n    model: gpt-3.5-turbo\n# You can also specify OpenAI\'s API key here\n#     api_key: <your-api-key>\nstyle:\n    user: "#00BEFE"\n    assistant: "#87CEEB"\n    system: "#cc0000"\n```\n',
+    'long_description': '# oregpt\n![workflow](https://github.com/shinichi-takayanagi/oregpt/actions/workflows/main.yml/badge.svg)\n[![license](https://img.shields.io/github/license/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/blob/master/LICENSE)\n[![release](https://img.shields.io/github/release/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/releases/latest)\n[![python-version](https://img.shields.io/pypi/pyversions/oregpt.svg)](https://pypi.org/project/oregpt/)\n[![pypi](https://img.shields.io/pypi/v/oregpt?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oregpt)\n\nA tiny GPT CLI tool.\nYou can chat with the GPT model developped by OpenAI and save the conversation as json.\n\n![oregpt](https://user-images.githubusercontent.com/24406372/236609166-0f2385b1-fd9e-4810-b80d-c19c44d13411.gif)\n\n## Installation\n### Get your own OpenAI API Key\nAssuming you have an environment variable with key named `OPENAI_API_KEY`.\nIf you don\'t have a OpenAI API key [visit here](https://platform.openai.com/account/api-keys), generate one and add it as an environment variable\n\n```bash\nexport OPENAI_API_KEY=<YOUR-OPENAI-API-KEY>\n\n```\n\n### Instal from PyPI\nYou can install the package using pip:\n\n```bash\n$ pip install oregpt\n```\n\n## Usage\nOnce you have installed oregpt, you can run it by typing:\n```bash\n$ oregpt\n```\n\n## Configuration\nYou can specify the place of conversation `log`,\n[style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)\nand\n[the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)\nin `~/.oregpt/config.yml`\n```yaml\n❯ cat ~/.oregpt/config.yml\nlog: /tmp/oregpt/\nopenai:\n    model: gpt-3.5-turbo\n# You can also specify OpenAI\'s API key here\n#     api_key: <your-api-key>\ncharacter:\n    user:\n        name: Me\n        style: "#00BEFE"\n    assistant:\n        name: AI\n        style: "#87CEEB"\n    system:\n        name: System\n        style: "#cc0000"\n```\n',
     'author': 'Shinichi Takayanagi',
     'author_email': 'shinichi.takayanagi@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/shinichi-takayanagi/oregpt',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `oregpt-0.1.0/PKG-INFO` & `oregpt-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oregpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tiny GPT CLI tool
 Home-page: https://github.com/shinichi-takayanagi/oregpt
 License: MIT
 Keywords: gpt-chatbot,gpt-cli,openai-cli
 Author: Shinichi Takayanagi
 Author-email: shinichi.takayanagi@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -18,24 +18,24 @@
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/shinichi-takayanagi/oregpt
 Description-Content-Type: text/markdown
 
 # oregpt
-A tiny GPT CLI tool.
-You can chat with the GPT model developped by OpenAI and save the conversation as json.
-
 ![workflow](https://github.com/shinichi-takayanagi/oregpt/actions/workflows/main.yml/badge.svg)
 [![license](https://img.shields.io/github/license/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/blob/master/LICENSE)
 [![release](https://img.shields.io/github/release/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/releases/latest)
 [![python-version](https://img.shields.io/pypi/pyversions/oregpt.svg)](https://pypi.org/project/oregpt/)
 [![pypi](https://img.shields.io/pypi/v/oregpt?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oregpt)
 
-![oregpt](https://user-images.githubusercontent.com/24406372/236361796-4a38af2b-b7b6-48e3-8ab6-dcba0be1532f.gif)
+A tiny GPT CLI tool.
+You can chat with the GPT model developped by OpenAI and save the conversation as json.
+
+![oregpt](https://user-images.githubusercontent.com/24406372/236609166-0f2385b1-fd9e-4810-b80d-c19c44d13411.gif)
 
 ## Installation
 ### Get your own OpenAI API Key
 Assuming you have an environment variable with key named `OPENAI_API_KEY`.
 If you don't have a OpenAI API key [visit here](https://platform.openai.com/account/api-keys), generate one and add it as an environment variable
 
 ```bash
@@ -53,21 +53,31 @@
 ## Usage
 Once you have installed oregpt, you can run it by typing:
 ```bash
 $ oregpt
 ```
 
 ## Configuration
-You can specify the place of conversation `log` , style (color etc) and the model provided by OpenAI in `~/.oregpt/config.yml`
-```
+You can specify the place of conversation `log`,
+[style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)
+and
+[the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)
+in `~/.oregpt/config.yml`
+```yaml
 ❯ cat ~/.oregpt/config.yml
 log: /tmp/oregpt/
 openai:
     model: gpt-3.5-turbo
 # You can also specify OpenAI's API key here
 #     api_key: <your-api-key>
-style:
-    user: "#00BEFE"
-    assistant: "#87CEEB"
-    system: "#cc0000"
+character:
+    user:
+        name: Me
+        style: "#00BEFE"
+    assistant:
+        name: AI
+        style: "#87CEEB"
+    system:
+        name: System
+        style: "#cc0000"
 ```
```

