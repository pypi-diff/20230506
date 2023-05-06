# Comparing `tmp/django-privates-2.0.0.tar.gz` & `tmp/django-privates-2.0.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-privates-2.0.0.tar", last modified: Fri May  5 16:06:04 2023, max compression
+gzip compressed data, was "django-privates-2.0.0.post0.tar", last modified: Sat May  6 14:15:22 2023, max compression
```

## Comparing `django-privates-2.0.0.tar` & `django-privates-2.0.0.post0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-05 16:05:57.000000 django-privates-2.0.0/Changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 16:05:57.000000 django-privates-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 16:05:57.000000 django-privates-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-05 16:06:04.654770 django-privates-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-05 16:05:57.000000 django-privates-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/django_privates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/privates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/storages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.650770 django-privates-2.0.0/privates/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.650770 django-privates-2.0.0/privates/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/privates/templates/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/templates/admin/widgets/clearable_private_file_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-05 16:06:04.654770 django-privates-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:05:57.000000 django-privates-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-05 16:05:57.000000 django-privates-2.0.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-05 16:05:57.000000 django-privates-2.0.0/tests/test_modelfield.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-05 16:05:57.000000 django-privates-2.0.0/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:22.256036 django-privates-2.0.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/Changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-06 14:15:22.256036 django-privates-2.0.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:22.252036 django-privates-2.0.0.post0/django_privates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-06 14:15:22.000000 django-privates-2.0.0.post0/django_privates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-06 14:15:22.000000 django-privates-2.0.0.post0/django_privates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 14:15:22.000000 django-privates-2.0.0.post0/django_privates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 14:15:22.000000 django-privates-2.0.0.post0/django_privates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-06 14:15:22.000000 django-privates-2.0.0.post0/django_privates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 14:15:22.000000 django-privates-2.0.0.post0/django_privates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:22.256036 django-privates-2.0.0.post0/privates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/storages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:22.252036 django-privates-2.0.0.post0/privates/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:22.252036 django-privates-2.0.0.post0/privates/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:22.256036 django-privates-2.0.0.post0/privates/templates/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/templates/admin/widgets/clearable_private_file_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/privates/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-06 14:15:22.256036 django-privates-2.0.0.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:15:22.256036 django-privates-2.0.0.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/tests/test_modelfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-06 14:15:15.000000 django-privates-2.0.0.post0/tests/test_storage.py
```

### Comparing `django-privates-2.0.0/Changelog.rst` & `django-privates-2.0.0.post0/Changelog.rst`

 * *Files identical despite different names*

### Comparing `django-privates-2.0.0/LICENSE` & `django-privates-2.0.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-privates-2.0.0/PKG-INFO` & `django-privates-2.0.0.post0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-privates
-Version: 2.0.0
-Summary: Batteries included private media integration in Django
+Version: 2.0.0.post0
+Summary: Simple private media integration for Django
 Home-page: https://github.com/sergei-maertens/django-privates
 Author: Sergei Maertens
 Author-email: info@regex-it.nl
 Keywords: django,media,private,storage
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -23,62 +23,38 @@
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
-============================================
-Django-privates - private media integrration
-============================================
-
-Django-privates makes it easy to work with login-protected ``FileField``\ s,
-all the way through your application.
-
-:Version: 2.0.0
-:Source: https://github.com/sergei-maertens/django-privates
-:Keywords: django, media, private, storage
+===============
+Django-privates
+===============
 
-|build-status| |linting| |coverage| |docs| |python-versions| |django-versions| |pypi-version|
-
-.. contents::
-
-.. section-numbering::
-
-Features
-========
-
-* Default private media storage, configurable via settings
-* Model field using the default storage
-* Easy admin integration
-* File serving through `sendfile`_ (supports nginx, apache, runserver,...)
+Simple private media integration for Django.
 
+|build-status| |linting| |coverage| |docs| |python-versions| |django-versions| |pypi-version|
 
-Installation
-============
-
-Install
--------
-
-.. code-block:: bash
-
-    pip install django-privates
+What does it do?
+================
 
-And then add ``privates`` to your ``INSTALLED_APPS`` for admin integration (
-template discovery):
+Django supports file uploads for user-generated content out of the box, which is
+typically *public* - think of images, videos...
 
