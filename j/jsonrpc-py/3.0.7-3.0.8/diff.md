# Comparing `tmp/jsonrpc-py-3.0.7.tar.gz` & `tmp/jsonrpc-py-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.7.tar", last modified: Wed May  3 09:14:02 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.8.tar", last modified: Sat May  6 14:57:44 2023, max compression
```

## Comparing `jsonrpc-py-3.0.7.tar` & `jsonrpc-py-3.0.8.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.022167 jsonrpc-py-3.0.7/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/Makefile
--rw-r--r--   0 root         (0) root         (0)     2852 2023-05-03 09:14:02.021167 jsonrpc-py-3.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:01.998165 jsonrpc-py-3.0.7/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:01.992165 jsonrpc-py-3.0.7/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.003166 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.010166 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.013166 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/docs/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.017166 jsonrpc-py-3.0.7/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9423 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.018167 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2852 2023-05-03 09:14:01.000000 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1988 2023-05-03 09:14:01.000000 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 09:14:01.000000 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-03 09:14:01.000000 jsonrpc-py-3.0.7/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 09:14:02.022167 jsonrpc-py-3.0.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 09:14:02.021167 jsonrpc-py-3.0.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13819 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     5717 2023-05-03 09:13:38.000000 jsonrpc-py-3.0.7/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.445853 jsonrpc-py-3.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-05-06 14:57:44.444853 jsonrpc-py-3.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.421851 jsonrpc-py-3.0.8/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.414850 jsonrpc-py-3.0.8/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.424851 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.432852 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.435852 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.439853 jsonrpc-py-3.0.8/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9422 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3300 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4098 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.441853 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-05-06 14:57:44.000000 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-05-06 14:57:44.000000 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 14:57:44.000000 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-06 14:57:44.000000 jsonrpc-py-3.0.8/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 14:57:44.445853 jsonrpc-py-3.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 14:57:44.444853 jsonrpc-py-3.0.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13819 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2023-05-06 14:57:19.000000 jsonrpc-py-3.0.8/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.7/.gitlab-ci.yml` & `jsonrpc-py-3.0.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/LICENSE` & `jsonrpc-py-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/Makefile` & `jsonrpc-py-3.0.8/Makefile`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/PKG-INFO` & `jsonrpc-py-3.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.7
+Version: 3.0.8
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
+Project-URL: Homepage, https://docs.jsonrpc.ru
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `jsonrpc-py-3.0.7/README.md` & `jsonrpc-py-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc-py-3.0.8/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc-py-3.0.8/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc-py-3.0.8/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/changelog.rst` & `jsonrpc-py-3.0.8/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/conf.py` & `jsonrpc-py-3.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/deployment.rst` & `jsonrpc-py-3.0.8/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/index.rst` & `jsonrpc-py-3.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/quickstart.rst` & `jsonrpc-py-3.0.8/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/docs/reference.rst` & `jsonrpc-py-3.0.8/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/jsonrpc/__init__.py` & `jsonrpc-py-3.0.8/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/jsonrpc/asgi.py` & `jsonrpc-py-3.0.8/jsonrpc/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             try:
                 result: Any = await shield(task)
                 return Response(body=result, response_id=request.request_id)
             except Error as error:
                 return Response(error=error, response_id=request.request_id)
 
         async def on_batch_request(request: BatchRequest) -> BatchResponse:
-            responses: list[AnyResponse] = await multiple_coroutines(map(self.process_request, request))
+            responses: tuple[AnyResponse, ...] = await multiple_coroutines(map(self.process_request, request))
             return BatchResponse([response for response in responses if isinstance(response, Response)])
 
         if isinstance(obj, Error):
             return on_error(obj)
         elif isinstance(obj, Request):
             return await on_request(obj)
         else:
@@ -241,10 +241,10 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}({self.data!r})"
 
     async def __call__(self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable) -> None:
         match scope:
             case {"type": "http", **kwargs}:  # noqa: F841
