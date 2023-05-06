# Comparing `tmp/pypreql-nlp-0.0.1.tar.gz` & `tmp/pypreql-nlp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-nlp-0.0.1.tar", last modified: Sat May  6 15:10:48 2023, max compression
+gzip compressed data, was "pypreql-nlp-0.0.2.tar", last modified: Sat May  6 16:14:21 2023, max compression
```

## Comparing `pypreql-nlp-0.0.1.tar` & `pypreql-nlp-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 15:10:48.306183 pypreql-nlp-0.0.1/
--rw-rw-rw-   0        0        0     2088 2023-05-06 15:10:48.294185 pypreql-nlp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-05-06 14:32:52.000000 pypreql-nlp-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 15:10:48.213563 pypreql-nlp-0.0.1/preql_nlp/
--rw-rw-rw-   0        0        0      170 2023-05-06 14:36:25.000000 pypreql-nlp-0.0.1/preql_nlp/__init__.py
--rw-rw-rw-   0        0        0       87 2023-05-03 00:35:57.000000 pypreql-nlp-0.0.1/preql_nlp/constants.py
--rw-rw-rw-   0        0        0     6253 2023-05-06 14:36:33.000000 pypreql-nlp-0.0.1/preql_nlp/main.py
--rw-rw-rw-   0        0        0      691 2023-05-06 13:22:05.000000 pypreql-nlp-0.0.1/preql_nlp/monkeypatch.py
-drwxrwxrwx   0        0        0        0 2023-05-06 15:10:48.255781 pypreql-nlp-0.0.1/preql_nlp/prompts/
--rw-rw-rw-   0        0        0      311 2023-05-03 00:57:14.000000 pypreql-nlp-0.0.1/preql_nlp/prompts/__init__.py
--rw-rw-rw-   0        0        0     2577 2023-05-06 13:21:22.000000 pypreql-nlp-0.0.1/preql_nlp/prompts/final_selection.py
--rw-rw-rw-   0        0        0     1000 2023-05-06 13:22:43.000000 pypreql-nlp-0.0.1/preql_nlp/prompts/prompt_executor.py
--rw-rw-rw-   0        0        0     1340 2023-05-06 13:21:22.000000 pypreql-nlp-0.0.1/preql_nlp/prompts/query_semantic_extraction.py
--rw-rw-rw-   0        0        0     1390 2023-05-05 21:43:44.000000 pypreql-nlp-0.0.1/preql_nlp/prompts/semantic_to_tokens.py
-drwxrwxrwx   0        0        0        0 2023-05-06 15:10:48.291733 pypreql-nlp-0.0.1/pypreql_nlp.egg-info/
--rw-rw-rw-   0        0        0     2088 2023-05-06 15:10:48.000000 pypreql-nlp-0.0.1/pypreql_nlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-06 15:10:48.000000 pypreql-nlp-0.0.1/pypreql_nlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 15:10:48.000000 pypreql-nlp-0.0.1/pypreql_nlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-06 15:10:48.000000 pypreql-nlp-0.0.1/pypreql_nlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 15:10:48.000000 pypreql-nlp-0.0.1/pypreql_nlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       94 2023-04-21 23:15:17.000000 pypreql-nlp-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 15:10:48.307196 pypreql-nlp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1426 2023-05-06 13:21:22.000000 pypreql-nlp-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:14:21.158986 pypreql-nlp-0.0.2/preql_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/monkeypatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/preql_nlp/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/final_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/prompt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/query_semantic_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/semantic_to_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/setup.py
```

### Comparing `pypreql-nlp-0.0.1/PKG-INFO` & `pypreql-nlp-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: pypreql-nlp
-Version: 0.0.1
-Summary: NLP interface for pypreql.
-Home-page: 
-Author: 
-Author-email: pypreql-community@gmail.com
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
-## PreQL NLP
-
-Natural language interface for generating PreQL query objects.
-
-PreQL is easier for a large language model to interact with as it requires only extract relevant concepts from a text,
-classifying them as metrics or dimensions, and mapping them to what is available in a model.
-
-This makes it more testable and less prone to hallucination than generating SQL directly. 
-
-Requires setting the following environment variables
-- OPENAI_API_KEY
-- OPENAI_MODEL
-
-Recommended to use "gpt-3.5-turbo" or higher as the model.
-
-## Examples
-
-### Basic BQ example
-
-
-```python
-from trilogy_public_models import models
-from preql import Executor, default_engine, Dialect
-from preql_nlp import build_query
-
-# define the model we want to parse
-environment = models["bigquery.stack_overflow"]
-
-# set up preql executor
-# default bigquery executor requires local default credentials configured
-executor = Dialect.BIGQUERY.default_executor(environment= environment)
-
-# build a query off text and the selected model
-processed_query = build_query(
-    "How many questions are asked per year?",
-    environment,
-)
-
-# make sure we got reasonable outputs
-for concept in processed_query.output_columns:
-    print(concept.name)
-
-# and run that to get our answer
-results = executor.execute_query(processed_query)
-for row in results:
-    print(row)
-```
-
-
-
-## Setting Up Your Environment
-
-Recommend that you work in a virtual environment with requirements from both requirements.txt and requirements-test.txt installed. The latter is necessary to run
-tests (surprise). 
-
-Pypreql-nlp is python 3.10+
+Metadata-Version: 2.1
+Name: pypreql-nlp
+Version: 0.0.2
+Summary: NLP interface for pypreql.
+Home-page: 
+Author: 
+Author-email: pypreql-community@gmail.com
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+## PreQL NLP
+
+Natural language interface for generating PreQL query objects.
+
+PreQL is easier for a large language model to interact with as it requires only extract relevant concepts from a text,
+classifying them as metrics or dimensions, and mapping them to what is available in a model.
+
+This makes it more testable and less prone to hallucination than generating SQL directly. 
+
+Requires setting the following environment variables
+- OPENAI_API_KEY
+- OPENAI_MODEL
+
+Recommended to use "gpt-3.5-turbo" or higher as the model.
+
+## Examples
+
+### Basic BQ example
+
+
+```python
+from trilogy_public_models import models
+from preql import Executor, default_engine, Dialect
+from preql_nlp import build_query
+
+# define the model we want to parse
+environment = models["bigquery.stack_overflow"]
+
+# set up preql executor
+# default bigquery executor requires local default credentials configured
+executor = Dialect.BIGQUERY.default_executor(environment= environment)
+
+# build a query off text and the selected model
+processed_query = build_query(
+    "How many questions are asked per year?",
+    environment,
+)
+
+# make sure we got reasonable outputs
+for concept in processed_query.output_columns:
+    print(concept.name)
+
+# and run that to get our answer
+results = executor.execute_query(processed_query)
+for row in results:
+    print(row)
+```
+
+
+
+## Setting Up Your Environment
+
+Recommend that you work in a virtual environment with requirements from both requirements.txt and requirements-test.txt installed. The latter is necessary to run
+tests (surprise). 
+
+Pypreql-nlp is python 3.10+
```

### Comparing `pypreql-nlp-0.0.1/README.md` & `pypreql-nlp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.1/preql_nlp/monkeypatch.py` & `pypreql-nlp-0.0.2/preql_nlp/monkeypatch.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from promptimize.prompt_cases import BasePromptCase, utils
-
-# patched method while waiting for upstream PR to be merged
-
-def patch_promptimize():
-    def test(self):
-        test_results = []
-        for evaluator in self.evaluators:
-            result = evaluator(self.response)
-            if not (utils.is_numeric(result) and 0 <= result <= 1):
-                raise Exception("Value should be between 0 and 1")
-            test_results.append(result)
-
-        if len(test_results):
-            self.execution.score = sum(test_results) / len(test_results)
-            self.execution.results = test_results
-        self.was_tested = True
-
-
+from promptimize.prompt_cases import BasePromptCase, utils
+
+# patched method while waiting for upstream PR to be merged
+
+def patch_promptimize():
+    def test(self):
+        test_results = []
+        for evaluator in self.evaluators:
+            result = evaluator(self.response)
+            if not (utils.is_numeric(result) and 0 <= result <= 1):
+                raise Exception("Value should be between 0 and 1")
+            test_results.append(result)
+
+        if len(test_results):
+            self.execution.score = sum(test_results) / len(test_results)
+            self.execution.results = test_results
+        self.was_tested = True
+
+
     BasePromptCase.test = test
