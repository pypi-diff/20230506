# Comparing `tmp/django-vectordb-0.1.0.tar.gz` & `tmp/django-vectordb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vectordb-0.1.0.tar", last modified: Fri May  5 07:22:14 2023, max compression
+gzip compressed data, was "django-vectordb-0.1.1.tar", last modified: Sat May  6 08:32:12 2023, max compression
```

## Comparing `django-vectordb-0.1.0.tar` & `django-vectordb-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,59 @@
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-05 07:22:14.905392 django-vectordb-0.1.0/
--rw-r--r--   0 pride      (501) staff       (20)    11357 2023-05-04 13:28:35.000000 django-vectordb-0.1.0/LICENSE
--rw-r--r--   0 pride      (501) staff       (20)    10200 2023-05-05 07:22:14.905545 django-vectordb-0.1.0/PKG-INFO
--rw-r--r--   0 pride      (501) staff       (20)     8800 2023-05-05 05:16:49.000000 django-vectordb-0.1.0/README.md
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-05 07:22:14.889410 django-vectordb-0.1.0/django_vectordb.egg-info/
--rw-r--r--   0 pride      (501) staff       (20)    10200 2023-05-05 07:22:14.000000 django-vectordb-0.1.0/django_vectordb.egg-info/PKG-INFO
--rw-r--r--   0 pride      (501) staff       (20)     1096 2023-05-05 07:22:14.000000 django-vectordb-0.1.0/django_vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 pride      (501) staff       (20)        1 2023-05-05 07:22:14.000000 django-vectordb-0.1.0/django_vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 pride      (501) staff       (20)      319 2023-05-05 07:22:14.000000 django-vectordb-0.1.0/django_vectordb.egg-info/requires.txt
--rw-r--r--   0 pride      (501) staff       (20)        9 2023-05-05 07:22:14.000000 django-vectordb-0.1.0/django_vectordb.egg-info/top_level.txt
--rw-r--r--   0 pride      (501) staff       (20)       80 2023-05-04 08:19:18.000000 django-vectordb-0.1.0/pyproject.toml
--rw-r--r--   0 pride      (501) staff       (20)     1888 2023-05-05 07:22:14.907024 django-vectordb-0.1.0/setup.cfg
--rw-r--r--   0 pride      (501) staff       (20)      216 2023-05-05 07:20:09.000000 django-vectordb-0.1.0/setup.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-05 07:22:14.898553 django-vectordb-0.1.0/vectordb/
--rw-r--r--   0 pride      (501) staff       (20)      291 2023-05-04 15:04:49.000000 django-vectordb-0.1.0/vectordb/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)      527 2023-05-05 06:20:34.000000 django-vectordb-0.1.0/vectordb/admin.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-05 07:22:14.900196 django-vectordb-0.1.0/vectordb/ann/
--rw-r--r--   0 pride      (501) staff       (20)      115 2023-05-03 14:11:45.000000 django-vectordb-0.1.0/vectordb/ann/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)     1051 2023-05-03 14:11:45.000000 django-vectordb-0.1.0/vectordb/ann/abcz.py
--rw-r--r--   0 pride      (501) staff       (20)     5918 2023-05-04 15:47:14.000000 django-vectordb-0.1.0/vectordb/ann/indexes.py
--rw-r--r--   0 pride      (501) staff       (20)      603 2023-05-04 15:46:27.000000 django-vectordb-0.1.0/vectordb/ann/singleton.py
--rw-r--r--   0 pride      (501) staff       (20)      248 2023-05-03 20:04:15.000000 django-vectordb-0.1.0/vectordb/apps.py
--rw-r--r--   0 pride      (501) staff       (20)     1827 2023-05-04 04:39:07.000000 django-vectordb-0.1.0/vectordb/embedding_functions.py
--rw-r--r--   0 pride      (501) staff       (20)     2813 2023-05-05 07:01:23.000000 django-vectordb-0.1.0/vectordb/manager.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-05 07:22:14.901346 django-vectordb-0.1.0/vectordb/migrations/
--rw-r--r--   0 pride      (501) staff       (20)     1892 2023-05-03 14:16:42.000000 django-vectordb-0.1.0/vectordb/migrations/0001_initial.py
--rw-r--r--   0 pride      (501) staff       (20)      887 2023-05-03 20:38:37.000000 django-vectordb-0.1.0/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py
--rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-03 14:10:09.000000 django-vectordb-0.1.0/vectordb/migrations/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)     2099 2023-05-04 20:10:03.000000 django-vectordb-0.1.0/vectordb/models.py
--rw-r--r--   0 pride      (501) staff       (20)     3824 2023-05-05 06:34:38.000000 django-vectordb-0.1.0/vectordb/queryset.py
--rw-r--r--   0 pride      (501) staff       (20)      342 2023-05-03 14:26:35.000000 django-vectordb-0.1.0/vectordb/serializers.py
--rw-r--r--   0 pride      (501) staff       (20)     1528 2023-05-05 06:33:16.000000 django-vectordb-0.1.0/vectordb/signals.py
--rw-r--r--   0 pride      (501) staff       (20)     1971 2023-05-04 20:13:05.000000 django-vectordb-0.1.0/vectordb/sync_signals.py
--rw-r--r--   0 pride      (501) staff       (20)     1475 2023-05-04 04:00:22.000000 django-vectordb-0.1.0/vectordb/tasks.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-05 07:22:14.905141 django-vectordb-0.1.0/vectordb/tests/
--rw-r--r--   0 pride      (501) staff       (20)       54 2023-05-04 20:37:23.000000 django-vectordb-0.1.0/vectordb/tests/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)      122 2023-05-04 20:37:23.000000 django-vectordb-0.1.0/vectordb/tests/apps.py
--rw-r--r--   0 pride      (501) staff       (20)      346 2023-05-04 20:37:23.000000 django-vectordb-0.1.0/vectordb/tests/models.py
--rw-r--r--   0 pride      (501) staff       (20)     1794 2023-05-04 13:22:55.000000 django-vectordb-0.1.0/vectordb/tests/settings.py
--rw-r--r--   0 pride      (501) staff       (20)     1170 2023-05-04 20:41:32.000000 django-vectordb-0.1.0/vectordb/tests/test_api_endpoint.py
--rw-r--r--   0 pride      (501) staff       (20)     2970 2023-05-04 20:41:19.000000 django-vectordb-0.1.0/vectordb/tests/test_db_indexes.py
--rw-r--r--   0 pride      (501) staff       (20)      686 2023-05-03 14:14:51.000000 django-vectordb-0.1.0/vectordb/tests/test_embedding_functions.py
--rw-r--r--   0 pride      (501) staff       (20)      627 2023-05-04 20:42:47.000000 django-vectordb-0.1.0/vectordb/tests/test_singleton_meta.py
--rw-r--r--   0 pride      (501) staff       (20)     3547 2023-05-04 19:22:55.000000 django-vectordb-0.1.0/vectordb/tests/test_vectordb.py
--rw-r--r--   0 pride      (501) staff       (20)       60 2023-05-03 14:10:09.000000 django-vectordb-0.1.0/vectordb/tests.py
--rw-r--r--   0 pride      (501) staff       (20)      280 2023-05-04 20:40:02.000000 django-vectordb-0.1.0/vectordb/urls.py
--rw-r--r--   0 pride      (501) staff       (20)     4013 2023-05-05 06:33:37.000000 django-vectordb-0.1.0/vectordb/utils.py
--rw-r--r--   0 pride      (501) staff       (20)     1744 2023-05-04 18:22:43.000000 django-vectordb-0.1.0/vectordb/validators.py
--rw-r--r--   0 pride      (501) staff       (20)     1232 2023-05-05 06:34:07.000000 django-vectordb-0.1.0/vectordb/views.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.923607 django-vectordb-0.1.1/
+-rw-r--r--   0 pride      (501) staff       (20)    11357 2023-05-04 13:28:35.000000 django-vectordb-0.1.1/LICENSE
+-rw-r--r--   0 pride      (501) staff       (20)    11705 2023-05-06 08:32:12.923974 django-vectordb-0.1.1/PKG-INFO
+-rw-r--r--   0 pride      (501) staff       (20)    10305 2023-05-06 08:01:40.000000 django-vectordb-0.1.1/README.md
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.782469 django-vectordb-0.1.1/django_vectordb.egg-info/
+-rw-r--r--   0 pride      (501) staff       (20)    11705 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 pride      (501) staff       (20)     1365 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 pride      (501) staff       (20)        1 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 pride      (501) staff       (20)      319 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/requires.txt
+-rw-r--r--   0 pride      (501) staff       (20)        9 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/top_level.txt
+-rw-r--r--   0 pride      (501) staff       (20)       80 2023-05-04 08:19:18.000000 django-vectordb-0.1.1/pyproject.toml
+-rw-r--r--   0 pride      (501) staff       (20)     1888 2023-05-06 08:32:12.928178 django-vectordb-0.1.1/setup.cfg
+-rw-r--r--   0 pride      (501) staff       (20)      216 2023-05-05 07:20:09.000000 django-vectordb-0.1.1/setup.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.805388 django-vectordb-0.1.1/vectordb/
+-rw-r--r--   0 pride      (501) staff       (20)      291 2023-05-04 15:04:49.000000 django-vectordb-0.1.1/vectordb/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)      527 2023-05-05 06:20:34.000000 django-vectordb-0.1.1/vectordb/admin.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.811137 django-vectordb-0.1.1/vectordb/ann/
+-rw-r--r--   0 pride      (501) staff       (20)      115 2023-05-03 14:11:45.000000 django-vectordb-0.1.1/vectordb/ann/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)     1051 2023-05-03 14:11:45.000000 django-vectordb-0.1.1/vectordb/ann/abcz.py
+-rw-r--r--   0 pride      (501) staff       (20)     5918 2023-05-04 15:47:14.000000 django-vectordb-0.1.1/vectordb/ann/indexes.py
+-rw-r--r--   0 pride      (501) staff       (20)      603 2023-05-04 15:46:27.000000 django-vectordb-0.1.1/vectordb/ann/singleton.py
+-rw-r--r--   0 pride      (501) staff       (20)      248 2023-05-03 20:04:15.000000 django-vectordb-0.1.1/vectordb/apps.py
+-rw-r--r--   0 pride      (501) staff       (20)      625 2023-05-06 07:32:16.000000 django-vectordb-0.1.1/vectordb/checks.py
+-rw-r--r--   0 pride      (501) staff       (20)     1827 2023-05-04 04:39:07.000000 django-vectordb-0.1.1/vectordb/embedding_functions.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.812593 django-vectordb-0.1.1/vectordb/management/
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:40.000000 django-vectordb-0.1.1/vectordb/management/__init__.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.817051 django-vectordb-0.1.1/vectordb/management/commands/
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:44.000000 django-vectordb-0.1.1/vectordb/management/commands/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)     1020 2023-05-06 07:56:41.000000 django-vectordb-0.1.1/vectordb/management/commands/vectordb_reset.py
+-rw-r--r--   0 pride      (501) staff       (20)     2276 2023-05-06 07:56:43.000000 django-vectordb-0.1.1/vectordb/management/commands/vectordb_sync.py
+-rw-r--r--   0 pride      (501) staff       (20)     2813 2023-05-05 07:01:23.000000 django-vectordb-0.1.1/vectordb/manager.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.827774 django-vectordb-0.1.1/vectordb/migrations/
+-rw-r--r--   0 pride      (501) staff       (20)     1892 2023-05-03 14:16:42.000000 django-vectordb-0.1.1/vectordb/migrations/0001_initial.py
+-rw-r--r--   0 pride      (501) staff       (20)      887 2023-05-03 20:38:37.000000 django-vectordb-0.1.1/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-03 14:10:09.000000 django-vectordb-0.1.1/vectordb/migrations/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)     2099 2023-05-04 20:10:03.000000 django-vectordb-0.1.1/vectordb/models.py
+-rw-r--r--   0 pride      (501) staff       (20)     4464 2023-05-06 08:24:10.000000 django-vectordb-0.1.1/vectordb/queryset.py
+-rw-r--r--   0 pride      (501) staff       (20)      342 2023-05-03 14:26:35.000000 django-vectordb-0.1.1/vectordb/serializers.py
+-rw-r--r--   0 pride      (501) staff       (20)     3541 2023-05-06 07:26:56.000000 django-vectordb-0.1.1/vectordb/settings.py
+-rw-r--r--   0 pride      (501) staff       (20)     1528 2023-05-05 06:33:16.000000 django-vectordb-0.1.1/vectordb/signals.py
+-rw-r--r--   0 pride      (501) staff       (20)     1971 2023-05-04 20:13:05.000000 django-vectordb-0.1.1/vectordb/sync_signals.py
+-rw-r--r--   0 pride      (501) staff       (20)     1475 2023-05-04 04:00:22.000000 django-vectordb-0.1.1/vectordb/tasks.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.922377 django-vectordb-0.1.1/vectordb/tests/
+-rw-r--r--   0 pride      (501) staff       (20)       54 2023-05-04 20:37:23.000000 django-vectordb-0.1.1/vectordb/tests/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)      122 2023-05-04 20:37:23.000000 django-vectordb-0.1.1/vectordb/tests/apps.py
+-rw-r--r--   0 pride      (501) staff       (20)      106 2023-05-06 07:32:13.000000 django-vectordb-0.1.1/vectordb/tests/dummy_module.py
+-rw-r--r--   0 pride      (501) staff       (20)      346 2023-05-04 20:37:23.000000 django-vectordb-0.1.1/vectordb/tests/models.py
+-rw-r--r--   0 pride      (501) staff       (20)     1794 2023-05-04 13:22:55.000000 django-vectordb-0.1.1/vectordb/tests/settings.py
+-rw-r--r--   0 pride      (501) staff       (20)     1170 2023-05-04 20:41:32.000000 django-vectordb-0.1.1/vectordb/tests/test_api_endpoint.py
+-rw-r--r--   0 pride      (501) staff       (20)     2970 2023-05-04 20:41:19.000000 django-vectordb-0.1.1/vectordb/tests/test_db_indexes.py
+-rw-r--r--   0 pride      (501) staff       (20)      686 2023-05-03 14:14:51.000000 django-vectordb-0.1.1/vectordb/tests/test_embedding_functions.py
+-rw-r--r--   0 pride      (501) staff       (20)     2606 2023-05-06 07:32:11.000000 django-vectordb-0.1.1/vectordb/tests/test_settings.py
+-rw-r--r--   0 pride      (501) staff       (20)      627 2023-05-04 20:42:47.000000 django-vectordb-0.1.1/vectordb/tests/test_singleton_meta.py
+-rw-r--r--   0 pride      (501) staff       (20)     3547 2023-05-04 19:22:55.000000 django-vectordb-0.1.1/vectordb/tests/test_vectordb.py
+-rw-r--r--   0 pride      (501) staff       (20)       60 2023-05-03 14:10:09.000000 django-vectordb-0.1.1/vectordb/tests.py
+-rw-r--r--   0 pride      (501) staff       (20)      280 2023-05-04 20:40:02.000000 django-vectordb-0.1.1/vectordb/urls.py
+-rw-r--r--   0 pride      (501) staff       (20)     3549 2023-05-06 07:28:17.000000 django-vectordb-0.1.1/vectordb/utils.py
+-rw-r--r--   0 pride      (501) staff       (20)     1744 2023-05-04 18:22:43.000000 django-vectordb-0.1.1/vectordb/validators.py
+-rw-r--r--   0 pride      (501) staff       (20)     1232 2023-05-05 06:34:07.000000 django-vectordb-0.1.1/vectordb/views.py
```

### Comparing `django-vectordb-0.1.0/LICENSE` & `django-vectordb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/PKG-INFO` & `django-vectordb-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vectordb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
 Home-page: https://github.com/pkavumba/django-vectordb.git
 Author: Pride Kavumba
 Author-email: pkavumba@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
 Provides-Extra: tests
 License-File: LICENSE
 
 # Django VectorDB
 
 ---
 
-Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications.
+Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
 - Native Django integration.
@@ -52,39 +52,43 @@
 
 ## Requirements
 
 ---
 
 Django VectorDB requires the following:
 
-- Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11)
-- Django (2.2, 3.0, 3.1, 3.2, 4.0, 4.1)
-- HNSWLib (0.7.0)
-- numpy
+- [Python][python] (3.6, 3.7, 3.8, 3.9, 3.10, 3.11)
+- [Django][django] (2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2)
+- [HNSWLib][hnswlib] (0.7.0)
+- [numpy][numpy]
 
 We **highly recommend** and only officially support the latest patch release of
 each Python and Django series.
 
 The following packages are optional:
 
-- Sentence-Transformers - Add support for converting text into vector embeddings used for similarity search
-- Django Rest Framework - Add API endpoint for VectorDB.
-- django-filter - Add metadata filtering support on the API endpoint.
+- [Sentence-Transformers][sentence-transformers] - Add support for converting text into vector embeddings used for similarity search
+- [Django Rest Framework][drf] - Add API endpoint for VectorDB.
+- [django-filters][django-filters] - Add metadata filtering support on the API endpoint.
 
 ---
 
 ## Installation
 
 Install using `pip`, it is recommended that you install the optional packages with:
 
-    pip install django-vectordb[standard] # This will install the optional dependencies above.
+```bash
+    pip install "django-vectordb[standard]" # This will install the optional dependencies above.
+```
 
 If you dont want to install the optional packages you can run:
 
