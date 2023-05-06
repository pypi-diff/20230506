# Comparing `tmp/findmyorder-1.3.2.tar.gz` & `tmp/findmyorder-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.3.2.tar", max compression
+gzip compressed data, was "findmyorder-1.3.3.tar", max compression
```

## Comparing `findmyorder-1.3.2.tar` & `findmyorder-1.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-06 04:29:32.633521 findmyorder-1.3.2/LICENSE
--rw-r--r--   0        0        0     2155 2023-05-06 04:29:32.633521 findmyorder-1.3.2/README.md
--rw-r--r--   0        0        0      113 2023-05-06 04:29:33.309527 findmyorder-1.3.2/findmyorder/__init__.py
--rw-r--r--   0        0        0      631 2023-05-06 04:29:32.633521 findmyorder-1.3.2/findmyorder/config.py
--rw-r--r--   0        0        0      566 2023-05-06 04:29:32.633521 findmyorder-1.3.2/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     4127 2023-05-06 04:29:32.633521 findmyorder-1.3.2/findmyorder/main.py
--rw-r--r--   0        0        0     1758 2023-05-06 04:29:33.309527 findmyorder-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-06 10:54:59.905983 findmyorder-1.3.3/LICENSE
+-rw-r--r--   0        0        0     2155 2023-05-06 10:54:59.905983 findmyorder-1.3.3/README.md
+-rw-r--r--   0        0        0      113 2023-05-06 10:55:00.561995 findmyorder-1.3.3/findmyorder/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-06 10:54:59.905983 findmyorder-1.3.3/findmyorder/config.py
+-rw-r--r--   0        0        0      566 2023-05-06 10:54:59.905983 findmyorder-1.3.3/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     4129 2023-05-06 10:54:59.905983 findmyorder-1.3.3/findmyorder/main.py
+-rw-r--r--   0        0        0     1758 2023-05-06 10:55:00.561995 findmyorder-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.3/PKG-INFO
```

### Comparing `findmyorder-1.3.2/LICENSE` & `findmyorder-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.2/README.md` & `findmyorder-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.2/findmyorder/config.py` & `findmyorder-1.3.3/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.2/findmyorder/default_settings.toml` & `findmyorder-1.3.3/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.2/findmyorder/main.py` & `findmyorder-1.3.3/findmyorder/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
     async def search(
         self,
         mystring: str,
     ) -> bool:
         """Search an order."""
         try:
-            logging.info(mystring)
+            logging.debug(mystring)
             string_check = mystring.split()[0]
-            logging.info("action identifier %s", settings.action_identifier)
+            logging.debug("action identifier %s", settings.action_identifier)
             if string_check.lower() in settings.action_identifier.lower():
                 logging.debug("found order in %s ", mystring)
                 return True
             logging.debug("no order in : %s using %s", mystring, settings.action_identifier)
             return False
         except Exception as e:
             logging.warning("SearchError: %s", e)
```

### Comparing `findmyorder-1.3.2/pyproject.toml` & `findmyorder-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.3.2"
+version = "1.3.3"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.3.2/PKG-INFO` & `findmyorder-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.3.2
+Version: 1.3.3
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

