# Comparing `tmp/django-admin-notice-1.1.4.tar.gz` & `tmp/django_admin_notice-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-admin-notice-1.1.4.tar", last modified: Fri Apr  9 22:39:15 2021, max compression
+gzip compressed data, was "django_admin_notice-2.0.0.tar", max compression
```

## Comparing `django-admin-notice-1.1.4.tar` & `django_admin_notice-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,8 @@
-drwxr-xr-x   0 john      (1000) users      (100)        0 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/
--rw-r--r--   0 john      (1000) users      (100)     1055 2021-03-31 23:06:48.000000 django-admin-notice-1.1.4/LICENSE
--rw-r--r--   0 john      (1000) users      (100)       77 2021-04-09 21:34:37.000000 django-admin-notice-1.1.4/MANIFEST.in
--rw-r--r--   0 john      (1000) users      (100)     5501 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)     3395 2021-04-09 01:02:45.000000 django-admin-notice-1.1.4/README.md
-drwxr-xr-x   0 john      (1000) users      (100)        0 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/admin_notice/
--rw-r--r--   0 john      (1000) users      (100)       22 2021-04-09 22:37:39.000000 django-admin-notice-1.1.4/admin_notice/__init__.py
--rw-r--r--   0 john      (1000) users      (100)       98 2021-04-07 21:18:55.000000 django-admin-notice-1.1.4/admin_notice/apps.py
--rw-r--r--   0 john      (1000) users      (100)      350 2021-04-07 19:24:16.000000 django-admin-notice-1.1.4/admin_notice/context_processors.py
-drwxr-xr-x   0 john      (1000) users      (100)        0 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/admin_notice/templates/
-drwxr-xr-x   0 john      (1000) users      (100)        0 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/admin_notice/templates/admin/
--rw-r--r--   0 john      (1000) users      (100)      624 2021-04-07 23:16:03.000000 django-admin-notice-1.1.4/admin_notice/templates/admin/base.html
-drwxr-xr-x   0 john      (1000) users      (100)        0 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/django_admin_notice.egg-info/
--rw-r--r--   0 john      (1000) users      (100)     5501 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/django_admin_notice.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      424 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/django_admin_notice.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) users      (100)        1 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/django_admin_notice.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) users      (100)        1 2021-04-07 17:31:36.000000 django-admin-notice-1.1.4/django_admin_notice.egg-info/not-zip-safe
--rw-r--r--   0 john      (1000) users      (100)      158 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/django_admin_notice.egg-info/requires.txt
--rw-r--r--   0 john      (1000) users      (100)       13 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/django_admin_notice.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) users      (100)     1377 2021-04-09 22:39:15.000000 django-admin-notice-1.1.4/setup.cfg
--rw-r--r--   0 john      (1000) users      (100)       38 2021-03-31 22:51:15.000000 django-admin-notice-1.1.4/setup.py
+-rw-r--r--   0        0        0     1055 2023-05-06 03:02:54.920043 django_admin_notice-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3062 2023-05-06 03:57:13.409746 django_admin_notice-2.0.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-06 03:02:54.920043 django_admin_notice-2.0.0/admin_notice/__init__.py
+-rw-r--r--   0        0        0       98 2023-05-06 03:02:54.920043 django_admin_notice-2.0.0/admin_notice/apps.py
+-rw-r--r--   0        0        0      350 2023-05-06 03:02:54.920043 django_admin_notice-2.0.0/admin_notice/context_processors.py
+-rw-r--r--   0        0        0      624 2023-05-06 03:02:54.920043 django_admin_notice-2.0.0/admin_notice/templates/admin/base.html
+-rw-r--r--   0        0        0     1643 2023-05-06 03:59:03.841781 django_admin_notice-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 django_admin_notice-2.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-admin-notice-1.1.4/LICENSE` & `django_admin_notice-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-notice-1.1.4/PKG-INFO` & `django_admin_notice-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,129 @@
 Metadata-Version: 2.1
 Name: django-admin-notice
