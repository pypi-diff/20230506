# Comparing `tmp/base_system-0.2.3.tar.gz` & `tmp/base_system-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.2.3.tar", last modified: Sat May  6 02:27:33 2023, max compression
+gzip compressed data, was "base_system-0.2.4.tar", last modified: Sat May  6 02:46:02 2023, max compression
```

## Comparing `base_system-0.2.3.tar` & `base_system-0.2.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.770831 base_system-0.2.3/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.3/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.3/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.702796 base_system-0.2.3/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.3/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.3/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11803 2023-05-06 02:25:35.000000 base_system-0.2.3/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.3/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.3/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.3/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.3/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.3/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-06 02:27:33.770831 base_system-0.2.3/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.3/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.710800 base_system-0.2.3/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.3/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.750821 base_system-0.2.3/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.3/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.3/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.3/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.3/base_system/__pycache__/export_viewset.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19488 2023-05-04 08:07:15.000000 base_system-0.2.3/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    27590 2023-05-06 02:21:51.000000 base_system-0.2.3/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.3/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3179 2023-05-06 02:06:30.000000 base_system-0.2.3/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23682 2023-05-06 02:13:02.000000 base_system-0.2.3/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-06 01:27:33.000000 base_system-0.2.3/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.3/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.3/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.3/base_system/auth.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.3/base_system/export_viewset.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.762827 base_system-0.2.3/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.3/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.3/base_system/migrations/0002_drugdirectory_code_medu_cur.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.3/base_system/migrations/0003_alter_extragroup_hospital.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.3/base_system/migrations/0004_alter_extragroup_role_name.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.3/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.766829 base_system-0.2.3/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.3/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.3/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.3/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.3/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.3/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25535 2023-05-04 08:07:06.000000 base_system-0.2.3/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23694 2023-05-06 02:21:50.000000 base_system-0.2.3/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.3/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     4071 2023-05-06 02:06:28.000000 base_system-0.2.3/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    58056 2023-05-06 02:12:59.000000 base_system-0.2.3/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14978 2023-05-04 08:34:21.000000 base_system-0.2.3/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.726808 base_system-0.2.3/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1810 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.3/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.3/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.3/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.3/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.3/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-06 02:27:33.770831 base_system-0.2.3/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-06 02:06:28.000000 base_system-0.2.3/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.705841 base_system-0.2.4/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.4/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.4/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.585773 base_system-0.2.4/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.4/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.4/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11801 2023-05-06 02:43:22.000000 base_system-0.2.4/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.4/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.4/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.4/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.4/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.4/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-06 02:46:02.705841 base_system-0.2.4/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.4/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.653812 base_system-0.2.4/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.4/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.681828 base_system-0.2.4/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.4/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.4/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.4/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.4/base_system/__pycache__/export_viewset.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19488 2023-05-04 08:07:15.000000 base_system-0.2.4/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    27610 2023-05-06 02:44:00.000000 base_system-0.2.4/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.4/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3179 2023-05-06 02:06:30.000000 base_system-0.2.4/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23682 2023-05-06 02:13:02.000000 base_system-0.2.4/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-06 01:27:33.000000 base_system-0.2.4/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.4/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.4/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.4/base_system/auth.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.4/base_system/export_viewset.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.693834 base_system-0.2.4/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.4/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.4/base_system/migrations/0002_drugdirectory_code_medu_cur.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.4/base_system/migrations/0003_alter_extragroup_hospital.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.4/base_system/migrations/0004_alter_extragroup_role_name.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.4/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.701839 base_system-0.2.4/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.4/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.4/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.4/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.4/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.4/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25535 2023-05-04 08:07:06.000000 base_system-0.2.4/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23752 2023-05-06 02:43:58.000000 base_system-0.2.4/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.4/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     4071 2023-05-06 02:06:28.000000 base_system-0.2.4/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    58056 2023-05-06 02:12:59.000000 base_system-0.2.4/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14978 2023-05-04 08:34:21.000000 base_system-0.2.4/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.665819 base_system-0.2.4/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1810 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.4/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.4/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.4/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.4/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.4/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-06 02:46:02.705841 base_system-0.2.4/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-06 02:44:49.000000 base_system-0.2.4/setup.py
```

### Comparing `base_system-0.2.3/.gitignore` & `base_system-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/BaseFunctionModule/settings.py` & `base_system-0.2.4/BaseFunctionModule/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 WSGI_APPLICATION = 'BaseFunctionModule.wsgi.application'
 
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.postgresql_psycopg2',
-        'NAME': 'basicdb',
+        'NAME': 'aptdb',
         'USER': 'postgres',
         'PASSWORD': 'postgres',
         'HOST': 'localhost',
         'PORT': '5432'
     }
 }
```

### Comparing `base_system-0.2.3/BaseFunctionModule/urls.py` & `base_system-0.2.4/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/LICENCE` & `base_system-0.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/PKG-INFO` & `base_system-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.2.3
+Version: 0.2.4
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.3/README.rst` & `base_system-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/__pycache__/export_viewset.cpython-39.pyc` & `base_system-0.2.4/base_system/__pycache__/export_viewset.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.2.4/base_system/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/__pycache__/serializers.cpython-39.pyc` & `base_system-0.2.4/base_system/__pycache__/serializers.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat May  6 02:21:50 2023 UTC, .py size: 23694 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 beb9 5564 8e5c 0000  a.........Ud.\..
+00000000: 610d 0d0a 0000 0000 eebe 5564 c85c 0000  a.........Ud.\..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ce02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
@@ -1046,680 +1046,681 @@
 00004150: 6c69 7a65 722e 4d65 7461 721c 0000 004e  lizer.Metar....N
 00004160: 2906 721f 0000 0072 2000 0000 7221 0000  ).r....r ...r!..
 00004170: 0072 1800 0000 7222 0000 0072 2300 0000  .r....r"...r#...
 00004180: 7225 0000 0072 2500 0000 7225 0000 0072  r%...r%...r%...r
 00004190: 2600 0000 7227 0000 00e9 0100 0073 0400  &...r'.......s..
 000041a0: 0000 0801 0401 7227 0000 0063 0200 0000  ......r'...c....
 000041b0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
