# Comparing `tmp/dynoptimdict-1.0.0.tar.gz` & `tmp/dynoptimdict-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynoptimdict-1.0.0.tar", max compression
+gzip compressed data, was "dynoptimdict-2.0.0.tar", max compression
```

## Comparing `dynoptimdict-1.0.0.tar` & `dynoptimdict-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       97 2023-05-01 09:14:25.789278 dynoptimdict-1.0.0/dynoptimdict/__init__.py
--rw-r--r--   0        0        0     1535 2023-05-01 09:14:25.792284 dynoptimdict-1.0.0/dynoptimdict/dynamic_data_dict.py
--rw-r--r--   0        0        0     1092 2023-04-11 00:59:45.609039 dynoptimdict-1.0.0/LICENSE
--rw-r--r--   0        0        0      808 2023-05-01 10:04:35.653869 dynoptimdict-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1233 2023-05-01 10:02:36.382144 dynoptimdict-1.0.0/README.md
--rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 dynoptimdict-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       84 2023-05-06 06:02:04.891584 dynoptimdict-2.0.0/dynoptimdict/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-06 06:07:00.593217 dynoptimdict-2.0.0/dynoptimdict/dynamic_dict.py
+-rw-r--r--   0        0        0     1092 2023-04-11 00:59:45.609039 dynoptimdict-2.0.0/LICENSE
+-rw-r--r--   0        0        0      802 2023-05-06 06:22:02.332046 dynoptimdict-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1233 2023-05-01 10:02:36.382144 dynoptimdict-2.0.0/README.md
+-rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 dynoptimdict-2.0.0/PKG-INFO
```

### Comparing `dynoptimdict-1.0.0/dynoptimdict/dynamic_data_dict.py` & `dynoptimdict-2.0.0/dynoptimdict/dynamic_dict.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,46 @@
-class DynamicDataDict(dict):
+from typing import Callable
+
+
+class DynamicDict(dict):
     def __init__(self):
         self.__get_value_operate_queue = []
         self.__get_value_operate_arg_list = []
 
-    def __repr__(self):  # Called when the object does not use the dictionary access operator, which is distinguished from calling method:special<__getitem__>.
-        self.__get_value(None)  # Get all dynamic data.
+    def __repr__(self):
+        """
+        Called when the object does not use the dictionary access operator,
+        which is distinguished from calling method:special<__getitem__>.
+        """
+        self.__get_value(None)  # Get all dynamic or static data.
         return super().__repr__()
 
     def __getitem__(self, key):
-        self.__get_value(key)  # Get the specified dynamic data.
+        self.__get_value(key)  # Get the specified dynamic or static data.
         return super().__getitem__(key)
 
-    def __setitem__(self, dynamic_data_name, get_dynamic_data_func: callable):
+    def __setitem__(self, data_name, get_dynamic_data_func_or_static_data_value):
         self.__get_value_operate_queue.append(self.__get_value_operate)
-        self.__get_value_operate_arg_list.append((dynamic_data_name, get_dynamic_data_func))
+        self.__get_value_operate_arg_list.append((data_name, get_dynamic_data_func_or_static_data_value))
 
     def keys(self):
         self.__get_value(None)
         return super().keys()
 
     def values(self):
         self.__get_value(None)
         return super().values()
 
     def items(self):
         self.__get_value(None)
         return super().items()
 
-    def __get_value_operate(self, key, dynamic_data_name, get_dynamic_data_func: callable):
-        if key == dynamic_data_name or key is None:
-            super().__setitem__(dynamic_data_name, get_dynamic_data_func())
+    def __get_value_operate(self, key, data_name, get_dynamic_data_func_or_static_data_value):
+        if key == data_name or key is None:
+            if isinstance(get_dynamic_data_func_or_static_data_value, Callable):  # Store dynamic data.
+                super().__setitem__(data_name, get_dynamic_data_func_or_static_data_value())
+            else:  # Store static data.
+                super().__setitem__(data_name, get_dynamic_data_func_or_static_data_value)
 
     def __get_value(self, key):
         for get_value_operate, get_value_operate_arg in zip(self.__get_value_operate_queue, self.__get_value_operate_arg_list):
             get_value_operate(key, get_value_operate_arg[0], get_value_operate_arg[1])
```

### Comparing `dynoptimdict-1.0.0/LICENSE` & `dynoptimdict-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynoptimdict-1.0.0/pyproject.toml` & `dynoptimdict-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "dynoptimdict"
-version = "1.0.0"
-description = "A dynamic data dict class that inherits and overrides the built-in dict class for special purposes. That provides real-time access to dynamic data, while still allowing the option to get only the specified data without calculating all. It adheres to the concept of program optimization which avoids loading if not used, saving both memory and time."
+version = "2.0.0"
+description = "A dynamic dict class that inherits and overrides the built-in dict class for special purposes. That provides real-time access to dynamic data, while still allowing the option to get only the specified data without calculating all. It adheres to the concept of program optimization which avoids loading if not used, saving both memory and time."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-Dynoptimdict"
 classifiers = [
-    "Development Status :: 3 - Alpha"
+    "Development Status :: 4 - Beta"
 ]
 packages = [{include = "dynoptimdict"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dynoptimdict-1.0.0/README.md` & `dynoptimdict-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dynoptimdict-1.0.0/PKG-INFO` & `dynoptimdict-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dynoptimdict
-Version: 1.0.0
-Summary: A dynamic data dict class that inherits and overrides the built-in dict class for special purposes. That provides real-time access to dynamic data, while still allowing the option to get only the specified data without calculating all. It adheres to the concept of program optimization which avoids loading if not used, saving both memory and time.
+Version: 2.0.0
+Summary: A dynamic dict class that inherits and overrides the built-in dict class for special purposes. That provides real-time access to dynamic data, while still allowing the option to get only the specified data without calculating all. It adheres to the concept of program optimization which avoids loading if not used, saving both memory and time.
 Home-page: https://github.com/leoweyr/Python-Dynoptimdict
 License: MIT
 Author: leoweyr
 Author-email: leoweyr@foxmail.com
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/leoweyr/Python-Dynoptimdict
```

