# Comparing `tmp/pypreql-nlp-0.0.2.tar.gz` & `tmp/pypreql-nlp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-nlp-0.0.2.tar", last modified: Sat May  6 16:14:21 2023, max compression
+gzip compressed data, was "pypreql-nlp-0.0.3.tar", last modified: Sat May  6 19:30:09 2023, max compression
```

## Comparing `pypreql-nlp-0.0.2.tar` & `pypreql-nlp-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:14:21.158986 pypreql-nlp-0.0.2/preql_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/monkeypatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/preql_nlp/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/final_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/prompt_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/query_semantic_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/preql_nlp/prompts/semantic_to_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 16:14:21.000000 pypreql-nlp-0.0.2/pypreql_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:14:21.162986 pypreql-nlp-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-06 16:14:07.000000 pypreql-nlp-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:30:09.823147 pypreql-nlp-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 19:30:09.823147 pypreql-nlp-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:30:09.819147 pypreql-nlp-0.0.3/preql_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/monkeypatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:30:09.819147 pypreql-nlp-0.0.3/preql_nlp/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/final_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/prompt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/query_semantic_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/semantic_to_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:30:09.823147 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 19:30:09.823147 pypreql-nlp-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/setup.py
```

### Comparing `pypreql-nlp-0.0.2/PKG-INFO` & `pypreql-nlp-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.2
+Version: 0.0.3
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.2/README.md` & `pypreql-nlp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.2/preql_nlp/main.py` & `pypreql-nlp-0.0.3/preql_nlp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,22 +192,30 @@
         matched = [c for c in input if concept in c.address]
         if not matched:
             continue
         final.append(OrderItem(expr=matched[0], order=Ordering(direction)))
     return OrderBy(items=final)
 
 
-def build_query(
+def parse_query(
     input_text: str,
     input_environment: Environment,
     debug: bool = False,
-) -> ProcessedQuery:
+):
     results = discover_inputs(input_text, input_environment, debug=debug)
     concepts = [input_environment.concepts[x] for x in results.select]
     order = parse_order(concepts, results.order)
     if debug:
         print("Concepts found")
         for c in concepts:
             print(c.address)
     query = Select(selection=concepts, limit=safe_limit(results.limit), order_by=order)
+    return query
 
+
+def build_query(
+    input_text: str,
+    input_environment: Environment,
+    debug: bool = False,
+) -> ProcessedQuery:
+    query = parse_query(input_text, input_environment, debug=debug)
     return process_query_v2(statement=query, environment=input_environment)
```

### Comparing `pypreql-nlp-0.0.2/preql_nlp/monkeypatch.py` & `pypreql-nlp-0.0.3/preql_nlp/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.2/preql_nlp/prompts/final_selection.py` & `pypreql-nlp-0.0.3/preql_nlp/prompts/final_selection.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.2/preql_nlp/prompts/prompt_executor.py` & `pypreql-nlp-0.0.3/preql_nlp/prompts/prompt_executor.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.2/preql_nlp/prompts/query_semantic_extraction.py` & `pypreql-nlp-0.0.3/preql_nlp/prompts/query_semantic_extraction.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.2/preql_nlp/prompts/semantic_to_tokens.py` & `pypreql-nlp-0.0.3/preql_nlp/prompts/semantic_to_tokens.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.2/pypreql_nlp.egg-info/PKG-INFO` & `pypreql-nlp-0.0.3/pypreql_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.2
+Version: 0.0.3
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.2/setup.py` & `pypreql-nlp-0.0.3/setup.py`

 * *Files identical despite different names*

