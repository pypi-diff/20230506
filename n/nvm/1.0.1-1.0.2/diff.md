# Comparing `tmp/nvm-1.0.1.tar.gz` & `tmp/nvm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvm-1.0.1.tar", last modified: Fri May  5 22:54:36 2023, max compression
+gzip compressed data, was "nvm-1.0.2.tar", last modified: Fri May  5 23:09:08 2023, max compression
```

## Comparing `nvm-1.0.1.tar` & `nvm-1.0.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.070642 nvm-1.0.1/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-1.0.1/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-1.0.1/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.062642 nvm-1.0.1/.github/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.062642 nvm-1.0.1/.github/ISSUE_TEMPLATE/
--rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-1.0.1/.github/PULL_REQUEST_TEMPLATE.md
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.062642 nvm-1.0.1/.github/workflows/
--rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-1.0.1/.github/workflows/build-main.yml
--rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-1.0.1/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-1.0.1/.readthedocs.yaml
--rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-1.0.1/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-1.0.1/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-1.0.1/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-1.0.1/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-1.0.1/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     3032 2023-05-03 20:09:42.000000 nvm-1.0.1/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     2171 2023-05-05 22:54:36.070642 nvm-1.0.1/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1204 2023-05-05 22:49:04.000000 nvm-1.0.1/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.062642 nvm-1.0.1/bin/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.1/bin/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-1.0.1/bin/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.062642 nvm-1.0.1/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.1/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.062642 nvm-1.0.1/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-1.0.1/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-1.0.1/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.062642 nvm-1.0.1/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.058642 nvm-1.0.1/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.058642 nvm-1.0.1/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.066642 nvm-1.0.1/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-1.0.1/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-1.0.1/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.058642 nvm-1.0.1/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.066642 nvm-1.0.1/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-1.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-1.0.1/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.1/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.1/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      588 2023-05-05 19:42:21.000000 nvm-1.0.1/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.066642 nvm-1.0.1/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.066642 nvm-1.0.1/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/source/authors.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5541 2023-05-04 00:55:18.000000 nvm-1.0.1/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-05 22:49:54.000000 nvm-1.0.1/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-04 00:48:09.000000 nvm-1.0.1/docs/source/nvm.aux_log.rst
--rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-05 13:07:38.000000 nvm-1.0.1/docs/source/nvm.aux_pandas.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 20:38:41.000000 nvm-1.0.1/docs/source/nvm.aux_str.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 23:04:50.000000 nvm-1.0.1/docs/source/nvm.aux_sys.rst
--rw-------   0 jiko      (1000) jiko      (1000)      384 2023-05-05 22:49:54.000000 nvm-1.0.1/docs/source/nvm.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-1.0.1/docs/source/usage.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.070642 nvm-1.0.1/nvm/
--rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 19:45:20.000000 nvm-1.0.1/nvm/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-05 22:54:36.070642 nvm-1.0.1/nvm/_version.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.070642 nvm-1.0.1/nvm/aux_log/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-1.0.1/nvm/aux_log/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-1.0.1/nvm/aux_log/aux_log.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.070642 nvm-1.0.1/nvm/aux_pandas/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      105 2023-05-04 02:17:41.000000 nvm-1.0.1/nvm/aux_pandas/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1590 2023-05-05 18:55:20.000000 nvm-1.0.1/nvm/aux_pandas/aux_pandas.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.070642 nvm-1.0.1/nvm/aux_str/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      179 2023-05-05 15:19:07.000000 nvm-1.0.1/nvm/aux_str/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     4940 2023-05-05 22:28:32.000000 nvm-1.0.1/nvm/aux_str/aux_str.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1789 2023-05-05 22:20:16.000000 nvm-1.0.1/nvm/aux_str/clean_str_mappings.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.070642 nvm-1.0.1/nvm/aux_sys/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-03 23:08:53.000000 nvm-1.0.1/nvm/aux_sys/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1342 2023-05-05 19:03:51.000000 nvm-1.0.1/nvm/aux_sys/aux_sys.py
--rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-1.0.1/nvm/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.070642 nvm-1.0.1/nvm.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     2171 2023-05-05 22:54:35.000000 nvm-1.0.1/nvm.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1635 2023-05-05 22:54:36.000000 nvm-1.0.1/nvm.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 22:54:35.000000 nvm-1.0.1/nvm.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-05 22:54:35.000000 nvm-1.0.1/nvm.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 22:54:35.000000 nvm-1.0.1/nvm.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-05 22:54:35.000000 nvm-1.0.1/nvm.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-05 22:54:35.000000 nvm-1.0.1/nvm.egg-info/top_level.txt
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-1.0.1/pyproject.toml
--rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 21:20:43.000000 nvm-1.0.1/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      673 2023-05-05 22:54:36.070642 nvm-1.0.1/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-05 21:35:05.000000 nvm-1.0.1/setup.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 22:54:36.070642 nvm-1.0.1/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-1.0.1/tests/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1563 2023-05-05 15:01:56.000000 nvm-1.0.1/tests/test_aux_str.py
--rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-1.0.1/tests/test_nvm.py
--rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-1.0.1/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-1.0.1/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-1.0.2/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-1.0.2/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.928891 nvm-1.0.2/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.928891 nvm-1.0.2/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-1.0.2/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.928891 nvm-1.0.2/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-1.0.2/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-1.0.2/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-1.0.2/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-1.0.2/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-1.0.2/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       69 2023-05-05 23:01:31.000000 nvm-1.0.2/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-1.0.2/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-1.0.2/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     3032 2023-05-03 20:09:42.000000 nvm-1.0.2/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     2146 2023-05-05 23:09:08.932891 nvm-1.0.2/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1199 2023-05-05 23:07:41.000000 nvm-1.0.2/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.928891 nvm-1.0.2/bin/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.2/bin/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-1.0.2/bin/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.2/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-1.0.2/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-1.0.2/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.928891 nvm-1.0.2/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.928891 nvm-1.0.2/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-1.0.2/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-1.0.2/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.928891 nvm-1.0.2/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-1.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-1.0.2/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.2/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.2/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      588 2023-05-05 19:42:21.000000 nvm-1.0.2/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/source/authors.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5541 2023-05-04 00:55:18.000000 nvm-1.0.2/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-05 23:08:53.000000 nvm-1.0.2/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-04 00:48:09.000000 nvm-1.0.2/docs/source/nvm.aux_log.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-05 13:07:38.000000 nvm-1.0.2/docs/source/nvm.aux_pandas.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 20:38:41.000000 nvm-1.0.2/docs/source/nvm.aux_str.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 23:04:50.000000 nvm-1.0.2/docs/source/nvm.aux_sys.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      384 2023-05-05 23:08:53.000000 nvm-1.0.2/docs/source/nvm.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-1.0.2/docs/source/usage.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/nvm/
+-rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 19:45:20.000000 nvm-1.0.2/nvm/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-05 23:09:08.932891 nvm-1.0.2/nvm/_version.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/nvm/aux_log/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-1.0.2/nvm/aux_log/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-1.0.2/nvm/aux_log/aux_log.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/nvm/aux_pandas/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      105 2023-05-04 02:17:41.000000 nvm-1.0.2/nvm/aux_pandas/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1590 2023-05-05 18:55:20.000000 nvm-1.0.2/nvm/aux_pandas/aux_pandas.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/nvm/aux_str/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      179 2023-05-05 15:19:07.000000 nvm-1.0.2/nvm/aux_str/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5209 2023-05-05 22:58:41.000000 nvm-1.0.2/nvm/aux_str/aux_str.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1789 2023-05-05 22:20:16.000000 nvm-1.0.2/nvm/aux_str/clean_str_mappings.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/nvm/aux_sys/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-03 23:08:53.000000 nvm-1.0.2/nvm/aux_sys/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1342 2023-05-05 19:03:51.000000 nvm-1.0.2/nvm/aux_sys/aux_sys.py
+-rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-1.0.2/nvm/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/nvm.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     2146 2023-05-05 23:09:08.000000 nvm-1.0.2/nvm.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1635 2023-05-05 23:09:08.000000 nvm-1.0.2/nvm.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 23:09:08.000000 nvm-1.0.2/nvm.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-05 23:09:08.000000 nvm-1.0.2/nvm.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 23:09:08.000000 nvm-1.0.2/nvm.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-05 23:09:08.000000 nvm-1.0.2/nvm.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-05 23:09:08.000000 nvm-1.0.2/nvm.egg-info/top_level.txt
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-1.0.2/pyproject.toml
+-rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 21:20:43.000000 nvm-1.0.2/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      673 2023-05-05 23:09:08.932891 nvm-1.0.2/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-05 21:35:05.000000 nvm-1.0.2/setup.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:09:08.932891 nvm-1.0.2/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-1.0.2/tests/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1563 2023-05-05 15:01:56.000000 nvm-1.0.2/tests/test_aux_str.py
+-rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-1.0.2/tests/test_nvm.py
+-rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-1.0.2/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-1.0.2/versioneer.py
```

### Comparing `nvm-1.0.1/.github/workflows/build-main.yml` & `nvm-1.0.2/.github/workflows/build-main.yml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/.gitignore` & `nvm-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/.readthedocs.yaml` & `nvm-1.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/CONTRIBUTING.rst` & `nvm-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/LICENSE` & `nvm-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/Makefile` & `nvm-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/PKG-INFO` & `nvm-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 1.0.1
+Version: 1.0.2
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -29,15 +29,15 @@
 NVM
 ===
 
 .. image:: https://img.shields.io/pypi/v/nvm?version=latest
    :target: https://pypi.python.org/pypi/nvm
    :alt: PyPI Version
 
