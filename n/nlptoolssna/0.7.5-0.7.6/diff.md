# Comparing `tmp/nlptoolssna-0.7.5.tar.gz` & `tmp/nlptoolssna-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.7.5.tar", last modified: Sat May  6 10:49:29 2023, max compression
+gzip compressed data, was "nlptoolssna-0.7.6.tar", last modified: Sat May  6 10:53:43 2023, max compression
```

## Comparing `nlptoolssna-0.7.5.tar` & `nlptoolssna-0.7.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.072758 nlptoolssna-0.7.5/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-06 10:49:29.073756 nlptoolssna-0.7.5/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.012376 nlptoolssna-0.7.5/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.7.5/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:28.985553 nlptoolssna-0.7.5/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:28.988606 nlptoolssna-0.7.5/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.014389 nlptoolssna-0.7.5/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.5/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.020376 nlptoolssna-0.7.5/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.5/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.7.5/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.5/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.5/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.7.5/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.027637 nlptoolssna-0.7.5/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.028613 nlptoolssna-0.7.5/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.5/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.032615 nlptoolssna-0.7.5/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.033633 nlptoolssna-0.7.5/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.7.5/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.7.5/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.035616 nlptoolssna-0.7.5/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.7.5/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.7.5/docs/source/api/morphology.rst
--rw-rw-rw-   0        0        0      168 2023-05-06 10:30:53.000000 nlptoolssna-0.7.5/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.7.5/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.7.5/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.7.5/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.7.5/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.038859 nlptoolssna-0.7.5/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.040858 nlptoolssna-0.7.5/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.7.5/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.7.5/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      379 2023-05-06 10:35:23.000000 nlptoolssna-0.7.5/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.049873 nlptoolssna-0.7.5/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.7.5/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.7.5/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.7.5/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.7.5/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.7.5/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.7.5/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.050860 nlptoolssna-0.7.5/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.7.5/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.057124 nlptoolssna-0.7.5/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.7.5/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.7.5/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     5305 2023-05-05 21:28:54.000000 nlptoolssna-0.7.5/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.7.5/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.7.5/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.059125 nlptoolssna-0.7.5/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.7.5/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.7.5/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.069757 nlptoolssna-0.7.5/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-06 10:49:28.000000 nlptoolssna-0.7.5/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1460 2023-05-06 10:49:28.000000 nlptoolssna-0.7.5/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 10:49:28.000000 nlptoolssna-0.7.5/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-06 10:49:28.000000 nlptoolssna-0.7.5/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.7.5/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-06 10:49:28.000000 nlptoolssna-0.7.5/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 10:49:28.000000 nlptoolssna-0.7.5/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-06 10:49:29.074796 nlptoolssna-0.7.5/setup.cfg
--rw-rw-rw-   0        0        0     2109 2023-05-06 10:49:14.000000 nlptoolssna-0.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:49:29.071757 nlptoolssna-0.7.5/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.7.5/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.637804 nlptoolssna-0.7.6/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-06 10:53:43.637804 nlptoolssna-0.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.574121 nlptoolssna-0.7.6/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.7.6/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.547026 nlptoolssna-0.7.6/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.549033 nlptoolssna-0.7.6/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.575135 nlptoolssna-0.7.6/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.6/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.581276 nlptoolssna-0.7.6/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.6/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.7.6/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.6/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.6/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.7.6/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.588556 nlptoolssna-0.7.6/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.589538 nlptoolssna-0.7.6/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.6/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.593581 nlptoolssna-0.7.6/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.595537 nlptoolssna-0.7.6/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.7.6/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.7.6/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.597535 nlptoolssna-0.7.6/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.7.6/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.7.6/docs/source/api/morphology.rst
+-rw-rw-rw-   0        0        0      168 2023-05-06 10:30:53.000000 nlptoolssna-0.7.6/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.7.6/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.7.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.7.6/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.7.6/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.603242 nlptoolssna-0.7.6/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.605241 nlptoolssna-0.7.6/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.7.6/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.7.6/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      132 2023-05-06 10:53:34.000000 nlptoolssna-0.7.6/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.615265 nlptoolssna-0.7.6/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.7.6/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.7.6/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.7.6/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.7.6/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.7.6/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.7.6/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.616266 nlptoolssna-0.7.6/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.7.6/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.622241 nlptoolssna-0.7.6/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.7.6/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.7.6/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     5305 2023-05-05 21:28:54.000000 nlptoolssna-0.7.6/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.7.6/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.7.6/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.624253 nlptoolssna-0.7.6/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.7.6/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.7.6/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.634806 nlptoolssna-0.7.6/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-06 10:53:43.000000 nlptoolssna-0.7.6/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1460 2023-05-06 10:53:43.000000 nlptoolssna-0.7.6/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 10:53:43.000000 nlptoolssna-0.7.6/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-06 10:53:43.000000 nlptoolssna-0.7.6/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.7.6/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-06 10:53:43.000000 nlptoolssna-0.7.6/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 10:53:43.000000 nlptoolssna-0.7.6/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-06 10:53:43.639804 nlptoolssna-0.7.6/setup.cfg
+-rw-rw-rw-   0        0        0     2109 2023-05-06 10:49:14.000000 nlptoolssna-0.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:53:43.636806 nlptoolssna-0.7.6/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.7.6/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.7.5/CONTRIBUTING.rst` & `nlptoolssna-0.7.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/LICENSE` & `nlptoolssna-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/PKG-INFO` & `nlptoolssna-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.7.5
+Version: 0.7.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.7.5/README.rst` & `nlptoolssna-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/docs/Makefile` & `nlptoolssna-0.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/docs/build/html/_images/download.png` & `nlptoolssna-0.7.6/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/docs/build/html/_static/download.png` & `nlptoolssna-0.7.6/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/docs/make.bat` & `nlptoolssna-0.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/docs/source/_static/download.png` & `nlptoolssna-0.7.6/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/docs/source/conf.py` & `nlptoolssna-0.7.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/docs/source/installation.rst` & `nlptoolssna-0.7.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.7.6/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/arabiner/data.py` & `nlptoolssna-0.7.6/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/arabiner/datasets.py` & `nlptoolssna-0.7.6/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/arabiner/helpers.py` & `nlptoolssna-0.7.6/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/arabiner/infer.py` & `nlptoolssna-0.7.6/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/arabiner/transforms.py` & `nlptoolssna-0.7.6/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/data/my_data.pickle` & `nlptoolssna-0.7.6/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/morphology/charsets.py` & `nlptoolssna-0.7.6/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.7.6/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.7.6/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.7.6/nlptoolssna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.7.5
+Version: 0.7.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.7.5/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.7.6/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/setup.cfg` & `nlptoolssna-0.7.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.5/setup.py` & `nlptoolssna-0.7.6/setup.py`

 * *Files identical despite different names*

