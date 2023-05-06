# Comparing `tmp/django-webperformers-humans-0.3.tar.gz` & `tmp/django-webperformers-humans-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webperformers-humans-0.3.tar", last modified: Sat May  6 12:05:45 2023, max compression
+gzip compressed data, was "django-webperformers-humans-0.3.1.tar", last modified: Sat May  6 12:18:54 2023, max compression
```

## Comparing `django-webperformers-humans-0.3.tar` & `django-webperformers-humans-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/
--rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-05 09:44:22.000000 django-webperformers-humans-0.3/LICENSE
--rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 11:52:59.000000 django-webperformers-humans-0.3/MANIFEST.in
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2199 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1136 2023-05-06 12:05:42.000000 django-webperformers-humans-0.3/README.rst
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.167135 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2199 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)      949 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/SOURCES.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/dependency_links.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/requires.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-06 12:05:45.000000 django-webperformers-humans-0.3/django_webperformers_humans.egg-info/top_level.txt
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.167135 django-webperformers-humans-0.3/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      168 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/admin.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/apps.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.167135 django-webperformers-humans-0.3/humans/helpers/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 10:11:08.000000 django-webperformers-humans-0.3/humans/helpers/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/helpers/images.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/humans/migrations/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1252 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/0001_initial.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      369 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/0002_human_position.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      377 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/0003_human_twitterurl.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      720 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/migrations/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      930 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/models.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/humans/signals/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/signals/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/signals/humans.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.167135 django-webperformers-humans-0.3/humans/templates/
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/humans/templates/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     3844 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/templates/humans/personPage.html
--rw-r--r--   0 tadas     (1000) tadas     (1000)     3264 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/templates/humans/teamComponent.html
--rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 11:39:28.000000 django-webperformers-humans-0.3/humans/templates/humans/teamPage.html
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/humans/templatetags/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/templatetags/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/templatetags/images.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/tests.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/urls.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2180 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3/humans/views.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-05 09:45:45.000000 django-webperformers-humans-0.3/pyproject.toml
--rw-r--r--   0 tadas     (1000) tadas     (1000)      937 2023-05-06 12:05:45.177135 django-webperformers-humans-0.3/setup.cfg
--rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-05 10:56:42.000000 django-webperformers-humans-0.3/setup.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-05 09:44:22.000000 django-webperformers-humans-0.3.1/LICENSE
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 11:52:59.000000 django-webperformers-humans-0.3.1/MANIFEST.in
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2201 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1136 2023-05-06 12:05:42.000000 django-webperformers-humans-0.3.1/README.rst
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2201 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      949 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/SOURCES.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/dependency_links.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/requires.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-06 12:18:54.000000 django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/top_level.txt
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      168 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/admin.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/apps.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/helpers/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 10:11:08.000000 django-webperformers-humans-0.3.1/humans/helpers/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/helpers/images.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/migrations/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1252 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/0001_initial.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      369 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/0002_human_position.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      377 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/0003_human_twitterurl.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      720 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/migrations/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      930 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/models.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/signals/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/signals/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/signals/humans.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.666770 django-webperformers-humans-0.3.1/humans/templates/
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/templates/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3844 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/templates/humans/personPage.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3264 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/templates/humans/teamComponent.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 11:39:28.000000 django-webperformers-humans-0.3.1/humans/templates/humans/teamPage.html
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/humans/templatetags/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/templatetags/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/templatetags/images.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/tests.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-05 09:01:31.000000 django-webperformers-humans-0.3.1/humans/urls.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2215 2023-05-06 12:18:18.000000 django-webperformers-humans-0.3.1/humans/views.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-05 09:45:45.000000 django-webperformers-humans-0.3.1/pyproject.toml
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      939 2023-05-06 12:18:54.676770 django-webperformers-humans-0.3.1/setup.cfg
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-05 10:56:42.000000 django-webperformers-humans-0.3.1/setup.py
```

### Comparing `django-webperformers-humans-0.3/LICENSE` & `django-webperformers-humans-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/PKG-INFO` & `django-webperformers-humans-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.3
+Version: 0.3.1
 Summary: A Django app to expose project team in seo-frienly way.
 Home-page: https://www.webperformers.net/
 Author: Your Name
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-webperformers-humans-0.3/README.rst` & `django-webperformers-humans-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/django_webperformers_humans.egg-info/PKG-INFO` & `django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.3
+Version: 0.3.1
 Summary: A Django app to expose project team in seo-frienly way.
 Home-page: https://www.webperformers.net/
 Author: Your Name
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-webperformers-humans-0.3/django_webperformers_humans.egg-info/SOURCES.txt` & `django-webperformers-humans-0.3.1/django_webperformers_humans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/helpers/images.py` & `django-webperformers-humans-0.3.1/humans/helpers/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/migrations/0001_initial.py` & `django-webperformers-humans-0.3.1/humans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py` & `django-webperformers-humans-0.3.1/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/models.py` & `django-webperformers-humans-0.3.1/humans/models.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/signals/humans.py` & `django-webperformers-humans-0.3.1/humans/signals/humans.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/templates/humans/personPage.html` & `django-webperformers-humans-0.3.1/humans/templates/humans/personPage.html`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/templates/humans/teamComponent.html` & `django-webperformers-humans-0.3.1/humans/templates/humans/teamComponent.html`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/templatetags/images.py` & `django-webperformers-humans-0.3.1/humans/templatetags/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3/humans/views.py` & `django-webperformers-humans-0.3.1/humans/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.http import Http404, HttpRequest, HttpResponse
+from django.http import Http404, HttpRequest, HttpResponse, HttpResponseNotFound
 from django.shortcuts import render
 from django.conf import settings
 from humans.models import Human
 from django.db.models import QuerySet
 from django.views.decorators.http import require_GET
 from django.utils.html import strip_tags
 