-000041c0: 4300 0000 7320 0000 0074 006a 016a 027c  C...s ...t.j.j.|
-000041d0: 0164 018d 017d 0274 037c 0264 0264 038d  .d...}.t.|.d.d..
-000041e0: 027d 037c 036a 0453 00a9 044e 2901 726c  .}.|.j.S...N).rl
-000041f0: 0000 0054 722f 0000 0029 0572 1800 0000  ...Tr/...).r....
-00004200: 725a 0000 0072 5c00 0000 72e9 0000 0072  rZ...r\...r....r
-00004210: 3300 0000 a904 7234 0000 0072 3500 0000  3.....r4...r5...
-00004220: 723b 0000 0072 3700 0000 7225 0000 0072  r;...r7...r%...r
-00004230: 2500 0000 7226 0000 0072 3800 0000 ed01  %...r&...r8.....
-00004240: 0000 7306 0000 0000 010e 010c 017a 2549  ..s..........z%I
-00004250: 6e73 7065 6374 696f 6e54 7970 6553 6572  nspectionTypeSer
-00004260: 6961 6c69 7a65 722e 6765 745f 6368 696c  ializer.get_chil
-00004270: 6472 656e 4e72 3900 0000 7225 0000 0072  drenNr9...r%...r
-00004280: 2500 0000 7225 0000 0072 2600 0000 72e9  %...r%...r&...r.
-00004290: 0000 00e4 0100 0073 0800 0000 0801 0402  .......s........
-000042a0: 0802 0e04 72e9 0000 0063 0000 0000 0000  ....r....c......
-000042b0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-000042c0: 0000 733e 0000 0065 005a 0164 005a 0264  ..s>...e.Z.d.Z.d
-000042d0: 015a 0365 04a0 05a1 005a 0665 04a0 05a1  .Z.e.....Z.e....
-000042e0: 005a 0747 0064 0264 0384 0064 0383 025a  .Z.G.d.d...d...Z
-000042f0: 0864 0464 0584 005a 0964 0664 0784 005a  .d.d...Z.d.d...Z
-00004300: 0a64 0853 0029 09da 2049 6e73 7065 6374  .d.S.).. Inspect
-00004310: 696f 6e44 6963 7469 6f6e 6172 6965 7353  ionDictionariesS
-00004320: 6572 6961 6c69 7a65 7275 1800 0000 e6a3  erializeru......
-00004330: 80e6 9fa5 e5ad 97e5 85b8 e5ba 8fe5 8897  ................
-00004340: e58c 96e5 99a8 6300 0000 0000 0000 0000  ......c.........
-00004350: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-00004360: 1400 0000 6500 5a01 6400 5a02 6503 5a04  ....e.Z.d.Z.e.Z.
-00004370: 6401 5a05 6402 5300 2903 7a25 496e 7370  d.Z.d.S.).z%Insp
-00004380: 6563 7469 6f6e 4469 6374 696f 6e61 7269  ectionDictionari
-00004390: 6573 5365 7269 616c 697a 6572 2e4d 6574  esSerializer.Met
-000043a0: 6172 1c00 0000 4ea9 0672 1f00 0000 7220  ar....N..r....r 
-000043b0: 0000 0072 2100 0000 720c 0000 0072 2200  ...r!...r....r".
-000043c0: 0000 7223 0000 0072 2500 0000 7225 0000  ..r#...r%...r%..
-000043d0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-000043e0: f801 0000 7304 0000 0008 0104 0172 2700  ....s........r'.
-000043f0: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00004400: 0000 0003 0000 0043 0000 0073 2200 0000  .......C...s"...
-00004410: 7400 6a01 6a02 7c01 6a03 6401 8d01 a004  t.j.j.|.j.d.....
-00004420: a100 7d02 7c02 721e 7c02 6a05 5300 6400  ..}.|.r.|.j.S.d.
-00004430: 5300 a902 4e29 0172 a900 0000 a906 7206  S...N).r......r.
-00004440: 0000 0072 5a00 0000 725c 0000 0072 ce00  ...rZ...r\...r..
-00004450: 0000 7246 0000 0072 7600 0000 72da 0000  ..rF...rv...r...
-00004460: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00004470: 72c3 0000 00fc 0100 0073 0600 0000 0001  r........s......
-00004480: 1401 0401 7a32 496e 7370 6563 7469 6f6e  ....z2Inspection
-00004490: 4469 6374 696f 6e61 7269 6573 5365 7269  DictionariesSeri
-000044a0: 616c 697a 6572 2e67 6574 5f68 6f73 7069  alizer.get_hospi
-000044b0: 7461 6c5f 6e61 6d65 6302 0000 0000 0000  tal_namec.......
-000044c0: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
-000044d0: 0073 2200 0000 7400 6a01 6a02 7c01 6a03  .s"...t.j.j.|.j.
-000044e0: 6401 8d01 a004 a100 7d02 7c02 721e 7c02  d.......}.|.r.|.
-000044f0: 6a05 5300 6400 5300 72ee 0000 00a9 0672  j.S.d.S.r......r
-00004500: 0700 0000 725a 0000 0072 5c00 0000 72cc  ....rZ...r\...r.
-00004510: 0000 0072 4600 0000 7276 0000 0072 db00  ...rF...rv...r..
-00004520: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
-00004530: 0072 bf00 0000 0102 0000 7306 0000 0000  .r........s.....
-00004540: 0114 0104 017a 3049 6e73 7065 6374 696f  .....z0Inspectio
-00004550: 6e44 6963 7469 6f6e 6172 6965 7353 6572  nDictionariesSer
-00004560: 6961 6c69 7a65 722e 6765 745f 6f66 6669  ializer.get_offi
-00004570: 6365 5f6e 616d 654e a90b 721f 0000 0072  ce_nameN..r....r
-00004580: 2000 0000 7221 0000 0072 2900 0000 7205   ...r!...r)...r.
-00004590: 0000 0072 3a00 0000 72cf 0000 0072 cd00  ...r:...r....r..
-000045a0: 0000 7227 0000 0072 c300 0000 72bf 0000  ..r'...r....r...
-000045b0: 0072 2500 0000 7225 0000 0072 2500 0000  .r%...r%...r%...
-000045c0: 7226 0000 0072 ec00 0000 f301 0000 730c  r&...r........s.
-000045d0: 0000 0008 0104 0108 0108 020e 0408 0572  ...............r
-000045e0: ec00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000045f0: 0000 0000 0003 0000 0040 0000 0073 4600  .........@...sF.
-00004600: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
-00004610: 6a05 6402 6403 8d01 5a06 6504 6a05 6404  j.d.d...Z.e.j.d.
-00004620: 6403 8d01 5a07 4700 6405 6406 8400 6406  d...Z.G.d.d...d.
-00004630: 8302 5a08 6407 6408 8400 5a09 6409 640a  ..Z.d.d...Z.d.d.
-00004640: 8400 5a0a 640b 5300 290c da26 4578 706f  ..Z.d.S.)..&Expo
-00004650: 7274 496e 7370 6563 7469 6f6e 4469 6374  rtInspectionDict
-00004660: 696f 6e61 7269 6573 5365 7269 616c 697a  ionariesSerializ
-00004670: 6572 751e 0000 00e5 afbc e587 bae6 a380  eru.............
-00004680: e69f a5e5 ad97 e585 b8e5 ba8f e588 97e5  ................
-00004690: 8c96 e599 a872 d100 0000 72a7 0000 0072  .....r....r....r
-000046a0: d400 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000046b0: 0000 0000 0001 0000 0040 0000 0073 1400  .........@...s..
-000046c0: 0000 6500 5a01 6400 5a02 6503 5a04 6401  ..e.Z.d.Z.e.Z.d.
-000046d0: 5a05 6402 5300 2903 7a2b 4578 706f 7274  Z.d.S.).z+Export
-000046e0: 496e 7370 6563 7469 6f6e 4469 6374 696f  InspectionDictio
-000046f0: 6e61 7269 6573 5365 7269 616c 697a 6572  nariesSerializer
-00004700: 2e4d 6574 61a9 08da 0c70 726f 6a65 6374  .Meta....project
-00004710: 5f63 6f64 65da 0c70 726f 6a65 6374 5f6e  _code..project_n
-00004720: 616d 6572 cf00 0000 72cd 0000 00da 0c70  amer....r......p
-00004730: 726f 6a65 6374 5f66 6565 73da 0a63 6f64  roject_fees..cod
-00004740: 655f 7372 7674 70da 0a6e 616d 655f 7372  e_srvtp..name_sr
-00004750: 7674 70da 0772 656d 6172 6b73 4e72 ed00  vtp..remarksNr..
-00004760: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
-00004770: 0072 2600 0000 7227 0000 000c 0200 0073  .r&...r'.......s
-00004780: 0400 0000 0801 0401 7227 0000 0063 0200  ........r'...c..
-00004790: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-000047a0: 0000 4300 0000 7322 0000 0074 006a 016a  ..C...s"...t.j.j
-000047b0: 027c 016a 0364 018d 01a0 04a1 007d 027c  .|.j.d.......}.|
-000047c0: 0272 1e7c 026a 0553 0064 0053 0072 ee00  .r.|.j.S.d.S.r..
-000047d0: 0000 72ef 0000 0072 da00 0000 7225 0000  ..r....r....r%..
-000047e0: 0072 2500 0000 7226 0000 0072 c300 0000  .r%...r&...r....
-000047f0: 1902 0000 7306 0000 0000 0114 0104 017a  ....s..........z
-00004800: 3845 7870 6f72 7449 6e73 7065 6374 696f  8ExportInspectio
-00004810: 6e44 6963 7469 6f6e 6172 6965 7353 6572  nDictionariesSer
-00004820: 6961 6c69 7a65 722e 6765 745f 686f 7370  ializer.get_hosp
-00004830: 6974 616c 5f6e 616d 6563 0200 0000 0000  ital_namec......
-00004840: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00004850: 0000 7322 0000 0074 006a 016a 027c 016a  ..s"...t.j.j.|.j
-00004860: 0364 018d 01a0 04a1 007d 027c 0272 1e7c  .d.......}.|.r.|
-00004870: 026a 0553 0064 0053 0072 ee00 0000 72f0  .j.S.d.S.r....r.
-00004880: 0000 0072 db00 0000 7225 0000 0072 2500  ...r....r%...r%.
-00004890: 0000 7226 0000 0072 bf00 0000 1e02 0000  ..r&...r........
-000048a0: 7306 0000 0000 0114 0104 017a 3645 7870  s..........z6Exp
-000048b0: 6f72 7449 6e73 7065 6374 696f 6e44 6963  ortInspectionDic
-000048c0: 7469 6f6e 6172 6965 7353 6572 6961 6c69  tionariesSeriali
-000048d0: 7a65 722e 6765 745f 6f66 6669 6365 5f6e  zer.get_office_n
-000048e0: 616d 654e 72f1 0000 0072 2500 0000 7225  ameNr....r%...r%
-000048f0: 0000 0072 2500 0000 7226 0000 0072 f200  ...r%...r&...r..
-00004900: 0000 0702 0000 730c 0000 0008 0104 010c  ......s.........
-00004910: 010c 020e 0d08 0572 f200 0000 6300 0000  .......r....c...
-00004920: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00004930: 0040 0000 0073 2e00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00004940: 5a02 6401 5a03 6504 a005 a100 5a06 4700  Z.d.Z.e.....Z.G.
-00004950: 6402 6403 8400 6403 8302 5a07 6404 6405  d.d...d...Z.d.d.
-00004960: 8400 5a08 6406 5300 2907 da19 4578 616d  ..Z.d.S.)...Exam
-00004970: 696e 6174 696f 6e54 7970 6553 6572 6961  inationTypeSeria
-00004980: 6c69 7a65 7275 1e00 0000 e6a3 80e9 aa8c  lizeru..........
-00004990: e5ad 97e5 85b8 e7b1 bbe5 9e8b e5ba 8fe5  ................
-000049a0: 8897 e58c 96e5 99a8 6300 0000 0000 0000  ........c.......
-000049b0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-000049c0: 0073 1400 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
-000049d0: 5a04 6401 5a05 6402 5300 2903 7a1e 4578  Z.d.Z.d.S.).z.Ex
-000049e0: 616d 696e 6174 696f 6e54 7970 6553 6572  aminationTypeSer
-000049f0: 6961 6c69 7a65 722e 4d65 7461 721c 0000  ializer.Metar...
-00004a00: 004e 2906 721f 0000 0072 2000 0000 7221  .N).r....r ...r!
-00004a10: 0000 0072 1700 0000 7222 0000 0072 2300  ...r....r"...r#.
-00004a20: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
-00004a30: 0072 2600 0000 7227 0000 0028 0200 0073  .r&...r'...(...s
-00004a40: 0400 0000 0801 0401 7227 0000 0063 0200  ........r'...c..
-00004a50: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00004a60: 0000 4300 0000 7320 0000 0074 006a 016a  ..C...s ...t.j.j
-00004a70: 027c 0164 018d 017d 0274 037c 0264 0264  .|.d...}.t.|.d.d
-00004a80: 038d 027d 037c 036a 0453 0072 ea00 0000  ...}.|.j.S.r....
-00004a90: 2905 7217 0000 0072 5a00 0000 725c 0000  ).r....rZ...r\..
-00004aa0: 0072 fa00 0000 7233 0000 0072 eb00 0000  .r....r3...r....
-00004ab0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-00004ac0: 3800 0000 2c02 0000 7306 0000 0000 010e  8...,...s.......
-00004ad0: 010c 017a 2645 7861 6d69 6e61 7469 6f6e  ...z&Examination
-00004ae0: 5479 7065 5365 7269 616c 697a 6572 2e67  TypeSerializer.g
-00004af0: 6574 5f63 6869 6c64 7265 6e4e 7239 0000  et_childrenNr9..
-00004b00: 0072 2500 0000 7225 0000 0072 2500 0000  .r%...r%...r%...
-00004b10: 7226 0000 0072 fa00 0000 2402 0000 7308  r&...r....$...s.
-00004b20: 0000 0008 0104 0108 020e 0472 fa00 0000  ...........r....
-00004b30: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00004b40: 0003 0000 0040 0000 0073 3e00 0000 6500  .....@...s>...e.
-00004b50: 5a01 6400 5a02 6401 5a03 6504 a005 a100  Z.d.Z.d.Z.e.....
-00004b60: 5a06 6504 a005 a100 5a07 4700 6402 6403  Z.e.....Z.G.d.d.
-00004b70: 8400 6403 8302 5a08 6404 6405 8400 5a09  ..d...Z.d.d...Z.
-00004b80: 6406 6407 8400 5a0a 6408 5300 2909 da21  d.d...Z.d.S.)..!
-00004b90: 4578 616d 696e 6174 696f 6e44 6963 7469  ExaminationDicti
-00004ba0: 6f6e 6172 6965 7353 6572 6961 6c69 7a65  onariesSerialize
-00004bb0: 7275 1800 0000 e6a3 80e9 aa8c e5ad 97e5  ru..............
-00004bc0: 85b8 e5ba 8fe5 8897 e58c 96e5 99a8 6300  ..............c.
-00004bd0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00004be0: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
-00004bf0: 6400 5a02 6503 5a04 6401 5a05 6402 5300  d.Z.e.Z.d.Z.d.S.
-00004c00: 2903 7a26 4578 616d 696e 6174 696f 6e44  ).z&ExaminationD
-00004c10: 6963 7469 6f6e 6172 6965 7353 6572 6961  ictionariesSeria
-00004c20: 6c69 7a65 722e 4d65 7461 721c 0000 004e  lizer.Metar....N
-00004c30: a906 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00004c40: 0072 0d00 0000 7222 0000 0072 2300 0000  .r....r"...r#...
-00004c50: 7225 0000 0072 2500 0000 7225 0000 0072  r%...r%...r%...r
-00004c60: 2600 0000 7227 0000 0037 0200 0073 0400  &...r'...7...s..
-00004c70: 0000 0801 0401 7227 0000 0063 0200 0000  ......r'...c....
-00004c80: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00004c90: 4300 0000 7322 0000 0074 006a 016a 027c  C...s"...t.j.j.|
-00004ca0: 016a 0364 018d 01a0 04a1 007d 027c 0272  .j.d.......}.|.r
-00004cb0: 1e7c 026a 0553 0064 0053 0072 ee00 0000  .|.j.S.d.S.r....
-00004cc0: 72ef 0000 0072 da00 0000 7225 0000 0072  r....r....r%...r
-00004cd0: 2500 0000 7226 0000 0072 c300 0000 3b02  %...r&...r....;.
-00004ce0: 0000 7306 0000 0000 0114 0104 017a 3345  ..s..........z3E
-00004cf0: 7861 6d69 6e61 7469 6f6e 4469 6374 696f  xaminationDictio
-00004d00: 6e61 7269 6573 5365 7269 616c 697a 6572  nariesSerializer
-00004d10: 2e67 6574 5f68 6f73 7069 7461 6c5f 6e61  .get_hospital_na
-00004d20: 6d65 6302 0000 0000 0000 0000 0000 0003  mec.............
-00004d30: 0000 0003 0000 0043 0000 0073 2200 0000  .......C...s"...
-00004d40: 7400 6a01 6a02 7c01 6a03 6401 8d01 a004  t.j.j.|.j.d.....
-00004d50: a100 7d02 7c02 721e 7c02 6a05 5300 6400  ..}.|.r.|.j.S.d.
-00004d60: 5300 72ee 0000 0072 f000 0000 72db 0000  S.r....r....r...
-00004d70: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00004d80: 72bf 0000 0040 0200 0073 0600 0000 0001  r....@...s......
-00004d90: 1401 0401 7a31 4578 616d 696e 6174 696f  ....z1Examinatio
-00004da0: 6e44 6963 7469 6f6e 6172 6965 7353 6572  nDictionariesSer
-00004db0: 6961 6c69 7a65 722e 6765 745f 6f66 6669  ializer.get_offi
-00004dc0: 6365 5f6e 616d 654e 72f1 0000 0072 2500  ce_nameNr....r%.
-00004dd0: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
-00004de0: 0072 fb00 0000 3202 0000 730c 0000 0008  .r....2...s.....
-00004df0: 0104 0108 0108 020e 0408 0572 fb00 0000  ...........r....
-00004e00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00004e10: 0003 0000 0040 0000 0073 4600 0000 6500  .....@...sF...e.
-00004e20: 5a01 6400 5a02 6401 5a03 6504 6a05 6402  Z.d.Z.d.Z.e.j.d.
-00004e30: 6403 8d01 5a06 6504 6a05 6404 6403 8d01  d...Z.e.j.d.d...
-00004e40: 5a07 4700 6405 6406 8400 6406 8302 5a08  Z.G.d.d...d...Z.
-00004e50: 6407 6408 8400 5a09 6409 640a 8400 5a0a  d.d...Z.d.d...Z.
-00004e60: 640b 5300 290c da27 4578 706f 7274 4578  d.S.)..'ExportEx
-00004e70: 616d 696e 6174 696f 6e44 6963 7469 6f6e  aminationDiction
-00004e80: 6172 6965 7353 6572 6961 6c69 7a65 7275  ariesSerializeru
-00004e90: 1e00 0000 e5af bce5 87ba e6a3 80e9 aa8c  ................
-00004ea0: e5ad 97e5 85b8 e5ba 8fe5 8897 e58c 96e5  ................
-00004eb0: 99a8 72d1 0000 0072 a700 0000 72d4 0000  ..r....r....r...
-00004ec0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00004ed0: 0000 0100 0000 4000 0000 7314 0000 0065  ......@...s....e
-00004ee0: 005a 0164 005a 0265 035a 0464 015a 0564  .Z.d.Z.e.Z.d.Z.d
-00004ef0: 0253 0029 037a 2c45 7870 6f72 7445 7861  .S.).z,ExportExa
-00004f00: 6d69 6e61 7469 6f6e 4469 6374 696f 6e61  minationDictiona
-00004f10: 7269 6573 5365 7269 616c 697a 6572 2e4d  riesSerializer.M
-00004f20: 6574 6172 f300 0000 4e72 fc00 0000 7225  etar....Nr....r%
-00004f30: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00004f40: 0000 7227 0000 004b 0200 0073 0400 0000  ..r'...K...s....
-00004f50: 0801 0401 7227 0000 0063 0200 0000 0000  ....r'...c......
-00004f60: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00004f70: 0000 7322 0000 0074 006a 016a 027c 016a  ..s"...t.j.j.|.j
-00004f80: 0364 018d 01a0 04a1 007d 027c 0272 1e7c  .d.......}.|.r.|
-00004f90: 026a 0553 0064 0053 0072 ee00 0000 72ef  .j.S.d.S.r....r.
-00004fa0: 0000 0072 da00 0000 7225 0000 0072 2500  ...r....r%...r%.
-00004fb0: 0000 7226 0000 0072 c300 0000 5802 0000  ..r&...r....X...
-00004fc0: 7306 0000 0000 0114 0104 017a 3945 7870  s..........z9Exp
-00004fd0: 6f72 7445 7861 6d69 6e61 7469 6f6e 4469  ortExaminationDi
-00004fe0: 6374 696f 6e61 7269 6573 5365 7269 616c  ctionariesSerial
-00004ff0: 697a 6572 2e67 6574 5f68 6f73 7069 7461  izer.get_hospita
-00005000: 6c5f 6e61 6d65 6302 0000 0000 0000 0000  l_namec.........
-00005010: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-00005020: 2200 0000 7400 6a01 6a02 7c01 6a03 6401  "...t.j.j.|.j.d.
-00005030: 8d01 a004 a100 7d02 7c02 721e 7c02 6a05  ......}.|.r.|.j.
-00005040: 5300 6400 5300 72ee 0000 0072 f000 0000  S.d.S.r....r....
-00005050: 72db 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
-00005060: 2600 0000 72bf 0000 005d 0200 0073 0600  &...r....]...s..
-00005070: 0000 0001 1401 0401 7a37 4578 706f 7274  ........z7Export
-00005080: 4578 616d 696e 6174 696f 6e44 6963 7469  ExaminationDicti
-00005090: 6f6e 6172 6965 7353 6572 6961 6c69 7a65  onariesSerialize
-000050a0: 722e 6765 745f 6f66 6669 6365 5f6e 616d  r.get_office_nam
-000050b0: 654e 72f1 0000 0072 2500 0000 7225 0000  eNr....r%...r%..
-000050c0: 0072 2500 0000 7226 0000 0072 fd00 0000  .r%...r&...r....
-000050d0: 4602 0000 730c 0000 0008 0104 010c 010c  F...s...........
-000050e0: 020e 0d08 0572 fd00 0000 6300 0000 0000  .....r....c.....
-000050f0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00005100: 0000 0073 5a00 0000 6500 5a01 6400 5a02  ...sZ...e.Z.d.Z.
-00005110: 6401 5a03 6504 6a05 6402 6403 8d01 5a06  d.Z.e.j.d.d...Z.
-00005120: 6504 6a05 6404 6403 8d01 5a07 6504 6a05  e.j.d.d...Z.e.j.
-00005130: 6405 6403 8d01 5a08 4700 6406 6407 8400  d.d...Z.G.d.d...
-00005140: 6407 8302 5a09 6408 6409 8400 5a0a 640a  d...Z.d.d...Z.d.
-00005150: 640b 8400 5a0b 640c 640d 8400 5a0c 640e  d...Z.d.d...Z.d.
-00005160: 5300 290f da1d 4578 706f 7274 4472 7567  S.)...ExportDrug
-00005170: 4469 7265 6374 6f72 7953 6572 6961 6c69  DirectorySeriali
-00005180: 7a65 72f5 1e00 0000 e5af bce5 87ba e88d  zer.............
-00005190: afe5 9381 e79b aee5 bd95 e5ba 8fe5 8897  ................
-000051a0: e58c 96e5 99a8 f50c 0000 00e5 88b6 e589  ................
-000051b0: 82e7 b1bb e59e 8b72 a700 0000 f506 0000  .......r........
-000051c0: 00e5 8886 e7b1 bbf5 0c00 0000 e88d afe5  ................
-000051d0: 9381 e7b1 bbe5 9e8b 6300 0000 0000 0000  ........c.......
-000051e0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-000051f0: 0073 1400 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
-00005200: 5a04 6401 5a05 6402 5300 2903 7a22 4578  Z.d.Z.d.S.).z"Ex
-00005210: 706f 7274 4472 7567 4469 7265 6374 6f72  portDrugDirector
-00005220: 7953 6572 6961 6c69 7a65 722e 4d65 7461  ySerializer.Meta
-00005230: 2913 da09 6472 7567 5f63 6f64 65da 0964  )...drug_code..d
-00005240: 7275 675f 6e61 6d65 da09 7374 616e 6461  rug_name..standa
-00005250: 7264 73da 0575 6e69 7473 da15 7072 6570  rds..units..prep
-00005260: 6172 6174 696f 6e5f 7479 7065 5f6e 616d  aration_type_nam
-00005270: 65da 0e64 7275 675f 7479 7065 5f6e 616d  e..drug_type_nam
-00005280: 65da 0d63 6174 6567 6f72 795f 6e61 6d65  e..category_name
-00005290: da0c 6f72 6967 696e 5f70 6c61 6365 da0c  ..origin_place..
-000052a0: 6d61 6e75 6661 6374 7572 6572 da09 756e  manufacturer..un
-000052b0: 6974 5f64 6f73 65da 0c6d 6561 7375 7265  it_dose..measure
-000052c0: 5f75 6e69 74da 0a73 746f 636b 5f6c 6566  _unit..stock_lef
-000052d0: 74da 0a73 746f 636b 5f75 6e69 74da 036d  t..stock_unit..m
-000052e0: 6963 da0c 7263 635f 6361 7465 676f 7279  ic..rcc_category
-000052f0: da0c 6973 5f65 7373 656e 7469 616c da08  ..is_essential..
-00005300: 6872 5f6c 6576 656c da07 6762 5f63 6f64  hr_level..gb_cod
-00005310: 65da 0767 625f 6e61 6d65 4ea9 0672 1f00  e..gb_nameN..r..
-00005320: 0000 7220 0000 0072 2100 0000 720e 0000  ..r ...r!...r...
-00005330: 0072 2200 0000 7223 0000 0072 2500 0000  .r"...r#...r%...
-00005340: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-00005350: 2700 0000 6a02 0000 7304 0000 0008 0104  '...j...s.......
-00005360: 0172 2700 0000 6302 0000 0000 0000 0000  .r'...c.........
-00005370: 0000 0003 0000 0001 0000 0043 0000 0073  ...........C...s
-00005380: 1400 0000 7c01 6a00 7d02 7c02 7210 7c02  ....|.j.}.|.r.|.
-00005390: 6a01 5300 6400 5300 724a 0000 00a9 02da  j.S.d.S.rJ......
-000053a0: 1070 7265 7061 7261 7469 6f6e 5f74 7970  .preparation_typ
-000053b0: 65da 0974 7970 655f 6e61 6d65 a903 7234  e..type_name..r4
-000053c0: 0000 0072 3500 0000 7218 0100 0072 2500  ...r5...r....r%.
-000053d0: 0000 7225 0000 0072 2600 0000 da19 6765  ..r%...r&.....ge
-000053e0: 745f 7072 6570 6172 6174 696f 6e5f 7479  t_preparation_ty
-000053f0: 7065 5f6e 616d 6582 0200 0073 0600 0000  pe_name....s....
-00005400: 0001 0601 0401 7a37 4578 706f 7274 4472  ......z7ExportDr
-00005410: 7567 4469 7265 6374 6f72 7953 6572 6961  ugDirectorySeria
-00005420: 6c69 7a65 722e 6765 745f 7072 6570 6172  lizer.get_prepar
-00005430: 6174 696f 6e5f 7479 7065 5f6e 616d 6563  ation_type_namec
-00005440: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00005450: 0100 0000 4300 0000 7314 0000 007c 016a  ....C...s....|.j
-00005460: 007d 027c 0272 107c 026a 0153 0064 0053  .}.|.r.|.j.S.d.S
-00005470: 0072 4a00 0000 a902 da08 6361 7465 676f  .rJ.......catego
-00005480: 7279 7209 0100 00a9 0372 3400 0000 7235  ryr......r4...r5
-00005490: 0000 0072 1d01 0000 7225 0000 0072 2500  ...r....r%...r%.
-000054a0: 0000 7226 0000 00da 1167 6574 5f63 6174  ..r&.....get_cat
-000054b0: 6567 6f72 795f 6e61 6d65 8702 0000 7306  egory_name....s.
-000054c0: 0000 0000 0106 0104 017a 2f45 7870 6f72  .........z/Expor
-000054d0: 7444 7275 6744 6972 6563 746f 7279 5365  tDrugDirectorySe
-000054e0: 7269 616c 697a 6572 2e67 6574 5f63 6174  rializer.get_cat
-000054f0: 6567 6f72 795f 6e61 6d65 6302 0000 0000  egory_namec.....
-00005500: 0000 0000 0000 0003 0000 0001 0000 0043  ...............C
-00005510: 0000 0073 1400 0000 7c01 6a00 7d02 7c02  ...s....|.j.}.|.
-00005520: 7210 7c02 6a01 5300 6400 5300 724a 0000  r.|.j.S.d.S.rJ..
-00005530: 00a9 02da 0964 7275 675f 7479 7065 7276  .....drug_typerv
-00005540: 0000 00a9 0372 3400 0000 7235 0000 0072  .....r4...r5...r
-00005550: 2101 0000 7225 0000 0072 2500 0000 7226  !...r%...r%...r&
-00005560: 0000 00da 1267 6574 5f64 7275 675f 7479  .....get_drug_ty
-00005570: 7065 5f6e 616d 658c 0200 0073 0600 0000  pe_name....s....
-00005580: 0001 0601 0401 7a30 4578 706f 7274 4472  ......z0ExportDr
-00005590: 7567 4469 7265 6374 6f72 7953 6572 6961  ugDirectorySeria
-000055a0: 6c69 7a65 722e 6765 745f 6472 7567 5f74  lizer.get_drug_t
-000055b0: 7970 655f 6e61 6d65 4e29 0d72 1f00 0000  ype_nameN).r....
-000055c0: 7220 0000 0072 2100 0000 7229 0000 0072  r ...r!...r)...r
-000055d0: 0500 0000 723a 0000 0072 0701 0000 7209  ....r:...r....r.
-000055e0: 0100 0072 0801 0000 7227 0000 0072 1b01  ...r....r'...r..
-000055f0: 0000 721f 0100 0072 2301 0000 7225 0000  ..r....r#...r%..
-00005600: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00005610: 72fe 0000 0063 0200 0073 1000 0000 0801  r....c...s......
-00005620: 0402 0c01 0c01 0c02 0e18 0805 0805 72fe  ..............r.
-00005630: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00005640: 0000 0000 0300 0000 4000 0000 732e 0000  ........@...s...
-00005650: 0065 005a 0164 005a 0264 015a 0365 04a0  .e.Z.d.Z.d.Z.e..
-00005660: 05a1 005a 0647 0064 0264 0384 0064 0383  ...Z.G.d.d...d..
-00005670: 025a 0764 0464 0584 005a 0864 0653 0029  .Z.d.d...Z.d.S.)
-00005680: 07da 1c50 6861 726d 6163 794d 616e 6167  ...PharmacyManag
-00005690: 656d 656e 7453 6572 6961 6c69 7a65 7275  ementSerializeru
-000056a0: 1800 0000 e88d afe6 88bf e7ae a1e7 9086  ................
-000056b0: e5ba 8fe5 8897 e58c 96e5 99a8 6300 0000  ............c...
-000056c0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-000056d0: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-000056e0: 5a02 6503 5a04 6401 5a05 6402 5a06 6403  Z.e.Z.d.Z.d.Z.d.
-000056f0: 5300 2904 7a21 5068 6172 6d61 6379 4d61  S.).z!PharmacyMa
-00005700: 6e61 6765 6d65 6e74 5365 7269 616c 697a  nagementSerializ
-00005710: 6572 2e4d 6574 6129 06da 0d70 6861 726d  er.Meta)...pharm
-00005720: 6163 795f 636f 6465 da0d 7068 6172 6d61  acy_code..pharma
-00005730: 6379 5f6e 616d 65da 0d70 6861 726d 6163  cy_name..pharmac
-00005740: 795f 7479 7065 72aa 0000 00da 0b62 656c  y_typer......bel
-00005750: 6f6e 675f 756e 6974 72e4 0000 00e9 0200  ong_unitr.......
-00005760: 0000 4e29 0772 1f00 0000 7220 0000 0072  ..N).r....r ...r
-00005770: 2100 0000 7211 0000 0072 2200 0000 7223  !...r....r"...r#
-00005780: 0000 00da 0564 6570 7468 7225 0000 0072  .....depthr%...r
-00005790: 2500 0000 7225 0000 0072 2600 0000 7227  %...r%...r&...r'
-000057a0: 0000 0096 0200 0073 0600 0000 0801 0401  .......s........
-000057b0: 0408 7227 0000 0063 0200 0000 0000 0000  ..r'...c........
-000057c0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-000057d0: 732c 0000 007c 016a 006a 0164 016b 0272  s,...|.j.j.d.k.r
-000057e0: 147c 016a 026a 0353 007c 016a 006a 0164  .|.j.j.S.|.j.j.d
-000057f0: 026b 0272 287c 016a 046a 0353 0064 0053  .k.r(|.j.j.S.d.S
-00005800: 0029 034e 7281 0000 0072 2901 0000 2905  .).Nr....r)...).
-00005810: 7227 0100 0072 3f00 0000 72c0 0000 0072  r'...r?...r....r
-00005820: 7600 0000 da0a 656e 7465 7270 7269 7365  v.....enterprise
-00005830: 7284 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
-00005840: 2600 0000 da0f 6765 745f 6265 6c6f 6e67  &.....get_belong
-00005850: 5f75 6e69 74a2 0200 0073 0800 0000 0001  _unit....s......
-00005860: 0c01 0801 0c01 7a2c 5068 6172 6d61 6379  ......z,Pharmacy
-00005870: 4d61 6e61 6765 6d65 6e74 5365 7269 616c  ManagementSerial
-00005880: 697a 6572 2e67 6574 5f62 656c 6f6e 675f  izer.get_belong_
-00005890: 756e 6974 4e29 0972 1f00 0000 7220 0000  unitN).r....r ..
-000058a0: 0072 2100 0000 7229 0000 0072 0500 0000  .r!...r)...r....
-000058b0: 723a 0000 0072 2801 0000 7227 0000 0072  r:...r(...r'...r
-000058c0: 2c01 0000 7225 0000 0072 2500 0000 7225  ,...r%...r%...r%
-000058d0: 0000 0072 2600 0000 7224 0100 0092 0200  ...r&...r$......
-000058e0: 0073 0800 0000 0801 0401 0802 0e0c 7224  .s............r$
-000058f0: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
-00005900: 0000 0000 0300 0000 4000 0000 7396 0000  ........@...s...
-00005910: 0065 005a 0164 005a 0264 015a 0365 046a  .e.Z.d.Z.d.Z.e.j
-00005920: 0564 0264 038d 015a 0665 046a 0564 0464  .d.d...Z.e.j.d.d
-00005930: 038d 015a 0765 046a 0564 0564 038d 015a  ...Z.e.j.d.d...Z
-00005940: 0865 046a 0564 0664 038d 015a 0965 046a  .e.j.d.d...Z.e.j
-00005950: 0564 0764 038d 015a 0a65 046a 0564 0864  .d.d...Z.e.j.d.d
-00005960: 038d 015a 0b47 0064 0964 0a84 0064 0a83  ...Z.G.d.d...d..
-00005970: 025a 0c64 0b64 0c84 005a 0d64 0d64 0e84  .Z.d.d...Z.d.d..
-00005980: 005a 0e64 0f64 1084 005a 0f64 1164 1284  .Z.d.d...Z.d.d..
-00005990: 005a 1064 1364 1484 005a 1164 1564 1684  .Z.d.d...Z.d.d..
-000059a0: 005a 1264 1753 0029 18da 1445 7870 6f72  .Z.d.S.)...Expor
-000059b0: 7455 7365 7253 6572 6961 6c69 7a65 7275  tUserSerializeru
-000059c0: 2200 0000 0a20 2020 20e5 afbc e587 bae7  "....    .......
-000059d0: 94a8 e688 b7e5 ba8f e588 97e5 8c96 e599  ................
-000059e0: a80a 2020 2020 72d1 0000 0072 a700 0000  ..    r....r....
-000059f0: 72d4 0000 0075 0600 0000 e881 8ce7 baa7  r....u..........
-00005a00: 750c 0000 00e7 bb91 e5ae 9ae5 8cbb e794  u...............
-00005a10: 9f75 1500 0000 e698 afe5 90a6 e4ba 92e8  .u..............
-00005a20: 8194 e7bd 91e6 8ea5 e8af 8a75 0c00 0000  ...........u....
-00005a30: e794 a8e6 88b7 e8a7 92e8 89b2 6300 0000  ............c...
-00005a40: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00005a50: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
-00005a60: 5a02 6503 5a04 6401 5a05 6402 5300 2903  Z.e.Z.d.Z.d.S.).
-00005a70: 7a19 4578 706f 7274 5573 6572 5365 7269  z.ExportUserSeri
-00005a80: 616c 697a 6572 2e4d 6574 6129 0872 c000  alizer.Meta).r..
-00005a90: 0000 72bc 0000 00da 0664 6f63 746f 72da  ..r......doctor.
-00005aa0: 0975 7365 725f 7261 6e6b 729c 0000 0072  .user_rankr....r
-00005ab0: 8c00 0000 72d9 0000 00da 0667 726f 7570  ....r......group
-00005ac0: 734e 729b 0000 0072 2500 0000 7225 0000  sNr....r%...r%..
-00005ad0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-00005ae0: b402 0000 7304 0000 0008 0104 0272 2700  ....s........r'.
-00005af0: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
-00005b00: 0000 0003 0000 0003 0000 0073 2a00 0000  ...........s*...
-00005b10: 7c01 6a00 a001 a100 8900 8700 6601 6401  |.j.........f.d.
-00005b20: 6402 8408 8800 4400 8301 7d02 6403 a002  d.....D...}.d...
-00005b30: 7c02 a101 7d03 7c03 5300 2904 4e63 0100  |...}.|.S.).Nc..
-00005b40: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00005b50: 0000 1300 0000 7316 0000 0067 007c 005d  ......s....g.|.]
-00005b60: 0e7d 0188 0072 047c 016a 0091 0271 0453  .}...r.|.j...q.S
-00005b70: 0072 2500 0000 2901 7276 0000 0029 0272  .r%...).rv...).r
-00005b80: 6500 0000 72e7 0000 00a9 0172 3001 0000  e...r......r0...
-00005b90: 7225 0000 0072 2600 0000 7266 0000 00c4  r%...r&...rf....
-00005ba0: 0200 0072 5700 0000 7a33 4578 706f 7274  ...rW...z3Export
-00005bb0: 5573 6572 5365 7269 616c 697a 6572 2e67  UserSerializer.g
-00005bc0: 6574 5f67 726f 7570 732e 3c6c 6f63 616c  et_groups.<local
-00005bd0: 733e 2e3c 6c69 7374 636f 6d70 3efa 012c  s>.<listcomp>..,
-00005be0: 2903 7230 0100 0072 4500 0000 da04 6a6f  ).r0...rE.....jo
-00005bf0: 696e 2904 7234 0000 0072 3500 0000 5a09  in).r4...r5...Z.
-00005c00: 726f 6c65 5f6c 6973 745a 0872 6f6c 655f  role_listZ.role_
-00005c10: 7374 7272 2500 0000 7231 0100 0072 2600  strr%...r1...r&.
-00005c20: 0000 da0a 6765 745f 6772 6f75 7073 c202  ....get_groups..
-00005c30: 0000 7308 0000 0000 010a 0112 010a 017a  ..s............z
-00005c40: 1f45 7870 6f72 7455 7365 7253 6572 6961  .ExportUserSeria
-00005c50: 6c69 7a65 722e 6765 745f 6772 6f75 7073  lizer.get_groups
-00005c60: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00005c70: 0001 0000 0043 0000 0073 1400 0000 7c01  .....C...s....|.
-00005c80: 6a00 7d02 7c02 7210 7c02 6a01 5300 6400  j.}.|.r.|.j.S.d.
-00005c90: 5300 724a 0000 0072 c200 0000 72da 0000  S.rJ...r....r...
-00005ca0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00005cb0: 72d2 0000 00c8 0200 0073 0600 0000 0001  r........s......
-00005cc0: 0601 0401 7a21 4578 706f 7274 5573 6572  ....z!ExportUser
-00005cd0: 5365 7269 616c 697a 6572 2e67 6574 5f68  Serializer.get_h
-00005ce0: 6f73 7069 7461 6c63 0200 0000 0000 0000  ospitalc........
-00005cf0: 0000 0000 0300 0000 0100 0000 4300 0000  ............C...
-00005d00: 7314 0000 007c 016a 007d 027c 0272 107c  s....|.j.}.|.r.|
-00005d10: 026a 0153 0064 0053 0072 4a00 0000 72be  .j.S.d.S.rJ...r.
-00005d20: 0000 0072 db00 0000 7225 0000 0072 2500  ...r....r%...r%.
-00005d30: 0000 7226 0000 0072 dc00 0000 cd02 0000  ..r&...r........
-00005d40: 7306 0000 0000 0106 0104 017a 1f45 7870  s..........z.Exp
-00005d50: 6f72 7455 7365 7253 6572 6961 6c69 7a65  ortUserSerialize
-00005d60: 722e 6765 745f 6f66 6669 6365 6302 0000  r.get_officec...
-00005d70: 0000 0000 0000 0000 0003 0000 0001 0000  ................
-00005d80: 0043 0000 0073 1400 0000 7c01 6a00 7d02  .C...s....|.j.}.
-00005d90: 7c02 7210 7c02 6a01 5300 6400 5300 724a  |.r.|.j.S.d.S.rJ
-00005da0: 0000 0029 0272 2f01 0000 7276 0000 0029  ...).r/...rv...)
-00005db0: 0372 3400 0000 7235 0000 0072 2f01 0000  .r4...r5...r/...
-00005dc0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-00005dd0: 0d67 6574 5f75 7365 725f 7261 6e6b d202  .get_user_rank..
-00005de0: 0000 7306 0000 0000 0106 0104 017a 2245  ..s..........z"E
-00005df0: 7870 6f72 7455 7365 7253 6572 6961 6c69  xportUserSeriali
-00005e00: 7a65 722e 6765 745f 7573 6572 5f72 616e  zer.get_user_ran
-00005e10: 6b63 0200 0000 0000 0000 0000 0000 0300  kc..............
-00005e20: 0000 0100 0000 4300 0000 7314 0000 007c  ......C...s....|
-00005e30: 016a 007d 027c 0272 107c 026a 0153 0064  .j.}.|.r.|.j.S.d
-00005e40: 0053 0072 4a00 0000 2902 722e 0100 0072  .S.rJ...).r....r
-00005e50: 7600 0000 a903 7234 0000 0072 3500 0000  v.....r4...r5...
-00005e60: 722e 0100 0072 2500 0000 7225 0000 0072  r....r%...r%...r
-00005e70: 2600 0000 da0a 6765 745f 646f 6374 6f72  &.....get_doctor
-00005e80: d702 0000 7306 0000 0000 0106 0104 017a  ....s..........z
-00005e90: 1f45 7870 6f72 7455 7365 7253 6572 6961  .ExportUserSeria
-00005ea0: 6c69 7a65 722e 6765 745f 646f 6374 6f72  lizer.get_doctor
-00005eb0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00005ec0: 0001 0000 0043 0000 0073 1400 0000 7c01  .....C...s....|.
-00005ed0: 6a00 7d02 7c02 7210 7c02 6a01 5300 6400  j.}.|.r.|.j.S.d.
-00005ee0: 5300 724a 0000 0029 0272 2e01 0000 72d9  S.rJ...).r....r.
-00005ef0: 0000 0072 3601 0000 7225 0000 0072 2500  ...r6...r%...r%.
-00005f00: 0000 7226 0000 00da 1567 6574 5f69 735f  ..r&.....get_is_
-00005f10: 6f6e 6c69 6e65 5f63 6f6e 7375 6c74 dc02  online_consult..
-00005f20: 0000 7306 0000 0000 0106 0104 017a 2a45  ..s..........z*E
-00005f30: 7870 6f72 7455 7365 7253 6572 6961 6c69  xportUserSeriali
-00005f40: 7a65 722e 6765 745f 6973 5f6f 6e6c 696e  zer.get_is_onlin
-00005f50: 655f 636f 6e73 756c 744e 2913 721f 0000  e_consultN).r...
-00005f60: 0072 2000 0000 7221 0000 0072 2900 0000  .r ...r!...r)...
-00005f70: 7205 0000 0072 3a00 0000 72c0 0000 0072  r....r:...r....r
-00005f80: bc00 0000 722f 0100 0072 2e01 0000 72d9  ....r/...r....r.
-00005f90: 0000 0072 3001 0000 7227 0000 0072 3401  ...r0...r'...r4.
-00005fa0: 0000 72d2 0000 0072 dc00 0000 7235 0100  ..r....r....r5..
-00005fb0: 0072 3701 0000 7238 0100 0072 2500 0000  .r7...r8...r%...
-00005fc0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-00005fd0: 2d01 0000 a902 0000 731c 0000 0008 0104  -.......s.......
-00005fe0: 030c 010c 010c 010c 010c 010c 020e 0e08  ................
-00005ff0: 0608 0508 0508 0508 0572 2d01 0000 6300  .........r-...c.
-00006000: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00006010: 0000 0040 0000 0073 4a00 0000 6500 5a01  ...@...sJ...e.Z.
-00006020: 6400 5a02 6503 a004 a100 5a05 6503 a004  d.Z.e.....Z.e...
-00006030: a100 5a06 6503 a004 a100 5a07 4700 6401  ..Z.e.....Z.G.d.
-00006040: 6402 8400 6402 8302 5a08 6403 6404 8400  d...d...Z.d.d...
-00006050: 5a09 6405 6406 8400 5a0a 6407 6408 8400  Z.d.d...Z.d.d...
-00006060: 5a0b 6409 5300 290a da17 4472 7567 4469  Z.d.S.)...DrugDi
-00006070: 7265 6374 6f72 7953 6572 6961 6c69 7a65  rectorySerialize
-00006080: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-00006090: 0000 0100 0000 4000 0000 7314 0000 0065  ......@...s....e
-000060a0: 005a 0164 005a 0265 035a 0464 015a 0564  .Z.d.Z.e.Z.d.Z.d
-000060b0: 0253 0029 037a 1c44 7275 6744 6972 6563  .S.).z.DrugDirec
-000060c0: 746f 7279 5365 7269 616c 697a 6572 2e4d  torySerializer.M
-000060d0: 6574 6172 1c00 0000 4e72 1601 0000 7225  etar....Nr....r%
-000060e0: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-000060f0: 0000 7227 0000 00e7 0200 0073 0400 0000  ..r'.......s....
-00006100: 0801 0401 7227 0000 0063 0200 0000 0000  ....r'...c......
-00006110: 0000 0000 0000 0300 0000 0100 0000 4300  ..............C.
-00006120: 0000 7314 0000 007c 016a 007d 027c 0272  ..s....|.j.}.|.r
-00006130: 107c 026a 0153 0064 0053 0072 4a00 0000  .|.j.S.d.S.rJ...
-00006140: 7217 0100 0072 1a01 0000 7225 0000 0072  r....r....r%...r
-00006150: 2500 0000 7226 0000 00da 1467 6574 5f70  %...r&.....get_p
-00006160: 7265 7061 7261 7469 6f6e 5f74 7970 65eb  reparation_type.
-00006170: 0200 0073 0600 0000 0001 0601 0401 7a2c  ...s..........z,
-00006180: 4472 7567 4469 7265 6374 6f72 7953 6572  DrugDirectorySer
-00006190: 6961 6c69 7a65 722e 6765 745f 7072 6570  ializer.get_prep
-000061a0: 6172 6174 696f 6e5f 7479 7065 6302 0000  aration_typec...
-000061b0: 0000 0000 0000 0000 0003 0000 0001 0000  ................
-000061c0: 0043 0000 0073 1400 0000 7c01 6a00 7d02  .C...s....|.j.}.
-000061d0: 7c02 7210 7c02 6a01 5300 6400 5300 724a  |.r.|.j.S.d.S.rJ
-000061e0: 0000 0072 2001 0000 7222 0100 0072 2500  ...r ...r"...r%.
-000061f0: 0000 7225 0000 0072 2600 0000 da0d 6765  ..r%...r&.....ge
-00006200: 745f 6472 7567 5f74 7970 65f0 0200 0073  t_drug_type....s
-00006210: 0600 0000 0001 0601 0401 7a25 4472 7567  ..........z%Drug
-00006220: 4469 7265 6374 6f72 7953 6572 6961 6c69  DirectorySeriali
-00006230: 7a65 722e 6765 745f 6472 7567 5f74 7970  zer.get_drug_typ
-00006240: 6563 0200 0000 0000 0000 0000 0000 0300  ec..............
-00006250: 0000 0100 0000 4300 0000 7314 0000 007c  ......C...s....|
-00006260: 016a 007d 027c 0272 107c 026a 0153 0064  .j.}.|.r.|.j.S.d
-00006270: 0053 0072 4a00 0000 721c 0100 0072 1e01  .S.rJ...r....r..
-00006280: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
-00006290: 0072 1f01 0000 f502 0000 7306 0000 0000  .r........s.....
-000062a0: 0106 0104 017a 2944 7275 6744 6972 6563  .....z)DrugDirec
-000062b0: 746f 7279 5365 7269 616c 697a 6572 2e67  torySerializer.g
-000062c0: 6574 5f63 6174 6567 6f72 795f 6e61 6d65  et_category_name
-000062d0: 4e29 0c72 1f00 0000 7220 0000 0072 2100  N).r....r ...r!.
-000062e0: 0000 7205 0000 0072 3a00 0000 7218 0100  ..r....r:...r...
-000062f0: 0072 2101 0000 7209 0100 0072 2700 0000  .r!...r....r'...
-00006300: 723a 0100 0072 3b01 0000 721f 0100 0072  r:...r;...r....r
-00006310: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
-00006320: 0000 0072 3901 0000 e202 0000 730e 0000  ...r9.......s...
-00006330: 0008 0108 0108 0108 020e 0408 0508 0572  ...............r
-00006340: 3901 0000 6300 0000 0000 0000 0000 0000  9...c...........
-00006350: 0000 0000 0003 0000 0040 0000 0073 1e00  .........@...s..
-00006360: 0000 6500 5a01 6400 5a02 6401 5a03 4700  ..e.Z.d.Z.d.Z.G.
-00006370: 6402 6403 8400 6403 8302 5a04 6404 5300  d.d...d...Z.d.S.
-00006380: 2905 da11 4170 6949 6e66 6f53 6572 6961  )...ApiInfoSeria
-00006390: 6c69 7a65 7275 2200 0000 0a20 2020 20e5  lizeru"....    .
-000063a0: 9b9e e586 99e5 8f82 e695 b0e5 ba8f e588  ................
-000063b0: 97e5 8c96 e599 a80a 2020 2020 6300 0000  ........    c...
-000063c0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-000063d0: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
-000063e0: 5a02 6503 5a04 6401 5a05 6402 5300 2903  Z.e.Z.d.Z.d.S.).
-000063f0: 7a16 4170 6949 6e66 6f53 6572 6961 6c69  z.ApiInfoSeriali
-00006400: 7a65 722e 4d65 7461 721c 0000 004e 2906  zer.Metar....N).
-00006410: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-00006420: 1200 0000 7222 0000 0072 2300 0000 7225  ....r"...r#...r%
-00006430: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00006440: 0000 7227 0000 0000 0300 0073 0400 0000  ..r'.......s....
-00006450: 0801 0401 7227 0000 004e 7228 0000 0072  ....r'...Nr(...r
-00006460: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
-00006470: 0000 0072 3c01 0000 fb02 0000 7304 0000  ...r<.......s...
-00006480: 0008 0104 0472 3c01 0000 6300 0000 0000  .....r<...c.....
-00006490: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-000064a0: 0000 0073 6e00 0000 6500 5a01 6400 5a02  ...sn...e.Z.d.Z.
-000064b0: 6401 5a03 6504 6a05 6402 6403 8d01 5a06  d.Z.e.j.d.d...Z.
-000064c0: 6504 6a05 6404 6403 8d01 5a07 6504 6a05  e.j.d.d...Z.e.j.
-000064d0: 6405 6403 8d01 5a08 6504 6a05 6406 6403  d.d...Z.e.j.d.d.
-000064e0: 8d01 5a09 4700 6407 6408 8400 6408 8302  ..Z.G.d.d...d...
-000064f0: 5a0a 6409 640a 8400 5a0b 640b 640c 8400  Z.d.d...Z.d.d...
-00006500: 5a0c 640d 640e 8400 5a0d 640f 6410 8400  Z.d.d...Z.d.d...
-00006510: 5a0e 6411 5300 2912 da1c 4578 706f 7274  Z.d.S.)...Export
-00006520: 5068 6172 6d61 6379 4472 7567 5365 7269  PharmacyDrugSeri
-00006530: 616c 697a 6572 72ff 0000 0072 0001 0000  alizerr....r....
-00006540: 72a7 0000 0075 0c00 0000 e88d afe6 88bf  r....u..........
-00006550: e590 8de7 a7b0 7201 0100 0072 0201 0000  ......r....r....
-00006560: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00006570: 0001 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
-00006580: 5a01 6400 5a02 6503 5a04 6401 5a05 6402  Z.d.Z.e.Z.d.Z.d.
-00006590: 5300 2903 7a21 4578 706f 7274 5068 6172  S.).z!ExportPhar
-000065a0: 6d61 6379 4472 7567 5365 7269 616c 697a  macyDrugSerializ
-000065b0: 6572 2e4d 6574 6129 1172 2601 0000 7203  er.Meta).r&...r.
-000065c0: 0100 0072 0401 0000 7205 0100 0072 0701  ...r....r....r..
-000065d0: 0000 7208 0100 0072 0901 0000 720a 0100  ..r....r....r...
-000065e0: 0072 0b01 0000 da0a 7661 6c69 645f 6461  .r......valid_da
-000065f0: 7465 da12 696e 7665 6e74 6f72 795f 7175  te..inventory_qu
-00006600: 616e 7469 7479 da10 6d65 6173 7572 656d  antity..measurem
-00006610: 656e 745f 756e 6974 da0f 636f 7374 5f75  ent_unit..cost_u
-00006620: 6e69 745f 7072 6963 65da 0b63 6f73 745f  nit_price..cost_
-00006630: 616d 6f75 6e74 da11 7265 7461 696c 5f75  amount..retail_u
-00006640: 6e69 745f 7072 6963 65da 0d72 6574 6169  nit_price..retai
-00006650: 6c5f 616d 6f75 6e74 72e4 0000 004e 2906  l_amountr....N).
-00006660: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-00006670: 1300 0000 7222 0000 0072 2300 0000 7225  ....r"...r#...r%
-00006680: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00006690: 0000 7227 0000 000c 0300 0073 0400 0000  ..r'.......s....
-000066a0: 0801 0401 7227 0000 0063 0200 0000 0000  ....r'...c......
-000066b0: 0000 0000 0000 0300 0000 0100 0000 4300  ..............C.
-000066c0: 0000 7314 0000 007c 016a 007d 027c 0272  ..s....|.j.}.|.r
-000066d0: 107c 026a 0153 0064 0053 0072 4a00 0000  .|.j.S.d.S.rJ...
-000066e0: 7217 0100 0072 1a01 0000 7225 0000 0072  r....r....r%...r
-000066f0: 2500 0000 7226 0000 0072 1b01 0000 2203  %...r&...r....".
-00006700: 0000 7306 0000 0000 0106 0104 017a 3645  ..s..........z6E
-00006710: 7870 6f72 7450 6861 726d 6163 7944 7275  xportPharmacyDru
-00006720: 6753 6572 6961 6c69 7a65 722e 6765 745f  gSerializer.get_
-00006730: 7072 6570 6172 6174 696f 6e5f 7479 7065  preparation_type
-00006740: 5f6e 616d 6563 0200 0000 0000 0000 0000  _namec..........
-00006750: 0000 0200 0000 0100 0000 4300 0000 7312  ..........C...s.
-00006760: 0000 007c 016a 0072 0e7c 016a 006a 0153  ...|.j.r.|.j.j.S
-00006770: 0064 0053 0072 4a00 0000 2902 da08 7068  .d.S.rJ...)...ph
-00006780: 6172 6d61 6379 7226 0100 0072 8400 0000  armacyr&...r....
-00006790: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-000067a0: 1167 6574 5f70 6861 726d 6163 795f 6e61  .get_pharmacy_na
-000067b0: 6d65 2703 0000 7304 0000 0000 0106 017a  me'...s........z
-000067c0: 2e45 7870 6f72 7450 6861 726d 6163 7944  .ExportPharmacyD
-000067d0: 7275 6753 6572 6961 6c69 7a65 722e 6765  rugSerializer.ge
-000067e0: 745f 7068 6172 6d61 6379 5f6e 616d 6563  t_pharmacy_namec
-000067f0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00006800: 0100 0000 4300 0000 7314 0000 007c 016a  ....C...s....|.j
-00006810: 007d 027c 0272 107c 026a 0153 0064 0053  .}.|.r.|.j.S.d.S
-00006820: 0072 4a00 0000 721c 0100 0072 1e01 0000  .rJ...r....r....
-00006830: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-00006840: 1f01 0000 2b03 0000 7306 0000 0000 0106  ....+...s.......
-00006850: 0104 017a 2e45 7870 6f72 7450 6861 726d  ...z.ExportPharm
-00006860: 6163 7944 7275 6753 6572 6961 6c69 7a65  acyDrugSerialize
-00006870: 722e 6765 745f 6361 7465 676f 7279 5f6e  r.get_category_n
-00006880: 616d 6563 0200 0000 0000 0000 0000 0000  amec............
-00006890: 0300 0000 0100 0000 4300 0000 7314 0000  ........C...s...
-000068a0: 007c 016a 007d 027c 0272 107c 026a 0153  .|.j.}.|.r.|.j.S
-000068b0: 0064 0053 0072 4a00 0000 7220 0100 0072  .d.S.rJ...r ...r
-000068c0: 2201 0000 7225 0000 0072 2500 0000 7226  "...r%...r%...r&
-000068d0: 0000 0072 2301 0000 3003 0000 7306 0000  ...r#...0...s...
-000068e0: 0000 0106 0104 017a 2f45 7870 6f72 7450  .......z/ExportP
-000068f0: 6861 726d 6163 7944 7275 6753 6572 6961  harmacyDrugSeria
-00006900: 6c69 7a65 722e 6765 745f 6472 7567 5f74  lizer.get_drug_t
-00006910: 7970 655f 6e61 6d65 4e29 0f72 1f00 0000  ype_nameN).r....
-00006920: 7220 0000 0072 2100 0000 7229 0000 0072  r ...r!...r)...r
-00006930: 0500 0000 723a 0000 0072 0701 0000 7226  ....r:...r....r&
-00006940: 0100 0072 0901 0000 7208 0100 0072 2700  ...r....r....r'.
-00006950: 0000 721b 0100 0072 4601 0000 721f 0100  ..r....rF...r...
-00006960: 0072 2301 0000 7225 0000 0072 2500 0000  .r#...r%...r%...
-00006970: 7225 0000 0072 2600 0000 723d 0100 0005  r%...r&...r=....
-00006980: 0300 0073 1400 0000 0801 0401 0c01 0c01  ...s............
-00006990: 0c01 0c02 0e16 0805 0804 0805 723d 0100  ............r=..
-000069a0: 004e 2940 da0b 646a 616e 676f 2e63 6f6e  .N)@..django.con
-000069b0: 6672 0200 0000 da1a 646a 616e 676f 2e63  fr......django.c
-000069c0: 6f6e 7472 6962 2e61 7574 682e 6d6f 6465  ontrib.auth.mode
-000069d0: 6c73 7203 0000 00da 2264 6a61 6e67 6f2e  lsr....."django.
-000069e0: 636f 6e74 7269 622e 636f 6e74 656e 7474  contrib.contentt
-000069f0: 7970 6573 2e6d 6f64 656c 7372 0400 0000  ypes.modelsr....
-00006a00: da0e 7265 7374 5f66 7261 6d65 776f 726b  ..rest_framework
-00006a10: 7205 0000 00da 1262 6173 655f 7379 7374  r......base_syst
-00006a20: 656d 2e6d 6f64 656c 7372 0600 0000 7207  em.modelsr....r.
-00006a30: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00006a40: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00006a50: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00006a60: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00006a70: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
-00006a80: 0000 0072 1800 0000 7219 0000 00da 0966  ...r....r......f
-00006a90: 756e 6374 6f6f 6c73 721a 0000 00da 0f4d  unctoolsr......M
-00006aa0: 6f64 656c 5365 7269 616c 697a 6572 721b  odelSerializerr.
-00006ab0: 0000 0072 2a00 0000 722b 0000 0072 3200  ...r*...r+...r2.
-00006ac0: 0000 7242 0000 0072 4e00 0000 7251 0000  ..rB...rN...rQ..
-00006ad0: 0072 8300 0000 da0a 5365 7269 616c 697a  .r......Serializ
-00006ae0: 6572 7286 0000 0072 9a00 0000 72a6 0000  err....r....r...
-00006af0: 0072 b400 0000 72b5 0000 0072 b700 0000  .r....r....r....
-00006b00: 72c9 0000 0072 d000 0000 72d3 0000 0072  r....r....r....r
-00006b10: e100 0000 72e2 0000 0072 e900 0000 72ec  ....r....r....r.
-00006b20: 0000 0072 f200 0000 72fa 0000 0072 fb00  ...r....r....r..
-00006b30: 0000 72fd 0000 0072 fe00 0000 7224 0100  ..r....r....r$..
-00006b40: 0072 2d01 0000 7239 0100 0072 3c01 0000  .r-...r9...r<...
-00006b50: 723d 0100 0072 2500 0000 7225 0000 0072  r=...r%...r%...r
-00006b60: 2500 0000 7226 0000 00da 083c 6d6f 6475  %...r&.....<modu
-00006b70: 6c65 3e01 0000 0073 4a00 0000 0c01 0c01  le>....sJ.......
-00006b80: 0c01 0c01 5403 0c01 0c03 120d 120a 1211  ....T...........
-00006b90: 120f 121e 120a 1250 120a 1219 121e 121c  .......P........
-00006ba0: 120b 120a 122b 1206 121f 1232 1217 121e  .....+.....2....
-00006bb0: 120f 1214 121d 120e 1214 121d 122f 1217  ............./..
-00006bc0: 1239 1219 120a                           .9....
+000041c0: 4300 0000 7328 0000 0074 006a 016a 027c  C...s(...t.j.j.|
+000041d0: 0164 018d 017d 027c 0272 2474 037c 0264  .d...}.|.r$t.|.d
+000041e0: 0264 038d 027d 037c 036a 0453 0064 0053  .d...}.|.j.S.d.S
+000041f0: 00a9 044e 2901 726c 0000 0054 722f 0000  ...N).rl...Tr/..
+00004200: 0029 0572 1800 0000 725a 0000 0072 5c00  .).r....rZ...r\.
+00004210: 0000 72e9 0000 0072 3300 0000 a904 7234  ..r....r3.....r4
+00004220: 0000 0072 3500 0000 723b 0000 0072 3700  ...r5...r;...r7.
+00004230: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
+00004240: 0072 3800 0000 ed01 0000 7308 0000 0000  .r8.......s.....
+00004250: 010e 0104 010c 017a 2549 6e73 7065 6374  .......z%Inspect
+00004260: 696f 6e54 7970 6553 6572 6961 6c69 7a65  ionTypeSerialize
+00004270: 722e 6765 745f 6368 696c 6472 656e 4e72  r.get_childrenNr
+00004280: 3900 0000 7225 0000 0072 2500 0000 7225  9...r%...r%...r%
+00004290: 0000 0072 2600 0000 72e9 0000 00e4 0100  ...r&...r.......
+000042a0: 0073 0800 0000 0801 0402 0802 0e04 72e9  .s............r.
+000042b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000042c0: 0000 0000 0300 0000 4000 0000 733e 0000  ........@...s>..
+000042d0: 0065 005a 0164 005a 0264 015a 0365 04a0  .e.Z.d.Z.d.Z.e..
+000042e0: 05a1 005a 0665 04a0 05a1 005a 0747 0064  ...Z.e.....Z.G.d
+000042f0: 0264 0384 0064 0383 025a 0864 0464 0584  .d...d...Z.d.d..
+00004300: 005a 0964 0664 0784 005a 0a64 0853 0029  .Z.d.d...Z.d.S.)
+00004310: 09da 2049 6e73 7065 6374 696f 6e44 6963  .. InspectionDic
+00004320: 7469 6f6e 6172 6965 7353 6572 6961 6c69  tionariesSeriali
+00004330: 7a65 7275 1800 0000 e6a3 80e6 9fa5 e5ad  zeru............
+00004340: 97e5 85b8 e5ba 8fe5 8897 e58c 96e5 99a8  ................
+00004350: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00004360: 0001 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
+00004370: 5a01 6400 5a02 6503 5a04 6401 5a05 6402  Z.d.Z.e.Z.d.Z.d.
+00004380: 5300 2903 7a25 496e 7370 6563 7469 6f6e  S.).z%Inspection
+00004390: 4469 6374 696f 6e61 7269 6573 5365 7269  DictionariesSeri
+000043a0: 616c 697a 6572 2e4d 6574 6172 1c00 0000  alizer.Metar....
+000043b0: 4ea9 0672 1f00 0000 7220 0000 0072 2100  N..r....r ...r!.
+000043c0: 0000 720c 0000 0072 2200 0000 7223 0000  ..r....r"...r#..
+000043d0: 0072 2500 0000 7225 0000 0072 2500 0000  .r%...r%...r%...
+000043e0: 7226 0000 0072 2700 0000 f901 0000 7304  r&...r'.......s.
+000043f0: 0000 0008 0104 0172 2700 0000 6302 0000  .......r'...c...
+00004400: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00004410: 0043 0000 0073 2200 0000 7400 6a01 6a02  .C...s"...t.j.j.
+00004420: 7c01 6a03 6401 8d01 a004 a100 7d02 7c02  |.j.d.......}.|.
+00004430: 721e 7c02 6a05 5300 6400 5300 a902 4e29  r.|.j.S.d.S...N)
+00004440: 0172 a900 0000 a906 7206 0000 0072 5a00  .r......r....rZ.
+00004450: 0000 725c 0000 0072 ce00 0000 7246 0000  ..r\...r....rF..
+00004460: 0072 7600 0000 72da 0000 0072 2500 0000  .rv...r....r%...
+00004470: 7225 0000 0072 2600 0000 72c3 0000 00fd  r%...r&...r.....
+00004480: 0100 0073 0600 0000 0001 1401 0401 7a32  ...s..........z2
+00004490: 496e 7370 6563 7469 6f6e 4469 6374 696f  InspectionDictio
+000044a0: 6e61 7269 6573 5365 7269 616c 697a 6572  nariesSerializer
+000044b0: 2e67 6574 5f68 6f73 7069 7461 6c5f 6e61  .get_hospital_na
+000044c0: 6d65 6302 0000 0000 0000 0000 0000 0003  mec.............
+000044d0: 0000 0003 0000 0043 0000 0073 2200 0000  .......C...s"...
+000044e0: 7400 6a01 6a02 7c01 6a03 6401 8d01 a004  t.j.j.|.j.d.....
+000044f0: a100 7d02 7c02 721e 7c02 6a05 5300 6400  ..}.|.r.|.j.S.d.
+00004500: 5300 72ee 0000 00a9 0672 0700 0000 725a  S.r......r....rZ
+00004510: 0000 0072 5c00 0000 72cc 0000 0072 4600  ...r\...r....rF.
+00004520: 0000 7276 0000 0072 db00 0000 7225 0000  ..rv...r....r%..
+00004530: 0072 2500 0000 7226 0000 0072 bf00 0000  .r%...r&...r....
+00004540: 0202 0000 7306 0000 0000 0114 0104 017a  ....s..........z
+00004550: 3049 6e73 7065 6374 696f 6e44 6963 7469  0InspectionDicti
+00004560: 6f6e 6172 6965 7353 6572 6961 6c69 7a65  onariesSerialize
+00004570: 722e 6765 745f 6f66 6669 6365 5f6e 616d  r.get_office_nam
+00004580: 654e a90b 721f 0000 0072 2000 0000 7221  eN..r....r ...r!
+00004590: 0000 0072 2900 0000 7205 0000 0072 3a00  ...r)...r....r:.
+000045a0: 0000 72cf 0000 0072 cd00 0000 7227 0000  ..r....r....r'..
+000045b0: 0072 c300 0000 72bf 0000 0072 2500 0000  .r....r....r%...
+000045c0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
+000045d0: ec00 0000 f401 0000 730c 0000 0008 0104  ........s.......
+000045e0: 0108 0108 020e 0408 0572 ec00 0000 6300  .........r....c.
+000045f0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00004600: 0000 0040 0000 0073 4600 0000 6500 5a01  ...@...sF...e.Z.
+00004610: 6400 5a02 6401 5a03 6504 6a05 6402 6403  d.Z.d.Z.e.j.d.d.
+00004620: 8d01 5a06 6504 6a05 6404 6403 8d01 5a07  ..Z.e.j.d.d...Z.
+00004630: 4700 6405 6406 8400 6406 8302 5a08 6407  G.d.d...d...Z.d.
+00004640: 6408 8400 5a09 6409 640a 8400 5a0a 640b  d...Z.d.d...Z.d.
+00004650: 5300 290c da26 4578 706f 7274 496e 7370  S.)..&ExportInsp
+00004660: 6563 7469 6f6e 4469 6374 696f 6e61 7269  ectionDictionari
+00004670: 6573 5365 7269 616c 697a 6572 751e 0000  esSerializeru...
+00004680: 00e5 afbc e587 bae6 a380 e69f a5e5 ad97  ................
+00004690: e585 b8e5 ba8f e588 97e5 8c96 e599 a872  ...............r
+000046a0: d100 0000 72a7 0000 0072 d400 0000 6300  ....r....r....c.
+000046b0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000046c0: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
+000046d0: 6400 5a02 6503 5a04 6401 5a05 6402 5300  d.Z.e.Z.d.Z.d.S.
+000046e0: 2903 7a2b 4578 706f 7274 496e 7370 6563  ).z+ExportInspec
+000046f0: 7469 6f6e 4469 6374 696f 6e61 7269 6573  tionDictionaries
+00004700: 5365 7269 616c 697a 6572 2e4d 6574 61a9  Serializer.Meta.
+00004710: 08da 0c70 726f 6a65 6374 5f63 6f64 65da  ...project_code.
+00004720: 0c70 726f 6a65 6374 5f6e 616d 6572 cf00  .project_namer..
+00004730: 0000 72cd 0000 00da 0c70 726f 6a65 6374  ..r......project
+00004740: 5f66 6565 73da 0a63 6f64 655f 7372 7674  _fees..code_srvt
+00004750: 70da 0a6e 616d 655f 7372 7674 70da 0772  p..name_srvtp..r
+00004760: 656d 6172 6b73 4e72 ed00 0000 7225 0000  emarksNr....r%..
+00004770: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00004780: 7227 0000 000d 0200 0073 0400 0000 0801  r'.......s......
+00004790: 0401 7227 0000 0063 0200 0000 0000 0000  ..r'...c........
+000047a0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+000047b0: 7322 0000 0074 006a 016a 027c 016a 0364  s"...t.j.j.|.j.d
+000047c0: 018d 01a0 04a1 007d 027c 0272 1e7c 026a  .......}.|.r.|.j
+000047d0: 0553 0064 0053 0072 ee00 0000 72ef 0000  .S.d.S.r....r...
+000047e0: 0072 da00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+000047f0: 7226 0000 0072 c300 0000 1a02 0000 7306  r&...r........s.
+00004800: 0000 0000 0114 0104 017a 3845 7870 6f72  .........z8Expor
+00004810: 7449 6e73 7065 6374 696f 6e44 6963 7469  tInspectionDicti
+00004820: 6f6e 6172 6965 7353 6572 6961 6c69 7a65  onariesSerialize
+00004830: 722e 6765 745f 686f 7370 6974 616c 5f6e  r.get_hospital_n
+00004840: 616d 6563 0200 0000 0000 0000 0000 0000  amec............
+00004850: 0300 0000 0300 0000 4300 0000 7322 0000  ........C...s"..
+00004860: 0074 006a 016a 027c 016a 0364 018d 01a0  .t.j.j.|.j.d....
+00004870: 04a1 007d 027c 0272 1e7c 026a 0553 0064  ...}.|.r.|.j.S.d
+00004880: 0053 0072 ee00 0000 72f0 0000 0072 db00  .S.r....r....r..
+00004890: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
+000048a0: 0072 bf00 0000 1f02 0000 7306 0000 0000  .r........s.....
+000048b0: 0114 0104 017a 3645 7870 6f72 7449 6e73  .....z6ExportIns
+000048c0: 7065 6374 696f 6e44 6963 7469 6f6e 6172  pectionDictionar
+000048d0: 6965 7353 6572 6961 6c69 7a65 722e 6765  iesSerializer.ge
+000048e0: 745f 6f66 6669 6365 5f6e 616d 654e 72f1  t_office_nameNr.
+000048f0: 0000 0072 2500 0000 7225 0000 0072 2500  ...r%...r%...r%.
+00004900: 0000 7226 0000 0072 f200 0000 0802 0000  ..r&...r........
+00004910: 730c 0000 0008 0104 010c 010c 020e 0d08  s...............
+00004920: 0572 f200 0000 6300 0000 0000 0000 0000  .r....c.........
+00004930: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00004940: 2e00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00004950: 6504 a005 a100 5a06 4700 6402 6403 8400  e.....Z.G.d.d...
+00004960: 6403 8302 5a07 6404 6405 8400 5a08 6406  d...Z.d.d...Z.d.
+00004970: 5300 2907 da19 4578 616d 696e 6174 696f  S.)...Examinatio
+00004980: 6e54 7970 6553 6572 6961 6c69 7a65 7275  nTypeSerializeru
+00004990: 1e00 0000 e6a3 80e9 aa8c e5ad 97e5 85b8  ................
+000049a0: e7b1 bbe5 9e8b e5ba 8fe5 8897 e58c 96e5  ................
+000049b0: 99a8 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000049c0: 0000 0001 0000 0040 0000 0073 1400 0000  .......@...s....
+000049d0: 6500 5a01 6400 5a02 6503 5a04 6401 5a05  e.Z.d.Z.e.Z.d.Z.
+000049e0: 6402 5300 2903 7a1e 4578 616d 696e 6174  d.S.).z.Examinat
+000049f0: 696f 6e54 7970 6553 6572 6961 6c69 7a65  ionTypeSerialize
+00004a00: 722e 4d65 7461 721c 0000 004e 2906 721f  r.Metar....N).r.
+00004a10: 0000 0072 2000 0000 7221 0000 0072 1700  ...r ...r!...r..
+00004a20: 0000 7222 0000 0072 2300 0000 7225 0000  ..r"...r#...r%..
+00004a30: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00004a40: 7227 0000 0029 0200 0073 0400 0000 0801  r'...)...s......
+00004a50: 0401 7227 0000 0063 0200 0000 0000 0000  ..r'...c........
+00004a60: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+00004a70: 7328 0000 0074 006a 016a 027c 0164 018d  s(...t.j.j.|.d..
+00004a80: 017d 027c 0272 2474 037c 0264 0264 038d  .}.|.r$t.|.d.d..
+00004a90: 027d 037c 036a 0453 0064 0053 0072 ea00  .}.|.j.S.d.S.r..
+00004aa0: 0000 2905 7217 0000 0072 5a00 0000 725c  ..).r....rZ...r\
+00004ab0: 0000 0072 fa00 0000 7233 0000 0072 eb00  ...r....r3...r..
+00004ac0: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
+00004ad0: 0072 3800 0000 2d02 0000 7308 0000 0000  .r8...-...s.....
+00004ae0: 010e 0104 010c 017a 2645 7861 6d69 6e61  .......z&Examina
+00004af0: 7469 6f6e 5479 7065 5365 7269 616c 697a  tionTypeSerializ
+00004b00: 6572 2e67 6574 5f63 6869 6c64 7265 6e4e  er.get_childrenN
+00004b10: 7239 0000 0072 2500 0000 7225 0000 0072  r9...r%...r%...r
+00004b20: 2500 0000 7226 0000 0072 fa00 0000 2502  %...r&...r....%.
+00004b30: 0000 7308 0000 0008 0104 0108 020e 0472  ..s............r
+00004b40: fa00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00004b50: 0000 0000 0003 0000 0040 0000 0073 3e00  .........@...s>.
+00004b60: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
+00004b70: a005 a100 5a06 6504 a005 a100 5a07 4700  ....Z.e.....Z.G.
+00004b80: 6402 6403 8400 6403 8302 5a08 6404 6405  d.d...d...Z.d.d.
+00004b90: 8400 5a09 6406 6407 8400 5a0a 6408 5300  ..Z.d.d...Z.d.S.
+00004ba0: 2909 da21 4578 616d 696e 6174 696f 6e44  )..!ExaminationD
+00004bb0: 6963 7469 6f6e 6172 6965 7353 6572 6961  ictionariesSeria
+00004bc0: 6c69 7a65 7275 1800 0000 e6a3 80e9 aa8c  lizeru..........
+00004bd0: e5ad 97e5 85b8 e5ba 8fe5 8897 e58c 96e5  ................
+00004be0: 99a8 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00004bf0: 0000 0001 0000 0040 0000 0073 1400 0000  .......@...s....
+00004c00: 6500 5a01 6400 5a02 6503 5a04 6401 5a05  e.Z.d.Z.e.Z.d.Z.
+00004c10: 6402 5300 2903 7a26 4578 616d 696e 6174  d.S.).z&Examinat
+00004c20: 696f 6e44 6963 7469 6f6e 6172 6965 7353  ionDictionariesS
+00004c30: 6572 6961 6c69 7a65 722e 4d65 7461 721c  erializer.Metar.
+00004c40: 0000 004e a906 721f 0000 0072 2000 0000  ...N..r....r ...
+00004c50: 7221 0000 0072 0d00 0000 7222 0000 0072  r!...r....r"...r
+00004c60: 2300 0000 7225 0000 0072 2500 0000 7225  #...r%...r%...r%
+00004c70: 0000 0072 2600 0000 7227 0000 0039 0200  ...r&...r'...9..
+00004c80: 0073 0400 0000 0801 0401 7227 0000 0063  .s........r'...c
+00004c90: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00004ca0: 0300 0000 4300 0000 7322 0000 0074 006a  ....C...s"...t.j
+00004cb0: 016a 027c 016a 0364 018d 01a0 04a1 007d  .j.|.j.d.......}
+00004cc0: 027c 0272 1e7c 026a 0553 0064 0053 0072  .|.r.|.j.S.d.S.r
+00004cd0: ee00 0000 72ef 0000 0072 da00 0000 7225  ....r....r....r%
+00004ce0: 0000 0072 2500 0000 7226 0000 0072 c300  ...r%...r&...r..
+00004cf0: 0000 3d02 0000 7306 0000 0000 0114 0104  ..=...s.........
+00004d00: 017a 3345 7861 6d69 6e61 7469 6f6e 4469  .z3ExaminationDi
+00004d10: 6374 696f 6e61 7269 6573 5365 7269 616c  ctionariesSerial
+00004d20: 697a 6572 2e67 6574 5f68 6f73 7069 7461  izer.get_hospita
+00004d30: 6c5f 6e61 6d65 6302 0000 0000 0000 0000  l_namec.........
+00004d40: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
+00004d50: 2200 0000 7400 6a01 6a02 7c01 6a03 6401  "...t.j.j.|.j.d.
+00004d60: 8d01 a004 a100 7d02 7c02 721e 7c02 6a05  ......}.|.r.|.j.
+00004d70: 5300 6400 5300 72ee 0000 0072 f000 0000  S.d.S.r....r....
+00004d80: 72db 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
+00004d90: 2600 0000 72bf 0000 0042 0200 0073 0600  &...r....B...s..
+00004da0: 0000 0001 1401 0401 7a31 4578 616d 696e  ........z1Examin
+00004db0: 6174 696f 6e44 6963 7469 6f6e 6172 6965  ationDictionarie
+00004dc0: 7353 6572 6961 6c69 7a65 722e 6765 745f  sSerializer.get_
+00004dd0: 6f66 6669 6365 5f6e 616d 654e 72f1 0000  office_nameNr...
+00004de0: 0072 2500 0000 7225 0000 0072 2500 0000  .r%...r%...r%...
+00004df0: 7226 0000 0072 fb00 0000 3402 0000 730c  r&...r....4...s.
+00004e00: 0000 0008 0104 0108 0108 020e 0408 0572  ...............r
+00004e10: fb00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00004e20: 0000 0000 0003 0000 0040 0000 0073 4600  .........@...sF.
+00004e30: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
+00004e40: 6a05 6402 6403 8d01 5a06 6504 6a05 6404  j.d.d...Z.e.j.d.
+00004e50: 6403 8d01 5a07 4700 6405 6406 8400 6406  d...Z.G.d.d...d.
+00004e60: 8302 5a08 6407 6408 8400 5a09 6409 640a  ..Z.d.d...Z.d.d.
+00004e70: 8400 5a0a 640b 5300 290c da27 4578 706f  ..Z.d.S.)..'Expo
+00004e80: 7274 4578 616d 696e 6174 696f 6e44 6963  rtExaminationDic
+00004e90: 7469 6f6e 6172 6965 7353 6572 6961 6c69  tionariesSeriali
+00004ea0: 7a65 7275 1e00 0000 e5af bce5 87ba e6a3  zeru............
+00004eb0: 80e9 aa8c e5ad 97e5 85b8 e5ba 8fe5 8897  ................
+00004ec0: e58c 96e5 99a8 72d1 0000 0072 a700 0000  ......r....r....
+00004ed0: 72d4 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00004ee0: 0000 0000 0000 0100 0000 4000 0000 7314  ..........@...s.
+00004ef0: 0000 0065 005a 0164 005a 0265 035a 0464  ...e.Z.d.Z.e.Z.d
+00004f00: 015a 0564 0253 0029 037a 2c45 7870 6f72  .Z.d.S.).z,Expor
+00004f10: 7445 7861 6d69 6e61 7469 6f6e 4469 6374  tExaminationDict
+00004f20: 696f 6e61 7269 6573 5365 7269 616c 697a  ionariesSerializ
+00004f30: 6572 2e4d 6574 6172 f300 0000 4e72 fc00  er.Metar....Nr..
+00004f40: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
+00004f50: 0072 2600 0000 7227 0000 004d 0200 0073  .r&...r'...M...s
+00004f60: 0400 0000 0801 0401 7227 0000 0063 0200  ........r'...c..
+00004f70: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00004f80: 0000 4300 0000 7322 0000 0074 006a 016a  ..C...s"...t.j.j
+00004f90: 027c 016a 0364 018d 01a0 04a1 007d 027c  .|.j.d.......}.|
+00004fa0: 0272 1e7c 026a 0553 0064 0053 0072 ee00  .r.|.j.S.d.S.r..
+00004fb0: 0000 72ef 0000 0072 da00 0000 7225 0000  ..r....r....r%..
+00004fc0: 0072 2500 0000 7226 0000 0072 c300 0000  .r%...r&...r....
+00004fd0: 5a02 0000 7306 0000 0000 0114 0104 017a  Z...s..........z
+00004fe0: 3945 7870 6f72 7445 7861 6d69 6e61 7469  9ExportExaminati
+00004ff0: 6f6e 4469 6374 696f 6e61 7269 6573 5365  onDictionariesSe
+00005000: 7269 616c 697a 6572 2e67 6574 5f68 6f73  rializer.get_hos
+00005010: 7069 7461 6c5f 6e61 6d65 6302 0000 0000  pital_namec.....
+00005020: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
+00005030: 0000 0073 2200 0000 7400 6a01 6a02 7c01  ...s"...t.j.j.|.
+00005040: 6a03 6401 8d01 a004 a100 7d02 7c02 721e  j.d.......}.|.r.
+00005050: 7c02 6a05 5300 6400 5300 72ee 0000 0072  |.j.S.d.S.r....r
+00005060: f000 0000 72db 0000 0072 2500 0000 7225  ....r....r%...r%
+00005070: 0000 0072 2600 0000 72bf 0000 005f 0200  ...r&...r...._..
+00005080: 0073 0600 0000 0001 1401 0401 7a37 4578  .s..........z7Ex
+00005090: 706f 7274 4578 616d 696e 6174 696f 6e44  portExaminationD
+000050a0: 6963 7469 6f6e 6172 6965 7353 6572 6961  ictionariesSeria
+000050b0: 6c69 7a65 722e 6765 745f 6f66 6669 6365  lizer.get_office
+000050c0: 5f6e 616d 654e 72f1 0000 0072 2500 0000  _nameNr....r%...
+000050d0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
+000050e0: fd00 0000 4802 0000 730c 0000 0008 0104  ....H...s.......
+000050f0: 010c 010c 020e 0d08 0572 fd00 0000 6300  .........r....c.
+00005100: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00005110: 0000 0040 0000 0073 5a00 0000 6500 5a01  ...@...sZ...e.Z.
+00005120: 6400 5a02 6401 5a03 6504 6a05 6402 6403  d.Z.d.Z.e.j.d.d.
+00005130: 8d01 5a06 6504 6a05 6404 6403 8d01 5a07  ..Z.e.j.d.d...Z.
+00005140: 6504 6a05 6405 6403 8d01 5a08 4700 6406  e.j.d.d...Z.G.d.
+00005150: 6407 8400 6407 8302 5a09 6408 6409 8400  d...d...Z.d.d...
+00005160: 5a0a 640a 640b 8400 5a0b 640c 640d 8400  Z.d.d...Z.d.d...
+00005170: 5a0c 640e 5300 290f da1d 4578 706f 7274  Z.d.S.)...Export
+00005180: 4472 7567 4469 7265 6374 6f72 7953 6572  DrugDirectorySer
+00005190: 6961 6c69 7a65 72f5 1e00 0000 e5af bce5  ializer.........
+000051a0: 87ba e88d afe5 9381 e79b aee5 bd95 e5ba  ................
+000051b0: 8fe5 8897 e58c 96e5 99a8 f50c 0000 00e5  ................
+000051c0: 88b6 e589 82e7 b1bb e59e 8b72 a700 0000  ...........r....
+000051d0: f506 0000 00e5 8886 e7b1 bbf5 0c00 0000  ................
+000051e0: e88d afe5 9381 e7b1 bbe5 9e8b 6300 0000  ............c...
+000051f0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00005200: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
+00005210: 5a02 6503 5a04 6401 5a05 6402 5300 2903  Z.e.Z.d.Z.d.S.).
+00005220: 7a22 4578 706f 7274 4472 7567 4469 7265  z"ExportDrugDire
+00005230: 6374 6f72 7953 6572 6961 6c69 7a65 722e  ctorySerializer.
+00005240: 4d65 7461 2913 da09 6472 7567 5f63 6f64  Meta)...drug_cod
+00005250: 65da 0964 7275 675f 6e61 6d65 da09 7374  e..drug_name..st
+00005260: 616e 6461 7264 73da 0575 6e69 7473 da15  andards..units..
+00005270: 7072 6570 6172 6174 696f 6e5f 7479 7065  preparation_type
+00005280: 5f6e 616d 65da 0e64 7275 675f 7479 7065  _name..drug_type
+00005290: 5f6e 616d 65da 0d63 6174 6567 6f72 795f  _name..category_
+000052a0: 6e61 6d65 da0c 6f72 6967 696e 5f70 6c61  name..origin_pla
+000052b0: 6365 da0c 6d61 6e75 6661 6374 7572 6572  ce..manufacturer
+000052c0: da09 756e 6974 5f64 6f73 65da 0c6d 6561  ..unit_dose..mea
+000052d0: 7375 7265 5f75 6e69 74da 0a73 746f 636b  sure_unit..stock
+000052e0: 5f6c 6566 74da 0a73 746f 636b 5f75 6e69  _left..stock_uni
+000052f0: 74da 036d 6963 da0c 7263 635f 6361 7465  t..mic..rcc_cate
+00005300: 676f 7279 da0c 6973 5f65 7373 656e 7469  gory..is_essenti
+00005310: 616c da08 6872 5f6c 6576 656c da07 6762  al..hr_level..gb
+00005320: 5f63 6f64 65da 0767 625f 6e61 6d65 4ea9  _code..gb_nameN.
+00005330: 0672 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+00005340: 720e 0000 0072 2200 0000 7223 0000 0072  r....r"...r#...r
+00005350: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
+00005360: 0000 0072 2700 0000 6c02 0000 7304 0000  ...r'...l...s...
+00005370: 0008 0104 0172 2700 0000 6302 0000 0000  .....r'...c.....
+00005380: 0000 0000 0000 0003 0000 0001 0000 0043  ...............C
+00005390: 0000 0073 1400 0000 7c01 6a00 7d02 7c02  ...s....|.j.}.|.
+000053a0: 7210 7c02 6a01 5300 6400 5300 724a 0000  r.|.j.S.d.S.rJ..
+000053b0: 00a9 02da 1070 7265 7061 7261 7469 6f6e  .....preparation
+000053c0: 5f74 7970 65da 0974 7970 655f 6e61 6d65  _type..type_name
+000053d0: a903 7234 0000 0072 3500 0000 7218 0100  ..r4...r5...r...
+000053e0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+000053f0: da19 6765 745f 7072 6570 6172 6174 696f  ..get_preparatio
+00005400: 6e5f 7479 7065 5f6e 616d 6584 0200 0073  n_type_name....s
+00005410: 0600 0000 0001 0601 0401 7a37 4578 706f  ..........z7Expo
+00005420: 7274 4472 7567 4469 7265 6374 6f72 7953  rtDrugDirectoryS
+00005430: 6572 6961 6c69 7a65 722e 6765 745f 7072  erializer.get_pr
+00005440: 6570 6172 6174 696f 6e5f 7479 7065 5f6e  eparation_type_n
+00005450: 616d 6563 0200 0000 0000 0000 0000 0000  amec............
+00005460: 0300 0000 0100 0000 4300 0000 7314 0000  ........C...s...
+00005470: 007c 016a 007d 027c 0272 107c 026a 0153  .|.j.}.|.r.|.j.S
+00005480: 0064 0053 0072 4a00 0000 a902 da08 6361  .d.S.rJ.......ca
+00005490: 7465 676f 7279 7209 0100 00a9 0372 3400  tegoryr......r4.
+000054a0: 0000 7235 0000 0072 1d01 0000 7225 0000  ..r5...r....r%..
+000054b0: 0072 2500 0000 7226 0000 00da 1167 6574  .r%...r&.....get
+000054c0: 5f63 6174 6567 6f72 795f 6e61 6d65 8902  _category_name..
+000054d0: 0000 7306 0000 0000 0106 0104 017a 2f45  ..s..........z/E
+000054e0: 7870 6f72 7444 7275 6744 6972 6563 746f  xportDrugDirecto
+000054f0: 7279 5365 7269 616c 697a 6572 2e67 6574  rySerializer.get
+00005500: 5f63 6174 6567 6f72 795f 6e61 6d65 6302  _category_namec.
+00005510: 0000 0000 0000 0000 0000 0003 0000 0001  ................
+00005520: 0000 0043 0000 0073 1400 0000 7c01 6a00  ...C...s....|.j.
+00005530: 7d02 7c02 7210 7c02 6a01 5300 6400 5300  }.|.r.|.j.S.d.S.
+00005540: 724a 0000 00a9 02da 0964 7275 675f 7479  rJ.......drug_ty
+00005550: 7065 7276 0000 00a9 0372 3400 0000 7235  perv.....r4...r5
+00005560: 0000 0072 2101 0000 7225 0000 0072 2500  ...r!...r%...r%.
+00005570: 0000 7226 0000 00da 1267 6574 5f64 7275  ..r&.....get_dru
+00005580: 675f 7479 7065 5f6e 616d 658e 0200 0073  g_type_name....s
+00005590: 0600 0000 0001 0601 0401 7a30 4578 706f  ..........z0Expo
+000055a0: 7274 4472 7567 4469 7265 6374 6f72 7953  rtDrugDirectoryS
+000055b0: 6572 6961 6c69 7a65 722e 6765 745f 6472  erializer.get_dr
+000055c0: 7567 5f74 7970 655f 6e61 6d65 4e29 0d72  ug_type_nameN).r
+000055d0: 1f00 0000 7220 0000 0072 2100 0000 7229  ....r ...r!...r)
+000055e0: 0000 0072 0500 0000 723a 0000 0072 0701  ...r....r:...r..
+000055f0: 0000 7209 0100 0072 0801 0000 7227 0000  ..r....r....r'..
+00005600: 0072 1b01 0000 721f 0100 0072 2301 0000  .r....r....r#...
+00005610: 7225 0000 0072 2500 0000 7225 0000 0072  r%...r%...r%...r
+00005620: 2600 0000 72fe 0000 0065 0200 0073 1000  &...r....e...s..
+00005630: 0000 0801 0402 0c01 0c01 0c02 0e18 0805  ................
+00005640: 0805 72fe 0000 0063 0000 0000 0000 0000  ..r....c........
+00005650: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00005660: 732e 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00005670: 0365 04a0 05a1 005a 0647 0064 0264 0384  .e.....Z.G.d.d..
+00005680: 0064 0383 025a 0764 0464 0584 005a 0864  .d...Z.d.d...Z.d
+00005690: 0653 0029 07da 1c50 6861 726d 6163 794d  .S.)...PharmacyM
+000056a0: 616e 6167 656d 656e 7453 6572 6961 6c69  anagementSeriali
+000056b0: 7a65 7275 1800 0000 e88d afe6 88bf e7ae  zeru............
+000056c0: a1e7 9086 e5ba 8fe5 8897 e58c 96e5 99a8  ................
+000056d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000056e0: 0001 0000 0040 0000 0073 1800 0000 6500  .....@...s....e.
+000056f0: 5a01 6400 5a02 6503 5a04 6401 5a05 6402  Z.d.Z.e.Z.d.Z.d.
+00005700: 5a06 6403 5300 2904 7a21 5068 6172 6d61  Z.d.S.).z!Pharma
+00005710: 6379 4d61 6e61 6765 6d65 6e74 5365 7269  cyManagementSeri
+00005720: 616c 697a 6572 2e4d 6574 6129 06da 0d70  alizer.Meta)...p
+00005730: 6861 726d 6163 795f 636f 6465 da0d 7068  harmacy_code..ph
+00005740: 6172 6d61 6379 5f6e 616d 65da 0d70 6861  armacy_name..pha
+00005750: 726d 6163 795f 7479 7065 72aa 0000 00da  rmacy_typer.....
+00005760: 0b62 656c 6f6e 675f 756e 6974 72e4 0000  .belong_unitr...
+00005770: 00e9 0200 0000 4e29 0772 1f00 0000 7220  ......N).r....r 
+00005780: 0000 0072 2100 0000 7211 0000 0072 2200  ...r!...r....r".
+00005790: 0000 7223 0000 00da 0564 6570 7468 7225  ..r#.....depthr%
+000057a0: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
+000057b0: 0000 7227 0000 0098 0200 0073 0600 0000  ..r'.......s....
+000057c0: 0801 0401 0408 7227 0000 0063 0200 0000  ......r'...c....
+000057d0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+000057e0: 4300 0000 732c 0000 007c 016a 006a 0164  C...s,...|.j.j.d
+000057f0: 016b 0272 147c 016a 026a 0353 007c 016a  .k.r.|.j.j.S.|.j
+00005800: 006a 0164 026b 0272 287c 016a 046a 0353  .j.d.k.r(|.j.j.S
+00005810: 0064 0053 0029 034e 7281 0000 0072 2901  .d.S.).Nr....r).
+00005820: 0000 2905 7227 0100 0072 3f00 0000 72c0  ..).r'...r?...r.
+00005830: 0000 0072 7600 0000 da0a 656e 7465 7270  ...rv.....enterp
+00005840: 7269 7365 7284 0000 0072 2500 0000 7225  riser....r%...r%
+00005850: 0000 0072 2600 0000 da0f 6765 745f 6265  ...r&.....get_be
+00005860: 6c6f 6e67 5f75 6e69 74a4 0200 0073 0800  long_unit....s..
+00005870: 0000 0001 0c01 0801 0c01 7a2c 5068 6172  ..........z,Phar
+00005880: 6d61 6379 4d61 6e61 6765 6d65 6e74 5365  macyManagementSe
+00005890: 7269 616c 697a 6572 2e67 6574 5f62 656c  rializer.get_bel
+000058a0: 6f6e 675f 756e 6974 4e29 0972 1f00 0000  ong_unitN).r....
+000058b0: 7220 0000 0072 2100 0000 7229 0000 0072  r ...r!...r)...r
+000058c0: 0500 0000 723a 0000 0072 2801 0000 7227  ....r:...r(...r'
+000058d0: 0000 0072 2c01 0000 7225 0000 0072 2500  ...r,...r%...r%.
+000058e0: 0000 7225 0000 0072 2600 0000 7224 0100  ..r%...r&...r$..
+000058f0: 0094 0200 0073 0800 0000 0801 0401 0802  .....s..........
+00005900: 0e0c 7224 0100 0063 0000 0000 0000 0000  ..r$...c........
+00005910: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00005920: 7396 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00005930: 0365 046a 0564 0264 038d 015a 0665 046a  .e.j.d.d...Z.e.j
+00005940: 0564 0464 038d 015a 0765 046a 0564 0564  .d.d...Z.e.j.d.d
+00005950: 038d 015a 0865 046a 0564 0664 038d 015a  ...Z.e.j.d.d...Z
+00005960: 0965 046a 0564 0764 038d 015a 0a65 046a  .e.j.d.d...Z.e.j
+00005970: 0564 0864 038d 015a 0b47 0064 0964 0a84  .d.d...Z.G.d.d..
+00005980: 0064 0a83 025a 0c64 0b64 0c84 005a 0d64  .d...Z.d.d...Z.d
+00005990: 0d64 0e84 005a 0e64 0f64 1084 005a 0f64  .d...Z.d.d...Z.d
+000059a0: 1164 1284 005a 1064 1364 1484 005a 1164  .d...Z.d.d...Z.d
+000059b0: 1564 1684 005a 1264 1753 0029 18da 1445  .d...Z.d.S.)...E
+000059c0: 7870 6f72 7455 7365 7253 6572 6961 6c69  xportUserSeriali
+000059d0: 7a65 7275 2200 0000 0a20 2020 20e5 afbc  zeru"....    ...
+000059e0: e587 bae7 94a8 e688 b7e5 ba8f e588 97e5  ................
+000059f0: 8c96 e599 a80a 2020 2020 72d1 0000 0072  ......    r....r
+00005a00: a700 0000 72d4 0000 0075 0600 0000 e881  ....r....u......
+00005a10: 8ce7 baa7 750c 0000 00e7 bb91 e5ae 9ae5  ....u...........
+00005a20: 8cbb e794 9f75 1500 0000 e698 afe5 90a6  .....u..........
+00005a30: e4ba 92e8 8194 e7bd 91e6 8ea5 e8af 8a75  ...............u
+00005a40: 0c00 0000 e794 a8e6 88b7 e8a7 92e8 89b2  ................
+00005a50: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00005a60: 0001 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
+00005a70: 5a01 6400 5a02 6503 5a04 6401 5a05 6402  Z.d.Z.e.Z.d.Z.d.
+00005a80: 5300 2903 7a19 4578 706f 7274 5573 6572  S.).z.ExportUser
+00005a90: 5365 7269 616c 697a 6572 2e4d 6574 6129  Serializer.Meta)
+00005aa0: 0872 c000 0000 72bc 0000 00da 0664 6f63  .r....r......doc
+00005ab0: 746f 72da 0975 7365 725f 7261 6e6b 729c  tor..user_rankr.
+00005ac0: 0000 0072 8c00 0000 72d9 0000 00da 0667  ...r....r......g
+00005ad0: 726f 7570 734e 729b 0000 0072 2500 0000  roupsNr....r%...
+00005ae0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
+00005af0: 2700 0000 b602 0000 7304 0000 0008 0104  '.......s.......
+00005b00: 0272 2700 0000 6302 0000 0000 0000 0000  .r'...c.........
+00005b10: 0000 0004 0000 0003 0000 0003 0000 0073  ...............s
+00005b20: 2a00 0000 7c01 6a00 a001 a100 8900 8700  *...|.j.........
+00005b30: 6601 6401 6402 8408 8800 4400 8301 7d02  f.d.d.....D...}.
+00005b40: 6403 a002 7c02 a101 7d03 7c03 5300 2904  d...|...}.|.S.).
+00005b50: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00005b60: 0000 0300 0000 1300 0000 7316 0000 0067  ..........s....g
+00005b70: 007c 005d 0e7d 0188 0072 047c 016a 0091  .|.].}...r.|.j..
+00005b80: 0271 0453 0072 2500 0000 2901 7276 0000  .q.S.r%...).rv..
+00005b90: 0029 0272 6500 0000 72e7 0000 00a9 0172  .).re...r......r
+00005ba0: 3001 0000 7225 0000 0072 2600 0000 7266  0...r%...r&...rf
+00005bb0: 0000 00c6 0200 0072 5700 0000 7a33 4578  .......rW...z3Ex
+00005bc0: 706f 7274 5573 6572 5365 7269 616c 697a  portUserSerializ
+00005bd0: 6572 2e67 6574 5f67 726f 7570 732e 3c6c  er.get_groups.<l
+00005be0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00005bf0: 3efa 012c 2903 7230 0100 0072 4500 0000  >..,).r0...rE...
+00005c00: da04 6a6f 696e 2904 7234 0000 0072 3500  ..join).r4...r5.
+00005c10: 0000 5a09 726f 6c65 5f6c 6973 745a 0872  ..Z.role_listZ.r
+00005c20: 6f6c 655f 7374 7272 2500 0000 7231 0100  ole_strr%...r1..
+00005c30: 0072 2600 0000 da0a 6765 745f 6772 6f75  .r&.....get_grou
+00005c40: 7073 c402 0000 7308 0000 0000 010a 0112  ps....s.........
+00005c50: 010a 017a 1f45 7870 6f72 7455 7365 7253  ...z.ExportUserS
+00005c60: 6572 6961 6c69 7a65 722e 6765 745f 6772  erializer.get_gr
+00005c70: 6f75 7073 6302 0000 0000 0000 0000 0000  oupsc...........
+00005c80: 0003 0000 0001 0000 0043 0000 0073 1400  .........C...s..
+00005c90: 0000 7c01 6a00 7d02 7c02 7210 7c02 6a01  ..|.j.}.|.r.|.j.
+00005ca0: 5300 6400 5300 724a 0000 0072 c200 0000  S.d.S.rJ...r....
+00005cb0: 72da 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
+00005cc0: 2600 0000 72d2 0000 00ca 0200 0073 0600  &...r........s..
+00005cd0: 0000 0001 0601 0401 7a21 4578 706f 7274  ........z!Export
+00005ce0: 5573 6572 5365 7269 616c 697a 6572 2e67  UserSerializer.g
+00005cf0: 6574 5f68 6f73 7069 7461 6c63 0200 0000  et_hospitalc....
+00005d00: 0000 0000 0000 0000 0300 0000 0100 0000  ................
+00005d10: 4300 0000 7314 0000 007c 016a 007d 027c  C...s....|.j.}.|
+00005d20: 0272 107c 026a 0153 0064 0053 0072 4a00  .r.|.j.S.d.S.rJ.
+00005d30: 0000 72be 0000 0072 db00 0000 7225 0000  ..r....r....r%..
+00005d40: 0072 2500 0000 7226 0000 0072 dc00 0000  .r%...r&...r....
+00005d50: cf02 0000 7306 0000 0000 0106 0104 017a  ....s..........z
+00005d60: 1f45 7870 6f72 7455 7365 7253 6572 6961  .ExportUserSeria
+00005d70: 6c69 7a65 722e 6765 745f 6f66 6669 6365  lizer.get_office
+00005d80: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00005d90: 0001 0000 0043 0000 0073 1400 0000 7c01  .....C...s....|.
+00005da0: 6a00 7d02 7c02 7210 7c02 6a01 5300 6400  j.}.|.r.|.j.S.d.
+00005db0: 5300 724a 0000 0029 0272 2f01 0000 7276  S.rJ...).r/...rv
+00005dc0: 0000 0029 0372 3400 0000 7235 0000 0072  ...).r4...r5...r
+00005dd0: 2f01 0000 7225 0000 0072 2500 0000 7226  /...r%...r%...r&
+00005de0: 0000 00da 0d67 6574 5f75 7365 725f 7261  .....get_user_ra
+00005df0: 6e6b d402 0000 7306 0000 0000 0106 0104  nk....s.........
+00005e00: 017a 2245 7870 6f72 7455 7365 7253 6572  .z"ExportUserSer
+00005e10: 6961 6c69 7a65 722e 6765 745f 7573 6572  ializer.get_user
+00005e20: 5f72 616e 6b63 0200 0000 0000 0000 0000  _rankc..........
+00005e30: 0000 0300 0000 0100 0000 4300 0000 7314  ..........C...s.
+00005e40: 0000 007c 016a 007d 027c 0272 107c 026a  ...|.j.}.|.r.|.j
+00005e50: 0153 0064 0053 0072 4a00 0000 2902 722e  .S.d.S.rJ...).r.
+00005e60: 0100 0072 7600 0000 a903 7234 0000 0072  ...rv.....r4...r
+00005e70: 3500 0000 722e 0100 0072 2500 0000 7225  5...r....r%...r%
+00005e80: 0000 0072 2600 0000 da0a 6765 745f 646f  ...r&.....get_do
+00005e90: 6374 6f72 d902 0000 7306 0000 0000 0106  ctor....s.......
+00005ea0: 0104 017a 1f45 7870 6f72 7455 7365 7253  ...z.ExportUserS
+00005eb0: 6572 6961 6c69 7a65 722e 6765 745f 646f  erializer.get_do
+00005ec0: 6374 6f72 6302 0000 0000 0000 0000 0000  ctorc...........
+00005ed0: 0003 0000 0001 0000 0043 0000 0073 1400  .........C...s..
+00005ee0: 0000 7c01 6a00 7d02 7c02 7210 7c02 6a01  ..|.j.}.|.r.|.j.
+00005ef0: 5300 6400 5300 724a 0000 0029 0272 2e01  S.d.S.rJ...).r..
+00005f00: 0000 72d9 0000 0072 3601 0000 7225 0000  ..r....r6...r%..
+00005f10: 0072 2500 0000 7226 0000 00da 1567 6574  .r%...r&.....get
+00005f20: 5f69 735f 6f6e 6c69 6e65 5f63 6f6e 7375  _is_online_consu
+00005f30: 6c74 de02 0000 7306 0000 0000 0106 0104  lt....s.........
+00005f40: 017a 2a45 7870 6f72 7455 7365 7253 6572  .z*ExportUserSer
+00005f50: 6961 6c69 7a65 722e 6765 745f 6973 5f6f  ializer.get_is_o
+00005f60: 6e6c 696e 655f 636f 6e73 756c 744e 2913  nline_consultN).
+00005f70: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+00005f80: 2900 0000 7205 0000 0072 3a00 0000 72c0  )...r....r:...r.
+00005f90: 0000 0072 bc00 0000 722f 0100 0072 2e01  ...r....r/...r..
+00005fa0: 0000 72d9 0000 0072 3001 0000 7227 0000  ..r....r0...r'..
+00005fb0: 0072 3401 0000 72d2 0000 0072 dc00 0000  .r4...r....r....
+00005fc0: 7235 0100 0072 3701 0000 7238 0100 0072  r5...r7...r8...r
+00005fd0: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
+00005fe0: 0000 0072 2d01 0000 ab02 0000 731c 0000  ...r-.......s...
+00005ff0: 0008 0104 030c 010c 010c 010c 010c 010c  ................
+00006000: 020e 0e08 0608 0508 0508 0508 0572 2d01  .............r-.
+00006010: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00006020: 0000 0003 0000 0040 0000 0073 4a00 0000  .......@...sJ...
+00006030: 6500 5a01 6400 5a02 6503 a004 a100 5a05  e.Z.d.Z.e.....Z.
+00006040: 6503 a004 a100 5a06 6503 a004 a100 5a07  e.....Z.e.....Z.
+00006050: 4700 6401 6402 8400 6402 8302 5a08 6403  G.d.d...d...Z.d.
+00006060: 6404 8400 5a09 6405 6406 8400 5a0a 6407  d...Z.d.d...Z.d.
+00006070: 6408 8400 5a0b 6409 5300 290a da17 4472  d...Z.d.S.)...Dr
+00006080: 7567 4469 7265 6374 6f72 7953 6572 6961  ugDirectorySeria
+00006090: 6c69 7a65 7263 0000 0000 0000 0000 0000  lizerc..........
+000060a0: 0000 0000 0000 0100 0000 4000 0000 7314  ..........@...s.
+000060b0: 0000 0065 005a 0164 005a 0265 035a 0464  ...e.Z.d.Z.e.Z.d
+000060c0: 015a 0564 0253 0029 037a 1c44 7275 6744  .Z.d.S.).z.DrugD
+000060d0: 6972 6563 746f 7279 5365 7269 616c 697a  irectorySerializ
+000060e0: 6572 2e4d 6574 6172 1c00 0000 4e72 1601  er.Metar....Nr..
+000060f0: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
+00006100: 0072 2600 0000 7227 0000 00e9 0200 0073  .r&...r'.......s
+00006110: 0400 0000 0801 0401 7227 0000 0063 0200  ........r'...c..
+00006120: 0000 0000 0000 0000 0000 0300 0000 0100  ................
+00006130: 0000 4300 0000 7314 0000 007c 016a 007d  ..C...s....|.j.}
+00006140: 027c 0272 107c 026a 0153 0064 0053 0072  .|.r.|.j.S.d.S.r
+00006150: 4a00 0000 7217 0100 0072 1a01 0000 7225  J...r....r....r%
+00006160: 0000 0072 2500 0000 7226 0000 00da 1467  ...r%...r&.....g
+00006170: 6574 5f70 7265 7061 7261 7469 6f6e 5f74  et_preparation_t
+00006180: 7970 65ed 0200 0073 0600 0000 0001 0601  ype....s........
+00006190: 0401 7a2c 4472 7567 4469 7265 6374 6f72  ..z,DrugDirector
+000061a0: 7953 6572 6961 6c69 7a65 722e 6765 745f  ySerializer.get_
+000061b0: 7072 6570 6172 6174 696f 6e5f 7479 7065  preparation_type
+000061c0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+000061d0: 0001 0000 0043 0000 0073 1400 0000 7c01  .....C...s....|.
+000061e0: 6a00 7d02 7c02 7210 7c02 6a01 5300 6400  j.}.|.r.|.j.S.d.
+000061f0: 5300 724a 0000 0072 2001 0000 7222 0100  S.rJ...r ...r"..
+00006200: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00006210: da0d 6765 745f 6472 7567 5f74 7970 65f2  ..get_drug_type.
+00006220: 0200 0073 0600 0000 0001 0601 0401 7a25  ...s..........z%
+00006230: 4472 7567 4469 7265 6374 6f72 7953 6572  DrugDirectorySer
+00006240: 6961 6c69 7a65 722e 6765 745f 6472 7567  ializer.get_drug
+00006250: 5f74 7970 6563 0200 0000 0000 0000 0000  _typec..........
+00006260: 0000 0300 0000 0100 0000 4300 0000 7314  ..........C...s.
+00006270: 0000 007c 016a 007d 027c 0272 107c 026a  ...|.j.}.|.r.|.j
+00006280: 0153 0064 0053 0072 4a00 0000 721c 0100  .S.d.S.rJ...r...
+00006290: 0072 1e01 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+000062a0: 7226 0000 0072 1f01 0000 f702 0000 7306  r&...r........s.
+000062b0: 0000 0000 0106 0104 017a 2944 7275 6744  .........z)DrugD
+000062c0: 6972 6563 746f 7279 5365 7269 616c 697a  irectorySerializ
+000062d0: 6572 2e67 6574 5f63 6174 6567 6f72 795f  er.get_category_
+000062e0: 6e61 6d65 4e29 0c72 1f00 0000 7220 0000  nameN).r....r ..
+000062f0: 0072 2100 0000 7205 0000 0072 3a00 0000  .r!...r....r:...
+00006300: 7218 0100 0072 2101 0000 7209 0100 0072  r....r!...r....r
+00006310: 2700 0000 723a 0100 0072 3b01 0000 721f  '...r:...r;...r.
+00006320: 0100 0072 2500 0000 7225 0000 0072 2500  ...r%...r%...r%.
+00006330: 0000 7226 0000 0072 3901 0000 e402 0000  ..r&...r9.......
+00006340: 730e 0000 0008 0108 0108 0108 020e 0408  s...............
+00006350: 0508 0572 3901 0000 6300 0000 0000 0000  ...r9...c.......
+00006360: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00006370: 0073 1e00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00006380: 5a03 4700 6402 6403 8400 6403 8302 5a04  Z.G.d.d...d...Z.
+00006390: 6404 5300 2905 da11 4170 6949 6e66 6f53  d.S.)...ApiInfoS
+000063a0: 6572 6961 6c69 7a65 7275 2200 0000 0a20  erializeru".... 
+000063b0: 2020 20e5 9b9e e586 99e5 8f82 e695 b0e5     .............
+000063c0: ba8f e588 97e5 8c96 e599 a80a 2020 2020  ............    
+000063d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000063e0: 0001 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
+000063f0: 5a01 6400 5a02 6503 5a04 6401 5a05 6402  Z.d.Z.e.Z.d.Z.d.
+00006400: 5300 2903 7a16 4170 6949 6e66 6f53 6572  S.).z.ApiInfoSer
+00006410: 6961 6c69 7a65 722e 4d65 7461 721c 0000  ializer.Metar...
+00006420: 004e 2906 721f 0000 0072 2000 0000 7221  .N).r....r ...r!
+00006430: 0000 0072 1200 0000 7222 0000 0072 2300  ...r....r"...r#.
+00006440: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
+00006450: 0072 2600 0000 7227 0000 0002 0300 0073  .r&...r'.......s
+00006460: 0400 0000 0801 0401 7227 0000 004e 7228  ........r'...Nr(
+00006470: 0000 0072 2500 0000 7225 0000 0072 2500  ...r%...r%...r%.
+00006480: 0000 7226 0000 0072 3c01 0000 fd02 0000  ..r&...r<.......
+00006490: 7304 0000 0008 0104 0472 3c01 0000 6300  s........r<...c.
+000064a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+000064b0: 0000 0040 0000 0073 6e00 0000 6500 5a01  ...@...sn...e.Z.
+000064c0: 6400 5a02 6401 5a03 6504 6a05 6402 6403  d.Z.d.Z.e.j.d.d.
+000064d0: 8d01 5a06 6504 6a05 6404 6403 8d01 5a07  ..Z.e.j.d.d...Z.
+000064e0: 6504 6a05 6405 6403 8d01 5a08 6504 6a05  e.j.d.d...Z.e.j.
+000064f0: 6406 6403 8d01 5a09 4700 6407 6408 8400  d.d...Z.G.d.d...
+00006500: 6408 8302 5a0a 6409 640a 8400 5a0b 640b  d...Z.d.d...Z.d.
+00006510: 640c 8400 5a0c 640d 640e 8400 5a0d 640f  d...Z.d.d...Z.d.
+00006520: 6410 8400 5a0e 6411 5300 2912 da1c 4578  d...Z.d.S.)...Ex
+00006530: 706f 7274 5068 6172 6d61 6379 4472 7567  portPharmacyDrug
+00006540: 5365 7269 616c 697a 6572 72ff 0000 0072  Serializerr....r
+00006550: 0001 0000 72a7 0000 0075 0c00 0000 e88d  ....r....u......
+00006560: afe6 88bf e590 8de7 a7b0 7201 0100 0072  ..........r....r
+00006570: 0201 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00006580: 0000 0000 0001 0000 0040 0000 0073 1400  .........@...s..
+00006590: 0000 6500 5a01 6400 5a02 6503 5a04 6401  ..e.Z.d.Z.e.Z.d.
+000065a0: 5a05 6402 5300 2903 7a21 4578 706f 7274  Z.d.S.).z!Export
+000065b0: 5068 6172 6d61 6379 4472 7567 5365 7269  PharmacyDrugSeri
+000065c0: 616c 697a 6572 2e4d 6574 6129 1172 2601  alizer.Meta).r&.
+000065d0: 0000 7203 0100 0072 0401 0000 7205 0100  ..r....r....r...
+000065e0: 0072 0701 0000 7208 0100 0072 0901 0000  .r....r....r....
+000065f0: 720a 0100 0072 0b01 0000 da0a 7661 6c69  r....r......vali
+00006600: 645f 6461 7465 da12 696e 7665 6e74 6f72  d_date..inventor
+00006610: 795f 7175 616e 7469 7479 da10 6d65 6173  y_quantity..meas
+00006620: 7572 656d 656e 745f 756e 6974 da0f 636f  urement_unit..co
+00006630: 7374 5f75 6e69 745f 7072 6963 65da 0b63  st_unit_price..c
+00006640: 6f73 745f 616d 6f75 6e74 da11 7265 7461  ost_amount..reta
+00006650: 696c 5f75 6e69 745f 7072 6963 65da 0d72  il_unit_price..r
+00006660: 6574 6169 6c5f 616d 6f75 6e74 72e4 0000  etail_amountr...
+00006670: 004e 2906 721f 0000 0072 2000 0000 7221  .N).r....r ...r!
+00006680: 0000 0072 1300 0000 7222 0000 0072 2300  ...r....r"...r#.
+00006690: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
+000066a0: 0072 2600 0000 7227 0000 000e 0300 0073  .r&...r'.......s
+000066b0: 0400 0000 0801 0401 7227 0000 0063 0200  ........r'...c..
+000066c0: 0000 0000 0000 0000 0000 0300 0000 0100  ................
+000066d0: 0000 4300 0000 7314 0000 007c 016a 007d  ..C...s....|.j.}
+000066e0: 027c 0272 107c 026a 0153 0064 0053 0072  .|.r.|.j.S.d.S.r
+000066f0: 4a00 0000 7217 0100 0072 1a01 0000 7225  J...r....r....r%
+00006700: 0000 0072 2500 0000 7226 0000 0072 1b01  ...r%...r&...r..
+00006710: 0000 2403 0000 7306 0000 0000 0106 0104  ..$...s.........
+00006720: 017a 3645 7870 6f72 7450 6861 726d 6163  .z6ExportPharmac
+00006730: 7944 7275 6753 6572 6961 6c69 7a65 722e  yDrugSerializer.
+00006740: 6765 745f 7072 6570 6172 6174 696f 6e5f  get_preparation_
+00006750: 7479 7065 5f6e 616d 6563 0200 0000 0000  type_namec......
+00006760: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+00006770: 0000 7312 0000 007c 016a 0072 0e7c 016a  ..s....|.j.r.|.j
+00006780: 006a 0153 0064 0053 0072 4a00 0000 2902  .j.S.d.S.rJ...).
+00006790: da08 7068 6172 6d61 6379 7226 0100 0072  ..pharmacyr&...r
+000067a0: 8400 0000 7225 0000 0072 2500 0000 7226  ....r%...r%...r&
+000067b0: 0000 00da 1167 6574 5f70 6861 726d 6163  .....get_pharmac
+000067c0: 795f 6e61 6d65 2903 0000 7304 0000 0000  y_name)...s.....
+000067d0: 0106 017a 2e45 7870 6f72 7450 6861 726d  ...z.ExportPharm
+000067e0: 6163 7944 7275 6753 6572 6961 6c69 7a65  acyDrugSerialize
+000067f0: 722e 6765 745f 7068 6172 6d61 6379 5f6e  r.get_pharmacy_n
+00006800: 616d 6563 0200 0000 0000 0000 0000 0000  amec............
+00006810: 0300 0000 0100 0000 4300 0000 7314 0000  ........C...s...
+00006820: 007c 016a 007d 027c 0272 107c 026a 0153  .|.j.}.|.r.|.j.S
+00006830: 0064 0053 0072 4a00 0000 721c 0100 0072  .d.S.rJ...r....r
+00006840: 1e01 0000 7225 0000 0072 2500 0000 7226  ....r%...r%...r&
+00006850: 0000 0072 1f01 0000 2d03 0000 7306 0000  ...r....-...s...
+00006860: 0000 0106 0104 017a 2e45 7870 6f72 7450  .......z.ExportP
+00006870: 6861 726d 6163 7944 7275 6753 6572 6961  harmacyDrugSeria
+00006880: 6c69 7a65 722e 6765 745f 6361 7465 676f  lizer.get_catego
+00006890: 7279 5f6e 616d 6563 0200 0000 0000 0000  ry_namec........
+000068a0: 0000 0000 0300 0000 0100 0000 4300 0000  ............C...
+000068b0: 7314 0000 007c 016a 007d 027c 0272 107c  s....|.j.}.|.r.|
+000068c0: 026a 0153 0064 0053 0072 4a00 0000 7220  .j.S.d.S.rJ...r 
+000068d0: 0100 0072 2201 0000 7225 0000 0072 2500  ...r"...r%...r%.
+000068e0: 0000 7226 0000 0072 2301 0000 3203 0000  ..r&...r#...2...
+000068f0: 7306 0000 0000 0106 0104 017a 2f45 7870  s..........z/Exp
+00006900: 6f72 7450 6861 726d 6163 7944 7275 6753  ortPharmacyDrugS
+00006910: 6572 6961 6c69 7a65 722e 6765 745f 6472  erializer.get_dr
+00006920: 7567 5f74 7970 655f 6e61 6d65 4e29 0f72  ug_type_nameN).r
+00006930: 1f00 0000 7220 0000 0072 2100 0000 7229  ....r ...r!...r)
+00006940: 0000 0072 0500 0000 723a 0000 0072 0701  ...r....r:...r..
+00006950: 0000 7226 0100 0072 0901 0000 7208 0100  ..r&...r....r...
+00006960: 0072 2700 0000 721b 0100 0072 4601 0000  .r'...r....rF...
+00006970: 721f 0100 0072 2301 0000 7225 0000 0072  r....r#...r%...r
+00006980: 2500 0000 7225 0000 0072 2600 0000 723d  %...r%...r&...r=
+00006990: 0100 0007 0300 0073 1400 0000 0801 0401  .......s........
+000069a0: 0c01 0c01 0c01 0c02 0e16 0805 0804 0805  ................
+000069b0: 723d 0100 004e 2940 da0b 646a 616e 676f  r=...N)@..django
+000069c0: 2e63 6f6e 6672 0200 0000 da1a 646a 616e  .confr......djan
+000069d0: 676f 2e63 6f6e 7472 6962 2e61 7574 682e  go.contrib.auth.
+000069e0: 6d6f 6465 6c73 7203 0000 00da 2264 6a61  modelsr....."dja
+000069f0: 6e67 6f2e 636f 6e74 7269 622e 636f 6e74  ngo.contrib.cont
+00006a00: 656e 7474 7970 6573 2e6d 6f64 656c 7372  enttypes.modelsr
+00006a10: 0400 0000 da0e 7265 7374 5f66 7261 6d65  ......rest_frame
+00006a20: 776f 726b 7205 0000 00da 1262 6173 655f  workr......base_
+00006a30: 7379 7374 656d 2e6d 6f64 656c 7372 0600  system.modelsr..
+00006a40: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00006a50: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00006a60: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00006a70: 1000 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+00006a80: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
+00006a90: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00006aa0: 00da 0966 756e 6374 6f6f 6c73 721a 0000  ...functoolsr...
+00006ab0: 00da 0f4d 6f64 656c 5365 7269 616c 697a  ...ModelSerializ
+00006ac0: 6572 721b 0000 0072 2a00 0000 722b 0000  err....r*...r+..
+00006ad0: 0072 3200 0000 7242 0000 0072 4e00 0000  .r2...rB...rN...
+00006ae0: 7251 0000 0072 8300 0000 da0a 5365 7269  rQ...r......Seri
+00006af0: 616c 697a 6572 7286 0000 0072 9a00 0000  alizerr....r....
+00006b00: 72a6 0000 0072 b400 0000 72b5 0000 0072  r....r....r....r
+00006b10: b700 0000 72c9 0000 0072 d000 0000 72d3  ....r....r....r.
+00006b20: 0000 0072 e100 0000 72e2 0000 0072 e900  ...r....r....r..
+00006b30: 0000 72ec 0000 0072 f200 0000 72fa 0000  ..r....r....r...
+00006b40: 0072 fb00 0000 72fd 0000 0072 fe00 0000  .r....r....r....
+00006b50: 7224 0100 0072 2d01 0000 7239 0100 0072  r$...r-...r9...r
+00006b60: 3c01 0000 723d 0100 0072 2500 0000 7225  <...r=...r%...r%
+00006b70: 0000 0072 2500 0000 7226 0000 00da 083c  ...r%...r&.....<
+00006b80: 6d6f 6475 6c65 3e01 0000 0073 4a00 0000  module>....sJ...
+00006b90: 0c01 0c01 0c01 0c01 5403 0c01 0c03 120d  ........T.......
+00006ba0: 120a 1211 120f 121e 120a 1250 120a 1219  ...........P....
+00006bb0: 121e 121c 120b 120a 122b 1206 121f 1232  .........+.....2
+00006bc0: 1217 121e 1210 1214 121d 120f 1214 121d  ................
+00006bd0: 122f 1217 1239 1219 120a                 ./...9....
```

### Comparing `base_system-0.2.3/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.2.4/base_system/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/__pycache__/views.cpython-39.pyc` & `base_system-0.2.4/base_system/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.2.4/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/auth.py` & `base_system-0.2.4/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/export_viewset.py` & `base_system-0.2.4/base_system/export_viewset.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/migrations/0001_initial.py` & `base_system-0.2.4/base_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/migrations/0003_alter_extragroup_hospital.py` & `base_system-0.2.4/base_system/migrations/0003_alter_extragroup_hospital.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc` & `base_system-0.2.4/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc` & `base_system-0.2.4/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc` & `base_system-0.2.4/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc` & `base_system-0.2.4/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/models.py` & `base_system-0.2.4/base_system/models.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/serializers.py` & `base_system-0.2.4/base_system/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,16 +488,17 @@
 
     class Meta:
         model = InspectionType
         fields = "__all__"
 
     def get_children(self, obj):
         children = InspectionType.objects.filter(parent=obj)
