# Comparing `tmp/base_system-0.2.2.tar.gz` & `tmp/base_system-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.2.2.tar", last modified: Thu May  4 08:35:25 2023, max compression
+gzip compressed data, was "base_system-0.2.3.tar", last modified: Sat May  6 02:27:33 2023, max compression
```

## Comparing `base_system-0.2.2.tar` & `base_system-0.2.3.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.982753 base_system-0.2.2/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.2/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.2/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.938723 base_system-0.2.2/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.2/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.2/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11868 2023-05-04 07:40:22.000000 base_system-0.2.2/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.2/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.2/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.2/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.2/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.2/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 08:35:25.982753 base_system-0.2.2/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.2/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.946728 base_system-0.2.2/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.2/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.966742 base_system-0.2.2/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.2/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.2/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.2/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19488 2023-05-04 08:07:15.000000 base_system-0.2.2/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.2.2/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.2/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.2.2/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    32490 2023-05-04 07:38:29.000000 base_system-0.2.2/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11925 2023-05-04 08:07:17.000000 base_system-0.2.2/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.2/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.2/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.2/base_system/auth.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.974747 base_system-0.2.2/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.2/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.2/base_system/migrations/0002_drugdirectory_code_medu_cur.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.2/base_system/migrations/0003_alter_extragroup_hospital.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.2/base_system/migrations/0004_alter_extragroup_role_name.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.2/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.978750 base_system-0.2.2/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.2/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.2/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.2/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.2/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25535 2023-05-04 08:07:06.000000 base_system-0.2.2/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.2.2/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.2/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.2.2/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    71807 2023-05-04 03:13:44.000000 base_system-0.2.2/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14978 2023-05-04 08:34:21.000000 base_system-0.2.2/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.954734 base_system-0.2.2/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1644 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.2/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.2/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.2/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.2/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.2/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-04 08:35:25.982753 base_system-0.2.2/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-04 08:34:21.000000 base_system-0.2.2/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.770831 base_system-0.2.3/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.3/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.3/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.702796 base_system-0.2.3/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.3/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.3/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11803 2023-05-06 02:25:35.000000 base_system-0.2.3/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.3/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.3/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.3/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.3/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.3/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-06 02:27:33.770831 base_system-0.2.3/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.3/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.710800 base_system-0.2.3/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.3/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.750821 base_system-0.2.3/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.3/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.3/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.3/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.3/base_system/__pycache__/export_viewset.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19488 2023-05-04 08:07:15.000000 base_system-0.2.3/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    27590 2023-05-06 02:21:51.000000 base_system-0.2.3/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.3/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3179 2023-05-06 02:06:30.000000 base_system-0.2.3/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23682 2023-05-06 02:13:02.000000 base_system-0.2.3/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-06 01:27:33.000000 base_system-0.2.3/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.3/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.3/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.3/base_system/auth.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.3/base_system/export_viewset.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.762827 base_system-0.2.3/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.3/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.3/base_system/migrations/0002_drugdirectory_code_medu_cur.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.3/base_system/migrations/0003_alter_extragroup_hospital.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.3/base_system/migrations/0004_alter_extragroup_role_name.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.3/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.766829 base_system-0.2.3/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.3/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.3/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.3/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.3/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.3/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25535 2023-05-04 08:07:06.000000 base_system-0.2.3/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23694 2023-05-06 02:21:50.000000 base_system-0.2.3/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.3/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     4071 2023-05-06 02:06:28.000000 base_system-0.2.3/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    58056 2023-05-06 02:12:59.000000 base_system-0.2.3/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14978 2023-05-04 08:34:21.000000 base_system-0.2.3/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:27:33.726808 base_system-0.2.3/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1810 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.3/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-06 02:27:33.000000 base_system-0.2.3/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.3/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.3/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.3/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.3/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-06 02:27:33.770831 base_system-0.2.3/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-06 02:06:28.000000 base_system-0.2.3/setup.py
```

### Comparing `base_system-0.2.2/.gitignore` & `base_system-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/BaseFunctionModule/settings.py` & `base_system-0.2.3/BaseFunctionModule/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,18 +122,14 @@
         },
     },
 ]
 
 WSGI_APPLICATION = 'BaseFunctionModule.wsgi.application'
 
 
-# 回写院内ip地址
-WRITEBACK_IP = 'http://ycswjw.com:8041'
-
-
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.postgresql_psycopg2',
         'NAME': 'basicdb',
         'USER': 'postgres',
         'PASSWORD': 'postgres',
         'HOST': 'localhost',
