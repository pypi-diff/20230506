# Comparing `tmp/pandasai-0.2.2.tar.gz` & `tmp/pandasai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.2.tar", max compression
+gzip compressed data, was "pandasai-0.2.3.tar", max compression
```

## Comparing `pandasai-0.2.2.tar` & `pandasai-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.2/LICENSE
--rw-r--r--   0        0        0     4396 2023-05-02 22:59:27.189355 pandasai-0.2.2/README.md
--rw-r--r--   0        0        0     6249 2023-05-03 14:53:42.378833 pandasai-0.2.2/pandasai/__init__.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.2/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.2/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.2/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.2/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.2.2/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3128 2023-05-02 20:00:39.808930 pandasai-0.2.2/pandasai/llm/base.py
--rw-r--r--   0        0        0      439 2023-04-30 23:42:14.083716 pandasai-0.2.2/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1167 2023-04-30 10:29:36.204761 pandasai-0.2.2/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3767 2023-05-02 20:00:39.809160 pandasai-0.2.2/pandasai/llm/openai.py
--rw-r--r--   0        0        0      677 2023-05-03 14:55:44.337550 pandasai-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5205 1970-01-01 00:00:00.000000 pandasai-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5247 2023-05-05 23:28:03.924620 pandasai-0.2.3/README.md
+-rw-r--r--   0        0        0     6453 2023-05-05 23:28:03.925325 pandasai-0.2.3/pandasai/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-05 23:28:03.925793 pandasai-0.2.3/pandasai/constants.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.3/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.3/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.3/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.3/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1466 2023-04-30 23:41:22.772250 pandasai-0.2.3/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3210 2023-05-05 23:28:03.926281 pandasai-0.2.3/pandasai/llm/base.py
+-rw-r--r--   0        0        0     1373 2023-05-05 23:28:03.926613 pandasai-0.2.3/pandasai/llm/base_hf.py
+-rw-r--r--   0        0        0      478 2023-05-04 23:23:32.559995 pandasai-0.2.3/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      755 2023-05-05 23:28:03.927032 pandasai-0.2.3/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3815 2023-05-05 23:28:00.731241 pandasai-0.2.3/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      668 2023-05-05 23:28:03.927474 pandasai-0.2.3/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0      695 2023-05-05 23:30:04.467535 pandasai-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6056 1970-01-01 00:00:00.000000 pandasai-0.2.3/PKG-INFO
```

### Comparing `pandasai-0.2.2/LICENSE` & `pandasai-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.2/README.md` & `pandasai-0.2.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # PandasAI 🐼
 
