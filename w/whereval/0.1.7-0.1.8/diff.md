# Comparing `tmp/whereval-0.1.7.tar.gz` & `tmp/whereval-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whereval-0.1.7.tar", max compression
+gzip compressed data, was "whereval-0.1.8.tar", max compression
```

## Comparing `whereval-0.1.7.tar` & `whereval-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1109 2022-04-13 20:51:01.734575 whereval-0.1.7/LICENSE
--rw-r--r--   0        0        0     2509 2022-04-13 20:53:12.750176 whereval-0.1.7/README.md
--rw-r--r--   0        0        0     1076 2022-04-17 03:58:54.098845 whereval-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      176 2022-04-14 19:17:27.712465 whereval-0.1.7/src/whereval/__init__.py
--rw-r--r--   0        0        0     8273 2022-04-17 04:06:10.281000 whereval-0.1.7/src/whereval/util.py
--rw-r--r--   0        0        0    33336 2022-04-17 04:10:31.800192 whereval-0.1.7/src/whereval/whereval.py
--rw-r--r--   0        0        0     3447 2022-04-17 16:07:25.268032 whereval-0.1.7/setup.py
--rw-r--r--   0        0        0     3623 2022-04-17 16:07:25.268645 whereval-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1109 2022-04-13 20:51:01.734575 whereval-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2509 2023-05-06 17:56:49.178424 whereval-0.1.8/README.md
+-rw-r--r--   0        0        0     1183 2023-05-06 17:56:20.835483 whereval-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      176 2022-04-14 19:17:27.712465 whereval-0.1.8/src/whereval/__init__.py
+-rw-r--r--   0        0        0     8273 2022-04-17 04:06:10.281000 whereval-0.1.8/src/whereval/util.py
+-rw-r--r--   0        0        0    33336 2022-04-17 04:10:31.800192 whereval-0.1.8/src/whereval/whereval.py
+-rw-r--r--   0        0        0     3505 2023-05-06 18:01:28.595203 whereval-0.1.8/setup.py
+-rw-r--r--   0        0        0     3762 2023-05-06 18:01:28.595923 whereval-0.1.8/PKG-INFO
```

### Comparing `whereval-0.1.7/LICENSE` & `whereval-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `whereval-0.1.7/README.md` & `whereval-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `whereval-0.1.7/pyproject.toml` & `whereval-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whereval"
-version = "0.1.7"
+version = "0.1.8"
 description = "Tool for parsing SQL like where expressions and evaluating against live data "
 license = "MIT"
 authors = ["Timothy C. Quinn"]
 readme = "README.md"
 homepage = "https://pypi.org/project/whereval"
 repository = "https://github.com/JavaScriptDude/WherEval"
 classifiers = [
@@ -16,20 +16,24 @@
     'Operating System :: POSIX :: SunOS/Solaris',
     'Operating System :: MacOS :: MacOS X',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.9"
-sqlparse = "0.4.2"
+sqlparse = "^0.4.2"
+numpy = "^1.21.2"
+texttable = "^1.6.4"
 
 
 [tool.poetry.dev-dependencies]
+unittest2 = "^1.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `whereval-0.1.7/src/whereval/util.py` & `whereval-0.1.8/src/whereval/util.py`

 * *Files identical despite different names*

### Comparing `whereval-0.1.7/src/whereval/whereval.py` & `whereval-0.1.8/src/whereval/whereval.py`

 * *Files identical despite different names*

### Comparing `whereval-0.1.7/setup.py` & `whereval-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['whereval']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['sqlparse==0.4.2']
+['numpy>=1.21.2,<2.0.0', 'sqlparse>=0.4.2,<0.5.0', 'texttable>=1.6.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'whereval',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Tool for parsing SQL like where expressions and evaluating against live data ',
     'long_description': '## WherEval\n\nTool for parsing SQL like where expressions and evaluating against live data \n\n### Installation\n\n```\npython3 -m pip install whereval\n```\n\n### Inspiration\nThis tool will scratch an itch I\'ve had for some cli tools where I want to pass complex filter expressions to control output / processing.\nFor instance with my `histstat` fork, I would like to have better filtering of networking information to be output to sqlite. See: https://github.com/JavaScriptDude/histstat\n\nAnother usecase for this is a tool I\'ve wanted to write where I can write a `tail -f` wrapper in python where I can define a filter in cli parameters to limit output to the console. Have not written this yet but its on my todo now that I\'ve got this API.\n\n### API Example\n\n#### (Ex1) Basic Concept:\n```python3\nfrom datetime import date\nfrom whereval import Where, util as wutil\n\nprint("\\n(Ex1) Basic Idea")\n\nsw = wutil.StopWatch()\n\n# Where query (terse example)\nqry = "(f0>=2+f1=1+f2=\'s\')|(f3~\'foo%\')"\n\n# Field and type spec\nspec = {\'f0\': int,\'f1\': bool,\'f2\': str,\'f3\': str, \'f4\': dt_date}\n\n# Instantiate Where\n#  - Parses query and uses data to form rules for data types and fields\nwher = Where(query=qry, spec=spec)\n\n\nprint(f"Query:\\n . raw:\\t{qry}\\n . compiled: {wher}\\n\\nTests:")\n\ndef _print(wher, data, tup): \n\t(ok, result, issues) = tup\n\tif not ok:\n\t\tprint(f"Eval failed for {wher}. Issues: {issues}")\n\telse:\n\t\tprint(f"\\t{result}\\tw/ data: {data}")\n\n# Evaluate expression against real data\ndata = {\'f0\': 2, \'f1\': True ,\'f2\': \'s\', \'f3\': \'foobar\'}\n_print(wher, data, wher.evaluate(data))\n\n# For different data\ndata[\'f3\'] = \'bazbar\'\n_print(wher, data, wher.evaluate(data))\n\n# For different data\ndata[\'f0\'] = 1\n_print(wher, data, wher.evaluate(data))\n\nprint(f"Completed. Elapsed: {sw.elapsed(3)}s")\n```\n\n#### Output of print:\n```\n(Ex1) Basic Idea\nQuery:\n . raw:\t(f0>=2+f1=1+f2=\'s\')|(f3~\'foo%\')\n . compiled: ( ( f0 >= 2 AND f1 = 1 AND f2 = \'s\' ) OR ( f3 like \'foo%\' ) )\n\nTests:\n\tTrue\tw/ data: {\'f0\': 2, \'f1\': True, \'f2\': \'s\', \'f3\': \'foobar\'}\n\tTrue\tw/ data: {\'f0\': 2, \'f1\': True, \'f2\': \'s\', \'f3\': \'bazbar\'}\n\tFalse\tw/ data: {\'f0\': 1, \'f1\': True, \'f2\': \'s\', \'f3\': \'bazbar\'}\nCompleted. Elapsed: 0.003s\n```\n\n\n### Query Syntax:\n\n```\n# General:\n#  Query must begin with \'(\' and end with \')\'\n#  NOT, IN, BETWEEN must be followed by parenthesis \'(\'\n# Boolean Operators:\n#   AND, OR, NOT\n# Equality Operators:\n#  =, !=, <, <=, >, >=, like\n# Special:\n#   !   -->  NOT\n#   +   -->  AND\n#   |   -->  OR\n#   <>  -->  !=\n#   ~   -->  like\n```',
     'author': 'Timothy C. Quinn',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/whereval',
```

### Comparing `whereval-0.1.7/PKG-INFO` & `whereval-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whereval
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tool for parsing SQL like where expressions and evaluating against live data 
 Home-page: https://pypi.org/project/whereval
 License: MIT
 Author: Timothy C. Quinn
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -13,19 +13,22 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: SunOS/Solaris
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
-Requires-Dist: sqlparse (==0.4.2)
+Requires-Dist: numpy (>=1.21.2,<2.0.0)
+Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
+Requires-Dist: texttable (>=1.6.4,<2.0.0)
 Project-URL: Repository, https://github.com/JavaScriptDude/WherEval
 Description-Content-Type: text/markdown
 
 ## WherEval
 
 Tool for parsing SQL like where expressions and evaluating against live data
```

