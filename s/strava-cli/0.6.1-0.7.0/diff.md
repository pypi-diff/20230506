# Comparing `tmp/strava-cli-0.6.1.tar.gz` & `tmp/strava-cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strava-cli-0.6.1.tar", last modified: Sat Sep 25 19:30:35 2021, max compression
+gzip compressed data, was "strava-cli-0.7.0.tar", last modified: Sat May  6 16:48:08 2023, max compression
```

## Comparing `strava-cli-0.6.1.tar` & `strava-cli-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:35.965279 strava-cli-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-09-25 19:30:26.000000 strava-cli-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-09-25 19:30:26.000000 strava-cli-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2021-09-25 19:30:35.961279 strava-cli-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2021-09-25 19:30:26.000000 strava-cli-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-09-25 19:30:26.000000 strava-cli-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-25 19:30:35.965279 strava-cli-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      876 2021-09-25 19:30:26.000000 strava-cli-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:35.961279 strava-cli-0.6.1/strava/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:35.961279 strava-cli-0.6.1/strava/api/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/api/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/api/activity.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/api/athlete.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/api/oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:35.961279 strava-cli-0.6.1/strava/api/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/api/templates/fail.html
--rw-r--r--   0 runner    (1001) docker     (121)      376 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/api/templates/ok.html
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/api/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:35.961279 strava-cli-0.6.1/strava/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      408 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/activities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/activity.py
--rw-r--r--   0 runner    (1001) docker     (121)      523 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/logout.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/commands/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:35.961279 strava-cli-0.6.1/strava/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/config/config_store.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/config/creds_store.py
--rw-r--r--   0 runner    (1001) docker     (121)      797 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/config/local_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-09-25 19:30:26.000000 strava-cli-0.6.1/strava/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-25 19:30:35.961279 strava-cli-0.6.1/strava_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2021-09-25 19:30:35.000000 strava-cli-0.6.1/strava_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      917 2021-09-25 19:30:35.000000 strava-cli-0.6.1/strava_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-25 19:30:35.000000 strava-cli-0.6.1/strava_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-25 19:30:35.000000 strava-cli-0.6.1/strava_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-09-25 19:30:35.000000 strava-cli-0.6.1/strava_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-25 19:30:35.000000 strava-cli-0.6.1/strava_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:48:08.054712 strava-cli-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-06 16:47:55.000000 strava-cli-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-06 16:47:55.000000 strava-cli-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-06 16:48:08.054712 strava-cli-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-06 16:47:55.000000 strava-cli-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-06 16:47:55.000000 strava-cli-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:48:08.054712 strava-cli-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-06 16:47:55.000000 strava-cli-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:48:08.050712 strava-cli-0.7.0/strava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:48:08.050712 strava-cli-0.7.0/strava/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/api/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/api/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/api/athlete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/api/oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:48:08.050712 strava-cli-0.7.0/strava/api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/api/templates/fail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/api/templates/ok.html
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/api/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:48:08.054712 strava-cli-0.7.0/strava/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/commands/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:48:08.054712 strava-cli-0.7.0/strava/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/config/config_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/config/creds_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/config/local_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-06 16:47:55.000000 strava-cli-0.7.0/strava/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:48:08.054712 strava-cli-0.7.0/strava_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-06 16:48:07.000000 strava-cli-0.7.0/strava_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-06 16:48:08.000000 strava-cli-0.7.0/strava_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:48:07.000000 strava-cli-0.7.0/strava_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-06 16:48:07.000000 strava-cli-0.7.0/strava_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 16:48:07.000000 strava-cli-0.7.0/strava_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 16:48:07.000000 strava-cli-0.7.0/strava_cli.egg-info/top_level.txt
```

### Comparing `strava-cli-0.6.1/LICENSE` & `strava-cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/PKG-INFO` & `strava-cli-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: strava-cli
-Version: 0.6.1
+Version: 0.7.0
 Summary: Strava Command-Line Tools
 Home-page: https://github.com/bwilczynski/strava-cli
 Author: Bartlomiej Wilczynski
 Author-email: me@bwilczynski.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strava command-line interface
 
 [![Build Status](https://dev.azure.com/bwilczyn/strava-cli/_apis/build/status/bwilczynski.strava-cli?branchName=master)](https://dev.azure.com/bwilczyn/strava-cli/_build/latest?definitionId=1&branchName=master)
@@ -152,9 +150,7 @@
 Error:   None
 ```
 
 Can upload multiple activities.
 ```sh
 strava upload ./*.gpx
 ```
-
-
```

### Comparing `strava-cli-0.6.1/README.md` & `strava-cli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/setup.py` & `strava-cli-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import os
 
 import setuptools
 
-VERSION = '0.6.1'
-DESCRIPTION = 'Strava Command-Line Tools'
+VERSION = "0.7.0"
+DESCRIPTION = "Strava Command-Line Tools"
 
 here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
-    python_requires='>=3.0',
-    name='strava-cli',
+    python_requires=">=3.0",
+    name="strava-cli",
     description=DESCRIPTION,
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     version=VERSION,
-    author='Bartlomiej Wilczynski',
-    author_email='me@bwilczynski.com',
-    url='https://github.com/bwilczynski/strava-cli',
+    author="Bartlomiej Wilczynski",
+    author_email="me@bwilczynski.com",
+    url="https://github.com/bwilczynski/strava-cli",
     packages=setuptools.find_packages(),
     install_requires=[
-        'click',
-        'requests',
-        'requests_oauthlib',
-        'tabulate',
-        'dateparser'
+        "click",
+        "requests",
+        "requests_oauthlib",
+        "tabulate",
+        "dateparser",
     ],
-    entry_points='''
+    entry_points="""
         [console_scripts]
         strava=strava.cli:cli
-    ''',
+    """,
     include_package_data=True,
 )
```

### Comparing `strava-cli-0.6.1/strava/api/_helpers.py` & `strava-cli-0.7.0/strava/api/_helpers.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/api/oauth2.py` & `strava-cli-0.7.0/strava/api/oauth2.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/cli.py` & `strava-cli-0.7.0/strava/cli.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/commands/activities.py` & `strava-cli-0.7.0/strava/commands/activities.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,13 +60,13 @@
 
 
 def _as_table(result):
     return [_format_summary_activity(activity) for activity in result]
 
 
 def _format_summary_activity(activity):
-    def format_name(name):
+    def format_name(name, activity):
         return format_activity_name(name, activity)
 
     formatters = {"name": format_name, **_SUMMARY_ACTIVITY_FORMATTERS}
 
     return apply_formatters(activity, formatters)
```

### Comparing `strava-cli-0.6.1/strava/commands/activity.py` & `strava-cli-0.7.0/strava/commands/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     table_format=TableFormat.PLAIN,
 )
 def _format_activity(result, output=None):
     return result if output == OutputType.JSON.value else _as_table(result)
 
 
 def _as_table(activity):
-    def format_name(name):
+    def format_name(name, activity=None):
         activity_name = format_activity_name(name, activity)
         activity_description = activity.get("description")
         return (
             f"{activity_name}{os.linesep}{activity_description}"
             if activity_description is not None
             else activity_name
         )
@@ -65,15 +65,15 @@
     def format_gear(gear):
         return f'{gear.get("name")} ({format_distance(gear.get("distance", 0))})'
 
     def format_heartrate_with_emoji(heartrate):
         return f"{click.style(emoji.RED_HEART, fg='red')} {format_heartrate(heartrate)}"
 
     def format_speed_with_emoji(speed):
-        return f"{click.style(emoji.RUNNING_SHOE, fg='yellow')} {format_speed(speed)}"
+        return f"{click.style(emoji.RUNNING_SHOE, fg='yellow')} {format_speed(speed, activity)}"
 
     def format_elevation_with_emoji(elevation):
         difference = round(elevation)
         arrow = (
             emoji.UP_ARROW
             if difference > 0
             else emoji.DOWN_ARROW
```

### Comparing `strava-cli-0.6.1/strava/commands/config.py` & `strava-cli-0.7.0/strava/commands/config.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/commands/login.py` & `strava-cli-0.7.0/strava/commands/login.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/commands/profile.py` & `strava-cli-0.7.0/strava/commands/profile.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/commands/stats.py` & `strava-cli-0.7.0/strava/commands/stats.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/commands/upload.py` & `strava-cli-0.7.0/strava/commands/upload.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/config/local_store.py` & `strava-cli-0.7.0/strava/config/local_store.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava/decorators.py` & `strava-cli-0.7.0/strava/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,27 @@
             def print_json(data):
                 prettified = json.dumps(data, indent=2, sort_keys=True)
                 click.echo(prettified)
 
             def print_table(data):
                 table_data = [data] if single else data
                 rows = [[row[header] for header in table_columns] for row in table_data]
+                output = kwargs.get("output")
+                tablefmt = table_format.value
+                if output.index("table") == 0:
+                    suffix = output.removeprefix("table")
+                    if suffix.startswith("+"):
+                        tablefmt = suffix[1:]
                 click.echo(
                     tabulate(
                         rows,
                         headers=(humanize(header) for header in table_columns)
                         if show_table_headers
                         else (),
-                        tablefmt=table_format.value,
+                        tablefmt=tablefmt,
                     )
                 )
 
             def print_quiet(data):
                 ids = [str(x.get("id")) for x in data]
                 click.echo(os.linesep.join(ids))
                 pass
```

### Comparing `strava-cli-0.6.1/strava/formatters.py` & `strava-cli-0.7.0/strava/formatters.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,79 +7,99 @@
 from strava import emoji
 import strava.settings
 
 N_A = "N/A"
 KM_TO_MI = 0.6213712
 
 
-def format_seconds(seconds):
+def format_seconds(seconds, activity=None):
     if seconds > 3600:
         mins = math.floor(seconds / 60)
         return f"{math.floor(mins / 60):.0f}h {mins % 60:.0f}m"
     else:
         return f"{math.floor(seconds / 60):02.0f}:{seconds % 60:02.0f}"
 
 
-def format_date(date):
+def format_date(date, activity=None):
     utc_date = datetime.strptime(date, "%Y-%m-%dT%H:%M:%SZ")
     return utc_date.replace(tzinfo=timezone.utc).astimezone()
 
 
-def format_distance(distance):
+def format_distance(distance, activity=None):
     distance = math.floor(distance / 10) / 100
     suffix = "km"
     if strava.settings.IMPERIAL_UNITS:
         suffix = "mi"
         distance = distance * KM_TO_MI
     return f"{distance:.2f} {suffix}"
 
 
-def format_speed(speed):
+def format_speed(speed, activity):
+    activity_types_with_speed = [
+        "alpineski",
+        "backcountryski",
+        "ebikeride",
+        "handcycle",
+        "nordicski",
+        "ride",
+        "rollerski",
+        "skateboard",
+        "snowboard",
+        "virtualride",
+    ]
+
     suffix = "km"
+    postfix = "kph"
     if strava.settings.IMPERIAL_UNITS:
         suffix = "mi"
+        postfix = "mph"
         speed = speed * KM_TO_MI
 
-    return f"{format_seconds(1000 / speed)} /{suffix}" if speed > 0 else None
+    if activity.get("type").lower() in activity_types_with_speed:
+        return f"{speed * 3.6:.1f} {postfix}" if speed > 0 else None
+    else:
+        return (
+            f"{format_seconds(1000 / speed, activity)} /{suffix}" if speed > 0 else None
+        )
 
 
-def format_heartrate(heartrate):
+def format_heartrate(heartrate, activity=None):
     return f"{heartrate:.0f} bpm"
 
 
-def format_activity_type(activity_type):
+def format_activity_type(activity_type, activity=None):
     type_emojis = {
         "run": emoji.PERSON_RUNNING,
         "walk": emoji.PERSON_WALKING,
         "ride": emoji.PERSON_BIKING,
         "swim": emoji.PERSON_SWIMMING,
         "workout": emoji.PERSON_LIFTING_WEIGHTS,
     }
     return type_emojis.get(activity_type.lower(), "")
 
 
-def format_elevation(elevation):
+def format_elevation(elevation, activity=None):
     return f"{round(elevation)} m"
 
 
 def humanize(word):
     word = word.replace("_", " ")
     word = re.sub(r"(?i)([a-z\d]*)", lambda m: m.group(1).lower(), word)
     word = re.sub(r"^\w", lambda m: m.group(0).upper(), word)
     return word
 
 
-def noop_formatter(value):
+def noop_formatter(value, activity=None):
     return value
 
 
-def format_activity_name(name, activity):
+def format_activity_name(name, activity=None):
     activity_type = format_activity_type(activity.get("type"))
     is_race = activity.get("workout_type", 0) == 1
     return f"{activity_type} {click.style(name, bold=is_race)}"
 
 
 def apply_formatters(activity, formatters):
     return {
-        k: formatter(activity[k]) if k in activity else N_A
+        k: formatter(activity[k], activity) if k in activity else N_A
         for k, formatter in formatters.items()
     }
```

### Comparing `strava-cli-0.6.1/strava/settings.py` & `strava-cli-0.7.0/strava/settings.py`

 * *Files identical despite different names*

### Comparing `strava-cli-0.6.1/strava_cli.egg-info/PKG-INFO` & `strava-cli-0.7.0/strava_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: strava-cli
-Version: 0.6.1
+Version: 0.7.0
 Summary: Strava Command-Line Tools
 Home-page: https://github.com/bwilczynski/strava-cli
 Author: Bartlomiej Wilczynski
 Author-email: me@bwilczynski.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strava command-line interface
 
 [![Build Status](https://dev.azure.com/bwilczyn/strava-cli/_apis/build/status/bwilczynski.strava-cli?branchName=master)](https://dev.azure.com/bwilczyn/strava-cli/_build/latest?definitionId=1&branchName=master)
@@ -152,9 +150,7 @@
 Error:   None
 ```
 
 Can upload multiple activities.
 ```sh
 strava upload ./*.gpx
 ```
-
-
```

### Comparing `strava-cli-0.6.1/strava_cli.egg-info/SOURCES.txt` & `strava-cli-0.7.0/strava_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