-.. image:: https://img.shields.io/pypi/l/nvm?color=blueviolet
+.. image:: https://img.shields.io/pypi/l/nvm?color=green
    :target: https://github.com/cogsys-io/nvm/blob/master/LICENSE
    :alt: License
 
 .. image:: https://img.shields.io/github/actions/workflow/status/cogsys-io/nvm/build-main.yml
    :alt: GitHub Workflow (Build Main) Status
    :target: https://github.com/cogsys-io/nvm
 
@@ -67,11 +67,8 @@
 .. _`cogsys-io/cogsys-io-cookiecutter-pypackage`: https://github.com/cogsys-io/cogsys-io-cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.0.0 (2023-05-03)
-------------------
-
-* First release on PyPI.
+* See https://pypi.org/project/nvm/#history
```

### Comparing `nvm-1.0.1/README.rst` & `nvm-1.0.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 NVM
 ===
 
 .. image:: https://img.shields.io/pypi/v/nvm?version=latest
    :target: https://pypi.python.org/pypi/nvm
    :alt: PyPI Version
 
-.. image:: https://img.shields.io/pypi/l/nvm?color=blueviolet
+.. image:: https://img.shields.io/pypi/l/nvm?color=green
    :target: https://github.com/cogsys-io/nvm/blob/master/LICENSE
    :alt: License
 
 .. image:: https://img.shields.io/github/actions/workflow/status/cogsys-io/nvm/build-main.yml
    :alt: GitHub Workflow (Build Main) Status
    :target: https://github.com/cogsys-io/nvm
