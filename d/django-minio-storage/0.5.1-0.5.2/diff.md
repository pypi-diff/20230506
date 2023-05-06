# Comparing `tmp/django-minio-storage-0.5.1.tar.gz` & `tmp/django-minio-storage-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-minio-storage-0.5.1.tar", last modified: Fri May  5 15:11:34 2023, max compression
+gzip compressed data, was "django-minio-storage-0.5.2.tar", last modified: Sat May  6 04:01:56 2023, max compression
```

## Comparing `django-minio-storage-0.5.1.tar` & `django-minio-storage-0.5.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.291364 django-minio-storage-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.flake8rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.267364 django-minio-storage-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.279364 django-minio-storage-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-05 15:11:34.291364 django-minio-storage-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.279364 django-minio-storage-0.5.1/django_minio_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/django_minio_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.279364 django-minio-storage-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/licences.md
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.283364 django-minio-storage-0.5.1/minio_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.283364 django-minio-storage-0.5.1/minio_storage/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.283364 django-minio-storage-0.5.1/minio_storage/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/management/commands/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/minio_storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 15:11:34.000000 django-minio-storage-0.5.1/minio_storage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:11:34.291364 django-minio-storage-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.287364 django-minio-storage-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.287364 django-minio-storage-0.5.1/tests/django_minio_storage_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/django_minio_storage_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/django_minio_storage_tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/django_minio_storage_tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/django_minio_storage_tests/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.287364 django-minio-storage-0.5.1/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:34.291364 django-minio-storage-0.5.1/tests/test_app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/bucket_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/custom_storage_class_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/managementcommand_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/retrieve_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/upload_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/test_app/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tests/watermelon-cat.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-05 15:11:19.000000 django-minio-storage-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.595380 django-minio-storage-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.flake8rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.579380 django-minio-storage-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.583380 django-minio-storage-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 04:01:56.595380 django-minio-storage-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.587380 django-minio-storage-0.5.2/django_minio_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/django_minio_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.587380 django-minio-storage-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/licences.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.587380 django-minio-storage-0.5.2/minio_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.587380 django-minio-storage-0.5.2/minio_storage/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/minio_storage/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/management/commands/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/minio_storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 04:01:56.000000 django-minio-storage-0.5.2/minio_storage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 04:01:56.595380 django-minio-storage-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/tests/django_minio_storage_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/django_minio_storage_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/django_minio_storage_tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/django_minio_storage_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/django_minio_storage_tests/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:56.591380 django-minio-storage-0.5.2/tests/test_app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/bucket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/custom_storage_class_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/managementcommand_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/retrieve_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/upload_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/test_app/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tests/watermelon-cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-06 04:01:34.000000 django-minio-storage-0.5.2/tox.ini
```

### Comparing `django-minio-storage-0.5.1/.github/workflows/release.yml` & `django-minio-storage-0.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/.github/workflows/tox.yml` & `django-minio-storage-0.5.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/CHANGELOG.md` & `django-minio-storage-0.5.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.5.2
+
+Add/fix more type hints.
+
 ## 0.5.1
 
 Fix type hints
 
 ## 0.5.0
 
 Switched the minio-py client library version from `<7` to `>=7`.
```

### Comparing `django-minio-storage-0.5.1/LICENSE-APACHE` & `django-minio-storage-0.5.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/LICENSE-MIT` & `django-minio-storage-0.5.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/PKG-INFO` & `django-minio-storage-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.1
+Version: 0.5.2
 Summary: Django file storage using the minio python client
 Home-page: https://github.com/py-pa/django-minio-storage
 Author: Tom Houlé
 Author-email: tom@kafunsho.be
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-minio-storage-0.5.1/README.md` & `django-minio-storage-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/django_minio_storage.egg-info/PKG-INFO` & `django-minio-storage-0.5.2/django_minio_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.1
+Version: 0.5.2
 Summary: Django file storage using the minio python client
 Home-page: https://github.com/py-pa/django-minio-storage
 Author: Tom Houlé
 Author-email: tom@kafunsho.be
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-minio-storage-0.5.1/django_minio_storage.egg-info/SOURCES.txt` & `django-minio-storage-0.5.2/django_minio_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/docs/development.md` & `django-minio-storage-0.5.2/docs/development.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/docs/index.md` & `django-minio-storage-0.5.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/docs/licences.md` & `django-minio-storage-0.5.2/docs/licences.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/docs/usage.md` & `django-minio-storage-0.5.2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/minio_storage/files.py` & `django-minio-storage-0.5.2/minio_storage/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from django.core.files.base import File
 from minio import error as merr
 
 from minio_storage.errors import minio_error
 
 if T.TYPE_CHECKING:
