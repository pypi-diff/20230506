# Comparing `tmp/ob-dj-feature-flags-0.0.3.tar.gz` & `tmp/ob-dj-feature-flags-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-dj-feature-flags-0.0.3.tar", last modified: Sat May  6 13:21:02 2023, max compression
+gzip compressed data, was "ob-dj-feature-flags-0.0.4.tar", last modified: Sat May  6 16:32:32 2023, max compression
```

## Comparing `ob-dj-feature-flags-0.0.3.tar` & `ob-dj-feature-flags-0.0.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.794696 ob-dj-feature-flags-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.778695 ob-dj-feature-flags-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.782695 ob-dj-feature-flags-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/.github/workflows/pre-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/.github/workflows/test-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-06 13:21:02.794696 ob-dj-feature-flags-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    94545 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.782695 ob-dj-feature-flags-0.0.3/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/config/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/config/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/config/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/docker-compose.env
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.782695 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.786695 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.786695 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/flags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/flags/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      288 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/flags/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/flags/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/flags/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.790696 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/todos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/todos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/todos/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/todos/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/todos/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.790696 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.790696 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/admin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      286 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.794696 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/migrations/0002_auto_20230503_2339.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.794696 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/todos/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/todos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/todos/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.794696 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/todos/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/todos/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/todos/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/todos/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.794696 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/utils/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:21:02.786695 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-06 13:21:02.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-06 13:21:02.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 13:21:02.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 13:21:02.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 13:21:02.000000 ob-dj-feature-flags-0.0.3/ob_dj_feature_flags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-06 13:21:02.798696 ob-dj-feature-flags-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-06 13:20:49.000000 ob-dj-feature-flags-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.391672 ob-dj-feature-flags-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.391672 ob-dj-feature-flags-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/.github/workflows/pre-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/.github/workflows/test-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    94545 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.391672 ob-dj-feature-flags-0.0.4/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/config/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/config/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/config/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/docker-compose.env
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.391672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.391672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.391672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/flags/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      288 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/flags/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/flags/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/flags/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.391672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/todos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/todos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/todos/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/todos/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/todos/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/admin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      286 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/migrations/0002_auto_20230503_2339.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/todos/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/todos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/todos/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/todos/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/todos/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/todos/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/todos/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/utils/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:32:32.391672 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-06 16:32:32.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-06 16:32:32.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:32:32.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 16:32:32.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 16:32:32.000000 ob-dj-feature-flags-0.0.4/ob_dj_feature_flags.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-06 16:32:32.395672 ob-dj-feature-flags-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-06 16:32:22.000000 ob-dj-feature-flags-0.0.4/setup.py
```

### Comparing `ob-dj-feature-flags-0.0.3/.github/workflows/pre-release.yml` & `ob-dj-feature-flags-0.0.4/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/.github/workflows/release.yml` & `ob-dj-feature-flags-0.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/.github/workflows/test-build.yml` & `ob-dj-feature-flags-0.0.4/.github/workflows/test-build.yml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/.pre-commit-config.yaml` & `ob-dj-feature-flags-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/Dockerfile` & `ob-dj-feature-flags-0.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/LICENSE` & `ob-dj-feature-flags-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/Makefile` & `ob-dj-feature-flags-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/PKG-INFO` & `ob-dj-feature-flags-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-dj-feature-flags
-Version: 0.0.3
+Version: 0.0.4
 Summary: OBytes django application for managing feature flags
 Home-page: https://www.obytes.com/
 Author: OBytes
 Author-email: hello@obytes.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,70 +19,62 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ob-dj-feature-flags
 