-Version: 1.1.4
-Summary: Show a floating notice banner above the Django admin interface
+Version: 2.0.0
+Summary: Show a floating notice banner above the Django admon interface
 Home-page: https://github.com/DoctorJohn/django-admin-notice
+License: MIT
 Author: Jonathan Ehwald
-Author-email: pypi@ehwald.info
-License: MIT License
-Description: # Django Admin Notice
-        
-        [![PyPI][pypi-image]][pypi-url]
-        [![License][license-image]][license-url]
-        [![Tests][tests-image]][tests-url]
-        
-        [pypi-image]: https://img.shields.io/pypi/v/django-admin-notice
-        [pypi-url]: https://pypi.org/project/django-admin-notice/
-        [license-image]: https://img.shields.io/pypi/l/django-admin-notice
-        [license-url]: https://github.com/DoctorJohn/django-admin-notice/blob/master/LICENSE
-        [tests-image]: https://github.com/DoctorJohn/django-admin-notice/workflows/Tests/badge.svg
-        [tests-url]: https://github.com/DoctorJohn/django-admin-notice/actions
-        
-        Show a floating notice banner above the Django admin interface.
-        Particularly useful for indicating the current deployment environment.
-        
-        ## Installation
-        
-        Install django-admin-notice via the Python Package Index (PyPI):
-        
-        `pip install django-admin-notice`
-        
-        Add `admin_notice` to your `INSTALLED_APPS` somewhere before `django.contrib.admin`.
-        
-        ```python
-        INSTALLED_APPS = [
-            "admin_notice",  # <-- Add this somewhere before "django.contrib.admin"
-            "django.contrib.admin",
-            # ... other apps
-        ]
-        ```
-        
-        Add `admin_notice.context_processors.notice` to the templates `context_processors`.
-        Having `django.template.context_processors.request` is required as well.
-        
-        ```python
-        TEMPLATES = [
-            {
-                "OPTIONS": {
-                    "context_processors": [
-                        "django.template.context_processors.request",  # <-- have this
-                        "admin_notice.context_processors.notice",  # <-- Add this
-                        # ... other context processors
-                    ]
-                },
-            },
-        ]
-        ```
-        
-        ## Settings
-        
-        Set the `ADMIN_NOTICE_TEXT` to the text you want to show above the admin interface.
-        No message is shown if this setting is missing or empty.
-        
-        ```python
-        ADMIN_NOTICE_TEXT = "Production environment"
-        ```
-        
-        Optionally specify a custom text color and background for your notice.
-        The default text color is `white` and the default background `red`.
-        
-        ```python
-        ADMIN_NOTICE_TEXT_COLOR = "white"
-        ADMIN_NOTICE_BACKGROUND = "red"
-        ```
-        
-        ### Tips
-        
-        It's a common use case to indicate the projects deployment environment.
-        The following configuration shows how to obtain the `django-admin-notice`
-        configuration from environment variables and how to configure a fallback.
-        
-        ```python
-        from os import environ
-        
-        ADMIN_NOTICE_TEXT = environ.get("ADMIN_NOTICE_TEXT", "Local environment")
-        ADMIN_NOTICE_TEXT_COLOR = environ.get("ADMIN_NOTICE_TEXT_COLOR", "white")
-        ADMIN_NOTICE_BACKGROUND = environ.get("ADMIN_NOTICE_BACKGROUND", "green")
-        ```
-        
-        ## Example
-        
-        Run `python manage.py runserver` after following the *Installation* section
-        to see a fully working example project.
-        
-        ## Contributing
-        
-        ### Setup
-        
-        1. Clone the repository and enter the cloned folder
-        2. (optional) Create and activate a dedicated Python virtual environment
-        3. Run `pip install -e ".[dev]"` to install the projects requirements
-        4. (optional) Run `pre-commit install` to install the pre-commit hook
-        
-        ### Pre-commit hook
-        
-        Our pre-commit hook formats and lints the code.
-        
-        ### Formatting and linting
-        
-        - Run `black admin_notice tests` to format the code
-        - Run `flake8 admin_notice tests` to lint the code
-        
-        ### Testing
-        
-        - Run `py.test --cov admin_notice tests` to run the tests in the current Python env
-        - Run `tox` to run the tests in all supported Python and Django environments
-        
-        ### Makefile
-        
-        All commands listed above have shortcut make recipes.
-        Take a look at the `Makefile` to learn more.
-        
-Platform: UNKNOWN
+Author-email: github@ehwald.info
+Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
+Requires-Dist: django (>=2.2)
+Project-URL: Documentation, https://github.com/DoctorJohn/django-admin-notice
+Project-URL: Repository, https://github.com/DoctorJohn/django-admin-notice
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+
+# Django Admin Notice
+
+[![PyPI][pypi-image]][pypi-url]
+![PyPI - Python Version][python-image]
+![PyPI - Django Version][django-image]
+[![License][license-image]][license-url]
+[![Tests][tests-image]][tests-url]
+
+[pypi-image]: https://img.shields.io/pypi/v/django-admin-notice
+[pypi-url]: https://pypi.org/project/django-admin-notice/
+[python-image]: https://img.shields.io/pypi/pyversions/django-admin-notice
+[django-image]: https://img.shields.io/pypi/djversions/django-admin-notice
+[license-image]: https://img.shields.io/pypi/l/django-admin-notice
+[license-url]: https://github.com/DoctorJohn/django-admin-notice/blob/master/LICENSE
+[tests-image]: https://github.com/DoctorJohn/django-admin-notice/workflows/Tests/badge.svg
+[tests-url]: https://github.com/DoctorJohn/django-admin-notice/actions
+
+Show a floating notice banner above the Django admin interface.
+Particularly useful for indicating the current deployment environment.
+
+![Admin notice preview](.github/images/preview.png)
+
+## Installation
+
+Install django-admin-notice by running `pip install django-admin-notice`
+
+Add `admin_notice` to your `INSTALLED_APPS` somewhere before `django.contrib.admin`.
+
+```python
+INSTALLED_APPS = [
+    "admin_notice",  # <-- Add this somewhere before "django.contrib.admin"
+    "django.contrib.admin",
+    # ... other apps
+]
+```
+
+Add `admin_notice.context_processors.notice` to the templates `context_processors`. 
+Having `django.template.context_processors.request` is required as well.
+
+```python
+TEMPLATES = [
+    {
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.request",  # <-- have this
+                "admin_notice.context_processors.notice",  # <-- Add this
+                # ... other context processors
+            ]
+        },
+    },
+]
+```
+
+## Settings
+
+Set the `ADMIN_NOTICE_TEXT` to the text you want to show above the admin interface.
+No message is shown if this setting is missing or empty.
+
+```python
+ADMIN_NOTICE_TEXT = "Production environment"
+```
+
+Optionally specify a custom text color and background for your notice.
+The default text color is `white` and the default background `red`.
+
+```python
+ADMIN_NOTICE_TEXT_COLOR = "white"
+ADMIN_NOTICE_BACKGROUND = "red"
+```
+
+### Tips
+
+It's a common use case to indicate the projects deployment environment.
+The following configuration shows how to obtain the `django-admin-notice`
+configuration from environment variables and how to configure a fallback.
+
+```python
+from os import environ
+
+ADMIN_NOTICE_TEXT = environ.get("ADMIN_NOTICE_TEXT", "Local environment")
+ADMIN_NOTICE_TEXT_COLOR = environ.get("ADMIN_NOTICE_TEXT_COLOR", "white")
+ADMIN_NOTICE_BACKGROUND = environ.get("ADMIN_NOTICE_BACKGROUND", "green")
+```
+
+## Example project
+
+Take a look at our Django example project under `tests/project`. You can run it by executing these commands:
+
+1. `poetry install`
+2. `poetry run python tests/project/manage.py migrate`
+3. `poetry run python tests/project/manage.py createsuperuser`
+4. `poetry run python tests/project/manage.py runserver`
+
```

### Comparing `django-admin-notice-1.1.4/README.md` & `django_admin_notice-2.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # Django Admin Notice
 
 [![PyPI][pypi-image]][pypi-url]
