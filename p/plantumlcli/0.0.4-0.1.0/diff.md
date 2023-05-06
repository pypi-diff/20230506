# Comparing `tmp/plantumlcli-0.0.4.tar.gz` & `tmp/plantumlcli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantumlcli-0.0.4.tar", last modified: Sat Nov 20 12:30:38 2021, max compression
+gzip compressed data, was "plantumlcli-0.1.0.tar", last modified: Sat May  6 15:02:47 2023, max compression
```

## Comparing `plantumlcli-0.0.4.tar` & `plantumlcli-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-20 12:30:38.825142 plantumlcli-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     9023 2021-11-20 12:30:38.825142 plantumlcli-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7787 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-20 12:30:38.809141 plantumlcli-0.0.4/plantumlcli/
--rw-r--r--   0 runner    (1001) docker     (116)       50 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-20 12:30:38.813141 plantumlcli-0.0.4/plantumlcli/config/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      214 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-20 12:30:38.817141 plantumlcli-0.0.4/plantumlcli/entrance/
--rw-r--r--   0 runner    (1001) docker     (116)       21 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/entrance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1324 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/entrance/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     5922 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/entrance/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     6126 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/entrance/general.py
--rw-r--r--   0 runner    (1001) docker     (116)     1031 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/entrance/local.py
--rw-r--r--   0 runner    (1001) docker     (116)     2654 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/entrance/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-20 12:30:38.817141 plantumlcli-0.0.4/plantumlcli/models/
--rw-r--r--   0 runner    (1001) docker     (116)       95 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4423 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/models/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     4539 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/models/local.py
--rw-r--r--   0 runner    (1001) docker     (116)     4991 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/models/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-20 12:30:38.821142 plantumlcli-0.0.4/plantumlcli/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      290 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2434 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (116)     1881 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (116)      714 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     1905 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (116)      387 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/plantumlcli/utils/function.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-20 12:30:38.813141 plantumlcli-0.0.4/plantumlcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9023 2021-11-20 12:30:38.000000 plantumlcli-0.0.4/plantumlcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      826 2021-11-20 12:30:38.000000 plantumlcli-0.0.4/plantumlcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-11-20 12:30:38.000000 plantumlcli-0.0.4/plantumlcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       62 2021-11-20 12:30:38.000000 plantumlcli-0.0.4/plantumlcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      417 2021-11-20 12:30:38.000000 plantumlcli-0.0.4/plantumlcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-11-20 12:30:38.000000 plantumlcli-0.0.4/plantumlcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-11-20 12:30:38.825142 plantumlcli-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2471 2021-11-20 12:30:09.000000 plantumlcli-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/models/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/models/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/setup.py
```

### Comparing `plantumlcli-0.0.4/LICENSE` & `plantumlcli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/PKG-INFO` & `plantumlcli-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: plantumlcli
-Version: 0.0.4
+Version: 0.1.0
 Summary: An easy-to-use plantuml cli for everyone.
 Home-page: https://github.com/HansBug/plantumlcli
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/HansBug/plantumlcli/blob/main/README.md
 Project-URL: Source, https://github.com/HansBug/plantumlcli
 Project-URL: Issue tracker, https://github.com/HansBug/plantumlcli/issues
-Keywords: An easy-to-use plantuml cli for everyone.
-Platform: UNKNOWN
+Keywords: python,plantuml,diagrams
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 # plantumlcli
 
@@ -63,15 +62,15 @@
 Install from source code
 
 ```bash
 git clone https://github.com/HansBug/plantumlcli
 cd plantumlcli && pip install .
 ```
 
-Python 3.5+ is required, pypy is also tested to be okay.
+Python 3.6+ is required, pypy is also tested to be okay.
 
 ## Using with cli
 
 ### Basic Usage
 
 Show version of `plantumlcli`
 
@@ -193,9 +192,7 @@
 
 ### Version 0.0.1
 
 Released 2020-11-29
 
 * The first official `plantumlcli` version, cheers!!! :beers:
 
-
-
```

### Comparing `plantumlcli-0.0.4/README.md` & `plantumlcli-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 Install from source code
 
 ```bash
 git clone https://github.com/HansBug/plantumlcli
 cd plantumlcli && pip install .
 ```
 
