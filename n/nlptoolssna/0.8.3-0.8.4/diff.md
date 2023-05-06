# Comparing `tmp/nlptoolssna-0.8.3.tar.gz` & `tmp/nlptoolssna-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.8.3.tar", last modified: Sat May  6 11:26:10 2023, max compression
+gzip compressed data, was "nlptoolssna-0.8.4.tar", last modified: Sat May  6 11:31:49 2023, max compression
```

## Comparing `nlptoolssna-0.8.3.tar` & `nlptoolssna-0.8.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.232126 nlptoolssna-0.8.3/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-06 11:26:10.232126 nlptoolssna-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.127866 nlptoolssna-0.8.3/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.8.3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.095813 nlptoolssna-0.8.3/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.095813 nlptoolssna-0.8.3/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.127866 nlptoolssna-0.8.3/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.3/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.136148 nlptoolssna-0.8.3/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.3/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.8.3/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.3/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.3/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.8.3/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.155378 nlptoolssna-0.8.3/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.155548 nlptoolssna-0.8.3/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.3/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.163587 nlptoolssna-0.8.3/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.163587 nlptoolssna-0.8.3/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.8.3/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.8.3/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.163587 nlptoolssna-0.8.3/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.8.3/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.8.3/docs/source/api/morphology.rst
--rw-rw-rw-   0        0        0      168 2023-05-06 10:30:53.000000 nlptoolssna-0.8.3/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.8.3/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.8.3/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.8.3/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.8.3/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.171574 nlptoolssna-0.8.3/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.171574 nlptoolssna-0.8.3/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.8.3/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.8.3/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      132 2023-05-06 11:17:54.000000 nlptoolssna-0.8.3/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.187590 nlptoolssna-0.8.3/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.8.3/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.8.3/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.8.3/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.8.3/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.8.3/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.8.3/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.187590 nlptoolssna-0.8.3/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.8.3/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.204383 nlptoolssna-0.8.3/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.8.3/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.8.3/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     5289 2023-05-06 11:26:00.000000 nlptoolssna-0.8.3/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.8.3/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.8.3/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.212618 nlptoolssna-0.8.3/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.8.3/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0    20573 2023-05-06 11:00:30.000000 nlptoolssna-0.8.3/nlptools/utils/implication.py
--rw-rw-rw-   0        0        0     7316 2023-05-06 11:04:48.000000 nlptoolssna-0.8.3/nlptools/utils/jaccard.py
--rw-rw-rw-   0        0        0     9326 2023-05-06 10:58:16.000000 nlptoolssna-0.8.3/nlptools/utils/parser.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.8.3/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.232126 nlptoolssna-0.8.3/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-06 11:26:09.000000 nlptoolssna-0.8.3/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-05-06 11:26:10.000000 nlptoolssna-0.8.3/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:26:09.000000 nlptoolssna-0.8.3/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-06 11:26:09.000000 nlptoolssna-0.8.3/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.8.3/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-05-06 11:26:09.000000 nlptoolssna-0.8.3/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 11:26:09.000000 nlptoolssna-0.8.3/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-06 11:26:10.232126 nlptoolssna-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     2109 2023-05-06 10:49:14.000000 nlptoolssna-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:26:10.232126 nlptoolssna-0.8.3/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.8.3/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.994287 nlptoolssna-0.8.4/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-06 11:31:49.994287 nlptoolssna-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.883821 nlptoolssna-0.8.4/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.8.4/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.845360 nlptoolssna-0.8.4/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.845360 nlptoolssna-0.8.4/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.891819 nlptoolssna-0.8.4/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.4/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.899820 nlptoolssna-0.8.4/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.4/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.8.4/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.4/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.8.4/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.8.4/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.912457 nlptoolssna-0.8.4/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.912457 nlptoolssna-0.8.4/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.8.4/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.920567 nlptoolssna-0.8.4/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.921054 nlptoolssna-0.8.4/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.8.4/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.8.4/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.921054 nlptoolssna-0.8.4/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.8.4/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.8.4/docs/source/api/morphology.rst
+-rw-rw-rw-   0        0        0      168 2023-05-06 10:30:53.000000 nlptoolssna-0.8.4/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.8.4/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.8.4/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.8.4/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.8.4/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.929103 nlptoolssna-0.8.4/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.929103 nlptoolssna-0.8.4/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.8.4/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.8.4/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      132 2023-05-06 11:17:54.000000 nlptoolssna-0.8.4/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.945067 nlptoolssna-0.8.4/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.8.4/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.8.4/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.8.4/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.8.4/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.8.4/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.8.4/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.945067 nlptoolssna-0.8.4/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.8.4/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.961920 nlptoolssna-0.8.4/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.8.4/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.8.4/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     5289 2023-05-06 11:26:00.000000 nlptoolssna-0.8.4/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.8.4/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.8.4/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.977877 nlptoolssna-0.8.4/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.8.4/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0    20573 2023-05-06 11:00:30.000000 nlptoolssna-0.8.4/nlptools/utils/implication.py
+-rw-rw-rw-   0        0        0     7316 2023-05-06 11:31:42.000000 nlptoolssna-0.8.4/nlptools/utils/jaccard.py
+-rw-rw-rw-   0        0        0     9326 2023-05-06 10:58:16.000000 nlptoolssna-0.8.4/nlptools/utils/parser.py
+-rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.8.4/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.986023 nlptoolssna-0.8.4/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-06 11:31:49.000000 nlptoolssna-0.8.4/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-05-06 11:31:49.000000 nlptoolssna-0.8.4/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:31:49.000000 nlptoolssna-0.8.4/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-06 11:31:49.000000 nlptoolssna-0.8.4/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.8.4/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-06 11:31:49.000000 nlptoolssna-0.8.4/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 11:31:49.000000 nlptoolssna-0.8.4/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-06 11:31:49.994287 nlptoolssna-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     2109 2023-05-06 10:49:14.000000 nlptoolssna-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:31:49.994287 nlptoolssna-0.8.4/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.8.4/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.8.3/CONTRIBUTING.rst` & `nlptoolssna-0.8.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/LICENSE` & `nlptoolssna-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/PKG-INFO` & `nlptoolssna-0.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.8.3/README.rst` & `nlptoolssna-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/docs/Makefile` & `nlptoolssna-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/docs/build/html/_images/download.png` & `nlptoolssna-0.8.4/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/docs/build/html/_static/download.png` & `nlptoolssna-0.8.4/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/docs/make.bat` & `nlptoolssna-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/docs/source/_static/download.png` & `nlptoolssna-0.8.4/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/docs/source/conf.py` & `nlptoolssna-0.8.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/docs/source/installation.rst` & `nlptoolssna-0.8.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.8.4/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/arabiner/data.py` & `nlptoolssna-0.8.4/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/arabiner/datasets.py` & `nlptoolssna-0.8.4/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/arabiner/helpers.py` & `nlptoolssna-0.8.4/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/arabiner/infer.py` & `nlptoolssna-0.8.4/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/arabiner/transforms.py` & `nlptoolssna-0.8.4/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/data/my_data.pickle` & `nlptoolssna-0.8.4/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/morphology/charsets.py` & `nlptoolssna-0.8.4/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.8.4/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.8.4/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/utils/implication.py` & `nlptoolssna-0.8.4/nlptools/utils/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/utils/jaccard.py` & `nlptoolssna-0.8.4/nlptools/utils/jaccard.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptools/utils/parser.py` & `nlptoolssna-0.8.4/nlptools/utils/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.8.4/nlptoolssna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.8.3/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.8.4/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/setup.cfg` & `nlptoolssna-0.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.8.3/setup.py` & `nlptoolssna-0.8.4/setup.py`

 * *Files identical despite different names*

