# Comparing `tmp/py_basic_commands-0.2.1.tar.gz` & `tmp/py_basic_commands-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_basic_commands-0.2.1.tar", last modified: Tue Apr  4 15:35:44 2023, max compression
+gzip compressed data, was "py_basic_commands-0.2.20.tar", last modified: Sat May  6 00:56:43 2023, max compression
```

## Comparing `py_basic_commands-0.2.1.tar` & `py_basic_commands-0.2.20.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:35:44.876767 py_basic_commands-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-04-04 15:35:44.876767 py_basic_commands-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:35:44.872767 py_basic_commands-0.2.1/py_basic_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/example_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:35:44.872767 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/create_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/create_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/get_src_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/join_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/remove_file_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/write_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:35:44.872767 py_basic_commands-0.2.1/py_basic_commands/fscripts/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/fscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/fscripts/finput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/fscripts/fprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/fscripts/fprint_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:35:44.872767 py_basic_commands-0.2.1/py_basic_commands/json_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/json_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/json_scripts/create_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/json_scripts/read_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/json_scripts/write_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:35:44.876767 py_basic_commands-0.2.1/py_basic_commands/other/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/other/basic_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/other/choose_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/other/function_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/py_basic_commands/other/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:35:44.872767 py_basic_commands-0.2.1/py_basic_commands.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-04-04 15:35:44.000000 py_basic_commands-0.2.1/py_basic_commands.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-04 15:35:44.000000 py_basic_commands-0.2.1/py_basic_commands.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:35:44.000000 py_basic_commands-0.2.1/py_basic_commands.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 15:35:44.000000 py_basic_commands-0.2.1/py_basic_commands.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-04 15:35:34.000000 py_basic_commands-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-04 15:35:44.876767 py_basic_commands-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.127602 py_basic_commands-0.2.20/py_basic_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/example_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.127602 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/create_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/get_src_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/join_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/remove_file_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/write_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/py_basic_commands/fscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/fscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/fscripts/finput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/fscripts/fprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/fscripts/fprint_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/py_basic_commands/json_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/json_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/json_scripts/create_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/json_scripts/read_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/json_scripts/write_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/py_basic_commands/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/basic_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/choose_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/function_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.127602 py_basic_commands-0.2.20/py_basic_commands.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 00:56:43.000000 py_basic_commands-0.2.20/py_basic_commands.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-06 00:56:43.000000 py_basic_commands-0.2.20/py_basic_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:56:43.000000 py_basic_commands-0.2.20/py_basic_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 00:56:43.000000 py_basic_commands-0.2.20/py_basic_commands.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/setup.cfg
```

### Comparing `py_basic_commands-0.2.1/LICENSE.md` & `py_basic_commands-0.2.20/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.1/PKG-INFO` & `py_basic_commands-0.2.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_basic_commands
-Version: 0.2.1
+Version: 0.2.20
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.1/README.md` & `py_basic_commands-0.2.20/README.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/__init__.py` & `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-from py_basic_commands.file_dir_scripts.create_dirs       import create_dirs
-from py_basic_commands.file_dir_scripts.create_file       import create_file
-from py_basic_commands.file_dir_scripts.get_src_path      import get_src_path
-from py_basic_commands.file_dir_scripts.join_path         import join_path
-from py_basic_commands.file_dir_scripts.read_file         import read_file
-from py_basic_commands.file_dir_scripts.remove_file_dir   import remove_file_dir
-from py_basic_commands.file_dir_scripts.write_file        import write_file
+from py_basic_commands.file_dir_scripts.create_dirs       import create_dirs, CreateDirs
+from py_basic_commands.file_dir_scripts.create_file       import create_file, CreateFile
+from py_basic_commands.file_dir_scripts.get_src_path      import get_src_path, GetSourcePath
+from py_basic_commands.file_dir_scripts.join_path         import join_path, JoinPath
+from py_basic_commands.file_dir_scripts.read_file         import read_file, ReadFile
+from py_basic_commands.file_dir_scripts.remove_file_dir   import remove_file_dir, RemoveFileDir
+from py_basic_commands.file_dir_scripts.write_file        import write_file, WriteFile
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/create_dirs.py` & `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/create_dirs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 from py_basic_commands.file_dir_scripts.get_src_path  import get_src_path
-from dataclasses    import dataclass
 from py_basic_commands.fscripts   import fprint
 from py_basic_commands.base   import Base