+```bash
     pip install django-vectordb
+```
 
 Add `'django-vectordb'` to your `INSTALLED_APPS` setting.
 
 ```python
     INSTALLED_APPS = [
         ...
         'vectordb',
@@ -173,24 +177,24 @@
         return f"{self.title} -- {self.description}"
 
     def get_vectordb_metadata(self):
         # Enable filtering by any of these metadata
         return {"title": self.title, "description": self.description, "user_id": self.user.id, "model": "post"}
 ```
 
-In an existing project, you can run the `sync_vectordb` management command to add all items to the database.
+In an existing project, you can run the `vectordb_sync` management command to add all items to the database.
 
 ```bash
-./manage.py sync_vectordb <app_name> <model_name>
+./manage.py vectordb_sync <app_name> <model_name>
 ```
 
 For this example:
 
 ```bash
-./manage.py sync_vectordb blog Post
+./manage.py vectordb_sync blog Post
 ```
 
 #### Manually adding items to the vector database
 
 VectorDB provides two utility methods for adding items to the database: `vectordb.add_instance` or `vectordb.add_text`. Note that for adding the instance, you need to provide the `get_vectordb_text` and an optional `get_vectordb_metadata` methods.
 
 ##### 1. Adding Model Instances
@@ -252,15 +256,15 @@
 
     def ready(self):
         import blog.signals
 ```
 
 These signals will sync the vectors when you create and delete instances. Note that signals are not called in bulk create, so you will need to sync manually when using those methods.
 
-Ensure that your models implement the `get_text()` and/or `serialize()` methods for proper syncing.
+Ensure that your models implement the `get_vectordb_text()` and/or `get_vectordb_metadata()` methods for proper syncing.
 
 ### Searching
 
 To search, simply call `vectordb.search()`:
 
 ```python
 vectordb.search("Some text", k=10) # k is the maximum number of results you want.