-ob-dj-feature-flags is a Django package for managing feature flags and controlling access to Django views & API endpoints using decorators.
+Feature flags are a powerful technique that allows you to enable/disable specific features in your application without deploying new code. This gives you the ability to control the behavior of your application dynamically and perform A/B testing, read more about feature flags [here](https://www.atlassian.com/continuous-delivery/principles/feature-flags).
+
+ob-dj-feature-flags provides a simple way to create and manage feature flags within your Django admin panel. It also provides decorators for views and viewsets to easily control access based on feature flags.
 
 ## Features
 
 - Create and manage feature flags within your Django admin panel.
-- Decorators for views and viewsets to easily control access based on feature flags.
-- Caching mechanism to improve performance when checking feature flag status.
-- Management command to scan viewsets and actions to populate the feature flags automatically (coming soon).
+- Add decorators to views and viewsets to control access based on the created feature flags.
+- Caching mechanism to reduce database hits when checking feature flag statuses.
+- Feature flags endpoint to use the same feature flags in your client apps.
+- Skip feature flags during tests or in the entire project.
 
-### Overview
+## Setup & Installation
 
-```python
-from ob_dj_feature_flags.utils.decorators import class_feature_flag, action_feature_flag
+1. Use pip to install ob-dj-feature-flags:
 
-@class_feature_flag("todos")
-class TodosViewSet(
-    mixins.CreateModelMixin,
-    mixins.ListModelMixin,
-    viewsets.GenericViewSet,
-):
-    permission_classes = [
-        permissions.AllowAny,
-    ]
-    queryset = Todo.objects.all()
-    serializer_class = TodosSerializer
-
-    @action_feature_flag("todos_list")
-    def list(self, request, *args, **kwargs):
-        return super().list(request, *args, **kwargs)
-
-    @action_feature_flag("todos_create")
-    def create(self, request, *args, **kwargs):
-        return super().create(request, *args, **kwargs)
+```shell
+pip install ob-dj-feature-flags
 ```
 
-In this example, the TodosViewSet class is decorated with `@class_feature_flag("todos")`, which checks if the 'todos' feature flag is active before allowing access to any actions within the viewset.
+2. Add "ob_dj_feature_flags" to your `INSTALLED_APPS` setting like this:
 
-Additionally, the list() method is decorated with `@action_feature_flag("todos_list")`, which checks if the 'todos_list' feature flag is active before allowing access to the list action. Similarly, the create() method is decorated with `@action_feature_flag("todos_create")`, which checks if the 'todos_create' feature flag is active before allowing access to the create action.
-
-By combining both class-level and action-level feature flags, you can control access to the entire viewset based on the 'todos' flag, as well as control access to specific actions within the viewset based on the corresponding flags ('todos_list' and 'todos_create' in this example).
-
-## Installation
+```python
+   # settings.py
+   INSTALLED_APPS = [
+        ...
+        "ob_dj_feature_flags.core.flags",
+   ]
+```
 
-Use pip to install ob-dj-feature-flags:
+3. If you plan to use the created feature flags in your client apps, add the feature flags endpoint to your project's urls.py:
 
-```shell
-pip install ob-dj-feature-flags
+```python
+   # urls.py
+   urlpatterns = [
+        ...
+        path('ob-dj-feature-flags/', include('ob_dj_feature_flags.apis.flags.urls')),
+   ]
 ```
 
+4. Run `python manage.py migrate` to create the feature flags table.
+
 ## Usage
 
 ### Creating Feature Flags
 
 Define feature flags in your Django project using the provided FeatureFlag admin. Each feature flag has a unique name and an active status.
 
-
 ### Decorating Views
 
 Use the `@action_feature_flag` decorator to control access to individual views based on feature flags. Apply the decorator to the desired view functions or class-based views. Example:
 
 ```python
 from ob_dj_feature_flags.utils.decorators import action_feature_flag
 
@@ -109,17 +101,17 @@
 
 This will check if the 'my_feature_flag' is active before allowing access to any actions within the viewset. If the flag is inactive, a JSON response with an error message and status code 404 will be returned.
 
 ### Use in Your Client Apps
 
 Integrating feature flags into your client apps allows you to control the behavior and enable/disable specific features dynamically. To leverage feature flags in your client app, follow these simple steps:
 
-1. At the startup time of your client app make a GET request to the feature flags endpoint of your backend API (`/flags/` by default).
+1. Make a GET request to the feature flags endpoint of your backend API (preferably at startup) `ob-dj-feature-flags/` (check step 3 of Setup & Installation section).
 2. The endpoint will provide a JSON response containing the list of feature flags along with their statuses.
-3. Store the feature flags and their statuses in your client app.
+3. Store the feature flags and their statuses somewhere in your client app.
 4. Use the feature flags to control the behavior of your client app (you can create a wrapper function or a custom hook to simplify this process).
 
 ## Skipping Feature Flags During Tests
 
 To skip feature flags during tests, you can use the `@skip_feature_flags` decorator. This decorator can be applied to test functions or test methods to bypass the feature flag checks within the tested views or viewsets.
 
 To use the `skip_feature_flags` decorator, import it from `ob_dj_feature_flags.utils.decorators` and apply it to your test functions or methods. Here's an example:
```

### Comparing `ob-dj-feature-flags-0.0.3/Pipfile` & `ob-dj-feature-flags-0.0.4/Pipfile`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/Pipfile.lock` & `ob-dj-feature-flags-0.0.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/README.md` & `ob-dj-feature-flags-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,57 @@
 # ob-dj-feature-flags
 
-ob-dj-feature-flags is a Django package for managing feature flags and controlling access to Django views & API endpoints using decorators.
+Feature flags are a powerful technique that allows you to enable/disable specific features in your application without deploying new code. This gives you the ability to control the behavior of your application dynamically and perform A/B testing, read more about feature flags [here](https://www.atlassian.com/continuous-delivery/principles/feature-flags).
+
+ob-dj-feature-flags provides a simple way to create and manage feature flags within your Django admin panel. It also provides decorators for views and viewsets to easily control access based on feature flags.
 
 ## Features
 
 - Create and manage feature flags within your Django admin panel.
-- Decorators for views and viewsets to easily control access based on feature flags.
-- Caching mechanism to improve performance when checking feature flag status.
-- Management command to scan viewsets and actions to populate the feature flags automatically (coming soon).
+- Add decorators to views and viewsets to control access based on the created feature flags.
+- Caching mechanism to reduce database hits when checking feature flag statuses.
+- Feature flags endpoint to use the same feature flags in your client apps.
+- Skip feature flags during tests or in the entire project.
 
-### Overview
+## Setup & Installation
 
-```python
-from ob_dj_feature_flags.utils.decorators import class_feature_flag, action_feature_flag
+1. Use pip to install ob-dj-feature-flags:
 
-@class_feature_flag("todos")
-class TodosViewSet(
-    mixins.CreateModelMixin,
-    mixins.ListModelMixin,
-    viewsets.GenericViewSet,
-):
-    permission_classes = [
-        permissions.AllowAny,
-    ]
-    queryset = Todo.objects.all()
-    serializer_class = TodosSerializer
-
-    @action_feature_flag("todos_list")
-    def list(self, request, *args, **kwargs):
-        return super().list(request, *args, **kwargs)
-
-    @action_feature_flag("todos_create")
-    def create(self, request, *args, **kwargs):
-        return super().create(request, *args, **kwargs)
+```shell
+pip install ob-dj-feature-flags
 ```
 
-In this example, the TodosViewSet class is decorated with `@class_feature_flag("todos")`, which checks if the 'todos' feature flag is active before allowing access to any actions within the viewset.
+2. Add "ob_dj_feature_flags" to your `INSTALLED_APPS` setting like this:
 
-Additionally, the list() method is decorated with `@action_feature_flag("todos_list")`, which checks if the 'todos_list' feature flag is active before allowing access to the list action. Similarly, the create() method is decorated with `@action_feature_flag("todos_create")`, which checks if the 'todos_create' feature flag is active before allowing access to the create action.
-
-By combining both class-level and action-level feature flags, you can control access to the entire viewset based on the 'todos' flag, as well as control access to specific actions within the viewset based on the corresponding flags ('todos_list' and 'todos_create' in this example).
-
-## Installation
+```python
+   # settings.py
+   INSTALLED_APPS = [
+        ...
+        "ob_dj_feature_flags.core.flags",
+   ]
+```
 
-Use pip to install ob-dj-feature-flags:
+3. If you plan to use the created feature flags in your client apps, add the feature flags endpoint to your project's urls.py:
 
-```shell
-pip install ob-dj-feature-flags
+```python
+   # urls.py
+   urlpatterns = [
+        ...
+        path('ob-dj-feature-flags/', include('ob_dj_feature_flags.apis.flags.urls')),
+   ]
 ```
 
+4. Run `python manage.py migrate` to create the feature flags table.
+
 ## Usage
 
 ### Creating Feature Flags
 
 Define feature flags in your Django project using the provided FeatureFlag admin. Each feature flag has a unique name and an active status.
 
-
 ### Decorating Views
 
 Use the `@action_feature_flag` decorator to control access to individual views based on feature flags. Apply the decorator to the desired view functions or class-based views. Example:
 
 ```python
 from ob_dj_feature_flags.utils.decorators import action_feature_flag
 
@@ -86,17 +78,17 @@
 
 This will check if the 'my_feature_flag' is active before allowing access to any actions within the viewset. If the flag is inactive, a JSON response with an error message and status code 404 will be returned.
 
 ### Use in Your Client Apps
 
 Integrating feature flags into your client apps allows you to control the behavior and enable/disable specific features dynamically. To leverage feature flags in your client app, follow these simple steps:
 
-1. At the startup time of your client app make a GET request to the feature flags endpoint of your backend API (`/flags/` by default).
+1. Make a GET request to the feature flags endpoint of your backend API (preferably at startup) `ob-dj-feature-flags/` (check step 3 of Setup & Installation section).
 2. The endpoint will provide a JSON response containing the list of feature flags along with their statuses.
-3. Store the feature flags and their statuses in your client app.
+3. Store the feature flags and their statuses somewhere in your client app.
 4. Use the feature flags to control the behavior of your client app (you can create a wrapper function or a custom hook to simplify this process).
 
 ## Skipping Feature Flags During Tests
 
 To skip feature flags during tests, you can use the `@skip_feature_flags` decorator. This decorator can be applied to test functions or test methods to bypass the feature flag checks within the tested views or viewsets.
 
 To use the `skip_feature_flags` decorator, import it from `ob_dj_feature_flags.utils.decorators` and apply it to your test functions or methods. Here's an example:
```

### Comparing `ob-dj-feature-flags-0.0.3/config/settings.py` & `ob-dj-feature-flags-0.0.4/config/settings.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/config/urls.py` & `ob-dj-feature-flags-0.0.4/config/urls.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/docker-compose.yml` & `ob-dj-feature-flags-0.0.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/manage.py` & `ob-dj-feature-flags-0.0.4/manage.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/apis/todos/views.py` & `ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/apis/todos/views.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/admin.py` & `ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/admin.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/migrations/0001_initial.py` & `ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/flags/models.py` & `ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/flags/models.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/core/todos/migrations/0001_initial.py` & `ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/core/todos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/ob_dj_feature_flags/utils/decorators.py` & `ob-dj-feature-flags-0.0.4/ob_dj_feature_flags/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/ob_dj_feature_flags.egg-info/PKG-INFO` & `ob-dj-feature-flags-0.0.4/ob_dj_feature_flags.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-dj-feature-flags
-Version: 0.0.3
+Version: 0.0.4
 Summary: OBytes django application for managing feature flags
 Home-page: https://www.obytes.com/
 Author: OBytes
 Author-email: hello@obytes.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,70 +19,62 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ob-dj-feature-flags
 
-ob-dj-feature-flags is a Django package for managing feature flags and controlling access to Django views & API endpoints using decorators.
+Feature flags are a powerful technique that allows you to enable/disable specific features in your application without deploying new code. This gives you the ability to control the behavior of your application dynamically and perform A/B testing, read more about feature flags [here](https://www.atlassian.com/continuous-delivery/principles/feature-flags).
+
+ob-dj-feature-flags provides a simple way to create and manage feature flags within your Django admin panel. It also provides decorators for views and viewsets to easily control access based on feature flags.
 
 ## Features
 
 - Create and manage feature flags within your Django admin panel.
-- Decorators for views and viewsets to easily control access based on feature flags.
-- Caching mechanism to improve performance when checking feature flag status.
-- Management command to scan viewsets and actions to populate the feature flags automatically (coming soon).
+- Add decorators to views and viewsets to control access based on the created feature flags.
+- Caching mechanism to reduce database hits when checking feature flag statuses.
+- Feature flags endpoint to use the same feature flags in your client apps.
+- Skip feature flags during tests or in the entire project.
 
-### Overview
+## Setup & Installation
 
-```python
-from ob_dj_feature_flags.utils.decorators import class_feature_flag, action_feature_flag
+1. Use pip to install ob-dj-feature-flags:
 
-@class_feature_flag("todos")
-class TodosViewSet(
-    mixins.CreateModelMixin,
-    mixins.ListModelMixin,
-    viewsets.GenericViewSet,
-):
-    permission_classes = [
-        permissions.AllowAny,
-    ]
-    queryset = Todo.objects.all()
-    serializer_class = TodosSerializer
-
-    @action_feature_flag("todos_list")
-    def list(self, request, *args, **kwargs):
-        return super().list(request, *args, **kwargs)
-
-    @action_feature_flag("todos_create")
-    def create(self, request, *args, **kwargs):
-        return super().create(request, *args, **kwargs)
+```shell
+pip install ob-dj-feature-flags
 ```
 
-In this example, the TodosViewSet class is decorated with `@class_feature_flag("todos")`, which checks if the 'todos' feature flag is active before allowing access to any actions within the viewset.
+2. Add "ob_dj_feature_flags" to your `INSTALLED_APPS` setting like this:
 
-Additionally, the list() method is decorated with `@action_feature_flag("todos_list")`, which checks if the 'todos_list' feature flag is active before allowing access to the list action. Similarly, the create() method is decorated with `@action_feature_flag("todos_create")`, which checks if the 'todos_create' feature flag is active before allowing access to the create action.
-
-By combining both class-level and action-level feature flags, you can control access to the entire viewset based on the 'todos' flag, as well as control access to specific actions within the viewset based on the corresponding flags ('todos_list' and 'todos_create' in this example).
-
-## Installation
+```python
+   # settings.py
+   INSTALLED_APPS = [
+        ...
+        "ob_dj_feature_flags.core.flags",
+   ]
+```
 
-Use pip to install ob-dj-feature-flags:
+3. If you plan to use the created feature flags in your client apps, add the feature flags endpoint to your project's urls.py:
 
-```shell
-pip install ob-dj-feature-flags
+```python
+   # urls.py
+   urlpatterns = [
+        ...
+        path('ob-dj-feature-flags/', include('ob_dj_feature_flags.apis.flags.urls')),
+   ]
 ```
 
+4. Run `python manage.py migrate` to create the feature flags table.
+
 ## Usage
 
 ### Creating Feature Flags
 
 Define feature flags in your Django project using the provided FeatureFlag admin. Each feature flag has a unique name and an active status.
 
-
 ### Decorating Views
 
 Use the `@action_feature_flag` decorator to control access to individual views based on feature flags. Apply the decorator to the desired view functions or class-based views. Example:
 
 ```python
 from ob_dj_feature_flags.utils.decorators import action_feature_flag
 
@@ -109,17 +101,17 @@
 
 This will check if the 'my_feature_flag' is active before allowing access to any actions within the viewset. If the flag is inactive, a JSON response with an error message and status code 404 will be returned.
 
 ### Use in Your Client Apps
 
 Integrating feature flags into your client apps allows you to control the behavior and enable/disable specific features dynamically. To leverage feature flags in your client app, follow these simple steps:
 
-1. At the startup time of your client app make a GET request to the feature flags endpoint of your backend API (`/flags/` by default).
+1. Make a GET request to the feature flags endpoint of your backend API (preferably at startup) `ob-dj-feature-flags/` (check step 3 of Setup & Installation section).
 2. The endpoint will provide a JSON response containing the list of feature flags along with their statuses.
-3. Store the feature flags and their statuses in your client app.
+3. Store the feature flags and their statuses somewhere in your client app.
 4. Use the feature flags to control the behavior of your client app (you can create a wrapper function or a custom hook to simplify this process).
 
 ## Skipping Feature Flags During Tests
 
 To skip feature flags during tests, you can use the `@skip_feature_flags` decorator. This decorator can be applied to test functions or test methods to bypass the feature flag checks within the tested views or viewsets.
 
 To use the `skip_feature_flags` decorator, import it from `ob_dj_feature_flags.utils.decorators` and apply it to your test functions or methods. Here's an example:
```

### Comparing `ob-dj-feature-flags-0.0.3/ob_dj_feature_flags.egg-info/SOURCES.txt` & `ob-dj-feature-flags-0.0.4/ob_dj_feature_flags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-dj-feature-flags-0.0.3/setup.cfg` & `ob-dj-feature-flags-0.0.4/setup.cfg`

 * *Files identical despite different names*