```

### Comparing `nvm-1.0.1/data/emacs-logo/emacs-128x128.png` & `nvm-1.0.2/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/data/emacs-logo/emacs.svg` & `nvm-1.0.2/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/docs/Makefile` & `nvm-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `nvm-1.0.2/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/docs/requirements.txt` & `nvm-1.0.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/docs/source/conf.py` & `nvm-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/docs/source/installation.rst` & `nvm-1.0.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/nvm/aux_log/aux_log.py` & `nvm-1.0.2/nvm/aux_log/aux_log.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/nvm/aux_pandas/aux_pandas.py` & `nvm-1.0.2/nvm/aux_pandas/aux_pandas.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/nvm/aux_str/aux_str.py` & `nvm-1.0.2/nvm/aux_str/aux_str.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,14 +112,34 @@
     >>> # Import example mappings:
     >>> from nvm.aux_str import CLEAN_STR_MAPPINGS_TINY
     >>> from nvm.aux_str import CLEAN_STR_MAPPINGS_LARGE
     >>> from nvm.aux_str import CLEAN_STR_MAPPINGS_HUGE
     >>> # Display one of them as JSON:
     >>> import srsly
     >>> print(srsly.json_dumps(CLEAN_STR_MAPPINGS_TINY, indent=2))
+    [
+      {
+        " ":[
+          "\\n",
+          "\\r",
+          "\\t"
+        ]
+      },
+      {
+        "-":[
+          "\\u2212",
+          "\\u2013",
+          "\\u2014",
+          "\\u2015",
+          "\\ufe63",
+          "\\uff0d"
+        ]
+      }
+    ]
+
 
     Note that we used |json_dumps|_ function from the |srsly|_ library
     to get indented JSON output.
 
     .. |srsly| replace:: ``srsly``
     .. _srsly: https://github.com/explosion/srsly
```

### Comparing `nvm-1.0.1/nvm/aux_str/clean_str_mappings.py` & `nvm-1.0.2/nvm/aux_str/clean_str_mappings.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/nvm/aux_sys/aux_sys.py` & `nvm-1.0.2/nvm/aux_sys/aux_sys.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/nvm.egg-info/PKG-INFO` & `nvm-1.0.2/nvm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 1.0.1
+Version: 1.0.2
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -29,15 +29,15 @@
 NVM
 ===
 
 .. image:: https://img.shields.io/pypi/v/nvm?version=latest
    :target: https://pypi.python.org/pypi/nvm
    :alt: PyPI Version
 
-.. image:: https://img.shields.io/pypi/l/nvm?color=blueviolet
+.. image:: https://img.shields.io/pypi/l/nvm?color=green
    :target: https://github.com/cogsys-io/nvm/blob/master/LICENSE
    :alt: License
 
 .. image:: https://img.shields.io/github/actions/workflow/status/cogsys-io/nvm/build-main.yml
    :alt: GitHub Workflow (Build Main) Status
    :target: https://github.com/cogsys-io/nvm
 
@@ -67,11 +67,8 @@
 .. _`cogsys-io/cogsys-io-cookiecutter-pypackage`: https://github.com/cogsys-io/cogsys-io-cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.0.0 (2023-05-03)
-------------------
-
-* First release on PyPI.
+* See https://pypi.org/project/nvm/#history
```

### Comparing `nvm-1.0.1/nvm.egg-info/SOURCES.txt` & `nvm-1.0.2/nvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/nvm.egg-info/requires.txt` & `nvm-1.0.2/nvm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/pyproject.toml` & `nvm-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/setup.cfg` & `nvm-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/setup.py` & `nvm-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/tests/test_aux_str.py` & `nvm-1.0.2/tests/test_aux_str.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/tests/test_nvm.py` & `nvm-1.0.2/tests/test_nvm.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/tox.ini` & `nvm-1.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `nvm-1.0.1/versioneer.py` & `nvm-1.0.2/versioneer.py`

 * *Files identical despite different names*