@@ -286,14 +290,32 @@
 vectordb.filter(text__icontains="Apple", metadata__title__icontains="IPhone", metadata__description__icontains="2023").search("Apple new phone", k=10)
 ```
 
 Refer to the [Django documentation](https://docs.djangoproject.com/en/4.2/topics/db/queries/) on querying the `JSONField` for more information on filtering.
 
 ---
 
+## Settings
+
+You can provide your settings in the `settings.py` file of your project. The following settings are available:
+
+```python
+    # settings.py
+    DJANGO_VECTOR_DB = {
+        "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
+        "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+        # Can be "cosine" or "l2"
+        "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
+        "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+        "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
+        "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
+        "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
+    }
+```
+
 ## Quickstart
 
 Can't wait to get started? The [quickstart guide][quickstart] is the fastest way to get up and running, and building APIs with REST framework.
 
 ---
 
 ## Development
@@ -319,7 +341,16 @@
 ```
 
 Or
 
 ```bash
 tox
 ```
+
+[python]: https://www.python.org
+[django]: https://www.djangoproject.com
+[numpy]: https://numpy.org
+[quickstart]: tutorial/quickstart.md
+[sentence-transformers]: https://www.sbert.net
+[hnswlib]: https://github.com/nmslib/hnswlib
+[drf]: https://www.django-rest-framework.org
+[django-filters]: https://pypi.org/project/django-filter/
```

### Comparing `django-vectordb-0.1.0/README.md` & `django-vectordb-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django VectorDB
 
 ---
 
-Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications.
+Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
 - Native Django integration.
@@ -17,39 +17,43 @@
 
 ## Requirements
 
 ---
 
 Django VectorDB requires the following:
 
-- Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11)
-- Django (2.2, 3.0, 3.1, 3.2, 4.0, 4.1)
-- HNSWLib (0.7.0)
-- numpy
+- [Python][python] (3.6, 3.7, 3.8, 3.9, 3.10, 3.11)
+- [Django][django] (2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2)
+- [HNSWLib][hnswlib] (0.7.0)
+- [numpy][numpy]
 
 We **highly recommend** and only officially support the latest patch release of
 each Python and Django series.
 
 The following packages are optional:
 
-- Sentence-Transformers - Add support for converting text into vector embeddings used for similarity search
-- Django Rest Framework - Add API endpoint for VectorDB.
-- django-filter - Add metadata filtering support on the API endpoint.
+- [Sentence-Transformers][sentence-transformers] - Add support for converting text into vector embeddings used for similarity search
+- [Django Rest Framework][drf] - Add API endpoint for VectorDB.
+- [django-filters][django-filters] - Add metadata filtering support on the API endpoint.
 
 ---
 
 ## Installation
 
 Install using `pip`, it is recommended that you install the optional packages with:
 
-    pip install django-vectordb[standard] # This will install the optional dependencies above.
+```bash
+    pip install "django-vectordb[standard]" # This will install the optional dependencies above.
+```
 
 If you dont want to install the optional packages you can run:
 
+```bash
     pip install django-vectordb
+```
 
 Add `'django-vectordb'` to your `INSTALLED_APPS` setting.
 
 ```python
     INSTALLED_APPS = [
         ...
         'vectordb',
@@ -138,24 +142,24 @@
         return f"{self.title} -- {self.description}"
 
     def get_vectordb_metadata(self):
         # Enable filtering by any of these metadata
         return {"title": self.title, "description": self.description, "user_id": self.user.id, "model": "post"}
 ```
 
-In an existing project, you can run the `sync_vectordb` management command to add all items to the database.
+In an existing project, you can run the `vectordb_sync` management command to add all items to the database.
 
 ```bash
-./manage.py sync_vectordb <app_name> <model_name>
+./manage.py vectordb_sync <app_name> <model_name>
 ```
 
 For this example:
 
 ```bash
-./manage.py sync_vectordb blog Post
+./manage.py vectordb_sync blog Post
 ```
 
 #### Manually adding items to the vector database
 
 VectorDB provides two utility methods for adding items to the database: `vectordb.add_instance` or `vectordb.add_text`. Note that for adding the instance, you need to provide the `get_vectordb_text` and an optional `get_vectordb_metadata` methods.
 
 ##### 1. Adding Model Instances
@@ -217,15 +221,15 @@
 
     def ready(self):
         import blog.signals
 ```
 
 These signals will sync the vectors when you create and delete instances. Note that signals are not called in bulk create, so you will need to sync manually when using those methods.
 
-Ensure that your models implement the `get_text()` and/or `serialize()` methods for proper syncing.
+Ensure that your models implement the `get_vectordb_text()` and/or `get_vectordb_metadata()` methods for proper syncing.
 
 ### Searching
 
 To search, simply call `vectordb.search()`:
 
 ```python
 vectordb.search("Some text", k=10) # k is the maximum number of results you want.
@@ -251,14 +255,32 @@
 vectordb.filter(text__icontains="Apple", metadata__title__icontains="IPhone", metadata__description__icontains="2023").search("Apple new phone", k=10)
 ```
 
 Refer to the [Django documentation](https://docs.djangoproject.com/en/4.2/topics/db/queries/) on querying the `JSONField` for more information on filtering.
 
 ---
 
+## Settings
+
+You can provide your settings in the `settings.py` file of your project. The following settings are available:
+
+```python
+    # settings.py
+    DJANGO_VECTOR_DB = {
+        "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
+        "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+        # Can be "cosine" or "l2"
+        "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
+        "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+        "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
+        "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
+        "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
+    }
+```
+
 ## Quickstart
 
 Can't wait to get started? The [quickstart guide][quickstart] is the fastest way to get up and running, and building APIs with REST framework.
 
 ---
 
 ## Development
@@ -284,7 +306,16 @@
 ```
 
 Or
 
 ```bash
 tox
 ```
