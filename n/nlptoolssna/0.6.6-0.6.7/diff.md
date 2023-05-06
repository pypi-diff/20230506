# Comparing `tmp/nlptoolssna-0.6.6.tar.gz` & `tmp/nlptoolssna-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.6.6.tar", last modified: Fri May  5 21:29:15 2023, max compression
+gzip compressed data, was "nlptoolssna-0.6.7.tar", last modified: Sat May  6 06:42:49 2023, max compression
```

## Comparing `nlptoolssna-0.6.6.tar` & `nlptoolssna-0.6.7.tar`

### file list

```diff
@@ -1,88 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.470716 nlptoolssna-0.6.6/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-05 21:29:15.470716 nlptoolssna-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.357340 nlptoolssna-0.6.6/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.6.6/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.311746 nlptoolssna-0.6.6/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.313664 nlptoolssna-0.6.6/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.359365 nlptoolssna-0.6.6/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.6/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.367142 nlptoolssna-0.6.6/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.6/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.6.6/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.6/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.6/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.6.6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.378861 nlptoolssna-0.6.6/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.380811 nlptoolssna-0.6.6/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.6/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.387649 nlptoolssna-0.6.6/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.389664 nlptoolssna-0.6.6/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.6.6/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.6.6/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.391555 nlptoolssna-0.6.6/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.6.6/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.6.6/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.397456 nlptoolssna-0.6.6/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.6.6/docs/source/api/utils/implication.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.399369 nlptoolssna-0.6.6/docs/source/api/utils/jaccard/
--rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.6.6/docs/source/api/utils/jaccard/jaccardFunction.rst
--rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.6.6/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.6.6/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.6.6/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.6.6/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.6.6/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.6.6/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.6.6/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.6.6/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.405224 nlptoolssna-0.6.6/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.409220 nlptoolssna-0.6.6/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.6.6/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.6.6/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.421849 nlptoolssna-0.6.6/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.6.6/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.6.6/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.6.6/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.6.6/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.6.6/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.6.6/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.423786 nlptoolssna-0.6.6/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.6.6/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.433544 nlptoolssna-0.6.6/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.6.6/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.6.6/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     5305 2023-05-05 21:28:54.000000 nlptoolssna-0.6.6/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.6.6/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.6.6/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.440393 nlptoolssna-0.6.6/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.6.6/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0    20588 2023-05-04 20:28:19.000000 nlptoolssna-0.6.6/nlptools/parse/implication.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.445260 nlptoolssna-0.6.6/nlptools/parse/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.6.6/nlptools/parse/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-05-05 21:27:38.000000 nlptoolssna-0.6.6/nlptools/parse/jaccard/jaccardFunction.py
--rw-rw-rw-   0        0        0     9326 2023-05-04 19:41:34.000000 nlptoolssna-0.6.6/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.449012 nlptoolssna-0.6.6/nlptools/tools/
--rw-rw-rw-   0        0        0        0 2023-05-05 21:18:08.000000 nlptoolssna-0.6.6/nlptools/tools/__init__.py
--rw-rw-rw-   0        0        0     9326 2023-05-05 21:18:44.000000 nlptoolssna-0.6.6/nlptools/tools/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.464677 nlptoolssna-0.6.6/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1801 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-05 21:29:15.472749 nlptoolssna-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.469754 nlptoolssna-0.6.6/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.519810 nlptoolssna-0.6.7/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-06 06:42:49.519810 nlptoolssna-0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.413559 nlptoolssna-0.6.7/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.6.7/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.381426 nlptoolssna-0.6.7/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.381426 nlptoolssna-0.6.7/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.413559 nlptoolssna-0.6.7/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.7/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.421822 nlptoolssna-0.6.7/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.7/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.6.7/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.7/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.7/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.6.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.437820 nlptoolssna-0.6.7/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.437820 nlptoolssna-0.6.7/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.7/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.445822 nlptoolssna-0.6.7/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.445822 nlptoolssna-0.6.7/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.6.7/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.6.7/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.453917 nlptoolssna-0.6.7/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.6.7/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.6.7/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.453917 nlptoolssna-0.6.7/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.6.7/docs/source/api/utils/implication.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.462240 nlptoolssna-0.6.7/docs/source/api/utils/jaccard/
+-rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.6.7/docs/source/api/utils/jaccard/jaccardFunction.rst
+-rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.6.7/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.6.7/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.6.7/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.6.7/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.6.7/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.6.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.6.7/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.6.7/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.462240 nlptoolssna-0.6.7/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.470262 nlptoolssna-0.6.7/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.6.7/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.6.7/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.478297 nlptoolssna-0.6.7/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.6.7/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.6.7/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.6.7/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.6.7/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.6.7/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.6.7/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.478297 nlptoolssna-0.6.7/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.6.7/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.494867 nlptoolssna-0.6.7/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.6.7/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.6.7/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     5305 2023-05-05 21:28:54.000000 nlptoolssna-0.6.7/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.6.7/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.6.7/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.494867 nlptoolssna-0.6.7/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.6.7/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0    20588 2023-05-04 20:28:19.000000 nlptoolssna-0.6.7/nlptools/parse/implication.py
+-rw-rw-rw-   0        0        0     7425 2023-05-06 06:38:54.000000 nlptoolssna-0.6.7/nlptools/parse/jaccard.py
+-rw-rw-rw-   0        0        0     9326 2023-05-04 19:41:34.000000 nlptoolssna-0.6.7/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.503167 nlptoolssna-0.6.7/nlptools/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-05 21:18:08.000000 nlptoolssna-0.6.7/nlptools/tools/__init__.py
+-rw-rw-rw-   0        0        0     9326 2023-05-05 21:18:44.000000 nlptoolssna-0.6.7/nlptools/tools/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.511394 nlptoolssna-0.6.7/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-06 06:42:49.000000 nlptoolssna-0.6.7/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1750 2023-05-06 06:42:49.000000 nlptoolssna-0.6.7/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 06:42:49.000000 nlptoolssna-0.6.7/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-06 06:42:49.000000 nlptoolssna-0.6.7/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.6.7/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      146 2023-05-06 06:42:49.000000 nlptoolssna-0.6.7/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 06:42:49.000000 nlptoolssna-0.6.7/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-06 06:42:49.519810 nlptoolssna-0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:42:49.519810 nlptoolssna-0.6.7/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.6.7/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.6.6/CONTRIBUTING.rst` & `nlptoolssna-0.6.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/LICENSE` & `nlptoolssna-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/PKG-INFO` & `nlptoolssna-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.6.6/README.rst` & `nlptoolssna-0.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/docs/Makefile` & `nlptoolssna-0.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/docs/build/html/_images/download.png` & `nlptoolssna-0.6.7/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/docs/build/html/_static/download.png` & `nlptoolssna-0.6.7/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/docs/make.bat` & `nlptoolssna-0.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/docs/source/_static/download.png` & `nlptoolssna-0.6.7/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/docs/source/conf.py` & `nlptoolssna-0.6.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/docs/source/installation.rst` & `nlptoolssna-0.6.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.6.7/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/arabiner/data.py` & `nlptoolssna-0.6.7/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/arabiner/datasets.py` & `nlptoolssna-0.6.7/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/arabiner/helpers.py` & `nlptoolssna-0.6.7/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/arabiner/infer.py` & `nlptoolssna-0.6.7/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/arabiner/transforms.py` & `nlptoolssna-0.6.7/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/data/my_data.pickle` & `nlptoolssna-0.6.7/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/morphology/charsets.py` & `nlptoolssna-0.6.7/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.6.7/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.6.7/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/parse/implication.py` & `nlptoolssna-0.6.7/nlptools/parse/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/parse/jaccard/jaccardFunction.py` & `nlptoolssna-0.6.7/nlptools/parse/jaccard.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/parse/parser.py` & `nlptoolssna-0.6.7/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptools/tools/parser.py` & `nlptoolssna-0.6.7/nlptools/tools/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.6.7/nlptoolssna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.6.6/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.6.7/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -44,17 +44,16 @@
 nlptools/morphology/__init__.py
 nlptools/morphology/charsets.py
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
 nlptools/parse/__init__.py
 nlptools/parse/implication.py
+nlptools/parse/jaccard.py
 nlptools/parse/parser.py
-nlptools/parse/jaccard/__init__.py
-nlptools/parse/jaccard/jaccardFunction.py
 nlptools/tools/__init__.py
 nlptools/tools/parser.py
 nlptoolssna.egg-info/PKG-INFO
 nlptoolssna.egg-info/SOURCES.txt
 nlptoolssna.egg-info/dependency_links.txt
 nlptoolssna.egg-info/entry_points.txt
 nlptoolssna.egg-info/not-zip-safe
```

### Comparing `nlptoolssna-0.6.6/setup.cfg` & `nlptoolssna-0.6.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.6/setup.py` & `nlptoolssna-0.6.7/setup.py`

 * *Files identical despite different names*

