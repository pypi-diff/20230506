# Comparing `tmp/chyp-0.2.tar.gz` & `tmp/chyp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.2.tar", last modified: Sat May  6 16:25:12 2023, max compression
+gzip compressed data, was "chyp-0.2.1.tar", last modified: Sat May  6 16:30:52 2023, max compression
```

## Comparing `chyp-0.2.tar` & `chyp-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 16:25:12.494561 chyp-0.2/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.2/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9607 2023-05-06 16:25:12.494561 chyp-0.2/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9087 2023-05-01 13:04:02.000000 chyp-0.2/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 16:25:12.494561 chyp-0.2/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.2/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.2/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15145 2023-05-05 09:54:14.000000 chyp-0.2/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 16:25:12.494561 chyp-0.2/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.2/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1159 2023-05-05 10:07:08.000000 chyp-0.2/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.2/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5868 2023-05-06 15:16:34.000000 chyp-0.2/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    13379 2023-05-06 13:26:34.000000 chyp-0.2/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.2/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.2/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2202 2023-05-06 10:20:10.000000 chyp-0.2/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.2/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9883 2023-05-05 09:52:49.000000 chyp-0.2/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9744 2023-04-28 09:32:11.000000 chyp-0.2/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5845 2023-05-05 10:04:52.000000 chyp-0.2/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2966 2023-03-29 10:44:17.000000 chyp-0.2/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1390 2023-04-26 10:03:49.000000 chyp-0.2/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.2/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3710 2023-05-05 22:35:47.000000 chyp-0.2/chyp/state.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4064 2023-04-23 21:13:55.000000 chyp-0.2/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 16:25:12.494561 chyp-0.2/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9607 2023-05-06 16:25:12.000000 chyp-0.2/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      566 2023-05-06 16:25:12.000000 chyp-0.2/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-06 16:25:12.000000 chyp-0.2/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-06 16:25:12.000000 chyp-0.2/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-06 16:25:12.000000 chyp-0.2/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-06 16:25:12.000000 chyp-0.2/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.2/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-06 16:25:12.494561 chyp-0.2/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1044 2023-05-06 14:45:09.000000 chyp-0.2/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 16:30:52.644269 chyp-0.2.1/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.2.1/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9628 2023-05-06 16:30:52.644269 chyp-0.2.1/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9087 2023-05-01 13:04:02.000000 chyp-0.2.1/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 16:30:52.644269 chyp-0.2.1/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.2.1/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.2.1/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    15145 2023-05-05 09:54:14.000000 chyp-0.2.1/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 16:30:52.644269 chyp-0.2.1/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.2.1/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1159 2023-05-05 10:07:08.000000 chyp-0.2.1/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.2.1/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     5868 2023-05-06 15:16:34.000000 chyp-0.2.1/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    13379 2023-05-06 13:26:34.000000 chyp-0.2.1/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.2.1/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.2.1/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2202 2023-05-06 10:20:10.000000 chyp-0.2.1/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.2.1/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9883 2023-05-05 09:52:49.000000 chyp-0.2.1/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9744 2023-04-28 09:32:11.000000 chyp-0.2.1/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     5845 2023-05-05 10:04:52.000000 chyp-0.2.1/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2966 2023-03-29 10:44:17.000000 chyp-0.2.1/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1390 2023-04-26 10:03:49.000000 chyp-0.2.1/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.2.1/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3710 2023-05-05 22:35:47.000000 chyp-0.2.1/chyp/state.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4064 2023-04-23 21:13:55.000000 chyp-0.2.1/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-06 16:30:52.644269 chyp-0.2.1/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9628 2023-05-06 16:30:52.000000 chyp-0.2.1/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      566 2023-05-06 16:30:52.000000 chyp-0.2.1/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-06 16:30:52.000000 chyp-0.2.1/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-06 16:30:52.000000 chyp-0.2.1/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-06 16:30:52.000000 chyp-0.2.1/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-06 16:30:52.000000 chyp-0.2.1/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.2.1/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-06 16:30:52.644269 chyp-0.2.1/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1065 2023-05-06 16:30:06.000000 chyp-0.2.1/setup.py
```

### Comparing `chyp-0.2/LICENSE` & `chyp-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.2/PKG-INFO` & `chyp-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.2
-Summary: A compositional hypergraph library
+Version: 0.2.1
+Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chyp-0.2/README.md` & `chyp-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/__init__.py` & `chyp-0.2.1/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/__main__.py` & `chyp-0.2.1/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/graph.py` & `chyp-0.2.1/chyp/graph.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/__init__.py` & `chyp-0.2.1/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/app.py` & `chyp-0.2.1/chyp/gui/app.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/codeview.py` & `chyp-0.2.1/chyp/gui/codeview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/document.py` & `chyp-0.2.1/chyp/gui/document.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/editor.py` & `chyp-0.2.1/chyp/gui/editor.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/graphscene.py` & `chyp-0.2.1/chyp/gui/graphscene.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/graphview.py` & `chyp-0.2.1/chyp/gui/graphview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/highlighter.py` & `chyp-0.2.1/chyp/gui/highlighter.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/gui/mainwindow.py` & `chyp-0.2.1/chyp/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/layout.py` & `chyp-0.2.1/chyp/layout.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/matcher.py` & `chyp-0.2.1/chyp/matcher.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/parser.py` & `chyp-0.2.1/chyp/parser.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/rewrite.py` & `chyp-0.2.1/chyp/rewrite.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/rule.py` & `chyp-0.2.1/chyp/rule.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/scraps.py` & `chyp-0.2.1/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/state.py` & `chyp-0.2.1/chyp/state.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp/term.py` & `chyp-0.2.1/chyp/term.py`

 * *Files identical despite different names*

### Comparing `chyp-0.2/chyp.egg-info/PKG-INFO` & `chyp-0.2.1/chyp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.2
-Summary: A compositional hypergraph library
+Version: 0.2.1
+Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chyp-0.2/chyp.egg-info/SOURCES.txt` & `chyp-0.2.1/chyp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chyp-0.2/setup.py` & `chyp-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.2",
+    version="0.2.1",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
-    description="A compositional hypergraph library",
+    description="An interactive theorem prover for monoidal categories",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
         "Bug Tracker": "https://github.com/akissinger/chyp/issues",
     },
     license="Apache2",
```