+
+[python]: https://www.python.org
+[django]: https://www.djangoproject.com
+[numpy]: https://numpy.org
+[quickstart]: tutorial/quickstart.md
+[sentence-transformers]: https://www.sbert.net
+[hnswlib]: https://github.com/nmslib/hnswlib
+[drf]: https://www.django-rest-framework.org
+[django-filters]: https://pypi.org/project/django-filter/
```

### Comparing `django-vectordb-0.1.0/django_vectordb.egg-info/PKG-INFO` & `django-vectordb-0.1.1/django_vectordb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vectordb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
 Home-page: https://github.com/pkavumba/django-vectordb.git
 Author: Pride Kavumba
 Author-email: pkavumba@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
 Provides-Extra: tests
 License-File: LICENSE
 
 # Django VectorDB
 
 ---
 
-Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications.
+Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
 - Native Django integration.
@@ -52,39 +52,43 @@
 
 ## Requirements
 
 ---
 
 Django VectorDB requires the following:
 
-- Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11)
-- Django (2.2, 3.0, 3.1, 3.2, 4.0, 4.1)
-- HNSWLib (0.7.0)
-- numpy
+- [Python][python] (3.6, 3.7, 3.8, 3.9, 3.10, 3.11)
+- [Django][django] (2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2)
+- [HNSWLib][hnswlib] (0.7.0)
+- [numpy][numpy]
 
 We **highly recommend** and only officially support the latest patch release of
 each Python and Django series.
 
 The following packages are optional:
 
-- Sentence-Transformers - Add support for converting text into vector embeddings used for similarity search
-- Django Rest Framework - Add API endpoint for VectorDB.
-- django-filter - Add metadata filtering support on the API endpoint.
+- [Sentence-Transformers][sentence-transformers] - Add support for converting text into vector embeddings used for similarity search
+- [Django Rest Framework][drf] - Add API endpoint for VectorDB.
+- [django-filters][django-filters] - Add metadata filtering support on the API endpoint.
 
 ---
 
 ## Installation
 
 Install using `pip`, it is recommended that you install the optional packages with:
 
-    pip install django-vectordb[standard] # This will install the optional dependencies above.
+```bash
+    pip install "django-vectordb[standard]" # This will install the optional dependencies above.
+```
 
 If you dont want to install the optional packages you can run:
 
+```bash
     pip install django-vectordb
+```
 
 Add `'django-vectordb'` to your `INSTALLED_APPS` setting.
 
 ```python
     INSTALLED_APPS = [
         ...
         'vectordb',
@@ -173,24 +177,24 @@
         return f"{self.title} -- {self.description}"
 
     def get_vectordb_metadata(self):
         # Enable filtering by any of these metadata
         return {"title": self.title, "description": self.description, "user_id": self.user.id, "model": "post"}
 ```
 
-In an existing project, you can run the `sync_vectordb` management command to add all items to the database.
+In an existing project, you can run the `vectordb_sync` management command to add all items to the database.
 
 ```bash
-./manage.py sync_vectordb <app_name> <model_name>
+./manage.py vectordb_sync <app_name> <model_name>
 ```
 
 For this example:
 
 ```bash
-./manage.py sync_vectordb blog Post
+./manage.py vectordb_sync blog Post
 ```
 
 #### Manually adding items to the vector database
 
 VectorDB provides two utility methods for adding items to the database: `vectordb.add_instance` or `vectordb.add_text`. Note that for adding the instance, you need to provide the `get_vectordb_text` and an optional `get_vectordb_metadata` methods.
 
 ##### 1. Adding Model Instances
@@ -252,15 +256,15 @@
 
     def ready(self):
         import blog.signals
 ```
 
 These signals will sync the vectors when you create and delete instances. Note that signals are not called in bulk create, so you will need to sync manually when using those methods.
 
-Ensure that your models implement the `get_text()` and/or `serialize()` methods for proper syncing.
+Ensure that your models implement the `get_vectordb_text()` and/or `get_vectordb_metadata()` methods for proper syncing.
 
 ### Searching
 
 To search, simply call `vectordb.search()`:
 
 ```python
 vectordb.search("Some text", k=10) # k is the maximum number of results you want.
@@ -286,14 +290,32 @@
 vectordb.filter(text__icontains="Apple", metadata__title__icontains="IPhone", metadata__description__icontains="2023").search("Apple new phone", k=10)
 ```
 
 Refer to the [Django documentation](https://docs.djangoproject.com/en/4.2/topics/db/queries/) on querying the `JSONField` for more information on filtering.
 
 ---
 
+## Settings
+
+You can provide your settings in the `settings.py` file of your project. The following settings are available:
+
+```python
+    # settings.py
+    DJANGO_VECTOR_DB = {
+        "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
+        "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+        # Can be "cosine" or "l2"
+        "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
+        "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+        "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
+        "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
+        "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
+    }
+```
+
 ## Quickstart
 
 Can't wait to get started? The [quickstart guide][quickstart] is the fastest way to get up and running, and building APIs with REST framework.
 
 ---
 
 ## Development
@@ -319,7 +341,16 @@
 ```
 
 Or
 
 ```bash
 tox
 ```
