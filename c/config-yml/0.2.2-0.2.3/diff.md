# Comparing `tmp/config_yml-0.2.2.tar.gz` & `tmp/config_yml-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_yml-0.2.2.tar", last modified: Fri Apr 28 10:56:10 2023, max compression
+gzip compressed data, was "config_yml-0.2.3.tar", last modified: Sat May  6 08:13:11 2023, max compression
```

## Comparing `config_yml-0.2.2.tar` & `config_yml-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 10:56:10.775020 config_yml-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-28 10:55:58.000000 config_yml-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/config_yml/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 10:55:58.000000 config_yml-0.2.2/config_yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-28 10:55:58.000000 config_yml-0.2.2/config_yml/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/config_yml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 10:56:10.000000 config_yml-0.2.2/config_yml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:56:10.775020 config_yml-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-28 10:55:58.000000 config_yml-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:56:10.775020 config_yml-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/data/config_existing.yml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/data/config_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-28 10:55:58.000000 config_yml-0.2.2/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-06 08:13:11.512197 config_yml-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 08:13:01.000000 config_yml-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/config_yml/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 08:13:01.000000 config_yml-0.2.3/config_yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-06 08:13:01.000000 config_yml-0.2.3/config_yml/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/config_yml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 08:13:11.000000 config_yml-0.2.3/config_yml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:13:11.512197 config_yml-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-06 08:13:01.000000 config_yml-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:11.512197 config_yml-0.2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/data/config_existing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/data/config_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-06 08:13:01.000000 config_yml-0.2.3/tests/test_config.py
```

### Comparing `config_yml-0.2.2/PKG-INFO` & `config_yml-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config_yml
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utility modules for Class management
 Home-page: https://github.com/Phornee/config_yml
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `config_yml-0.2.2/config_yml/config.py` & `config_yml-0.2.3/config_yml/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,21 +103,21 @@
 
         if config:
             if template_config:
                 self._merge_config(config, template_config)
                 self.config = template_config
             else:
                 self.config = config
+            self._after_reading()
         else:  # No previous config
             if template_config:  # If config file doesn´t exist, but template does, write config with template content
                 self.update(template_config)
+                self._after_reading()
                 self.write()
 
-        self._after_reading()
-
     def _after_reading(self):
         """ Postprocess to adapt the yaml conig recently read
         """
 
     def _before_writting(self):
         """ By default, it makes nothing and just return a reference to the original member config
             If needed, it can modify the data before reading, and return a copy instead
@@ -141,15 +141,15 @@
         if isinstance(dest_config, dict):
             for key, value in source_config.items():
                 if key not in dest_config:
                     if isinstance(value, dict):
                         dest_config[key] = {}
                     elif isinstance(value, list):
                         dest_config[key] = []
-                if type(value) in [int, str]:
+                if type(value) in [int, str, bool, float, tuple]:
                     dest_config[key] = value
                 Config._merge_config(source_config[key], dest_config[key])
         elif isinstance(dest_config, list):
             if not isinstance(source_config, list):
                 raise TypeError()
             for elem in source_config:
                 if elem not in dest_config:
```

### Comparing `config_yml-0.2.2/config_yml.egg-info/PKG-INFO` & `config_yml-0.2.3/config_yml.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-yml
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utility modules for Class management
 Home-page: https://github.com/Phornee/config_yml
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `config_yml-0.2.2/setup.py` & `config_yml-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="config_yml",
-    version="0.2.2",
+    version="0.2.3",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Utility modules for Class management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/config_yml",
     packages=setuptools.find_packages(),
```

### Comparing `config_yml-0.2.2/tests/test_config.py` & `config_yml-0.2.3/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """ Unit tests """
 import unittest
-import os
 from pathlib import Path
-import shutil
 import yaml
 
 from config_yml import Config
 
 
 class Testing(unittest.TestCase):
     """Unittesting class"""
```

