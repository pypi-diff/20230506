# Comparing `tmp/jaaql-monitor-1.2.42.tar.gz` & `tmp/jaaql-monitor-1.2.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.42.tar", last modified: Sat May  6 11:31:55 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.43.tar", last modified: Sat May  6 11:32:59 2023, max compression
```

## Comparing `jaaql-monitor-1.2.42.tar` & `jaaql-monitor-1.2.43.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:31:55.990230 jaaql-monitor-1.2.42/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.42/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:31:55.990230 jaaql-monitor-1.2.42/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.42/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:31:55.986232 jaaql-monitor-1.2.42/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:31:55.000000 jaaql-monitor-1.2.42/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-06 11:31:55.000000 jaaql-monitor-1.2.42/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:31:55.000000 jaaql-monitor-1.2.42/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 11:31:55.000000 jaaql-monitor-1.2.42/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 11:31:55.000000 jaaql-monitor-1.2.42/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 11:31:55.989238 jaaql-monitor-1.2.42/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.42/monitor/__init__.py
--rw-rw-rw-   0        0        0    25584 2023-05-06 11:31:45.000000 jaaql-monitor-1.2.42/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-06 11:31:46.000000 jaaql-monitor-1.2.42/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-06 11:31:55.990230 jaaql-monitor-1.2.42/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:32:59.591781 jaaql-monitor-1.2.43/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.43/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:32:59.590781 jaaql-monitor-1.2.43/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.43/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:32:59.587781 jaaql-monitor-1.2.43/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:32:59.000000 jaaql-monitor-1.2.43/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-06 11:32:59.000000 jaaql-monitor-1.2.43/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:32:59.000000 jaaql-monitor-1.2.43/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 11:32:59.000000 jaaql-monitor-1.2.43/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 11:32:59.000000 jaaql-monitor-1.2.43/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:32:59.589781 jaaql-monitor-1.2.43/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.43/monitor/__init__.py
+-rw-rw-rw-   0        0        0    25587 2023-05-06 11:32:45.000000 jaaql-monitor-1.2.43/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-06 11:32:49.000000 jaaql-monitor-1.2.43/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:32:59.591781 jaaql-monitor-1.2.43/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.43/setup.py
```

### Comparing `jaaql-monitor-1.2.42/LICENSE.txt` & `jaaql-monitor-1.2.43/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.42/PKG-INFO` & `jaaql-monitor-1.2.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.42
+Version: 1.2.43
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.42/README.md` & `jaaql-monitor-1.2.43/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.42/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.43/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.42
+Version: 1.2.43
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.42/monitor/main.py` & `jaaql-monitor-1.2.43/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
         state.cur_file_line = line_err_num
         buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
         start_line_num = max(0, line_err_num - 10) + 1
         end_line_num = min(line_err_num + 3, len(buffer_lines)) + 1
         buffer_lines = buffer_lines[start_line_num - 1:end_line_num - 1]
 
         marker_line = marker_lines[0]
-        marker_line = marker_line[lines_with_line_number.index(":"):]
+        marker_line = marker_line[lines_with_line_number[0].index(":"):]
         marker_line = "      " + marker_line
 
         buffer_lines = [str(start_line_num + idx).rjust(5, '0') + "> " +
                         (line + "\n" + marker_line if start_line_num + idx == line_err_num else line)
                         for idx, line in zip(range(len(buffer_lines)), buffer_lines)]
         print_buffer = "\n".join(buffer_lines) + "\n\n\n" + print_buffer
         additional_line_message = "query "
```

### Comparing `jaaql-monitor-1.2.42/setup.py` & `jaaql-monitor-1.2.43/setup.py`

 * *Files identical despite different names*

