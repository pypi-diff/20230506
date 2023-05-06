# Comparing `tmp/jaaql-monitor-1.2.46.tar.gz` & `tmp/jaaql-monitor-1.2.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.46.tar", last modified: Sat May  6 11:44:17 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.47.tar", last modified: Sat May  6 11:45:41 2023, max compression
```

## Comparing `jaaql-monitor-1.2.46.tar` & `jaaql-monitor-1.2.47.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:44:17.368219 jaaql-monitor-1.2.46/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.46/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:44:17.367219 jaaql-monitor-1.2.46/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.46/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:44:17.364189 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 11:44:17.000000 jaaql-monitor-1.2.46/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 11:44:17.366219 jaaql-monitor-1.2.46/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.46/monitor/__init__.py
--rw-rw-rw-   0        0        0    25614 2023-05-06 11:44:06.000000 jaaql-monitor-1.2.46/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-06 11:44:08.000000 jaaql-monitor-1.2.46/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-06 11:44:17.368219 jaaql-monitor-1.2.46/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.46/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:45:41.951510 jaaql-monitor-1.2.47/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.47/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:45:41.950511 jaaql-monitor-1.2.47/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.47/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:45:41.946513 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 11:45:41.000000 jaaql-monitor-1.2.47/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:45:41.949511 jaaql-monitor-1.2.47/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.47/monitor/__init__.py
+-rw-rw-rw-   0        0        0    25619 2023-05-06 11:45:27.000000 jaaql-monitor-1.2.47/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-06 11:45:31.000000 jaaql-monitor-1.2.47/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:45:41.951510 jaaql-monitor-1.2.47/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.47/setup.py
```

### Comparing `jaaql-monitor-1.2.46/LICENSE.txt` & `jaaql-monitor-1.2.47/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.46/PKG-INFO` & `jaaql-monitor-1.2.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.46
+Version: 1.2.47
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.46/README.md` & `jaaql-monitor-1.2.47/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.46/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.47/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.46
+Version: 1.2.47
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.46/monitor/main.py` & `jaaql-monitor-1.2.47/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         marker_line = marker_line[lines_with_line_number[0].index(":"):]
         marker_line = "     " + marker_line
 
         buffer_lines = [str(start_line_num + idx).rjust(5, '0') + "> " +
                         (line + "\n" + marker_line if start_line_num + idx == line_err_num else line)
                         for idx, line in zip(range(len(buffer_lines)), buffer_lines)]
 
-        print(err.replace("\r\n", "\n").split("\n"))
+        print(len(err.replace("\r\n", "\n").split("\n")))
 
         err = "\n".join(err.replace("\r\n", "\n").split("\n")[:-2])
         err = err + "\n" + "\n".join(buffer_lines)
         err = "\\<b\\>" + err + "\\<\\b\\>"
     get_message(state, err, line_offset, print_buffer)
```

### Comparing `jaaql-monitor-1.2.46/setup.py` & `jaaql-monitor-1.2.47/setup.py`

 * *Files identical despite different names*

