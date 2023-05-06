# Comparing `tmp/django-webperformers-humans-0.2.tar.gz` & `tmp/django-webperformers-humans-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webperformers-humans-0.2.tar", last modified: Fri May  5 11:00:49 2023, max compression
+gzip compressed data, was "django-webperformers-humans-0.3.tar", last modified: Sat May  6 12:05:45 2023, max compression
```

## Comparing `django-webperformers-humans-0.2.tar` & `django-webperformers-humans-0.3.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-05 11:00:49.312456 django-webperformers-humans-0.2/
--rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-05 09:44:22.000000 django-webperformers-humans-0.2/LICENSE
--rw-r--r--   0 tadas     (1000) tadas     (1000)      128 2023-05-05 10:07:38.000000 django-webperformers-humans-0.2/MANIFEST.in
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2026 2023-05-05 11:00:49.312456 django-webperformers-humans-0.2/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)      963 2023-05-05 10:59:11.000000 django-webperformers-humans-0.2/README.rst
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-05 11:00:49.302456 django-webperformers-humans-0.2/django_webperformers_humans.egg-info/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2026 2023-05-05 11:00:49.000000 django-webperformers-humans-0.2/django_webperformers_humans.egg-info/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)      828 2023-05-05 11:00:49.000000 django-webperformers-humans-0.2/django_webperformers_humans.egg-info/SOURCES.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-05 11:00:49.000000 django-webperformers-humans-0.2/django_webperformers_humans.egg-info/dependency_links.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-05 11:00:49.000000 django-webperformers-humans-0.2/django_webperformers_humans.egg-info/requires.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-05 11:00:49.000000 django-webperformers-humans-0.2/django_webperformers_humans.egg-info/top_level.txt
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-05 11:00:49.302456 django-webperformers-humans-0.2/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      168 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/admin.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/apps.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-05 11:00:49.302456 django-webperformers-humans-0.2/humans/helpers/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 10:11:08.000000 django-webperformers-humans-0.2/humans/helpers/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/helpers/images.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-05 11:00:49.302456 django-webperformers-humans-0.2/humans/migrations/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1252 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/migrations/0001_initial.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      369 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/migrations/0002_human_position.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      377 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/migrations/0003_human_twitterurl.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      720 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/migrations/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      930 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/models.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-05 11:00:49.302456 django-webperformers-humans-0.2/humans/signals/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/signals/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/signals/humans.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-05 11:00:49.312456 django-webperformers-humans-0.2/humans/templatetags/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/templatetags/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/templatetags/images.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/tests.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/urls.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2180 2023-05-05 09:01:31.000000 django-webperformers-humans-0.2/humans/views.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-05 09:45:45.000000 django-webperformers-humans-0.2/pyproject.toml
--rw-r--r--   0 tadas     (1000) tadas     (1000)      937 2023-05-05 11:00:49.312456 django-webperformers-humans-0.2/setup.cfg
--rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-05 10:56:42.000000 django-webperformers-humans-0.2/setup.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-05 09:44:22.000000 django-webperformers-humans-0.3/LICENSE
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 11:52:59.000000 django-webperformers-humans-0.3/MANIFEST.in
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2199 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1136 2023-05-06 12:05:42.000000 django-webperformers-humans-0.3/README.rst
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.167135 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2199 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      949 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/SOURCES.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/dependency_links.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/requires.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/top_level.txt
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.167135 django-webperformers-humans-0.3/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      168 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/admin.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/apps.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.167135 django-webperformers-humans-0.3/humans/helpers/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 10:11:08.000000 django-webperformers-humans-0.3/humans/helpers/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/helpers/images.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/humans/migrations/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1252 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/0001_initial.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      369 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/0002_human_position.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      377 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/0003_human_twitterurl.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      720 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      930 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/models.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/humans/signals/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/signals/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/signals/humans.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.167135 django-webperformers-humans-0.3/humans/templates/
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/humans/templates/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3844 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/templates/humans/personPage.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3264 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/templates/humans/teamComponent.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 11:39:28.000000 django-webperformers-humans-0.3/humans/templates/humans/teamPage.html
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/humans/templatetags/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/templatetags/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/templatetags/images.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/tests.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/urls.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2180 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/views.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-05 09:45:45.000000 django-webperformers-humans-0.3/pyproject.toml
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      937 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/setup.cfg
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-05 10:56:42.000000 django-webperformers-humans-0.3/setup.py
```

### Comparing `django-webperformers-humans-0.2/LICENSE` & `django-webperformers-humans-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.2/PKG-INFO` & `django-webperformers-humans-0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.2
+Version: 0.3
 Summary: A Django app to expose project team in seo-frienly way.
 Home-page: https://www.webperformers.net/
 Author: Your Name
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -25,26 +25,29 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Django humans
 =====
 
