# Comparing `tmp/datanalyse-0.0.1.tar.gz` & `tmp/datanalyse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanalyse-0.0.1.tar", last modified: Sat May  6 19:21:56 2023, max compression
+gzip compressed data, was "datanalyse-0.0.2.tar", last modified: Sat May  6 20:46:07 2023, max compression
```

## Comparing `datanalyse-0.0.1.tar` & `datanalyse-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-05-06 19:06:32.333418 datanalyse-0.0.1/LICENSE
--rw-r--r--   0        0        0      429 2023-05-06 19:17:22.033872 datanalyse-0.0.1/README.md
--rw-r--r--   0        0        0      609 2023-05-06 19:21:56.959462 datanalyse-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-06 12:49:40.254042 datanalyse-0.0.1/src/datanalyse/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 12:49:40.254042 datanalyse-0.0.1/src/datanalyse/dataelement/__init__.py
--rw-r--r--   0        0        0     8724 2023-05-06 12:49:40.254042 datanalyse-0.0.1/src/datanalyse/dataelement/dataelement.py
--rw-r--r--   0        0        0      919 1970-01-01 00:00:00.000000 datanalyse-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-06 19:06:32.333418 datanalyse-0.0.2/LICENSE
+-rw-r--r--   0        0        0      459 2023-05-06 20:17:48.271205 datanalyse-0.0.2/README.md
+-rw-r--r--   0        0        0      609 2023-05-06 20:46:07.702109 datanalyse-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-05-06 20:41:01.003922 datanalyse-0.0.2/src/datanalyse/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 12:49:40.254042 datanalyse-0.0.2/src/datanalyse/dataelement/__init__.py
+-rw-r--r--   0        0        0     8724 2023-05-06 19:27:23.414206 datanalyse-0.0.2/src/datanalyse/dataelement/dataelement.py
+-rw-r--r--   0        0        0      703 2023-04-28 12:58:07.459695 datanalyse-0.0.2/src/datanalyse/pfade.py
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 datanalyse-0.0.2/PKG-INFO
```

### Comparing `datanalyse-0.0.1/LICENSE` & `datanalyse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.1/pyproject.toml` & `datanalyse-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "pdm-backend",
     "pandas",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "datanalyse"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Maximilian Beyer", email = "maximilian.beyer@tu-dresden.de" },
 ]
 description = "A data analysis package."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `datanalyse-0.0.1/src/datanalyse/dataelement/dataelement.py` & `datanalyse-0.0.2/src/datanalyse/dataelement/dataelement.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.1/PKG-INFO` & `datanalyse-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: datanalyse
-Version: 0.0.1
+Version: 0.0.2
 Summary: A data analysis package.
 Author-Email: Maximilian Beyer <maximilian.beyer@tu-dresden.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/MakusuB/datanalyse
 Project-URL: Bug tracker, https://github.com/MakusuB/datanalyse/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # datanalyse
 
-Datanalyse it a data analysis package - mainly of experimental data from the Combined Energy Lab at TU Dresden, but perhaps useful for others as well. However, due to its absolute alpha status, I cannot recommend it to anybody in the world but me.
+The package name datanalyse is a suitcase word for data and analyse - mainly of experimental data from the Combined Energy Lab at TU Dresden, but perhaps useful for others as well. However, due to its absolute alpha status, I cannot recommend it to anybody in the world but me.
 
 It is more or less a tool-kit for my daily work as an experimentalist and data scientist and makes use of the fantastic packages pandas, pathlib and matplotlib.
```