+[![release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![lint](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai/month)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
 Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
 
@@ -21,56 +22,58 @@
 
 ```bash
 pip install pandasai
 ```
 
 ## Usage
 
+> Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
+
 PandasAI is designed to be used in conjunction with Pandas. It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of Pandas DataFrames. For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
 from pandasai import PandasAI
 
 # Sample DataFrame
 df = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
-    "gdp": [21400000, 2940000, 2830000, 3870000, 2160000, 1350000, 1780000, 1320000, 516000, 14000000],
-    "happiness_index": [7.3, 7.2, 6.5, 7.0, 6.0, 6.3, 7.3, 7.3, 5.9, 5.0]
+    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 # Instantiate a LLM
 from pandasai.llm.openai import OpenAI
 llm = OpenAI()
 
 pandas_ai = PandasAI(llm)
 pandas_ai.run(df, prompt='Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
-0     United States
 6            Canada
 7         Australia
 1    United Kingdom
 3           Germany
+0     United States
 Name: country, dtype: object
 ```
 
 Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
 
 ```python
 pandas_ai.run(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
 ```
 
 The above code will return the following:
 
 ```
-14516000
+19012600725504
 ```
 
 You can also ask PandasAI to draw a graph:
 
 ```python
 pandas_ai.run(
     df,
@@ -94,27 +97,33 @@
 
 As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
 
 ```python
 # OpenAI
 llm = OpenAI(api_token="YOUR_OPENAI_API_KEY")
 
-# OpenAssistant
-llm = OpenAssistant(api_token="YOUR_HF_API_KEY")
+# Starcoder
+llm = Starcoder(api_token="YOUR_HF_API_KEY")
 ```
 
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
 For more information, please see the [contributing guidelines](CONTRIBUTING.md).
 
+After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
+
+```bash
+pre-commit install
+```
+
 ### Todo
 
 - [ ] Add support for more LLMs
 - [ ] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add unit tests
 - [ ] Add contributing guidelines
```

### Comparing `pandasai-0.2.2/pandasai/__init__.py` & `pandasai-0.2.3/pandasai/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """ PandasAI is a wrapper around a LLM to make dataframes convesational """
 import io
 import sys
+from typing import Optional
+
 import pandas as pd
-from .llm.base import LLM
-from .helpers.notebook import Notebook
+
+from .constants import END_CODE_TAG, START_CODE_TAG
 from .exceptions import LLMNotFoundError
+from .helpers.notebook import Notebook
+from .llm.base import LLM
 
 
+# pylint: disable=too-many-instance-attributes
 class PandasAI:
-    """PandasAI is a wrapper around a LLM to make dataframes convesational"""
+    """PandasAI is a wrapper around a LLM to make dataframes conversational"""
 
     _task_instruction: str = """
 There is a dataframe in pandas (python).
 The name of the dataframe is `df`.
 This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
 
-Return the python code (do not import anything) and make sure to prefix the python code with <startCode> exactly and suffix the code with <endCode> exactly 
+Return the python code (do not import anything) and make sure to prefix the python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly 
 to get the answer to the following question :
 """
     _response_instruction: str = """
 Question: {question}
 Answer: {answer}
 
 Rewrite the answer to the question in a conversational way.
@@ -30,25 +35,25 @@
     For the task defined below:
     {orig_task}
     you generated this python code:
     {code}
     and this fails with the following error:
     {error_returned}
     Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error.
-    Make sure to prefix the python code with <startCode> exactly and suffix the code with <endCode> exactly.
+    Make sure to prefix the python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
     """
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = True
     _enforce_privacy: bool = False
     _max_retries: int = 3
     _original_instruction_and_prompt = None
     _is_notebook: bool = False
-    last_code_generated: str = None
-    code_output: str = None
+    last_code_generated: Optional[str] = None
+    code_output: Optional[str] = None
 
     def __init__(
         self,
         llm=None,
         conversational=True,
         verbose=False,
         enforce_privacy=False,
@@ -83,29 +88,30 @@
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
     ) -> str:
         """Run the LLM with the given prompt"""
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
-        rows_to_display = 5
-        if self._enforce_privacy:
-            rows_to_display = 0
-
+        rows_to_display = 0 if self._enforce_privacy else 5
         code = self._llm.generate_code(
             self._task_instruction.format(
                 df_head=data_frame.head(rows_to_display),
                 rows_to_display=rows_to_display,
+                START_CODE_TAG=START_CODE_TAG,
+                END_CODE_TAG=END_CODE_TAG,
             ),
             prompt,
         )
         self._original_instruction_and_prompt = (
             self._task_instruction.format(
                 df_head=data_frame.head(rows_to_display),
                 rows_to_display=rows_to_display,
+                START_CODE_TAG=START_CODE_TAG,
+                END_CODE_TAG=END_CODE_TAG,
             )
             + prompt
         )
         self.last_code_generated = code
         self.log(
             f"""
 Code generated:
@@ -168,20 +174,17 @@
         sys.stdout = sys.__stdout__
         captured_output = output.getvalue()
 
         # Evaluate the last line and return its value or the captured output
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
         if last_line.startswith("print(") and last_line.endswith(")"):
-            # Last line is already printing
-            return eval(last_line[6:-1])
-        # Evaluate last line and return its value or the captured output
+            last_line = last_line[6:-1]
         try:
-            result = eval(last_line)
-            return result
-        except:
+            return eval(last_line)
+        except Exception:  # pylint: disable=W0718
             return captured_output
 
     def log(self, message: str):
         """Log a message"""
         if self._verbose:
             print(message)
```

### Comparing `pandasai-0.2.2/pandasai/exceptions.py` & `pandasai-0.2.3/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.2/pandasai/helpers/notebook.py` & `pandasai-0.2.3/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.2/pandasai/llm/alpaca.py` & `pandasai-0.2.3/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.2/pandasai/llm/base.py` & `pandasai-0.2.3/pandasai/llm/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """ Base class to implement a new LLM. """
 
-import re
 import ast
+import re
+from typing import Optional
+
 import astor
+
+from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
-    NoCodeFoundError,
     MethodNotImplementedError,
+    NoCodeFoundError,
 )
 
 
 class LLM:
     """Base class to implement a new LLM."""
 
-    last_prompt: str = None
+    last_prompt: Optional[str] = None
 
     @property
     def type(self) -> str:
         """
         Return type of LLM.
 
         Raises:
@@ -26,20 +30,19 @@
         Returns:
             str: Type of LLM a string
         """
         raise APIKeyNotFoundError("Type has not been implemented")
 
     def _remove_imports(self, code: str) -> str:
         tree = ast.parse(code)
-        new_body = []
-
-        for node in tree.body:
-            if not isinstance(node, (ast.Import, ast.ImportFrom)):
-                new_body.append(node)
-
+        new_body = [
+            node
+            for node in tree.body
+            if not isinstance(node, (ast.Import, ast.ImportFrom))
+        ]
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree)
 
     def _polish_code(self, code: str) -> str:
         """
         Polish the code by removing the leading "python" or "py",  \
         removing the imports and removing trailing spaces and new lines.
@@ -78,16 +81,17 @@
 
         Returns:
             str: Extracted code from the response
         """
         code = response
         if len(response.split(separator)) > 1:
             code = response.split(separator)[1]
-        if re.match(r"<startCode>([\s\S]*?)<\/?endCode>", code):
-            code = re.findall(r"<startCode>([\s\S]*?)<\/?endCode>", code)[0]
+        match = re.search(rf"{START_CODE_TAG}(.*){END_CODE_TAG}", code, re.DOTALL)
+        if match:
+            code = match.group(1).strip()
         code = self._polish_code(code)
         if not self._is_python_code(code):
             raise NoCodeFoundError("No code found in the response")
 
         return code
 
     def call(self, instruction: str, value: str) -> None:
```

### Comparing `pandasai-0.2.2/pandasai/llm/openai.py` & `pandasai-0.2.3/pandasai/llm/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """OpenAI LLM"""
 
 import os
-from dotenv import load_dotenv
+from typing import Optional
+
 import openai
-from .base import LLM
+from dotenv import load_dotenv
+
 from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
+from .base import LLM
 
 load_dotenv()
 
 
 class OpenAI(LLM):
     """OpenAI LLM"""
 
@@ -25,19 +28,19 @@
     api_token: str
     model: str = "gpt-3.5-turbo"
     temperature: float = 0
     max_tokens: int = 512
     top_p: float = 1
     frequency_penalty: float = 0
     presence_penalty: float = 0.6
-    stop: str = None
+    stop: Optional[str] = None
 
     def __init__(
         self,
-        api_token: str = None,
+        api_token: Optional[str] = None,
         **kwargs,
     ):
         self.api_token = api_token or os.getenv("OPENAI_API_KEY")
         if self.api_token is None:
             raise APIKeyNotFoundError("OpenAI API key is required")
         openai.api_key = self.api_token
 
@@ -55,15 +58,15 @@
         ]
         for key, value in kwargs.items():
             if key in valid_params:
                 setattr(self, key, value)
 
     def completion(self, prompt: str) -> str:
         """
-        Query the completation API
+        Query the completion API
 
         Args:
             prompt (str): Prompt
 
         Returns:
             str: LLM response
         """
```

### Comparing `pandasai-0.2.2/pyproject.toml` & `pandasai-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.2"
+version = "0.2.3"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -18,11 +18,12 @@
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 pylint = "^2.17.3"
 pytest = "^7.3.1"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pandasai-0.2.2/PKG-INFO` & `pandasai-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.2
+Version: 0.2.3
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PandasAI 🐼
 
+[![release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![lint](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai/month)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
 Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
 
@@ -41,56 +42,58 @@
 
 ```bash
 pip install pandasai
 ```
 
 ## Usage
 
+> Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
+
 PandasAI is designed to be used in conjunction with Pandas. It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of Pandas DataFrames. For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
 from pandasai import PandasAI
 
 # Sample DataFrame
 df = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
-    "gdp": [21400000, 2940000, 2830000, 3870000, 2160000, 1350000, 1780000, 1320000, 516000, 14000000],
-    "happiness_index": [7.3, 7.2, 6.5, 7.0, 6.0, 6.3, 7.3, 7.3, 5.9, 5.0]
+    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
+    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 # Instantiate a LLM
 from pandasai.llm.openai import OpenAI
 llm = OpenAI()
 
 pandas_ai = PandasAI(llm)
 pandas_ai.run(df, prompt='Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
-0     United States
 6            Canada
 7         Australia
 1    United Kingdom
 3           Germany
+0     United States
 Name: country, dtype: object
 ```
 
 Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
 
 ```python
 pandas_ai.run(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
 ```
 
 The above code will return the following:
 
 ```
-14516000
+19012600725504
 ```
 
 You can also ask PandasAI to draw a graph:
 
 ```python
 pandas_ai.run(
     df,
@@ -114,27 +117,33 @@
 
 As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
 
 ```python
 # OpenAI
 llm = OpenAI(api_token="YOUR_OPENAI_API_KEY")
 
-# OpenAssistant
-llm = OpenAssistant(api_token="YOUR_HF_API_KEY")
+# Starcoder
+llm = Starcoder(api_token="YOUR_HF_API_KEY")
 ```
 
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
 For more information, please see the [contributing guidelines](CONTRIBUTING.md).
 
+After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
+
+```bash
+pre-commit install
+```
+
 ### Todo
 
 - [ ] Add support for more LLMs
 - [ ] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add unit tests
 - [ ] Add contributing guidelines
```