+Warning - templates are built using TailwindCSS - you need to build a styles for them manually
+
 Humans is a Django app:
     1. Exposing hunans.txt file
     2. Exposing project team over /team/ path
     3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
     1. teamComponent.html - main component of displaying team members
     2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
     3. personPage.html - page, displayng each tem member individually, and extending base template. Base template should have humansContent block.
 
+To ovveride them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
```

### Comparing `django-webperformers-humans-0.2/README.rst` & `django-webperformers-humans-0.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Django humans
 =====
 
+Warning - templates are built using TailwindCSS - you need to build a styles for them manually
+
 Humans is a Django app:
     1. Exposing hunans.txt file
     2. Exposing project team over /team/ path
     3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
     1. teamComponent.html - main component of displaying team members
     2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
     3. personPage.html - page, displayng each tem member individually, and extending base template. Base template should have humansContent block.
 
+To ovveride them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
```

### Comparing `django-webperformers-humans-0.2/django_webperformers_humans.egg-info/PKG-INFO` & `django-webperformers-humans-0.3/django_webperformers_humans.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.2
+Version: 0.3
 Summary: A Django app to expose project team in seo-frienly way.
 Home-page: https://www.webperformers.net/
 Author: Your Name
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -25,26 +25,29 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Django humans
 =====
 
+Warning - templates are built using TailwindCSS - you need to build a styles for them manually
+
 Humans is a Django app:
     1. Exposing hunans.txt file
     2. Exposing project team over /team/ path
     3. Exposing each project team member over /team/member-name path
 
 Model Humans is created to manage team members and their information
 
 App uses templates:
     1. teamComponent.html - main component of displaying team members
     2. teamPage.html - page, including teamComponent.html component, and extending base template. Base template should have humansContent block.
     3. personPage.html - page, displayng each tem member individually, and extending base template. Base template should have humansContent block.
 
+To ovveride them, just create same files in your templates dir humans folder
 
 Quick start
 -----------
 
 1. Add "humans" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
```

### Comparing `django-webperformers-humans-0.2/django_webperformers_humans.egg-info/SOURCES.txt` & `django-webperformers-humans-0.3/django_webperformers_humans.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 humans/migrations/0001_initial.py
 humans/migrations/0002_human_position.py
 humans/migrations/0003_human_twitterurl.py
 humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
 humans/migrations/__init__.py
 humans/signals/__init__.py
 humans/signals/humans.py
+humans/templates/humans/personPage.html
+humans/templates/humans/teamComponent.html
+humans/templates/humans/teamPage.html
 humans/templatetags/__init__.py
 humans/templatetags/images.py
```

### Comparing `django-webperformers-humans-0.2/humans/helpers/images.py` & `django-webperformers-humans-0.3/humans/helpers/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.2/humans/migrations/0001_initial.py` & `django-webperformers-humans-0.3/humans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.2/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py` & `django-webperformers-humans-0.3/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.2/humans/models.py` & `django-webperformers-humans-0.3/humans/models.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.2/humans/signals/humans.py` & `django-webperformers-humans-0.3/humans/signals/humans.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.2/humans/templatetags/images.py` & `django-webperformers-humans-0.3/humans/templatetags/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.2/humans/views.py` & `django-webperformers-humans-0.3/humans/views.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.2/setup.cfg` & `django-webperformers-humans-0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-webperformers-humans
-version = 0.2
+version = 0.3
 description = A Django app to expose project team in seo-frienly way.
 url = https://www.webperformers.net/
 author = Your Name
 author_email = tadas@webperformers.net
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

