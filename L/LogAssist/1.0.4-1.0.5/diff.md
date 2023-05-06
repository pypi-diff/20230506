# Comparing `tmp/LogAssist-1.0.4.tar.gz` & `tmp/LogAssist-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogAssist-1.0.4.tar", last modified: Fri May  5 08:57:38 2023, max compression
+gzip compressed data, was "LogAssist-1.0.5.tar", last modified: Sat May  6 03:00:32 2023, max compression
```

## Comparing `LogAssist-1.0.4.tar` & `LogAssist-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:57:38.854025 LogAssist-1.0.4/
--rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-05 08:57:38.841626 LogAssist-1.0.4/LogAssist/
--rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.4/LogAssist/__init__.py
--rw-rw-rw-   0        0        0     7282 2023-05-05 08:56:34.000000 LogAssist-1.0.4/LogAssist/log.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:57:38.850485 LogAssist-1.0.4/LogAssist.egg-info/
--rw-rw-rw-   0        0        0     2420 2023-05-05 08:57:38.000000 LogAssist-1.0.4/LogAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-05 08:57:38.000000 LogAssist-1.0.4/LogAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:57:38.000000 LogAssist-1.0.4/LogAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 08:57:38.000000 LogAssist-1.0.4/LogAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2420 2023-05-05 08:57:38.852967 LogAssist-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2023-05-05 01:15:35.000000 LogAssist-1.0.4/README.md
--rw-rw-rw-   0        0        0      709 2023-05-05 08:56:58.000000 LogAssist-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 08:57:38.855033 LogAssist-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-05-05 08:56:52.000000 LogAssist-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:00:32.129565 LogAssist-1.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-06 03:00:32.115585 LogAssist-1.0.5/LogAssist/
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.5/LogAssist/__init__.py
+-rw-rw-rw-   0        0        0     6904 2023-05-06 02:58:52.000000 LogAssist-1.0.5/LogAssist/log.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:00:32.126619 LogAssist-1.0.5/LogAssist.egg-info/
+-rw-rw-rw-   0        0        0     2441 2023-05-06 03:00:31.000000 LogAssist-1.0.5/LogAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-06 03:00:31.000000 LogAssist-1.0.5/LogAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 03:00:31.000000 LogAssist-1.0.5/LogAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 03:00:31.000000 LogAssist-1.0.5/LogAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2441 2023-05-06 03:00:32.128028 LogAssist-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1756 2023-05-06 02:59:35.000000 LogAssist-1.0.5/README.md
+-rw-rw-rw-   0        0        0      709 2023-05-06 03:00:02.000000 LogAssist-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 03:00:32.129565 LogAssist-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      874 2023-05-06 02:59:53.000000 LogAssist-1.0.5/setup.py
```

### Comparing `LogAssist-1.0.4/LICENSE` & `LogAssist-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.4/LogAssist/log.py` & `LogAssist-1.0.5/LogAssist/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,25 +25,23 @@
         5: 'VERB',
         10: 'DEBUG',
         20: 'INFO',
         30: 'WARN',
         40: 'ERROR'
     }
 
-    # Default file name for logging
-    file_name = 'Logger.log'
-
     # Logger information and configuration
     log_info = {
         'prev_remove': False,
         'out_console': True,
         'out_file': True,
+        'log_level': 'debug',
         'dir_name': './log',
         'log_file': 'Logger.log',
-        'log_level': 'debug',
+        'log_path': '',
     }
 
     log_level = level_list['info']
 
     # Initialize the logger with the specified log level, file name, and log removal option
     def init(log_level='verbose', dir_name='./log', file_name='Logger.log', prev_log_remove=False, out_console=True, out_file=True):
         """
@@ -53,34 +51,24 @@
         :param dir_name: The directory name to use for log files. Default is './log'.
         :param file_name: The file name to use for logging. Default is None, which will create a file named "Logger.log".
         :param prev_log_remove: Whether to remove the existing log file on initialization. Default is False.
         :param out_console: Whether to output log messages to the console. Default is True.
         :param out_file: Whether to output log messages to a file. Default is True.
         """
         Logger.set_log_level(log_level)
-        Logger.file_name = file_name
         Logger.log_info['prev_remove'] = prev_log_remove
