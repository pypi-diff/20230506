# Comparing `tmp/findmyorder-1.3.3.tar.gz` & `tmp/findmyorder-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.3.3.tar", max compression
+gzip compressed data, was "findmyorder-1.3.4.tar", max compression
```

## Comparing `findmyorder-1.3.3.tar` & `findmyorder-1.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-06 10:54:59.905983 findmyorder-1.3.3/LICENSE
--rw-r--r--   0        0        0     2155 2023-05-06 10:54:59.905983 findmyorder-1.3.3/README.md
--rw-r--r--   0        0        0      113 2023-05-06 10:55:00.561995 findmyorder-1.3.3/findmyorder/__init__.py
--rw-r--r--   0        0        0      631 2023-05-06 10:54:59.905983 findmyorder-1.3.3/findmyorder/config.py
--rw-r--r--   0        0        0      566 2023-05-06 10:54:59.905983 findmyorder-1.3.3/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     4129 2023-05-06 10:54:59.905983 findmyorder-1.3.3/findmyorder/main.py
--rw-r--r--   0        0        0     1758 2023-05-06 10:55:00.561995 findmyorder-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-06 20:06:50.638873 findmyorder-1.3.4/LICENSE
+-rw-r--r--   0        0        0     2155 2023-05-06 20:06:50.638873 findmyorder-1.3.4/README.md
+-rw-r--r--   0        0        0      113 2023-05-06 20:06:51.298876 findmyorder-1.3.4/findmyorder/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-06 20:06:50.638873 findmyorder-1.3.4/findmyorder/config.py
+-rw-r--r--   0        0        0      566 2023-05-06 20:06:50.638873 findmyorder-1.3.4/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     4135 2023-05-06 20:06:50.638873 findmyorder-1.3.4/findmyorder/main.py
+-rw-r--r--   0        0        0     1758 2023-05-06 20:06:51.298876 findmyorder-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 findmyorder-1.3.4/PKG-INFO
```

### Comparing `findmyorder-1.3.3/LICENSE` & `findmyorder-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.3/README.md` & `findmyorder-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.3/findmyorder/config.py` & `findmyorder-1.3.4/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.3/findmyorder/default_settings.toml` & `findmyorder-1.3.4/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.3.3/findmyorder/main.py` & `findmyorder-1.3.4/findmyorder/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
  FindMyOrder Main
 """
 import logging
 from datetime import datetime
 
-from pyparsing import Combine, Optional, Word, alphas, nums, one_of, pyparsing_common,  Suppress
+from pyparsing import (
+    Combine, Optional, Word, alphas,
+    nums, one_of, pyparsing_common,
+    Suppress)
 
 from .config import settings
 
 
 class FindMyOrder:
     """find an order class """
 
@@ -25,54 +28,55 @@
         try:
             logging.debug(mystring)
             string_check = mystring.split()[0]
             logging.debug("action identifier %s", settings.action_identifier)
             if string_check.lower() in settings.action_identifier.lower():
                 logging.debug("found order in %s ", mystring)
                 return True
-            logging.debug("no order in : %s using %s", mystring, settings.action_identifier)
+            logging.debug("no order found")
             return False
         except Exception as e:
             logging.warning("SearchError: %s", e)
             return False
 
     async def identify_order(
             self,
             mystring: str,
             ) -> dict:
         """Identify an order."""
         logging.debug("identify_order: %s", mystring)
         try:
             action = one_of(
                 settings.action_identifier, caseless=True
-                ).set_results_name("action").set_parse_action(pyparsing_common.upcase_tokens)
+                ).set_results_name("action").set_parse_action(
+                    pyparsing_common.upcase_tokens)
             instrument = Word(
                 alphas
                 ).set_results_name("instrument")
             stop_loss = Combine(
-                    Suppress(settings.stop_loss_identifier) 
+                    Suppress(settings.stop_loss_identifier)
                     + Word(nums)
                 ).set_results_name("stop_loss")
             take_profit = Combine(
-                Suppress(settings.take_profit_identifier) 
+                Suppress(settings.take_profit_identifier)
                 + Word(nums)
                 ).set_results_name("take_profit")
             quantity = Combine(
-                Suppress(settings.quantity_identifier) 
+                Suppress(settings.quantity_identifier)
                 + Word(nums)
                 + Optional(Suppress("%"))
                 ).set_results_name("quantity")
             order_type = one_of(
                 settings.order_type_identifier, caseless=True
                 ).set_results_name("order_type")
             leverage_type = one_of(
                 settings.leverage_type_identifier, caseless=True
                 ).set_results_name("leverage_type")
             comment = Combine(
-                    Suppress(settings.comment_identifier) 
+                    Suppress(settings.comment_identifier)
                     + Word(alphas)
                 ).set_results_name("comment")
 
             # for action in settings.actions:
             # print(f"{action.identifier} ({action.type})")
             order_grammar = (
                 action("action")
@@ -96,24 +100,25 @@
         except Exception as e:
             logging.exception("IdentifyError: %s", e)
             return None
 
     async def get_order(
         self,
         msg: str,
-        ):
+    ):
         """get an order."""
         try:
             logging.debug("get_order %s", msg)
 
             if await self.search(msg):
                 logging.info("get_order found in %s", msg)
                 order = await self.identify_order(msg)
                 logging.info("order: %s", order)
                 if isinstance(order, dict):
-                    order["timestamp"] = datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
+                    order["timestamp"] = datetime.utcnow().strftime(
+                        "%Y-%m-%dT%H:%M:%SZ")
                 return order
             return None
 
         except Exception as e:
             logging.exception("GetOrderError: %s", e)
             return None
```

### Comparing `findmyorder-1.3.3/pyproject.toml` & `findmyorder-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.3.3"
+version = "1.3.4"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.3.3/PKG-INFO` & `findmyorder-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.3.3
+Version: 1.3.4
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