+
+[python]: https://www.python.org
+[django]: https://www.djangoproject.com
+[numpy]: https://numpy.org
+[quickstart]: tutorial/quickstart.md
+[sentence-transformers]: https://www.sbert.net
+[hnswlib]: https://github.com/nmslib/hnswlib
+[drf]: https://www.django-rest-framework.org
+[django-filters]: https://pypi.org/project/django-filter/
```

### Comparing `django-vectordb-0.1.0/django_vectordb.egg-info/SOURCES.txt` & `django-vectordb-0.1.1/django_vectordb.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -7,36 +7,44 @@
 django_vectordb.egg-info/SOURCES.txt
 django_vectordb.egg-info/dependency_links.txt
 django_vectordb.egg-info/requires.txt
 django_vectordb.egg-info/top_level.txt
 vectordb/__init__.py
 vectordb/admin.py
 vectordb/apps.py
+vectordb/checks.py
 vectordb/embedding_functions.py
 vectordb/manager.py
 vectordb/models.py
 vectordb/queryset.py
 vectordb/serializers.py
+vectordb/settings.py
 vectordb/signals.py
 vectordb/sync_signals.py
 vectordb/tasks.py
 vectordb/tests.py
 vectordb/urls.py
 vectordb/utils.py
 vectordb/validators.py
 vectordb/views.py
 vectordb/ann/__init__.py
 vectordb/ann/abcz.py
 vectordb/ann/indexes.py
 vectordb/ann/singleton.py
+vectordb/management/__init__.py
+vectordb/management/commands/__init__.py
+vectordb/management/commands/vectordb_reset.py
+vectordb/management/commands/vectordb_sync.py
 vectordb/migrations/0001_initial.py
 vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py
 vectordb/migrations/__init__.py
 vectordb/tests/__init__.py
 vectordb/tests/apps.py
+vectordb/tests/dummy_module.py
 vectordb/tests/models.py
 vectordb/tests/settings.py
 vectordb/tests/test_api_endpoint.py
 vectordb/tests/test_db_indexes.py
 vectordb/tests/test_embedding_functions.py
+vectordb/tests/test_settings.py
 vectordb/tests/test_singleton_meta.py
 vectordb/tests/test_vectordb.py
```

### Comparing `django-vectordb-0.1.0/setup.cfg` & `django-vectordb-0.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-vectordb
-version = 0.1.0
+version = 0.1.1
 description = Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
 long_description = file: README.md
 url = https://github.com/pkavumba/django-vectordb.git
 author = Pride Kavumba
 author_email = pkavumba@gmail.com
 license = Apache License 2.0
 classifiers =
```

### Comparing `django-vectordb-0.1.0/vectordb/admin.py` & `django-vectordb-0.1.1/vectordb/admin.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/ann/abcz.py` & `django-vectordb-0.1.1/vectordb/ann/abcz.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/ann/indexes.py` & `django-vectordb-0.1.1/vectordb/ann/indexes.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/ann/singleton.py` & `django-vectordb-0.1.1/vectordb/ann/singleton.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/embedding_functions.py` & `django-vectordb-0.1.1/vectordb/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/manager.py` & `django-vectordb-0.1.1/vectordb/manager.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/migrations/0001_initial.py` & `django-vectordb-0.1.1/vectordb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py` & `django-vectordb-0.1.1/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/models.py` & `django-vectordb-0.1.1/vectordb/models.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/queryset.py` & `django-vectordb-0.1.1/vectordb/queryset.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 
 import logging
 import time
 import numpy as np
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from .ann.indexes import HNSWIndex, BFIndex
+from vectordb.settings import vectordb_settings
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(" VectorDB ")
 
 
 class VectorQuerySet(models.QuerySet):
-    def _get_related_vectors(self, query_embeddings, vectors, k=10, ids_list=None):
+    def _get_related_vectors(
+        self, query_embeddings, vectors, k: int | None = None, ids_list=None
+    ):
+        if k is None:
+            k = vectordb_settings.DEFAULT_MAX_N_RESULTS
         manager = self.model.objects
         vector_count = len(vectors)
         # k cannot be greater than the number of vectors. Don't raise an error
         k = min(k, vector_count)
 
         if vector_count == 0:
             return self.none()
@@ -25,22 +30,27 @@
         embeddings = np.frombuffer(b"".join(embeddings_list), dtype=np.float32).reshape(
             vector_count, -1
         )
 
         if vector_count < 10_000:
             index = BFIndex(
                 max_elements=vector_count,
-                dim=embeddings.shape[1],
+                dim=vectordb_settings.DEFAULT_EMBEDDING_DIMENSION,
+                space=vectordb_settings.DEFAULT_EMBEDDING_SPACE,
                 should_not_cache=True,
             )
             index.add(embeddings, ids=ids_list)
             labels, distances = index.search(query_embeddings, k)
         else:
             if manager.index is None:
-                manager.index = HNSWIndex(self.embedding_dim, max_elements=vector_count)
+                manager.index = HNSWIndex(
+                    max_elements=vector_count,
+                    dim=vectordb_settings.DEFAULT_EMBEDDING_DIMENSION,
+                    space=vectordb_settings.DEFAULT_EMBEDDING_SPACE,
+                )
                 manager.index.add(embeddings, ids=ids_list)
 
             labels, distances = manager.index.search(
                 query_embeddings, k, ids__in=ids_list
             )
         labels: list[int] = labels[0].tolist()
         distances: list[float] = distances[0].tolist()
