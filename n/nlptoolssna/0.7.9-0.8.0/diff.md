# Comparing `tmp/nlptoolssna-0.7.9.tar.gz` & `tmp/nlptoolssna-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.7.9.tar", last modified: Sat May  6 11:07:34 2023, max compression
+gzip compressed data, was "nlptoolssna-0.8.0.tar", last modified: Sat May  6 11:12:13 2023, max compression
```

## Comparing `nlptoolssna-0.7.9.tar` & `nlptoolssna-0.8.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.309728 nlptoolssna-0.7.9/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-06 11:07:34.309728 nlptoolssna-0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.240968 nlptoolssna-0.7.9/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.7.9/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.213463 nlptoolssna-0.7.9/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.214470 nlptoolssna-0.7.9/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.241968 nlptoolssna-0.7.9/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.9/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.246969 nlptoolssna-0.7.9/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.9/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.7.9/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.9/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.9/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.7.9/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.256242 nlptoolssna-0.7.9/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.257242 nlptoolssna-0.7.9/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.9/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.260241 nlptoolssna-0.7.9/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.261242 nlptoolssna-0.7.9/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.7.9/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.7.9/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.262242 nlptoolssna-0.7.9/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.7.9/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.7.9/docs/source/api/morphology.rst
--rw-rw-rw-   0        0        0      168 2023-05-06 10:30:53.000000 nlptoolssna-0.7.9/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.7.9/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.7.9/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.7.9/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.7.9/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.266559 nlptoolssna-0.7.9/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.270557 nlptoolssna-0.7.9/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.7.9/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.7.9/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      296 2023-05-06 11:07:14.000000 nlptoolssna-0.7.9/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.277553 nlptoolssna-0.7.9/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.7.9/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.7.9/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.7.9/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.7.9/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.7.9/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.7.9/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.279157 nlptoolssna-0.7.9/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.7.9/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.288177 nlptoolssna-0.7.9/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.7.9/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.7.9/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     5305 2023-05-06 11:03:06.000000 nlptoolssna-0.7.9/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.7.9/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.7.9/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.294242 nlptoolssna-0.7.9/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.7.9/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0    20573 2023-05-06 11:00:30.000000 nlptoolssna-0.7.9/nlptools/utils/implication.py
--rw-rw-rw-   0        0        0     7316 2023-05-06 11:04:48.000000 nlptoolssna-0.7.9/nlptools/utils/jaccard.py
--rw-rw-rw-   0        0        0     9326 2023-05-06 10:58:16.000000 nlptoolssna-0.7.9/nlptools/utils/parser.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.7.9/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.306381 nlptoolssna-0.7.9/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-06 11:07:33.000000 nlptoolssna-0.7.9/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-05-06 11:07:34.000000 nlptoolssna-0.7.9/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:07:33.000000 nlptoolssna-0.7.9/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-06 11:07:33.000000 nlptoolssna-0.7.9/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.7.9/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-06 11:07:34.000000 nlptoolssna-0.7.9/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 11:07:34.000000 nlptoolssna-0.7.9/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-06 11:07:34.311735 nlptoolssna-0.7.9/setup.cfg
--rw-rw-rw-   0        0        0     2109 2023-05-06 10:49:14.000000 nlptoolssna-0.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:07:34.308380 nlptoolssna-0.7.9/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.7.9/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.424149 nlptoolssna-0.8.0/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-06 11:12:13.424149 nlptoolssna-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.342386 nlptoolssna-0.8.0/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.8.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.308972 nlptoolssna-0.8.0/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.316983 nlptoolssna-0.8.0/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.342386 nlptoolssna-0.8.0/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.0/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.350434 nlptoolssna-0.8.0/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.0/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.8.0/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.0/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.0/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.8.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.358575 nlptoolssna-0.8.0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.366395 nlptoolssna-0.8.0/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.0/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.366395 nlptoolssna-0.8.0/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.366395 nlptoolssna-0.8.0/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.8.0/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.8.0/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.366395 nlptoolssna-0.8.0/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.8.0/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.8.0/docs/source/api/morphology.rst
+-rw-rw-rw-   0        0        0      168 2023-05-06 10:30:53.000000 nlptoolssna-0.8.0/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.8.0/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.8.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.8.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.8.0/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.374405 nlptoolssna-0.8.0/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.382403 nlptoolssna-0.8.0/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.8.0/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.8.0/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      550 2023-05-06 11:12:01.000000 nlptoolssna-0.8.0/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.390568 nlptoolssna-0.8.0/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.8.0/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.8.0/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.8.0/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.8.0/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.8.0/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.8.0/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.390568 nlptoolssna-0.8.0/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.8.0/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.398688 nlptoolssna-0.8.0/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.8.0/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.8.0/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     5305 2023-05-06 11:03:06.000000 nlptoolssna-0.8.0/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.8.0/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.8.0/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.406706 nlptoolssna-0.8.0/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.8.0/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0    20573 2023-05-06 11:00:30.000000 nlptoolssna-0.8.0/nlptools/utils/implication.py
+-rw-rw-rw-   0        0        0     7316 2023-05-06 11:04:48.000000 nlptoolssna-0.8.0/nlptools/utils/jaccard.py
+-rw-rw-rw-   0        0        0     9326 2023-05-06 10:58:16.000000 nlptoolssna-0.8.0/nlptools/utils/parser.py
+-rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.8.0/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.424149 nlptoolssna-0.8.0/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-06 11:12:13.000000 nlptoolssna-0.8.0/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-05-06 11:12:13.000000 nlptoolssna-0.8.0/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:12:13.000000 nlptoolssna-0.8.0/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-06 11:12:13.000000 nlptoolssna-0.8.0/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.8.0/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-06 11:12:13.000000 nlptoolssna-0.8.0/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 11:12:13.000000 nlptoolssna-0.8.0/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-06 11:12:13.432538 nlptoolssna-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     2109 2023-05-06 10:49:14.000000 nlptoolssna-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:12:13.424149 nlptoolssna-0.8.0/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.8.0/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.7.9/CONTRIBUTING.rst` & `nlptoolssna-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/LICENSE` & `nlptoolssna-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/PKG-INFO` & `nlptoolssna-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.7.9
+Version: 0.8.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.7.9/README.rst` & `nlptoolssna-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/docs/Makefile` & `nlptoolssna-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/docs/build/html/_images/download.png` & `nlptoolssna-0.8.0/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/docs/build/html/_static/download.png` & `nlptoolssna-0.8.0/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/docs/make.bat` & `nlptoolssna-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/docs/source/_static/download.png` & `nlptoolssna-0.8.0/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/docs/source/conf.py` & `nlptoolssna-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/docs/source/installation.rst` & `nlptoolssna-0.8.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.8.0/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/arabiner/data.py` & `nlptoolssna-0.8.0/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/arabiner/datasets.py` & `nlptoolssna-0.8.0/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/arabiner/helpers.py` & `nlptoolssna-0.8.0/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/arabiner/infer.py` & `nlptoolssna-0.8.0/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/arabiner/transforms.py` & `nlptoolssna-0.8.0/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/data/my_data.pickle` & `nlptoolssna-0.8.0/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/morphology/charsets.py` & `nlptoolssna-0.8.0/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.8.0/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.8.0/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/utils/implication.py` & `nlptoolssna-0.8.0/nlptools/utils/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/utils/jaccard.py` & `nlptoolssna-0.8.0/nlptools/utils/jaccard.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptools/utils/parser.py` & `nlptoolssna-0.8.0/nlptools/utils/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.8.0/nlptoolssna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.7.9
+Version: 0.8.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.7.9/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.8.0/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/setup.cfg` & `nlptoolssna-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.9/setup.py` & `nlptoolssna-0.8.0/setup.py`

 * *Files identical despite different names*

