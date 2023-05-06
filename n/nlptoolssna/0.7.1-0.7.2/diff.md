# Comparing `tmp/nlptoolssna-0.7.1.tar.gz` & `tmp/nlptoolssna-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.7.1.tar", last modified: Sat May  6 08:31:44 2023, max compression
+gzip compressed data, was "nlptoolssna-0.7.2.tar", last modified: Sat May  6 08:34:51 2023, max compression
```

## Comparing `nlptoolssna-0.7.1.tar` & `nlptoolssna-0.7.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.795743 nlptoolssna-0.7.1/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-06 08:31:44.795743 nlptoolssna-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.700195 nlptoolssna-0.7.1/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.7.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.667833 nlptoolssna-0.7.1/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.667833 nlptoolssna-0.7.1/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.700195 nlptoolssna-0.7.1/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.1/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.708212 nlptoolssna-0.7.1/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.1/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.7.1/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.1/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.1/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.7.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.721392 nlptoolssna-0.7.1/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.721392 nlptoolssna-0.7.1/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.1/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.730907 nlptoolssna-0.7.1/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.730907 nlptoolssna-0.7.1/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.7.1/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.7.1/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.738929 nlptoolssna-0.7.1/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.7.1/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.7.1/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.738929 nlptoolssna-0.7.1/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.7.1/docs/source/api/utils/implication.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.746962 nlptoolssna-0.7.1/docs/source/api/utils/jaccard/
--rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.7.1/docs/source/api/utils/jaccard/jaccardFunction.rst
--rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.7.1/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.7.1/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.7.1/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.7.1/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.7.1/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.7.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.7.1/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.7.1/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.746962 nlptoolssna-0.7.1/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.754934 nlptoolssna-0.7.1/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.7.1/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.7.1/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.762947 nlptoolssna-0.7.1/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.7.1/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.7.1/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.7.1/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.7.1/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.7.1/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.7.1/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.762947 nlptoolssna-0.7.1/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.7.1/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.770927 nlptoolssna-0.7.1/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.7.1/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.7.1/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     5305 2023-05-05 21:28:54.000000 nlptoolssna-0.7.1/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.7.1/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.7.1/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.778938 nlptoolssna-0.7.1/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.7.1/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0    20574 2023-05-06 08:28:29.000000 nlptoolssna-0.7.1/nlptools/parse/implication.py
--rw-rw-rw-   0        0        0     7425 2023-05-06 08:29:41.000000 nlptoolssna-0.7.1/nlptools/parse/jaccard.py
--rw-rw-rw-   0        0        0     9326 2023-05-04 19:41:34.000000 nlptoolssna-0.7.1/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.778938 nlptoolssna-0.7.1/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 08:30:13.000000 nlptoolssna-0.7.1/nlptools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.795245 nlptoolssna-0.7.1/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-06 08:31:44.000000 nlptoolssna-0.7.1/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1725 2023-05-06 08:31:44.000000 nlptoolssna-0.7.1/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 08:31:44.000000 nlptoolssna-0.7.1/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-06 08:31:44.000000 nlptoolssna-0.7.1/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.7.1/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2023-05-06 08:31:44.000000 nlptoolssna-0.7.1/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 08:31:44.000000 nlptoolssna-0.7.1/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-06 08:31:44.795743 nlptoolssna-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:31:44.795743 nlptoolssna-0.7.1/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.7.1/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.319095 nlptoolssna-0.7.2/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-06 08:34:51.319095 nlptoolssna-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.218254 nlptoolssna-0.7.2/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.7.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.185754 nlptoolssna-0.7.2/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.185754 nlptoolssna-0.7.2/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.226283 nlptoolssna-0.7.2/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.2/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.234255 nlptoolssna-0.7.2/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.2/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.7.2/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.2/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.7.2/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.7.2/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.244390 nlptoolssna-0.7.2/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.244390 nlptoolssna-0.7.2/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.7.2/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.252409 nlptoolssna-0.7.2/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.252409 nlptoolssna-0.7.2/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.7.2/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.7.2/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.252409 nlptoolssna-0.7.2/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.7.2/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.7.2/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.260411 nlptoolssna-0.7.2/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.7.2/docs/source/api/utils/implication.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.260411 nlptoolssna-0.7.2/docs/source/api/utils/jaccard/
+-rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.7.2/docs/source/api/utils/jaccard/jaccardFunction.rst
+-rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.7.2/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.7.2/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.7.2/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.7.2/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.7.2/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.7.2/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.7.2/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.7.2/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.268685 nlptoolssna-0.7.2/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.268685 nlptoolssna-0.7.2/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.7.2/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.7.2/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.276771 nlptoolssna-0.7.2/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.7.2/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.7.2/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.7.2/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.7.2/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.7.2/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.7.2/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.285016 nlptoolssna-0.7.2/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.7.2/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.293134 nlptoolssna-0.7.2/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.7.2/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.7.2/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     5305 2023-05-05 21:28:54.000000 nlptoolssna-0.7.2/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.7.2/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.7.2/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.301777 nlptoolssna-0.7.2/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.7.2/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0    20574 2023-05-06 08:28:29.000000 nlptoolssna-0.7.2/nlptools/parse/implication.py
+-rw-rw-rw-   0        0        0     7425 2023-05-06 08:29:41.000000 nlptoolssna-0.7.2/nlptools/parse/jaccard.py
+-rw-rw-rw-   0        0        0     9326 2023-05-04 19:41:34.000000 nlptoolssna-0.7.2/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.302276 nlptoolssna-0.7.2/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 08:30:13.000000 nlptoolssna-0.7.2/nlptools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.311083 nlptoolssna-0.7.2/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-06 08:34:50.000000 nlptoolssna-0.7.2/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1725 2023-05-06 08:34:51.000000 nlptoolssna-0.7.2/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 08:34:50.000000 nlptoolssna-0.7.2/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-06 08:34:50.000000 nlptoolssna-0.7.2/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 08:34:50.000000 nlptoolssna-0.7.2/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      146 2023-05-06 08:34:50.000000 nlptoolssna-0.7.2/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 08:34:50.000000 nlptoolssna-0.7.2/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-06 08:34:51.319095 nlptoolssna-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:34:51.319095 nlptoolssna-0.7.2/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.7.2/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.7.1/CONTRIBUTING.rst` & `nlptoolssna-0.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/LICENSE` & `nlptoolssna-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/PKG-INFO` & `nlptoolssna-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.7.1/README.rst` & `nlptoolssna-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/docs/Makefile` & `nlptoolssna-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/docs/build/html/_images/download.png` & `nlptoolssna-0.7.2/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/docs/build/html/_static/download.png` & `nlptoolssna-0.7.2/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/docs/make.bat` & `nlptoolssna-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/docs/source/_static/download.png` & `nlptoolssna-0.7.2/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/docs/source/conf.py` & `nlptoolssna-0.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/docs/source/installation.rst` & `nlptoolssna-0.7.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.7.2/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/arabiner/data.py` & `nlptoolssna-0.7.2/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/arabiner/datasets.py` & `nlptoolssna-0.7.2/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/arabiner/helpers.py` & `nlptoolssna-0.7.2/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/arabiner/infer.py` & `nlptoolssna-0.7.2/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/arabiner/transforms.py` & `nlptoolssna-0.7.2/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/data/my_data.pickle` & `nlptoolssna-0.7.2/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/morphology/charsets.py` & `nlptoolssna-0.7.2/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.7.2/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.7.2/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/parse/implication.py` & `nlptoolssna-0.7.2/nlptools/parse/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/parse/jaccard.py` & `nlptoolssna-0.7.2/nlptools/parse/jaccard.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptools/parse/parser.py` & `nlptoolssna-0.7.2/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.7.2/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.7.1/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.7.2/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/setup.cfg` & `nlptoolssna-0.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.7.1/setup.py` & `nlptoolssna-0.7.2/setup.py`

 * *Files identical despite different names*

