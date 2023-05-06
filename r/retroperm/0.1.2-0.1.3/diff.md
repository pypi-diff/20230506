# Comparing `tmp/retroperm-0.1.2.tar.gz` & `tmp/retroperm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retroperm-0.1.2.tar", last modified: Sat May  6 02:01:44 2023, max compression
+gzip compressed data, was "retroperm-0.1.3.tar", last modified: Sat May  6 02:31:25 2023, max compression
```

## Comparing `retroperm-0.1.2.tar` & `retroperm-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:01:44.178377 retroperm-0.1.2/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     7647 2023-04-13 09:48:15.000000 retroperm-0.1.2/LICENSE
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-05-06 02:01:44.178377 retroperm-0.1.2/PKG-INFO
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      239 2023-03-30 22:52:41.000000 retroperm-0.1.2/README.md
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      564 2023-05-06 02:01:35.000000 retroperm-0.1.2/pyproject.toml
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:01:44.174377 retroperm-0.1.2/retroperm/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       22 2023-03-30 22:52:41.000000 retroperm-0.1.2/retroperm/__init__.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:01:44.178377 retroperm-0.1.2/retroperm/analysis/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:41.000000 retroperm-0.1.2/retroperm/analysis/__init__.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1676 2023-03-30 22:52:41.000000 retroperm-0.1.2/retroperm/analysis/functions.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      713 2023-03-30 15:19:36.000000 retroperm-0.1.2/retroperm/analysis/permfinder.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     4225 2023-03-28 14:41:57.000000 retroperm-0.1.2/retroperm/analysis/resolver.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1969 2023-04-01 19:20:53.000000 retroperm-0.1.2/retroperm/analysis/utils.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     1372 2023-03-24 18:26:08.000000 retroperm-0.1.2/retroperm/analysis/utils_angrmgmt.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     9088 2023-04-26 00:16:19.000000 retroperm-0.1.2/retroperm/project.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:01:44.178377 retroperm-0.1.2/retroperm/rules/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      182 2023-04-27 19:14:13.000000 retroperm-0.1.2/retroperm/rules/__init__.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      147 2023-04-18 01:01:52.000000 retroperm-0.1.2/retroperm/rules/argument_rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      697 2023-04-25 15:27:54.000000 retroperm-0.1.2/retroperm/rules/ban_category_rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      995 2023-04-25 15:25:33.000000 retroperm-0.1.2/retroperm/rules/ban_library_function_rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     2240 2023-04-25 15:15:54.000000 retroperm-0.1.2/retroperm/rules/data.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       43 2023-04-11 22:53:49.000000 retroperm-0.1.2/retroperm/rules/default_rules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     4005 2023-05-06 01:58:11.000000 retroperm-0.1.2/retroperm/rules/filesystem_rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      241 2023-04-06 17:49:41.000000 retroperm-0.1.2/retroperm/rules/pathrules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      571 2023-04-20 18:44:23.000000 retroperm-0.1.2/retroperm/rules/rule.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      754 2023-03-30 17:57:42.000000 retroperm-0.1.2/retroperm/rules/ruleList.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:22.000000 retroperm-0.1.2/retroperm/rules/rules.py
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-30 01:49:39.000000 retroperm-0.1.2/retroperm/setup.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:01:44.178377 retroperm-0.1.2/retroperm.egg-info/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-05-06 02:01:44.000000 retroperm-0.1.2/retroperm.egg-info/PKG-INFO
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      832 2023-05-06 02:01:44.000000 retroperm-0.1.2/retroperm.egg-info/SOURCES.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)        1 2023-05-06 02:01:44.000000 retroperm-0.1.2/retroperm.egg-info/dependency_links.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       32 2023-05-06 02:01:44.000000 retroperm-0.1.2/retroperm.egg-info/requires.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       10 2023-05-06 02:01:44.000000 retroperm-0.1.2/retroperm.egg-info/top_level.txt
--rw-rw-r--   0 spyre     (1000) spyre     (1000)      550 2023-05-06 02:01:44.178377 retroperm-0.1.2/setup.cfg
--rw-rw-r--   0 spyre     (1000) spyre     (1000)       37 2023-03-30 22:52:41.000000 retroperm-0.1.2/setup.py
-drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:01:44.178377 retroperm-0.1.2/tests/
--rw-rw-r--   0 spyre     (1000) spyre     (1000)     5661 2023-04-26 00:20:51.000000 retroperm-0.1.2/tests/test_project.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:31:25.714818 retroperm-0.1.3/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     7647 2023-04-13 09:48:15.000000 retroperm-0.1.3/LICENSE
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-05-06 02:31:25.714818 retroperm-0.1.3/PKG-INFO
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      239 2023-03-30 22:52:41.000000 retroperm-0.1.3/README.md
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      564 2023-05-06 02:31:14.000000 retroperm-0.1.3/pyproject.toml
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:31:25.710818 retroperm-0.1.3/retroperm/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       22 2023-03-30 22:52:41.000000 retroperm-0.1.3/retroperm/__init__.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:31:25.710818 retroperm-0.1.3/retroperm/analysis/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:41.000000 retroperm-0.1.3/retroperm/analysis/__init__.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1676 2023-03-30 22:52:41.000000 retroperm-0.1.3/retroperm/analysis/functions.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      713 2023-03-30 15:19:36.000000 retroperm-0.1.3/retroperm/analysis/permfinder.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     4225 2023-03-28 14:41:57.000000 retroperm-0.1.3/retroperm/analysis/resolver.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1969 2023-04-01 19:20:53.000000 retroperm-0.1.3/retroperm/analysis/utils.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     1372 2023-03-24 18:26:08.000000 retroperm-0.1.3/retroperm/analysis/utils_angrmgmt.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     9088 2023-04-26 00:16:19.000000 retroperm-0.1.3/retroperm/project.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:31:25.710818 retroperm-0.1.3/retroperm/rules/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      182 2023-04-27 19:14:13.000000 retroperm-0.1.3/retroperm/rules/__init__.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      147 2023-04-18 01:01:52.000000 retroperm-0.1.3/retroperm/rules/argument_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      697 2023-04-25 15:27:54.000000 retroperm-0.1.3/retroperm/rules/ban_category_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      995 2023-04-25 15:25:33.000000 retroperm-0.1.3/retroperm/rules/ban_library_function_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     2240 2023-04-25 15:15:54.000000 retroperm-0.1.3/retroperm/rules/data.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       43 2023-04-11 22:53:49.000000 retroperm-0.1.3/retroperm/rules/default_rules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     2766 2023-05-06 02:28:04.000000 retroperm-0.1.3/retroperm/rules/filesystem_rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      241 2023-04-06 17:49:41.000000 retroperm-0.1.3/retroperm/rules/pathrules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      571 2023-04-20 18:44:23.000000 retroperm-0.1.3/retroperm/rules/rule.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      754 2023-03-30 17:57:42.000000 retroperm-0.1.3/retroperm/rules/ruleList.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-24 14:52:22.000000 retroperm-0.1.3/retroperm/rules/rules.py
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        0 2023-03-30 01:49:39.000000 retroperm-0.1.3/retroperm/setup.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:31:25.710818 retroperm-0.1.3/retroperm.egg-info/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      882 2023-05-06 02:31:25.000000 retroperm-0.1.3/retroperm.egg-info/PKG-INFO
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      832 2023-05-06 02:31:25.000000 retroperm-0.1.3/retroperm.egg-info/SOURCES.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)        1 2023-05-06 02:31:25.000000 retroperm-0.1.3/retroperm.egg-info/dependency_links.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       32 2023-05-06 02:31:25.000000 retroperm-0.1.3/retroperm.egg-info/requires.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       10 2023-05-06 02:31:25.000000 retroperm-0.1.3/retroperm.egg-info/top_level.txt
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)      550 2023-05-06 02:31:25.714818 retroperm-0.1.3/setup.cfg
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)       37 2023-03-30 22:52:41.000000 retroperm-0.1.3/setup.py
+drwxrwxr-x   0 spyre     (1000) spyre     (1000)        0 2023-05-06 02:31:25.714818 retroperm-0.1.3/tests/
+-rw-rw-r--   0 spyre     (1000) spyre     (1000)     5661 2023-04-26 00:20:51.000000 retroperm-0.1.3/tests/test_project.py
```

### Comparing `retroperm-0.1.2/LICENSE` & `retroperm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/PKG-INFO` & `retroperm-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retroperm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A retroactive effective binary permission deduction tool
 Home-page: https://github.com/SpiritSeal/retroperm
 Author-email: Saketh Reddy <yssaketh@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SpiritSeal/retroperm
 Project-URL: Bug Tracker, https://github.com/SpiritSeal/retroperm/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `retroperm-0.1.2/pyproject.toml` & `retroperm-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retroperm"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Saketh Reddy", email="yssaketh@gmail.com" },
 ]
 description = "A retroactive effective binary permission deduction tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `retroperm-0.1.2/retroperm/analysis/functions.py` & `retroperm-0.1.3/retroperm/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/analysis/permfinder.py` & `retroperm-0.1.3/retroperm/analysis/permfinder.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/analysis/resolver.py` & `retroperm-0.1.3/retroperm/analysis/resolver.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/analysis/utils.py` & `retroperm-0.1.3/retroperm/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/analysis/utils_angrmgmt.py` & `retroperm-0.1.3/retroperm/analysis/utils_angrmgmt.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/project.py` & `retroperm-0.1.3/retroperm/project.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/rules/ban_category_rule.py` & `retroperm-0.1.3/retroperm/rules/ban_category_rule.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/rules/ban_library_function_rule.py` & `retroperm-0.1.3/retroperm/rules/ban_library_function_rule.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/rules/data.py` & `retroperm-0.1.3/retroperm/rules/data.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/rules/rule.py` & `retroperm-0.1.3/retroperm/rules/rule.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm/rules/ruleList.py` & `retroperm-0.1.3/retroperm/rules/ruleList.py`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/retroperm.egg-info/PKG-INFO` & `retroperm-0.1.3/retroperm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retroperm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A retroactive effective binary permission deduction tool
 Home-page: https://github.com/SpiritSeal/retroperm
 Author-email: Saketh Reddy <yssaketh@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SpiritSeal/retroperm
 Project-URL: Bug Tracker, https://github.com/SpiritSeal/retroperm/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `retroperm-0.1.2/retroperm.egg-info/SOURCES.txt` & `retroperm-0.1.3/retroperm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/setup.cfg` & `retroperm-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `retroperm-0.1.2/tests/test_project.py` & `retroperm-0.1.3/tests/test_project.py`

 * *Files identical despite different names*