-        serializer = InspectionTypeSerializer(children, many=True)
-        return serializer.data
+        if children:
+            serializer = InspectionTypeSerializer(children, many=True)
+            return serializer.data
 
 
 class InspectionDictionariesSerializer(serializers.ModelSerializer):
     """检查字典序列化器"""
     hospital_name = serializers.SerializerMethodField()
     office_name = serializers.SerializerMethodField()
 
@@ -551,16 +552,17 @@
 
     class Meta:
         model = ExaminationType
         fields = "__all__"
 
     def get_children(self, obj):
         children = ExaminationType.objects.filter(parent=obj)
-        serializer = ExaminationTypeSerializer(children, many=True)
-        return serializer.data
+        if children:
+            serializer = ExaminationTypeSerializer(children, many=True)
+            return serializer.data
 
 
 class ExaminationDictionariesSerializer(serializers.ModelSerializer):
     """检验字典序列化器"""
     hospital_name = serializers.SerializerMethodField()
     office_name = serializers.SerializerMethodField()
```

### Comparing `base_system-0.2.3/base_system/urls.py` & `base_system-0.2.4/base_system/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/views.py` & `base_system-0.2.4/base_system/views.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system/viewsets.py` & `base_system-0.2.4/base_system/viewsets.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/base_system.egg-info/PKG-INFO` & `base_system-0.2.4/base_system.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.2.3
+Version: 0.2.4
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.3/base_system.egg-info/SOURCES.txt` & `base_system-0.2.4/base_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/init_data.json` & `base_system-0.2.4/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/manage.py` & `base_system-0.2.4/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/requirements.txt` & `base_system-0.2.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/runtests.py` & `base_system-0.2.4/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.3/setup.py` & `base_system-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.2.3',
+    version='0.2.4',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://github.com/zcjwin",
```

