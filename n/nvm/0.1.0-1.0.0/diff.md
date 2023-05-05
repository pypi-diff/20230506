# Comparing `tmp/nvm-0.1.0.tar.gz` & `tmp/nvm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvm-0.1.0.tar", last modified: Fri May  5 21:34:42 2023, max compression
+gzip compressed data, was "nvm-1.0.0.tar", last modified: Fri May  5 22:31:11 2023, max compression
```

## Comparing `nvm-0.1.0.tar` & `nvm-1.0.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-0.1.0/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-0.1.0/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/.github/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/.github/ISSUE_TEMPLATE/
--rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/.github/workflows/
--rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-0.1.0/.github/workflows/build-main.yml
--rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-0.1.0/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-0.1.0/.readthedocs.yaml
--rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-0.1.0/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-0.1.0/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-0.1.0/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-0.1.0/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-0.1.0/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     3032 2023-05-03 20:09:42.000000 nvm-0.1.0/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     2048 2023-05-05 21:34:42.970808 nvm-0.1.0/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1081 2023-05-05 21:31:52.000000 nvm-0.1.0/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/bin/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.1.0/bin/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-0.1.0/bin/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.1.0/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-0.1.0/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-0.1.0/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.962808 nvm-0.1.0/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.962808 nvm-0.1.0/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-0.1.0/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-0.1.0/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.962808 nvm-0.1.0/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-0.1.0/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-0.1.0/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-0.1.0/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      588 2023-05-05 19:42:21.000000 nvm-0.1.0/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/authors.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5541 2023-05-04 00:55:18.000000 nvm-0.1.0/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-05 19:03:25.000000 nvm-0.1.0/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-04 00:48:09.000000 nvm-0.1.0/docs/source/nvm.aux_log.rst
--rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-05 13:07:38.000000 nvm-0.1.0/docs/source/nvm.aux_pandas.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 20:38:41.000000 nvm-0.1.0/docs/source/nvm.aux_str.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 23:04:50.000000 nvm-0.1.0/docs/source/nvm.aux_sys.rst
--rw-------   0 jiko      (1000) jiko      (1000)      384 2023-05-05 19:03:25.000000 nvm-0.1.0/docs/source/nvm.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/usage.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/
--rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 19:45:20.000000 nvm-0.1.0/nvm/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/_version.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/aux_log/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-0.1.0/nvm/aux_log/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-0.1.0/nvm/aux_log/aux_log.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/aux_pandas/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      105 2023-05-04 02:17:41.000000 nvm-0.1.0/nvm/aux_pandas/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1590 2023-05-05 18:55:20.000000 nvm-0.1.0/nvm/aux_pandas/aux_pandas.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/aux_str/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      179 2023-05-05 15:19:07.000000 nvm-0.1.0/nvm/aux_str/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     3135 2023-05-05 21:16:37.000000 nvm-0.1.0/nvm/aux_str/aux_str.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1790 2023-05-05 15:15:18.000000 nvm-0.1.0/nvm/aux_str/clean_str_mappings.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/aux_sys/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-03 23:08:53.000000 nvm-0.1.0/nvm/aux_sys/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1342 2023-05-05 19:03:51.000000 nvm-0.1.0/nvm/aux_sys/aux_sys.py
--rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-0.1.0/nvm/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     2048 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1635 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/top_level.txt
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-0.1.0/pyproject.toml
--rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 21:20:43.000000 nvm-0.1.0/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      673 2023-05-05 21:34:42.970808 nvm-0.1.0/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-03 18:32:02.000000 nvm-0.1.0/setup.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-0.1.0/tests/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1563 2023-05-05 15:01:56.000000 nvm-0.1.0/tests/test_aux_str.py
--rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-0.1.0/tests/test_nvm.py
--rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-0.1.0/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-0.1.0/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.933110 nvm-1.0.0/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-1.0.0/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-1.0.0/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.925110 nvm-1.0.0/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.925110 nvm-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.925110 nvm-1.0.0/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-1.0.0/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-1.0.0/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-1.0.0/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-1.0.0/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-1.0.0/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-1.0.0/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-1.0.0/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-1.0.0/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     3032 2023-05-03 20:09:42.000000 nvm-1.0.0/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     2048 2023-05-05 22:31:11.933110 nvm-1.0.0/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1081 2023-05-05 21:31:52.000000 nvm-1.0.0/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.925110 nvm-1.0.0/bin/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.0/bin/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-1.0.0/bin/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.925110 nvm-1.0.0/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.0/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.925110 nvm-1.0.0/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-1.0.0/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-1.0.0/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.925110 nvm-1.0.0/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.921110 nvm-1.0.0/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.921110 nvm-1.0.0/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.929110 nvm-1.0.0/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-1.0.0/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-1.0.0/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.921110 nvm-1.0.0/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.929110 nvm-1.0.0/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-1.0.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-1.0.0/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.0/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.0/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      588 2023-05-05 19:42:21.000000 nvm-1.0.0/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.929110 nvm-1.0.0/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.929110 nvm-1.0.0/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/source/authors.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5541 2023-05-04 00:55:18.000000 nvm-1.0.0/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-05 22:29:53.000000 nvm-1.0.0/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-04 00:48:09.000000 nvm-1.0.0/docs/source/nvm.aux_log.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-05 13:07:38.000000 nvm-1.0.0/docs/source/nvm.aux_pandas.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 20:38:41.000000 nvm-1.0.0/docs/source/nvm.aux_str.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 23:04:50.000000 nvm-1.0.0/docs/source/nvm.aux_sys.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      384 2023-05-05 22:29:53.000000 nvm-1.0.0/docs/source/nvm.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-1.0.0/docs/source/usage.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.933110 nvm-1.0.0/nvm/
+-rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 19:45:20.000000 nvm-1.0.0/nvm/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-05 22:31:11.933110 nvm-1.0.0/nvm/_version.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.933110 nvm-1.0.0/nvm/aux_log/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-1.0.0/nvm/aux_log/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-1.0.0/nvm/aux_log/aux_log.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.933110 nvm-1.0.0/nvm/aux_pandas/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      105 2023-05-04 02:17:41.000000 nvm-1.0.0/nvm/aux_pandas/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1590 2023-05-05 18:55:20.000000 nvm-1.0.0/nvm/aux_pandas/aux_pandas.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.933110 nvm-1.0.0/nvm/aux_str/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      179 2023-05-05 15:19:07.000000 nvm-1.0.0/nvm/aux_str/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     4940 2023-05-05 22:28:32.000000 nvm-1.0.0/nvm/aux_str/aux_str.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1789 2023-05-05 22:20:16.000000 nvm-1.0.0/nvm/aux_str/clean_str_mappings.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.933110 nvm-1.0.0/nvm/aux_sys/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-03 23:08:53.000000 nvm-1.0.0/nvm/aux_sys/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1342 2023-05-05 19:03:51.000000 nvm-1.0.0/nvm/aux_sys/aux_sys.py
+-rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-1.0.0/nvm/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.933110 nvm-1.0.0/nvm.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     2048 2023-05-05 22:31:11.000000 nvm-1.0.0/nvm.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1635 2023-05-05 22:31:11.000000 nvm-1.0.0/nvm.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 22:31:11.000000 nvm-1.0.0/nvm.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-05 22:31:11.000000 nvm-1.0.0/nvm.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 22:31:11.000000 nvm-1.0.0/nvm.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-05 22:31:11.000000 nvm-1.0.0/nvm.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-05 22:31:11.000000 nvm-1.0.0/nvm.egg-info/top_level.txt
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-1.0.0/pyproject.toml
+-rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 21:20:43.000000 nvm-1.0.0/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      673 2023-05-05 22:31:11.933110 nvm-1.0.0/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-05 21:35:05.000000 nvm-1.0.0/setup.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:31:11.933110 nvm-1.0.0/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-1.0.0/tests/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1563 2023-05-05 15:01:56.000000 nvm-1.0.0/tests/test_aux_str.py
+-rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-1.0.0/tests/test_nvm.py
+-rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-1.0.0/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-1.0.0/versioneer.py
```

### Comparing `nvm-0.1.0/.github/workflows/build-main.yml` & `nvm-1.0.0/.github/workflows/build-main.yml`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/.gitignore` & `nvm-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/.readthedocs.yaml` & `nvm-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/CONTRIBUTING.rst` & `nvm-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/LICENSE` & `nvm-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/Makefile` & `nvm-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/PKG-INFO` & `nvm-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 0.1.0
+Version: 1.0.0
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-0.1.0/README.rst` & `nvm-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/data/emacs-logo/emacs-128x128.png` & `nvm-1.0.0/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/data/emacs-logo/emacs.svg` & `nvm-1.0.0/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/docs/Makefile` & `nvm-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `nvm-1.0.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/docs/requirements.txt` & `nvm-1.0.0/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/docs/source/conf.py` & `nvm-1.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/docs/source/installation.rst` & `nvm-1.0.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/nvm/aux_log/aux_log.py` & `nvm-1.0.0/nvm/aux_log/aux_log.py`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/nvm/aux_pandas/aux_pandas.py` & `nvm-1.0.0/nvm/aux_pandas/aux_pandas.py`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/nvm/aux_str/clean_str_mappings.py` & `nvm-1.0.0/nvm/aux_str/clean_str_mappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 CLEAN_STR_MAPPINGS_TINY = [
     {
         " ": [  # Unicode Character 'SPACE' (U+0020)
             "\n",  # LF (Line Feed)
             "\r",  # CR (Carriage Return)
-            "\t",  # TAB (Horizontal Tab)
+            "\t",  # HT (Horizontal Tab)
         ],
     },
     {
         "-": [  # Unicode Character 'HYPHEN-MINUS' (U+002D) # chr(45) ord("-") ord("\u002D")
             "\u2212",  # Unicode Character 'MINUS SIGN' (U+2212)
             "\u2013",  # Unicode Character 'EN DASH' (U+2013) # chr(8211) ↔ ord("–") ↔ ord("\u2013")
             "\u2014",  # Unicode Character 'EM DASH' (U+2014)
```

### Comparing `nvm-0.1.0/nvm/aux_sys/aux_sys.py` & `nvm-1.0.0/nvm/aux_sys/aux_sys.py`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/nvm.egg-info/PKG-INFO` & `nvm-1.0.0/nvm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 0.1.0
+Version: 1.0.0
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-0.1.0/nvm.egg-info/SOURCES.txt` & `nvm-1.0.0/nvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/nvm.egg-info/requires.txt` & `nvm-1.0.0/nvm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/pyproject.toml` & `nvm-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/setup.cfg` & `nvm-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/setup.py` & `nvm-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/tests/test_aux_str.py` & `nvm-1.0.0/tests/test_aux_str.py`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/tests/test_nvm.py` & `nvm-1.0.0/tests/test_nvm.py`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/tox.ini` & `nvm-1.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `nvm-0.1.0/versioneer.py` & `nvm-1.0.0/versioneer.py`

 * *Files identical despite different names*