```

### Comparing `base_system-0.2.2/BaseFunctionModule/urls.py` & `base_system-0.2.3/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/LICENCE` & `base_system-0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/PKG-INFO` & `base_system-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.2.2
+Version: 0.2.3
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.2/README.rst` & `base_system-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.2.3/base_system/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.2.3/base_system/__pycache__/urls.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 27 02:23:59 2023 UTC, .py size: 3855 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,190 +1,199 @@
-00000000: 610d 0d0a 0000 0000 bfdc 4964 0f0f 0000  a.........Id....
+00000000: 610d 0d0a 0000 0000 24b6 5564 e70f 0000  a.......$.Ud....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 3802 0000 6400  .....@...s8...d.
+00000020: 0012 0000 0040 0000 0073 5802 0000 6400  .....@...sX...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6405 6406 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 0100 6401 6408 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
-00000080: 6409 6c0e 6d0f 5a0f 0100 6401 640a 6c0e  d.l.m.Z...d.d.l.
-00000090: 6d10 5a10 0100 6401 640b 6c0e 6d11 5a11  m.Z...d.d.l.m.Z.
-000000a0: 0100 6504 640c 6509 6a12 8302 6504 640d  ..e.d.e.j...e.d.
-000000b0: 650f 8302 6504 640e 6510 8302 6504 640f  e...e.d.e...e.d.
-000000c0: 6511 8302 6504 6410 650b a013 a100 6411  e...e.d.e.....d.
-000000d0: 6412 8d03 6504 6413 6509 6a14 8302 6504  d...e.d.e.j...e.
-000000e0: 6414 650d 6a15 8302 6504 6415 650d 6a16  d.e.j...e.d.e.j.
-000000f0: 8302 6504 6416 6509 6a17 8302 6504 6417  ..e.d.e.j...e.d.
-00000100: 6509 6a18 8302 6504 6418 6509 6a19 8302  e.j...e.d.e.j...
-00000110: 6504 6419 6509 6a1a 8302 6504 641a 6509  e.d.e.j...e.d.e.
-00000120: 6a1b 8302 6504 641b 6509 6a1c 8302 6504  j...e.d.e.j...e.
-00000130: 641c 6509 6a1d 8302 6504 641d 650d 6a1e  d.e.j...e.d.e.j.
-00000140: 8302 6710 5a1f 6507 a020 a100 5a21 6521  ..g.Z.e.. ..Z!e!
-00000150: a012 641e 6509 6a22 a102 0100 6521 a012  ..d.e.j"....e!..
-00000160: 641f 6509 6a23 a102 0100 6521 a012 6420  d.e.j#....e!..d 
-00000170: 6509 6a24 a102 0100 6521 a012 6421 6509  e.j$....e!..d!e.
-00000180: 6a25 a102 0100 6521 a012 6422 6509 6a26  j%....e!..d"e.j&
-00000190: a102 0100 6521 a012 6423 650d 6a27 a102  ....e!..d#e.j'..
-000001a0: 0100 6521 a012 6424 6509 6a28 a102 0100  ..e!..d$e.j(....
-000001b0: 6521 a012 6425 6509 6a29 a102 0100 6521  e!..d%e.j)....e!
-000001c0: a012 6426 6509 6a2a a102 0100 6521 a012  ..d&e.j*....e!..
-000001d0: 6427 6509 6a2b a102 0100 6521 a012 6428  d'e.j+....e!..d(
-000001e0: 6509 6a2c a102 0100 6521 a012 6429 6509  e.j,....e!..d)e.
-000001f0: 6a2d a102 0100 6521 a012 642a 6509 6a2e  j-....e!..d*e.j.
-00000200: a102 0100 6521 a012 642b 6509 6a2f a102  ....e!..d+e.j/..
-00000210: 0100 6521 a012 642c 6509 6a30 a102 0100  ..e!..d,e.j0....
-00000220: 6521 a012 642d 6509 6a31 a102 0100 6521  e!..d-e.j1....e!
-00000230: a012 642e 650d 6a32 a102 0100 6521 a012  ..d.e.j2....e!..
-00000240: 642f 650d 6a33 a102 0100 6521 a012 6430  d/e.j3....e!..d0
-00000250: 650d 6a34 a102 0100 651f 6521 6a35 3700  e.j4....e.e!j57.
-00000260: 5a1f 6431 5300 2932 6176 0200 004d 6564  Z.d1S.)2av...Med
-00000270: 6963 616c 5379 7374 656d 2055 524c 2043  icalSystem URL C
-00000280: 6f6e 6669 6775 7261 7469 6f6e 0a0a 5468  onfiguration..Th
-00000290: 6520 6075 726c 7061 7474 6572 6e73 6020  e `urlpatterns` 
-000002a0: 6c69 7374 2072 6f75 7465 7320 5552 4c73  list routes URLs
-000002b0: 2074 6f20 7669 6577 732e 2046 6f72 206d   to views. For m
-000002c0: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
-000002d0: 706c 6561 7365 2073 6565 3a0a 2020 2020  please see:.    
-000002e0: 6874 7470 733a 2f2f 646f 6373 2e64 6a61  https://docs.dja
-000002f0: 6e67 6f70 726f 6a65 6374 2e63 6f6d 2f65  ngoproject.com/e
-00000300: 6e2f 342e 312f 746f 7069 6373 2f68 7474  n/4.1/topics/htt
-00000310: 702f 7572 6c73 2f0a 4578 616d 706c 6573  p/urls/.Examples
-00000320: 3a0a 4675 6e63 7469 6f6e 2076 6965 7773  :.Function views
-00000330: 0a20 2020 2031 2e20 4164 6420 616e 2069  .    1. Add an i
-00000340: 6d70 6f72 743a 2020 6672 6f6d 206d 795f  mport:  from my_
-00000350: 6170 7020 696d 706f 7274 2076 6965 7773  app import views
-00000360: 0a20 2020 2032 2e20 4164 6420 6120 5552  .    2. Add a UR
-00000370: 4c20 746f 2075 726c 7061 7474 6572 6e73  L to urlpatterns
-00000380: 3a20 2070 6174 6828 2727 2c20 7669 6577  :  path('', view
-00000390: 732e 686f 6d65 2c20 6e61 6d65 3d27 686f  s.home, name='ho
-000003a0: 6d65 2729 0a43 6c61 7373 2d62 6173 6564  me').Class-based
-000003b0: 2076 6965 7773 0a20 2020 2031 2e20 4164   views.    1. Ad
-000003c0: 6420 616e 2069 6d70 6f72 743a 2020 6672  d an import:  fr
-000003d0: 6f6d 206f 7468 6572 5f61 7070 2e76 6965  om other_app.vie
-000003e0: 7773 2069 6d70 6f72 7420 486f 6d65 0a20  ws import Home. 
-000003f0: 2020 2032 2e20 4164 6420 6120 5552 4c20     2. Add a URL 
-00000400: 746f 2075 726c 7061 7474 6572 6e73 3a20  to urlpatterns: 
-00000410: 2070 6174 6828 2727 2c20 486f 6d65 2e61   path('', Home.a
-00000420: 735f 7669 6577 2829 2c20 6e61 6d65 3d27  s_view(), name='
-00000430: 686f 6d65 2729 0a49 6e63 6c75 6469 6e67  home').Including
-00000440: 2061 6e6f 7468 6572 2055 524c 636f 6e66   another URLconf
-00000450: 0a20 2020 2031 2e20 496d 706f 7274 2074  .    1. Import t
-00000460: 6865 2069 6e63 6c75 6465 2829 2066 756e  he include() fun
-00000470: 6374 696f 6e3a 2066 726f 6d20 646a 616e  ction: from djan
-00000480: 676f 2e75 726c 7320 696d 706f 7274 2069  go.urls import i
-00000490: 6e63 6c75 6465 2c20 7061 7468 0a20 2020  nclude, path.   
-000004a0: 2032 2e20 4164 6420 6120 5552 4c20 746f   2. Add a URL to
-000004b0: 2075 726c 7061 7474 6572 6e73 3a20 2070   urlpatterns:  p
-000004c0: 6174 6828 2762 6c6f 672f 272c 2069 6e63  ath('blog/', inc
-000004d0: 6c75 6465 2827 626c 6f67 2e75 726c 7327  lude('blog.urls'
-000004e0: 2929 0ae9 0000 0000 2901 da05 6164 6d69  ))......)...admi
-000004f0: 6e29 02da 0470 6174 68da 0769 6e63 6c75  n)...path..inclu
-00000500: 6465 2901 da07 726f 7574 6572 73e9 0100  de)...routers...
-00000510: 0000 2901 da05 7669 6577 7329 01da 0f50  ..)...views)...P
-00000520: 6572 6d69 7373 696f 6e73 5669 6577 2901  ermissionsView).
-00000530: da08 7669 6577 7365 7473 2901 da10 6f62  ..viewsets)...ob
-00000540: 7461 696e 5f6a 7774 5f74 6f6b 656e 2901  tain_jwt_token).
-00000550: da11 7265 6672 6573 685f 6a77 745f 746f  ..refresh_jwt_to
-00000560: 6b65 6e29 01da 1076 6572 6966 795f 6a77  ken)...verify_jw
-00000570: 745f 746f 6b65 6e7a 0972 6567 6973 7465  t_tokenz.registe
-00000580: 722f 7a06 6c6f 6769 6e2f 7a0e 746f 6b65  r/z.login/z.toke
-00000590: 6e2f 7265 6672 6573 682f 7a07 7665 7269  n/refresh/z.veri
-000005a0: 6679 2f7a 0c70 6572 6d69 7373 696f 6e73  fy/z.permissions
-000005b0: 2fda 0b70 6572 6d69 7373 696f 6e73 2901  /..permissions).
-000005c0: da04 6e61 6d65 7a10 6368 616e 6765 2d70  ..namez.change-p
-000005d0: 6173 7377 6f72 642f 7a10 616c 6c2d 7065  assword/z.all-pe
-000005e0: 726d 6973 7369 6f6e 732f 7a09 6f77 6e2d  rmissions/z.own-
-000005f0: 6d65 6e75 2f7a 1669 6d70 6f72 745f 706f  menu/z.import_po
-00000600: 7369 7469 6f6e 5f74 6974 6c65 2f7a 0e69  sition_title/z.i
-00000610: 6d70 6f72 745f 6f66 6669 6365 2f7a 0e69  mport_office/z.i
-00000620: 6d70 6f72 745f 646f 6374 6f72 2f7a 0f69  mport_doctor/z.i
-00000630: 6d70 6f72 745f 696e 735f 6469 632f 7a0f  mport_ins_dic/z.
-00000640: 696d 706f 7274 5f65 7861 5f64 6963 2f7a  import_exa_dic/z
-00000650: 1069 6d70 6f72 745f 6472 7567 5f64 6972  .import_drug_dir
-00000660: 2f7a 1569 6d70 6f72 745f 7068 6172 6d61  /z.import_pharma
-00000670: 6379 5f64 7275 672f 7a11 6d65 6e75 5f70  cy_drug/z.menu_p
-00000680: 6572 6d69 7373 696f 6e73 2f5a 0f65 7870  ermissions/Z.exp
-00000690: 6f72 745f 686f 7370 6974 616c 5a0d 6578  ort_hospitalZ.ex
-000006a0: 706f 7274 5f6f 6666 6963 655a 0c65 7870  port_officeZ.exp
-000006b0: 6f72 745f 6772 6f75 705a 0d65 7870 6f72  ort_groupZ.expor
-000006c0: 745f 646f 6374 6f72 5a0b 6578 706f 7274  t_doctorZ.export
-000006d0: 5f75 7365 72da 0667 726f 7570 73da 0575  _user..groups..u
-000006e0: 7365 7273 5a07 696e 735f 6469 635a 0e65  sersZ.ins_dicZ.e
-000006f0: 7870 6f72 745f 696e 735f 6469 635a 0765  xport_ins_dicZ.e
-00000700: 7861 5f64 6963 5a0e 6578 706f 7274 5f65  xa_dicZ.export_e
-00000710: 7861 5f64 6963 5a15 6578 706f 7274 5f64  xa_dicZ.export_d
-00000720: 7275 675f 6469 7265 6374 6f72 795a 1465  rug_directoryZ.e
-00000730: 7870 6f72 745f 7068 6172 6d61 6379 5f64  xport_pharmacy_d
-00000740: 7275 675a 1370 6861 726d 6163 795f 6d61  rugZ.pharmacy_ma
-00000750: 6e61 6765 6d65 6e74 5a10 6472 7567 5f64  nagementZ.drug_d
-00000760: 6972 6563 746f 7269 6573 5a07 6170 696e  irectoriesZ.apin
-00000770: 666f 735a 0968 6f73 7069 7461 6c73 5a07  fosZ.hospitalsZ.
-00000780: 6f66 6669 6365 73da 0764 6f63 746f 7273  offices..doctors
-00000790: 4e29 36da 075f 5f64 6f63 5f5f da0e 646a  N)6..__doc__..dj
-000007a0: 616e 676f 2e63 6f6e 7472 6962 7202 0000  ango.contribr...
-000007b0: 00da 0b64 6a61 6e67 6f2e 7572 6c73 7203  ...django.urlsr.
-000007c0: 0000 0072 0400 0000 da0e 7265 7374 5f66  ...r......rest_f
-000007d0: 7261 6d65 776f 726b 7205 0000 00da 0072  rameworkr......r
-000007e0: 0700 0000 da11 6261 7365 5f73 7973 7465  ......base_syste
-000007f0: 6d2e 7669 6577 7372 0800 0000 da0b 6261  m.viewsr......ba
-00000800: 7365 5f73 7973 7465 6d72 0900 0000 5a18  se_systemr....Z.
-00000810: 7265 7374 5f66 7261 6d65 776f 726b 5f6a  rest_framework_j
-00000820: 7774 2e76 6965 7773 720a 0000 0072 0b00  wt.viewsr....r..
-00000830: 0000 720c 0000 00da 0872 6567 6973 7465  ..r......registe
-00000840: 72da 0761 735f 7669 6577 5a0f 6368 616e  r..as_viewZ.chan
-00000850: 6765 5f70 6173 7377 6f72 645a 0f61 6c6c  ge_passwordZ.all
-00000860: 5f70 6572 6d69 7373 696f 6e73 5a13 6765  _permissionsZ.ge
-00000870: 745f 6f77 6e5f 7065 726d 6973 7369 6f6e  t_own_permission
-00000880: 735a 1569 6d70 6f72 745f 706f 7369 7469  sZ.import_positi
-00000890: 6f6e 5f74 6974 6c65 5a0d 696d 706f 7274  on_titleZ.import
-000008a0: 5f6f 6666 6963 655a 0d69 6d70 6f72 745f  _officeZ.import_
-000008b0: 646f 6374 6f72 5a1e 696d 706f 7274 5f69  doctorZ.import_i
-000008c0: 6e73 7065 6374 696f 6e5f 6469 6374 696f  nspection_dictio
-000008d0: 6e61 7269 6573 5a1f 696d 706f 7274 5f65  nariesZ.import_e
-000008e0: 7861 6d69 6e61 7469 6f6e 5f64 6963 7469  xamination_dicti
-000008f0: 6f6e 6172 6965 735a 1569 6d70 6f72 745f  onariesZ.import_
-00000900: 6472 7567 5f64 6972 6563 746f 7279 5a14  drug_directoryZ.
-00000910: 696d 706f 7274 5f70 6861 726d 6163 795f  import_pharmacy_
-00000920: 6472 7567 5a10 6d65 6e75 5f70 6572 6d69  drugZ.menu_permi
-00000930: 7373 696f 6e73 da0b 7572 6c70 6174 7465  ssions..urlpatte
-00000940: 726e 735a 0d44 6566 6175 6c74 526f 7574  rnsZ.DefaultRout
-00000950: 6572 da06 726f 7574 6572 5a19 486f 7370  er..routerZ.Hosp
-00000960: 6974 616c 496e 666f 4578 706f 7274 5669  italInfoExportVi
-00000970: 6577 5365 745a 174f 6666 6963 6549 6e66  ewSetZ.OfficeInf
-00000980: 6f45 7870 6f72 7456 6965 7753 6574 5a12  oExportViewSetZ.
-00000990: 4772 6f75 7045 7870 6f72 7456 6965 7753  GroupExportViewS
-000009a0: 6574 5a17 446f 6374 6f72 496e 666f 4578  etZ.DoctorInfoEx
-000009b0: 706f 7274 5669 6577 5365 745a 1555 7365  portViewSetZ.Use
-000009c0: 7249 6e66 6f45 7870 6f72 7456 6965 7753  rInfoExportViewS
-000009d0: 6574 5a0c 4772 6f75 7056 6965 7753 6574  etZ.GroupViewSet
-000009e0: 5a0b 5573 6572 5669 6577 5365 745a 1d49  Z.UserViewSetZ.I
-000009f0: 6e73 7065 6374 696f 6e44 6963 7469 6f6e  nspectionDiction
-00000a00: 6172 6965 7356 6965 7753 6574 5a27 496e  ariesViewSetZ'In
-00000a10: 7370 6563 7469 6f6e 4469 6374 696f 6e61  spectionDictiona
-00000a20: 7269 6573 496e 666f 4578 706f 7274 5669  riesInfoExportVi
-00000a30: 6577 5365 745a 1e45 7861 6d69 6e61 7469  ewSetZ.Examinati
-00000a40: 6f6e 4469 6374 696f 6e61 7269 6573 5669  onDictionariesVi
-00000a50: 6577 5365 745a 2845 7861 6d69 6e61 7469  ewSetZ(Examinati
-00000a60: 6f6e 4469 6374 696f 6e61 7269 6573 496e  onDictionariesIn
-00000a70: 666f 4578 706f 7274 5669 6577 5365 745a  foExportViewSetZ
-00000a80: 1a44 7275 6744 6972 6563 746f 7279 4578  .DrugDirectoryEx
-00000a90: 706f 7274 5669 6577 5365 745a 1950 6861  portViewSetZ.Pha
-00000aa0: 726d 6163 7944 7275 6745 7870 6f72 7456  rmacyDrugExportV
-00000ab0: 6965 7753 6574 5a19 5068 6172 6d61 6379  iewSetZ.Pharmacy
-00000ac0: 4d61 6e61 6765 6d65 6e74 5669 6577 5365  ManagementViewSe
-00000ad0: 745a 1444 7275 6744 6972 6563 746f 7279  tZ.DrugDirectory
-00000ae0: 5669 6577 5365 745a 0e41 7069 496e 666f  ViewSetZ.ApiInfo
-00000af0: 5669 6577 5365 745a 0f48 6f73 7069 7461  ViewSetZ.Hospita
-00000b00: 6c56 6965 7753 6574 5a0d 4f66 6669 6365  lViewSetZ.Office
-00000b10: 5669 6577 5365 745a 0d44 6f63 746f 7256  ViewSetZ.DoctorV
-00000b20: 6965 7753 6574 da04 7572 6c73 a900 721e  iewSet..urls..r.
-00000b30: 0000 0072 1e00 0000 fa35 2f68 6f6d 652f  ...r.....5/home/
-00000b40: 6c79 682f 776f 726b 2f42 6173 6546 756e  lyh/work/BaseFun
-00000b50: 6374 696f 6e4d 6f64 756c 652f 6261 7365  ctionModule/base
-00000b60: 5f73 7973 7465 6d2f 7572 6c73 2e70 79da  _system/urls.py.
-00000b70: 083c 6d6f 6475 6c65 3e01 0000 0073 5e00  .<module>....s^.
-00000b80: 0000 040f 0c01 1001 0c02 0c01 0c01 0c01  ................
-00000b90: 0c01 0c01 0c04 0a01 0801 0801 0801 1001  ................
-00000ba0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00000bb0: 0a01 0a01 0aef 0414 0801 0e01 0e01 0e01  ................
-00000bc0: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
-00000bd0: 0e01 0e01 0e01 0e01 0e03 0e01 0e01 0e02  ................
+00000070: 0100 6401 6408 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
+00000080: 0100 6401 6409 6c0f 6d10 5a10 0100 6401  ..d.d.l.m.Z...d.
+00000090: 640a 6c0f 6d11 5a11 0100 6401 640b 6c0f  d.l.m.Z...d.d.l.
+000000a0: 6d12 5a12 0100 6504 640c 6509 6a13 8302  m.Z...e.d.e.j...
+000000b0: 6504 640d 6510 8302 6504 640e 6511 8302  e.d.e...e.d.e...
+000000c0: 6504 640f 6512 8302 6504 6410 650b a014  e.d.e...e.d.e...
+000000d0: a100 6411 6412 8d03 6504 6413 6509 6a15  ..d.d...e.d.e.j.
+000000e0: 8302 6504 6414 650d 6a16 8302 6504 6415  ..e.d.e.j...e.d.
+000000f0: 650d 6a17 8302 6504 6416 6509 6a18 8302  e.j...e.d.e.j...
+00000100: 6504 6417 6509 6a19 8302 6504 6418 6509  e.d.e.j...e.d.e.
+00000110: 6a1a 8302 6504 6419 6509 6a1b 8302 6504  j...e.d.e.j...e.
+00000120: 641a 6509 6a1c 8302 6504 641b 6509 6a1d  d.e.j...e.d.e.j.
+00000130: 8302 6504 641c 6509 6a1e 8302 6504 641d  ..e.d.e.j...e.d.
+00000140: 650d 6a1f 8302 6710 5a20 6507 a021 a100  e.j...g.Z e..!..
+00000150: 5a22 6522 a013 641e 650d 6a23 a102 0100  Z"e"..d.e.j#....
+00000160: 6522 a013 641f 650d 6a24 a102 0100 6522  e"..d.e.j$....e"
+00000170: a013 6420 650d 6a25 a102 0100 6522 a013  ..d e.j%....e"..
+00000180: 6421 650d 6a26 a102 0100 6522 a013 6422  d!e.j&....e"..d"
+00000190: 6509 6a27 a102 0100 6522 a013 6423 6509  e.j'....e"..d#e.
+000001a0: 6a28 a102 0100 6522 a013 6424 6509 6a29  j(....e"..d$e.j)
+000001b0: a102 0100 6522 a013 6425 6509 6a2a a102  ....e"..d%e.j*..
+000001c0: 0100 6522 a013 6426 6509 6a2b a102 0100  ..e"..d&e.j+....
+000001d0: 6522 a013 6427 6509 6a2c a102 0100 6522  e"..d'e.j,....e"
+000001e0: a013 6428 6509 6a2d a102 0100 6522 a013  ..d(e.j-....e"..
+000001f0: 6429 6509 6a2e a102 0100 6522 a013 642a  d)e.j.....e"..d*
+00000200: 650e 6a2f a102 0100 6522 a013 642b 650e  e.j/....e"..d+e.
+00000210: 6a30 a102 0100 6522 a013 642c 650e 6a31  j0....e"..d,e.j1
+00000220: a102 0100 6522 a013 642d 650e 6a32 a102  ....e"..d-e.j2..
+00000230: 0100 6522 a013 642e 650e 6a33 a102 0100  ..e"..d.e.j3....
+00000240: 6522 a013 642f 650e 6a34 a102 0100 6522  e"..d/e.j4....e"
+00000250: a013 6430 650e 6a35 a102 0100 6522 a013  ..d0e.j5....e"..
+00000260: 6431 650e 6a36 a102 0100 6522 a013 6432  d1e.j6....e"..d2
+00000270: 650e 6a37 a102 0100 6520 6522 6a38 3700  e.j7....e e"j87.
+00000280: 5a20 6433 5300 2934 6176 0200 004d 6564  Z d3S.)4av...Med
+00000290: 6963 616c 5379 7374 656d 2055 524c 2043  icalSystem URL C
+000002a0: 6f6e 6669 6775 7261 7469 6f6e 0a0a 5468  onfiguration..Th
+000002b0: 6520 6075 726c 7061 7474 6572 6e73 6020  e `urlpatterns` 
+000002c0: 6c69 7374 2072 6f75 7465 7320 5552 4c73  list routes URLs
+000002d0: 2074 6f20 7669 6577 732e 2046 6f72 206d   to views. For m
+000002e0: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
+000002f0: 706c 6561 7365 2073 6565 3a0a 2020 2020  please see:.    
+00000300: 6874 7470 733a 2f2f 646f 6373 2e64 6a61  https://docs.dja
+00000310: 6e67 6f70 726f 6a65 6374 2e63 6f6d 2f65  ngoproject.com/e
+00000320: 6e2f 342e 312f 746f 7069 6373 2f68 7474  n/4.1/topics/htt
+00000330: 702f 7572 6c73 2f0a 4578 616d 706c 6573  p/urls/.Examples
+00000340: 3a0a 4675 6e63 7469 6f6e 2076 6965 7773  :.Function views
+00000350: 0a20 2020 2031 2e20 4164 6420 616e 2069  .    1. Add an i
+00000360: 6d70 6f72 743a 2020 6672 6f6d 206d 795f  mport:  from my_
+00000370: 6170 7020 696d 706f 7274 2076 6965 7773  app import views
+00000380: 0a20 2020 2032 2e20 4164 6420 6120 5552  .    2. Add a UR
+00000390: 4c20 746f 2075 726c 7061 7474 6572 6e73  L to urlpatterns
+000003a0: 3a20 2070 6174 6828 2727 2c20 7669 6577  :  path('', view
+000003b0: 732e 686f 6d65 2c20 6e61 6d65 3d27 686f  s.home, name='ho
+000003c0: 6d65 2729 0a43 6c61 7373 2d62 6173 6564  me').Class-based
+000003d0: 2076 6965 7773 0a20 2020 2031 2e20 4164   views.    1. Ad
+000003e0: 6420 616e 2069 6d70 6f72 743a 2020 6672  d an import:  fr
+000003f0: 6f6d 206f 7468 6572 5f61 7070 2e76 6965  om other_app.vie
+00000400: 7773 2069 6d70 6f72 7420 486f 6d65 0a20  ws import Home. 
+00000410: 2020 2032 2e20 4164 6420 6120 5552 4c20     2. Add a URL 
+00000420: 746f 2075 726c 7061 7474 6572 6e73 3a20  to urlpatterns: 
+00000430: 2070 6174 6828 2727 2c20 486f 6d65 2e61   path('', Home.a
+00000440: 735f 7669 6577 2829 2c20 6e61 6d65 3d27  s_view(), name='
+00000450: 686f 6d65 2729 0a49 6e63 6c75 6469 6e67  home').Including
+00000460: 2061 6e6f 7468 6572 2055 524c 636f 6e66   another URLconf
+00000470: 0a20 2020 2031 2e20 496d 706f 7274 2074  .    1. Import t
+00000480: 6865 2069 6e63 6c75 6465 2829 2066 756e  he include() fun
+00000490: 6374 696f 6e3a 2066 726f 6d20 646a 616e  ction: from djan
+000004a0: 676f 2e75 726c 7320 696d 706f 7274 2069  go.urls import i
+000004b0: 6e63 6c75 6465 2c20 7061 7468 0a20 2020  nclude, path.   
+000004c0: 2032 2e20 4164 6420 6120 5552 4c20 746f   2. Add a URL to
+000004d0: 2075 726c 7061 7474 6572 6e73 3a20 2070   urlpatterns:  p
+000004e0: 6174 6828 2762 6c6f 672f 272c 2069 6e63  ath('blog/', inc
+000004f0: 6c75 6465 2827 626c 6f67 2e75 726c 7327  lude('blog.urls'
+00000500: 2929 0ae9 0000 0000 2901 da05 6164 6d69  ))......)...admi
+00000510: 6e29 02da 0470 6174 68da 0769 6e63 6c75  n)...path..inclu
+00000520: 6465 2901 da07 726f 7574 6572 73e9 0100  de)...routers...
+00000530: 0000 2901 da05 7669 6577 7329 01da 0f50  ..)...views)...P
+00000540: 6572 6d69 7373 696f 6e73 5669 6577 2902  ermissionsView).
+00000550: da08 7669 6577 7365 7473 da0e 6578 706f  ..viewsets..expo
+00000560: 7274 5f76 6965 7773 6574 2901 da10 6f62  rt_viewset)...ob
+00000570: 7461 696e 5f6a 7774 5f74 6f6b 656e 2901  tain_jwt_token).
+00000580: da11 7265 6672 6573 685f 6a77 745f 746f  ..refresh_jwt_to
+00000590: 6b65 6e29 01da 1076 6572 6966 795f 6a77  ken)...verify_jw
+000005a0: 745f 746f 6b65 6e7a 0972 6567 6973 7465  t_tokenz.registe
+000005b0: 722f 7a06 6c6f 6769 6e2f 7a0e 746f 6b65  r/z.login/z.toke
+000005c0: 6e2f 7265 6672 6573 682f 7a07 7665 7269  n/refresh/z.veri
+000005d0: 6679 2f7a 0c70 6572 6d69 7373 696f 6e73  fy/z.permissions
+000005e0: 2fda 0b70 6572 6d69 7373 696f 6e73 2901  /..permissions).
+000005f0: da04 6e61 6d65 7a10 6368 616e 6765 2d70  ..namez.change-p
+00000600: 6173 7377 6f72 642f 7a10 616c 6c2d 7065  assword/z.all-pe
+00000610: 726d 6973 7369 6f6e 732f 7a09 6f77 6e2d  rmissions/z.own-
+00000620: 6d65 6e75 2f7a 1669 6d70 6f72 745f 706f  menu/z.import_po
+00000630: 7369 7469 6f6e 5f74 6974 6c65 2f7a 0e69  sition_title/z.i
+00000640: 6d70 6f72 745f 6f66 6669 6365 2f7a 0e69  mport_office/z.i
+00000650: 6d70 6f72 745f 646f 6374 6f72 2f7a 0f69  mport_doctor/z.i
+00000660: 6d70 6f72 745f 696e 735f 6469 632f 7a0f  mport_ins_dic/z.
+00000670: 696d 706f 7274 5f65 7861 5f64 6963 2f7a  import_exa_dic/z
+00000680: 1069 6d70 6f72 745f 6472 7567 5f64 6972  .import_drug_dir
+00000690: 2f7a 1569 6d70 6f72 745f 7068 6172 6d61  /z.import_pharma
+000006a0: 6379 5f64 7275 672f 7a11 6d65 6e75 5f70  cy_drug/z.menu_p
+000006b0: 6572 6d69 7373 696f 6e73 2f5a 0968 6f73  ermissions/Z.hos
+000006c0: 7069 7461 6c73 5a07 6f66 6669 6365 73da  pitalsZ.offices.
+000006d0: 0764 6f63 746f 7273 da06 6772 6f75 7073  .doctors..groups
+000006e0: da05 7573 6572 735a 0761 7069 6e66 6f73  ..usersZ.apinfos
+000006f0: 5a0f 696e 7370 6563 7469 6f6e 7479 7065  Z.inspectiontype
+00000700: 735a 0769 6e73 5f64 6963 5a10 6578 616d  sZ.ins_dicZ.exam
+00000710: 696e 6174 696f 6e74 7970 6573 5a07 6578  inationtypesZ.ex
+00000720: 615f 6469 635a 1370 6861 726d 6163 795f  a_dicZ.pharmacy_
+00000730: 6d61 6e61 6765 6d65 6e74 5a10 6472 7567  managementZ.drug
+00000740: 5f64 6972 6563 746f 7269 6573 5a0f 6578  _directoriesZ.ex
+00000750: 706f 7274 5f68 6f73 7069 7461 6c5a 0d65  port_hospitalZ.e
+00000760: 7870 6f72 745f 6f66 6669 6365 5a0c 6578  xport_officeZ.ex
+00000770: 706f 7274 5f67 726f 7570 5a0d 6578 706f  port_groupZ.expo
+00000780: 7274 5f64 6f63 746f 725a 0b65 7870 6f72  rt_doctorZ.expor
+00000790: 745f 7573 6572 5a0e 6578 706f 7274 5f69  t_userZ.export_i
+000007a0: 6e73 5f64 6963 5a0e 6578 706f 7274 5f65  ns_dicZ.export_e
+000007b0: 7861 5f64 6963 5a15 6578 706f 7274 5f64  xa_dicZ.export_d
+000007c0: 7275 675f 6469 7265 6374 6f72 795a 1465  rug_directoryZ.e
+000007d0: 7870 6f72 745f 7068 6172 6d61 6379 5f64  xport_pharmacy_d
+000007e0: 7275 674e 2939 da07 5f5f 646f 635f 5fda  rugN)9..__doc__.
+000007f0: 0e64 6a61 6e67 6f2e 636f 6e74 7269 6272  .django.contribr
+00000800: 0200 0000 da0b 646a 616e 676f 2e75 726c  ......django.url
+00000810: 7372 0300 0000 7204 0000 00da 0e72 6573  sr....r......res
+00000820: 745f 6672 616d 6577 6f72 6b72 0500 0000  t_frameworkr....
+00000830: da00 7207 0000 00da 1162 6173 655f 7379  ..r......base_sy
+00000840: 7374 656d 2e76 6965 7773 7208 0000 00da  stem.viewsr.....
+00000850: 0b62 6173 655f 7379 7374 656d 7209 0000  .base_systemr...
+00000860: 0072 0a00 0000 5a18 7265 7374 5f66 7261  .r....Z.rest_fra
+00000870: 6d65 776f 726b 5f6a 7774 2e76 6965 7773  mework_jwt.views
+00000880: 720b 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000890: 0872 6567 6973 7465 72da 0761 735f 7669  .register..as_vi
+000008a0: 6577 5a0f 6368 616e 6765 5f70 6173 7377  ewZ.change_passw
+000008b0: 6f72 645a 0f61 6c6c 5f70 6572 6d69 7373  ordZ.all_permiss
+000008c0: 696f 6e73 5a13 6765 745f 6f77 6e5f 7065  ionsZ.get_own_pe
+000008d0: 726d 6973 7369 6f6e 735a 1569 6d70 6f72  rmissionsZ.impor
+000008e0: 745f 706f 7369 7469 6f6e 5f74 6974 6c65  t_position_title
+000008f0: 5a0d 696d 706f 7274 5f6f 6666 6963 655a  Z.import_officeZ
+00000900: 0d69 6d70 6f72 745f 646f 6374 6f72 5a1e  .import_doctorZ.
+00000910: 696d 706f 7274 5f69 6e73 7065 6374 696f  import_inspectio
+00000920: 6e5f 6469 6374 696f 6e61 7269 6573 5a1f  n_dictionariesZ.
+00000930: 696d 706f 7274 5f65 7861 6d69 6e61 7469  import_examinati
+00000940: 6f6e 5f64 6963 7469 6f6e 6172 6965 735a  on_dictionariesZ
+00000950: 1569 6d70 6f72 745f 6472 7567 5f64 6972  .import_drug_dir
+00000960: 6563 746f 7279 5a14 696d 706f 7274 5f70  ectoryZ.import_p
+00000970: 6861 726d 6163 795f 6472 7567 5a10 6d65  harmacy_drugZ.me
+00000980: 6e75 5f70 6572 6d69 7373 696f 6e73 da0b  nu_permissions..
+00000990: 7572 6c70 6174 7465 726e 735a 0d44 6566  urlpatternsZ.Def
+000009a0: 6175 6c74 526f 7574 6572 da06 726f 7574  aultRouter..rout
+000009b0: 6572 5a0f 486f 7370 6974 616c 5669 6577  erZ.HospitalView
+000009c0: 5365 745a 0d4f 6666 6963 6556 6965 7753  SetZ.OfficeViewS
+000009d0: 6574 5a0d 446f 6374 6f72 5669 6577 5365  etZ.DoctorViewSe
+000009e0: 745a 0c47 726f 7570 5669 6577 5365 745a  tZ.GroupViewSetZ
+000009f0: 0b55 7365 7256 6965 7753 6574 5a0e 4170  .UserViewSetZ.Ap
+00000a00: 6949 6e66 6f56 6965 7753 6574 5a15 496e  iInfoViewSetZ.In
+00000a10: 7370 6563 7469 6f6e 5479 7065 5669 6577  spectionTypeView
+00000a20: 5365 745a 1d49 6e73 7065 6374 696f 6e44  SetZ.InspectionD
+00000a30: 6963 7469 6f6e 6172 6965 7356 6965 7753  ictionariesViewS
+00000a40: 6574 5a16 4578 616d 696e 6174 696f 6e54  etZ.ExaminationT
+00000a50: 7970 6556 6965 7753 6574 5a1e 4578 616d  ypeViewSetZ.Exam
+00000a60: 696e 6174 696f 6e44 6963 7469 6f6e 6172  inationDictionar
+00000a70: 6965 7356 6965 7753 6574 5a19 5068 6172  iesViewSetZ.Phar
+00000a80: 6d61 6379 4d61 6e61 6765 6d65 6e74 5669  macyManagementVi
+00000a90: 6577 5365 745a 1444 7275 6744 6972 6563  ewSetZ.DrugDirec
+00000aa0: 746f 7279 5669 6577 5365 745a 1948 6f73  toryViewSetZ.Hos
+00000ab0: 7069 7461 6c49 6e66 6f45 7870 6f72 7456  pitalInfoExportV
+00000ac0: 6965 7753 6574 5a17 4f66 6669 6365 496e  iewSetZ.OfficeIn
+00000ad0: 666f 4578 706f 7274 5669 6577 5365 745a  foExportViewSetZ
+00000ae0: 1247 726f 7570 4578 706f 7274 5669 6577  .GroupExportView
+00000af0: 5365 745a 1744 6f63 746f 7249 6e66 6f45  SetZ.DoctorInfoE
+00000b00: 7870 6f72 7456 6965 7753 6574 5a15 5573  xportViewSetZ.Us
+00000b10: 6572 496e 666f 4578 706f 7274 5669 6577  erInfoExportView
+00000b20: 5365 745a 2749 6e73 7065 6374 696f 6e44  SetZ'InspectionD
+00000b30: 6963 7469 6f6e 6172 6965 7349 6e66 6f45  ictionariesInfoE
+00000b40: 7870 6f72 7456 6965 7753 6574 5a28 4578  xportViewSetZ(Ex
+00000b50: 616d 696e 6174 696f 6e44 6963 7469 6f6e  aminationDiction
+00000b60: 6172 6965 7349 6e66 6f45 7870 6f72 7456  ariesInfoExportV
+00000b70: 6965 7753 6574 5a1a 4472 7567 4469 7265  iewSetZ.DrugDire
+00000b80: 6374 6f72 7945 7870 6f72 7456 6965 7753  ctoryExportViewS
+00000b90: 6574 5a19 5068 6172 6d61 6379 4472 7567  etZ.PharmacyDrug
+00000ba0: 4578 706f 7274 5669 6577 5365 74da 0475  ExportViewSet..u
+00000bb0: 726c 73a9 0072 1f00 0000 721f 0000 00fa  rls..r....r.....
+00000bc0: 352f 686f 6d65 2f6c 7968 2f77 6f72 6b2f  5/home/lyh/work/
+00000bd0: 4261 7365 4675 6e63 7469 6f6e 4d6f 6475  BaseFunctionModu
+00000be0: 6c65 2f62 6173 655f 7379 7374 656d 2f75  le/base_system/u
+00000bf0: 726c 732e 7079 da08 3c6d 6f64 756c 653e  rls.py..<module>
+00000c00: 0100 0000 7362 0000 0004 0f0c 0110 010c  ....sb..........
+00000c10: 020c 010c 0110 010c 010c 010c 040a 0108  ................
+00000c20: 0108 0108 0110 010a 010a 010a 010a 010a  ................
+00000c30: 010a 010a 010a 010a 010a 010a ef04 1408  ................
+00000c40: 020e 010e 010e 010e 010e 010e 020e 010e  ................
+00000c50: 010e 010e 010e 010e 020e 010e 010e 010e  ................
+00000c60: 010e 010e 010e 010e 010e 02              ...........
```

### Comparing `base_system-0.2.2/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.2.3/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  4 08:07:06 2023 UTC, .py size: 14932 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aa67 5364 543a 0000  a........gSdT:..
+00000000: 610d 0d0a 0000 0000 0d6e 5364 823a 0000  a........nSd.:..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6401 6c05 5a06 6400 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6406 6c0e  m.Z.m.Z...d.d.l.
@@ -237,510 +237,511 @@
 00000ec0: 0000 da0a 7365 7269 616c 697a 6572 7224  ....serializerr$
 00000ed0: 0000 0072 2400 0000 7225 0000 0072 5a00  ...r$...r%...rZ.
 00000ee0: 0000 7100 0000 731a 0000 0000 0210 0110  ..q...s.........
 00000ef0: 0212 0104 0110 011c 0110 0108 030a 020a  ................
 00000f00: 010c 0108 017a 1347 726f 7570 5669 6577  .....z.GroupView
 00000f10: 5365 742e 6372 6561 7465 6302 0000 0000  Set.createc.....
 00000f20: 0000 0000 0000 0006 0000 0004 0000 0043  ...............C
-00000f30: 0000 0073 ce00 0000 7400 8300 7d02 7c01  ...s....t...}.|.
+00000f30: 0000 0073 dc00 0000 7400 8300 7d02 7c01  ...s....t...}.|.
 00000f40: a001 6401 a101 7c02 6401 3c00 7c01 a001  ..d...|.d.<.|...
 00000f50: 6402 6403 a102 7c02 6402 3c00 7c01 a001  d.d...|.d.<.|...
 00000f60: 6404 a101 7c02 6405 3c00 7c01 a001 6406  d...|.d.<.|...d.
 00000f70: a101 7c02 6406 3c00 7c01 a001 6407 a101  ..|.d.<.|...d...
 00000f80: 7c02 6407 3c00 7c01 a001 6408 a101 7c02  |.d.<.|...d...|.