@@ -57,21 +67,21 @@
                 default=models.Value(0.0),
                 output_field=models.FloatField(),
             )
         )
 
         return queryset.order_by("distance")
 
-    def related_text(self, text: str, k: int = 10):
+    def related_text(self, text: str, k: int | None = None):
         vectors = self
         ids_list = [vector.id for vector in vectors]
         query_embeddings = self.model.objects.embedding_fn([text])
         return self._get_related_vectors(query_embeddings, vectors, k, ids_list)
 
-    def related_objects(self, model_object, k=10):
+    def related_objects(self, model_object, k: int | None = None):
         content_type = ContentType.objects.get_for_model(model_object)
 
         if self.filter(content_type=content_type, object_id=model_object.id).exists():
             query_object = self.get(
                 content_type=content_type, object_id=model_object.id
             )
             query_embeddings = np.frombuffer(
@@ -82,21 +92,26 @@
 
         vectors = self.filter(content_type=content_type).exclude(
             object_id=model_object.id, content_type=content_type
         )
         ids_list = [vector.id for vector in vectors]
         return self._get_related_vectors(query_embeddings, vectors, k, ids_list)
 
-    def search(self, query, k=10):
+    def search(self, query, k: int | None = None):
         if isinstance(query, models.Model):
             start = time.time()
             results = self.related_objects(query, k=k)
+            results.search_time = time.time() - start
             logger.info(f"Search took {1000*(time.time() - start)}ms")
             return results
 
         if isinstance(query, str):
             start = time.time()
             results = self.related_text(query, k=k)
             logger.info(f"Search took  {1000*(time.time() - start)}ms")
+            results.search_time = time.time() - start
             return results
         else:
             raise ValueError("Query must be a model instance or string")
+
+    def related(self, *args, **kwargs):
+        return self.search(*args, **kwargs)
```

### Comparing `django-vectordb-0.1.0/vectordb/signals.py` & `django-vectordb-0.1.1/vectordb/signals.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/sync_signals.py` & `django-vectordb-0.1.1/vectordb/sync_signals.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/tasks.py` & `django-vectordb-0.1.1/vectordb/tasks.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/tests/settings.py` & `django-vectordb-0.1.1/vectordb/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/tests/test_api_endpoint.py` & `django-vectordb-0.1.1/vectordb/tests/test_api_endpoint.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/tests/test_db_indexes.py` & `django-vectordb-0.1.1/vectordb/tests/test_db_indexes.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/tests/test_embedding_functions.py` & `django-vectordb-0.1.1/vectordb/tests/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/tests/test_singleton_meta.py` & `django-vectordb-0.1.1/vectordb/tests/test_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/tests/test_vectordb.py` & `django-vectordb-0.1.1/vectordb/tests/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/utils.py` & `django-vectordb-0.1.1/vectordb/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import os
 import importlib
 from django.conf import settings
 from django.core.serializers import serialize
 from django.db import models
 import numpy as np
+from vectordb.settings import vectordb_settings
 
 
 from .validators import validate_vector_data
 
 try:
     import celery
     from . import tasks
@@ -23,20 +24,14 @@
 
 except ImportError:
     has_celery = False
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
-EMBEDDING_FN = getattr(settings, "EMBEDDING_FN", None)
-EMBEDDING_DIM = getattr(settings, "EMBEDDING_DIM", None)
-
-if EMBEDDING_FN is not None and EMBEDDING_DIM is None:
-    raise ValueError("EMBEDDING_FN is set but EMBEDDING_DIM is not set")
-
 
 def flatten_object_json(serialized_data):
     flattened_data = {}
 
     # Add the model and primary key information
     flattened_data["model"] = serialized_data["model"]
     flattened_data["pk"] = serialized_data["pk"]
@@ -115,26 +110,18 @@
     if embedding is not None and has_celery:
         embedding = tasks.create_vector.delay(text)
 
     return vector
 
 
 def get_embedding_function():
-    if EMBEDDING_FN is not None:
-        module_name, function_name = settings.EMBEDDING_FN.rsplit(".", 1)
-        module = importlib.import_module(module_name)
-        embedding_fn = getattr(module, function_name)
-    else:
-        from .embedding_functions import SentenceTransformerEncoder
-
-        embedding_dim = (
-            SentenceTransformerEncoder().model.get_sentence_embedding_dimension()
-        )
-
-        embedding_fn = SentenceTransformerEncoder()
+    embedding_fn = vectordb_settings.DEFAULT_EMBEDDING_CLASS(
+        model_name=vectordb_settings.DEFAULT_EMBEDDING_MODEL
+    )
+    embedding_dim = vectordb_settings.DEFAULT_EMBEDDING_DIMENSION
     return embedding_fn, embedding_dim
 
 
 def _populate_index(manager: models.Manager):
     vectors = manager.only("id", "embedding").all()
     vector_count = vectors.count()
```

### Comparing `django-vectordb-0.1.0/vectordb/validators.py` & `django-vectordb-0.1.1/vectordb/validators.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.0/vectordb/views.py` & `django-vectordb-0.1.1/vectordb/views.py`

 * *Files identical despite different names*

