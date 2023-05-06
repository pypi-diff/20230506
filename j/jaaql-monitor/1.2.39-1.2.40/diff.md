# Comparing `tmp/jaaql-monitor-1.2.39.tar.gz` & `tmp/jaaql-monitor-1.2.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.39.tar", last modified: Sat May  6 11:27:21 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.40.tar", last modified: Sat May  6 11:28:18 2023, max compression
```

## Comparing `jaaql-monitor-1.2.39.tar` & `jaaql-monitor-1.2.40.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:27:21.041501 jaaql-monitor-1.2.39/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.39/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:27:21.040501 jaaql-monitor-1.2.39/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.39/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:27:21.037490 jaaql-monitor-1.2.39/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:27:20.000000 jaaql-monitor-1.2.39/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-06 11:27:20.000000 jaaql-monitor-1.2.39/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:27:20.000000 jaaql-monitor-1.2.39/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 11:27:20.000000 jaaql-monitor-1.2.39/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 11:27:20.000000 jaaql-monitor-1.2.39/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 11:27:21.039491 jaaql-monitor-1.2.39/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.39/monitor/__init__.py
--rw-rw-rw-   0        0        0    25572 2023-05-06 11:27:08.000000 jaaql-monitor-1.2.39/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-06 11:27:11.000000 jaaql-monitor-1.2.39/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-06 11:27:21.041501 jaaql-monitor-1.2.39/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.39/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:18.865212 jaaql-monitor-1.2.40/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.40/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:28:18.865212 jaaql-monitor-1.2.40/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.40/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:18.861214 jaaql-monitor-1.2.40/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:28:18.000000 jaaql-monitor-1.2.40/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-06 11:28:18.000000 jaaql-monitor-1.2.40/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:28:18.000000 jaaql-monitor-1.2.40/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 11:28:18.000000 jaaql-monitor-1.2.40/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 11:28:18.000000 jaaql-monitor-1.2.40/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:18.864212 jaaql-monitor-1.2.40/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.40/monitor/__init__.py
+-rw-rw-rw-   0        0        0    25581 2023-05-06 11:28:07.000000 jaaql-monitor-1.2.40/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-06 11:28:09.000000 jaaql-monitor-1.2.40/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:28:18.865212 jaaql-monitor-1.2.40/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.40/setup.py
```

### Comparing `jaaql-monitor-1.2.39/LICENSE.txt` & `jaaql-monitor-1.2.40/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.39/PKG-INFO` & `jaaql-monitor-1.2.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.39
+Version: 1.2.40
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.39/README.md` & `jaaql-monitor-1.2.40/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.39/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.40/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.39
+Version: 1.2.40
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.39/monitor/main.py` & `jaaql-monitor-1.2.40/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
     divided_lines = [line for line in [err_line.strip() for err_line in err.split("\n")]]
     lines_with_line_number = [line for line in divided_lines if line.startswith("LINE ")]
     marker_lines = [line for line in [err_line for err_line in err.split("\n")] if line.strip() == "^"]
 
     additional_line_message = ""
     print_buffer = dump_buffer(state, "")
     if len(lines_with_line_number) != 0:
-        line_err_num = int(divided_lines[0].split("LINE ")[1].split(":")[0])
+        line_err_num = int(lines_with_line_number[0].split("LINE ")[1].split(":")[0])
         state.cur_file_line = line_err_num
         buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
         start_line_num = max(0, line_err_num - 10) + 1
         end_line_num = min(line_err_num + 3, len(buffer_lines)) + 1
         buffer_lines = buffer_lines[start_line_num - 1:end_line_num - 1]
 
         marker_line = marker_lines[0]
```

### Comparing `jaaql-monitor-1.2.39/setup.py` & `jaaql-monitor-1.2.40/setup.py`

 * *Files identical despite different names*

