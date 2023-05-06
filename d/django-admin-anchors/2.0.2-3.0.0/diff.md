# Comparing `tmp/django_admin_anchors-2.0.2.tar.gz` & `tmp/django_admin_anchors-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_anchors-2.0.2.tar", max compression
+gzip compressed data, was "django_admin_anchors-3.0.0.tar", max compression
```

## Comparing `django_admin_anchors-2.0.2.tar` & `django_admin_anchors-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1055 2021-03-31 23:06:48.789207 django_admin_anchors-2.0.2/LICENSE
--rw-r--r--   0        0        0     2050 2023-05-05 13:35:42.593916 django_admin_anchors-2.0.2/README.md
--rw-r--r--   0        0        0       78 2023-05-05 13:35:42.593916 django_admin_anchors-2.0.2/admin_anchors/__init__.py
--rw-r--r--   0        0        0     1698 2023-05-05 13:35:42.593916 django_admin_anchors-2.0.2/admin_anchors/decorators.py
--rw-r--r--   0        0        0     1199 2023-05-05 13:35:42.593916 django_admin_anchors-2.0.2/admin_anchors/utils.py
--rw-r--r--   0        0        0     1660 2023-05-05 13:41:56.391537 django_admin_anchors-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 django_admin_anchors-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2021-03-31 23:06:48.789207 django_admin_anchors-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2589 2023-05-06 02:21:27.934531 django_admin_anchors-3.0.0/README.md
+-rw-r--r--   0        0        0       78 2023-05-05 13:35:42.593916 django_admin_anchors-3.0.0/admin_anchors/__init__.py
+-rw-r--r--   0        0        0     1918 2023-05-06 02:21:27.934531 django_admin_anchors-3.0.0/admin_anchors/decorators.py
+-rw-r--r--   0        0        0      937 2023-05-06 02:21:27.934531 django_admin_anchors-3.0.0/admin_anchors/utils.py
+-rw-r--r--   0        0        0     1631 2023-05-06 02:21:35.071360 django_admin_anchors-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 django_admin_anchors-3.0.0/PKG-INFO
```

### Comparing `django_admin_anchors-2.0.2/LICENSE` & `django_admin_anchors-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_anchors-2.0.2/README.md` & `django_admin_anchors-3.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,27 +11,33 @@
 [python-image]: https://img.shields.io/pypi/pyversions/django-admin-anchors
 [django-image]: https://img.shields.io/pypi/djversions/django-admin-anchors
 [license-image]: https://img.shields.io/pypi/l/django-admin-anchors
 [license-url]: https://github.com/DoctorJohn/django-admin-anchors/blob/master/LICENSE
 [tests-image]: https://github.com/DoctorJohn/django-admin-anchors/workflows/Tests/badge.svg
 [tests-url]: https://github.com/DoctorJohn/django-admin-anchors/actions
 
-Turn Django admin list display items into clickable links to related objects using
-decorators.
+Turn Django admin list display items into clickable links to related
+objects using decorators.
+
+Clicking admin anchors will redirect to a filtered changelist view
+showing the related objects. This allows you to get a quick overview
+and run actions on the filtered objects.
 
 ## Installation
 
 `pip install django-admin-anchors`
 
 ## Usage
 
 Take a look at the `tests/project` directory to see a runnable example project.
 
 ### Add links to the object list page
 
+![Object list page](.github/images/list.png)
+
 ```python
 from django.contrib import admin
 from admin_anchors import admin_anchor
 from yourapp.models import Team
 
 
 @admin.register(Team)
@@ -47,15 +53,17 @@
         return "Captains profile"
 
     @admin_anchor("members")
     def members_link(self, instance):
         return f"{instance.members.count()} members"
 ```
 
-### Add links to the object edit page
+### Add links to the object update page
+
+![Object change page](.github/images/change.png)
 
 ```python
 from django.contrib import admin
 from admin_anchors import admin_anchor
 from yourapp.models import Player
 
 
@@ -63,7 +71,16 @@
 class PlayerAdmin(admin.ModelAdmin):
     readonly_fields = ["profile_link"]
 
     @admin_anchor("profile")
     def profile_link(self, instance):
         return "Profile"
 ```