-00000f90: 6408 3c00 7402 7c02 6409 8d01 7d03 7c03  d.<.t.|.d...}.|.
-00000fa0: 6a03 640a 640b 8d01 0100 7c03 6a04 7d02  j.d.d.....|.j.}.
-00000fb0: 7400 8300 7d04 7c01 a001 640c a101 7d05  t...}.|...d...}.
-00000fc0: 7c05 7290 7c05 6e02 6700 7c04 640c 3c00  |.r.|.n.g.|.d.<.
-00000fd0: 7c01 a001 640d a101 72c6 7c01 a001 640d  |...d...r.|...d.
-00000fe0: a101 7c04 640d 3c00 7405 7c04 6409 8d01  ..|.d.<.t.|.d...
-00000ff0: 7d03 7c03 6a03 640a 640b 8d01 0100 7c02  }.|.j.d.d.....|.
-00001000: 7c04 6602 5300 290e 4eda 046e 6f74 65da  |.f.S.).N..note.
-00001010: 0969 735f 6163 7469 7665 e901 0000 00da  .is_active......
-00001020: 0b68 6f73 7069 7461 6c5f 6964 da08 686f  .hospital_id..ho
-00001030: 7370 6974 616c 7232 0000 00da 0c63 7265  spitalr2.....cre
-00001040: 6174 6564 5f75 7365 72da 0972 6f6c 655f  ated_user..role_
-00001050: 636f 6465 7253 0000 0054 7254 0000 0072  coderS...TrT...r
-00001060: 5200 0000 723d 0000 0029 06da 0464 6963  R...r=...)...dic
-00001070: 74da 0367 6574 7212 0000 0072 5c00 0000  t..getr....r\...
-00001080: 722c 0000 0072 1100 0000 2906 7221 0000  r,...r....).r!..
-00001090: 0072 2c00 0000 7260 0000 0072 6200 0000  .r,...r`...rb...
-000010a0: 7261 0000 0072 3800 0000 7224 0000 0072  ra...r8...r$...r
-000010b0: 2400 0000 7225 0000 0072 5900 0000 8500  $...r%...rY.....
-000010c0: 0000 7324 0000 0000 0206 020e 0110 010e  ..s$............
-000010d0: 010e 010e 010e 010a 010c 0106 0306 010a  ................
-000010e0: 0210 010a 010e 010a 010c 037a 1747 726f  ...........z.Gro
-000010f0: 7570 5669 6577 5365 742e 6368 6563 6b5f  upViewSet.check_
-00001100: 6461 7461 6302 0000 0000 0000 0000 0000  datac...........
-00001110: 0008 0000 0004 0000 004f 0000 0073 c200  .........O...s..
-00001120: 0000 7c00 a000 a100 7d04 7c04 6a01 7d05  ..|.....}.|.j.}.
-00001130: 7c01 6a02 a003 6401 a101 7c04 6a04 6b02  |.j...d...|.j.k.
-00001140: 7228 7c01 6a02 6401 3d00 7c00 a005 7c01  r(|.j.d.=.|...|.
-00001150: 6a02 a101 5c02 7d06 7d07 7c06 6402 1900  j...\.}.}.|.d...
-00001160: 7c05 5f06 7c06 6403 1900 7c05 5f07 7c06  |._.|.d...|._.|.
-00001170: 6404 1900 7c05 5f08 7c06 6405 1900 7c05  d...|._.|.d...|.
-00001180: 5f09 7c06 6406 1900 7c05 5f0a 7c06 6407  _.|.d...|._.|.d.
-00001190: 1900 7c05 5f0b 7c06 6408 1900 7c05 5f0c  ..|._.|.d...|._.
-000011a0: 7c05 a00d a100 0100 7c07 a003 6401 7c04  |.......|...d.|.
-000011b0: 6a04 a102 7c04 5f04 7c04 6a0e a00f 7c07  j...|._.|.j...|.
-000011c0: 6409 1900 a101 0100 7c04 a00d a100 0100  d.......|.......
-000011d0: 7410 7411 7c04 8301 6a02 7412 6a13 640a  t.t.|...j.t.j.d.
-000011e0: 8d02 5300 290b 4e72 3d00 0000 7263 0000  ..S.).Nr=...rc..
-000011f0: 0072 6400 0000 7232 0000 0072 6700 0000  .rd...r2...rg...
-00001200: 7268 0000 0072 6900 0000 da09 726f 6c65  rh...ri.....role
-00001210: 5f6e 616d 6572 5200 0000 722b 0000 0029  _namerR...r+...)
-00001220: 1472 2d00 0000 da0b 6578 7472 615f 6772  .r-.....extra_gr
-00001230: 6f75 7072 2c00 0000 726b 0000 0072 3d00  oupr,...rk...r=.
-00001240: 0000 7259 0000 0072 6300 0000 7264 0000  ..rY...rc...rd..
-00001250: 00da 0569 6e64 6578 7266 0000 0072 6800  ...indexrf...rh.
-00001260: 0000 7269 0000 0072 6c00 0000 725b 0000  ..ri...rl...r[..
-00001270: 0072 3800 0000 724a 0000 0072 0200 0000  .r8...rJ...r....
-00001280: 7211 0000 0072 0c00 0000 da16 4854 5450  r....r......HTTP
-00001290: 5f32 3035 5f52 4553 4554 5f43 4f4e 5445  _205_RESET_CONTE
-000012a0: 4e54 2908 7221 0000 0072 3500 0000 725e  NT).r!...r5...r^
-000012b0: 0000 0072 5f00 0000 7229 0000 0072 6d00  ...r_...r)...rm.
-000012c0: 0000 7260 0000 0072 6100 0000 7224 0000  ..r`...ra...r$..
-000012d0: 0072 2400 0000 7225 0000 00da 0675 7064  .r$...r%.....upd
-000012e0: 6174 65a0 0000 0073 2200 0000 0002 0801  ate....s".......
-000012f0: 0601 1201 0801 1001 0a01 0a01 0a01 0a01  ................
-00001300: 0a01 0a01 0a01 0801 1002 1001 0801 7a13  ..............z.
-00001310: 4772 6f75 7056 6965 7753 6574 2e75 7064  GroupViewSet.upd
-00001320: 6174 654e 2915 da08 5f5f 6e61 6d65 5f5f  ateN)...__name__
-00001330: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00001340: 7175 616c 6e61 6d65 5f5f 7207 0000 0072  qualname__r....r
-00001350: 2e00 0000 7231 0000 00da 0871 7565 7279  ....r1.....query
-00001360: 7365 7472 1100 0000 da10 7365 7269 616c  setr......serial
-00001370: 697a 6572 5f63 6c61 7373 da0d 6669 6c74  izer_class..filt
-00001380: 6572 5f66 6965 6c64 7372 2000 0000 720b  er_fieldsr ...r.
-00001390: 0000 0072 3900 0000 723a 0000 0072 4700  ...r9...r:...rG.
-000013a0: 0000 7233 0000 0072 1900 0000 da06 6174  ..r3...r......at
-000013b0: 6f6d 6963 725a 0000 0072 5900 0000 7270  omicrZ...rY...rp
-000013c0: 0000 0072 2400 0000 7224 0000 0072 2400  ...r$...r$...r$.
-000013d0: 0000 7225 0000 0072 1a00 0000 1500 0000  ..r%...r........
-000013e0: 7320 0000 0008 010a 0104 0104 0308 060c  s ..............
-000013f0: 010a 090c 010a 080c 010a 1a08 2204 010a  ............"...
-00001400: 1308 1b04 0172 1a00 0000 6300 0000 0000  .....r....c.....
-00001410: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00001420: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00001430: 6503 6a04 a005 a100 5a06 6507 5a08 6401  e.j.....Z.e.Z.d.
-00001440: 5a09 6402 5300 2903 da11 4578 7472 6147  Z.d.S.)...ExtraG
-00001450: 726f 7570 5669 6577 5365 7472 1b00 0000  roupViewSetr....
-00001460: 4e29 0a72 7100 0000 7272 0000 0072 7300  N).rq...rr...rs.
-00001470: 0000 720d 0000 0072 2e00 0000 7231 0000  ..r....r....r1..
-00001480: 0072 7400 0000 7212 0000 0072 7500 0000  .rt...r....ru...
-00001490: 7276 0000 0072 2400 0000 7224 0000 0072  rv...r$...r$...r
-000014a0: 2400 0000 7225 0000 0072 7800 0000 bc00  $...r%...rx.....
-000014b0: 0000 7306 0000 0008 010a 0104 0172 7800  ..s..........rx.
-000014c0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000014d0: 0000 0002 0000 0040 0000 0073 2200 0000  .......@...s"...
-000014e0: 6500 5a01 6400 5a02 6503 6a04 a005 a100  e.Z.d.Z.e.j.....
-000014f0: 5a06 6507 5a08 6401 5a09 6402 5a0a 6401  Z.e.Z.d.Z.d.Z.d.
-00001500: 5300 2903 da17 436f 6e74 656e 7454 7970  S.)...ContentTyp
-00001510: 6543 6174 6573 5669 6577 5365 744e 721b  eCatesViewSetNr.
-00001520: 0000 0029 0b72 7100 0000 7272 0000 0072  ...).rq...rr...r
-00001530: 7300 0000 720e 0000 0072 2e00 0000 7231  s...r....r....r1
-00001540: 0000 0072 7400 0000 7213 0000 0072 7500  ...rt...r....ru.
-00001550: 0000 da10 7061 6769 6e61 7469 6f6e 5f63  ....pagination_c
-00001560: 6c61 7373 7276 0000 0072 2400 0000 7224  lassrv...r$...r$
-00001570: 0000 0072 2400 0000 7225 0000 0072 7900  ...r$...r%...ry.
-00001580: 0000 c200 0000 7308 0000 0008 010a 0104  ......s.........
-00001590: 0104 0172 7900 0000 6300 0000 0000 0000  ...ry...c.......
-000015a0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-000015b0: 0073 1e00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
-000015c0: 6a04 a005 a100 5a06 6507 5a08 6401 5a09  j.....Z.e.Z.d.Z.
-000015d0: 6402 5300 2903 da14 436f 6e74 656e 7454  d.S.)...ContentT
-000015e0: 7970 6545 7856 6965 7753 6574 721b 0000  ypeExViewSetr...
-000015f0: 004e 290a 7271 0000 0072 7200 0000 7273  .N).rq...rr...rs
-00001600: 0000 0072 0f00 0000 722e 0000 0072 3100  ...r....r....r1.
-00001610: 0000 7274 0000 0072 1400 0000 7275 0000  ..rt...r....ru..
-00001620: 0072 7600 0000 7224 0000 0072 2400 0000  .rv...r$...r$...
-00001630: 7224 0000 0072 2500 0000 727b 0000 00c9  r$...r%...r{....
-00001640: 0000 0073 0600 0000 0801 0a01 0401 727b  ...s..........r{
-00001650: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001660: 0700 0000 0400 0000 4300 0000 7356 0000  ........C...sV..
-00001670: 007c 006a 00a0 0164 01a1 017d 0174 026a  .|.j...d...}.t.j
-00001680: 036a 017c 006a 00a0 0164 01a1 0164 028d  .j.|.j...d...d..
-00001690: 017d 027c 026a 047d 0374 056a 036a 067c  .}.|.j.}.t.j.j.|
-000016a0: 0364 038d 01a0 07a1 007d 0474 087d 0574  .d.......}.t.}.t
-000016b0: 097c 057c 0464 0483 037d 0674 0a64 057c  .|.|.d...}.t.d.|
-000016c0: 0669 0183 0153 0029 064e da07 7573 6572  .i...S.).N..user
-000016d0: 5f69 6429 0172 3000 0000 2901 da09 6772  _id).r0...)...gr
-000016e0: 6f75 705f 5f69 6e72 0100 0000 722c 0000  oup__inr....r,..
-000016f0: 0029 0b72 2600 0000 726b 0000 0072 1000  .).r&...rk...r..
-00001700: 0000 722e 0000 00da 0d67 6574 5f61 6c6c  ..r......get_all
-00001710: 6772 6f75 7073 7208 0000 0072 2f00 0000  groupsr....r/...
-00001720: da08 6469 7374 696e 6374 7215 0000 00da  ..distinctr.....
-00001730: 0f67 6574 5f70 6572 6d69 7373 696f 6e73  .get_permissions
-00001740: 7209 0000 0029 0772 3500 0000 727c 0000  r....).r5...r|..
-00001750: 00da 0475 7365 725a 0961 6c6c 6772 6f75  ...userZ.allgrou
-00001760: 7073 7238 0000 0072 6200 0000 da09 6d65  psr8...rb.....me
-00001770: 6e75 5f6c 6973 7472 2400 0000 7224 0000  nu_listr$...r$..
-00001780: 0072 2500 0000 da13 6765 745f 6f77 6e5f  .r%.....get_own_
-00001790: 7065 726d 6973 7369 6f6e 73cf 0000 0073  permissions....s
-000017a0: 0e00 0000 0001 0c01 1605 0601 1201 0401  ................
-000017b0: 0c01 7283 0000 0063 0100 0000 0000 0000  ..r....c........
-000017c0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-000017d0: 7326 0000 0074 006a 01a0 02a1 007d 0174  s&...t.j.....}.t
-000017e0: 037d 0274 047c 027c 0164 0183 037d 0374  .}.t.|.|.d...}.t
-000017f0: 0564 027c 0369 0183 0153 00a9 034e 7265  .d.|.i...S...Nre
-00001800: 0000 0072 2c00 0000 a906 7208 0000 0072  ...r,.....r....r
-00001810: 2e00 0000 7231 0000 0072 1500 0000 7280  ....r1...r....r.
-00001820: 0000 0072 0900 0000 a904 7235 0000 0072  ...r......r5...r
-00001830: 3800 0000 7262 0000 0072 8200 0000 7224  8...rb...r....r$
-00001840: 0000 0072 2400 0000 7225 0000 00da 0f61  ...r$...r%.....a
-00001850: 6c6c 5f70 6572 6d69 7373 696f 6e73 dd00  ll_permissions..
-00001860: 0000 7308 0000 0000 010a 0104 010c 0172  ..s............r
-00001870: 8700 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00001880: 0000 0000 0004 0000 0040 0000 0073 2800  .........@...s(.
-00001890: 0000 6500 5a01 6400 5a02 6503 6a04 6a05  ..e.Z.d.Z.e.j.j.
-000018a0: 6401 6402 6403 8d02 5a06 6507 5a08 6402  d.d.d...Z.e.Z.d.
-000018b0: 5a09 6404 5a0a 6402 5300 2905 da0b 4d65  Z.d.Z.d.S.)...Me
-000018c0: 6e75 5669 6577 5365 7454 4e29 0272 6400  nuViewSetTN).rd.
-000018d0: 0000 721e 0000 0072 1b00 0000 290b 7271  ..r....r....).rq
-000018e0: 0000 0072 7200 0000 7273 0000 0072 0e00  ...rr...rs...r..
-000018f0: 0000 722e 0000 0072 2f00 0000 7274 0000  ..r....r/...rt..
-00001900: 0072 1500 0000 7275 0000 0072 7a00 0000  .r....ru...rz...
-00001910: 7276 0000 0072 2400 0000 7224 0000 0072  rv...r$...r$...r
-00001920: 2400 0000 7225 0000 0072 8800 0000 e400  $...r%...r......
-00001930: 0000 7308 0000 0008 0110 0104 0104 0172  ..s............r
-00001940: 8800 0000 6303 0000 0000 0000 0000 0000  ....c...........
-00001950: 000d 0000 0007 0000 0003 0000 0073 2c01  .............s,.
-00001960: 0000 7400 7401 6401 6402 8400 7c01 8302  ..t.t.d.d...|...
-00001970: 8301 7d03 7402 6a03 6a04 6403 7c03 6404  ..}.t.j.j.d.|.d.
-00001980: 8d02 7d04 7400 7401 6405 6402 8400 7c04  ..}.t.t.d.d...|.
-00001990: 8302 8301 7d05 7405 6a03 6a04 7c05 6406  ....}.t.j.j.|.d.
-000019a0: 8d01 a006 6407 a101 7d06 6700 7d07 7c06  ....d...}.g.}.|.
-000019b0: 4400 5d0e 7d08 7407 7c07 7c08 8302 0100  D.].}.t.|.|.....
-000019c0: 7150 7c07 7c06 3700 7d07 7400 7408 7c07  qP|.|.7.}.t.t.|.
-000019d0: 8301 8301 7d07 7c00 7c07 6403 6408 8d02  ....}.|.|.d.d...
-000019e0: 7d09 7c09 6a09 7d0a 6409 640a 8400 7c0a  }.|.j.}.d.d...|.
-000019f0: 4400 8301 7d0b 7c0a 4400 5d7e 8900 8700  D...}.|.D.]~....
-00001a00: 6601 640b 640a 8408 7c0a 4400 8301 7d0c  f.d.d...|.D...}.
-00001a10: 740a 7c0c 640c 6402 8400 640d 8d02 7d0c  t.|.d.d...d...}.
-00001a20: 7c0c 8800 640e 3c00 7402 6a03 6a04 740b  |...d.<.t.j.j.t.
-00001a30: 8800 640f 1900 a00c 6410 6411 a102 8301  ..d.....d.d.....
-00001a40: 6412 8d01 a00d a100 7d04 7c02 7298 7c04  d.......}.|.r.|.
-00001a50: 7298 7c0c 6700 6b02 7298 7400 7401 6413  r.|.g.k.r.t.t.d.
-00001a60: 6402 8400 7c04 6a0e 6a0f a010 a100 8302  d...|.j.j.......
-00001a70: 8301 8800 640e 3c00 7198 740a 7c0b 6414  ....d.<.q.t.|.d.
-00001a80: 6402 8400 640d 8d02 7d0b 7c0b 5300 2915  d...d...}.|.S.).
-00001a90: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
-00001aa0: 0000 0100 0000 5300 0000 7306 0000 007c  ......S...s....|
-00001ab0: 006a 0053 0072 1c00 0000 2901 722a 0000  .j.S.r....).r*..
-00001ac0: 0029 01da 0470 6572 6d72 2400 0000 7224  .)...permr$...r$
-00001ad0: 0000 0072 2500 0000 7241 0000 00ec 0000  ...r%...rA......
-00001ae0: 0072 4800 0000 7a21 6765 745f 7065 726d  .rH...z!get_perm
-00001af0: 6973 7369 6f6e 732e 3c6c 6f63 616c 733e  issions.<locals>
-00001b00: 2e3c 6c61 6d62 6461 3e54 2902 7264 0000  .<lambda>T).rd..
-00001b10: 005a 1363 6f6e 7465 6e74 5f74 7970 655f  .Z.content_type_
-00001b20: 6964 5f5f 696e 6301 0000 0000 0000 0000  id__inc.........
-00001b30: 0000 0001 0000 0001 0000 0053 0000 0073  ...........S...s
-00001b40: 0600 0000 7c00 6a00 5300 721c 0000 00a9  ....|.j.S.r.....
-00001b50: 01da 1363 6f6e 7465 6e74 5f74 7970 655f  ...content_type_
-00001b60: 6361 745f 6964 2901 da03 6361 7472 2400  cat_id)...catr$.
-00001b70: 0000 7224 0000 0072 2500 0000 7241 0000  ..r$...r%...rA..
-00001b80: 00ee 0000 0072 4800 0000 2901 da06 6964  .....rH...)...id
-00001b90: 5f5f 696e 7232 0000 00a9 01da 046d 616e  __inr2.......man
-00001ba0: 7963 0100 0000 0000 0000 0000 0000 0200  yc..............
-00001bb0: 0000 0400 0000 5300 0000 7318 0000 0067  ......S...s....g
-00001bc0: 007c 005d 107d 017c 0164 0019 0073 047c  .|.].}.|.d...s.|
-00001bd0: 0191 0271 0453 0029 0172 1e00 0000 7224  ...q.S.).r....r$
-00001be0: 0000 0029 02da 022e 30da 046d 656e 7572  ...)....0..menur
-00001bf0: 2400 0000 7224 0000 0072 2500 0000 da0a  $...r$...r%.....
-00001c00: 3c6c 6973 7463 6f6d 703e f800 0000 7248  <listcomp>....rH
-00001c10: 0000 007a 2367 6574 5f70 6572 6d69 7373  ...z#get_permiss
-00001c20: 696f 6e73 2e3c 6c6f 6361 6c73 3e2e 3c6c  ions.<locals>.<l
-00001c30: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
-00001c40: 0000 0000 0002 0000 0008 0000 0013 0000  ................
-00001c50: 0073 2c00 0000 6700 7c00 5d24 7d01 7c01  .s,...g.|.]$}.|.
-00001c60: 6400 1900 7400 8800 6401 1900 a001 6402  d...t...d.....d.
-00001c70: 6403 a102 8301 6b02 7204 7c01 9102 7104  d.....k.r.|...q.
-00001c80: 5300 2904 721e 0000 0072 3000 0000 da01  S.).r....r0.....
-00001c90: 6eda 0029 02da 0369 6e74 da07 7265 706c  n..)...int..repl
-00001ca0: 6163 6529 0272 9000 0000 da08 6368 696c  ace).r......chil
-00001cb0: 6472 656e a901 da06 6d65 6e75 5f31 7224  dren....menu_1r$
-00001cc0: 0000 0072 2500 0000 7292 0000 00fa 0000  ...r%...r.......
-00001cd0: 0072 4800 0000 6301 0000 0000 0000 0000  .rH...c.........
-00001ce0: 0000 0001 0000 0002 0000 0053 0000 0073  ...........S...s
-00001cf0: 0800 0000 7c00 6401 1900 5300 a902 4e72  ....|.d...S...Nr
-00001d00: 3200 0000 7224 0000 00a9 01da 0178 7224  2...r$.......xr$
-00001d10: 0000 0072 2400 0000 7225 0000 0072 4100  ...r$...r%...rA.
-00001d20: 0000 fb00 0000 7248 0000 0029 01da 036b  ......rH...)...k
-00001d30: 6579 7297 0000 0072 3000 0000 7293 0000  eyr....r0...r...
-00001d40: 0072 9400 0000 728a 0000 0063 0100 0000  .r....r....c....
-00001d50: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00001d60: 5300 0000 7312 0000 007c 006a 007c 006a  S...s....|.j.|.j
-00001d70: 017c 006a 0264 019c 0353 0072 3b00 0000  .|.j.d...S.r;...
-00001d80: 723c 0000 0072 3f00 0000 7224 0000 0072  r<...r?...r$...r
-00001d90: 2400 0000 7225 0000 0072 4100 0000 0001  $...r%...rA.....
-00001da0: 0000 7248 0000 0063 0100 0000 0000 0000  ..rH...c........
-00001db0: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
-00001dc0: 7308 0000 007c 0064 0119 0053 0072 9a00  s....|.d...S.r..
-00001dd0: 0000 7224 0000 0072 9b00 0000 7224 0000  ..r$...r....r$..
-00001de0: 0072 2400 0000 7225 0000 0072 4100 0000  .r$...r%...rA...
-00001df0: 0201 0000 7248 0000 0029 1172 4d00 0000  ....rH...).rM...
-00001e00: 7243 0000 0072 0f00 0000 722e 0000 0072  rC...r....r....r
-00001e10: 2f00 0000 720e 0000 0072 3200 0000 7220  /...r....r2...r 
-00001e20: 0000 0072 4a00 0000 722c 0000 00da 0673  ...rJ...r,.....s
-00001e30: 6f72 7465 6472 9500 0000 7296 0000 00da  ortedr....r.....
-00001e40: 0566 6972 7374 7244 0000 0072 4500 0000  .firstrD...rE...
-00001e50: 7231 0000 0029 0d72 6200 0000 7238 0000  r1...).rb...r8..
-00001e60: 00da 0576 616c 7565 da10 636f 6e74 656e  ...value..conten
-00001e70: 745f 7479 7065 5f69 6473 da0f 636f 6e74  t_type_ids..cont
-00001e80: 656e 745f 7479 7065 5f65 785a 1463 6f6e  ent_type_exZ.con
-00001e90: 7465 6e74 5f74 7970 655f 6361 745f 6964  tent_type_cat_id
-00001ea0: 735a 1163 6f6e 7465 6e74 5f74 7970 655f  sZ.content_type_
-00001eb0: 6361 7473 da08 7265 6c5f 6c69 7374 da03  cats..rel_list..
-00001ec0: 7265 6cda 0f73 6572 6961 6c69 7a65 725f  rel..serializer_
-00001ed0: 7265 6c73 da08 616c 6c5f 6d65 6e75 7282  rels..all_menur.
-00001ee0: 0000 00da 0d63 6869 6c64 7265 6e5f 6c69  .....children_li
-00001ef0: 7374 7224 0000 0072 9800 0000 7225 0000  str$...r....r%..
-00001f00: 0072 8000 0000 eb00 0000 7330 0000 0000  .r........s0....
-00001f10: 0112 0110 0112 0114 0104 0108 010c 0108  ................
-00001f20: 010c 010c 0106 020e 0108 0112 0110 0108  ................
-00001f30: 0122 0104 010c 010a 010a ff0c 0210 0172  .".............r
-00001f40: 8000 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00001f50: 0004 0000 0004 0000 0043 0000 0073 2600  .........C...s&.
-00001f60: 0000 7400 6a01 a002 a100 7d01 7403 7d02  ..t.j.....}.t.}.
-00001f70: 7404 7c02 7c01 6401 8303 7d03 7405 6402  t.|.|.d...}.t.d.
-00001f80: 7c03 6901 8301 5300 7284 0000 0072 8500  |.i...S.r....r..
-00001f90: 0000 7286 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
-00001fa0: 0072 2500 0000 da10 6d65 6e75 5f70 6572  .r%.....menu_per
-00001fb0: 6d69 7373 696f 6e73 0601 0000 7308 0000  missions....s...
-00001fc0: 0000 010a 0104 010c 0172 a800 0000 6302  .........r....c.
-00001fd0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001fe0: 0000 0043 0000 0073 2c00 0000 7c01 6a00  ...C...s,...|.j.
-00001ff0: 7228 7c01 6a00 7c00 7601 7228 7c00 a001  r(|.j.|.v.r(|...
-00002000: 7c01 6a00 a101 0100 7402 7c00 7c01 6a00  |.j.....t.|.|.j.
-00002010: 8302 0100 7c00 5300 721c 0000 0072 1d00  ....|.S.r....r..
-00002020: 0000 2902 7222 0000 0072 2300 0000 7224  ..).r"...r#...r$
-00002030: 0000 0072 2400 0000 7225 0000 0072 2000  ...r$...r%...r .
-00002040: 0000 0d01 0000 730a 0000 0000 0106 010a  ......s.........
-00002050: 010c 010c 0172 2000 0000 6300 0000 0000  .....r ...c.....
-00002060: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00002070: 0000 0073 4200 0000 6500 5a01 6400 5a02  ...sB...e.Z.d.Z.
-00002080: 6503 6a04 6401 6402 6403 8d02 5a05 6503  e.j.d.d.d...Z.e.
-00002090: 6a04 6404 6402 6403 8d02 5a06 6503 6a04  j.d.d.d...Z.e.j.
-000020a0: 6405 6406 8d01 5a07 4700 6407 6408 8400  d.d...Z.G.d.d...
-000020b0: 6408 8302 5a08 6409 5300 290a da0e 486f  d...Z.d.S.)...Ho
-000020c0: 7370 6974 616c 4669 6c74 6572 723d 0000  spitalFilterr=..
-000020d0: 00da 0969 636f 6e74 6169 6e73 a902 da0a  ...icontains....
-000020e0: 6669 656c 645f 6e61 6d65 da0b 6c6f 6f6b  field_name..look
-000020f0: 7570 5f65 7870 72da 0763 6f64 656e 756d  up_expr..codenum
-00002100: 721e 0000 00a9 0172 ac00 0000 6300 0000  r......r....c...
-00002110: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00002120: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
-00002130: 5a02 6503 5a04 6401 5a05 6402 5300 2903  Z.e.Z.d.Z.d.S.).
-00002140: 7a13 486f 7370 6974 616c 4669 6c74 6572  z.HospitalFilter
-00002150: 2e4d 6574 6129 0372 3d00 0000 72ae 0000  .Meta).r=...r...
-00002160: 0072 1e00 0000 4e29 0672 7100 0000 7272  .r....N).rq...rr
-00002170: 0000 0072 7300 0000 7204 0000 0072 4900  ...rs...r....rI.
-00002180: 0000 da06 6669 656c 6473 7224 0000 0072  ....fieldsr$...r
-00002190: 2400 0000 7224 0000 0072 2500 0000 da04  $...r$...r%.....
-000021a0: 4d65 7461 1a01 0000 7304 0000 0008 0104  Meta....s.......
-000021b0: 0172 b100 0000 4e29 0972 7100 0000 7272  .r....N).rq...rr
-000021c0: 0000 0072 7300 0000 da07 6669 6c74 6572  ...rs.....filter
-000021d0: 73da 0a43 6861 7246 696c 7465 7272 3d00  s..CharFilterr=.
-000021e0: 0000 72ae 0000 0072 1e00 0000 72b1 0000  ..r....r....r...
-000021f0: 0072 2400 0000 7224 0000 0072 2400 0000  .r$...r$...r$...
-00002200: 7225 0000 0072 a900 0000 1501 0000 7308  r%...r........s.
-00002210: 0000 0008 010e 010e 010c 0272 a900 0000  ...........r....
-00002220: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002230: 0003 0000 0040 0000 0073 2800 0000 6500  .....@...s(...e.
-00002240: 5a01 6400 5a02 6503 6a04 6a05 6401 6402  Z.d.Z.e.j.j.d.d.
-00002250: 8d01 a006 6403 a101 5a07 6508 5a09 650a  ....d...Z.e.Z.e.
-00002260: 5a0b 6404 5300 2905 da0f 486f 7370 6974  Z.d.S.)...Hospit
-00002270: 616c 5669 6577 5365 7454 a901 7264 0000  alViewSetT..rd..
-00002280: 0072 3000 0000 4e29 0c72 7100 0000 7272  .r0...N).rq...rr
-00002290: 0000 0072 7300 0000 7204 0000 0072 2e00  ...rs...r....r..
-000022a0: 0000 722f 0000 0072 3200 0000 7274 0000  ..r/...r2...rt..
-000022b0: 0072 1600 0000 7275 0000 0072 a900 0000  .r....ru...r....
-000022c0: da0f 6669 6c74 6572 7365 745f 636c 6173  ..filterset_clas
-000022d0: 7372 2400 0000 7224 0000 0072 2400 0000  sr$...r$...r$...
-000022e0: 7225 0000 0072 b400 0000 2301 0000 7306  r%...r....#...s.
-000022f0: 0000 0008 0114 0104 0172 b400 0000 6300  .........r....c.
-00002300: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00002310: 0000 0040 0000 0073 5c00 0000 6500 5a01  ...@...s\...e.Z.
-00002320: 6400 5a02 6503 6a04 6401 6402 6403 8d02  d.Z.e.j.d.d.d...
-00002330: 5a05 6503 6a04 6404 6402 6403 8d02 5a06  Z.e.j.d.d.d...Z.
-00002340: 6503 6a04 6405 6402 6403 8d02 5a07 6503  e.j.d.d.d...Z.e.
-00002350: 6a04 6406 6407 8d01 5a08 6503 6a04 6408  j.d.d...Z.e.j.d.
-00002360: 6407 8d01 5a09 4700 6409 640a 8400 640a  d...Z.G.d.d...d.
-00002370: 8302 5a0a 640b 5300 290c da0c 4f66 6669  ..Z.d.S.)...Offi
-00002380: 6365 4669 6c74 6572 723d 0000 0072 aa00  ceFilterr=...r..
-00002390: 0000 72ab 0000 0072 ae00 0000 da0b 6f66  ..r....r......of
-000023a0: 6669 6365 5f74 7970 6572 6700 0000 72af  fice_typerg...r.
-000023b0: 0000 0072 1e00 0000 6300 0000 0000 0000  ...r....c.......
-000023c0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-000023d0: 0073 1800 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
-000023e0: 5a04 6401 5a05 6402 5a06 6403 5300 2904  Z.d.Z.d.Z.d.S.).
-000023f0: 7a11 4f66 6669 6365 4669 6c74 6572 2e4d  z.OfficeFilter.M
-00002400: 6574 6172 1b00 0000 2903 723d 0000 0072  etar....).r=...r
-00002410: ae00 0000 72b8 0000 004e 2907 7271 0000  ....r....N).rq..
-00002420: 0072 7200 0000 7273 0000 0072 0500 0000  .rr...rs...r....
-00002430: 7249 0000 0072 b000 0000 da0d 7365 6172  rI...r......sear
-00002440: 6368 5f66 6965 6c64 7372 2400 0000 7224  ch_fieldsr$...r$
-00002450: 0000 0072 2400 0000 7225 0000 0072 b100  ...r$...r%...r..
-00002460: 0000 3101 0000 7306 0000 0008 0104 0104  ..1...s.........
-00002470: 0172 b100 0000 4e29 0b72 7100 0000 7272  .r....N).rq...rr
-00002480: 0000 0072 7300 0000 72b2 0000 0072 b300  ...rs...r....r..
-00002490: 0000 723d 0000 0072 ae00 0000 72b8 0000  ..r=...r....r...
-000024a0: 0072 6700 0000 721e 0000 0072 b100 0000  .rg...r....r....
-000024b0: 7224 0000 0072 2400 0000 7224 0000 0072  r$...r$...r$...r
-000024c0: 2500 0000 72b7 0000 002a 0100 0073 0c00  %...r....*...s..
-000024d0: 0000 0801 0e01 0e01 0e01 0c01 0c02 72b7  ..............r.
-000024e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000024f0: 0000 0000 0300 0000 4000 0000 732a 0000  ........@...s*..
-00002500: 0065 005a 0164 005a 0265 036a 046a 0564  .e.Z.d.Z.e.j.j.d
-00002510: 0164 028d 015a 0665 075a 0865 095a 0a64  .d...Z.e.Z.e.Z.d
-00002520: 0364 0484 005a 0b64 0553 0029 06da 0d4f  .d...Z.d.S.)...O
-00002530: 6666 6963 6556 6965 7753 6574 5472 b500  fficeViewSetTr..
-00002540: 0000 6302 0000 0000 0000 0000 0000 0007  ..c.............
-00002550: 0000 0004 0000 004f 0000 0073 5e00 0000  .......O...s^...
-00002560: 7c00 a000 7c00 a001 a100 a101 7d04 6401  |...|.......}.d.
-00002570: 7c00 6a02 6a03 a004 a100 7600 7242 7c00  |.j.j.....v.rB|.
-00002580: a005 7c04 a101 7d05 7c00 6a06 7c05 6402  ..|...}.|.j.|.d.
-00002590: 6403 8d02 7d06 7c00 a007 7c06 6a08 a101  d...}.|...|.j...
-000025a0: 5300 7c00 6a06 7c04 6402 6403 8d02 7d06  S.|.j.|.d.d...}.
-000025b0: 7409 6404 7c06 6a08 6901 8301 5300 2905  t.d.|.j.i...S.).
-000025c0: 4eda 0470 6167 6554 728e 0000 00da 0772  N..pageTr......r
-000025d0: 6573 756c 7473 290a da0f 6669 6c74 6572  esults)...filter
-000025e0: 5f71 7565 7279 7365 74da 0c67 6574 5f71  _queryset..get_q
-000025f0: 7565 7279 7365 7472 3500 0000 da0c 7175  uerysetr5.....qu
-00002600: 6572 795f 7061 7261 6d73 da04 6b65 7973  ery_params..keys
-00002610: da11 7061 6769 6e61 7465 5f71 7565 7279  ..paginate_query
-00002620: 7365 74da 0e67 6574 5f73 6572 6961 6c69  set..get_seriali
-00002630: 7a65 72da 1667 6574 5f70 6167 696e 6174  zer..get_paginat
-00002640: 6564 5f72 6573 706f 6e73 6572 2c00 0000  ed_responser,...
-00002650: 7202 0000 0029 0772 2100 0000 7235 0000  r....).r!...r5..
-00002660: 0072 5e00 0000 725f 0000 0072 7400 0000  .r^...r_...rt...
-00002670: 72bb 0000 0072 6200 0000 7224 0000 0072  r....rb...r$...r
-00002680: 2400 0000 7225 0000 0072 4d00 0000 3d01  $...r%...rM...=.
-00002690: 0000 730e 0000 0000 010e 0210 010a 020e  ..s.............
-000026a0: 010c 020e 017a 124f 6666 6963 6556 6965  .....z.OfficeVie
-000026b0: 7753 6574 2e6c 6973 744e 290c 7271 0000  wSet.listN).rq..
-000026c0: 0072 7200 0000 7273 0000 0072 0500 0000  .rr...rs...r....
-000026d0: 722e 0000 0072 2f00 0000 7274 0000 0072  r....r/...rt...r
-000026e0: 1700 0000 7275 0000 0072 b700 0000 72b6  ....ru...r....r.
-000026f0: 0000 0072 4d00 0000 7224 0000 0072 2400  ...rM...r$...r$.
-00002700: 0000 7224 0000 0072 2500 0000 72ba 0000  ..r$...r%...r...
-00002710: 0037 0100 0073 0800 0000 0801 0e01 0402  .7...s..........
-00002720: 0402 72ba 0000 0063 0000 0000 0000 0000  ..r....c........
-00002730: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00002740: 7344 0000 0065 005a 0164 005a 0265 036a  sD...e.Z.d.Z.e.j
-00002750: 0464 0164 0264 038d 025a 0565 036a 0464  .d.d.d...Z.e.j.d
-00002760: 0464 0264 038d 025a 0665 036a 0464 0564  .d.d...Z.e.j.d.d
-00002770: 0264 038d 025a 0747 0064 0664 0784 0064  .d...Z.G.d.d...d
-00002780: 0783 025a 0864 0853 0029 09da 0c44 6f63  ...Z.d.S.)...Doc
-00002790: 746f 7246 696c 7465 7272 3d00 0000 72aa  torFilterr=...r.
-000027a0: 0000 0072 ab00 0000 da0a 6a6f 625f 6e75  ...r......job_nu
-000027b0: 6d62 6572 da05 7068 6f6e 6563 0000 0000  mber..phonec....
-000027c0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-000027d0: 4000 0000 7318 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-000027e0: 0265 035a 0464 015a 0564 025a 0664 0353  .e.Z.d.Z.d.Z.d.S
-000027f0: 0029 047a 1144 6f63 746f 7246 696c 7465  .).z.DoctorFilte
-00002800: 722e 4d65 7461 721b 0000 0029 0372 3d00  r.Metar....).r=.
-00002810: 0000 72c5 0000 0072 c600 0000 4e29 0772  ..r....r....N).r
-00002820: 7100 0000 7272 0000 0072 7300 0000 7206  q...rr...rs...r.
-00002830: 0000 0072 4900 0000 72b0 0000 0072 b900  ...rI...r....r..
-00002840: 0000 7224 0000 0072 2400 0000 7224 0000  ..r$...r$...r$..
-00002850: 0072 2500 0000 72b1 0000 004f 0100 0073  .r%...r....O...s
-00002860: 0600 0000 0801 0401 0401 72b1 0000 004e  ..........r....N
-00002870: 2909 7271 0000 0072 7200 0000 7273 0000  ).rq...rr...rs..
-00002880: 0072 b200 0000 72b3 0000 0072 3d00 0000  .r....r....r=...
-00002890: 72c5 0000 0072 c600 0000 72b1 0000 0072  r....r....r....r
-000028a0: 2400 0000 7224 0000 0072 2400 0000 7225  $...r$...r$...r%
-000028b0: 0000 0072 c400 0000 4a01 0000 7308 0000  ...r....J...s...
-000028c0: 0008 010e 010e 010e 0272 c400 0000 6300  .........r....c.
-000028d0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000028e0: 0000 0040 0000 0073 3200 0000 6500 5a01  ...@...s2...e.Z.
-000028f0: 6400 5a02 6503 6a04 6a05 6401 6402 8d01  d.Z.e.j.j.d.d...
-00002900: 5a06 6507 5a08 6509 5a0a 6403 6404 8400  Z.e.Z.e.Z.d.d...
-00002910: 5a0b 6405 6406 8400 5a0c 6407 5300 2908  Z.d.d...Z.d.S.).
-00002920: da0d 446f 6374 6f72 5669 6577 5365 7454  ..DoctorViewSetT
-00002930: 72b5 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00002940: 0000 0800 0000 0500 0000 4f00 0000 73aa  ..........O...s.
-00002950: 0000 007c 00a0 007c 00a0 01a1 00a1 017d  ...|...|.......}
-00002960: 0464 007d 0564 017c 006a 026a 03a0 04a1  .d.}.d.|.j.j....
-00002970: 0076 0072 2c7c 00a0 057c 04a1 017d 057c  .v.r,|...|...}.|
-00002980: 0564 0075 0172 4e7c 006a 067c 0564 0264  .d.u.rN|.j.|.d.d
-00002990: 038d 027d 067c 00a0 077c 066a 08a1 0153  ...}.|...|.j...S
-000029a0: 0064 047c 006a 026a 03a0 04a1 0076 0072  .d.|.j.j.....v.r
-000029b0: 8e7c 006a 026a 03a0 0964 04a1 017d 077c  .|.j.j...d...}.|
-000029c0: 006a 067c 0464 0264 047c 0769 0164 058d  .j.|.d.d.|.i.d..
-000029d0: 037d 0674 0a64 067c 066a 0869 0183 0153  .}.t.d.|.j.i...S
-000029e0: 007c 006a 067c 0464 0264 038d 027d 0674  .|.j.|.d.d...}.t
-000029f0: 0a64 067c 066a 0869 0183 0153 0029 074e  .d.|.j.i...S.).N
-00002a00: 72bb 0000 0054 728e 0000 00da 0866 6565  r....Tr......fee
-00002a10: 5f74 7970 6529 0272 8f00 0000 da07 636f  _type).r......co
-00002a20: 6e74 6578 7472 bc00 0000 290b 72bd 0000  ntextr....).r...
-00002a30: 0072 be00 0000 7235 0000 0072 bf00 0000  .r....r5...r....
-00002a40: 72c0 0000 0072 c100 0000 72c2 0000 0072  r....r....r....r
-00002a50: c300 0000 722c 0000 0072 6b00 0000 7202  ....r,...rk...r.
-00002a60: 0000 0029 0872 2100 0000 7235 0000 0072  ...).r!...r5...r
-00002a70: 5e00 0000 725f 0000 0072 7400 0000 72bb  ^...r_...rt...r.
-00002a80: 0000 0072 6200 0000 72c8 0000 0072 2400  ...rb...r....r$.
-00002a90: 0000 7224 0000 0072 2500 0000 724d 0000  ..r$...r%...rM..
-00002aa0: 005a 0100 0073 1a00 0000 0001 0e01 0401  .Z...s..........
-00002ab0: 1001 0a01 0801 0e01 0c01 1001 0e01 1401  ................
-00002ac0: 0e02 0e01 7a12 446f 6374 6f72 5669 6577  ....z.DoctorView
-00002ad0: 5365 742e 6c69 7374 6302 0000 0000 0000  Set.listc.......
-00002ae0: 0000 0000 0007 0000 0004 0000 004f 0000  .............O..
-00002af0: 0073 5600 0000 7c00 a000 a100 7d04 6401  .sV...|.....}.d.
-00002b00: 7c00 6a01 6a02 a003 a100 7600 7242 7c00  |.j.j.....v.rB|.
-00002b10: 6a01 6a02 a004 6401 a101 7d05 7c00 6a05  j.j...d...}.|.j.
-00002b20: 7c04 6401 7c05 6901 6402 8d02 7d06 7406  |.d.|.i.d...}.t.
-00002b30: 7c06 6a07 8301 5300 7c00 a005 7c04 a101  |.j...S.|...|...
-00002b40: 7d06 7406 7c06 6a07 8301 5300 2903 4e72  }.t.|.j...S.).Nr
-00002b50: c800 0000 2901 72c9 0000 0029 0872 2d00  ....).r....).r-.
-00002b60: 0000 7235 0000 0072 bf00 0000 72c0 0000  ..r5...r....r...
-00002b70: 0072 6b00 0000 72c2 0000 0072 0200 0000  .rk...r....r....
-00002b80: 722c 0000 0029 0772 2100 0000 7235 0000  r,...).r!...r5..
-00002b90: 0072 5e00 0000 725f 0000 00da 0869 6e73  .r^...r_.....ins
-00002ba0: 7461 6e63 6572 c800 0000 7262 0000 0072  tancer....rb...r
-00002bb0: 2400 0000 7224 0000 0072 2500 0000 da08  $...r$...r%.....
-00002bc0: 7265 7472 6965 7665 6a01 0000 730e 0000  retrievej...s...
-00002bd0: 0000 0108 0110 010e 0112 010a 010a 017a  ...............z
-00002be0: 1644 6f63 746f 7256 6965 7753 6574 2e72  .DoctorViewSet.r
-00002bf0: 6574 7269 6576 654e 290d 7271 0000 0072  etrieveN).rq...r
-00002c00: 7200 0000 7273 0000 0072 0600 0000 722e  r...rs...r....r.
-00002c10: 0000 0072 2f00 0000 7274 0000 0072 1800  ...r/...rt...r..
-00002c20: 0000 7275 0000 0072 c400 0000 72b6 0000  ..ru...r....r...
-00002c30: 0072 4d00 0000 72cb 0000 0072 2400 0000  .rM...r....r$...
-00002c40: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
-00002c50: c700 0000 5501 0000 730a 0000 0008 010e  ....U...s.......
-00002c60: 0104 0104 0208 1072 c700 0000 2936 7256  .......r....)6rV
-00002c70: 0000 00da 1772 6573 745f 6672 616d 6577  .....rest_framew
-00002c80: 6f72 6b2e 7265 7370 6f6e 7365 7202 0000  ork.responser...
-00002c90: 00da 1772 6573 745f 6672 616d 6577 6f72  ...rest_framewor
-00002ca0: 6b2e 7669 6577 7365 7473 7203 0000 00da  k.viewsetsr.....
-00002cb0: 0e64 6a61 6e67 6f5f 6669 6c74 6572 7372  .django_filtersr
-00002cc0: b200 0000 da12 6261 7365 5f73 7973 7465  ......base_syste
-00002cd0: 6d2e 6d6f 6465 6c73 7204 0000 0072 0500  m.modelsr....r..
-00002ce0: 0000 7206 0000 00da 1a64 6a61 6e67 6f2e  ..r......django.
-00002cf0: 636f 6e74 7269 622e 6175 7468 2e6d 6f64  contrib.auth.mod
-00002d00: 656c 7372 0700 0000 7208 0000 00da 0b64  elsr....r......d
-00002d10: 6a61 6e67 6f2e 6874 7470 7209 0000 00da  jango.httpr.....
-00002d20: 1972 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
-00002d30: 6578 6365 7074 696f 6e73 720a 0000 00da  exceptionsr.....
-00002d40: 1972 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
-00002d50: 6465 636f 7261 746f 7273 720b 0000 00da  decoratorsr.....
-00002d60: 0e72 6573 745f 6672 616d 6577 6f72 6b72  .rest_frameworkr
-00002d70: 0c00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
-00002d80: 0000 0072 1000 0000 da17 6261 7365 5f73  ...r......base_s
-00002d90: 7973 7465 6d2e 7365 7269 616c 697a 6572  ystem.serializer
-00002da0: 7372 1100 0000 7212 0000 0072 1300 0000  sr....r....r....
-00002db0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00002dc0: 1700 0000 7218 0000 00da 0964 6a61 6e67  ....r......djang
-00002dd0: 6f2e 6462 7219 0000 0072 1a00 0000 7278  o.dbr....r....rx
-00002de0: 0000 0072 7900 0000 727b 0000 0072 8300  ...ry...r{...r..
-00002df0: 0000 7287 0000 0072 8800 0000 7280 0000  ..r....r....r...
-00002e00: 0072 a800 0000 7220 0000 00da 0946 696c  .r....r .....Fil
-00002e10: 7465 7253 6574 72a9 0000 0072 b400 0000  terSetr....r....
-00002e20: 72b7 0000 0072 ba00 0000 72c4 0000 0072  r....r....r....r
-00002e30: c700 0000 7224 0000 0072 2400 0000 7224  ....r$...r$...r$
-00002e40: 0000 0072 2500 0000 da08 3c6d 6f64 756c  ...r%.....<modul
-00002e50: 653e 0100 0000 733a 0000 0008 020c 010c  e>....s:........
-00002e60: 0108 0114 0310 010c 010c 010c 010c 021c  ................
-00002e70: 0128 020c 0310 7f00 2810 0610 0710 0608  .(......(.......
-00002e80: 0e08 0710 0708 1b08 0708 0812 0e10 0712  ................
-00002e90: 0d10 1312 0b                             .....
+00000f90: 6408 3c00 7c01 a001 6409 a101 7c02 640a  d.<.|...d...|.d.
+00000fa0: 3c00 7402 7c02 640b 8d01 7d03 7c03 6a03  <.t.|.d...}.|.j.
+00000fb0: 640c 640d 8d01 0100 7c03 6a04 7d02 7400  d.d.....|.j.}.t.
+00000fc0: 8300 7d04 7c01 a001 640e a101 7d05 7c05  ..}.|...d...}.|.
+00000fd0: 729e 7c05 6e02 6700 7c04 640e 3c00 7c01  r.|.n.g.|.d.<.|.
+00000fe0: a001 6409 a101 72d4 7c01 a001 6409 a101  ..d...r.|...d...
+00000ff0: 7c04 6409 3c00 7405 7c04 640b 8d01 7d03  |.d.<.t.|.d...}.
+00001000: 7c03 6a03 640c 640d 8d01 0100 7c02 7c04  |.j.d.d.....|.|.
+00001010: 6602 5300 290f 4eda 046e 6f74 65da 0969  f.S.).N..note..i
+00001020: 735f 6163 7469 7665 e901 0000 00da 0b68  s_active.......h
+00001030: 6f73 7069 7461 6c5f 6964 da08 686f 7370  ospital_id..hosp
+00001040: 6974 616c 7232 0000 00da 0c63 7265 6174  italr2.....creat
+00001050: 6564 5f75 7365 72da 0972 6f6c 655f 636f  ed_user..role_co
+00001060: 6465 723d 0000 00da 0972 6f6c 655f 6e61  der=.....role_na
+00001070: 6d65 7253 0000 0054 7254 0000 0072 5200  merS...TrT...rR.
+00001080: 0000 2906 da04 6469 6374 da03 6765 7472  ..)...dict..getr
+00001090: 1200 0000 725c 0000 0072 2c00 0000 7211  ....r\...r,...r.
+000010a0: 0000 0029 0672 2100 0000 722c 0000 0072  ...).r!...r,...r
+000010b0: 6000 0000 7262 0000 0072 6100 0000 7238  `...rb...ra...r8
+000010c0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+000010d0: 0000 7259 0000 0085 0000 0073 2600 0000  ..rY.......s&...
+000010e0: 0002 0602 0e01 1001 0e01 0e01 0e01 0e01  ................
+000010f0: 0e01 0a01 0c01 0603 0601 0a02 1001 0a01  ................
+00001100: 0e01 0a01 0c03 7a17 4772 6f75 7056 6965  ......z.GroupVie
+00001110: 7753 6574 2e63 6865 636b 5f64 6174 6163  wSet.check_datac
+00001120: 0200 0000 0000 0000 0000 0000 0800 0000  ................
+00001130: 0400 0000 4f00 0000 73c2 0000 007c 00a0  ....O...s....|..
+00001140: 00a1 007d 047c 046a 017d 057c 016a 02a0  ...}.|.j.}.|.j..
+00001150: 0364 01a1 017c 046a 046b 0272 287c 016a  .d...|.j.k.r(|.j
+00001160: 0264 013d 007c 00a0 057c 016a 02a1 015c  .d.=.|...|.j...\
+00001170: 027d 067d 077c 0664 0219 007c 055f 067c  .}.}.|.d...|._.|
+00001180: 0664 0319 007c 055f 077c 0664 0419 007c  .d...|._.|.d...|
+00001190: 055f 087c 0664 0519 007c 055f 097c 0664  ._.|.d...|._.|.d
+000011a0: 0619 007c 055f 0a7c 0664 0719 007c 055f  ...|._.|.d...|._
+000011b0: 0b7c 0664 0819 007c 055f 0c7c 05a0 0da1  .|.d...|._.|....
+000011c0: 0001 007c 07a0 0364 017c 046a 04a1 027c  ...|...d.|.j...|
+000011d0: 045f 047c 046a 0ea0 0f7c 0764 0919 00a1  ._.|.j...|.d....
+000011e0: 0101 007c 04a0 0da1 0001 0074 1074 117c  ...|.......t.t.|
+000011f0: 0483 016a 0274 126a 1364 0a8d 0253 0029  ...j.t.j.d...S.)
+00001200: 0b4e 723d 0000 0072 6300 0000 7264 0000  .Nr=...rc...rd..
+00001210: 0072 3200 0000 7267 0000 0072 6800 0000  .r2...rg...rh...
+00001220: 7269 0000 0072 6a00 0000 7252 0000 0072  ri...rj...rR...r
+00001230: 2b00 0000 2914 722d 0000 00da 0b65 7874  +...).r-.....ext
+00001240: 7261 5f67 726f 7570 722c 0000 0072 6c00  ra_groupr,...rl.
+00001250: 0000 723d 0000 0072 5900 0000 7263 0000  ..r=...rY...rc..
+00001260: 0072 6400 0000 da05 696e 6465 7872 6600  .rd.....indexrf.
+00001270: 0000 7268 0000 0072 6900 0000 726a 0000  ..rh...ri...rj..
+00001280: 0072 5b00 0000 7238 0000 0072 4a00 0000  .r[...r8...rJ...
+00001290: 7202 0000 0072 1100 0000 720c 0000 00da  r....r....r.....
+000012a0: 1648 5454 505f 3230 355f 5245 5345 545f  .HTTP_205_RESET_
+000012b0: 434f 4e54 454e 5429 0872 2100 0000 7235  CONTENT).r!...r5
+000012c0: 0000 0072 5e00 0000 725f 0000 0072 2900  ...r^...r_...r).
+000012d0: 0000 726d 0000 0072 6000 0000 7261 0000  ..rm...r`...ra..
+000012e0: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+000012f0: da06 7570 6461 7465 a100 0000 7322 0000  ..update....s"..
+00001300: 0000 0208 0106 0112 0108 0110 010a 010a  ................
+00001310: 010a 010a 010a 010a 010a 0108 0110 0210  ................
+00001320: 0108 017a 1347 726f 7570 5669 6577 5365  ...z.GroupViewSe
+00001330: 742e 7570 6461 7465 4e29 15da 085f 5f6e  t.updateN)...__n
+00001340: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00001350: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00001360: 0700 0000 722e 0000 0072 3100 0000 da08  ....r....r1.....
+00001370: 7175 6572 7973 6574 7211 0000 00da 1073  querysetr......s
+00001380: 6572 6961 6c69 7a65 725f 636c 6173 73da  erializer_class.
+00001390: 0d66 696c 7465 725f 6669 656c 6473 7220  .filter_fieldsr 
+000013a0: 0000 0072 0b00 0000 7239 0000 0072 3a00  ...r....r9...r:.
+000013b0: 0000 7247 0000 0072 3300 0000 7219 0000  ..rG...r3...r...
+000013c0: 00da 0661 746f 6d69 6372 5a00 0000 7259  ...atomicrZ...rY
+000013d0: 0000 0072 7000 0000 7224 0000 0072 2400  ...rp...r$...r$.
+000013e0: 0000 7224 0000 0072 2500 0000 721a 0000  ..r$...r%...r...
+000013f0: 0015 0000 0073 2000 0000 0801 0a01 0401  .....s .........
+00001400: 0403 0806 0c01 0a09 0c01 0a08 0c01 0a1a  ................
+00001410: 0822 0401 0a13 081c 0401 721a 0000 0063  ."........r....c
+00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001430: 0200 0000 4000 0000 731e 0000 0065 005a  ....@...s....e.Z
+00001440: 0164 005a 0265 036a 04a0 05a1 005a 0665  .d.Z.e.j.....Z.e
+00001450: 075a 0864 015a 0964 0253 0029 03da 1145  .Z.d.Z.d.S.)...E
+00001460: 7874 7261 4772 6f75 7056 6965 7753 6574  xtraGroupViewSet
+00001470: 721b 0000 004e 290a 7271 0000 0072 7200  r....N).rq...rr.
+00001480: 0000 7273 0000 0072 0d00 0000 722e 0000  ..rs...r....r...
+00001490: 0072 3100 0000 7274 0000 0072 1200 0000  .r1...rt...r....
+000014a0: 7275 0000 0072 7600 0000 7224 0000 0072  ru...rv...r$...r
+000014b0: 2400 0000 7224 0000 0072 2500 0000 7278  $...r$...r%...rx
+000014c0: 0000 00bd 0000 0073 0600 0000 0801 0a01  .......s........
+000014d0: 0401 7278 0000 0063 0000 0000 0000 0000  ..rx...c........
+000014e0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+000014f0: 7322 0000 0065 005a 0164 005a 0265 036a  s"...e.Z.d.Z.e.j
+00001500: 04a0 05a1 005a 0665 075a 0864 015a 0964  .....Z.e.Z.d.Z.d
+00001510: 025a 0a64 0153 0029 03da 1743 6f6e 7465  .Z.d.S.)...Conte
+00001520: 6e74 5479 7065 4361 7465 7356 6965 7753  ntTypeCatesViewS
+00001530: 6574 4e72 1b00 0000 290b 7271 0000 0072  etNr....).rq...r
+00001540: 7200 0000 7273 0000 0072 0e00 0000 722e  r...rs...r....r.
+00001550: 0000 0072 3100 0000 7274 0000 0072 1300  ...r1...rt...r..
+00001560: 0000 7275 0000 00da 1070 6167 696e 6174  ..ru.....paginat
+00001570: 696f 6e5f 636c 6173 7372 7600 0000 7224  ion_classrv...r$
+00001580: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00001590: 0000 7279 0000 00c3 0000 0073 0800 0000  ..ry.......s....
+000015a0: 0801 0a01 0401 0401 7279 0000 0063 0000  ........ry...c..
+000015b0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+000015c0: 0000 4000 0000 731e 0000 0065 005a 0164  ..@...s....e.Z.d
+000015d0: 005a 0265 036a 04a0 05a1 005a 0665 075a  .Z.e.j.....Z.e.Z
+000015e0: 0864 015a 0964 0253 0029 03da 1443 6f6e  .d.Z.d.S.)...Con
+000015f0: 7465 6e74 5479 7065 4578 5669 6577 5365  tentTypeExViewSe
+00001600: 7472 1b00 0000 4e29 0a72 7100 0000 7272  tr....N).rq...rr
+00001610: 0000 0072 7300 0000 720f 0000 0072 2e00  ...rs...r....r..
+00001620: 0000 7231 0000 0072 7400 0000 7214 0000  ..r1...rt...r...
+00001630: 0072 7500 0000 7276 0000 0072 2400 0000  .ru...rv...r$...
+00001640: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
+00001650: 7b00 0000 ca00 0000 7306 0000 0008 010a  {.......s.......
+00001660: 0104 0172 7b00 0000 6301 0000 0000 0000  ...r{...c.......
+00001670: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
+00001680: 0073 5600 0000 7c00 6a00 a001 6401 a101  .sV...|.j...d...
+00001690: 7d01 7402 6a03 6a01 7c00 6a00 a001 6401  }.t.j.j.|.j...d.
+000016a0: a101 6402 8d01 7d02 7c02 6a04 7d03 7405  ..d...}.|.j.}.t.
+000016b0: 6a03 6a06 7c03 6403 8d01 a007 a100 7d04  j.j.|.d.......}.
+000016c0: 7408 7d05 7409 7c05 7c04 6404 8303 7d06  t.}.t.|.|.d...}.
+000016d0: 740a 6405 7c06 6901 8301 5300 2906 4eda  t.d.|.i...S.).N.
+000016e0: 0775 7365 725f 6964 2901 7230 0000 0029  .user_id).r0...)
+000016f0: 01da 0967 726f 7570 5f5f 696e 7201 0000  ...group__inr...
+00001700: 0072 2c00 0000 290b 7226 0000 0072 6c00  .r,...).r&...rl.
+00001710: 0000 7210 0000 0072 2e00 0000 da0d 6765  ..r....r......ge
+00001720: 745f 616c 6c67 726f 7570 7372 0800 0000  t_allgroupsr....
+00001730: 722f 0000 00da 0864 6973 7469 6e63 7472  r/.....distinctr
+00001740: 1500 0000 da0f 6765 745f 7065 726d 6973  ......get_permis
+00001750: 7369 6f6e 7372 0900 0000 2907 7235 0000  sionsr....).r5..
+00001760: 0072 7c00 0000 da04 7573 6572 5a09 616c  .r|.....userZ.al
+00001770: 6c67 726f 7570 7372 3800 0000 7262 0000  lgroupsr8...rb..
+00001780: 00da 096d 656e 755f 6c69 7374 7224 0000  ...menu_listr$..
+00001790: 0072 2400 0000 7225 0000 00da 1367 6574  .r$...r%.....get
+000017a0: 5f6f 776e 5f70 6572 6d69 7373 696f 6e73  _own_permissions
+000017b0: d000 0000 730e 0000 0000 010c 0116 0506  ....s...........
+000017c0: 0112 0104 010c 0172 8300 0000 6301 0000  .......r....c...
+000017d0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+000017e0: 0043 0000 0073 2600 0000 7400 6a01 a002  .C...s&...t.j...
+000017f0: a100 7d01 7403 7d02 7404 7c02 7c01 6401  ..}.t.}.t.|.|.d.
+00001800: 8303 7d03 7405 6402 7c03 6901 8301 5300  ..}.t.d.|.i...S.
+00001810: a903 4e72 6500 0000 722c 0000 00a9 0672  ..Nre...r,.....r
+00001820: 0800 0000 722e 0000 0072 3100 0000 7215  ....r....r1...r.
+00001830: 0000 0072 8000 0000 7209 0000 00a9 0472  ...r....r......r
+00001840: 3500 0000 7238 0000 0072 6200 0000 7282  5...r8...rb...r.
+00001850: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00001860: 0000 da0f 616c 6c5f 7065 726d 6973 7369  ....all_permissi
+00001870: 6f6e 73de 0000 0073 0800 0000 0001 0a01  ons....s........
+00001880: 0401 0c01 7287 0000 0063 0000 0000 0000  ....r....c......
+00001890: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+000018a0: 0000 7328 0000 0065 005a 0164 005a 0265  ..s(...e.Z.d.Z.e
+000018b0: 036a 046a 0564 0164 0264 038d 025a 0665  .j.j.d.d.d...Z.e
+000018c0: 075a 0864 025a 0964 045a 0a64 0253 0029  .Z.d.Z.d.Z.d.S.)
+000018d0: 05da 0b4d 656e 7556 6965 7753 6574 544e  ...MenuViewSetTN
+000018e0: 2902 7264 0000 0072 1e00 0000 721b 0000  ).rd...r....r...
+000018f0: 0029 0b72 7100 0000 7272 0000 0072 7300  .).rq...rr...rs.
+00001900: 0000 720e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
+00001910: 0072 7400 0000 7215 0000 0072 7500 0000  .rt...r....ru...
+00001920: 727a 0000 0072 7600 0000 7224 0000 0072  rz...rv...r$...r
+00001930: 2400 0000 7224 0000 0072 2500 0000 7288  $...r$...r%...r.
+00001940: 0000 00e5 0000 0073 0800 0000 0801 1001  .......s........
+00001950: 0401 0401 7288 0000 0063 0300 0000 0000  ....r....c......
+00001960: 0000 0000 0000 0d00 0000 0700 0000 0300  ................
+00001970: 0000 732c 0100 0074 0074 0164 0164 0284  ..s,...t.t.d.d..
+00001980: 007c 0183 0283 017d 0374 026a 036a 0464  .|.....}.t.j.j.d
+00001990: 037c 0364 048d 027d 0474 0074 0164 0564  .|.d...}.t.t.d.d
+000019a0: 0284 007c 0483 0283 017d 0574 056a 036a  ...|.....}.t.j.j
+000019b0: 047c 0564 068d 01a0 0664 07a1 017d 0667  .|.d.....d...}.g
+000019c0: 007d 077c 0644 005d 0e7d 0874 077c 077c  .}.|.D.].}.t.|.|
+000019d0: 0883 0201 0071 507c 077c 0637 007d 0774  .....qP|.|.7.}.t
+000019e0: 0074 087c 0783 0183 017d 077c 007c 0764  .t.|.....}.|.|.d
+000019f0: 0364 088d 027d 097c 096a 097d 0a64 0964  .d...}.|.j.}.d.d
+00001a00: 0a84 007c 0a44 0083 017d 0b7c 0a44 005d  ...|.D...}.|.D.]
+00001a10: 7e89 0087 0066 0164 0b64 0a84 087c 0a44  ~....f.d.d...|.D
+00001a20: 0083 017d 0c74 0a7c 0c64 0c64 0284 0064  ...}.t.|.d.d...d
+00001a30: 0d8d 027d 0c7c 0c88 0064 0e3c 0074 026a  ...}.|...d.<.t.j
+00001a40: 036a 0474 0b88 0064 0f19 00a0 0c64 1064  .j.t...d.....d.d
+00001a50: 11a1 0283 0164 128d 01a0 0da1 007d 047c  .....d.......}.|
+00001a60: 0272 987c 0472 987c 0c67 006b 0272 9874  .r.|.r.|.g.k.r.t
+00001a70: 0074 0164 1364 0284 007c 046a 0e6a 0fa0  .t.d.d...|.j.j..
+00001a80: 10a1 0083 0283 0188 0064 0e3c 0071 9874  .........d.<.q.t
+00001a90: 0a7c 0b64 1464 0284 0064 0d8d 027d 0b7c  .|.d.d...d...}.|
+00001aa0: 0b53 0029 154e 6301 0000 0000 0000 0000  .S.).Nc.........
+00001ab0: 0000 0001 0000 0001 0000 0053 0000 0073  ...........S...s
+00001ac0: 0600 0000 7c00 6a00 5300 721c 0000 0029  ....|.j.S.r....)
+00001ad0: 0172 2a00 0000 2901 da04 7065 726d 7224  .r*...)...permr$
+00001ae0: 0000 0072 2400 0000 7225 0000 0072 4100  ...r$...r%...rA.
+00001af0: 0000 ed00 0000 7248 0000 007a 2167 6574  ......rH...z!get
+00001b00: 5f70 6572 6d69 7373 696f 6e73 2e3c 6c6f  _permissions.<lo
+00001b10: 6361 6c73 3e2e 3c6c 616d 6264 613e 5429  cals>.<lambda>T)
+00001b20: 0272 6400 0000 5a13 636f 6e74 656e 745f  .rd...Z.content_
+00001b30: 7479 7065 5f69 645f 5f69 6e63 0100 0000  type_id__inc....
+00001b40: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00001b50: 5300 0000 7306 0000 007c 006a 0053 0072  S...s....|.j.S.r
+00001b60: 1c00 0000 a901 da13 636f 6e74 656e 745f  ........content_
+00001b70: 7479 7065 5f63 6174 5f69 6429 01da 0363  type_cat_id)...c
+00001b80: 6174 7224 0000 0072 2400 0000 7225 0000  atr$...r$...r%..
+00001b90: 0072 4100 0000 ef00 0000 7248 0000 0029  .rA.......rH...)
+00001ba0: 01da 0669 645f 5f69 6e72 3200 0000 a901  ...id__inr2.....
+00001bb0: da04 6d61 6e79 6301 0000 0000 0000 0000  ..manyc.........
+00001bc0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00001bd0: 1800 0000 6700 7c00 5d10 7d01 7c01 6400  ....g.|.].}.|.d.
+00001be0: 1900 7304 7c01 9102 7104 5300 2901 721e  ..s.|...q.S.).r.
+00001bf0: 0000 0072 2400 0000 2902 da02 2e30 da04  ...r$...)....0..
+00001c00: 6d65 6e75 7224 0000 0072 2400 0000 7225  menur$...r$...r%
+00001c10: 0000 00da 0a3c 6c69 7374 636f 6d70 3ef9  .....<listcomp>.
+00001c20: 0000 0072 4800 0000 7a23 6765 745f 7065  ...rH...z#get_pe
+00001c30: 726d 6973 7369 6f6e 732e 3c6c 6f63 616c  rmissions.<local
+00001c40: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+00001c50: 0000 0000 0000 0000 0000 0200 0000 0800  ................
+00001c60: 0000 1300 0000 732c 0000 0067 007c 005d  ......s,...g.|.]
+00001c70: 247d 017c 0164 0019 0074 0088 0064 0119  $}.|.d...t...d..
+00001c80: 00a0 0164 0264 03a1 0283 016b 0272 047c  ...d.d.....k.r.|
+00001c90: 0191 0271 0453 0029 0472 1e00 0000 7230  ...q.S.).r....r0
+00001ca0: 0000 00da 016e da00 2902 da03 696e 74da  .....n..)...int.
+00001cb0: 0772 6570 6c61 6365 2902 7290 0000 00da  .replace).r.....
+00001cc0: 0863 6869 6c64 7265 6ea9 01da 066d 656e  .children....men
+00001cd0: 755f 3172 2400 0000 7225 0000 0072 9200  u_1r$...r%...r..
+00001ce0: 0000 fb00 0000 7248 0000 0063 0100 0000  ......rH...c....
+00001cf0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00001d00: 5300 0000 7308 0000 007c 0064 0119 0053  S...s....|.d...S
+00001d10: 00a9 024e 7232 0000 0072 2400 0000 a901  ...Nr2...r$.....
+00001d20: da01 7872 2400 0000 7224 0000 0072 2500  ..xr$...r$...r%.
+00001d30: 0000 7241 0000 00fc 0000 0072 4800 0000  ..rA.......rH...
+00001d40: 2901 da03 6b65 7972 9700 0000 7230 0000  )...keyr....r0..
+00001d50: 0072 9300 0000 7294 0000 0072 8a00 0000  .r....r....r....
+00001d60: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001d70: 0004 0000 0053 0000 0073 1200 0000 7c00  .....S...s....|.
+00001d80: 6a00 7c00 6a01 7c00 6a02 6401 9c03 5300  j.|.j.|.j.d...S.
+00001d90: 723b 0000 0072 3c00 0000 723f 0000 0072  r;...r<...r?...r
+00001da0: 2400 0000 7224 0000 0072 2500 0000 7241  $...r$...r%...rA
+00001db0: 0000 0001 0100 0072 4800 0000 6301 0000  .......rH...c...
+00001dc0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00001dd0: 0053 0000 0073 0800 0000 7c00 6401 1900  .S...s....|.d...
+00001de0: 5300 729a 0000 0072 2400 0000 729b 0000  S.r....r$...r...
+00001df0: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+00001e00: 7241 0000 0003 0100 0072 4800 0000 2911  rA.......rH...).
+00001e10: 724d 0000 0072 4300 0000 720f 0000 0072  rM...rC...r....r
+00001e20: 2e00 0000 722f 0000 0072 0e00 0000 7232  ....r/...r....r2
+00001e30: 0000 0072 2000 0000 724a 0000 0072 2c00  ...r ...rJ...r,.
+00001e40: 0000 da06 736f 7274 6564 7295 0000 0072  ....sortedr....r
+00001e50: 9600 0000 da05 6669 7273 7472 4400 0000  ......firstrD...
+00001e60: 7245 0000 0072 3100 0000 290d 7262 0000  rE...r1...).rb..
+00001e70: 0072 3800 0000 da05 7661 6c75 65da 1063  .r8.....value..c
+00001e80: 6f6e 7465 6e74 5f74 7970 655f 6964 73da  ontent_type_ids.
+00001e90: 0f63 6f6e 7465 6e74 5f74 7970 655f 6578  .content_type_ex
+00001ea0: 5a14 636f 6e74 656e 745f 7479 7065 5f63  Z.content_type_c
+00001eb0: 6174 5f69 6473 5a11 636f 6e74 656e 745f  at_idsZ.content_
+00001ec0: 7479 7065 5f63 6174 73da 0872 656c 5f6c  type_cats..rel_l
+00001ed0: 6973 74da 0372 656c da0f 7365 7269 616c  ist..rel..serial
+00001ee0: 697a 6572 5f72 656c 73da 0861 6c6c 5f6d  izer_rels..all_m
+00001ef0: 656e 7572 8200 0000 da0d 6368 696c 6472  enur......childr
+00001f00: 656e 5f6c 6973 7472 2400 0000 7298 0000  en_listr$...r...
+00001f10: 0072 2500 0000 7280 0000 00ec 0000 0073  .r%...r........s
+00001f20: 3000 0000 0001 1201 1001 1201 1401 0401  0...............
+00001f30: 0801 0c01 0801 0c01 0c01 0602 0e01 0801  ................
+00001f40: 1201 1001 0801 2201 0401 0c01 0a01 0aff  ......".........
+00001f50: 0c02 1001 7280 0000 0063 0100 0000 0000  ....r....c......
+00001f60: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
+00001f70: 0000 7326 0000 0074 006a 01a0 02a1 007d  ..s&...t.j.....}
+00001f80: 0174 037d 0274 047c 027c 0164 0183 037d  .t.}.t.|.|.d...}
+00001f90: 0374 0564 027c 0369 0183 0153 0072 8400  .t.d.|.i...S.r..
+00001fa0: 0000 7285 0000 0072 8600 0000 7224 0000  ..r....r....r$..
+00001fb0: 0072 2400 0000 7225 0000 00da 106d 656e  .r$...r%.....men
+00001fc0: 755f 7065 726d 6973 7369 6f6e 7307 0100  u_permissions...
+00001fd0: 0073 0800 0000 0001 0a01 0401 0c01 72a8  .s............r.
+00001fe0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00001ff0: 0200 0000 0300 0000 4300 0000 732c 0000  ........C...s,..
+00002000: 007c 016a 0072 287c 016a 007c 0076 0172  .|.j.r(|.j.|.v.r
+00002010: 287c 00a0 017c 016a 00a1 0101 0074 027c  (|...|.j.....t.|
+00002020: 007c 016a 0083 0201 007c 0053 0072 1c00  .|.j.....|.S.r..
+00002030: 0000 721d 0000 0029 0272 2200 0000 7223  ..r....).r"...r#
+00002040: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00002050: 0000 7220 0000 000e 0100 0073 0a00 0000  ..r .......s....
+00002060: 0001 0601 0a01 0c01 0c01 7220 0000 0063  ..........r ...c
+00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002080: 0400 0000 4000 0000 7342 0000 0065 005a  ....@...sB...e.Z
+00002090: 0164 005a 0265 036a 0464 0164 0264 038d  .d.Z.e.j.d.d.d..
+000020a0: 025a 0565 036a 0464 0464 0264 038d 025a  .Z.e.j.d.d.d...Z
+000020b0: 0665 036a 0464 0564 068d 015a 0747 0064  .e.j.d.d...Z.G.d
+000020c0: 0764 0884 0064 0883 025a 0864 0953 0029  .d...d...Z.d.S.)
+000020d0: 0ada 0e48 6f73 7069 7461 6c46 696c 7465  ...HospitalFilte
+000020e0: 7272 3d00 0000 da09 6963 6f6e 7461 696e  rr=.....icontain
+000020f0: 73a9 02da 0a66 6965 6c64 5f6e 616d 65da  s....field_name.
+00002100: 0b6c 6f6f 6b75 705f 6578 7072 da07 636f  .lookup_expr..co
+00002110: 6465 6e75 6d72 1e00 0000 a901 72ac 0000  denumr......r...
+00002120: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00002130: 0000 0100 0000 4000 0000 7314 0000 0065  ......@...s....e
+00002140: 005a 0164 005a 0265 035a 0464 015a 0564  .Z.d.Z.e.Z.d.Z.d
+00002150: 0253 0029 037a 1348 6f73 7069 7461 6c46  .S.).z.HospitalF
+00002160: 696c 7465 722e 4d65 7461 2903 723d 0000  ilter.Meta).r=..
+00002170: 0072 ae00 0000 721e 0000 004e 2906 7271  .r....r....N).rq
+00002180: 0000 0072 7200 0000 7273 0000 0072 0400  ...rr...rs...r..
+00002190: 0000 7249 0000 00da 0666 6965 6c64 7372  ..rI.....fieldsr
+000021a0: 2400 0000 7224 0000 0072 2400 0000 7225  $...r$...r$...r%
+000021b0: 0000 00da 044d 6574 611b 0100 0073 0400  .....Meta....s..
+000021c0: 0000 0801 0401 72b1 0000 004e 2909 7271  ......r....N).rq
+000021d0: 0000 0072 7200 0000 7273 0000 00da 0766  ...rr...rs.....f
+000021e0: 696c 7465 7273 da0a 4368 6172 4669 6c74  ilters..CharFilt
+000021f0: 6572 723d 0000 0072 ae00 0000 721e 0000  err=...r....r...
+00002200: 0072 b100 0000 7224 0000 0072 2400 0000  .r....r$...r$...
+00002210: 7224 0000 0072 2500 0000 72a9 0000 0016  r$...r%...r.....
+00002220: 0100 0073 0800 0000 0801 0e01 0e01 0c02  ...s............
+00002230: 72a9 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00002240: 0000 0000 0000 0300 0000 4000 0000 7328  ..........@...s(
+00002250: 0000 0065 005a 0164 005a 0265 036a 046a  ...e.Z.d.Z.e.j.j
+00002260: 0564 0164 028d 01a0 0664 03a1 015a 0765  .d.d.....d...Z.e
+00002270: 085a 0965 0a5a 0b64 0453 0029 05da 0f48  .Z.e.Z.d.S.)...H
+00002280: 6f73 7069 7461 6c56 6965 7753 6574 54a9  ospitalViewSetT.
+00002290: 0172 6400 0000 7230 0000 004e 290c 7271  .rd...r0...N).rq
+000022a0: 0000 0072 7200 0000 7273 0000 0072 0400  ...rr...rs...r..
+000022b0: 0000 722e 0000 0072 2f00 0000 7232 0000  ..r....r/...r2..
+000022c0: 0072 7400 0000 7216 0000 0072 7500 0000  .rt...r....ru...
+000022d0: 72a9 0000 00da 0f66 696c 7465 7273 6574  r......filterset
+000022e0: 5f63 6c61 7373 7224 0000 0072 2400 0000  _classr$...r$...
+000022f0: 7224 0000 0072 2500 0000 72b4 0000 0024  r$...r%...r....$
+00002300: 0100 0073 0600 0000 0801 1401 0401 72b4  ...s..........r.
+00002310: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002320: 0000 0000 0400 0000 4000 0000 735c 0000  ........@...s\..
+00002330: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
+00002340: 0264 038d 025a 0565 036a 0464 0464 0264  .d...Z.e.j.d.d.d
+00002350: 038d 025a 0665 036a 0464 0564 0264 038d  ...Z.e.j.d.d.d..
+00002360: 025a 0765 036a 0464 0664 078d 015a 0865  .Z.e.j.d.d...Z.e
+00002370: 036a 0464 0864 078d 015a 0947 0064 0964  .j.d.d...Z.G.d.d
+00002380: 0a84 0064 0a83 025a 0a64 0b53 0029 0cda  ...d...Z.d.S.)..
+00002390: 0c4f 6666 6963 6546 696c 7465 7272 3d00  .OfficeFilterr=.
+000023a0: 0000 72aa 0000 0072 ab00 0000 72ae 0000  ..r....r....r...
+000023b0: 00da 0b6f 6666 6963 655f 7479 7065 7267  ...office_typerg
+000023c0: 0000 0072 af00 0000 721e 0000 0063 0000  ...r....r....c..
+000023d0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+000023e0: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
+000023f0: 005a 0265 035a 0464 015a 0564 025a 0664  .Z.e.Z.d.Z.d.Z.d
+00002400: 0353 0029 047a 114f 6666 6963 6546 696c  .S.).z.OfficeFil
+00002410: 7465 722e 4d65 7461 721b 0000 0029 0372  ter.Metar....).r
+00002420: 3d00 0000 72ae 0000 0072 b800 0000 4e29  =...r....r....N)
+00002430: 0772 7100 0000 7272 0000 0072 7300 0000  .rq...rr...rs...
+00002440: 7205 0000 0072 4900 0000 72b0 0000 00da  r....rI...r.....
+00002450: 0d73 6561 7263 685f 6669 656c 6473 7224  .search_fieldsr$
+00002460: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00002470: 0000 72b1 0000 0032 0100 0073 0600 0000  ..r....2...s....
+00002480: 0801 0401 0401 72b1 0000 004e 290b 7271  ......r....N).rq
+00002490: 0000 0072 7200 0000 7273 0000 0072 b200  ...rr...rs...r..
+000024a0: 0000 72b3 0000 0072 3d00 0000 72ae 0000  ..r....r=...r...
+000024b0: 0072 b800 0000 7267 0000 0072 1e00 0000  .r....rg...r....
+000024c0: 72b1 0000 0072 2400 0000 7224 0000 0072  r....r$...r$...r
+000024d0: 2400 0000 7225 0000 0072 b700 0000 2b01  $...r%...r....+.
+000024e0: 0000 730c 0000 0008 010e 010e 010e 010c  ..s.............
+000024f0: 010c 0272 b700 0000 6300 0000 0000 0000  ...r....c.......
+00002500: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00002510: 0073 2a00 0000 6500 5a01 6400 5a02 6503  .s*...e.Z.d.Z.e.
+00002520: 6a04 6a05 6401 6402 8d01 5a06 6507 5a08  j.j.d.d...Z.e.Z.
+00002530: 6509 5a0a 6403 6404 8400 5a0b 6405 5300  e.Z.d.d...Z.d.S.
+00002540: 2906 da0d 4f66 6669 6365 5669 6577 5365  )...OfficeViewSe
+00002550: 7454 72b5 0000 0063 0200 0000 0000 0000  tTr....c........
+00002560: 0000 0000 0700 0000 0400 0000 4f00 0000  ............O...
+00002570: 735e 0000 007c 00a0 007c 00a0 01a1 00a1  s^...|...|......
+00002580: 017d 0464 017c 006a 026a 03a0 04a1 0076  .}.d.|.j.j.....v
+00002590: 0072 427c 00a0 057c 04a1 017d 057c 006a  .rB|...|...}.|.j
+000025a0: 067c 0564 0264 038d 027d 067c 00a0 077c  .|.d.d...}.|...|
+000025b0: 066a 08a1 0153 007c 006a 067c 0464 0264  .j...S.|.j.|.d.d
+000025c0: 038d 027d 0674 0964 047c 066a 0869 0183  ...}.t.d.|.j.i..
+000025d0: 0153 0029 054e da04 7061 6765 5472 8e00  .S.).N..pageTr..
+000025e0: 0000 da07 7265 7375 6c74 7329 0ada 0f66  ....results)...f
+000025f0: 696c 7465 725f 7175 6572 7973 6574 da0c  ilter_queryset..
+00002600: 6765 745f 7175 6572 7973 6574 7235 0000  get_querysetr5..
+00002610: 00da 0c71 7565 7279 5f70 6172 616d 73da  ...query_params.
+00002620: 046b 6579 73da 1170 6167 696e 6174 655f  .keys..paginate_
+00002630: 7175 6572 7973 6574 da0e 6765 745f 7365  queryset..get_se
+00002640: 7269 616c 697a 6572 da16 6765 745f 7061  rializer..get_pa
+00002650: 6769 6e61 7465 645f 7265 7370 6f6e 7365  ginated_response
+00002660: 722c 0000 0072 0200 0000 2907 7221 0000  r,...r....).r!..
+00002670: 0072 3500 0000 725e 0000 0072 5f00 0000  .r5...r^...r_...
+00002680: 7274 0000 0072 bb00 0000 7262 0000 0072  rt...r....rb...r
+00002690: 2400 0000 7224 0000 0072 2500 0000 724d  $...r$...r%...rM
+000026a0: 0000 003e 0100 0073 0e00 0000 0001 0e02  ...>...s........
+000026b0: 1001 0a02 0e01 0c02 0e01 7a12 4f66 6669  ..........z.Offi
+000026c0: 6365 5669 6577 5365 742e 6c69 7374 4e29  ceViewSet.listN)
+000026d0: 0c72 7100 0000 7272 0000 0072 7300 0000  .rq...rr...rs...
+000026e0: 7205 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
+000026f0: 7400 0000 7217 0000 0072 7500 0000 72b7  t...r....ru...r.
+00002700: 0000 0072 b600 0000 724d 0000 0072 2400  ...r....rM...r$.
+00002710: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00002720: 0072 ba00 0000 3801 0000 7308 0000 0008  .r....8...s.....
+00002730: 010e 0104 0204 0272 ba00 0000 6300 0000  .......r....c...
+00002740: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00002750: 0040 0000 0073 4400 0000 6500 5a01 6400  .@...sD...e.Z.d.
+00002760: 5a02 6503 6a04 6401 6402 6403 8d02 5a05  Z.e.j.d.d.d...Z.
+00002770: 6503 6a04 6404 6402 6403 8d02 5a06 6503  e.j.d.d.d...Z.e.
+00002780: 6a04 6405 6402 6403 8d02 5a07 4700 6406  j.d.d.d...Z.G.d.
+00002790: 6407 8400 6407 8302 5a08 6408 5300 2909  d...d...Z.d.S.).
+000027a0: da0c 446f 6374 6f72 4669 6c74 6572 723d  ..DoctorFilterr=
+000027b0: 0000 0072 aa00 0000 72ab 0000 00da 0a6a  ...r....r......j
+000027c0: 6f62 5f6e 756d 6265 72da 0570 686f 6e65  ob_number..phone
+000027d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000027e0: 0001 0000 0040 0000 0073 1800 0000 6500  .....@...s....e.
+000027f0: 5a01 6400 5a02 6503 5a04 6401 5a05 6402  Z.d.Z.e.Z.d.Z.d.
+00002800: 5a06 6403 5300 2904 7a11 446f 6374 6f72  Z.d.S.).z.Doctor
+00002810: 4669 6c74 6572 2e4d 6574 6172 1b00 0000  Filter.Metar....
+00002820: 2903 723d 0000 0072 c500 0000 72c6 0000  ).r=...r....r...
+00002830: 004e 2907 7271 0000 0072 7200 0000 7273  .N).rq...rr...rs
+00002840: 0000 0072 0600 0000 7249 0000 0072 b000  ...r....rI...r..
+00002850: 0000 72b9 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
+00002860: 0072 2400 0000 7225 0000 0072 b100 0000  .r$...r%...r....
+00002870: 5001 0000 7306 0000 0008 0104 0104 0172  P...s..........r
+00002880: b100 0000 4e29 0972 7100 0000 7272 0000  ....N).rq...rr..
+00002890: 0072 7300 0000 72b2 0000 0072 b300 0000  .rs...r....r....
+000028a0: 723d 0000 0072 c500 0000 72c6 0000 0072  r=...r....r....r
+000028b0: b100 0000 7224 0000 0072 2400 0000 7224  ....r$...r$...r$
+000028c0: 0000 0072 2500 0000 72c4 0000 004b 0100  ...r%...r....K..
+000028d0: 0073 0800 0000 0801 0e01 0e01 0e02 72c4  .s............r.
+000028e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000028f0: 0000 0000 0300 0000 4000 0000 7332 0000  ........@...s2..
+00002900: 0065 005a 0164 005a 0265 036a 046a 0564  .e.Z.d.Z.e.j.j.d
+00002910: 0164 028d 015a 0665 075a 0865 095a 0a64  .d...Z.e.Z.e.Z.d
+00002920: 0364 0484 005a 0b64 0564 0684 005a 0c64  .d...Z.d.d...Z.d
+00002930: 0753 0029 08da 0d44 6f63 746f 7256 6965  .S.)...DoctorVie
+00002940: 7753 6574 5472 b500 0000 6302 0000 0000  wSetTr....c.....
+00002950: 0000 0000 0000 0008 0000 0005 0000 004f  ...............O
+00002960: 0000 0073 aa00 0000 7c00 a000 7c00 a001  ...s....|...|...
+00002970: a100 a101 7d04 6400 7d05 6401 7c00 6a02  ....}.d.}.d.|.j.
+00002980: 6a03 a004 a100 7600 722c 7c00 a005 7c04  j.....v.r,|...|.
+00002990: a101 7d05 7c05 6400 7501 724e 7c00 6a06  ..}.|.d.u.rN|.j.
+000029a0: 7c05 6402 6403 8d02 7d06 7c00 a007 7c06  |.d.d...}.|...|.
+000029b0: 6a08 a101 5300 6404 7c00 6a02 6a03 a004  j...S.d.|.j.j...
+000029c0: a100 7600 728e 7c00 6a02 6a03 a009 6404  ..v.r.|.j.j...d.
+000029d0: a101 7d07 7c00 6a06 7c04 6402 6404 7c07  ..}.|.j.|.d.d.|.
+000029e0: 6901 6405 8d03 7d06 740a 6406 7c06 6a08  i.d...}.t.d.|.j.
+000029f0: 6901 8301 5300 7c00 6a06 7c04 6402 6403  i...S.|.j.|.d.d.
+00002a00: 8d02 7d06 740a 6406 7c06 6a08 6901 8301  ..}.t.d.|.j.i...
+00002a10: 5300 2907 4e72 bb00 0000 5472 8e00 0000  S.).Nr....Tr....
+00002a20: da08 6665 655f 7479 7065 2902 728f 0000  ..fee_type).r...
+00002a30: 00da 0763 6f6e 7465 7874 72bc 0000 0029  ...contextr....)
+00002a40: 0b72 bd00 0000 72be 0000 0072 3500 0000  .r....r....r5...
+00002a50: 72bf 0000 0072 c000 0000 72c1 0000 0072  r....r....r....r
+00002a60: c200 0000 72c3 0000 0072 2c00 0000 726c  ....r....r,...rl
+00002a70: 0000 0072 0200 0000 2908 7221 0000 0072  ...r....).r!...r
+00002a80: 3500 0000 725e 0000 0072 5f00 0000 7274  5...r^...r_...rt
+00002a90: 0000 0072 bb00 0000 7262 0000 0072 c800  ...r....rb...r..
+00002aa0: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00002ab0: 0072 4d00 0000 5b01 0000 731a 0000 0000  .rM...[...s.....
+00002ac0: 010e 0104 0110 010a 0108 010e 010c 0110  ................
+00002ad0: 010e 0114 010e 020e 017a 1244 6f63 746f  .........z.Docto
+00002ae0: 7256 6965 7753 6574 2e6c 6973 7463 0200  rViewSet.listc..
+00002af0: 0000 0000 0000 0000 0000 0700 0000 0400  ................
+00002b00: 0000 4f00 0000 7356 0000 007c 00a0 00a1  ..O...sV...|....
+00002b10: 007d 0464 017c 006a 016a 02a0 03a1 0076  .}.d.|.j.j.....v
+00002b20: 0072 427c 006a 016a 02a0 0464 01a1 017d  .rB|.j.j...d...}
+00002b30: 057c 006a 057c 0464 017c 0569 0164 028d  .|.j.|.d.|.i.d..
+00002b40: 027d 0674 067c 066a 0783 0153 007c 00a0  .}.t.|.j...S.|..
+00002b50: 057c 04a1 017d 0674 067c 066a 0783 0153  .|...}.t.|.j...S
+00002b60: 0029 034e 72c8 0000 0029 0172 c900 0000  .).Nr....).r....
+00002b70: 2908 722d 0000 0072 3500 0000 72bf 0000  ).r-...r5...r...
+00002b80: 0072 c000 0000 726c 0000 0072 c200 0000  .r....rl...r....
+00002b90: 7202 0000 0072 2c00 0000 2907 7221 0000  r....r,...).r!..
+00002ba0: 0072 3500 0000 725e 0000 0072 5f00 0000  .r5...r^...r_...
+00002bb0: da08 696e 7374 616e 6365 72c8 0000 0072  ..instancer....r
+00002bc0: 6200 0000 7224 0000 0072 2400 0000 7225  b...r$...r$...r%
+00002bd0: 0000 00da 0872 6574 7269 6576 656b 0100  .....retrievek..
+00002be0: 0073 0e00 0000 0001 0801 1001 0e01 1201  .s..............
+00002bf0: 0a01 0a01 7a16 446f 6374 6f72 5669 6577  ....z.DoctorView
+00002c00: 5365 742e 7265 7472 6965 7665 4e29 0d72  Set.retrieveN).r
+00002c10: 7100 0000 7272 0000 0072 7300 0000 7206  q...rr...rs...r.
+00002c20: 0000 0072 2e00 0000 722f 0000 0072 7400  ...r....r/...rt.
+00002c30: 0000 7218 0000 0072 7500 0000 72c4 0000  ..r....ru...r...
+00002c40: 0072 b600 0000 724d 0000 0072 cb00 0000  .r....rM...r....
+00002c50: 7224 0000 0072 2400 0000 7224 0000 0072  r$...r$...r$...r
+00002c60: 2500 0000 72c7 0000 0056 0100 0073 0a00  %...r....V...s..
+00002c70: 0000 0801 0e01 0401 0402 0810 72c7 0000  ............r...
+00002c80: 0029 3672 5600 0000 da17 7265 7374 5f66  .)6rV.....rest_f
+00002c90: 7261 6d65 776f 726b 2e72 6573 706f 6e73  ramework.respons
+00002ca0: 6572 0200 0000 da17 7265 7374 5f66 7261  er......rest_fra
+00002cb0: 6d65 776f 726b 2e76 6965 7773 6574 7372  mework.viewsetsr
+00002cc0: 0300 0000 da0e 646a 616e 676f 5f66 696c  ......django_fil
+00002cd0: 7465 7273 72b2 0000 00da 1262 6173 655f  tersr......base_
+00002ce0: 7379 7374 656d 2e6d 6f64 656c 7372 0400  system.modelsr..
+00002cf0: 0000 7205 0000 0072 0600 0000 da1a 646a  ..r....r......dj
+00002d00: 616e 676f 2e63 6f6e 7472 6962 2e61 7574  ango.contrib.aut
+00002d10: 682e 6d6f 6465 6c73 7207 0000 0072 0800  h.modelsr....r..
+00002d20: 0000 da0b 646a 616e 676f 2e68 7474 7072  ....django.httpr
+00002d30: 0900 0000 da19 7265 7374 5f66 7261 6d65  ......rest_frame
+00002d40: 776f 726b 2e65 7863 6570 7469 6f6e 7372  work.exceptionsr
+00002d50: 0a00 0000 da19 7265 7374 5f66 7261 6d65  ......rest_frame
+00002d60: 776f 726b 2e64 6563 6f72 6174 6f72 7372  work.decoratorsr
+00002d70: 0b00 0000 da0e 7265 7374 5f66 7261 6d65  ......rest_frame
+00002d80: 776f 726b 720c 0000 0072 0d00 0000 720e  workr....r....r.
+00002d90: 0000 0072 0f00 0000 7210 0000 00da 1762  ...r....r......b
+00002da0: 6173 655f 7379 7374 656d 2e73 6572 6961  ase_system.seria
+00002db0: 6c69 7a65 7273 7211 0000 0072 1200 0000  lizersr....r....
+00002dc0: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00002dd0: 1600 0000 7217 0000 0072 1800 0000 da09  ....r....r......
+00002de0: 646a 616e 676f 2e64 6272 1900 0000 721a  django.dbr....r.
+00002df0: 0000 0072 7800 0000 7279 0000 0072 7b00  ...rx...ry...r{.
+00002e00: 0000 7283 0000 0072 8700 0000 7288 0000  ..r....r....r...
+00002e10: 0072 8000 0000 72a8 0000 0072 2000 0000  .r....r....r ...
+00002e20: da09 4669 6c74 6572 5365 7472 a900 0000  ..FilterSetr....
+00002e30: 72b4 0000 0072 b700 0000 72ba 0000 0072  r....r....r....r
+00002e40: c400 0000 72c7 0000 0072 2400 0000 7224  ....r....r$...r$
+00002e50: 0000 0072 2400 0000 7225 0000 00da 083c  ...r$...r%.....<
+00002e60: 6d6f 6475 6c65 3e01 0000 0073 3a00 0000  module>....s:...
+00002e70: 0802 0c01 0c01 0801 1403 1001 0c01 0c01  ................
+00002e80: 0c01 0c02 1c01 2802 0c03 107f 0029 1006  ......(......)..
+00002e90: 1007 1006 080e 0807 1007 081b 0807 0808  ................
+00002ea0: 120e 1007 120d 1013 120b                 ..........
```

### Comparing `base_system-0.2.2/base_system/auth.py` & `base_system-0.2.3/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/migrations/0001_initial.py` & `base_system-0.2.3/base_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/migrations/0003_alter_extragroup_hospital.py` & `base_system-0.2.3/base_system/migrations/0003_alter_extragroup_hospital.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc` & `base_system-0.2.3/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc` & `base_system-0.2.3/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc` & `base_system-0.2.3/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/models.py` & `base_system-0.2.3/base_system/models.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system/serializers.py` & `base_system-0.2.3/base_system/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.conf import settings
 from django.contrib.auth.models import Permission
 from django.contrib.contenttypes.models import ContentType
 from rest_framework import serializers
 from base_system.models import Hospital, Office, Doctor, PositionTitle, User, ExtraGroup, InspectionDictionaries, \
     ExaminationDictionaries, DrugDirectory, DrugCategory, DrugPreparationType, PharmacyManagement, ApiInfo, \
-    PharmacyDrug, ContentTypeCates, ContentTypeEx, ExpenseStandard
+    PharmacyDrug, ContentTypeCates, ContentTypeEx, ExpenseStandard, ExaminationType, InspectionType
 from django.contrib.auth.models import Group
 from functools import reduce
 
 
 class ExtraGroupSerializer(serializers.ModelSerializer):
     """
     角色扩充序列化
@@ -477,14 +477,29 @@
 
     def get_extra_group(self, obj):
         group = obj.group
         if group:
             return obj.group.name
 
 
+class InspectionTypeSerializer(serializers.ModelSerializer):
+    """检查字典类型序列化器"""
+
+    children = serializers.SerializerMethodField()
+
+    class Meta:
+        model = InspectionType
+        fields = "__all__"
+
+    def get_children(self, obj):
+        children = InspectionType.objects.filter(parent=obj)
+        serializer = InspectionTypeSerializer(children, many=True)
+        return serializer.data
+
+
 class InspectionDictionariesSerializer(serializers.ModelSerializer):
     """检查字典序列化器"""
     hospital_name = serializers.SerializerMethodField()
     office_name = serializers.SerializerMethodField()
 
     class Meta:
         model = InspectionDictionaries
@@ -526,14 +541,28 @@
 
     def get_office_name(self, obj):
         office = Office.objects.filter(codenum=obj.office_code).first()
         if office:
             return office.name
 
 
+class ExaminationTypeSerializer(serializers.ModelSerializer):
+    """检验字典类型序列化器"""
+    children = serializers.SerializerMethodField()
+
+    class Meta:
+        model = ExaminationType
+        fields = "__all__"
+
+    def get_children(self, obj):
+        children = ExaminationType.objects.filter(parent=obj)
+        serializer = ExaminationTypeSerializer(children, many=True)
+        return serializer.data
+
+
 class ExaminationDictionariesSerializer(serializers.ModelSerializer):
     """检验字典序列化器"""
     hospital_name = serializers.SerializerMethodField()
     office_name = serializers.SerializerMethodField()
 
     class Meta:
         model = ExaminationDictionaries
```

### Comparing `base_system-0.2.2/base_system/urls.py` & `base_system-0.2.3/base_system/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 from django.contrib import admin
 from django.urls import path, include
 from rest_framework import routers
 
 from . import views
 from base_system.views import PermissionsView
-from base_system import viewsets
+from base_system import viewsets, export_viewset
 from rest_framework_jwt.views import obtain_jwt_token
 from rest_framework_jwt.views import refresh_jwt_token
 from rest_framework_jwt.views import verify_jwt_token
 
 urlpatterns = [
     # path('login/',views.login),
     path('register/', views.register),
@@ -41,30 +41,33 @@
     path('import_exa_dic/', views.import_examination_dictionaries),  # 导入检验字典excel表数据
     path('import_drug_dir/', views.import_drug_directory),  # 导入药品目录excel表数据
     path('import_pharmacy_drug/', views.import_pharmacy_drug),  # 导入药房药品excel表数据
     path('menu_permissions/', viewsets.menu_permissions),
 
 ]
 router = routers.DefaultRouter()
-router.register(r'export_hospital', views.HospitalInfoExportViewSet)  # 医院信息导出接口
-router.register(r'export_office', views.OfficeInfoExportViewSet)  # 科室信息导出接口
-router.register(r'export_group', views.GroupExportViewSet)  # 角色信息导出接口
-router.register(r'export_doctor', views.DoctorInfoExportViewSet)  # 医生信息导出接口
-router.register(r'export_user', views.UserInfoExportViewSet)  # 用户信息导出接口
+
+router.register(r'hospitals', viewsets.HospitalViewSet)
+router.register(r'offices', viewsets.OfficeViewSet)
+router.register(r'doctors', viewsets.DoctorViewSet)
 router.register(r'groups', viewsets.GroupViewSet)  # 角色
 router.register(r'users', views.UserViewSet)  # 用户信息
+router.register(r'apinfos', views.ApiInfoViewSet)  # 接口信息
+
+router.register(r'inspectiontypes', views.InspectionTypeViewSet)
 router.register(r'ins_dic', views.InspectionDictionariesViewSet)  # 检查字典
-router.register(r'export_ins_dic', views.InspectionDictionariesInfoExportViewSet)  # 导出检查字典
+router.register(r'examinationtypes', views.ExaminationTypeViewSet)
 router.register(r'exa_dic', views.ExaminationDictionariesViewSet)  # 检验字典
-router.register(r'export_exa_dic', views.ExaminationDictionariesInfoExportViewSet)  # 导出检验字典
-router.register(r'export_drug_directory', views.DrugDirectoryExportViewSet)  # 导出药品目录
-router.register(r'export_pharmacy_drug', views.PharmacyDrugExportViewSet)  # 导出药房药品目录
 router.register(r'pharmacy_management', views.PharmacyManagementViewSet)  # 药房管理
 router.register(r'drug_directories', views.DrugDirectoryViewSet)  # 药品目录
-router.register(r'apinfos', views.ApiInfoViewSet)  # 接口信息
 
-# 预约相关
-router.register(r'hospitals', viewsets.HospitalViewSet)
-router.register(r'offices', viewsets.OfficeViewSet)
-router.register(r'doctors', viewsets.DoctorViewSet)
+router.register(r'export_hospital', export_viewset.HospitalInfoExportViewSet)  # 医院信息导出接口
+router.register(r'export_office', export_viewset.OfficeInfoExportViewSet)  # 科室信息导出接口
+router.register(r'export_group', export_viewset.GroupExportViewSet)  # 角色信息导出接口
+router.register(r'export_doctor', export_viewset.DoctorInfoExportViewSet)  # 医生信息导出接口
+router.register(r'export_user', export_viewset.UserInfoExportViewSet)  # 用户信息导出接口
+router.register(r'export_ins_dic', export_viewset.InspectionDictionariesInfoExportViewSet)  # 导出检查字典
+router.register(r'export_exa_dic', export_viewset.ExaminationDictionariesInfoExportViewSet)  # 导出检验字典
+router.register(r'export_drug_directory', export_viewset.DrugDirectoryExportViewSet)  # 导出药品目录
+router.register(r'export_pharmacy_drug', export_viewset.PharmacyDrugExportViewSet)  # 导出药房药品目录
 
 urlpatterns += router.urls
```

### Comparing `base_system-0.2.2/base_system/views.py` & `base_system-0.2.3/base_system/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 import requests
 import xlrd2
 
 import pyDes
 from django.contrib.auth.backends import ModelBackend
 from django.contrib.auth.hashers import make_password
 from django.contrib.auth.models import Permission
+from django.db import transaction
 from django.http import JsonResponse, HttpResponse
 import django_filters as filters
 from drf_excel.mixins import XLSXFileMixin
 from drf_excel.renderers import XLSXRenderer
 from rest_framework import status
 from rest_framework.decorators import action
 from rest_framework.generics import ListAPIView
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.viewsets import ReadOnlyModelViewSet, ModelViewSet
 
 from base_system.models import Hospital, Office, Doctor, PositionTitle, User, ExtraGroup, InspectionDictionaries, \
     ExaminationDictionaries, DrugDirectory, PharmacyManagement, ExpenseStandard, ApiInfo, \
-    DrugPreparationType, DrugType, DrugCategory, PharmacyDrug
-from base_system.serializers import ExportHospitalSerializer, ExportOfficeSerializer, UserSerializer, \
+    DrugPreparationType, DrugType, DrugCategory, PharmacyDrug, InspectionType, ExaminationType
+from base_system.serializers import UserSerializer, \
     PasswordSerializer, InspectionDictionariesSerializer, ExaminationDictionariesSerializer, \
-    ExportInspectionDictionariesSerializer, ExportExaminationDictionariesSerializer, ExportDrugDirectorySerializer, \
-    PharmacyManagementSerializer, ExportDoctorSerializer, ExportUserSerializer, DrugDirectorySerializer, \
-    ApiInfoSerializer, ExportPharmacyDrugSerializer
-from base_system.serializers import PermissionSerializer, ExportGroupSerializer
+    PharmacyManagementSerializer, DrugDirectorySerializer, \
+    ApiInfoSerializer, InspectionTypeSerializer, ExaminationTypeSerializer
+from base_system.serializers import PermissionSerializer
 from django.conf import settings as django_settings
 
 
 import xlrd as xlrd
 from xlrd import xldate_as_tuple
 import re
 import pinyin
@@ -155,251 +155,15 @@
         :return:
         """
         x = base64.standard_b64decode(text.encode())
         x = self.cryptor.decrypt(x)
         return x.decode()
 
 
-column_header = {
-    'height': 25,
-    'style': {
-        'fill': {
-            'fill_type': 'solid',
-            'start_color': 'FFCCFFCC',
-        },
-        'alignment': {
-            'horizontal': 'center',
-            'vertical': 'center',
-            'wrapText': True,
-            'shrink_to_fit': True,
-        },
-        'border_side': {
-            'border_style': 'thin',
-            'color': 'FF000000',
-        },
-        'font': {
-            'name': 'Arial',
-            'size': 14,
-            'bold': True,
-            'color': 'FF000000',
-        },
-    },
-}
-
-body = {
-    'style': {
-        'fill': {
-            'fill_type': 'solid',
-            'start_color': 'FFCCFFCC',
-        },
-        'alignment': {
-            'horizontal': 'center',
-            'vertical': 'center',
-            'wrapText': True,
-            'shrink_to_fit': True,
-        },
-        'border_side': {
-            'border_style': 'thin',
-            'color': 'FF000000',
-        },
-        'font': {
-            'name': 'Arial',
-            'size': 14,
-            'bold': False,
-            'color': 'FF000000',
-        }
-    },
-    'height': 40,
-}
-
-
-class HospitalInfoFilter(filters.FilterSet):
-    name = filters.CharFilter(field_name="name", lookup_expr='icontains')
-    codenum = filters.CharFilter(field_name="codenum", lookup_expr='icontains')
-    parent = filters.CharFilter(field_name="parent")
-
-    class Meta:
-        model = Hospital
-        fields = "__all__"
-
-        # fields = (
-        #     "name",
-        #     "codenum",
-        #     "parent",
-        # )
-
-
-class HospitalInfoExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-    pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = Hospital.objects.all()
-    serializer_class = ExportHospitalSerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'hospital_export.xlsx'
-    filterset_class = HospitalInfoFilter
-    # filterset_fields = {"name": ["exact", "iexact", "contains", "icontains"], "is_active": ["exact", "in"]}
-
-    header = {
-        'tab_title': "医院信息",
-        'header_title': "医院信息",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
-
-
-class OfficeInfoFilter(filters.FilterSet):
-    name = filters.CharFilter(field_name="name", lookup_expr='icontains')
-    hospital = filters.CharFilter(field_name="hospital", lookup_expr='icontains')
-
-    class Meta:
-        model = Office
-        fields = "__all__"
-
-        # fields = (
-        #     "name",
-        #     "hospital",
-        # )
-
-
-class OfficeInfoExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-    pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = Office.objects.all()
-    serializer_class = ExportOfficeSerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'office_export.xlsx'
-    filterset_class = OfficeInfoFilter
-
-    header = {
-        'tab_title': "科室信息",
-        'header_title': "科室信息",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
-
-
-class DoctorInfoFilter(filters.FilterSet):
-    name = filters.CharFilter(field_name="name", lookup_expr='icontains')
-    hospital = filters.CharFilter(field_name="hospital", lookup_expr='icontains')
-
-    class Meta:
-        model = Doctor
-        fields = "__all__"
-        # fields = (
-        #     "name",
-        #     "hospital",
-        # )
-
-
-class DoctorInfoExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-    """医生信息导出接口"""
-    pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = Doctor.objects.all()
-    serializer_class = ExportDoctorSerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'doctor_export.xlsx'
-    # filterset_fields = {"name": ["exact", "iexact", "contains", "icontains"], "is_active": ["exact", "in"]}
-    filterset_class = DoctorInfoFilter
-
-    header = {
-        'tab_title': "医生信息",
-        'header_title': "医生信息",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
-
-
-import xlrd
-
-
+@transaction.atomic
 def import_position_title(request):
     """导入excel表数据"""
     created_user = request.POST.get('created_user')
     excel_file = request.FILES.get('excel_file', '')  # 获取前端上传的文件
     file_type = excel_file.name.split('.')[1].split('"')[0]  # 拿到文件后缀
     # file_type = excel_file.name.split('.')[1]  # 拿到文件后缀
     data_list = []
@@ -467,15 +231,15 @@
 
     class Meta:
         model = User
         fields = "__all__"
 
 
 class UserViewSet(ModelViewSet):
-    queryset = User.objects.all().order_by('id')
+    queryset = User.objects.all().order_by('-id')
     serializer_class = UserSerializer
     filterset_class = UserFilter
     filter_fields = "__all__"
 
     @action(methods=["PUT"], detail=True)
     def change_password(self, request, pk):
         # 更改密码
@@ -488,57 +252,19 @@
         user.error_times = 0
         user.is_change_pwd = False
         user.save()
 
         return Response(data={"message": "修改成功"}, status=status.HTTP_205_RESET_CONTENT)
 
 
-class GroupExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
+class InspectionTypeViewSet(ModelViewSet):
+    """检查字典"""
+    queryset = InspectionType.objects.filter(parent=None)
+    serializer_class = InspectionTypeSerializer
     pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = ExtraGroup.objects.all()
-    serializer_class = ExportGroupSerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'group_export.xlsx'
-    # filterset_fields = {"name": ["exact", "iexact", "contains", "icontains"], "is_active": ["exact", "in"]}
-
-    header = {
-        'tab_title': "角色信息",
-        'header_title': "角色信息",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
 
 
 class InspectionDictFilter(filters.FilterSet):
     project_code = filters.CharFilter(field_name="project_code", lookup_expr="icontains")
     project_name = filters.CharFilter(field_name="project_name", lookup_expr="icontains")
     hospital_code = filters.CharFilter(field_name="hospital_code", lookup_expr="icontains")
     office_code = filters.CharFilter(field_name="office_code", lookup_expr="icontains")
@@ -547,15 +273,15 @@
     class Meta:
         model = InspectionDictionaries
         fields = "__all__"
 
 
 class InspectionDictionariesViewSet(ModelViewSet):
     """检查字典"""
-    queryset = InspectionDictionaries.objects.all().order_by('id')
+    queryset = InspectionDictionaries.objects.all().order_by('-id')
     serializer_class = InspectionDictionariesSerializer
     # filter_fields = "__all__"
     filterset_class = InspectionDictFilter
 
     # 导入json文件数据
     # def create(self, request, *args, **kwargs):
     #     with open('spdic.json', encoding='utf-8') as a:
@@ -571,58 +297,19 @@
     #                 project_fees=res['price'],
     #                 code_srvtp=res['code_srvtp'],
     #                 name_srvtp=res['name_srvtp'],
     #             )
     #     return Response({"data": data})
 
 
-class InspectionDictionariesInfoExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-    """导出检查字典"""
+class ExaminationTypeViewSet(ModelViewSet):
+    """检查字典"""
+    queryset = ExaminationType.objects.filter(parent=None)
+    serializer_class = ExaminationTypeSerializer
     pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = InspectionDictionaries.objects.all()
-    serializer_class = ExportInspectionDictionariesSerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'InspectionDictionaries_export.xlsx'
-    filterset_fields = {"project_name": ["exact", "iexact", "contains", "icontains"], "is_active": ["exact", "in"]}
-
-    header = {
-        'tab_title': "检查字典",
-        'header_title': "检查字典",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
 
 
 class ExaminationDictFilter(filters.FilterSet):
     project_code = filters.CharFilter(field_name="project_code", lookup_expr="icontains")
     project_name = filters.CharFilter(field_name="project_name", lookup_expr="icontains")
     hospital_code = filters.CharFilter(field_name="hospital_code", lookup_expr="icontains")
     office_code = filters.CharFilter(field_name="office_code", lookup_expr="icontains")
@@ -631,15 +318,15 @@
     class Meta:
         model = ExaminationDictionaries
         fields = "__all__"
 
 
 class ExaminationDictionariesViewSet(ModelViewSet):
     """检验字典"""
-    queryset = ExaminationDictionaries.objects.all().order_by('id')
+    queryset = ExaminationDictionaries.objects.all().order_by('-id')
     serializer_class = ExaminationDictionariesSerializer
     # filter_fields = "__all__"
     filterset_class = ExaminationDictFilter
 
     # 导入json文件数据
     # def create(self, request, *args, **kwargs):
     #     with open('response.json', encoding='utf-8') as a:
@@ -657,113 +344,22 @@
     #                     project_fees=res.get('price'),
     #                     code_srvtp=res['code_srvtp'],
     #                     name_srvtp=res['name_srvtp'],
     #                 )
     #     return Response({"data": data})
 
 
-class ExaminationDictionariesInfoExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-    """导出检验字典"""
-    pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = ExaminationDictionaries.objects.all()
-    serializer_class = ExportExaminationDictionariesSerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'ExaminationDictionaries_export.xlsx'
-    filterset_fields = {"project_name": ["exact", "iexact", "contains", "icontains"], "is_active": ["exact", "in"]}
-
-    header = {
-        'tab_title': "检验字典",
-        'header_title': "检验字典",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
-
-
-class DrugDirectoryExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-    """导出药品目录"""
-    pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = DrugDirectory.objects.all()
-    serializer_class = ExportDrugDirectorySerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'drug_directory.xlsx'
-    filterset_fields = {"drug_name": ["exact", "iexact", "contains", "icontains"], "is_active": ["exact", "in"]}
-
-    header = {
-        'tab_title': "药品目录",
-        'header_title': "药品目录",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
-
-
 class PharmacyManagementViewSet(ModelViewSet):
     """药房管理"""
-    queryset = PharmacyManagement.objects.all().order_by('id')
+    queryset = PharmacyManagement.objects.all().order_by('-id')
     serializer_class = PharmacyManagementSerializer
     filter_fields = "__all__"
 
 
+@transaction.atomic
 def import_office(request):
     """导入excel表科室数据"""
     created_user = request.POST.get('created_user')
     excel_file = request.FILES.get('excel_file', '')  # 获取前端上传的文件
     file_type = excel_file.name.split('.')[1].split('"')[0]  # 拿到文件后缀
     # file_type = excel_file.name.split('.')[1]  # 拿到文件后缀
     data_list = []
@@ -837,14 +433,15 @@
     if data_list:
         res = {"data": data_list}
     else:
         res = {"data": "文件内容格式有误，请检查内容格式是否正确！"}
     return JsonResponse(res)
 
 
+@transaction.atomic
 def import_doctor(request):
     """导入excel表医生数据"""
     created_user = request.POST.get('created_user')
     excel_file = request.FILES.get('excel_file', '')  # 获取前端上传的文件
     file_type = excel_file.name.split('.')[1].split('"')[0]  # 拿到文件后缀
     # file_type = excel_file.name.split('.')[1]  # 拿到文件后缀
     data_list = []
@@ -896,15 +493,15 @@
                                     "name": name,
                                     "hospital": hospital_name,
                                     "office_name": office_name,
                                     "doc_rank_name": None,
                                     "is_online_consult": None,
                                     "created_time": None,
                                     "created_by": created_user,
-                                    "msg": "该条记录医院查询有误，请检查！！！已自动跳过该条记录的导入",
+                                    "msg": "该条记录医院下的科室查询有误，请检查！！！已自动跳过该条记录的导入",
                                 }
                                 data_list.append(excel_data)
                                 continue
                         gender = row_values[4]
                         if gender:
                             if gender == '男':
                                 gender_vlue = '1'
@@ -987,52 +584,51 @@
                                 "gender": gender_vlue,
                                 "phone": phone_int,
                                 "idcardnum": idnum_int,
                                 # "created_time": datetime.datetime.now(),
                                 # "updated_time": datetime.datetime.now(),
                                 "created_by": created_user,
                             })
-
-                            Initial_hospital = get_pinyin_initials(hospital_name)  # 医院首字母
-                            Initial_doc_rank = get_pinyin_initials(doc_rank_name)  # 职称首字母
-                            combination_hd1 = f'1_{Initial_hospital}_{Initial_doc_rank}'  # '1_WYRMYY_FZRYS'
-                            es_1 = ExpenseStandard.objects.filter(standard_code=combination_hd1,
-                                                                  hospital_id=hospital_id).first()
-                            combination_hd2 = f'2_{Initial_hospital}_{Initial_doc_rank}'
-                            es_2 = ExpenseStandard.objects.filter(standard_code=combination_hd2,
-                                                                  hospital_id=hospital_id).first()
-                            combination_hd3 = f'3_{Initial_hospital}_{Initial_doc_rank}'
-                            es_3 = ExpenseStandard.objects.filter(standard_code=combination_hd3,
-                                                                  hospital_id=hospital_id).first()
-                            combination_hd4 = f'4_{Initial_hospital}_{Initial_doc_rank}'
-                            es_4 = ExpenseStandard.objects.filter(standard_code=combination_hd4,
-                                                                  hospital_id=hospital_id).first()
-                            if es_1 or es_2 or es_3 or es_4:  # 四个标准中至少存在一条存在，否则跳过为其增加费用标准
-                                es_list = []
-                                es_list.append(es_1)
-                                es_list.append(es_2)
-                                es_list.append(es_3)
-                                es_list.append(es_4)
-                                for es in es_list:
-                                    es.doctors.add(doctor1)
-                            else:
-                                excel_data = {
-                                    "job_number": job_number,
-                                    "name": name,
-                                    "hospital": hospital_name,
-                                    "office_name": office_name,
-                                    "doc_rank_name": doc_rank_name,
-                                    "is_online_consult": is_online_consult,
-                                    "created_time": datetime.datetime.now(),
-                                    "created_by": created_user,
-                                    "msg": "成功！但是费用标准查询出错！！！请手动为该医生添加费用标准！！！",
-                                }
-                                data_list.append(excel_data)
-                                continue
-
+                            if is_true:  # 仅在允许互联网接诊时调用以下逻辑
+                                Initial_hospital = get_pinyin_initials(hospital_name)  # 医院首字母
+                                Initial_doc_rank = get_pinyin_initials(doc_rank_name)  # 职称首字母
+                                combination_hd1 = f'1_{Initial_hospital}_{Initial_doc_rank}'  # '1_WYRMYY_FZRYS'
+                                es_1 = ExpenseStandard.objects.filter(standard_code=combination_hd1,
+                                                                      hospital_id=hospital_id).first()
+                                combination_hd2 = f'2_{Initial_hospital}_{Initial_doc_rank}'
+                                es_2 = ExpenseStandard.objects.filter(standard_code=combination_hd2,
+                                                                      hospital_id=hospital_id).first()
+                                combination_hd3 = f'3_{Initial_hospital}_{Initial_doc_rank}'
+                                es_3 = ExpenseStandard.objects.filter(standard_code=combination_hd3,
+                                                                      hospital_id=hospital_id).first()
+                                combination_hd4 = f'4_{Initial_hospital}_{Initial_doc_rank}'
+                                es_4 = ExpenseStandard.objects.filter(standard_code=combination_hd4,
+                                                                      hospital_id=hospital_id).first()
+                                if es_1 or es_2 or es_3 or es_4:  # 四个标准中至少存在一条存在，否则跳过为其增加费用标准
+                                    es_list = []
+                                    es_list.append(es_1)
+                                    es_list.append(es_2)
+                                    es_list.append(es_3)
+                                    es_list.append(es_4)
+                                    for es in es_list:
+                                        es.doctors.add(doctor1)
+                                else:
+                                    excel_data = {
+                                        "job_number": job_number,
+                                        "name": name,
+                                        "hospital": hospital_name,
+                                        "office_name": office_name,
+                                        "doc_rank_name": doc_rank_name,
+                                        "is_online_consult": is_online_consult,
+                                        "created_time": datetime.datetime.now(),
+                                        "created_by": created_user,
+                                        "msg": "成功！但是费用标准查询出错！！！请手动为该医生添加费用标准！！！",
+                                    }
+                                    data_list.append(excel_data)
+                                    continue
                         excel_data = {
                             "job_number": job_number,
                             "name": name,
                             "hospital": hospital_name,
                             "office_name": office_name,
                             "doc_rank_name": doc_rank_name,
                             "is_online_consult": is_online_consult,
@@ -1060,60 +656,14 @@
 #
 # # 示例
 # name = "张三"
 # initials = get_pinyin_initials(name)
 # print(initials)  # "ZS"
 
 
-class UserInfoExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-    """用户信息导出接口"""
-    pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = User.objects.all()
-    serializer_class = ExportUserSerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'user_export.xlsx'
-    # filterset_fields = {"name": ["exact", "iexact", "contains", "icontains"], "is_active": ["exact", "in"]}
-    filterset_fields = "__all__"
-    header = {
-        'tab_title': "用户信息",
-        'header_title': "用户信息",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
-
-
 class DrugDirectoryFilter(filters.FilterSet):
     drug_code = filters.CharFilter(field_name="drug_code", lookup_expr="icontains")
     drug_name = filters.CharFilter(field_name="drug_name", lookup_expr="icontains")
     specification = filters.CharFilter(field_name="standards", lookup_expr="icontains")
     measure_unit = filters.CharFilter(field_name="measure_unit", lookup_expr="icontains")
     preparation_type = filters.CharFilter(field_name="preparation_type__name", lookup_expr="icontains")
     category = filters.CharFilter(field_name="category__name", lookup_expr="icontains")
@@ -1142,15 +692,15 @@
         if symbol in keyword:
             return True
     else:
         return False
 
 
 class DrugDirectoryViewSet(ModelViewSet):
-    queryset = DrugDirectory.objects.all()
+    queryset = DrugDirectory.objects.all().order_by('-id')
     serializer_class = DrugDirectorySerializer
     filterset_class = DrugDirectoryFilter
 
     def list(self, request, *args, **kwargs):
         hospital_code = self.request.query_params.get('hospital_code')
         drug_name = self.request.query_params.get('drug_name')
         page = self.request.query_params.get('page')
@@ -1188,18 +738,19 @@
                 return self.get_paginated_response(serializer.data)
 
             serializer = self.get_serializer(queryset, many=True)
             return Response(serializer.data)
 
 
 class ApiInfoViewSet(ModelViewSet):
-    queryset = ApiInfo.objects.all()
+    queryset = ApiInfo.objects.all().order_by('-id')
     serializer_class = ApiInfoSerializer
 
 
+@transaction.atomic
 def import_inspection_dictionaries(request):
     """导入检查字典excel表数据"""
     created_user = request.POST.get('created_user')
     excel_file = request.FILES.get('excel_file', '')  # 获取前端上传的文件
     file_type = excel_file.name.split('.')[1].split('"')[0]  # 拿到文件后缀
     # file_type = excel_file.name.split('.')[1]  # 拿到文件后缀
     data_list = []
@@ -1267,14 +818,15 @@
     if data_list:
         res = {"data": data_list}
     else:
         res = {"data": "文件内容格式有误，请检查内容格式是否正确！"}
     return JsonResponse(res)
 
 
+@transaction.atomic
 def import_examination_dictionaries(request):
     """导入检验字典excel表数据"""
     created_user = request.POST.get('created_user')
     excel_file = request.FILES.get('excel_file', '')  # 获取前端上传的文件
     file_type = excel_file.name.split('.')[1].split('"')[0]  # 拿到文件后缀
     # file_type = excel_file.name.split('.')[1]  # 拿到文件后缀
     data_list = []
@@ -1342,14 +894,15 @@
     if data_list:
         res = {"data": data_list}
     else:
         res = {"data": "文件内容格式有误，请检查内容格式是否正确！"}
     return JsonResponse(res)
 
 
+@transaction.atomic
 def import_drug_directory(request):
     """导入药品目录excel表数据"""
     created_user = request.POST.get('created_user')
     excel_file = request.FILES.get('excel_file', '')  # 获取前端上传的文件
     file_type = excel_file.name.split('.')[1].split('"')[0]  # 拿到文件后缀
     # file_type = excel_file.name.split('.')[1]  # 拿到文件后缀
     data_list = []
@@ -1463,60 +1016,15 @@
     if data_list:
         res = {"data": data_list}
     else:
         res = {"data": "文件内容格式有误，请检查内容格式是否正确！"}
     return JsonResponse(res)
 
 
-class PharmacyDrugExportViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-    """导出药房药品目录"""
-    pagination_class = None
-    xlsx_use_labels = True
-    xlsx_boolean_labels = {True: "是", False: "否"}
-    queryset = PharmacyDrug.objects.all()
-    serializer_class = ExportPharmacyDrugSerializer
-    renderer_classes = (XLSXRenderer,)
-    filename = 'pharmacy_drug.xlsx'
-    filterset_fields = {"drug_name": ["exact", "iexact", "contains", "icontains"], "is_active": ["exact", "in"]}
-
-    header = {
-        'tab_title': "药房-药品目录",
-        'header_title': "药房-药品目录",
-        'height': 25,
-        'style': {
-            'fill': {
-                'fill_type': 'solid',
-                'start_color': 'FFCCFFCC',
-            },
-            'alignment': {
-                'horizontal': 'center',
-                'vertical': 'center',
-                'wrapText': True,
-                'shrink_to_fit': True,
-            },
-            'border_side': {
-                'border_style': 'thin',
-                'color': 'FF000000',
-            },
-            'font': {
-                'name': 'Arial',
-                'size': 14,
-                'bold': True,
-                'color': 'FF000000',
-            },
-        },
-    }
-
-    def get_body(self):
-        return body
-
-    def get_column_header(self):
-        return column_header
-
-
+@transaction.atomic
 def import_pharmacy_drug(request):
     """导入药房药品excel表数据"""
     created_user = request.POST.get('created_user')
     excel_file = request.FILES.get('excel_file', '')  # 获取前端上传的文件
     file_type = excel_file.name.split('.')[1].split('"')[0]  # 拿到文件后缀
     # file_type = excel_file.name.split('.')[1]  # 拿到文件后缀
     data_list = []
```

### Comparing `base_system-0.2.2/base_system/viewsets.py` & `base_system-0.2.3/base_system/viewsets.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/base_system.egg-info/PKG-INFO` & `base_system-0.2.3/base_system.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.2.2
+Version: 0.2.3
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.2/base_system.egg-info/SOURCES.txt` & `base_system-0.2.3/base_system.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 BaseFunctionModule/settings.py
 BaseFunctionModule/urls.py
 BaseFunctionModule/wsgi.py
 base_system/__init__.py
 base_system/admin.py
 base_system/apps.py
 base_system/auth.py
+base_system/export_viewset.py
 base_system/models.py
 base_system/serializers.py
 base_system/tests.py
 base_system/urls.py
 base_system/views.py
 base_system/viewsets.py
 base_system.egg-info/PKG-INFO
@@ -29,22 +30,24 @@
 base_system.egg-info/dependency_links.txt
 base_system.egg-info/not-zip-safe
 base_system.egg-info/requires.txt
 base_system.egg-info/top_level.txt
 base_system/__pycache__/__init__.cpython-39.pyc
 base_system/__pycache__/admin.cpython-39.pyc
 base_system/__pycache__/apps.cpython-39.pyc
+base_system/__pycache__/export_viewset.cpython-39.pyc
 base_system/__pycache__/models.cpython-39.pyc
 base_system/__pycache__/serializers.cpython-39.pyc
 base_system/__pycache__/tests.cpython-39.pyc
 base_system/__pycache__/urls.cpython-39.pyc
 base_system/__pycache__/views.cpython-39.pyc
 base_system/__pycache__/viewsets.cpython-39.pyc
 base_system/migrations/0001_initial.py
 base_system/migrations/0002_drugdirectory_code_medu_cur.py
 base_system/migrations/0003_alter_extragroup_hospital.py
 base_system/migrations/0004_alter_extragroup_role_name.py
 base_system/migrations/__init__.py
 base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
 base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
 base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
+base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
 base_system/migrations/__pycache__/__init__.cpython-39.pyc
```

### Comparing `base_system-0.2.2/init_data.json` & `base_system-0.2.3/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/manage.py` & `base_system-0.2.3/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/requirements.txt` & `base_system-0.2.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/runtests.py` & `base_system-0.2.3/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.2/setup.py` & `base_system-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.2.2',
+    version='0.2.3',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://github.com/zcjwin",
```

