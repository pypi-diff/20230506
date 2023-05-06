# Comparing `tmp/jaaql-monitor-1.2.35.tar.gz` & `tmp/jaaql-monitor-1.2.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.35.tar", last modified: Sat May  6 11:05:29 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.36.tar", last modified: Sat May  6 11:08:38 2023, max compression
```

## Comparing `jaaql-monitor-1.2.35.tar` & `jaaql-monitor-1.2.36.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:05:29.271488 jaaql-monitor-1.2.35/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.35/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:05:29.271488 jaaql-monitor-1.2.35/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.35/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:05:29.267474 jaaql-monitor-1.2.35/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:05:29.000000 jaaql-monitor-1.2.35/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-06 11:05:29.000000 jaaql-monitor-1.2.35/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:05:29.000000 jaaql-monitor-1.2.35/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 11:05:29.000000 jaaql-monitor-1.2.35/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 11:05:29.000000 jaaql-monitor-1.2.35/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 11:05:29.270475 jaaql-monitor-1.2.35/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.35/monitor/__init__.py
--rw-rw-rw-   0        0        0    25058 2023-05-06 11:05:16.000000 jaaql-monitor-1.2.35/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-06 11:05:19.000000 jaaql-monitor-1.2.35/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-06 11:05:29.271488 jaaql-monitor-1.2.35/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:08:38.509005 jaaql-monitor-1.2.36/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.36/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:08:38.507986 jaaql-monitor-1.2.36/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.36/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:08:38.504985 jaaql-monitor-1.2.36/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:08:38.000000 jaaql-monitor-1.2.36/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-06 11:08:38.000000 jaaql-monitor-1.2.36/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:08:38.000000 jaaql-monitor-1.2.36/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 11:08:38.000000 jaaql-monitor-1.2.36/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 11:08:38.000000 jaaql-monitor-1.2.36/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:08:38.506985 jaaql-monitor-1.2.36/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.36/monitor/__init__.py
+-rw-rw-rw-   0        0        0    25004 2023-05-06 11:08:13.000000 jaaql-monitor-1.2.36/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-06 11:08:28.000000 jaaql-monitor-1.2.36/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:08:38.509005 jaaql-monitor-1.2.36/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.36/setup.py
```

### Comparing `jaaql-monitor-1.2.35/LICENSE.txt` & `jaaql-monitor-1.2.36/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.35/PKG-INFO` & `jaaql-monitor-1.2.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.35
+Version: 1.2.36
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.35/README.md` & `jaaql-monitor-1.2.36/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.35/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.36/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.35
+Version: 1.2.36
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.35/monitor/main.py` & `jaaql-monitor-1.2.36/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,17 +359,17 @@
     if len(divided_lines) != 0:
         line_err_num = int(divided_lines[0].split("LINE ")[1].split(":")[0])
         buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
         start_line_num = max(0, line_err_num - 10) + 1
         end_line_num = min(line_err_num, len(buffer_lines)) + 1
         buffer_lines = buffer_lines[start_line_num - 1:end_line_num - 1]
         buffer_lines = [str(start_line_num + idx) + "| " +
-                        ('<b><font color="red">' + line + '</font></b>' if start_line_num + idx == line_err_num else line)
+                        (line if start_line_num + idx == line_err_num else line)
                         for idx, line in zip(range(len(buffer_lines)), buffer_lines)]
-        print_buffer = "<i>" + "\n".join(buffer_lines) + "</i>\n\n\n" + print_buffer
+        print_buffer = "\n".join(buffer_lines) + "\n\n\n" + print_buffer
 
     get_message(state, err, line_offset, print_buffer)
 
 
 def print_error(state, err, line_offset: int = 0):
     get_message(state, err, line_offset, dump_buffer(state, ""))
```

### Comparing `jaaql-monitor-1.2.35/setup.py` & `jaaql-monitor-1.2.36/setup.py`

 * *Files identical despite different names*