@@ -15,42 +15,41 @@
     team:QuerySet
     if request.user.is_superuser:
         team:QuerySet = Human.objects.all()
     else:
         team:QuerySet = Human.objects.filter(isPublished=True)
     return team
 
-# Create your views here.
 def teamPageView(request:HttpRequest):
     context:dict = {}
     getBaseTemplate(context)
     team:QuerySet = getTeam(request)
     if (team.__len__() > 0 or request.user.is_superuser):
         context["team"] = team
         return render(request, 'humans/teamPage.html', context=context)
     else:
-        return Http404()
+        return HttpResponseNotFound()
 
 def personView (request:HttpRequest, personSlug:str):
     context:dict = {}
     getBaseTemplate(context)
     try:
         person:Human = Human.objects.get(customSlug=personSlug)
         context["person"] = person
         return render(request, 'humans/personPage.html', context=context)
     except Human.DoesNotExist:
-        return Http404()
+        return HttpResponseNotFound()
 
 @require_GET
 def humans_txt(request):
     response:str = "/* TEAM */\n\n"
     team:QuerySet = getTeam(request)
     if (team.__len__() > 0 or request.user.is_superuser):
         person:Human
         for person in team:
             personString:str = "--------------------------------------------\n"
             personString = personString + f"""Title: {person.position}\nName: {person.name}\nSite: {person.websiteUrl}\nTwitter: {person.twitterUrl}\nLinkedIn: {person.linkedInUrl}\nAbout:\n{strip_tags(person.smallDescription)}\n"""
             personString = personString + "--------------------------------------------\n"
             response = response + personString
         return HttpResponse (response, content_type="text/plain")
     else:
-        return Http404()
+        return HttpResponseNotFound()
```

### Comparing `django-webperformers-humans-0.3/setup.cfg` & `django-webperformers-humans-0.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-webperformers-humans
-version = 0.3
+version = 0.3.1
 description = A Django app to expose project team in seo-frienly way.
 url = https://www.webperformers.net/
 author = Your Name
 author_email = tadas@webperformers.net
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