+from dataclasses    import dataclass
 from os     import makedirs
 
 @dataclass
 class CreateDirs(Base):
     def __post_init__(self):
         super().__init__()
 
 
-    def config(self, **kwargs):
-        """Conmfigure `create_dirs` variables"""
-        self._config(**kwargs)
-
-
     def __call__(self, dst_path:str, do_print:bool=None) -> bool:
             """Create all required directories for the given path.
             
             Parameters:
             - `dst_path` (str): Destination path; can include the file name at the end.
             - `do_print` (bool): Whether to print or not. Default is `True`
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/create_file.py` & `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/create_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,14 @@
 @dataclass
 class CreateFile(Base):
     _force:bool = False
 
     def __post_init__(self):
         super().__init__()
 
-    
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'force':
-                self._force = value
-
 
     def _create_empty_file(self, dst_path:str) -> bool:
         """Create an empty file at the specified path.
         
         Parameters:
         - `dst_path` (str): The path to create the file at.
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/get_src_path.py` & `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/get_src_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,24 @@
 class GetSourcePath(Base):
     _ret_val:bool = 'a'
 
     def __post_init__(self):
         super().__init__()
 
 
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'ret_val':
-                self._ret_val = value
-
-
     def __call__(self, src_path:str, ret_val=None, do_print:bool=None) -> Any:
         """Get the path for the given source.
         
         Parameters:
         - `src_path` (str): The path to the source.
-        - `ret_val` (str): Whether to return the `'d'`irectory path, `'fnam'`e of the file, or `'a'`ll (default).
-        
+        - `ret_val` (str): Whether to return the 
+            - `'d'`: directory path
+            - `'fnam'`: name of the file
+            - `'a'`: all (default)
+
         Returns:
         - `Any`: If `ret_val` is `'d'`, the directory path. If `ret_val` is `'fnam'`, the filename. Otherwise, a tuple containing the directory path and the filename.
         """
 
         if not src_path:
             fprint('No source path given')
             return None
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/join_path.py` & `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/join_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,14 @@
     _remove_empty:bool=True
     _dir_end:bool=False
 
     def __post_init__(self):
         super().__init__(False)
 
 
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'join_with':
-                self._join_with = value
-            elif key == 'remove_empty':
-                self._remove_empty = value
-            elif key == 'dir_end':
-                self._dir_end = value
-
-
     def __call__(self, *args:str, join_with:str=None, remove_empty:bool=None, dir_end:bool=None, do_print:bool=None) -> str:
         r"""Join path segments together, removing certain characters (`<>:"/\|?*`) and adjust for correct slash direction.
 
         Parameters:
         - `*args` (str): One or more path segments to join.
         - `join_with` (str): The separator to use when joining the path segments. Default is `'/'`.
         - `remove_empty` (bool): Remove empty strings. Default is `True`.
@@ -54,15 +41,15 @@
         fprint.config(do_print=do_print)
 
         # Iterate through args and join them together
         new_args = []
         for arg_indx, arg in enumerate(args):
             # Remove invalid characters
             arg = split_join(split_join(arg, '\\'), '/')
-            arg = arg.translate({ord(c): None for c in '<>:"|?*'})
+            arg = arg.translate({ord(c): None for c in '<>"|?*'}) # ":" is an invalid character on Windows, but drivers can use it. E.g. "C:\"
 
             # Remove empty strings
             split_arg = arg.split('/')
             if '' in split_arg and remove_empty:
                 fprint(f'Empty string found in input arg (indx: {arg_indx}): {arg!r}')
                 split_arg = [x for x in split_arg if x != '']
                 arg = join_with.join(split_arg)
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/read_file.py` & `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/read_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,35 +15,14 @@
     _do_lower:bool = False
     _encoding:str = 'utf-8'
 
 
     def __post_init__(self):
         super().__init__()
 
-
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'create':
-                self._create = value
-            elif key == 'ret_did_create':
-                self._ret_did_create = value
-            elif key == 'splitlines':
-                self._splitlines = value
-            elif key == 'remove_empty':
-                self._remove_empty = value
-            elif key == 'do_strip':
-                self._do_strip = value
-            elif key == 'do_lower':
-                self._do_lower = value
-            elif key == 'encoding':
-                self._encoding = value
-
     
     def __call__(self, file_path:str, create:bool=None, ret_did_create:bool=None, splitlines:bool=None, remove_empty:bool=None, do_strip:bool=None, do_lower:bool=None, encoding:str=None, do_print:bool=None) -> Any:
         """Read the contents of a file.
         
         Parameters:
         - `file_path` (str): The path to the file to read.
         - `create` (bool): Whether to create the file if it does not exist. Default is `False`
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/file_dir_scripts/remove_file_dir.py` & `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/remove_file_dir.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from py_basic_commands.other.basic_commands     import try_traceback
 from py_basic_commands.file_dir_scripts   import read_file