-    from minio_storage.storage import Storage
+    from minio_storage.storage import MinioStorage
 
 logger = getLogger("minio_storage")
 
 
 class ReadOnlyMixin:
     """File class mixin which disallows .write() calls"""
 
@@ -32,65 +32,67 @@
     def seek(self, *args, **kwargs) -> bool:
         # TODO: maybe exception is better
         # raise NotImplementedError('seek is not supported')
         return False
 
 
 class MinioStorageFile(File):
-    def __init__(self, name: str, mode: str, storage: "Storage", **kwargs):
-        self._storage: "Storage" = storage
+    def __init__(self, name: str, mode: str, storage: "MinioStorage", **kwargs):
+        self._storage: "MinioStorage" = storage
         self.name: str = name
         self._mode: str = mode
         self._file = None
 
 
 class ReadOnlyMinioObjectFile(MinioStorageFile, ReadOnlyMixin, NonSeekableMixin):
     """A django File class which directly exposes the underlying minio object. This
     means the the instance doesnt support functions like .seek() and is required to
     be closed to be able to reuse minio connections."""
 
     def __init__(
         self,
         name: str,
         mode: str,
-        storage: "Storage",
+        storage: "MinioStorage",
         max_memory_size: T.Optional[int] = None,
         **kwargs,
     ):
         if mode.find("w") > -1:
             raise NotImplementedError(
                 "ReadOnlyMinioObjectFile storage only support read modes"
             )
         if max_memory_size is not None:
             self.max_memory_size = max_memory_size
         super().__init__(name, mode, storage)
 
-    def _get_file(self):
+    @property
+    def file(self):
+        obj = None
         if self._file is None:
             try:
                 obj = self._storage.client.get_object(
                     self._storage.bucket_name, self.name
                 )
                 self._file = obj
                 return self._file
             except merr.InvalidResponseError as error:
                 logger.warn(error)
                 raise OSError(f"File {self.name} does not exist")
             finally:
                 try:
-                    obj.release_conn()
+                    if obj:
+                        obj.release_conn()
                 except Exception as e:
                     logger.error(str(e))
         return self._file
 
+    @file.setter
     def _set_file(self, value):
         self._file = value
 
-    file = property(_get_file, _set_file)
-
     def close(self):
         try:
             self.file.close()
         finally:
             self.file.release_conn()
 
 
@@ -100,28 +102,30 @@
 
     max_memory_size: int = 1024 * 1024 * 10
 
     def __init__(
         self,
         name: str,
         mode: str,
-        storage: "Storage",
+        storage: "MinioStorage",
         max_memory_size: T.Optional[int] = None,
         **kwargs,
     ):
         if mode.find("w") > -1:
             raise NotImplementedError(
                 "ReadOnlySpooledTemporaryFile storage only support read modes"
             )
         if max_memory_size is not None:
             self.max_memory_size = max_memory_size
         super().__init__(name, mode, storage)
 
-    def _get_file(self):
+    @property
+    def file(self):
         if self._file is None:
+            obj = None
             try:
                 obj = self._storage.client.get_object(
                     self._storage.bucket_name, self.name
                 )
                 self._file = tempfile.SpooledTemporaryFile(
                     max_size=self.max_memory_size
                 )
@@ -129,21 +133,21 @@
                     self._file.write(d)
                 self._file.seek(0)
                 return self._file
             except merr.InvalidResponseError as error:
                 raise minio_error(f"File {self.name} does not exist", error)
             finally:
                 try:
-                    obj.release_conn()
+                    if obj:
+                        obj.release_conn()
                 except Exception as e:
                     logger.error(str(e))
         return self._file
 
+    @file.setter
     def _set_file(self, value):
         self._file = value
 
-    file = property(_get_file, _set_file)
-
     def close(self):
         if self._file is not None:
             self._file.close()
             self._file = None
```

### Comparing `django-minio-storage-0.5.1/minio_storage/management/commands/minio.py` & `django-minio-storage-0.5.2/minio_storage/management/commands/minio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import argparse
 import json
 import sys
+import typing as T
 from string import Template
 from unittest.mock import patch
 
 import minio.error
 from django.core.management.base import BaseCommand, CommandError
 from django.utils.module_loading import import_string
 
@@ -41,20 +41,16 @@
 
         cmds = parser.add_subparsers(
             dest="command",
             title="subcommands",
             description="valid subcommands",
             # required=True,
         )
