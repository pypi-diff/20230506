# Comparing `tmp/amplify-sched-0.0.1.tar.gz` & `tmp/amplify-sched-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplify-sched-0.0.1.tar", last modified: Sat May  6 15:14:30 2023, max compression
+gzip compressed data, was "amplify-sched-0.0.1rc1.tar", last modified: Sat May  6 14:10:30 2023, max compression
```

## Comparing `amplify-sched-0.0.1.tar` & `amplify-sched-0.0.1rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:14:30.648428 amplify-sched-0.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-06 13:38:38.000000 amplify-sched-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-06 15:14:30.648428 amplify-sched-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-06 13:38:38.000000 amplify-sched-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:14:30.646428 amplify-sched-0.0.1/amplify_sched/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-30 08:18:25.000000 amplify-sched-0.0.1/amplify_sched/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    71139 2023-05-06 13:38:38.000000 amplify-sched-0.0.1/amplify_sched/amplify_sched.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:14:30.648428 amplify-sched-0.0.1/amplify_sched.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-06 15:14:30.000000 amplify-sched-0.0.1/amplify_sched.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-06 15:14:30.000000 amplify-sched-0.0.1/amplify_sched.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 15:14:30.000000 amplify-sched-0.0.1/amplify_sched.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 15:14:30.000000 amplify-sched-0.0.1/amplify_sched.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-06 15:14:30.000000 amplify-sched-0.0.1/amplify_sched.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-06 15:14:30.000000 amplify-sched-0.0.1/amplify_sched.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-30 08:18:25.000000 amplify-sched-0.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1138 2023-05-06 15:14:30.649428 amplify-sched-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-30 08:18:25.000000 amplify-sched-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:14:30.648428 amplify-sched-0.0.1/test/
--rw-rw-rw-   0 root         (0) root         (0)    10483 2023-05-06 14:37:14.000000 amplify-sched-0.0.1/test/test_scheduling_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:10:30.551874 amplify-sched-0.0.1rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-06 13:35:12.000000 amplify-sched-0.0.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-06 14:10:30.551874 amplify-sched-0.0.1rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-06 13:35:12.000000 amplify-sched-0.0.1rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:10:30.549873 amplify-sched-0.0.1rc1/amplify_sched/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-30 08:18:25.000000 amplify-sched-0.0.1rc1/amplify_sched/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    71139 2023-05-06 13:35:12.000000 amplify-sched-0.0.1rc1/amplify_sched/amplify_sched.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:10:30.550874 amplify-sched-0.0.1rc1/amplify_sched.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-06 14:10:30.000000 amplify-sched-0.0.1rc1/amplify_sched.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-06 14:10:30.000000 amplify-sched-0.0.1rc1/amplify_sched.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 14:10:30.000000 amplify-sched-0.0.1rc1/amplify_sched.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 14:10:30.000000 amplify-sched-0.0.1rc1/amplify_sched.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-06 14:10:30.000000 amplify-sched-0.0.1rc1/amplify_sched.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-06 14:10:30.000000 amplify-sched-0.0.1rc1/amplify_sched.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-30 08:18:25.000000 amplify-sched-0.0.1rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-05-06 14:10:30.552873 amplify-sched-0.0.1rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-30 08:18:25.000000 amplify-sched-0.0.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:10:30.551874 amplify-sched-0.0.1rc1/test/
+-rw-rw-rw-   0 root         (0) root         (0)    10499 2023-05-06 10:52:08.000000 amplify-sched-0.0.1rc1/test/test_scheduling_model.py
```

### Comparing `amplify-sched-0.0.1/LICENSE` & `amplify-sched-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `amplify-sched-0.0.1/PKG-INFO` & `amplify-sched-0.0.1rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplify-sched
-Version: 0.0.1
+Version: 0.0.1rc1
 Summary: Amplify Scheduling Engine SDK
 Home-page: https://amplify.fixstars.com
 Author: Kosuzke Suzuki
 Author-email: kosuke.suzuki@fixstars.com
 Keywords: fixstars,amplify,sdk,job-shop,scheduling,operations research,optimization
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
```

### Comparing `amplify-sched-0.0.1/amplify_sched/amplify_sched.py` & `amplify-sched-0.0.1rc1/amplify_sched/amplify_sched.py`

 * *Files identical despite different names*

### Comparing `amplify-sched-0.0.1/amplify_sched.egg-info/PKG-INFO` & `amplify-sched-0.0.1rc1/amplify_sched.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplify-sched
-Version: 0.0.1
+Version: 0.0.1rc1
 Summary: Amplify Scheduling Engine SDK
 Home-page: https://amplify.fixstars.com
 Author: Kosuzke Suzuki
 Author-email: kosuke.suzuki@fixstars.com
 Keywords: fixstars,amplify,sdk,job-shop,scheduling,operations research,optimization
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
```

### Comparing `amplify-sched-0.0.1/setup.cfg` & `amplify-sched-0.0.1rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amplify-sched
-version = 0.0.1
+version = 0.0.1-rc.1
 author = Kosuzke Suzuki
 author_email = kosuke.suzuki@fixstars.com
 url = https://amplify.fixstars.com
 description = Amplify Scheduling Engine SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files =
```

### Comparing `amplify-sched-0.0.1/test/test_scheduling_model.py` & `amplify-sched-0.0.1rc1/test/test_scheduling_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     model.jobs["J2"].task(0).deadline = 20
     t = Task()
     model.jobs["J3"].append(t)
     t.processing_times["M2"] = 5
 
     model.machines["M1"].add_setup_time(10, "J1", "J2")
     data = model._create_request_data(10)
+    print(data)
     assert data == {
         "model": {
             "jobs": [
                 {"tasks": [{"processing_times": [[10, 0], [5, 1]], "transportation_times": [[10, 1, 0], [10, 0, 1]]}]},
                 {
                     "tasks": [
                         {
```

