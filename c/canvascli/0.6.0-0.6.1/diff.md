# Comparing `tmp/canvascli-0.6.0.tar.gz` & `tmp/canvascli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvascli-0.6.0.tar", last modified: Wed May  3 19:01:14 2023, max compression
+gzip compressed data, was "canvascli-0.6.1.tar", last modified: Sat May  6 00:30:24 2023, max compression
```

## Comparing `canvascli-0.6.0.tar` & `canvascli-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-03 19:01:14.015461 canvascli-0.6.0/
--rw-rw-r--   0 joel      (1000) joel      (1000)     1069 2021-06-02 17:43:36.000000 canvascli-0.6.0/LICENSE
--rw-rw-r--   0 joel      (1000) joel      (1000)       52 2022-02-28 07:42:04.000000 canvascli-0.6.0/MANIFEST.in
--rw-rw-r--   0 joel      (1000) joel      (1000)     4005 2023-05-03 19:01:14.015461 canvascli-0.6.0/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     3700 2023-04-09 23:39:09.000000 canvascli-0.6.0/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-03 19:01:14.015461 canvascli-0.6.0/canvascli/
--rw-rw-r--   0 joel      (1000) joel      (1000)       72 2022-03-02 16:22:02.000000 canvascli-0.6.0/canvascli/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      497 2023-05-03 19:01:14.015461 canvascli-0.6.0/canvascli/_version.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    61599 2023-04-24 15:51:31.000000 canvascli-0.6.0/canvascli/main.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-03 19:01:14.015461 canvascli-0.6.0/canvascli.egg-info/
--rw-rw-r--   0 joel      (1000) joel      (1000)     4005 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      324 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)       49 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/entry_points.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      144 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/requires.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)       10 2023-05-03 19:01:14.000000 canvascli-0.6.0/canvascli.egg-info/top_level.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      197 2023-05-03 19:01:14.015461 canvascli-0.6.0/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)      979 2023-04-12 21:40:16.000000 canvascli-0.6.0/setup.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    80044 2022-02-28 07:42:04.000000 canvascli-0.6.0/versioneer.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-06 00:30:24.716419 canvascli-0.6.1/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1069 2021-06-02 17:43:36.000000 canvascli-0.6.1/LICENSE
+-rw-rw-r--   0 joel      (1000) joel      (1000)       52 2022-02-28 07:42:04.000000 canvascli-0.6.1/MANIFEST.in
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4005 2023-05-06 00:30:24.716419 canvascli-0.6.1/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3700 2023-04-09 23:39:09.000000 canvascli-0.6.1/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-06 00:30:24.716419 canvascli-0.6.1/canvascli/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       72 2022-03-02 16:22:02.000000 canvascli-0.6.1/canvascli/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      497 2023-05-06 00:30:24.716419 canvascli-0.6.1/canvascli/_version.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    61592 2023-05-06 00:20:57.000000 canvascli-0.6.1/canvascli/main.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-06 00:30:24.716419 canvascli-0.6.1/canvascli.egg-info/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4005 2023-05-06 00:30:24.000000 canvascli-0.6.1/canvascli.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)      324 2023-05-06 00:30:24.000000 canvascli-0.6.1/canvascli.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-05-06 00:30:24.000000 canvascli-0.6.1/canvascli.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)       49 2023-05-06 00:30:24.000000 canvascli-0.6.1/canvascli.egg-info/entry_points.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      144 2023-05-06 00:30:24.000000 canvascli-0.6.1/canvascli.egg-info/requires.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)       10 2023-05-06 00:30:24.000000 canvascli-0.6.1/canvascli.egg-info/top_level.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      197 2023-05-06 00:30:24.716419 canvascli-0.6.1/setup.cfg
+-rw-rw-r--   0 joel      (1000) joel      (1000)      979 2023-04-12 21:40:16.000000 canvascli-0.6.1/setup.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    80044 2022-02-28 07:42:04.000000 canvascli-0.6.1/versioneer.py
```

### Comparing `canvascli-0.6.0/LICENSE` & `canvascli-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canvascli-0.6.0/PKG-INFO` & `canvascli-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvascli
-Version: 0.6.0
+Version: 0.6.1
 Summary: A CLI to reformat and review Canvas grades
 Home-page: https://github.com/joelostblom/canvascli
 Author: Joel Ostblom
 Author-email: joelostblom@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `canvascli-0.6.0/README.md` & `canvascli-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `canvascli-0.6.0/canvascli/main.py` & `canvascli-0.6.1/canvascli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
             desc='Downloading student grades',
             bar_format='{desc}... {n}{unit}'
         )
         for enrollment in enrollments_progress_bar:
             canvas_grades['User ID'].append(enrollment.user['id'])
 
             # `sis_user_id` is removed from concluded courses by Canvas
-            if hasattr(enrollment.user, 'sis_user_id'):
+            if 'sis_user_id' in enrollment.user:
                 canvas_grades['Student Number'].append(enrollment.user['sis_user_id'])
             else:
                 # A warning about this case is emitted further down
                 canvas_grades['Student Number'].append('N/A')
             surname, preferred_name = enrollment.user['sortable_name'].split(', ')
             canvas_grades['Surname'].append(surname)
             canvas_grades['Preferred Name'].append(preferred_name)
```

### Comparing `canvascli-0.6.0/canvascli.egg-info/PKG-INFO` & `canvascli-0.6.1/canvascli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvascli
-Version: 0.6.0
+Version: 0.6.1
 Summary: A CLI to reformat and review Canvas grades
 Home-page: https://github.com/joelostblom/canvascli
 Author: Joel Ostblom
 Author-email: joelostblom@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `canvascli-0.6.0/setup.py` & `canvascli-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `canvascli-0.6.0/versioneer.py` & `canvascli-0.6.1/versioneer.py`

 * *Files identical despite different names*