```

### Comparing `pypreql-nlp-0.0.1/preql_nlp/prompts/final_selection.py` & `pypreql-nlp-0.0.2/preql_nlp/prompts/final_selection.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-def process_concept(concept: str):
-    return concept
-
-
-def gen_selection_v1(concepts: list[str], question: str):
-    concept_string = ", ".join(
-        [f'"{process_concept(concept)}"' for concept in concepts]
-    )
-    return f"""
-System: You are a helpful AI that selects the most relevant matching concepts to answer a question from a provided list.
-
-Guidelines:
-* you can assume the user will always provide a list of phrases
-* you can assume the user will always provide a question
-* only return concepts provided by the user
-* concepts are dot seperated and in quotes, e.g. "sales" or "product.revenue"
-* return the concepts that together best match the user question
-* reason about each match step by step, e.g. "first match the concept 'product' to the word 'product' in the question, then match the concept 'revenue' to the word 'revenue' in the question, and together these enable aggregating revenue by year"
-The output should be a VALID JSON blob with the following keys and values:
-* matches: a list of concepts from the user provided list that together best match the 
-* reasoning: a string explaining your step by step reasoning for the matches
-User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "what product colors had the most revenue in 2024?"]
-System:
-{{"matches": ["product.color", "order.revenue.sum", "order.year" ],
-"reasoning": "product.color matches the user request for product colors, and order revenue sum would enable aggregating revenue to the color. Order year is required to filter to 2024." }}
-User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "What are the sales by state?"
-System:
-{{"matches": ["order.state", "order.revenue.sum"],
-"reasoning": "order.state is the best match for state when looking at revenue, and order.revenue.sum would enable aggregating revenue." }}
-User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"]  question: "What are the average sales by state?"
-System:
-{{"matches": ["order.state", "order.revenue.avg"],
-"reasoning": "order.state is the best match for state, and order.revenue.avg would capture average revenue." }}
-User: concepts:"[{concept_string}]" question: "{question}"
-System:
-
-"""
+def process_concept(concept: str):
+    return concept
+
+
+def gen_selection_v1(concepts: list[str], question: str):
+    concept_string = ", ".join(
+        [f'"{process_concept(concept)}"' for concept in concepts]
+    )
+    return f"""
+System: You are a helpful AI that selects the most relevant matching concepts to answer a question from a provided list.
+
+Guidelines:
+* you can assume the user will always provide a list of phrases
+* you can assume the user will always provide a question
+* only return concepts provided by the user
+* concepts are dot seperated and in quotes, e.g. "sales" or "product.revenue"
+* return the concepts that together best match the user question
+* reason about each match step by step, e.g. "first match the concept 'product' to the word 'product' in the question, then match the concept 'revenue' to the word 'revenue' in the question, and together these enable aggregating revenue by year"
+The output should be a VALID JSON blob with the following keys and values:
+* matches: a list of concepts from the user provided list that together best match the 
+* reasoning: a string explaining your step by step reasoning for the matches
+User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "what product colors had the most revenue in 2024?"]
+System:
+{{"matches": ["product.color", "order.revenue.sum", "order.year" ],
+"reasoning": "product.color matches the user request for product colors, and order revenue sum would enable aggregating revenue to the color. Order year is required to filter to 2024." }}
+User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "What are the sales by state?"
+System:
+{{"matches": ["order.state", "order.revenue.sum"],
+"reasoning": "order.state is the best match for state when looking at revenue, and order.revenue.sum would enable aggregating revenue." }}
+User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"]  question: "What are the average sales by state?"
+System:
+{{"matches": ["order.state", "order.revenue.avg"],
+"reasoning": "order.state is the best match for state, and order.revenue.avg would capture average revenue." }}
+User: concepts:"[{concept_string}]" question: "{question}"
+System:
+
+"""
```

### Comparing `pypreql-nlp-0.0.1/preql_nlp/prompts/query_semantic_extraction.py` & `pypreql-nlp-0.0.2/preql_nlp/prompts/query_semantic_extraction.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-def gen_extraction_prompt_v1(input: str):
-    return f"""
-System: You are a helpful AI that translates ambiguous business questions into structured outputs.
-For a provided question, you will determine if there are metrics or aggregates or dimensions,
-as well as any limit, order, of filtering. 
-
-The output should be a VALID JSON blob with the following keys and values:
-- metrics: a list of concepts from the question that should be aggregated
-- dimensions: a list of concepts from the question which are not metrics
-- limit: a number of records to limit the results to, -1 if none specified
-- order: a list of fields to order the results by, with the option to specify ascending or descending
-- filtering: a list of criteria to restrict the results by
-
-
-User: "What are the top 10 products by sales?"
-System:
-{{
-"metrics":["sales"],
-"dimensions": ["products"],
-"limit": 10,
-"order": ["sales desc"],
-"filtering": []
-}}
-
-User: "What are the sales by line of business and state?"
-System:
-{{
-"metrics":["average sales"],
-"dimensions": ["line of business", "state],
-"limit": -1,
-"order": [],
-"filtering": []
-}}
-
-User: "What is the average sales by state?"
-System:
-{{
-"metrics":["average state sales"],
-"dimensions": [],
-"limit": -1,
-"order": [],
-"filtering": []
-}}
-
-User: "{input}"
-System:
-
-"""
+def gen_extraction_prompt_v1(input: str):
+    return f"""
+System: You are a helpful AI that translates ambiguous business questions into structured outputs.
+For a provided question, you will determine if there are metrics or aggregates or dimensions,
+as well as any limit, order, of filtering. 
+
+The output should be a VALID JSON blob with the following keys and values:
+- metrics: a list of concepts from the question that should be aggregated
+- dimensions: a list of concepts from the question which are not metrics
+- limit: a number of records to limit the results to, -1 if none specified
+- order: a list of fields to order the results by, with the option to specify ascending or descending
+- filtering: a list of criteria to restrict the results by
+
+
+User: "What are the top 10 products by sales?"
+System:
+{{
+"metrics":["sales"],
+"dimensions": ["products"],
+"limit": 10,
+"order": ["sales desc"],
+"filtering": []
+}}
+
+User: "What are the sales by line of business and state?"
+System:
+{{
+"metrics":["average sales"],
+"dimensions": ["line of business", "state],
+"limit": -1,
+"order": [],
+"filtering": []
+}}
+
+User: "What is the average sales by state?"
+System:
+{{
+"metrics":["average state sales"],
+"dimensions": [],
+"limit": -1,
+"order": [],
+"filtering": []
+}}
+
+User: "{input}"
+System:
+
+"""
```

### Comparing `pypreql-nlp-0.0.1/preql_nlp/prompts/semantic_to_tokens.py` & `pypreql-nlp-0.0.2/preql_nlp/prompts/semantic_to_tokens.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import List
-
-
-def gen_structured_prompt_v1(phrases:List[str], tokens:str)->str:
-    phrase_str = ', '.join(phrases)
-    user_input = f"Given the tokens {tokens}, match tokens to the phrases {phrase_str}"
-    template = f"""\
-System: you are an AI that helps a user map phrases to tokens by associating a phrase with tokens related to the words
-in the phrase.
-Guidelines:
-* you can assume the user will always provide a list of phrases
-* you can assume the user will always provide a list of tokens
-* only return tokens provided by the user
-The output should be a VALID JSON blob with the phrases as keys and arrays of tokens as values:
-* If a phrase has no matches, return an empty array
-User: given the tokens ["color", "product", "year", "revenue"], match tokens to the phrases ["product revenue", "product color", "product revenue by year", "yearly revenue"]
-System:
-{{
-    "product revenue": ["product", "revenue"],
-    "product color": ["product", "color"],
-    "product revenue by year": ["product", "revenue", "year"],
-    "yearly revenue": ["year", "revenue"]
-}}
-User: given the tokens ["product", "count", "order", "year"], match tokens to the phrases ["products sold", "orders"]
-System:
-{{
-    "products sold": ["product", "count"],
-    "orders": ["order", "count"]
-}}
-User: { user_input }
-System:
-"""  # noqa"""
-    return template
-
+from typing import List
+
+
+def gen_structured_prompt_v1(phrases:List[str], tokens:str)->str:
+    phrase_str = ', '.join(phrases)
+    user_input = f"Given the tokens {tokens}, match tokens to the phrases {phrase_str}"
+    template = f"""\
+System: you are an AI that helps a user map phrases to tokens by associating a phrase with tokens related to the words
+in the phrase.
+Guidelines:
+* you can assume the user will always provide a list of phrases
+* you can assume the user will always provide a list of tokens
+* only return tokens provided by the user
+The output should be a VALID JSON blob with the phrases as keys and arrays of tokens as values:
+* If a phrase has no matches, return an empty array
+User: given the tokens ["color", "product", "year", "revenue"], match tokens to the phrases ["product revenue", "product color", "product revenue by year", "yearly revenue"]
+System:
+{{
+    "product revenue": ["product", "revenue"],
+    "product color": ["product", "color"],
+    "product revenue by year": ["product", "revenue", "year"],
+    "yearly revenue": ["year", "revenue"]
+}}
+User: given the tokens ["product", "count", "order", "year"], match tokens to the phrases ["products sold", "orders"]
+System:
+{{
+    "products sold": ["product", "count"],
+    "orders": ["order", "count"]
+}}
+User: { user_input }
+System:
+"""  # noqa"""
+    return template
+
```

### Comparing `pypreql-nlp-0.0.1/pypreql_nlp.egg-info/PKG-INFO` & `pypreql-nlp-0.0.2/pypreql_nlp.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: pypreql-nlp
-Version: 0.0.1
-Summary: NLP interface for pypreql.
-Home-page: 
-Author: 
-Author-email: pypreql-community@gmail.com
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
-## PreQL NLP
-
-Natural language interface for generating PreQL query objects.
-
-PreQL is easier for a large language model to interact with as it requires only extract relevant concepts from a text,
-classifying them as metrics or dimensions, and mapping them to what is available in a model.
-
-This makes it more testable and less prone to hallucination than generating SQL directly. 
-
-Requires setting the following environment variables
-- OPENAI_API_KEY
-- OPENAI_MODEL
-
-Recommended to use "gpt-3.5-turbo" or higher as the model.
-
-## Examples
-
-### Basic BQ example
-
-
-```python
-from trilogy_public_models import models
-from preql import Executor, default_engine, Dialect
-from preql_nlp import build_query
-
-# define the model we want to parse
-environment = models["bigquery.stack_overflow"]
-
-# set up preql executor
-# default bigquery executor requires local default credentials configured
-executor = Dialect.BIGQUERY.default_executor(environment= environment)
-
-# build a query off text and the selected model
-processed_query = build_query(
-    "How many questions are asked per year?",
-    environment,
-)
-
-# make sure we got reasonable outputs
-for concept in processed_query.output_columns:
-    print(concept.name)
-
-# and run that to get our answer
-results = executor.execute_query(processed_query)
-for row in results:
-    print(row)
-```
-
-
-
-## Setting Up Your Environment
-
-Recommend that you work in a virtual environment with requirements from both requirements.txt and requirements-test.txt installed. The latter is necessary to run
-tests (surprise). 
-
-Pypreql-nlp is python 3.10+
+Metadata-Version: 2.1
+Name: pypreql-nlp
+Version: 0.0.2
+Summary: NLP interface for pypreql.
+Home-page: 
+Author: 
+Author-email: pypreql-community@gmail.com
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+## PreQL NLP
+
+Natural language interface for generating PreQL query objects.
+
+PreQL is easier for a large language model to interact with as it requires only extract relevant concepts from a text,
+classifying them as metrics or dimensions, and mapping them to what is available in a model.
+
+This makes it more testable and less prone to hallucination than generating SQL directly. 
+
+Requires setting the following environment variables
+- OPENAI_API_KEY
+- OPENAI_MODEL
+
+Recommended to use "gpt-3.5-turbo" or higher as the model.
+
+## Examples
+
+### Basic BQ example
+
+
+```python
+from trilogy_public_models import models
+from preql import Executor, default_engine, Dialect
+from preql_nlp import build_query
+
+# define the model we want to parse
+environment = models["bigquery.stack_overflow"]
+
+# set up preql executor
+# default bigquery executor requires local default credentials configured
+executor = Dialect.BIGQUERY.default_executor(environment= environment)
+
+# build a query off text and the selected model
+processed_query = build_query(
+    "How many questions are asked per year?",
+    environment,
+)
+
+# make sure we got reasonable outputs
+for concept in processed_query.output_columns:
+    print(concept.name)
+
+# and run that to get our answer
+results = executor.execute_query(processed_query)
+for row in results:
+    print(row)
+```
+
+
+
+## Setting Up Your Environment
+
+Recommend that you work in a virtual environment with requirements from both requirements.txt and requirements-test.txt installed. The latter is necessary to run
+tests (surprise). 
+
+Pypreql-nlp is python 3.10+
```

### Comparing `pypreql-nlp-0.0.1/setup.py` & `pypreql-nlp-0.0.2/setup.py`

 * *Files identical despite different names*

