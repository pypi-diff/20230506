# Comparing `tmp/dbt-ai-0.0.7a0.tar.gz` & `tmp/dbt-ai-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.0.7a0.tar", last modified: Sat May  6 12:58:58 2023, max compression
+gzip compressed data, was "dbt-ai-0.0.8a0.tar", last modified: Sat May  6 13:05:57 2023, max compression
```

## Comparing `dbt-ai-0.0.7a0.tar` & `dbt-ai-0.0.8a0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 12:58:58.627895 dbt-ai-0.0.7a0/
--rw-r--r--   0 armalite  (1000) armalite  (1000)       34 2023-05-05 05:14:16.000000 dbt-ai-0.0.7a0/MANIFEST.in
--rw-r--r--   0 armalite  (1000) armalite  (1000)     2004 2023-05-06 12:58:58.627895 dbt-ai-0.0.7a0/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1824 2023-05-06 12:58:42.000000 dbt-ai-0.0.7a0/README.md
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 12:58:58.627895 dbt-ai-0.0.7a0/dbt_ai/
--rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.0.7a0/dbt_ai/__init__.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 10:40:22.000000 dbt-ai-0.0.7a0/dbt_ai/ai.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     2633 2023-05-06 09:35:47.000000 dbt-ai-0.0.7a0/dbt_ai/dbt.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)      528 2023-05-06 08:28:32.000000 dbt-ai-0.0.7a0/dbt_ai/helper.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 09:36:12.000000 dbt-ai-0.0.7a0/dbt_ai/main.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.0.7a0/dbt_ai/py.typed
--rw-r--r--   0 armalite  (1000) armalite  (1000)      795 2023-05-06 12:58:28.000000 dbt-ai-0.0.7a0/dbt_ai/report.py
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 12:58:58.627895 dbt-ai-0.0.7a0/dbt_ai.egg-info/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     2004 2023-05-06 12:58:58.000000 dbt-ai-0.0.7a0/dbt_ai.egg-info/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)      338 2023-05-06 12:58:58.000000 dbt-ai-0.0.7a0/dbt_ai.egg-info/SOURCES.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-06 12:58:58.000000 dbt-ai-0.0.7a0/dbt_ai.egg-info/dependency_links.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-06 12:58:58.000000 dbt-ai-0.0.7a0/dbt_ai.egg-info/entry_points.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)      155 2023-05-06 12:58:58.000000 dbt-ai-0.0.7a0/dbt_ai.egg-info/requires.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-06 12:58:58.000000 dbt-ai-0.0.7a0/dbt_ai.egg-info/top_level.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1542 2023-05-06 12:58:49.000000 dbt-ai-0.0.7a0/pyproject.toml
--rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-06 12:58:58.627895 dbt-ai-0.0.7a0/setup.cfg
--rw-r--r--   0 armalite  (1000) armalite  (1000)      165 2023-05-06 12:18:31.000000 dbt-ai-0.0.7a0/setup.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.0.8a0/MANIFEST.in
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     2004 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1824 2023-05-06 13:05:14.000000 dbt-ai-0.0.8a0/README.md
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/dbt_ai/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.0.8a0/dbt_ai/__init__.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 10:40:22.000000 dbt-ai-0.0.8a0/dbt_ai/ai.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     2633 2023-05-06 09:35:47.000000 dbt-ai-0.0.8a0/dbt_ai/dbt.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      528 2023-05-06 08:28:32.000000 dbt-ai-0.0.8a0/dbt_ai/helper.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 09:36:12.000000 dbt-ai-0.0.8a0/dbt_ai/main.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.0.8a0/dbt_ai/py.typed
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      795 2023-05-06 12:58:28.000000 dbt-ai-0.0.8a0/dbt_ai/report.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/dbt_ai/templates/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3099 2023-05-06 10:46:28.000000 dbt-ai-0.0.8a0/dbt_ai/templates/report_template.html
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/dbt_ai.egg-info/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     2004 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      376 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/entry_points.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      155 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/requires.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/top_level.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1542 2023-05-06 13:05:47.000000 dbt-ai-0.0.8a0/pyproject.toml
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/setup.cfg
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      165 2023-05-06 12:18:31.000000 dbt-ai-0.0.8a0/setup.py
```

### Comparing `dbt-ai-0.0.7a0/PKG-INFO` & `dbt-ai-0.0.8a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.0.7a0
+pip install dbt-ai==0.0.8a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.0.7a0/README.md` & `dbt-ai-0.0.8a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.0.7a0
+pip install dbt-ai==0.0.8a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.0.7a0/dbt_ai/ai.py` & `dbt-ai-0.0.8a0/dbt_ai/ai.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.7a0/dbt_ai/dbt.py` & `dbt-ai-0.0.8a0/dbt_ai/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.7a0/dbt_ai/helper.py` & `dbt-ai-0.0.8a0/dbt_ai/helper.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.7a0/dbt_ai/main.py` & `dbt-ai-0.0.8a0/dbt_ai/main.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.7a0/dbt_ai/report.py` & `dbt-ai-0.0.8a0/dbt_ai/report.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.7a0/dbt_ai.egg-info/PKG-INFO` & `dbt-ai-0.0.8a0/dbt_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.0.7a0
+pip install dbt-ai==0.0.8a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.0.7a0/pyproject.toml` & `dbt-ai-0.0.8a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dbt-ai"
 description = "AI powered DBT helper application"
-version = "0.0.7-alpha"
+version = "0.0.8-alpha"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "dbt-snowflake~=1.4",
     "openai~=0.27",
     "pyyaml~=6.0",
     "markdown2~=2.4",
```