-                return await HTTPHandler(scope, receive, send, self.__class__)  # type: ignore[arg-type]
+                await HTTPHandler(scope, receive, send, self.__class__)  # type: ignore[arg-type]
             case _:
                 raise ValueError("Only ASGI/HTTP connections are allowed.")
```

### Comparing `jsonrpc-py-3.0.7/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.8/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/jsonrpc/errors.py` & `jsonrpc-py-3.0.8/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/jsonrpc/request.py` & `jsonrpc-py-3.0.8/jsonrpc/request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/jsonrpc/response.py` & `jsonrpc-py-3.0.8/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/jsonrpc/serializer.py` & `jsonrpc-py-3.0.8/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/jsonrpc/utilities.py` & `jsonrpc-py-3.0.8/jsonrpc/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,59 +54,56 @@
         #: ---
         #: Non-hashable, non-iterable:
         raise
 
     return obj
 
 
-@dataclass(eq=False, slots=True)
+@dataclass(repr=False, eq=False, slots=True)
 class multiple_coroutines(Generic[T]):
     coroutines: Iterable[CoroutineLike[T]]
-    results: list[tuple[int, T]] = field(default_factory=list, init=False)
+    queue: list[tuple[int, T]] = field(default_factory=list, init=False)
 
-    def __repr__(self) -> str:
-        return f"{self.__class__.__qualname__}({self.coroutines!r})"
-
-    def __await__(self) -> Generator[Any, None, list[T]]:
+    def __await__(self) -> Generator[Any, None, tuple[T, ...]]:
         #: ---
         #: Create a suitable iterator by calling __await__ on a coroutine.
         return self.__await_impl__().__await__()
 
-    async def __await_impl__(self) -> list[T]:
+    async def __await_impl__(self) -> tuple[T, ...]:
         context: Final[Context] = copy_context()
         try:
             async with TaskGroup() as tg:
-                for priority, coroutine in enumerate(self.coroutines):
+                for task_id, coroutine in enumerate(self.coroutines):
                     task: Task[T] = tg.create_task(coroutine, context=context)
-                    callback: partial[None] = partial(self.populate_results, priority=priority)
+                    callback: partial[None] = partial(self.populate_results, task_id=task_id)
                     task.add_done_callback(callback, context=context)
         except BaseExceptionGroup as exc_group:
             #: ---
             #: Propagate the first raised exception from exception group:
-            exc, *_ = self.exception_from_group(exc_group)
-            raise exc from None
+            for exc in self.exception_from_group(exc_group):
+                raise exc from None
 
-        return list(self.iter_results())
+        return tuple(self.iter_results())
 
-    def populate_results(self, task: Task[T], *, priority: int) -> None:
+    def populate_results(self, task: Task[T], *, task_id: int) -> None:
         if not task.cancelled() and task.exception() is None:
             result: Final[T] = task.result()
-            heappush(self.results, (priority, result))
+            heappush(self.queue, (task_id, result))
 
     def exception_from_group(self, exc: BaseException) -> Iterator[BaseException]:
-        if isinstance(exc_group := exc, BaseExceptionGroup):
-            for nested in exc_group.exceptions:
+        if isinstance(exc, BaseExceptionGroup):
+            for nested in exc.exceptions:
                 yield from self.exception_from_group(nested)
         else:
             yield exc
 
     def iter_results(self) -> Iterator[T]:
         while True:
             try:
-                _, result = heappop(self.results)
+                _, result = heappop(self.queue)
                 yield result
             except IndexError:
                 break
 
 
 @final
 class UndefinedType:
