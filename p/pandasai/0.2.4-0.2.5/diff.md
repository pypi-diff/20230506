# Comparing `tmp/pandasai-0.2.4.tar.gz` & `tmp/pandasai-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.4.tar", max compression
+gzip compressed data, was "pandasai-0.2.5.tar", max compression
```

## Comparing `pandasai-0.2.4.tar` & `pandasai-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.4/LICENSE
--rw-r--r--   0        0        0     5247 2023-05-06 14:24:46.810520 pandasai-0.2.4/README.md
--rw-r--r--   0        0        0     6453 2023-05-06 14:24:46.811042 pandasai-0.2.4/pandasai/__init__.py
--rw-r--r--   0        0        0      107 2023-05-06 12:44:40.585715 pandasai-0.2.4/pandasai/constants.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.4/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.4/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.4/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.4/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1466 2023-05-06 14:21:04.361561 pandasai-0.2.4/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3210 2023-05-06 12:44:40.586309 pandasai-0.2.4/pandasai/llm/base.py
--rw-r--r--   0        0        0     1373 2023-05-06 12:44:40.586634 pandasai-0.2.4/pandasai/llm/base_hf.py
--rw-r--r--   0        0        0      478 2023-05-04 23:23:32.559995 pandasai-0.2.4/pandasai/llm/fake.py
--rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.4/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3815 2023-05-05 23:28:00.731241 pandasai-0.2.4/pandasai/llm/openai.py
--rw-r--r--   0        0        0      668 2023-05-06 12:44:40.587820 pandasai-0.2.4/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0      695 2023-05-06 14:24:58.661027 pandasai-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6056 1970-01-01 00:00:00.000000 pandasai-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5641 2023-05-06 14:25:32.707401 pandasai-0.2.5/README.md
+-rw-r--r--   0        0        0     6656 2023-05-06 14:25:32.707820 pandasai-0.2.5/pandasai/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-06 12:44:40.585715 pandasai-0.2.5/pandasai/constants.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.5/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.5/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4513 2023-05-06 14:25:32.708135 pandasai-0.2.5/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.5/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.5/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1466 2023-05-06 14:21:04.361561 pandasai-0.2.5/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3210 2023-05-06 12:44:40.586309 pandasai-0.2.5/pandasai/llm/base.py
+-rw-r--r--   0        0        0     1373 2023-05-06 12:44:40.586634 pandasai-0.2.5/pandasai/llm/base_hf.py
+-rw-r--r--   0        0        0      478 2023-05-04 23:23:32.559995 pandasai-0.2.5/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.5/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3815 2023-05-05 23:28:00.731241 pandasai-0.2.5/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      668 2023-05-06 12:44:40.587820 pandasai-0.2.5/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0      695 2023-05-06 14:25:48.769779 pandasai-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 pandasai-0.2.5/PKG-INFO
```

### Comparing `pandasai-0.2.4/LICENSE` & `pandasai-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/README.md` & `pandasai-0.2.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -81,14 +81,20 @@
 )
 ```
 
 ![Chart](images/histogram-chart.png?raw=true)
 
 You can find more examples in the [examples](examples) directory.
 
+## Privacy & Security
+In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
+
+Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
+
+
 ## Environment Variables
 
 In order to set the API key for the LLM (Hugging Face Hub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
 
 ```bash
 cp .env.example .env
 ```
```

### Comparing `pandasai-0.2.4/pandasai/__init__.py` & `pandasai-0.2.5/pandasai/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import sys
 from typing import Optional
 
 import pandas as pd
 
 from .constants import END_CODE_TAG, START_CODE_TAG
 from .exceptions import LLMNotFoundError
+from .helpers.anonymizer import anonymize_dataframe_head
 from .helpers.notebook import Notebook
 from .llm.base import LLM
 
 
-# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-instance-attributes disable=too-many-arguments
 class PandasAI:
     """PandasAI is a wrapper around a LLM to make dataframes conversational"""
 
     _task_instruction: str = """
 There is a dataframe in pandas (python).
 The name of the dataframe is `df`.
 This is the result of `print(df.head({rows_to_display}))`:
@@ -84,31 +85,37 @@
 
     def run(
         self,
         data_frame: pd.DataFrame,
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
+        anonymize_df: bool = True,
     ) -> str:
         """Run the LLM with the given prompt"""
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
         rows_to_display = 0 if self._enforce_privacy else 5
+
+        df_head = data_frame.head(rows_to_display)
+        if anonymize_df:
+            df_head = anonymize_dataframe_head(df_head)
+
         code = self._llm.generate_code(
             self._task_instruction.format(
-                df_head=data_frame.head(rows_to_display),
+                df_head=df_head,
                 rows_to_display=rows_to_display,
                 START_CODE_TAG=START_CODE_TAG,
                 END_CODE_TAG=END_CODE_TAG,
             ),
             prompt,
         )
         self._original_instruction_and_prompt = (
             self._task_instruction.format(
-                df_head=data_frame.head(rows_to_display),
+                df_head=df_head,
                 rows_to_display=rows_to_display,
                 START_CODE_TAG=START_CODE_TAG,
                 END_CODE_TAG=END_CODE_TAG,
             )
             + prompt
         )
         self.last_code_generated = code
```

### Comparing `pandasai-0.2.4/pandasai/exceptions.py` & `pandasai-0.2.5/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/pandasai/helpers/notebook.py` & `pandasai-0.2.5/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/pandasai/llm/alpaca.py` & `pandasai-0.2.5/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/pandasai/llm/base.py` & `pandasai-0.2.5/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/pandasai/llm/base_hf.py` & `pandasai-0.2.5/pandasai/llm/base_hf.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/pandasai/llm/open_assistant.py` & `pandasai-0.2.5/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/pandasai/llm/openai.py` & `pandasai-0.2.5/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/pandasai/llm/starcoder.py` & `pandasai-0.2.5/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.4/pyproject.toml` & `pandasai-0.2.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.4"
+version = "0.2.5"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.2.4/PKG-INFO` & `pandasai-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -101,14 +101,20 @@
 )
 ```
 
 ![Chart](images/histogram-chart.png?raw=true)
 
 You can find more examples in the [examples](examples) directory.
 
+## Privacy & Security
+In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
+
+Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
+
+
 ## Environment Variables
 
 In order to set the API key for the LLM (Hugging Face Hub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
 
 ```bash
 cp .env.example .env
 ```
```