-.. code-block:: python
+However, often you want to expose files only to correctly authenticated users because
+they have a sensitive nature, for example invoice PDFs or tenant-specific documents.
 
-    INSTALLED_APPS = [
-        ...,
+django-privates achieves the latter while being as convenient as Django's core
+``FileField`` and derivatives.
 
-        'privates',
+Usage
+=====
 
-        ...
-    ]
+The installation and usage `documentation`_ is hosted on ReadTheDocs.
 
 
 .. |build-status| image:: https://github.com/sergei-maertens/django-privates/workflows/Run%20CI/badge.svg
     :target: https://github.com/sergei-maertens/django-privates/actions?query=workflow%3A%22Run+CI%22
     :alt: Run CI
 
 .. |linting| image:: https://github.com/sergei-maertens/django-privates/workflows/Code%20quality%20checks/badge.svg
@@ -96,8 +72,8 @@
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-privates.svg
 
 .. |django-versions| image:: https://img.shields.io/pypi/djversions/django-privates.svg
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-privates.svg
     :target: https://pypi.org/project/django-privates/
 
-.. _sendfile: https://pypi.org/project/django-sendfile2/
+.. _documentation: https://django-privates.readthedocs.io/
```

### Comparing `django-privates-2.0.0/django_privates.egg-info/PKG-INFO` & `django-privates-2.0.0.post0/django_privates.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-privates
-Version: 2.0.0
-Summary: Batteries included private media integration in Django
+Version: 2.0.0.post0
+Summary: Simple private media integration for Django
 Home-page: https://github.com/sergei-maertens/django-privates
 Author: Sergei Maertens
 Author-email: info@regex-it.nl
 Keywords: django,media,private,storage
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -23,62 +23,38 @@
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
-============================================
-Django-privates - private media integrration
-============================================
-
-Django-privates makes it easy to work with login-protected ``FileField``\ s,
-all the way through your application.
-
-:Version: 2.0.0
-:Source: https://github.com/sergei-maertens/django-privates
-:Keywords: django, media, private, storage
+===============
+Django-privates
+===============
 
-|build-status| |linting| |coverage| |docs| |python-versions| |django-versions| |pypi-version|
-
-.. contents::
-
-.. section-numbering::
-
-Features
-========
-
-* Default private media storage, configurable via settings
-* Model field using the default storage
-* Easy admin integration
-* File serving through `sendfile`_ (supports nginx, apache, runserver,...)
+Simple private media integration for Django.
 
+|build-status| |linting| |coverage| |docs| |python-versions| |django-versions| |pypi-version|
 
-Installation
-============
-
-Install
--------
-
-.. code-block:: bash
-
-    pip install django-privates
+What does it do?
+================
 
-And then add ``privates`` to your ``INSTALLED_APPS`` for admin integration (
-template discovery):
+Django supports file uploads for user-generated content out of the box, which is
+typically *public* - think of images, videos...
 
-.. code-block:: python
+However, often you want to expose files only to correctly authenticated users because
+they have a sensitive nature, for example invoice PDFs or tenant-specific documents.
 
-    INSTALLED_APPS = [
-        ...,
+django-privates achieves the latter while being as convenient as Django's core
+``FileField`` and derivatives.
 
-        'privates',
+Usage
+=====
 
-        ...
-    ]
+The installation and usage `documentation`_ is hosted on ReadTheDocs.
 
 
 .. |build-status| image:: https://github.com/sergei-maertens/django-privates/workflows/Run%20CI/badge.svg
     :target: https://github.com/sergei-maertens/django-privates/actions?query=workflow%3A%22Run+CI%22
     :alt: Run CI
 
 .. |linting| image:: https://github.com/sergei-maertens/django-privates/workflows/Code%20quality%20checks/badge.svg
@@ -96,8 +72,8 @@
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-privates.svg
 
 .. |django-versions| image:: https://img.shields.io/pypi/djversions/django-privates.svg
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-privates.svg
     :target: https://pypi.org/project/django-privates/
 