+![PyPI - Python Version][python-image]
+![PyPI - Django Version][django-image]
 [![License][license-image]][license-url]
 [![Tests][tests-image]][tests-url]
 
 [pypi-image]: https://img.shields.io/pypi/v/django-admin-notice
 [pypi-url]: https://pypi.org/project/django-admin-notice/
+[python-image]: https://img.shields.io/pypi/pyversions/django-admin-notice
+[django-image]: https://img.shields.io/pypi/djversions/django-admin-notice
 [license-image]: https://img.shields.io/pypi/l/django-admin-notice
 [license-url]: https://github.com/DoctorJohn/django-admin-notice/blob/master/LICENSE
 [tests-image]: https://github.com/DoctorJohn/django-admin-notice/workflows/Tests/badge.svg
 [tests-url]: https://github.com/DoctorJohn/django-admin-notice/actions
 
 Show a floating notice banner above the Django admin interface.
 Particularly useful for indicating the current deployment environment.
 
-## Installation
+![Admin notice preview](.github/images/preview.png)
 
-Install django-admin-notice via the Python Package Index (PyPI):
+## Installation
 
-`pip install django-admin-notice`
+Install django-admin-notice by running `pip install django-admin-notice`
 
 Add `admin_notice` to your `INSTALLED_APPS` somewhere before `django.contrib.admin`.
 
 ```python
 INSTALLED_APPS = [
     "admin_notice",  # <-- Add this somewhere before "django.contrib.admin"
     "django.contrib.admin",
     # ... other apps
 ]
 ```
 