-Python 3.5+ is required, pypy is also tested to be okay.
+Python 3.6+ is required, pypy is also tested to be okay.
 
 ## Using with cli
 
 ### Basic Usage
 
 Show version of `plantumlcli`
```

### Comparing `plantumlcli-0.0.4/plantumlcli/entrance/base.py` & `plantumlcli-0.1.0/plantumlcli/entry/base.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/entrance/cli.py` & `plantumlcli-0.1.0/plantumlcli/entry/cli.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/entrance/general.py` & `plantumlcli-0.1.0/plantumlcli/entry/general.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/entrance/local.py` & `plantumlcli-0.1.0/plantumlcli/entry/local.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/entrance/remote.py` & `plantumlcli-0.1.0/plantumlcli/entry/remote.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/models/base.py` & `plantumlcli-0.1.0/plantumlcli/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,24 +47,24 @@
         """
         pass
 
     @classmethod
     def autoload(cls, *args, **kwargs):
         """
         Autoload plantuml object from given arguments
-        :return: auto-loaded plantuml object
+        :return: autoloaded plantuml object
         """
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     def _check_version(self, version: str):
         pass
 
     @abstractmethod
     def _get_version(self) -> str:
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     @property
     def version(self) -> str:
         """
         Get version information from this plantuml
         :return: version information
         """
@@ -88,15 +88,15 @@
         :return: True if is okay, otherwise False
         """
         self._check()
         return True
 
     @abstractmethod
     def _generate_uml_data(self, type_: PlantumlResourceType, code: str) -> bytes:
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     def dump(self, path: str, type_: Union[int, str, PlantumlResourceType], code: str):
         """
         Dump uml data to file
         :param path: file path
         :param type_: resource type
         :param code: source code
@@ -131,15 +131,15 @@
 
 
 _Tp = TypeVar('_Tp', bound=Plantuml)
 
 
 def try_plantuml(cls: Type[_Tp], *args, **kwargs) -> Tuple[bool, Union[Optional[_Tp], Exception]]:
     """