-.. _sendfile: https://pypi.org/project/django-sendfile2/
+.. _documentation: https://django-privates.readthedocs.io/
```

### Comparing `django-privates-2.0.0/django_privates.egg-info/SOURCES.txt` & `django-privates-2.0.0.post0/django_privates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-privates-2.0.0/privates/storages.py` & `django-privates-2.0.0.post0/privates/storages.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from django.utils.functional import LazyObject, cached_property
 
 
 class PrivateMediaFileSystemStorage(FileSystemStorage):
     """
     Storage that puts files in the private media folder that isn't
     globally available.
+
+    * ``settings.PRIVATE_MEDIA_ROOT`` is used to determine where to write the files
+    * ``settings.PRIVATE_MEDIA_URL`` is the internal URL used for files.
     """
 
     def _clear_cached_properties(self, setting, **kwargs):
         super()._clear_cached_properties(setting, **kwargs)
         if setting == "PRIVATE_MEDIA_ROOT":
             self.__dict__.pop("base_location", None)
             self.__dict__.pop("location", None)
@@ -25,12 +28,19 @@
     def base_url(self):
         if self._base_url is not None and not self._base_url.endswith("/"):
             self._base_url += "/"
         return self._value_or_setting(self._base_url, settings.PRIVATE_MEDIA_URL)
 
 
 class PrivateMediaStorage(LazyObject):
+    """
+    Lazily initialized :class:`PrivateMediaFileSystemStorage`
+    """
+
     def _setup(self):
         self._wrapped = PrivateMediaFileSystemStorage()
 
 
 private_media_storage = PrivateMediaStorage()
+"""
+A default (lazy) private media storage, configured via Django settings.
+"""
```

### Comparing `django-privates-2.0.0/privates/templates/admin/widgets/clearable_private_file_input.html` & `django-privates-2.0.0.post0/privates/templates/admin/widgets/clearable_private_file_input.html`

 * *Files identical despite different names*

### Comparing `django-privates-2.0.0/privates/views.py` & `django-privates-2.0.0.post0/privates/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,39 @@
+from typing import Optional
+
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from django.views.generic import DetailView
 
 from django_sendfile import sendfile
 
 
 class PrivateMediaView(PermissionRequiredMixin, DetailView):
     """
-    Verify the permission required and send the filefield via sendfile.
+    Verify the required permission and send the filefield content via sendfile.
+
+    The permissions of the user are verified before sending back any data. If the user
+    has the correct permissions, the path of the specified field name is looked up on
+    the object and passed to sendfile, which transforms it into the appropriate response
+    header so the web-server can serve the file contents.
 
     :param permission_required: the permission required to view the file
     :param model: the model class to look up the object
-    :param file_field: the name of the ``Filefield``
     """
 
-    file_field = None
-    # see :func:`sendfile.sendfile` for available parameters
-    sendfile_options = None
+    file_field: str = ""
+    """
+    Name of the file field on the model to look up.
+
+    The path (on-disk) of the file is passed along to :func:`django_sendfile.sendfile`.
+    """
+    sendfile_options: Optional[dict] = None
+    """
+    Additional options for :func:`django_sendfile.sendfile`.
+    """
 
-    def get_sendfile_opts(self):
+    def get_sendfile_opts(self) -> dict:
         return self.sendfile_options or {}
 
     def get(self, request, *args, **kwargs):
         filename = getattr(self.get_object(), self.file_field).path
         sendfile_options = self.get_sendfile_opts()
         return sendfile(request, filename, **sendfile_options)
```

### Comparing `django-privates-2.0.0/privates/widgets.py` & `django-privates-2.0.0.post0/privates/widgets.py`

 * *Files identical despite different names*

### Comparing `django-privates-2.0.0/setup.cfg` & `django-privates-2.0.0.post0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = django-privates
-version = 2.0.0
-description = Batteries included private media integration in Django
+version = 2.0.0-post0
+description = Simple private media integration for Django
 long_description = file: README.rst
 url = https://github.com/sergei-maertens/django-privates
 license = 
 author = Sergei Maertens
 author_email = info@regex-it.nl
 keywords = django, media, private, storage
 classifiers =
```

### Comparing `django-privates-2.0.0/tests/test_admin.py` & `django-privates-2.0.0.post0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-privates-2.0.0/tests/test_storage.py` & `django-privates-2.0.0.post0/tests/test_storage.py`

 * *Files identical despite different names*