-Add `admin_notice.context_processors.notice` to the templates `context_processors`.
+Add `admin_notice.context_processors.notice` to the templates `context_processors`. 
 Having `django.template.context_processors.request` is required as well.
 
 ```python
 TEMPLATES = [
     {
         "OPTIONS": {
             "context_processors": [
@@ -74,39 +78,15 @@
 from os import environ
 
 ADMIN_NOTICE_TEXT = environ.get("ADMIN_NOTICE_TEXT", "Local environment")
 ADMIN_NOTICE_TEXT_COLOR = environ.get("ADMIN_NOTICE_TEXT_COLOR", "white")
 ADMIN_NOTICE_BACKGROUND = environ.get("ADMIN_NOTICE_BACKGROUND", "green")
 ```
 
-## Example
-
-Run `python manage.py runserver` after following the *Installation* section
-to see a fully working example project.
-
-## Contributing
-
-### Setup
-
-1. Clone the repository and enter the cloned folder
-2. (optional) Create and activate a dedicated Python virtual environment
-3. Run `pip install -e ".[dev]"` to install the projects requirements
-4. (optional) Run `pre-commit install` to install the pre-commit hook
-
-### Pre-commit hook
-
-Our pre-commit hook formats and lints the code.
-
-### Formatting and linting
-
-- Run `black admin_notice tests` to format the code
-- Run `flake8 admin_notice tests` to lint the code
-
-### Testing
-
-- Run `py.test --cov admin_notice tests` to run the tests in the current Python env
-- Run `tox` to run the tests in all supported Python and Django environments
+## Example project
 
-### Makefile
+Take a look at our Django example project under `tests/project`. You can run it by executing these commands:
 
-All commands listed above have shortcut make recipes.
-Take a look at the `Makefile` to learn more.
+1. `poetry install`
+2. `poetry run python tests/project/manage.py migrate`
+3. `poetry run python tests/project/manage.py createsuperuser`
+4. `poetry run python tests/project/manage.py runserver`
```

### Comparing `django-admin-notice-1.1.4/admin_notice/templates/admin/base.html` & `django_admin_notice-2.0.0/admin_notice/templates/admin/base.html`

 * *Files identical despite different names*

