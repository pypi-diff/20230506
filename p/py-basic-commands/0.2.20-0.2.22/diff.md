# Comparing `tmp/py_basic_commands-0.2.20.tar.gz` & `tmp/py_basic_commands-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_basic_commands-0.2.20.tar", last modified: Sat May  6 00:56:43 2023, max compression
+gzip compressed data, was "py_basic_commands-0.2.22.tar", last modified: Sat May  6 01:15:31 2023, max compression
```

## Comparing `py_basic_commands-0.2.20.tar` & `py_basic_commands-0.2.22.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.127602 py_basic_commands-0.2.20/py_basic_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/example_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.127602 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/create_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/create_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/get_src_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/join_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/remove_file_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/write_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/py_basic_commands/fscripts/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/fscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/fscripts/finput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/fscripts/fprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/fscripts/fprint_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/py_basic_commands/json_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/json_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/json_scripts/create_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/json_scripts/read_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/json_scripts/write_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/py_basic_commands/other/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/basic_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/choose_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/function_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/py_basic_commands/other/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:56:43.127602 py_basic_commands-0.2.20/py_basic_commands.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 00:56:43.000000 py_basic_commands-0.2.20/py_basic_commands.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-06 00:56:43.000000 py_basic_commands-0.2.20/py_basic_commands.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:56:43.000000 py_basic_commands-0.2.20/py_basic_commands.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 00:56:43.000000 py_basic_commands-0.2.20/py_basic_commands.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-06 00:56:29.000000 py_basic_commands-0.2.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-06 00:56:43.131602 py_basic_commands-0.2.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.703888 py_basic_commands-0.2.22/py_basic_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/example_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/create_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/get_src_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/join_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/remove_file_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/write_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/py_basic_commands/fscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/fscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/fscripts/finput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/fscripts/fprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/fscripts/fprint_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/py_basic_commands/json_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/json_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/json_scripts/create_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/json_scripts/read_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/json_scripts/write_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/py_basic_commands/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/basic_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/choose_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/function_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/py_basic_commands/other/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:15:31.703888 py_basic_commands-0.2.22/py_basic_commands.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 01:15:31.000000 py_basic_commands-0.2.22/py_basic_commands.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-06 01:15:31.000000 py_basic_commands-0.2.22/py_basic_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:15:31.000000 py_basic_commands-0.2.22/py_basic_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 01:15:31.000000 py_basic_commands-0.2.22/py_basic_commands.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-06 01:15:20.000000 py_basic_commands-0.2.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-06 01:15:31.707888 py_basic_commands-0.2.22/setup.cfg
```

### Comparing `py_basic_commands-0.2.20/LICENSE.md` & `py_basic_commands-0.2.22/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/PKG-INFO` & `py_basic_commands-0.2.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_basic_commands
-Version: 0.2.20
+Version: 0.2.22
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.20/README.md` & `py_basic_commands-0.2.22/README.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/__init__.py` & `py_basic_commands-0.2.22/py_basic_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/base.py` & `py_basic_commands-0.2.22/py_basic_commands/base.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/__init__.py` & `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/create_dirs.py` & `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/create_dirs.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             - `dst_path` (str): Destination path; can include the file name at the end.
             - `do_print` (bool): Whether to print or not. Default is `True`
             
             Returns:
             - `bool`: If all directories were created or not"""
 
             # Check input values
-            do_print = self._check_input_val(do_print, self._do_print)
+            do_print = self._check_input_val(do_print, self.do_print)
 
             fprint.config(do_print=do_print)
 
             if dst_path == '':
                 return False
 
             dir_path = get_src_path(dst_path, ret_val='d', do_print=do_print)
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/create_file.py` & `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/create_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         if dst_path == '':
             fprint('No path specified')
             return False
 
         # Check input values
         force = self._check_input_val(force, self._force)
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         # Check if file already exists
         create_dirs(dst_path, do_print=do_print)
 
         if exists(dst_path):
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/get_src_path.py` & `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/get_src_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         if not src_path:
             fprint('No source path given')
             return None
 
         # Check input values
         ret_val = self._check_input_val(ret_val, self._ret_val)
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         root, ext = splitext(src_path)
         if not ext:
             dir_path = root
             fnam = ''
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/join_path.py` & `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/join_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             """Split a string and then join it back together"""
             return join_with.join(var.split(split_with))
         
         # Check input values
         join_with = self._check_input_val(join_with, self._join_with)
         remove_empty = self._check_input_val(remove_empty, self._remove_empty)
         dir_end = self._check_input_val(dir_end, self._dir_end)
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         # Iterate through args and join them together
         new_args = []
         for arg_indx, arg in enumerate(args):
             # Remove invalid characters
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/read_file.py` & `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/read_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         create      = self._check_input_val(create, self._create)
         ret_did_create = self._check_input_val(ret_did_create, self._ret_did_create)
         splitlines  = self._check_input_val(splitlines, self._splitlines)
         remove_empty = self._check_input_val(remove_empty, self._remove_empty)
         do_strip    = self._check_input_val(do_strip, self._do_strip)
         do_lower    = self._check_input_val(do_lower, self._do_lower)
         encoding    = self._check_input_val(encoding, self._encoding)
-        do_print    = self._check_input_val(do_print, self._do_print)
+        do_print    = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         lines, did_create = try_reading()
 
         # Return the file contents
         if ret_did_create:
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/remove_file_dir.py` & `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/remove_file_dir.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         
         Returns:
         - `bool`: Whether the file or directory was removed.
         """
 
         # Check input values
         force    = self._check_input_val(force, self._force)
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         if do == 'd': # Directory
             try:
                 dir_content = listdir(do_path)
             except FileNotFoundError:
                 fprint(f'Directory path not found: {do_path}')
                 return False
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/file_dir_scripts/write_file.py` & `py_basic_commands-0.2.22/py_basic_commands/file_dir_scripts/write_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         """
 
         # Check input values
         append = self._check_input_val(append, self._append)
         force_create = self._check_input_val(force_create, self._force_create)
         remove_duplicates = self._check_input_val(remove_duplicates, self._remove_duplicates)
         encoding = self._check_input_val(encoding, self._encoding)
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         if text.__class__.__name__ == 'ndarray':
             text = text.tolist()
         
         if text.__class__.__name__ in ('list', 'tuple', 'set'):
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/fscripts/finput.py` & `py_basic_commands-0.2.22/py_basic_commands/fscripts/finput.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/fscripts/fprint.py` & `py_basic_commands-0.2.22/py_basic_commands/fscripts/fprint.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/fscripts/fprint_array.py` & `py_basic_commands-0.2.22/py_basic_commands/fscripts/fprint_array.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/json_scripts/create_json.py` & `py_basic_commands-0.2.22/py_basic_commands/json_scripts/create_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         
         Returns:
         - `bool`: Whether the file was created.
         """
 
         # Check input values
         force = self._check_input_val(force, self._force)
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         write_empty_json = lambda: open(file_path, 'w').write(json.dumps({}, indent=4))
 
         did_create = create_file(file_path, force=force, do_print=do_print)
         if did_create:
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/json_scripts/read_json.py` & `py_basic_commands-0.2.22/py_basic_commands/json_scripts/read_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         - `do_print` (bool): Whether to get feedback printed to terminal or not. Default is `True`.
         
         Returns:
         - `Any`: The data from the JSON file, as a dictionary or list.
         """
 
         # Check input values
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         try:
             with open(file_path, 'r') as f:
                 file_data = json.load(f)
             return file_data
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/json_scripts/write_json.py` & `py_basic_commands-0.2.22/py_basic_commands/json_scripts/write_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         Return:
         - `bool`: Whether the file was created.
         """
 
         # Check input values
         indent = self._check_input_val(indent, self._indent)
         force = self._check_input_val(force, self._force)
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         fprint.config(do_print=do_print)
 
         try:
             if data.__class__.__name__ == ('str'):
                 data = json.loads(data)
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/other/basic_commands.py` & `py_basic_commands-0.2.22/py_basic_commands/other/basic_commands.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/other/choose_from_list.py` & `py_basic_commands-0.2.22/py_basic_commands/other/choose_from_list.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/py_basic_commands/other/function_timer.py` & `py_basic_commands-0.2.22/py_basic_commands/other/function_timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
                 if ret_time:
                     return ret_val, time_delta
                 return ret_val
             return wrapper
         
         # Check input values
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
         ret_time = self._check_input_val(ret_time, self._ret_time)
         skip_intro = self._check_input_val(skip_intro, self._skip_intro)
         skip_inputs = self._check_input_val(skip_inputs, self._skip_inputs)
 
         return timer
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands/other/timer.py` & `py_basic_commands-0.2.22/py_basic_commands/other/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.timer_lst:dict[str,float] = {}
 
 
     def start_timer(self, timer_name:str, do_print:bool=True) -> bool:
         """Start a timer with a specified name"""
 
         # Chek values
