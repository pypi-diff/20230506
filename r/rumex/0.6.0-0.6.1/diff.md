# Comparing `tmp/rumex-0.6.0.tar.gz` & `tmp/rumex-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rumex-0.6.0.tar", max compression
+gzip compressed data, was "rumex-0.6.1.tar", max compression
```

## Comparing `rumex-0.6.0.tar` & `rumex-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      721 2023-05-05 01:19:14.413580 rumex-0.6.0/LICENSE
--rw-r--r--   0        0        0     1835 2023-05-05 01:19:14.413580 rumex-0.6.0/README.rst
--rw-r--r--   0        0        0      916 2023-05-05 01:19:14.417580 rumex-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-05 01:19:14.417580 rumex-0.6.0/rumex/__init__.py
--rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.6.0/rumex/parsing/__init__.py
--rw-r--r--   0        0        0     3493 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/parsing/builder.py
--rw-r--r--   0        0        0     1032 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/parsing/core.py
--rw-r--r--   0        0        0     8906 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/parsing/parser.py
--rw-r--r--   0        0        0      990 2023-05-02 00:37:46.737147 rumex-0.6.0/rumex/parsing/table.py
--rw-r--r--   0        0        0     2797 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/parsing/tokenizer.py
--rw-r--r--   0        0        0    13962 2023-05-05 01:19:14.417580 rumex-0.6.0/rumex/runner.py
--rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.6.0/rumex/tests/__init__.py
--rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.6.0/rumex/tests/test_data.py
--rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.6.0/rumex/tests/test_error_reporting.py
--rw-r--r--   0        0        0     2749 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/tests/test_execution.py
--rw-r--r--   0        0        0     5554 2023-04-24 20:26:14.685112 rumex-0.6.0/rumex/tests/test_no_execution_cases.py
--rw-r--r--   0        0        0     6717 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/tests/test_simple_execution.py
--rw-r--r--   0        0        0     2390 2023-05-05 01:19:14.417580 rumex-0.6.0/rumex/utils.py
--rw-r--r--   0        0        0     2166 1970-01-01 00:00:00.000000 rumex-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2023-05-05 01:19:14.413580 rumex-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1896 2023-05-06 00:38:54.995163 rumex-0.6.1/README.rst
+-rw-r--r--   0        0        0      916 2023-05-06 00:38:54.995163 rumex-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-06 00:38:54.995163 rumex-0.6.1/rumex/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.6.1/rumex/parsing/__init__.py
+-rw-r--r--   0        0        0     3493 2023-05-03 23:39:13.199906 rumex-0.6.1/rumex/parsing/builder.py
+-rw-r--r--   0        0        0     1032 2023-05-03 23:39:13.199906 rumex-0.6.1/rumex/parsing/core.py
+-rw-r--r--   0        0        0     8906 2023-05-03 23:39:13.199906 rumex-0.6.1/rumex/parsing/parser.py
+-rw-r--r--   0        0        0      990 2023-05-02 00:37:46.737147 rumex-0.6.1/rumex/parsing/table.py
+-rw-r--r--   0        0        0     2797 2023-05-03 23:39:13.199906 rumex-0.6.1/rumex/parsing/tokenizer.py
+-rw-r--r--   0        0        0    13962 2023-05-05 01:19:14.417580 rumex-0.6.1/rumex/runner.py
+-rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.6.1/rumex/tests/__init__.py
+-rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.6.1/rumex/tests/test_data.py
+-rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.6.1/rumex/tests/test_error_reporting.py
+-rw-r--r--   0        0        0     2749 2023-05-03 23:39:13.199906 rumex-0.6.1/rumex/tests/test_execution.py
+-rw-r--r--   0        0        0     5554 2023-04-24 20:26:14.685112 rumex-0.6.1/rumex/tests/test_no_execution_cases.py
+-rw-r--r--   0        0        0     6717 2023-05-03 23:39:13.199906 rumex-0.6.1/rumex/tests/test_simple_execution.py
+-rw-r--r--   0        0        0     2390 2023-05-05 01:19:14.417580 rumex-0.6.1/rumex/utils.py
+-rw-r--r--   0        0        0     2227 1970-01-01 00:00:00.000000 rumex-0.6.1/PKG-INFO
```

### Comparing `rumex-0.6.0/LICENSE` & `rumex-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/README.rst` & `rumex-0.6.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 `Behaviour Driven Development`_ (BDD) testing library.
 
 Rumex is trying to be more of a library rather than a framework.
 This approach aims to increase flexibility and reduce dependency
 on design choices made by designers of alternative frameworks.
 
+Installation
+------------
+
+.. code::
+
+    pip install rumex
+
 
 Basic example
 -------------
 
 .. code:: python
 
     import rumex
```

### Comparing `rumex-0.6.0/pyproject.toml` & `rumex-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rumex"
-version = "0.6.0"
+version = "0.6.1"
 
 description = ""
 authors = ["uigctaw <uigctaw@metadata.social>"]
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
```

### Comparing `rumex-0.6.0/rumex/parsing/builder.py` & `rumex-0.6.1/rumex/parsing/builder.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/parsing/core.py` & `rumex-0.6.1/rumex/parsing/core.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/parsing/parser.py` & `rumex-0.6.1/rumex/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/parsing/table.py` & `rumex-0.6.1/rumex/parsing/table.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/parsing/tokenizer.py` & `rumex-0.6.1/rumex/parsing/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/runner.py` & `rumex-0.6.1/rumex/runner.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/tests/__init__.py` & `rumex-0.6.1/rumex/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/tests/test_data.py` & `rumex-0.6.1/rumex/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/tests/test_error_reporting.py` & `rumex-0.6.1/rumex/tests/test_error_reporting.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/tests/test_execution.py` & `rumex-0.6.1/rumex/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/tests/test_no_execution_cases.py` & `rumex-0.6.1/rumex/tests/test_no_execution_cases.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/tests/test_simple_execution.py` & `rumex-0.6.1/rumex/tests/test_simple_execution.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/rumex/utils.py` & `rumex-0.6.1/rumex/utils.py`

 * *Files identical despite different names*

### Comparing `rumex-0.6.0/PKG-INFO` & `rumex-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rumex
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Author: uigctaw
 Author-email: uigctaw@metadata.social
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,14 +16,21 @@
 
 `Behaviour Driven Development`_ (BDD) testing library.
 
 Rumex is trying to be more of a library rather than a framework.
 This approach aims to increase flexibility and reduce dependency
 on design choices made by designers of alternative frameworks.
 
+Installation
+------------
+
+.. code::
+
+    pip install rumex
+
 
 Basic example
 -------------
 
 .. code:: python
 
     import rumex
```

