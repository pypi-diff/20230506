# Comparing `tmp/django-scaffold-tools-0.0.8.tar.gz` & `tmp/django-scaffold-tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-scaffold-tools-0.0.8.tar", last modified: Sun Aug  2 16:18:22 2020, max compression
+gzip compressed data, was "dist/django-scaffold-tools-0.0.9.tar", last modified: Mon Aug  3 00:54:52 2020, max compression
```

## Comparing `django-scaffold-tools-0.0.8.tar` & `django-scaffold-tools-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,16 @@
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.327474 django-scaffold-tools-0.0.8/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)    11357 2020-08-01 09:14:06.000000 django-scaffold-tools-0.0.8/LICENSE
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      143 2020-08-02 14:47:31.000000 django-scaffold-tools-0.0.8/MANIFEST.in
--rw-rw-r--   0 alfred    (1000) alfred    (1000)     1831 2020-08-02 16:18:22.327474 django-scaffold-tools-0.0.8/PKG-INFO
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      599 2020-08-01 09:32:29.000000 django-scaffold-tools-0.0.8/README.rst
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.319474 django-scaffold-tools-0.0.8/docs/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        0 2020-08-01 09:38:46.000000 django-scaffold-tools-0.0.8/docs/.gitkeep
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      943 2020-08-02 16:18:22.327474 django-scaffold-tools-0.0.8/setup.cfg
--rw-rw-r--   0 alfred    (1000) alfred    (1000)     1200 2020-08-02 13:42:40.000000 django-scaffold-tools-0.0.8/setup.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.319474 django-scaffold-tools-0.0.8/src/
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.323474 django-scaffold-tools-0.0.8/src/django_scaffold_tools.egg-info/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)     1831 2020-08-02 16:18:22.000000 django-scaffold-tools-0.0.8/src/django_scaffold_tools.egg-info/PKG-INFO
--rw-rw-r--   0 alfred    (1000) alfred    (1000)     1362 2020-08-02 16:18:22.000000 django-scaffold-tools-0.0.8/src/django_scaffold_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        1 2020-08-02 16:18:22.000000 django-scaffold-tools-0.0.8/src/django_scaffold_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      183 2020-08-02 16:18:22.000000 django-scaffold-tools-0.0.8/src/django_scaffold_tools.egg-info/requires.txt
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        9 2020-08-02 16:18:22.000000 django-scaffold-tools-0.0.8/src/django_scaffold_tools.egg-info/top_level.txt
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.323474 django-scaffold-tools-0.0.8/src/scaffold/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        0 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/__init__.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.323474 django-scaffold-tools-0.0.8/src/scaffold/exceptions/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        0 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/exceptions/__init__.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      931 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/exceptions/exceptions.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      785 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/exceptions/middleware.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      439 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/exceptions/utils.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.323474 django-scaffold-tools-0.0.8/src/scaffold/models/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        0 2020-08-02 00:56:25.000000 django-scaffold-tools-0.0.8/src/scaffold/models/__init__.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.323474 django-scaffold-tools-0.0.8/src/scaffold/models/abstract/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        0 2020-08-02 00:56:49.000000 django-scaffold-tools-0.0.8/src/scaffold/models/abstract/__init__.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)     9880 2020-08-02 08:13:25.000000 django-scaffold-tools-0.0.8/src/scaffold/models/abstract/member.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)     7651 2020-08-02 01:11:41.000000 django-scaffold-tools-0.0.8/src/scaffold/models/abstract/meta.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.323474 django-scaffold-tools-0.0.8/src/scaffold/models/entity/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        0 2020-08-02 00:57:07.000000 django-scaffold-tools-0.0.8/src/scaffold/models/entity/__init__.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.323474 django-scaffold-tools-0.0.8/src/scaffold/models/entity/media/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        0 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/models/entity/media/__init__.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      179 2020-08-02 01:14:35.000000 django-scaffold-tools-0.0.8/src/scaffold/models/entity/media/admin.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      108 2020-08-02 01:15:17.000000 django-scaffold-tools-0.0.8/src/scaffold/models/entity/media/apps.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)     4159 2020-08-02 01:18:49.000000 django-scaffold-tools-0.0.8/src/scaffold/models/entity/media/models.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      413 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/models/entity/media/serializers.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)       60 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/models/entity/media/tests.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      438 2020-08-01 09:14:42.000000 django-scaffold-tools-0.0.8/src/scaffold/models/entity/media/views.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.327474 django-scaffold-tools-0.0.8/src/scaffold/modules/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)       39 2020-08-02 08:08:16.000000 django-scaffold-tools-0.0.8/src/scaffold/modules/__init__.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      189 2020-08-01 15:37:02.000000 django-scaffold-tools-0.0.8/src/scaffold/modules/apps.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      392 2020-08-01 15:40:51.000000 django-scaffold-tools-0.0.8/src/scaffold/modules/fullclean.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.327474 django-scaffold-tools-0.0.8/src/scaffold/restframework/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)        0 2020-08-01 12:43:45.000000 django-scaffold-tools-0.0.8/src/scaffold/restframework/__init__.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)      195 2020-08-01 15:38:58.000000 django-scaffold-tools-0.0.8/src/scaffold/restframework/apps.py
--rwxrwxr-x   0 alfred    (1000) alfred    (1000)      336 2020-08-01 15:47:28.000000 django-scaffold-tools-0.0.8/src/scaffold/restframework/authentication.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)    16673 2020-08-01 15:55:52.000000 django-scaffold-tools-0.0.8/src/scaffold/restframework/filters.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)     1485 2020-08-01 15:40:11.000000 django-scaffold-tools-0.0.8/src/scaffold/restframework/pagination.py
--rwxrwxr-x   0 alfred    (1000) alfred    (1000)      696 2020-08-01 15:44:38.000000 django-scaffold-tools-0.0.8/src/scaffold/restframework/permissions.py
-drwxrwxr-x   0 alfred    (1000) alfred    (1000)        0 2020-08-02 16:18:22.327474 django-scaffold-tools-0.0.8/src/scaffold/settings/
--rw-rw-r--   0 alfred    (1000) alfred    (1000)    11483 2020-08-02 08:14:58.000000 django-scaffold-tools-0.0.8/src/scaffold/settings/__init__.py
--rw-rw-r--   0 alfred    (1000) alfred    (1000)       18 2020-08-02 16:18:17.000000 django-scaffold-tools-0.0.8/src/scaffold/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-03 00:54:52.540724 django-scaffold-tools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2020-08-03 00:54:41.000000 django-scaffold-tools-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      143 2020-08-03 00:54:41.000000 django-scaffold-tools-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1831 2020-08-03 00:54:52.540724 django-scaffold-tools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      599 2020-08-03 00:54:41.000000 django-scaffold-tools-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-03 00:54:52.540724 django-scaffold-tools-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-08-03 00:54:41.000000 django-scaffold-tools-0.0.9/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2020-08-03 00:54:52.540724 django-scaffold-tools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1200 2020-08-03 00:54:41.000000 django-scaffold-tools-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-03 00:54:52.540724 django-scaffold-tools-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-03 00:54:52.540724 django-scaffold-tools-0.0.9/src/django_scaffold_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1831 2020-08-03 00:54:52.000000 django-scaffold-tools-0.0.9/src/django_scaffold_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      307 2020-08-03 00:54:52.000000 django-scaffold-tools-0.0.9/src/django_scaffold_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-03 00:54:52.000000 django-scaffold-tools-0.0.9/src/django_scaffold_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      190 2020-08-03 00:54:52.000000 django-scaffold-tools-0.0.9/src/django_scaffold_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-03 00:54:52.000000 django-scaffold-tools-0.0.9/src/django_scaffold_tools.egg-info/top_level.txt
```

### Comparing `django-scaffold-tools-0.0.8/LICENSE` & `django-scaffold-tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-scaffold-tools-0.0.8/PKG-INFO` & `django-scaffold-tools-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-scaffold-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A reusable django-app set for a DRF django project, starting support from django 3.0.
 Home-page: https://github.com/easecloud/django-scaffold-tools
 Author: Alfred Huang
 Author-email: 57082212@qq.com
 License: Apache License Version 2.0
 Description: =====================
         django-scaffold-tools
```

### Comparing `django-scaffold-tools-0.0.8/README.rst` & `django-scaffold-tools-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-scaffold-tools-0.0.8/setup.cfg` & `django-scaffold-tools-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-scaffold-tools-0.0.8/setup.py` & `django-scaffold-tools-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `django-scaffold-tools-0.0.8/src/django_scaffold_tools.egg-info/PKG-INFO` & `django-scaffold-tools-0.0.9/src/django_scaffold_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-scaffold-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A reusable django-app set for a DRF django project, starting support from django 3.0.
 Home-page: https://github.com/easecloud/django-scaffold-tools
 Author: Alfred Huang
 Author-email: 57082212@qq.com
 License: Apache License Version 2.0
 Description: =====================
         django-scaffold-tools
```

