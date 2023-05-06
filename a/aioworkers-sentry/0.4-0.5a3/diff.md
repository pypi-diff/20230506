# Comparing `tmp/aioworkers-sentry-0.4.tar.gz` & `tmp/aioworkers_sentry-0.5a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aioworkers-sentry-0.4.tar", last modified: Sat May  9 00:42:02 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aioworkers-sentry-0.4.tar` & `aioworkers_sentry-0.5a3.tar`

### file list

```diff
@@ -1,17 +1,8 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry/
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/aioworkers_sentry/sentry.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2020-05-09 00:41:49.000000 aioworkers-sentry-0.4/aioworkers_sentry/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/aioworkers_sentry/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2554 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/aioworkers_sentry/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1985 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1985 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      361 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/aioworkers_sentry.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2020-05-09 00:42:02.000000 aioworkers-sentry-0.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1467 2020-05-09 00:41:17.000000 aioworkers-sentry-0.4/setup.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioworkers_sentry-0.5a3/aioworkers_sentry/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 aioworkers_sentry-0.5a3/aioworkers_sentry/client.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aioworkers_sentry-0.5a3/aioworkers_sentry/sentry.ini
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 aioworkers_sentry-0.5a3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aioworkers_sentry-0.5a3/LICENSE
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aioworkers_sentry-0.5a3/README.rst
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 aioworkers_sentry-0.5a3/pyproject.toml
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 aioworkers_sentry-0.5a3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aioworkers-sentry-0.4/PKG-INFO` & `aioworkers_sentry-0.5a3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,98 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aioworkers-sentry
-Version: 0.4
+Version: 0.5a3
 Summary: aioworkers plugin for Sentry
-Home-page: https://github.com/aioworkers/aioworkers-sentry
-Author: Alexander Bogushov
-Author-email: abogushov@gmail.com
-License: Apache Software License 2.0
-Description: aioworkers-sentry
-        =================
-        
-        .. image:: https://travis-ci.org/aioworkers/aioworkers-sentry.svg?branch=master
-          :target: https://travis-ci.org/aioworkers/aioworkers-sentry
-        
-        .. image:: https://img.shields.io/pypi/v/aioworkers-sentry.svg
-          :target: https://pypi.python.org/pypi/aioworkers-sentry
-        
-        
-        aioworkers plugin to work with Sentry. Creates Sentry client and handler according configuration
-        and setup logging.
-        
-        Usage
-        -----
-        
-        Install plugin:
-        
-        .. code-block:: shell
-        
-            pip install aioworkers-sentry
-        
-        
-        Add to your config:
-        
-        .. code-block:: yaml
-        
-            sentry:
-                dsn: <your sentry dsn>
-                release: 1.0.0
-                environment: DEV
-                integrations:
-                  - sentry_sdk.integrations.aiohttp.AioHttpIntegration
-        
-        
-        Development
-        -----------
-        
-        Install dev requirements:
-        
-        
-        .. code-block:: shell
-        
-            pipenv install --dev --skip-lock
-        
-        
-        Run tests:
-        
-        .. code-block:: shell
-        
-            pipenv run pytest
-        
-Keywords: aioworkers sentry
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/aioworkers/aioworkers-sentry
+Project-URL: Documentation, https://github.com/aioworkers/aioworkers-sentry
+Project-URL: Issues, https://github.com/aioworkers/aioworkers-sentry/issues
+Project-URL: Source, https://github.com/aioworkers/aioworkers-sentry
+Author-email: Alexander Bogushov <abogushov@gmail.com>, Alexander Malev <malev@somedev.ru>
+License-Expression: Apache-2.0
+License-File: LICENSE
+Keywords: aioworkers,sentry
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Requires-Dist: aioworkers>=0.13
+Requires-Dist: sentry-sdk>=1.22
+Description-Content-Type: text/x-rst
+
+aioworkers-sentry
+=================
+
+.. image:: https://github.com/aioworkers/aioworkers-sentry/workflows/Tests/badge.svg
+  :target: https://github.com/aioworkers/aioworkers-sentry/actions?query=workflow%3ATests
+
+.. image:: https://codecov.io/gh/aioworkers/aioworkers-sentry/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/aioworkers/aioworkers-sentry
+
+.. image:: https://img.shields.io/pypi/v/aioworkers-sentry.svg
+  :target: https://pypi.org/project/aioworkers-sentry
+
+.. image:: https://img.shields.io/pypi/pyversions/aioworkers-sentry.svg
+  :target: https://pypi.org/project/aioworkers-sentry
+  :alt: Python versions
+
+.. image:: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
+   :alt: Hatch project
+   :target: https://github.com/pypa/hatch
+
+
+aioworkers plugin to work with Sentry. Creates Sentry client and handler according configuration
+and setup logging.
+
+Usage
+-----
+
+Install plugin:
+
+.. code-block:: shell
+
+    pip install aioworkers-sentry
+
+
+Add to your config:
+
+.. code-block:: yaml
+
+    sentry:
+        dsn: <your sentry dsn>
+        release: 1.0.0
+        environment: DEV
+        integrations:
+          - sentry_sdk.integrations.aiohttp.AioHttpIntegration
+
+
+Development
+-----------
+
+Format code:
+
+.. code-block:: shell
+
+    hatch run style:fmt
+
+
+Run tests:
+
+.. code-block:: shell
+
+    hatch run pytest
+
+
+Run tests with coverage:
+
+.. code-block:: shell
+
+    hatch run cov
```

