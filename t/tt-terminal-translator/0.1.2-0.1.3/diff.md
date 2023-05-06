# Comparing `tmp/tt_terminal_translator-0.1.2.tar.gz` & `tmp/tt_terminal_translator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tt_terminal_translator-0.1.2.tar", max compression
+gzip compressed data, was "tt_terminal_translator-0.1.3.tar", max compression
```

## Comparing `tt_terminal_translator-0.1.2.tar` & `tt_terminal_translator-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.2/LICENSE
--rw-r--r--   0        0        0     1895 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.2/README.md
--rw-r--r--   0        0        0     1725 2023-05-06 03:14:58.833218 tt_terminal_translator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2439 2023-05-06 03:14:32.129998 tt_terminal_translator-0.1.2/src/terminal_translator/config.py
--rw-r--r--   0        0        0     2517 2023-05-06 03:14:41.539958 tt_terminal_translator-0.1.2/src/terminal_translator/main.py
--rw-r--r--   0        0        0      452 2023-05-06 03:14:32.106665 tt_terminal_translator-0.1.2/src/terminal_translator/version.py
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1895 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.3/README.md
+-rw-r--r--   0        0        0     1725 2023-05-06 03:29:50.160326 tt_terminal_translator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2439 2023-05-06 03:14:32.129998 tt_terminal_translator-0.1.3/src/terminal_translator/config.py
+-rw-r--r--   0        0        0     2517 2023-05-06 03:14:41.539958 tt_terminal_translator-0.1.3/src/terminal_translator/main.py
+-rw-r--r--   0        0        0      359 2023-05-06 03:29:43.733677 tt_terminal_translator-0.1.3/src/terminal_translator/version.py
+-rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.3/PKG-INFO
```

### Comparing `tt_terminal_translator-0.1.2/LICENSE` & `tt_terminal_translator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.2/README.md` & `tt_terminal_translator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.2/pyproject.toml` & `tt_terminal_translator-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tt-terminal-translator"
-version = "0.1.2"
+version = "0.1.3"
 description = "Terminal Translator is a translation CLI that uses the Google Cloud API. "
 authors = ["gbPagano <guilhermebpagano@gmail.com>"]
 readme = "README.md"
 packages = [{include = "terminal_translator", from = "src"}]
 classifiers = [  
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tt_terminal_translator-0.1.2/src/terminal_translator/config.py` & `tt_terminal_translator-0.1.3/src/terminal_translator/config.py`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.2/src/terminal_translator/main.py` & `tt_terminal_translator-0.1.3/src/terminal_translator/main.py`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.2/PKG-INFO` & `tt_terminal_translator-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tt-terminal-translator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Terminal Translator is a translation CLI that uses the Google Cloud API. 
 Author: gbPagano
 Author-email: guilhermebpagano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

