# Comparing `tmp/pyutils_basstal-0.4.1.tar.gz` & `tmp/pyutils_basstal-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutils_basstal-0.4.1.tar", last modified: Wed Apr 26 03:59:01 2023, max compression
+gzip compressed data, was "pyutils_basstal-0.4.2.tar", last modified: Sat May  6 09:08:10 2023, max compression
```

## Comparing `pyutils_basstal-0.4.1.tar` & `pyutils_basstal-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 03:59:01.835052 pyutils_basstal-0.4.1/
--rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1473 2023-04-26 03:59:01.835052 pyutils_basstal-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      609 2022-12-30 10:22:58.000000 pyutils_basstal-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 03:59:01.812114 pyutils_basstal-0.4.1/pyutils/
--rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.1/pyutils/__init__.py
--rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.1/pyutils/autoupgrade.py
--rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.1/pyutils/executor.py
--rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.1/pyutils/fsext.py
--rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.1/pyutils/shorthand.py
--rw-rw-rw-   0        0        0     5102 2023-04-25 08:50:55.000000 pyutils_basstal-0.4.1/pyutils/simplelogger.py
--rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.1/pyutils/templite.py
-drwxrwxrwx   0        0        0        0 2023-04-26 03:59:01.834081 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/
--rw-rw-rw-   0        0        0     1473 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 03:59:01.835052 pyutils_basstal-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     8820 2023-04-26 03:57:31.000000 pyutils_basstal-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:08:10.764166 pyutils_basstal-0.4.2/
+-rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1473 2023-05-06 09:08:10.763168 pyutils_basstal-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2022-12-30 10:22:58.000000 pyutils_basstal-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 09:08:10.745216 pyutils_basstal-0.4.2/pyutils/
+-rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.2/pyutils/__init__.py
+-rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.2/pyutils/autoupgrade.py
+-rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.2/pyutils/executor.py
+-rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.2/pyutils/fsext.py
+-rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.2/pyutils/shorthand.py
+-rw-rw-rw-   0        0        0     5159 2023-05-06 09:04:36.000000 pyutils_basstal-0.4.2/pyutils/simplelogger.py
+-rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.2/pyutils/templite.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:08:10.763168 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/
+-rw-rw-rw-   0        0        0     1473 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 09:08:10.764166 pyutils_basstal-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     8820 2023-05-06 09:07:56.000000 pyutils_basstal-0.4.2/setup.py
```

### Comparing `pyutils_basstal-0.4.1/LICENSE.txt` & `pyutils_basstal-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.1/PKG-INFO` & `pyutils_basstal-0.4.2/pyutils_basstal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyutils_basstal
-Version: 0.4.1
+Name: pyutils-basstal
+Version: 0.4.2
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.4.1/README.md` & `pyutils_basstal-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.1/pyutils/autoupgrade.py` & `pyutils_basstal-0.4.2/pyutils/autoupgrade.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.1/pyutils/executor.py` & `pyutils_basstal-0.4.2/pyutils/executor.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.1/pyutils/fsext.py` & `pyutils_basstal-0.4.2/pyutils/fsext.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.1/pyutils/shorthand.py` & `pyutils_basstal-0.4.2/pyutils/shorthand.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.1/pyutils/simplelogger.py` & `pyutils_basstal-0.4.2/pyutils/simplelogger.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         message = SimpleLogger._preprocess_message(message)
         SimpleLogger._info_logger.info(message)
 
     @staticmethod
     def warning(message, bold=False):
         message = SimpleLogger._preprocess_message(message)
         message = SimpleLogger._color_message(message, 33, bold)
-        SimpleLogger._logger.warning(message)
+        SimpleLogger._info_logger.warning(message)
 
     @staticmethod
     def error(message, bold=False):
         if ErrorRaiseExcpetion:
             raise Exception(message)
         message = SimpleLogger._preprocess_message(message)
         message = SimpleLogger._color_message(message, 31, bold)
@@ -82,16 +82,18 @@
             return
         file_handler = SimpleLogger.__hanlder_cache[file_path]
         SimpleLogger._logger.removeHandler(file_handler)
         SimpleLogger._info_logger.removeHandler(file_handler)
         file_handler.close()
         del SimpleLogger.__hanlder_cache[file_path]
 
+
 logger = SimpleLogger._logger
 
+
 def info(message, bold=False):
     SimpleLogger.info(message, bold)
 
 
 def warning(message, bold=False):
     SimpleLogger.warning(message, bold)
 
@@ -107,27 +109,28 @@
                 """NOTE:ignore any parameters after 'message'
 
                 Args:
                     message (_type_): _description_
                 """
                 assertion(message)
                 original_func(message, *args)
+            self.hook_func = real_hook_func
             if original_func == SimpleLogger.warning:
                 SimpleLogger.warning = real_hook_func
             elif original_func == SimpleLogger.info:
                 SimpleLogger.info = real_hook_func
             elif original_func == SimpleLogger.error:
                 SimpleLogger.error = real_hook_func
 
         def __exit__(self, exception_type, exception_value, traceback):
-            if original_func == SimpleLogger.warning:
+            if self.hook_func == SimpleLogger.warning:
                 SimpleLogger.warning = original_func
-            elif original_func == SimpleLogger.info:
+            elif self.hook_func == SimpleLogger.info:
                 SimpleLogger.info = original_func
-            elif original_func == SimpleLogger.error:
+            elif self.hook_func == SimpleLogger.error:
                 SimpleLogger.error = original_func
     return Restore()
 
 
 def hook_info(assertion):
     """给 logger.info 加钩子以检测 info 信息是否符合预期"""
     return __hook__dispatch(assertion, SimpleLogger.info)
```

### Comparing `pyutils_basstal-0.4.1/pyutils/templite.py` & `pyutils_basstal-0.4.2/pyutils/templite.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.1/pyutils_basstal.egg-info/PKG-INFO` & `pyutils_basstal-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyutils-basstal
-Version: 0.4.1
+Name: pyutils_basstal
+Version: 0.4.2
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.4.1/pyutils_basstal.egg-info/SOURCES.txt` & `pyutils_basstal-0.4.2/pyutils_basstal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.1/setup.py` & `pyutils_basstal-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="pyutils_basstal",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.1",  # Required
+    version="0.4.2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="self used py utils",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