-from dataclasses    import dataclass
 from py_basic_commands.fscripts   import fprint
-from shutil     import rmtree
 from py_basic_commands.base   import Base
+from dataclasses    import dataclass
+from shutil     import rmtree
 from os     import listdir, remove
 
 
 @dataclass
 class RemoveFileDir(Base):
     _force:bool = True
 
     def __post_init__(self):
         super().__init__()
 
-    
-    def config(self, **kwargs):
-        """Configure `remove_file_dir` variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'force':
-                self._force = value
 
     @try_traceback(print_traceback=True)
     def __call__(self, do:str, do_path:str, force:bool=False, do_print:bool=True) -> bool:
         """Remove a file or directory at the specified path.
         
         Parameters:
         - `do` (str): Whether to remove a `'d'`irectory or a `'f'`ile.
@@ -37,16 +29,14 @@
         - `bool`: Whether the file or directory was removed.
         """
 
         # Check input values
         force    = self._check_input_val(force, self._force)
         do_print = self._check_input_val(do_print, self._do_print)
 
-        fprint.config(do_print=do_print)
-
         if do == 'd': # Directory
             try:
                 dir_content = listdir(do_path)
             except FileNotFoundError:
                 fprint(f'Directory path not found: {do_path}')
                 return False
             except NotADirectoryError:
@@ -66,17 +56,35 @@
                 return False
 
         elif do == 'f': # File
             lines = read_file(do_path)
             if lines and not force:
                 fprint(f'File is not empty, not removing: {do_path}')
                 return False
-            remove(do_path)
+            try:
+                remove(do_path)
+            except FileNotFoundError:
+                fprint(f'File path not found: {do_path}')
+                return False
+            except IsADirectoryError:
+                fprint(f'Path is a directory: {do_path}')
+                return False
+            except PermissionError:
+                fprint(f'Permission denied: {do_path}')
+                return False
+            except OSError:
+                fprint(f'File is being used by another process: {do_path}')
+                return False
+            except Exception as err:
+                fprint(f'Error removing file: {do_path}')
+                raise err
+
             fprint(f'File removed: {do_path}')
             return True
 
 
 remove_file_dir = RemoveFileDir()
 
 if __name__ == '__main__':
     # Test code
-    remove_file_dir('d', 'Test folder', force=True)
+    remove_file_dir.config(do_print=False)
+    remove_file_dir('d', 'Test folder', force=True, do_print=False)
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/fscripts/finput.py` & `py_basic_commands-0.2.20/py_basic_commands/fscripts/finput.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,29 +10,14 @@
     _use_suffix:bool = True
     _ret_type:type = str
 
     def __post_init__(self):
         super().__init__()
 
 
-    def config(self, **kwargs):
-        """Configure `finput` values"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'text':
-                self._text = value
-            elif key == 'nl':
-                self._nl = value
-            elif key == 'use_suffix':
-                self._use_suffix = value
-            elif key == 'ret_type':
-                self._ret_type = value
-
-
     def __call__(self, text:str=None, ret_type:type=None, nl:bool=None, use_suffix:bool=None):
         """Get input from the user and return it as a specified type.
         
         Parameters:
         - `text` (str): The text to prompt the user with. Default is an `'Input: '`.
         - `ret_type` (type): The type to return the input as. Default is `str`.
         - `nl` (bool): Whether to append a newline character after the input. Default is `True`.
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/fscripts/fprint.py` & `py_basic_commands-0.2.20/py_basic_commands/fscripts/fprint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,38 @@
 from dataclasses    import dataclass
 from typing     import Any
 from py_basic_commands.base   import Base
 
 @dataclass
 class Fprint(Base):
-    _nl:bool = True
-    _flush:bool = False
-    _end = None
+    nl:bool = True
+    flush:bool = False
+    end = None
 
     def __post_init__(self):
         super().__init__()
 
 
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'nl':
-                self._nl = value
-            elif key == 'flush':
-                self._flush = value
-            elif key == 'end':
-                self._end = value
-
-
     def __call__(self, *args:Any, nl:bool=None, flush:bool=None, do_print:bool=None, end:str=None) -> None:
         """Print one or more objects to the console, with optional newline, flushing, and ending characters.
         
         Parameters:
         - `args` (*Any): One or more objects to print.
         - `nl` (bool): Whether to append a newline character to the output.
         - `flush` (bool): Whether to flush the output buffer.
         - `do_print` (bool): Whether to actually print the output.
         - `end` (str): The string to print at the end of the output.
         """
         # TODO: Add `sep` input parameter (separator between objects to print)
 
         # Check input values
-        nl = self._check_input_val(nl, self._nl) 
-        flush = self._check_input_val(flush, self._flush)
-        do_print = self._check_input_val(do_print, self._do_print)
-        end = self._check_input_val(end, self._end)
+        nl = self._check_input_val(nl, self.nl) 
+        flush = self._check_input_val(flush, self.flush)
+        do_print = self._check_input_val(do_print, self.do_print)
+        end = self._check_input_val(end, self.end)
         if not args:
             args = ('\n')
 
         if not do_print:
             return
 
         for arg_indx, arg in enumerate(args):
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/fscripts/fprint_array.py` & `py_basic_commands-0.2.20/py_basic_commands/fscripts/fprint_array.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,30 +13,14 @@
     _start_num:int=0
     _nl:bool=True
 
     def __post_init__(self):
         super().__init__()
 
 
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'header':
-                self._header = value
-            elif key == 'indx_brackets':
-                self._indx_brackets = value
-            elif key == 'print_num':
-                self._print_num = value
-            elif key == 'start_num':
-                self._start_num = value
-            elif key == 'nl':
-                self._nl = value
-
     def __call__(self, arr, header:str=None, indx_brackets:str=None, print_num=None, start_num:int=None, nl:bool=None) -> None:
         """This function prints the elements of an array along with their index numbers.
 
         Parameters:
         - `arr` (`list`|`set`|`tuple`|`dict`): The input array whose elements are to be printed.
         - `header` (str):  The header message to be printed before the array elements. Defaults is ''.
         - `indx_brackets` (str): The type of brackets to be used for index numbers. Defaults is '`[]`'.
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/json_scripts/create_json.py` & `py_basic_commands-0.2.20/py_basic_commands/json_scripts/create_json.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,23 +11,14 @@
 class CreateJson(Base):
     _force:bool = True
 
     def __post_init__(self):
         super().__init__()
 
 