-        cmds._parser_class = argparse.ArgumentParser  # circumvent Django 1.11 bug
-
         cmds.add_parser(self.CHECK, help="check bucket")
-
         cmds.add_parser(self.CREATE, help="make bucket")
-
         cmds.add_parser(self.DELETE, help="remove an empty bucket")
 
         ls = cmds.add_parser(self.LIST, help="list bucket objects or buckets")
         ls.add_argument("--dirs", action="store_true", help="include directories")
         ls.add_argument("--files", action="store_true", help="include files")
         ls.add_argument(
             "-r", "--recursive", action="store_true", help="find files recursive"
@@ -136,15 +132,15 @@
         except ImportError:
             raise CommandError(f"could not find storage class: {class_name}")
         if not issubclass(storage_class, MinioStorage):
             raise CommandError(f"{class_name} is not an sub class of MinioStorage.")
 
         # TODO: maybe another way
         with patch.object(storage_class, "_init_check", return_value=None):
-            storage = storage_class()
+            storage = storage_class()  # type: ignore
             return storage
 
     def bucket_exists(self, storage, bucket_name):
         exists = storage.client.bucket_exists(bucket_name)
         if not exists:
             raise CommandError(f"bucket {bucket_name} does not exist")
 
@@ -158,15 +154,15 @@
         storage,
         bucket_name: str,
         *,
         prefix: str,
         list_dirs: bool,
         list_files: bool,
         recursive: bool,
-        format: str = None,
+        format: T.Optional[str] = None,
         summary: bool = True,
     ):
         try:
             objs = storage.client.list_objects(
                 bucket_name, prefix=prefix, recursive=recursive
             )
```

### Comparing `django-minio-storage-0.5.1/minio_storage/policy.py` & `django-minio-storage-0.5.2/minio_storage/policy.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/minio_storage/storage.py` & `django-minio-storage-0.5.2/minio_storage/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import minio
 import minio.error as merr
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.storage import Storage
 from django.utils import timezone
 from django.utils.deconstruct import deconstructible
+from minio.datatypes import Object
 
 from minio_storage.errors import minio_error
 from minio_storage.files import ReadOnlySpooledTemporaryFile
 from minio_storage.policy import Policy
 
 logger = getLogger("minio_storage")
 
@@ -102,20 +103,17 @@
     def _create_base_url_client(client: minio.Minio, bucket_name: str, base_url: str):
         """
         Clone a Minio client, using a different endpoint from `base_url`.
         """
         base_url_parts = urlsplit(base_url)
 
         # Clone from the normal client, but with base_url as the endpoint
-        credentials = client._provider.retrieve()
         base_url_client = minio.Minio(
             base_url_parts.netloc,
-            access_key=credentials.access_key,
-            secret_key=credentials.secret_key,
-            session_token=credentials.session_token,
+            credentials=client._provider,
             secure=base_url_parts.scheme == "https",
             # The bucket region may be auto-detected by client (via an HTTP
             # request), so don't just use client._region
             region=client._get_region(bucket_name, None),
             http_client=client._http,
         )
 
@@ -246,16 +244,16 @@
         except merr.S3Error:
             raise
         except merr.InvalidResponseError as error:
             raise minio_error(f"Could not list directory {path}", error)
 
     def size(self, name: str) -> int:
         try:
-            info = self.client.stat_object(self.bucket_name, name)
-            return info.size
+            info: Object = self.client.stat_object(self.bucket_name, name)
+            return info.size  # type: ignore
         except merr.InvalidResponseError as error:
             raise minio_error(f"Could not access file size for {name}", error)
 
     def _presigned_url(
         self, name: str, max_age: T.Optional[datetime.timedelta] = None
     ) -> T.Optional[str]:
         kwargs = {}
@@ -289,15 +287,15 @@
             )
         if url:
             return str(url)
         return None
 
     def url(
         self, name: str, *args, max_age: T.Optional[datetime.timedelta] = None
-    ) -> T.Optional[str]:
+    ) -> str:
         url = ""
         if self.presign_urls:
             url = self._presigned_url(name, max_age=max_age)
         else:
 
             def strip_beg(path):
                 while path.startswith("/"):
@@ -313,15 +311,17 @@
                 url = "{}/{}".format(strip_end(self.base_url), quote(strip_beg(name)))
             else:
                 url = "{}/{}/{}".format(
                     strip_end(self.endpoint_url),
                     self.bucket_name,
                     quote(strip_beg(name)),
                 )
