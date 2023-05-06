# Comparing `tmp/aioworkers-sentry-0.3a3.tar.gz` & `tmp/aioworkers-sentry-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aioworkers-sentry-0.3a3.tar", last modified: Sun Nov 10 13:28:43 2019, max compression
+gzip compressed data, was "dist/aioworkers-sentry-0.4.tar", last modified: Sat May  9 00:42:02 2020, max compression
```

## Comparing `aioworkers-sentry-0.3a3.tar` & `aioworkers-sentry-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-10 13:28:43.000000 aioworkers-sentry-0.3a3/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-10 13:28:43.000000 aioworkers-sentry-0.3a3/aioworkers_sentry/
--rw-rw-r--   0 travis    (2000) travis    (2000)      146 2019-11-10 13:27:55.000000 aioworkers-sentry-0.3a3/aioworkers_sentry/sentry.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-11-10 13:28:31.000000 aioworkers-sentry-0.3a3/aioworkers_sentry/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2019-11-10 13:27:55.000000 aioworkers-sentry-0.3a3/aioworkers_sentry/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2190 2019-11-10 13:27:55.000000 aioworkers-sentry-0.3a3/aioworkers_sentry/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2019-11-10 13:27:55.000000 aioworkers-sentry-0.3a3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1979 2019-11-10 13:28:43.000000 aioworkers-sentry-0.3a3/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-10 13:28:43.000000 aioworkers-sentry-0.3a3/aioworkers_sentry.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1979 2019-11-10 13:28:42.000000 aioworkers-sentry-0.3a3/aioworkers_sentry.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-10 13:28:42.000000 aioworkers-sentry-0.3a3/aioworkers_sentry.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2019-11-10 13:28:42.000000 aioworkers-sentry-0.3a3/aioworkers_sentry.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      361 2019-11-10 13:28:42.000000 aioworkers-sentry-0.3a3/aioworkers_sentry.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2019-11-10 13:28:42.000000 aioworkers-sentry-0.3a3/aioworkers_sentry.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2019-11-10 13:28:43.000000 aioworkers-sentry-0.3a3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2019-11-10 13:27:55.000000 aioworkers-sentry-0.3a3/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1451 2019-11-10 13:27:55.000000 aioworkers-sentry-0.3a3/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      155 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/aioworkers_sentry/sentry.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2020-05-09 00:41:49.000000 aioworkers-sentry-0.4/aioworkers_sentry/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/aioworkers_sentry/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2554 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/aioworkers_sentry/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      118 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1985 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1985 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      361 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      371 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      902 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1467 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/setup.py
```

### Comparing `aioworkers-sentry-0.3a3/aioworkers_sentry/client.py` & `aioworkers-sentry-0.4/aioworkers_sentry/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+import multiprocessing
 from typing import Any, Dict, Mapping, Optional
 
 import sentry_sdk
 from aioworkers.core.base import AbstractEntity
 from aioworkers.core.config import ValueExtractor
 from aioworkers.utils import import_name
 
+TAG_PROCESS = 'process'
+
 
 class Sentry(AbstractEntity):
     set_tag = sentry_sdk.set_tag
     set_user = sentry_sdk.set_user
     set_extra = sentry_sdk.set_extra
     start_span = sentry_sdk.start_span
     capture_event = sentry_sdk.capture_event
     capture_message = sentry_sdk.capture_message
     capture_exception = sentry_sdk.capture_exception
     add_breadcrumb = sentry_sdk.add_breadcrumb
     last_event_id = sentry_sdk.last_event_id
 
     _client_config_keys = frozenset({
         'dsn', 'release', 'environment',
+        'with_locals',
         'max_breadcrumbs', 'server_name',
         'shutdown_timeout',
         'in_app_include', 'in_app_exclude',
         'default_integrations', 'dist',
         'sample_rate',
         'send_default_pii',
         'http_proxy',
@@ -60,7 +64,16 @@
                 continue
             factory = import_name(name)
             integrations.append(factory(**params))
         if integrations:
             kwargs.update(integrations=integrations)
         self.client = sentry_sdk.Client(**kwargs)
         sentry_sdk.Hub.main.bind_client(self.client)
+
+    async def init(self):
+        await super().init()
+        tags = self.config.get('tags')
+        if isinstance(tags, list):
+            if TAG_PROCESS in tags:
+                sentry_sdk.set_tag(
+                    TAG_PROCESS, multiprocessing.current_process().name,
+                )
```

### Comparing `aioworkers-sentry-0.3a3/PKG-INFO` & `aioworkers-sentry-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aioworkers-sentry
-Version: 0.3a3
+Version: 0.4
 Summary: aioworkers plugin for Sentry
 Home-page: https://github.com/aioworkers/aioworkers-sentry
 Author: Alexander Bogushov
 Author-email: abogushov@gmail.com
 License: Apache Software License 2.0
 Description: aioworkers-sentry
         =================
@@ -56,14 +56,14 @@
         
         .. code-block:: shell
         
             pipenv run pytest
         
 Keywords: aioworkers sentry
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aioworkers-sentry-0.3a3/aioworkers_sentry.egg-info/PKG-INFO` & `aioworkers-sentry-0.4/aioworkers_sentry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aioworkers-sentry
-Version: 0.3a3
+Version: 0.4
 Summary: aioworkers plugin for Sentry
 Home-page: https://github.com/aioworkers/aioworkers-sentry
 Author: Alexander Bogushov
 Author-email: abogushov@gmail.com
 License: Apache Software License 2.0
 Description: aioworkers-sentry
         =================
@@ -56,14 +56,14 @@
         
         .. code-block:: shell
         
             pipenv run pytest
         
 Keywords: aioworkers sentry
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aioworkers-sentry-0.3a3/README.rst` & `aioworkers-sentry-0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aioworkers-sentry-0.3a3/setup.py` & `aioworkers-sentry-0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 version = __import__('aioworkers_sentry').__version__
 
 requirements = [
     'aioworkers>=0.13',
-    'sentry_sdk',
+    'sentry_sdk>=0.14.3',
 ]
 
 if sys.version_info < (3, 7):
     requirements.append('aiocontextvars')
 
 test_requirements = [
     'pytest',
@@ -41,15 +41,15 @@
         i for i in find_packages() if i.startswith('aioworkers_sentry')
     ],
     include_package_data=True,
     install_requires=requirements,
     license='Apache Software License 2.0',
     keywords='aioworkers sentry',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
```

