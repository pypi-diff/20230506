# Comparing `tmp/pypreql-nlp-0.0.3.tar.gz` & `tmp/pypreql-nlp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-nlp-0.0.3.tar", last modified: Sat May  6 19:30:09 2023, max compression
+gzip compressed data, was "pypreql-nlp-0.0.4.tar", last modified: Sat May  6 21:50:45 2023, max compression
```

## Comparing `pypreql-nlp-0.0.3.tar` & `pypreql-nlp-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:30:09.823147 pypreql-nlp-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 19:30:09.823147 pypreql-nlp-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:30:09.819147 pypreql-nlp-0.0.3/preql_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/monkeypatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:30:09.819147 pypreql-nlp-0.0.3/preql_nlp/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/final_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/prompt_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/query_semantic_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/preql_nlp/prompts/semantic_to_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:30:09.823147 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 19:30:09.000000 pypreql-nlp-0.0.3/pypreql_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 19:30:09.823147 pypreql-nlp-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-06 19:29:56.000000 pypreql-nlp-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:45.892298 pypreql-nlp-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 21:50:45.892298 pypreql-nlp-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:45.888298 pypreql-nlp-0.0.4/preql_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/monkeypatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:45.888298 pypreql-nlp-0.0.4/preql_nlp/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/final_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/prompt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/query_semantic_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/preql_nlp/prompts/semantic_to_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:45.892298 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 21:50:45.000000 pypreql-nlp-0.0.4/pypreql_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:50:45.892298 pypreql-nlp-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-06 21:50:35.000000 pypreql-nlp-0.0.4/setup.py
```

### Comparing `pypreql-nlp-0.0.3/PKG-INFO` & `pypreql-nlp-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.3
+Version: 0.0.4
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.3/README.md` & `pypreql-nlp-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.3/preql_nlp/main.py` & `pypreql-nlp-0.0.4/preql_nlp/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,29 +174,41 @@
     if not input:
         return DEFAULT_LIMIT
     if input in (-1, 0):
         return DEFAULT_LIMIT
     return input
 
 
-def parse_order(input: List[Concept], ordering: List[str] | None) -> OrderBy:
+def safe_parse_order_item(
+    input: str, input_concepts: List[Concept]
+) -> OrderItem | None:
+    concept, direction = input.split(" ", 1)
+    matched = [c for c in input_concepts if concept in c.address]
+    if not matched:
+        return None
+    try:
+        order = Ordering(direction)
+    except Exception:
+        return None
+    return OrderItem(expr=matched[0], order=order)
+
+
+def parse_order(input_concepts: List[Concept], ordering: List[str] | None) -> OrderBy:
     default_order = [
         OrderItem(expr=c, order=Ordering.DESCENDING)
-        for c in input
+        for c in input_concepts
         if c.purpose == Purpose.METRIC
     ]
     if not ordering:
         return OrderBy(default_order)
     final = []
     for order in ordering:
-        concept, direction = order.split(" ", 1)
-        matched = [c for c in input if concept in c.address]
-        if not matched:
-            continue
-        final.append(OrderItem(expr=matched[0], order=Ordering(direction)))
+        parsed = safe_parse_order_item(order, input_concepts)
+        if parsed:
+            final.append(parsed)
     return OrderBy(items=final)
 
 
 def parse_query(
     input_text: str,
     input_environment: Environment,
     debug: bool = False,
```

### Comparing `pypreql-nlp-0.0.3/preql_nlp/monkeypatch.py` & `pypreql-nlp-0.0.4/preql_nlp/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.3/preql_nlp/prompts/final_selection.py` & `pypreql-nlp-0.0.4/preql_nlp/prompts/final_selection.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.3/preql_nlp/prompts/prompt_executor.py` & `pypreql-nlp-0.0.4/preql_nlp/prompts/prompt_executor.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.3/preql_nlp/prompts/query_semantic_extraction.py` & `pypreql-nlp-0.0.4/preql_nlp/prompts/query_semantic_extraction.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.3/preql_nlp/prompts/semantic_to_tokens.py` & `pypreql-nlp-0.0.4/preql_nlp/prompts/semantic_to_tokens.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.3/pypreql_nlp.egg-info/PKG-INFO` & `pypreql-nlp-0.0.4/pypreql_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.3
+Version: 0.0.4
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.3/setup.py` & `pypreql-nlp-0.0.4/setup.py`

 * *Files identical despite different names*