-        return url
+        if url:
+            return url
+        raise OSError(f"could not produce URL for {name}")
 
     @property
     def endpoint_url(self):
         return self.client._base_url._url.geturl()
 
     def accessed_time(self, name: str) -> datetime.datetime:
         """
@@ -333,20 +333,22 @@
         """
         Not available via the S3 API
         """
         return self.modified_time(name)
 
     def modified_time(self, name: str) -> datetime.datetime:
         try:
-            info = self.client.stat_object(self.bucket_name, name)
-            return info.last_modified
+            info: Object = self.client.stat_object(self.bucket_name, name)
+            if info.last_modified:
+                return info.last_modified  # type: ignore
         except merr.InvalidResponseError as error:
             raise minio_error(
                 f"Could not access modification time for file {name}", error
             )
+        raise OSError(f"Could not access modification time for file {name}")
 
 
 _NoValue = object()
 
 
 def get_setting(name: str, default=_NoValue) -> T.Any:
     result = getattr(settings, name, default)
```

### Comparing `django-minio-storage-0.5.1/setup.py` & `django-minio-storage-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tests/django_minio_storage_tests/settings.py` & `django-minio-storage-0.5.2/tests/django_minio_storage_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tests/django_minio_storage_tests/urls.py` & `django-minio-storage-0.5.2/tests/django_minio_storage_tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tests/test_app/tests/bucket_tests.py` & `django-minio-storage-0.5.2/tests/test_app/tests/bucket_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tests/test_app/tests/custom_storage_class_tests.py` & `django-minio-storage-0.5.2/tests/test_app/tests/custom_storage_class_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,22 +92,23 @@
             # files are closed after the copying is done.
             #
             with open(filename, "wb") as out_file, storage.open(
                 storage_filename
             ) as storage_file:
                 # Copy the stream from the http stream to the out_file
                 #
-                shutil.copyfileobj(storage_file.file, out_file)
+                shutil.copyfileobj(storage_file.file, out_file)  # type: ignore
 
                 #
                 # We are not using the ReadOnlyMinioObjectFile type so we can't seek in
                 # it.
                 #
                 with self.assertRaises(io.UnsupportedOperation):
-                    storage_file.file.seek()
+                    if storage_file.file:
+                        storage_file.file.seek(0)
 
             workspace_files = os.listdir(workspace)
             print(workspace_files)  # prints: ['secret.txt']
 
             #
             # Process the file with external tools or something....
             #
```

### Comparing `django-minio-storage-0.5.1/tests/test_app/tests/delete_tests.py` & `django-minio-storage-0.5.2/tests/test_app/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tests/test_app/tests/managementcommand_tests.py` & `django-minio-storage-0.5.2/tests/test_app/tests/managementcommand_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tests/test_app/tests/retrieve_tests.py` & `django-minio-storage-0.5.2/tests/test_app/tests/retrieve_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tests/test_app/tests/upload_tests.py` & `django-minio-storage-0.5.2/tests/test_app/tests/upload_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,21 +88,21 @@
             "Last-Modified",
             "Server",
             "Vary",
             "X-Amz-Request-Id",
             "X-Xss-Protection",
             "Date",
         }
-        self.assertTrue(metadata_attrs.issubset(res.metadata.keys()))
+        self.assertTrue(metadata_attrs.issubset(res.metadata.keys()))  # type: ignore
 
 
 @override_settings(
     MINIO_STORAGE_MEDIA_OBJECT_METADATA={"Cache-Control": "max-age=1000"},
 )
 class TestDefaultObjectMetadata(BaseTestMixin, TestCase):
     def test_default_metadata(self):
         ivan = self.media_storage.save("pelican.txt", ContentFile(b"Ivan le Pelican"))
         res = self.media_storage.client.stat_object(
             self.media_storage.bucket_name, ivan
         )
 
-        self.assertEqual(res.metadata["Cache-Control"], "max-age=1000")
+        self.assertEqual(res.metadata["Cache-Control"], "max-age=1000")  # type: ignore
```

### Comparing `django-minio-storage-0.5.1/tests/test_app/tests/utils.py` & `django-minio-storage-0.5.2/tests/test_app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tests/watermelon-cat.jpg` & `django-minio-storage-0.5.2/tests/watermelon-cat.jpg`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.1/tox.ini` & `django-minio-storage-0.5.2/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,18 @@
     coverage html
 depends=py311-django42-minioknown
 
 [testenv:pyright]
 basepython = python3
 deps =
         pyright
+        django-stubs==4.2.0
         -rdev-requirements.txt
 commands =
-    pyright --skipunannotated --level WARNING
+    pyright --level WARNING
 
 
 [testenv:lint]
 setenv=
     PYTHONWARNINGS=ignore
 basepython = python3
 deps =
```