-        do_print = self._check_input_val(do_print, self._do_print)
+        do_print = self._check_input_val(do_print, self.do_print)
 
         if self.timer_lst.get(timer_name):
             print(f'Timer with name already started: {timer_name}')
             return False
 
         self.timer_lst[timer_name] = perf_counter()
         fprint(f'Timer started: {timer_name}', do_print=do_print)
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands.egg-info/PKG-INFO` & `py_basic_commands-0.2.22/py_basic_commands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-basic-commands
-Version: 0.2.20
+Version: 0.2.22
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.20/py_basic_commands.egg-info/SOURCES.txt` & `py_basic_commands-0.2.22/py_basic_commands.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.20/pyproject.toml` & `py_basic_commands-0.2.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_basic_commands"
-version = "0.2.20"
+version = "0.2.22"
 authors = [
   { name="Rasmus Ohert", email="rassemichael@gmail.com" },
 ]
 description = "Basic tools for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py_basic_commands-0.2.20/setup.cfg` & `py_basic_commands-0.2.22/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py_basic_commands
-version = 0.2.20
+version = 0.2.22
 author = Rasmus Ohert
 author_email = rassemichael@gmail.com
 description = Basic tools for Python
 long_description = A package that has some basic tools for your basic Python needs
 url = https://github.com/RasseTheBoy/Py_Basic_Commands
 keywords = python, tool, help
 classifiers =
```