+
+## Example project
+
+Take a look at our Django example project under `tests/project`.
+You can run it by executing these commands:
+
+1. `poetry install`
+2. `poetry run python tests/project/manage.py migrate`
+3. `poetry run python tests/project/manage.py runserver`
```

### Comparing `django_admin_anchors-2.0.2/pyproject.toml` & `django_admin_anchors-3.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 [tool.poetry]
 name = "django-admin-anchors"
-version = "2.0.2"
+version = "3.0.0"
 description = "Link related objects in Django admin using decorators"
 license = "MIT"
 authors = ["Jonathan Ehwald <github@ehwald.info>"]
 readme = "README.md"
 homepage = "https://github.com/DoctorJohn/django-admin-anchors"
 repository = "https://github.com/DoctorJohn/django-admin-anchors"
 documentation = "https://github.com/DoctorJohn/django-admin-anchors"
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
-    "Framework :: Django :: 3.0",
-    "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 packages = [ { include = "admin_anchors" } ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-Django = ">=2.2"
+python = "^3.8"
+Django = ">=3.2"
 
-[tool.poetry.dev-dependencies]
-flake8 = "^4.0.1"
-black = "^22.1.0"
-isort = "^5.10.1"
-pre-commit = "^2.17.0"
-pytest = "^7.0.1"
-pytest-cov = "^3.0.0"
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.264"
+black = "^23.3.0"
+pre-commit = "^3.3.1"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 pytest-django = "^4.5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+line-length = 119
+ignore = ["E501"]
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.project.project.settings"
```

### Comparing `django_admin_anchors-2.0.2/PKG-INFO` & `django_admin_anchors-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: django-admin-anchors
-Version: 2.0.2
+Version: 3.0.0
 Summary: Link related objects in Django admin using decorators
 Home-page: https://github.com/DoctorJohn/django-admin-anchors
 License: MIT
 Author: Jonathan Ehwald
 Author-email: github@ehwald.info
-Requires-Python: >=3.7,<4.0
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
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Dist: Django (>=2.2)
+Requires-Dist: Django (>=3.2)
 Project-URL: Documentation, https://github.com/DoctorJohn/django-admin-anchors
 Project-URL: Repository, https://github.com/DoctorJohn/django-admin-anchors
 Description-Content-Type: text/markdown
 
 # Django Admin Anchors
 
 [![PyPI][pypi-image]][pypi-url]
@@ -49,27 +47,33 @@
 [python-image]: https://img.shields.io/pypi/pyversions/django-admin-anchors
 [django-image]: https://img.shields.io/pypi/djversions/django-admin-anchors
 [license-image]: https://img.shields.io/pypi/l/django-admin-anchors
 [license-url]: https://github.com/DoctorJohn/django-admin-anchors/blob/master/LICENSE
 [tests-image]: https://github.com/DoctorJohn/django-admin-anchors/workflows/Tests/badge.svg
 [tests-url]: https://github.com/DoctorJohn/django-admin-anchors/actions
 
-Turn Django admin list display items into clickable links to related objects using
-decorators.
+Turn Django admin list display items into clickable links to related
+objects using decorators.
+
+Clicking admin anchors will redirect to a filtered changelist view
+showing the related objects. This allows you to get a quick overview
+and run actions on the filtered objects.
 
 ## Installation
 
 `pip install django-admin-anchors`
 
 ## Usage
 
 Take a look at the `tests/project` directory to see a runnable example project.
 
 ### Add links to the object list page
 
+![Object list page](.github/images/list.png)
+
 ```python
 from django.contrib import admin
 from admin_anchors import admin_anchor
 from yourapp.models import Team
 
 
 @admin.register(Team)
@@ -85,15 +89,17 @@
         return "Captains profile"
 
     @admin_anchor("members")
     def members_link(self, instance):
         return f"{instance.members.count()} members"
 ```
 
-### Add links to the object edit page
+### Add links to the object update page
+
+![Object change page](.github/images/change.png)
 
 ```python
 from django.contrib import admin
 from admin_anchors import admin_anchor
 from yourapp.models import Player
 
 
@@ -102,7 +108,16 @@
     readonly_fields = ["profile_link"]
 
     @admin_anchor("profile")
     def profile_link(self, instance):
         return "Profile"
 ```
 
+## Example project
+
+Take a look at our Django example project under `tests/project`.
+You can run it by executing these commands:
+
+1. `poetry install`
+2. `poetry run python tests/project/manage.py migrate`
+3. `poetry run python tests/project/manage.py runserver`
+
```