-    Try initialize plantuml object
+    Try to initialize plantuml object
     :param cls: plantuml class
     :param args: arguments
     :param kwargs: key-word arguments
     :return: (True, Plantuml) when success and (False, Exception) when failed
     """
     try:
         return True, cls.autoload(*args, **kwargs)
```

### Comparing `plantumlcli-0.0.4/plantumlcli/models/local.py` & `plantumlcli-0.1.0/plantumlcli/models/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 import re
+import shutil
 from tempfile import TemporaryDirectory, NamedTemporaryFile
 from typing import Tuple, Optional, Mapping, Any
 
-import where
-
 from .base import Plantuml, PlantumlResourceType
 from ..utils import load_binary_file, save_text_file, CommandLineExecuteError, execute
 
 PLANTUML_JAR_ENV = 'PLANTUML_JAR'
 
 
 def find_java_from_env() -> Optional[str]:
-    return where.first('java')
+    return shutil.which('java')
 
 
 def find_java(java: Optional[str] = None) -> Optional[str]:
     return java or find_java_from_env()
 
 
 def find_plantuml_from_env() -> Optional[str]:
@@ -60,15 +59,15 @@
         Plantuml.__init__(self)
 
         self.__java = java
         self.__plantuml = plantuml
         _check_local(self.__java, self.__plantuml)
 
     @classmethod
-    def autoload(cls, java: str = None, plantuml: str = None, **kwargs) -> 'LocalPlantuml':
+    def autoload(cls, java: Optional[str] = None, plantuml: Optional[str] = None, **kwargs) -> 'LocalPlantuml':
         """
         Autoload LocalPlantuml object from given parameters and the environment
         :param java: java executable file path
         :param plantuml: plantuml jar file path
         :param kwargs: other arguments
         :return: local plantuml object
         """
```

### Comparing `plantumlcli-0.0.4/plantumlcli/models/remote.py` & `plantumlcli-0.1.0/plantumlcli/models/remote.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/utils/concurrent.py` & `plantumlcli-0.1.0/plantumlcli/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/utils/decorator.py` & `plantumlcli-0.1.0/plantumlcli/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/utils/encoding.py` & `plantumlcli-0.1.0/plantumlcli/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/utils/execute.py` & `plantumlcli-0.1.0/plantumlcli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli/utils/file.py` & `plantumlcli-0.1.0/plantumlcli/utils/file.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.0.4/plantumlcli.egg-info/PKG-INFO` & `plantumlcli-0.1.0/plantumlcli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: plantumlcli
-Version: 0.0.4
+Version: 0.1.0
 Summary: An easy-to-use plantuml cli for everyone.
 Home-page: https://github.com/HansBug/plantumlcli
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/HansBug/plantumlcli/blob/main/README.md
 Project-URL: Source, https://github.com/HansBug/plantumlcli
 Project-URL: Issue tracker, https://github.com/HansBug/plantumlcli/issues
-Keywords: An easy-to-use plantuml cli for everyone.
-Platform: UNKNOWN
+Keywords: python,plantuml,diagrams
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 # plantumlcli
 
@@ -63,15 +62,15 @@
 Install from source code
 
 ```bash
 git clone https://github.com/HansBug/plantumlcli
 cd plantumlcli && pip install .
 ```
 
-Python 3.5+ is required, pypy is also tested to be okay.
+Python 3.6+ is required, pypy is also tested to be okay.
 
 ## Using with cli
 
 ### Basic Usage
 
 Show version of `plantumlcli`
 
@@ -193,9 +192,7 @@
 
 ### Version 0.0.1
 
 Released 2020-11-29
 
 * The first official `plantumlcli` version, cheers!!! :beers:
 
-
-
```

### Comparing `plantumlcli-0.0.4/plantumlcli.egg-info/SOURCES.txt` & `plantumlcli-0.1.0/plantumlcli.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements-doc.txt
+requirements-test.txt
+requirements.txt
 setup.py
 plantumlcli/__init__.py
 plantumlcli.egg-info/PKG-INFO
 plantumlcli.egg-info/SOURCES.txt
 plantumlcli.egg-info/dependency_links.txt
 plantumlcli.egg-info/entry_points.txt
 plantumlcli.egg-info/requires.txt
 plantumlcli.egg-info/top_level.txt
 plantumlcli/config/__init__.py
 plantumlcli/config/meta.py
-plantumlcli/entrance/__init__.py
-plantumlcli/entrance/base.py
-plantumlcli/entrance/cli.py
-plantumlcli/entrance/general.py
-plantumlcli/entrance/local.py
-plantumlcli/entrance/remote.py
+plantumlcli/entry/__init__.py
+plantumlcli/entry/base.py
+plantumlcli/entry/cli.py
+plantumlcli/entry/general.py
+plantumlcli/entry/local.py
+plantumlcli/entry/remote.py
 plantumlcli/models/__init__.py
 plantumlcli/models/base.py
 plantumlcli/models/local.py
 plantumlcli/models/remote.py
 plantumlcli/utils/__init__.py
 plantumlcli/utils/concurrent.py
 plantumlcli/utils/decorator.py
```

### Comparing `plantumlcli-0.0.4/setup.py` & `plantumlcli-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,40 +38,40 @@
     ),
     description=meta['__DESCRIPTION__'],
     long_description=readme,
     long_description_content_type='text/markdown',
     author=meta['__AUTHOR__'],
     author_email=meta['__AUTHOR_EMAIL__'],
     license='Apache License, Version 2.0',
-    keywords='An easy-to-use plantuml cli for everyone.',
+    keywords='python, plantuml, diagrams',
     url='https://github.com/HansBug/plantumlcli',
 
     # environment
-    python_requires=">=3.5",
+    python_requires=">=3.7",
     install_requires=requirements,
     tests_require=group_requirements['test'],
     extras_require=group_requirements,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     include_package_data=True,
     project_urls={
         'Documentation': 'https://github.com/HansBug/plantumlcli/blob/main/README.md',
         'Source': 'https://github.com/HansBug/plantumlcli',
         "Issue tracker": "https://github.com/HansBug/plantumlcli/issues",
     },
     entry_points={
         'console_scripts': [
-            'plantumlcli=plantumlcli.entrance.cli:cli'
+            'plantumlcli=plantumlcli.entry.cli:cli'
         ]
     },
 )
```

