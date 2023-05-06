# Comparing `tmp/interactive_multi_category_table-0.0.1.tar.gz` & `tmp/interactive_multi_category_table-0.0.2.tar.gz`

## Comparing `interactive_multi_category_table-0.0.1.tar` & `interactive_multi_category_table-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/examples/ai4science.json
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/examples/dinner.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/interactive_multi_category_table/__init__.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/interactive_multi_category_table/main.py
--rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/interactive_multi_category_table/utils.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/LICENSE
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/README.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/examples/ai4science.json
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/examples/dinner.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/interactive_multi_category_table/__init__.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/interactive_multi_category_table/main.py
+-rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/interactive_multi_category_table/utils.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/README.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 interactive_multi_category_table-0.0.2/PKG-INFO
```

### Comparing `interactive_multi_category_table-0.0.1/examples/ai4science.json` & `interactive_multi_category_table-0.0.2/examples/ai4science.json`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.1/examples/dinner.json` & `interactive_multi_category_table-0.0.2/examples/dinner.json`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.1/interactive_multi_category_table/main.py` & `interactive_multi_category_table-0.0.2/interactive_multi_category_table/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from dash import Dash, html, dcc, callback, Output, Input
-from utils import parse_json, gen_html_table, get_radioitems_options
+from .utils import parse_json, gen_html_table, get_radioitems_options
 
 def run_app(json_file_path):
     json_data, category_list, tag_list, category_dict = parse_json(json_file_path)
 
     row_category_value_init = category_list[0]
     column_category_value_init = category_list[1]
     row_category_options, column_category_options = get_radioitems_options(category_list, row_category_value_init, column_category_value_init)
```

### Comparing `interactive_multi_category_table-0.0.1/interactive_multi_category_table/utils.py` & `interactive_multi_category_table-0.0.2/interactive_multi_category_table/utils.py`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.1/.gitignore` & `interactive_multi_category_table-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.1/LICENSE` & `interactive_multi_category_table-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `interactive_multi_category_table-0.0.1/README.md` & `interactive_multi_category_table-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # interactive-multi-category-table
 
 In many different scenarios, contents are single-categorized and multi-tagged, by which I mean there are multiple tags but one single (though may be hierarchical) category system, e.g., file systems, blogs, etc. However, sometimes contents can be categorized from different category views. For storage or lookup, one category system is OK; but for visualization and analysis, flexibly organizing the contents with different category views will be very handy.
 
-This repo targets addressing such demand by creating interactive tables with alternative category views, from formatted json input, based on dash.
+This repo targets addressing such demand by creating interactive tables with alternative category views, from formatted json input, based on [dash](https://dash.plotly.com/).
 
 # usage
 
 Simply run
 ```python
 import interactive_multi_category_table as imct
```

### Comparing `interactive_multi_category_table-0.0.1/pyproject.toml` & `interactive_multi_category_table-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "interactive_multi_category_table"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Xiang CHEN", email="xiangchen.ai@outlook.com" },
+    {name="Xiang CHEN", email="xiangchen.ai@outlook.com"},
 ]
-description = "A package to create interactive tables with alternative category views, from formatted json input, based on dash."
+description = "A python package to create interactive tables with alternative category views, from formatted json input, based on dash."
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "dash",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/XiangCHEN-dvi/interactive-multi-category-table"
 "Bug Tracker" = "https://github.com/XiangCHEN-dvi/interactive-multi-category-table/issues"
```

### Comparing `interactive_multi_category_table-0.0.1/PKG-INFO` & `interactive_multi_category_table-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: interactive_multi_category_table
-Version: 0.0.1
-Summary: A package to create interactive tables with alternative category views, from formatted json input, based on dash.
+Version: 0.0.2
+Summary: A python package to create interactive tables with alternative category views, from formatted json input, based on dash.
 Project-URL: Homepage, https://github.com/XiangCHEN-dvi/interactive-multi-category-table
 Project-URL: Bug Tracker, https://github.com/XiangCHEN-dvi/interactive-multi-category-table/issues
 Author-email: Xiang CHEN <xiangchen.ai@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: dash
 Description-Content-Type: text/markdown
 
 # interactive-multi-category-table
 
 In many different scenarios, contents are single-categorized and multi-tagged, by which I mean there are multiple tags but one single (though may be hierarchical) category system, e.g., file systems, blogs, etc. However, sometimes contents can be categorized from different category views. For storage or lookup, one category system is OK; but for visualization and analysis, flexibly organizing the contents with different category views will be very handy.
 
-This repo targets addressing such demand by creating interactive tables with alternative category views, from formatted json input, based on dash.
+This repo targets addressing such demand by creating interactive tables with alternative category views, from formatted json input, based on [dash](https://dash.plotly.com/).
 
 # usage
 
 Simply run
 ```python
 import interactive_multi_category_table as imct
```