```

### Comparing `jsonrpc-py-3.0.7/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.8/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.7
+Version: 3.0.8
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
+Project-URL: Homepage, https://docs.jsonrpc.ru
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `jsonrpc-py-3.0.7/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.0.8/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 docs/changelog/v3.x.x/v3.0.1.rst
 docs/changelog/v3.x.x/v3.0.2.rst
 docs/changelog/v3.x.x/v3.0.3.rst
 docs/changelog/v3.x.x/v3.0.4.rst
 docs/changelog/v3.x.x/v3.0.5.rst
 docs/changelog/v3.x.x/v3.0.6.rst
 docs/changelog/v3.x.x/v3.0.7.rst
+docs/changelog/v3.x.x/v3.0.8.rst
 jsonrpc/__init__.py
 jsonrpc/asgi.py
 jsonrpc/dispatcher.py
 jsonrpc/errors.py
 jsonrpc/py.typed
 jsonrpc/request.py
 jsonrpc/response.py
```

### Comparing `jsonrpc-py-3.0.7/pyproject.toml` & `jsonrpc-py-3.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 name = "JSON-RPC Development Group"
 email = "dev@jsonrpc.ru"
 
 [project.license]
 text = "BSD-3-Clause"
 
 [project.urls]
+"Homepage" = "https://docs.jsonrpc.ru"
 "Source Code" = "https://gitlab.com/jsonrpc/jsonrpc-py"
 "Documentation" = "https://docs.jsonrpc.ru"
 "Change Log" = "https://docs.jsonrpc.ru/changelog.html"
 
 [tool.black]
 line_length = 140
 preview = true
```

### Comparing `jsonrpc-py-3.0.7/tests/test_asgi.py` & `jsonrpc-py-3.0.8/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/tests/test_dispatcher.py` & `jsonrpc-py-3.0.8/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/tests/test_errors.py` & `jsonrpc-py-3.0.8/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/tests/test_request.py` & `jsonrpc-py-3.0.8/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/tests/test_response.py` & `jsonrpc-py-3.0.8/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/tests/test_serializer.py` & `jsonrpc-py-3.0.8/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.7/tests/test_utilities.py` & `jsonrpc-py-3.0.8/tests/test_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from asyncio import create_task, sleep, wait_for
-from collections.abc import MutableSequence
 from typing import Any, Literal, NoReturn
 from unittest import IsolatedAsyncioTestCase, TestCase
 from unittest.mock import AsyncMock, MagicMock, sentinel
 
 from jsonrpc.utilities import Undefined, UndefinedType, ensure_async, make_hashable, multiple_coroutines
 
 
@@ -68,32 +67,31 @@
 
     async def test_multiple_coroutines(self) -> None:
         mocks: set[AsyncMock] = {AsyncMock(return_value=i) for i in ("a", "b", "c")}
 
         async def inner(mock: AsyncMock) -> Any:
             return await mock()
 
-        results: list[str] = await multiple_coroutines(map(inner, mocks))
-        self.assertIsInstance(results, MutableSequence)
-        self.assertCountEqual(results, ["a", "b", "c"])
+        results: tuple[str, ...] = await multiple_coroutines(map(inner, mocks))
+        self.assertCountEqual(results, ("a", "b", "c"))
 
         for mock in mocks:
             with self.subTest(mock=mock):
                 mock.assert_awaited_once()
 
     async def test_multiple_coroutines_preserved_order(self) -> None:
-        results: list[str] = await multiple_coroutines(
+        results: tuple[str, ...] = await multiple_coroutines(
             (
                 sleep(0.04, "a"),  # <-- accepted latest but should be first in results
                 sleep(0.02, "b"),  # <-- accepted second and should be second in results
                 sleep(0.01, "c"),  # <-- accepted first but should be third in results
                 sleep(0.03, "d"),  # <-- accepted third but should be latest in results
             )
         )
-        self.assertListEqual(results, ["a", "b", "c", "d"])
+        self.assertTupleEqual(results, ("a", "b", "c", "d"))
 
     async def test_multiple_coroutines_exception(self) -> None:
         first_exception_mock: AsyncMock = AsyncMock(side_effect=Exception("first exception"))
         second_exception_mock: AsyncMock = AsyncMock(side_effect=Exception("second exception"))
 
         async def inner(mock: AsyncMock) -> Any:
             return await mock()
```