-    def config(self, **kwargs):
-        """Configure `create_json` variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'force':
-                self._force = value
-
-
     def __call__(self, file_path:str, force:bool=None, do_print:bool=None) -> bool:
         """Create a new empty JSON file.
         
         Parameters:
         - `file_path` (str): The path for the new JSON file.
         - `force` (bool): Whether to overwrite any existing file with the same name. Default is `True`.
         - `do_print` (bool): Whether to print information about the file creation process. Default is `True`.
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/json_scripts/read_json.py` & `py_basic_commands-0.2.20/py_basic_commands/json_scripts/read_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import json
-from dataclasses    import dataclass
-from traceback  import format_exc
+
 from py_basic_commands.fscripts   import fprint
 from py_basic_commands.base   import Base
+from dataclasses    import dataclass
+from traceback  import format_exc
+from typing     import Any
 
 
 @dataclass
 class ReadJson(Base):
     def __post_init__(self):
         super().__init__()
 
 
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-
-    def __call__(self, file_path:str, do_print:bool=None):
+    def __call__(self, file_path:str, do_print:bool=None) -> Any:
         """Read data from a JSON file.
         
         Parameters:
         - `file_path` (str): The path of the JSON file to read from.
         - `do_print` (bool): Whether to get feedback printed to terminal or not. Default is `True`.
         
         Returns:
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/json_scripts/write_json.py` & `py_basic_commands-0.2.20/py_basic_commands/json_scripts/write_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,17 @@
 @dataclass
 class WriteJson(Base):
     _indent:bool = True
     _force:bool = False
 
     def __post_init__(self):
         super().__init__()
-
-
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'indent':
-                self._indent = value
-            elif key == 'force':
-                self._force = value
                 
 
-    def __call__(self, data:Any, file_path:str, indent:int=None, force:bool=None, do_print:bool=None) -> bool:
+    def __call__(self, data:Any, file_path:str, force:bool=None, indent:int=None, do_print:bool=None) -> bool:
         """Write data to a JSON file.
         
         Parameters:
         - `data` (Any): The data to write to the JSON file. This can be a dictionary, list, or a string representation of JSON.
         - `file_path` (str): The path of the JSON file to write to.
         - `indent` (int): The number of spaces to use for indentation in the JSON file. Default is `4`.
         - `force` (bool): Whether to overwrite any existing data in the JSON file. Default is `False`.
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/other/basic_commands.py` & `py_basic_commands-0.2.20/py_basic_commands/other/basic_commands.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.1/py_basic_commands/other/choose_from_list.py` & `py_basic_commands-0.2.20/py_basic_commands/other/choose_from_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,33 +14,14 @@
     _choose_until_correct:bool = True
 
 
     def __post_init__(self):
         super().__init__()
 
 