-        if Logger.log_info['prev_remove']:
-            Logger.log_remove()
-        Logger.log_info['dir_name'] = dir_name
         Logger.log_info['log_level'] = log_level
         Logger.log_info['out_console'] = out_console
         Logger.log_info['out_file'] = out_file
+        Logger.log_info['log_dir'] = dir_name
         Logger.log_info['log_file'] = file_name
-
-    # Initialize the logger with the specified logger information
-    @staticmethod
-    def logger_init(log_info):
-        """
-        :param log_info: a dictionary of logger information, including log level, file name, and logging options
-        """
-        Logger.log_info = log_info
+        Logger.log_info['log_path'] = Logger.log_info['log_dir'] + \
+            "/" + Logger.log_info['log_file']
         if Logger.log_info['prev_remove']:
             Logger.log_remove()
-        Logger.set_log_level(Logger.log_info['log_level'])
 
     # Set the logging level
     @staticmethod
     def set_log_level(log_level: str):
         """
         :param log_level: the log level to set (debug, info, warning, or error)
         """
@@ -98,16 +86,16 @@
     # Remove the log file if the option is enabled
     @staticmethod
     def log_remove():
         """
         Remove the log file if the log_remove option is enabled
         """
         if Logger.log_info['prev_remove']:
-            if os.path.exists(Logger.file_name):
-                os.remove(Logger.file_name)
+            if os.path.exists(Logger.log_info['log_path']):
+                os.remove(Logger.log_info['log_path'])
 
     # Print a log message
     def log_print(tag, message, level, exc_info=None):
         """
         Print a log message
 
         :param tag: The tag to add to the log message
@@ -121,15 +109,15 @@
             if exc_info:
                 traceback_str = "".join(traceback.format_exception(*exc_info))
                 log_p += "\n" + traceback_str
                 log_f += traceback_str
             if Logger.log_info['out_console']:
                 print(log_p)
             if Logger.log_info['out_file']:
-                new_dir_path = Logger.log_info['dir_name'] + "/"
+                new_dir_path = Logger.log_info['log_dir'] + "/"
                 if not os.path.exists(new_dir_path):
                     os.makedirs(new_dir_path)
                 if Logger.log_info['out_file']:
                     with open(new_dir_path + Logger.log_info['log_file'], mode="a") as file:
                         file.write(log_f)
 
     # Log a verbose message
```

### Comparing `LogAssist-1.0.4/LogAssist.egg-info/PKG-INFO` & `LogAssist-1.0.5/LogAssist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
 Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
@@ -41,14 +41,16 @@
 from LogAssist.log import Logger
 ```
 
 2. Initialize the logger with your desired settings:
 
 ```python
 Logger.init(log_level='verbose', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
+# or
+Logger.init()
 ```
 
 3. Use the logger in your code:
 
 ```python
 Logger.verbose('MyTag', 'This is a verbose message')
 Logger.debug('MyTag', 'This is a debug message')
```

### Comparing `LogAssist-1.0.4/PKG-INFO` & `LogAssist-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
 Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
@@ -41,14 +41,16 @@
 from LogAssist.log import Logger
 ```
 
 2. Initialize the logger with your desired settings:
 
 ```python
 Logger.init(log_level='verbose', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
+# or
+Logger.init()
 ```
 
 3. Use the logger in your code:
 
 ```python
 Logger.verbose('MyTag', 'This is a verbose message')
 Logger.debug('MyTag', 'This is a debug message')
```

### Comparing `LogAssist-1.0.4/README.md` & `LogAssist-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from LogAssist.log import Logger
 ```
 
 2. Initialize the logger with your desired settings:
 
 ```python
 Logger.init(log_level='verbose', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
+# or
+Logger.init()
 ```
 
 3. Use the logger in your code:
 
 ```python
 Logger.verbose('MyTag', 'This is a verbose message')
 Logger.debug('MyTag', 'This is a debug message')
```

### Comparing `LogAssist-1.0.4/pyproject.toml` & `LogAssist-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LogAssist"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "A simple and customizable logging library for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `LogAssist-1.0.4/setup.py` & `LogAssist-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='LogAssist',
-    version='1.0.4',
+    version='1.0.5',
     description='LogAssist package',
     author='horrible-gh',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/LogAssist.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

