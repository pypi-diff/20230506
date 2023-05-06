# Comparing `tmp/jaaql-monitor-1.2.45.tar.gz` & `tmp/jaaql-monitor-1.2.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.45.tar", last modified: Sat May  6 11:37:01 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.46.tar", last modified: Sat May  6 11:44:17 2023, max compression
```

## Comparing `jaaql-monitor-1.2.45.tar` & `jaaql-monitor-1.2.46.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:37:01.260275 jaaql-monitor-1.2.45/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.45/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:37:01.260275 jaaql-monitor-1.2.45/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.45/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:37:01.256274 jaaql-monitor-1.2.45/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:37:01.000000 jaaql-monitor-1.2.45/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-06 11:37:01.000000 jaaql-monitor-1.2.45/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:37:01.000000 jaaql-monitor-1.2.45/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 11:37:01.000000 jaaql-monitor-1.2.45/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 11:37:01.000000 jaaql-monitor-1.2.45/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 11:37:01.259274 jaaql-monitor-1.2.45/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.45/monitor/__init__.py
--rw-rw-rw-   0        0        0    25614 2023-05-06 11:36:47.000000 jaaql-monitor-1.2.45/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-06 11:36:49.000000 jaaql-monitor-1.2.45/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-06 11:37:01.260275 jaaql-monitor-1.2.45/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:44:17.368219 jaaql-monitor-1.2.46/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.46/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:44:17.367219 jaaql-monitor-1.2.46/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.46/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:44:17.364189 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:44:17.366219 jaaql-monitor-1.2.46/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.46/monitor/__init__.py
+-rw-rw-rw-   0        0        0    25614 2023-05-06 11:44:06.000000 jaaql-monitor-1.2.46/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-06 11:44:08.000000 jaaql-monitor-1.2.46/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:44:17.368219 jaaql-monitor-1.2.46/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.46/setup.py
```

### Comparing `jaaql-monitor-1.2.45/LICENSE.txt` & `jaaql-monitor-1.2.46/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.45/PKG-INFO` & `jaaql-monitor-1.2.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.45
+Version: 1.2.46
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.45/README.md` & `jaaql-monitor-1.2.46/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.45/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.46/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.45
+Version: 1.2.46
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.45/monitor/main.py` & `jaaql-monitor-1.2.46/monitor/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -325,15 +325,15 @@
         username = input("Username: ").strip()
         password = getpass(prompt='Password: ', stream=None)
 
     return ConnectionInfo(jaaql_url, username, password, None, state.override_url)
 
 
 def dump_buffer(state, start: str = "\n\n"):
-    return ("%sBuffer[ " % start) + str(len(state.fetched_query.strip())) + "]: with contents:\n" + state.fetched_query.strip() + "\n\n"
+    return ("%sBuffer [" % start) + str(len(state.fetched_query.strip())) + "]:\n" + state.fetched_query.strip() + "\n\n"
 
 
 def get_message(state, err, line_offset, buffer, additional_line_message: str = ""):
     caller = getframeinfo(stack()[1][0])
     file_message = ""
     if state.file_name is not None:
         file_message = "Error on " + additional_line_message + "line %d of file '%s':\n\n" % (state.cur_file_line - line_offset, state.file_name)
@@ -353,15 +353,14 @@
 
 
 def submit_error(state, err, line_offset: int = 0):
     divided_lines = [line for line in [err_line.strip() for err_line in err.split("\n")]]
     lines_with_line_number = [line for line in divided_lines if line.startswith("LINE ")]
     marker_lines = [line for line in [err_line for err_line in err.split("\n")] if line.strip() == "^"]
 
-    additional_line_message = ""
     print_buffer = dump_buffer(state, "")
     if len(lines_with_line_number) != 0:
         line_err_num = int(lines_with_line_number[0].split("LINE ")[1].split(":")[0])
         state.cur_file_line = line_err_num
         buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
         start_line_num = max(0, line_err_num - 10) + 1
         end_line_num = min(line_err_num + 3, len(buffer_lines)) + 1
@@ -370,18 +369,21 @@
         marker_line = marker_lines[0]
         marker_line = marker_line[lines_with_line_number[0].index(":"):]
         marker_line = "     " + marker_line
 
         buffer_lines = [str(start_line_num + idx).rjust(5, '0') + "> " +
                         (line + "\n" + marker_line if start_line_num + idx == line_err_num else line)
                         for idx, line in zip(range(len(buffer_lines)), buffer_lines)]
-        additional_line_message = "query "
-        err = "\n".join(buffer_lines) + "\n" + "\n".join(err.replace("\r\n", "\n").split("\n")[:-2])
 
-    get_message(state, err, line_offset, print_buffer, additional_line_message)
+        print(err.replace("\r\n", "\n").split("\n"))
+
+        err = "\n".join(err.replace("\r\n", "\n").split("\n")[:-2])
+        err = err + "\n" + "\n".join(buffer_lines)
+        err = "\\<b\\>" + err + "\\<\\b\\>"
+    get_message(state, err, line_offset, print_buffer)
 
 
 def print_error(state, err, line_offset: int = 0):
     get_message(state, err, line_offset, dump_buffer(state, ""))
 
 
 def wipe_jaaql_box(state: State):
```

### Comparing `jaaql-monitor-1.2.45/setup.py` & `jaaql-monitor-1.2.46/setup.py`

 * *Files identical despite different names*