-    def config(self, **kwargs):
-        """Configure variables"""
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'header_text':
-                self._header_text = value
-            elif key == 'header_nl':
-                self._header_nl = value
-            elif key == 'input_text':
-                self._input_text = value
-            elif key == 'choose_total':
-                self._choose_total = value
-            elif key == 'start_num':
-                self._start_num = value
-            elif key == 'choose_until_correct':
-                self._choose_until_correct = value
-
-
     def __call__(self, _array:Any, header_text:str=None, header_nl:bool=None, input_text:str=None, choose_total:int=None, start_num:int=None, choose_until_correct:bool=None) -> list:
         """Prompt the user to choose one or more values from a list.
         
         Parameters:
         - `_array` (Any): The list of values to choose from.
         - `header_text` (str): The text to display as a header. Default is `''`
         - `header_nl` (bool): Whether to append a newline character after the header. Default is `False`
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/other/function_timer.py` & `py_basic_commands-0.2.20/py_basic_commands/other/function_timer.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,25 +10,14 @@
     _ret_time:bool = False
     _skip_intro:bool = True
     _skip_inputs:bool = True    
     
     def __post_init__(self) -> None:
         super().__init__()
 
-    def config(self, **kwargs):
-        self._config(**kwargs)
-
-        for key, value in kwargs.items():
-            if key == 'ret_time':
-                self._ret_time = value
-            elif key == 'skip_intro':
-                self._skip_intro = value
-            elif key == 'skip_inputs':
-                self._skip_inputs = value
-
 
     # TODO: Add self.do_print to function
     def _func_timer(self, do_print:bool=True, ret_time:bool=False, skip_intro:bool=True, skip_inputs:bool=True):
         def timer(func):
             @wraps(func)
             def wrapper(*args, **kwargs):
                 fprint(f'Function timer started: {self._get_func_name(func)}', do_print=not skip_intro and do_print)
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands/other/timer.py` & `py_basic_commands-0.2.20/py_basic_commands/other/timer.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.1/py_basic_commands.egg-info/PKG-INFO` & `py_basic_commands-0.2.20/py_basic_commands.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-basic-commands
-Version: 0.2.1
+Version: 0.2.20
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.1/py_basic_commands.egg-info/SOURCES.txt` & `py_basic_commands-0.2.20/py_basic_commands.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.1/pyproject.toml` & `py_basic_commands-0.2.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_basic_commands"
-version = "0.2.01"
+version = "0.2.20"
 authors = [
   { name="Rasmus Ohert", email="rassemichael@gmail.com" },
 ]
 description = "Basic tools for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py_basic_commands-0.2.1/setup.cfg` & `py_basic_commands-0.2.20/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py_basic_commands
-version = 0.2.01
+version = 0.2.20
 author = Rasmus Ohert
 author_email = rassemichael@gmail.com
 description = Basic tools for Python
 long_description = A package that has some basic tools for your basic Python needs
 url = https://github.com/RasseTheBoy/Py_Basic_Commands
 keywords = python, tool, help
 classifiers =
```

