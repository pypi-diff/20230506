# Comparing `tmp/dbt-ai-0.0.3.tar.gz` & `tmp/dbt-ai-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.0.3.tar", last modified: Sat May  6 11:07:22 2023, max compression
+gzip compressed data, was "dbt-ai-0.0.4a0.tar", last modified: Sat May  6 11:15:47 2023, max compression
```

## Comparing `dbt-ai-0.0.3.tar` & `dbt-ai-0.0.4a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 11:07:22.147895 dbt-ai-0.0.3/
--rw-r--r--   0 armalite  (1000) armalite  (1000)       34 2023-05-05 05:14:16.000000 dbt-ai-0.0.3/MANIFEST.in
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1988 2023-05-06 11:07:22.147895 dbt-ai-0.0.3/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1810 2023-05-06 11:06:19.000000 dbt-ai-0.0.3/README.md
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 11:07:22.147895 dbt-ai-0.0.3/dbt_ai/
--rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.0.3/dbt_ai/__init__.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 10:40:22.000000 dbt-ai-0.0.3/dbt_ai/ai.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     2633 2023-05-06 09:35:47.000000 dbt-ai-0.0.3/dbt_ai/dbt.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)      528 2023-05-06 08:28:32.000000 dbt-ai-0.0.3/dbt_ai/helper.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 09:36:12.000000 dbt-ai-0.0.3/dbt_ai/main.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.0.3/dbt_ai/py.typed
--rw-r--r--   0 armalite  (1000) armalite  (1000)      667 2023-05-06 09:44:21.000000 dbt-ai-0.0.3/dbt_ai/report.py
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 11:07:22.147895 dbt-ai-0.0.3/dbt_ai.egg-info/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1988 2023-05-06 11:07:22.000000 dbt-ai-0.0.3/dbt_ai.egg-info/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)      305 2023-05-06 11:07:22.000000 dbt-ai-0.0.3/dbt_ai.egg-info/SOURCES.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-06 11:07:22.000000 dbt-ai-0.0.3/dbt_ai.egg-info/dependency_links.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)      155 2023-05-06 11:07:22.000000 dbt-ai-0.0.3/dbt_ai.egg-info/requires.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-06 11:07:22.000000 dbt-ai-0.0.3/dbt_ai.egg-info/top_level.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1536 2023-05-06 11:06:09.000000 dbt-ai-0.0.3/pyproject.toml
--rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-06 11:07:22.147895 dbt-ai-0.0.3/setup.cfg
--rw-r--r--   0 armalite  (1000) armalite  (1000)       81 2023-05-05 05:14:16.000000 dbt-ai-0.0.3/setup.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 11:15:47.357895 dbt-ai-0.0.4a0/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       34 2023-05-05 05:14:16.000000 dbt-ai-0.0.4a0/MANIFEST.in
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1891 2023-05-06 11:15:47.357895 dbt-ai-0.0.4a0/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1711 2023-05-06 11:15:37.000000 dbt-ai-0.0.4a0/README.md
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 11:15:47.357895 dbt-ai-0.0.4a0/dbt_ai/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.0.4a0/dbt_ai/__init__.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 10:40:22.000000 dbt-ai-0.0.4a0/dbt_ai/ai.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     2633 2023-05-06 09:35:47.000000 dbt-ai-0.0.4a0/dbt_ai/dbt.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      528 2023-05-06 08:28:32.000000 dbt-ai-0.0.4a0/dbt_ai/helper.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 09:36:12.000000 dbt-ai-0.0.4a0/dbt_ai/main.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.0.4a0/dbt_ai/py.typed
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      667 2023-05-06 09:44:21.000000 dbt-ai-0.0.4a0/dbt_ai/report.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 11:15:47.357895 dbt-ai-0.0.4a0/dbt_ai.egg-info/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1891 2023-05-06 11:15:47.000000 dbt-ai-0.0.4a0/dbt_ai.egg-info/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      305 2023-05-06 11:15:47.000000 dbt-ai-0.0.4a0/dbt_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-06 11:15:47.000000 dbt-ai-0.0.4a0/dbt_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      155 2023-05-06 11:15:47.000000 dbt-ai-0.0.4a0/dbt_ai.egg-info/requires.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-06 11:15:47.000000 dbt-ai-0.0.4a0/dbt_ai.egg-info/top_level.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1542 2023-05-06 11:15:22.000000 dbt-ai-0.0.4a0/pyproject.toml
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-06 11:15:47.357895 dbt-ai-0.0.4a0/setup.cfg
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       81 2023-05-05 05:14:16.000000 dbt-ai-0.0.4a0/setup.py
```

### Comparing `dbt-ai-0.0.3/PKG-INFO` & `dbt-ai-0.0.4a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
-NOTE: Production PIP MODULE IS NOT YET AVAILABLE
-
-The test application can be installed from TestPypi:
+You can install the application here
 ```bash
-pip install -i https://test.pypi.org/simple/ dbt-ai==0.0.3
+pip install dbt-ai==0.0.3
 ```
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key. 
     - Trial version gives you a certain amount of credits allowing you to make many API calls
     - Usage beyond the trial credits require billing details. [API usage pricing](https://openai.com/pricing) provides more info
```

### Comparing `dbt-ai-0.0.3/README.md` & `dbt-ai-0.0.4a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
-NOTE: Production PIP MODULE IS NOT YET AVAILABLE
-
-The test application can be installed from TestPypi:
+You can install the application here
 ```bash
-pip install -i https://test.pypi.org/simple/ dbt-ai==0.0.3
+pip install dbt-ai==0.0.3
 ```
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key. 
     - Trial version gives you a certain amount of credits allowing you to make many API calls
     - Usage beyond the trial credits require billing details. [API usage pricing](https://openai.com/pricing) provides more info
```

### Comparing `dbt-ai-0.0.3/dbt_ai/ai.py` & `dbt-ai-0.0.4a0/dbt_ai/ai.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.3/dbt_ai/dbt.py` & `dbt-ai-0.0.4a0/dbt_ai/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.3/dbt_ai/helper.py` & `dbt-ai-0.0.4a0/dbt_ai/helper.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.3/dbt_ai/main.py` & `dbt-ai-0.0.4a0/dbt_ai/main.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.3/dbt_ai/report.py` & `dbt-ai-0.0.4a0/dbt_ai/report.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.3/dbt_ai.egg-info/PKG-INFO` & `dbt-ai-0.0.4a0/dbt_ai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
-NOTE: Production PIP MODULE IS NOT YET AVAILABLE
-
-The test application can be installed from TestPypi:
+You can install the application here
 ```bash
-pip install -i https://test.pypi.org/simple/ dbt-ai==0.0.3
+pip install dbt-ai==0.0.3
 ```
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key. 
     - Trial version gives you a certain amount of credits allowing you to make many API calls
     - Usage beyond the trial credits require billing details. [API usage pricing](https://openai.com/pricing) provides more info
```

### Comparing `dbt-ai-0.0.3/pyproject.toml` & `dbt-ai-0.0.4a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dbt-ai"
 description = "AI powered DBT helper application"
-version = "0.0.3"
+version = "0.0.4-alpha"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "dbt-snowflake~=1.4",
     "openai~=0.27",
     "pyyaml~=6.0",
     "markdown2~=2.4",
```

