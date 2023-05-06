# Comparing `tmp/oronium-1.0.8.tar.gz` & `tmp/oronium-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oronium-1.0.8.tar", max compression
+gzip compressed data, was "oronium-1.0.9.tar", max compression
```

## Comparing `oronium-1.0.8.tar` & `oronium-1.0.9.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    35126 2023-01-14 14:09:35.110191 oronium-1.0.8/LICENSE
--rw-r--r--   0        0        0      845 2023-03-12 11:24:28.254297 oronium-1.0.8/pyproject.toml
--rw-r--r--   0        0        0       28 2023-01-14 14:09:35.112122 oronium-1.0.8/webbot/__init__.py
--rw-r--r--   0        0        0    28783 2023-03-12 11:19:17.973077 oronium-1.0.8/webbot/webbot.py
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 oronium-1.0.8/setup.py
--rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 oronium-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35126 2023-01-14 14:09:35.110191 oronium-1.0.9/LICENSE
+-rw-r--r--   0        0        0      844 2023-05-06 07:46:33.677056 oronium-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-01-14 14:09:35.112122 oronium-1.0.9/webbot/__init__.py
+-rw-r--r--   0        0        0    28783 2023-03-12 11:19:17.973077 oronium-1.0.9/webbot/webbot.py
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 oronium-1.0.9/PKG-INFO
```

### Comparing `oronium-1.0.8/LICENSE` & `oronium-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oronium-1.0.8/pyproject.toml` & `oronium-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "oronium"
-version = "1.0.8"
+version = "1.0.9"
 description = "Webbot selenium driver for testing openremote"
 authors = ["Michal Rutka <michal@openremote.io>"]
 maintainers = ["OpenRemote <developers@openremote.io>"]
 repository = "https://github.com/aktur/webbot"
 keywords = ['webbot', 'selenium', 'chromium']
 classifiers = ["Topic :: Home Automation ", "Topic :: Utilities "]
 license = "AGPLv3"
 packages = [
     { include="webbot", from="." },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 selenium = "^3.141.0"
-webdriver-manager = ">= 3.8.5"
+webdriver-manager = "==3.8.5"
 
 [tool.poetry.dev-dependencies]
 behave = "^1.2.6"
 black = "^20.8b1"
 pre-commit = "^2.10.1"
 
 [build-system]
```

### Comparing `oronium-1.0.8/webbot/webbot.py` & `oronium-1.0.9/webbot/webbot.py`

 * *Files identical despite different names*

### Comparing `oronium-1.0.8/PKG-INFO` & `oronium-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oronium
-Version: 1.0.8
+Version: 1.0.9
 Summary: Webbot selenium driver for testing openremote
 Home-page: https://github.com/aktur/webbot
 License: AGPLv3
 Keywords: webbot,selenium,chromium
 Author: Michal Rutka
 Author-email: michal@openremote.io
 Maintainer: OpenRemote
@@ -16,9 +16,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation 
 Classifier: Topic :: Utilities 
 Requires-Dist: selenium (>=3.141.0,<4.0.0)
-Requires-Dist: webdriver-manager (>=3.8.5)
+Requires-Dist: webdriver-manager (==3.8.5)
 Project-URL: Repository, https://github.com/aktur/webbot
```

