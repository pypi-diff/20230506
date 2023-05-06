# Comparing `tmp/LogAssist-1.0.5.tar.gz` & `tmp/LogAssist-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogAssist-1.0.5.tar", last modified: Sat May  6 03:00:32 2023, max compression
+gzip compressed data, was "LogAssist-1.0.6.tar", last modified: Sat May  6 03:08:48 2023, max compression
```

## Comparing `LogAssist-1.0.5.tar` & `LogAssist-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:00:32.129565 LogAssist-1.0.5/
--rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.5/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-06 03:00:32.115585 LogAssist-1.0.5/LogAssist/
--rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.5/LogAssist/__init__.py
--rw-rw-rw-   0        0        0     6904 2023-05-06 02:58:52.000000 LogAssist-1.0.5/LogAssist/log.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:00:32.126619 LogAssist-1.0.5/LogAssist.egg-info/
--rw-rw-rw-   0        0        0     2441 2023-05-06 03:00:31.000000 LogAssist-1.0.5/LogAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-06 03:00:31.000000 LogAssist-1.0.5/LogAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:00:31.000000 LogAssist-1.0.5/LogAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 03:00:31.000000 LogAssist-1.0.5/LogAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2441 2023-05-06 03:00:32.128028 LogAssist-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1756 2023-05-06 02:59:35.000000 LogAssist-1.0.5/README.md
--rw-rw-rw-   0        0        0      709 2023-05-06 03:00:02.000000 LogAssist-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 03:00:32.129565 LogAssist-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-05-06 02:59:53.000000 LogAssist-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:08:48.334051 LogAssist-1.0.6/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.6/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-06 03:08:48.321787 LogAssist-1.0.6/LogAssist/
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.6/LogAssist/__init__.py
+-rw-rw-rw-   0        0        0     6990 2023-05-06 03:07:24.000000 LogAssist-1.0.6/LogAssist/log.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:08:48.330517 LogAssist-1.0.6/LogAssist.egg-info/
+-rw-rw-rw-   0        0        0     2441 2023-05-06 03:08:47.000000 LogAssist-1.0.6/LogAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-06 03:08:48.000000 LogAssist-1.0.6/LogAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 03:08:47.000000 LogAssist-1.0.6/LogAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 03:08:47.000000 LogAssist-1.0.6/LogAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2441 2023-05-06 03:08:48.332546 LogAssist-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1756 2023-05-06 02:59:35.000000 LogAssist-1.0.6/README.md
+-rw-rw-rw-   0        0        0      709 2023-05-06 03:08:32.000000 LogAssist-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 03:08:48.335057 LogAssist-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      874 2023-05-06 03:08:39.000000 LogAssist-1.0.6/setup.py
```

### Comparing `LogAssist-1.0.5/LICENSE` & `LogAssist-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.5/LogAssist/log.py` & `LogAssist-1.0.6/LogAssist/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,18 @@
         :param out_file: Whether to output log messages to a file. Default is True.
         """
         Logger.set_log_level(log_level)
         Logger.log_info['prev_remove'] = prev_log_remove
         Logger.log_info['log_level'] = log_level
         Logger.log_info['out_console'] = out_console
         Logger.log_info['out_file'] = out_file
-        Logger.log_info['log_dir'] = dir_name
+        if dir_name:
+            Logger.log_info['log_dir'] = dir_name
+        else:
+            Logger.log_info['log_dir'] = ''
         Logger.log_info['log_file'] = file_name
         Logger.log_info['log_path'] = Logger.log_info['log_dir'] + \
             "/" + Logger.log_info['log_file']
         if Logger.log_info['prev_remove']:
             Logger.log_remove()
 
     # Set the logging level
```

### Comparing `LogAssist-1.0.5/LogAssist.egg-info/PKG-INFO` & `LogAssist-1.0.6/LogAssist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
 Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
```

### Comparing `LogAssist-1.0.5/PKG-INFO` & `LogAssist-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
 Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
```

### Comparing `LogAssist-1.0.5/README.md` & `LogAssist-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.5/pyproject.toml` & `LogAssist-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LogAssist"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "A simple and customizable logging library for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `LogAssist-1.0.5/setup.py` & `LogAssist-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='LogAssist',
-    version='1.0.5',
+    version='1.0.6',
     description='LogAssist package',
     author='horrible-gh',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/LogAssist.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

