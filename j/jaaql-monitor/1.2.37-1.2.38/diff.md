# Comparing `tmp/jaaql-monitor-1.2.37.tar.gz` & `tmp/jaaql-monitor-1.2.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.37.tar", last modified: Sat May  6 11:10:13 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.38.tar", last modified: Sat May  6 11:19:35 2023, max compression
```

## Comparing `jaaql-monitor-1.2.37.tar` & `jaaql-monitor-1.2.38.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:10:13.886701 jaaql-monitor-1.2.37/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.37/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:10:13.886701 jaaql-monitor-1.2.37/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.37/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:10:13.882701 jaaql-monitor-1.2.37/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:10:13.000000 jaaql-monitor-1.2.37/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-06 11:10:13.000000 jaaql-monitor-1.2.37/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:10:13.000000 jaaql-monitor-1.2.37/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 11:10:13.000000 jaaql-monitor-1.2.37/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 11:10:13.000000 jaaql-monitor-1.2.37/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 11:10:13.885701 jaaql-monitor-1.2.37/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.37/monitor/__init__.py
--rw-rw-rw-   0        0        0    25007 2023-05-06 11:10:02.000000 jaaql-monitor-1.2.37/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-06 11:10:04.000000 jaaql-monitor-1.2.37/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-06 11:10:13.886701 jaaql-monitor-1.2.37/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.37/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:19:35.959348 jaaql-monitor-1.2.38/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.38/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:19:35.958354 jaaql-monitor-1.2.38/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.38/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:19:35.954360 jaaql-monitor-1.2.38/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:19:35.000000 jaaql-monitor-1.2.38/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-06 11:19:35.000000 jaaql-monitor-1.2.38/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:19:35.000000 jaaql-monitor-1.2.38/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 11:19:35.000000 jaaql-monitor-1.2.38/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 11:19:35.000000 jaaql-monitor-1.2.38/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:19:35.957372 jaaql-monitor-1.2.38/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.38/monitor/__init__.py
+-rw-rw-rw-   0        0        0    25432 2023-05-06 11:19:20.000000 jaaql-monitor-1.2.38/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-06 11:19:26.000000 jaaql-monitor-1.2.38/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:19:35.959348 jaaql-monitor-1.2.38/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.38/setup.py
```

### Comparing `jaaql-monitor-1.2.37/LICENSE.txt` & `jaaql-monitor-1.2.38/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.37/PKG-INFO` & `jaaql-monitor-1.2.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.37
+Version: 1.2.38
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.37/README.md` & `jaaql-monitor-1.2.38/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.37/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.38/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.37
+Version: 1.2.38
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.37/monitor/main.py` & `jaaql-monitor-1.2.38/monitor/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,19 +328,19 @@
     return ConnectionInfo(jaaql_url, username, password, None, state.override_url)
 
 
 def dump_buffer(state, start: str = "\n\n"):
     return ("%sBuffer was length " % start) + str(len(state.fetched_query.strip())) + " with contents:\n" + state.fetched_query.strip() + "\n\n"
 
 
-def get_message(state, err, line_offset, buffer):
+def get_message(state, err, line_offset, buffer, additional_line_message: str = ""):
     caller = getframeinfo(stack()[1][0])
     file_message = ""
     if state.file_name is not None:
-        file_message = "Error on line %d of file '%s':\n\n" % (state.cur_file_line - line_offset, state.file_name)
+        file_message = "Error on " + additional_line_message + "line %d of file '%s':\n\n" % (state.cur_file_line - line_offset, state.file_name)
     debug_message = " [%s:%d]" % (caller.filename, caller.lineno)
     if not state.is_script() or not state.is_debugging:
         debug_message = ""
     buffer = "\n" + buffer
     if not state.is_script():
         buffer = ""
 
@@ -349,29 +349,34 @@
         if state.do_exit:
             exit(1)
         else:
             raise JAAQLMonitorException(file_message + err + debug_message + buffer)
 
 
 def submit_error(state, err, line_offset: int = 0):
-    divided_lines = [line for line in [err_line.strip() for err_line in err.split("\n")] if line.startswith("LINE ")]
+    divided_lines = [line for line in [err_line.strip() for err_line in err.split("\n")]]
+    lines_with_line_number = [line for line in divided_lines if line.startswith("LINE ")]
+    marker_lines = [line for line in [err_line for err_line in err.split("\n")] if line.strip() == "^"]
 
+    additional_line_message = ""
     print_buffer = dump_buffer(state, "")
-    if len(divided_lines) != 0:
+    if len(lines_with_line_number) != 0:
         line_err_num = int(divided_lines[0].split("LINE ")[1].split(":")[0])
+        state.cur_file_line = line_err_num
         buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
-        start_line_num = max(0, line_err_num - 7) + 1
+        start_line_num = max(0, line_err_num - 10) + 1
         end_line_num = min(line_err_num + 3, len(buffer_lines)) + 1
         buffer_lines = buffer_lines[start_line_num - 1:end_line_num - 1]
-        buffer_lines = [str(start_line_num + idx) + "| " +
-                        (line if start_line_num + idx == line_err_num else line)
+        buffer_lines = [str(start_line_num + idx).rjust(5, '0') + "> " +
+                        (line + "\n" + marker_lines[0] if start_line_num + idx == line_err_num else line)
                         for idx, line in zip(range(len(buffer_lines)), buffer_lines)]
         print_buffer = "\n".join(buffer_lines) + "\n\n\n" + print_buffer
+        additional_line_message = "query "
 
-    get_message(state, err, line_offset, print_buffer)
+    get_message(state, err, line_offset, print_buffer, additional_line_message)
 
 
 def print_error(state, err, line_offset: int = 0):
     get_message(state, err, line_offset, dump_buffer(state, ""))
 
 
 def wipe_jaaql_box(state: State):
```

### Comparing `jaaql-monitor-1.2.37/setup.py` & `jaaql-monitor-1.2.38/setup.py`

 * *Files identical despite different names*

