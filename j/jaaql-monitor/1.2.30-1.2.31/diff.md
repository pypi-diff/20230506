# Comparing `tmp/jaaql-monitor-1.2.30.tar.gz` & `tmp/jaaql-monitor-1.2.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.30.tar", last modified: Fri May  5 11:32:31 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.31.tar", last modified: Sat May  6 10:57:00 2023, max compression
```

## Comparing `jaaql-monitor-1.2.30.tar` & `jaaql-monitor-1.2.31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:32:31.816358 jaaql-monitor-1.2.30/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.30/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-05 11:32:31.815358 jaaql-monitor-1.2.30/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.30/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 11:32:31.812362 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 11:32:31.000000 jaaql-monitor-1.2.30/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 11:32:31.815358 jaaql-monitor-1.2.30/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.30/monitor/__init__.py
--rw-rw-rw-   0        0        0    23822 2023-05-05 11:32:21.000000 jaaql-monitor-1.2.30/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-05 11:32:22.000000 jaaql-monitor-1.2.30/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-05 11:32:31.816358 jaaql-monitor-1.2.30/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:57:00.895034 jaaql-monitor-1.2.31/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.31/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-06 10:57:00.895034 jaaql-monitor-1.2.31/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.31/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 10:57:00.889021 jaaql-monitor-1.2.31/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-06 10:57:00.000000 jaaql-monitor-1.2.31/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-06 10:57:00.000000 jaaql-monitor-1.2.31/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 10:57:00.000000 jaaql-monitor-1.2.31/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 10:57:00.000000 jaaql-monitor-1.2.31/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 10:57:00.000000 jaaql-monitor-1.2.31/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 10:57:00.893461 jaaql-monitor-1.2.31/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.31/monitor/__init__.py
+-rw-rw-rw-   0        0        0    25011 2023-05-06 10:56:34.000000 jaaql-monitor-1.2.31/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-06 10:56:36.000000 jaaql-monitor-1.2.31/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 10:57:00.895997 jaaql-monitor-1.2.31/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.31/setup.py
```

### Comparing `jaaql-monitor-1.2.30/LICENSE.txt` & `jaaql-monitor-1.2.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.30/PKG-INFO` & `jaaql-monitor-1.2.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.30
+Version: 1.2.31
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.30/README.md` & `jaaql-monitor-1.2.31/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.30/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.31/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.30
+Version: 1.2.31
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.30/monitor/main.py` & `jaaql-monitor-1.2.31/monitor/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,18 @@
 
         self.log("Request took " + str(self.time_delta_ms(start_time, datetime.now())) + "ms")
 
         if res.status_code == 200:
             format_query_output(self, res.json())
         else:
             if handle_error:
-                print_error(self, res.text)
+                if endpoint == ENDPOINT__submit:
+                    print_submit_error(self, res.text)
+                else:
+                    print_error(self, res.text)
 
         return res
 
 
 def split_by_lines(split_str, gap=1):
     split_str = split_str.split("".join(["\r\n"] * gap))
     if len(split_str) == 1:
@@ -325,33 +328,56 @@
     return ConnectionInfo(jaaql_url, username, password, None, state.override_url)
 
 
 def dump_buffer(state, start: str = "\n\n"):
     return ("%sBuffer was length " % start) + str(len(state.fetched_query.strip())) + " with contents:\n" + state.fetched_query.strip() + "\n\n"
 
 
-def print_error(state, err, line_offset: int = 0):
+def get_message(state, err, line_offset, buffer):
     caller = getframeinfo(stack()[1][0])
     file_message = ""
     if state.file_name is not None:
         file_message = "Error on line %d of file '%s':\n\n" % (state.cur_file_line - line_offset, state.file_name)
     debug_message = " [%s:%d]" % (caller.filename, caller.lineno)
     if not state.is_script() or not state.is_debugging:
         debug_message = ""
-    buffer = "\n" + dump_buffer(state, "")
+    buffer = "\n" + buffer
     if not state.is_script():
         buffer = ""
+
     print(file_message + err + debug_message + buffer, file=sys.stderr)
     if state.is_script():
         if state.do_exit:
             exit(1)
         else:
             raise JAAQLMonitorException(file_message + err + debug_message + buffer)
 
 
+def submit_error(state, err, line_offset: int = 0):
+    divided_lines = [line for line in err.split("\n").trim() if line.startswith("LINE ")]
+
+    print_buffer = dump_buffer(state, "")
+    if len(divided_lines) != 0:
+        line_err_num = int(divided_lines[0].split("LINE ")[1].split(":")[0])
+        buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
+        start_line_num = max(0, line_err_num - 10) + 1
+        end_line_num = min(line_err_num, len(buffer_lines)) + 1
+        buffer_lines = buffer_lines[start_line_num - 1:end_line_num - 1]
+        buffer_lines = [str(start_line_num + idx) + "| " +
+                        ('<b><font color="red">' + line + '</font></b>' if start_line_num + idx == line_err_num else line)
+                        for idx, line in zip(range(len(buffer_lines)))]
+        print_buffer = "<i>\n".join(buffer_lines) + "</i>" + print_buffer
+
+    get_message(state, err, line_offset, print_buffer)
+
+
+def print_error(state, err, line_offset: int = 0):
+    get_message(state, err, line_offset, dump_buffer(state, ""))
+
+
 def wipe_jaaql_box(state: State):
     res = state.request_handler(METHOD__post, ENDPOINT__wipe, handle_error=False)
 
     if res.status_code != 200:
         print_error(state, "Error wiping jaaql box, received status code %d and message:\n\n\t%s" % (res.status_code, res.text))
```

### Comparing `jaaql-monitor-1.2.30/setup.py` & `jaaql-monitor-1.2.31/setup.py`

 * *Files identical despite different names*

