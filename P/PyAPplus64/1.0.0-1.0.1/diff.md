# Comparing `tmp/PyAPplus64-1.0.0.tar.gz` & `tmp/PyAPplus64-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAPplus64-1.0.0.tar", last modified: Thu May  4 14:11:30 2023, max compression
+gzip compressed data, was "PyAPplus64-1.0.1.tar", last modified: Sat May  6 20:22:25 2023, max compression
```

## Comparing `PyAPplus64-1.0.0.tar` & `PyAPplus64-1.0.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.768470 PyAPplus64-1.0.0/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1095 2023-05-04 13:06:10.000000 PyAPplus64-1.0.0/LICENSE
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      116 2023-05-04 12:51:18.000000 PyAPplus64-1.0.0/MANIFEST.in
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3451 2023-05-04 13:58:22.765470 PyAPplus64-1.0.0/PKG-INFO
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2601 2023-05-04 13:56:43.000000 PyAPplus64-1.0.0/README.md
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.159464 PyAPplus64-1.0.0/docs/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      638 2023-03-25 10:16:40.000000 PyAPplus64-1.0.0/docs/Makefile
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.068462 PyAPplus64-1.0.0/docs/build/
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.271465 PyAPplus64-1.0.0/docs/build/html/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      230 2023-04-28 08:50:36.000000 PyAPplus64-1.0.0/docs/build/html/.buildinfo
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.319465 PyAPplus64-1.0.0/docs/build/html/_sources/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-03-25 15:50:40.000000 PyAPplus64-1.0.0/docs/build/html/_sources/abhaengigkeiten.rst.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4548 2023-03-25 21:40:51.000000 PyAPplus64-1.0.0/docs/build/html/_sources/anwendungen.rst.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2299 2023-04-28 08:29:24.000000 PyAPplus64-1.0.0/docs/build/html/_sources/beschreibung.rst.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2558 2023-04-02 12:13:36.000000 PyAPplus64-1.0.0/docs/build/html/_sources/examples.rst.txt
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.327465 PyAPplus64-1.0.0/docs/build/html/_sources/generated/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1711 2023-03-25 10:47:31.000000 PyAPplus64-1.0.0/docs/build/html/_sources/generated/PyAPplus64.rst.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      186 2023-03-25 17:36:43.000000 PyAPplus64-1.0.0/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.461467 PyAPplus64-1.0.0/docs/build/html/_static/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     8441 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/base-stemmer.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    14764 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/basic.css
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     9726 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/doctools.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      655 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      286 2021-01-01 06:53:29.000000 PyAPplus64-1.0.0/docs/build/html/_static/file.png
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    17955 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/german-stemmer.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   288619 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/jquery.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    16663 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/language_data.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       90 2021-01-01 06:53:29.000000 PyAPplus64-1.0.0/docs/build/html/_static/minus.png
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4271 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/nature.css
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       90 2021-01-01 06:53:29.000000 PyAPplus64-1.0.0/docs/build/html/_static/plus.png
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5719 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/pygments.css
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    17035 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4099 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/translations.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    68705 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/_static/underscore.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     8900 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/abhaengigkeiten.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    23507 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/anwendungen.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     7997 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/beschreibung.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    95849 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/examples.html
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.469467 PyAPplus64-1.0.0/docs/build/html/generated/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   321386 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/generated/PyAPplus64.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    47217 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/genindex.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4948 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/index.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1957 2023-04-28 08:50:36.000000 PyAPplus64-1.0.0/docs/build/html/objects.inv
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     6290 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/py-modindex.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3742 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/search.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    24661 2023-05-04 12:56:24.000000 PyAPplus64-1.0.0/docs/build/html/searchindex.js
--rwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)      114 2023-05-04 12:56:52.000000 PyAPplus64-1.0.0/docs/builddocs.sh
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      804 2023-05-04 12:57:07.000000 PyAPplus64-1.0.0/docs/make.bat
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.520467 PyAPplus64-1.0.0/docs/source/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-03-25 15:50:40.000000 PyAPplus64-1.0.0/docs/source/abhaengigkeiten.rst
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4548 2023-03-25 21:40:51.000000 PyAPplus64-1.0.0/docs/source/anwendungen.rst
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2299 2023-04-28 09:19:27.000000 PyAPplus64-1.0.0/docs/source/beschreibung.rst
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1524 2023-05-04 12:57:16.000000 PyAPplus64-1.0.0/docs/source/conf.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2558 2023-05-04 12:51:18.000000 PyAPplus64-1.0.0/docs/source/examples.rst
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      186 2023-03-25 17:36:43.000000 PyAPplus64-1.0.0/docs/source/index.rst
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.571468 PyAPplus64-1.0.0/examples/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1403 2023-05-04 12:58:45.000000 PyAPplus64-1.0.0/examples/adhoc_report.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      756 2023-05-04 12:59:22.000000 PyAPplus64-1.0.0/examples/applus-server.yaml
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1120 2023-05-04 12:59:18.000000 PyAPplus64-1.0.0/examples/check_dokumente.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2268 2023-05-04 12:59:32.000000 PyAPplus64-1.0.0/examples/copy_artikel.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     7249 2023-05-04 13:00:01.000000 PyAPplus64-1.0.0/examples/mengenabweichung.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      988 2023-05-04 13:50:46.000000 PyAPplus64-1.0.0/pyproject.toml
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       38 2023-05-04 13:58:22.770470 PyAPplus64-1.0.0/setup.cfg
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.099463 PyAPplus64-1.0.0/src/
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.683469 PyAPplus64-1.0.0/src/PyAPplus64/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      734 2023-05-04 13:00:15.000000 PyAPplus64-1.0.0/src/PyAPplus64/__init__.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    12557 2023-05-04 13:00:50.000000 PyAPplus64-1.0.0/src/PyAPplus64/applus.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5745 2023-05-04 13:00:22.000000 PyAPplus64-1.0.0/src/PyAPplus64/applus_db.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5463 2023-05-04 13:00:27.000000 PyAPplus64-1.0.0/src/PyAPplus64/applus_scripttool.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3200 2023-05-04 13:00:33.000000 PyAPplus64-1.0.0/src/PyAPplus64/applus_server.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2091 2023-05-04 13:00:39.000000 PyAPplus64-1.0.0/src/PyAPplus64/applus_sysconf.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    12308 2023-05-04 13:00:45.000000 PyAPplus64-1.0.0/src/PyAPplus64/applus_usexml.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    23159 2023-05-04 13:00:58.000000 PyAPplus64-1.0.0/src/PyAPplus64/duplicate.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4775 2023-05-04 13:01:06.000000 PyAPplus64-1.0.0/src/PyAPplus64/pandas.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 12:51:19.000000 PyAPplus64-1.0.0/src/PyAPplus64/py.typed
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    27730 2023-05-04 13:01:16.000000 PyAPplus64-1.0.0/src/PyAPplus64/sql_utils.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1764 2023-05-04 13:01:22.000000 PyAPplus64-1.0.0/src/PyAPplus64/utils.py
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.736470 PyAPplus64-1.0.0/src/PyAPplus64.egg-info/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3451 2023-05-04 13:58:21.000000 PyAPplus64-1.0.0/src/PyAPplus64.egg-info/PKG-INFO
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2180 2023-05-04 13:58:22.000000 PyAPplus64-1.0.0/src/PyAPplus64.egg-info/SOURCES.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)        1 2023-05-04 13:58:22.000000 PyAPplus64-1.0.0/src/PyAPplus64.egg-info/dependency_links.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       48 2023-05-04 13:58:22.000000 PyAPplus64-1.0.0/src/PyAPplus64.egg-info/requires.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       11 2023-05-04 13:58:22.000000 PyAPplus64-1.0.0/src/PyAPplus64.egg-info/top_level.txt
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 13:58:22.752470 PyAPplus64-1.0.0/tests/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      796 2023-05-04 13:01:31.000000 PyAPplus64-1.0.0/tests/test_applus_db.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    13881 2023-05-04 13:01:37.000000 PyAPplus64-1.0.0/tests/test_sql_utils.py
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:25.056602 PyAPplus64-1.0.1/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1095 2023-05-04 13:06:10.000000 PyAPplus64-1.0.1/LICENSE
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      116 2023-05-04 12:51:18.000000 PyAPplus64-1.0.1/MANIFEST.in
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4008 2023-05-06 20:22:25.053602 PyAPplus64-1.0.1/PKG-INFO
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3158 2023-05-04 14:57:06.000000 PyAPplus64-1.0.1/README.md
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.423595 PyAPplus64-1.0.1/docs/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      638 2023-03-25 10:16:40.000000 PyAPplus64-1.0.1/docs/Makefile
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.321594 PyAPplus64-1.0.1/docs/build/
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.528596 PyAPplus64-1.0.1/docs/build/html/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      230 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/.buildinfo
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.581597 PyAPplus64-1.0.1/docs/build/html/_sources/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-03-25 15:50:40.000000 PyAPplus64-1.0.1/docs/build/html/_sources/abhaengigkeiten.rst.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4585 2023-05-06 17:30:57.000000 PyAPplus64-1.0.1/docs/build/html/_sources/anwendungen.rst.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2299 2023-04-28 09:19:27.000000 PyAPplus64-1.0.1/docs/build/html/_sources/beschreibung.rst.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2825 2023-05-06 17:30:57.000000 PyAPplus64-1.0.1/docs/build/html/_sources/examples.rst.txt
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.589597 PyAPplus64-1.0.1/docs/build/html/_sources/generated/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1711 2023-03-25 10:47:31.000000 PyAPplus64-1.0.1/docs/build/html/_sources/generated/PyAPplus64.rst.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      186 2023-03-25 17:36:43.000000 PyAPplus64-1.0.1/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.734598 PyAPplus64-1.0.1/docs/build/html/_static/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     8133 2021-11-17 15:47:22.000000 PyAPplus64-1.0.1/docs/build/html/_static/base-stemmer.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    14667 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/basic.css
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     9630 2021-11-17 15:50:47.000000 PyAPplus64-1.0.1/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      353 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      286 2021-01-01 06:53:29.000000 PyAPplus64-1.0.1/docs/build/html/_static/file.png
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    17647 2021-11-17 15:47:22.000000 PyAPplus64-1.0.1/docs/build/html/_static/german-stemmer.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   288550 2022-02-21 10:29:39.000000 PyAPplus64-1.0.1/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    16661 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       90 2021-01-01 06:53:29.000000 PyAPplus64-1.0.1/docs/build/html/_static/minus.png
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4181 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/nature.css
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       90 2021-01-01 06:53:29.000000 PyAPplus64-1.0.1/docs/build/html/_static/plus.png
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5432 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    16950 2021-12-19 12:55:13.000000 PyAPplus64-1.0.1/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3792 2021-12-19 12:55:13.000000 PyAPplus64-1.0.1/docs/build/html/_static/translations.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    68398 2021-12-16 10:20:19.000000 PyAPplus64-1.0.1/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     8606 2023-05-06 20:11:52.000000 PyAPplus64-1.0.1/docs/build/html/abhaengigkeiten.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    23321 2023-05-06 20:11:52.000000 PyAPplus64-1.0.1/docs/build/html/anwendungen.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     7705 2023-05-06 20:11:52.000000 PyAPplus64-1.0.1/docs/build/html/beschreibung.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   109765 2023-05-06 20:11:52.000000 PyAPplus64-1.0.1/docs/build/html/examples.html
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.742598 PyAPplus64-1.0.1/docs/build/html/generated/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   321089 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/generated/PyAPplus64.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    46923 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/genindex.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4654 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/index.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1962 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/objects.inv
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5996 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/py-modindex.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3448 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/search.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    25310 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/searchindex.js
+-rwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)      114 2023-05-04 12:56:52.000000 PyAPplus64-1.0.1/docs/builddocs.sh
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      804 2023-05-04 12:57:07.000000 PyAPplus64-1.0.1/docs/make.bat
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.806599 PyAPplus64-1.0.1/docs/source/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-03-25 15:50:40.000000 PyAPplus64-1.0.1/docs/source/abhaengigkeiten.rst
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4585 2023-05-06 17:30:57.000000 PyAPplus64-1.0.1/docs/source/anwendungen.rst
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2299 2023-04-28 09:19:27.000000 PyAPplus64-1.0.1/docs/source/beschreibung.rst
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1561 2023-05-06 20:20:57.000000 PyAPplus64-1.0.1/docs/source/conf.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2825 2023-05-06 17:30:57.000000 PyAPplus64-1.0.1/docs/source/examples.rst
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      186 2023-03-25 17:36:43.000000 PyAPplus64-1.0.1/docs/source/index.rst
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.858600 PyAPplus64-1.0.1/examples/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/examples/adhoc_report.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      756 2023-05-04 12:59:22.000000 PyAPplus64-1.0.1/examples/applus-server.yaml
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1266 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/examples/check_dokumente.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2295 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/examples/copy_artikel.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     7447 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/examples/mengenabweichung.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      988 2023-05-06 20:20:57.000000 PyAPplus64-1.0.1/pyproject.toml
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       38 2023-05-06 20:22:25.058602 PyAPplus64-1.0.1/setup.cfg
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.355594 PyAPplus64-1.0.1/src/
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.973601 PyAPplus64-1.0.1/src/PyAPplus64/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      735 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/src/PyAPplus64/__init__.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    12530 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5691 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_db.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     6563 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_scripttool.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3148 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_server.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2130 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_sysconf.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    12187 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_usexml.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    22880 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/duplicate.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4765 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/pandas.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 12:51:19.000000 PyAPplus64-1.0.1/src/PyAPplus64/py.typed
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    27330 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/sql_utils.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1724 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/utils.py
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:25.023601 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4008 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/PKG-INFO
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2180 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/SOURCES.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)        1 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/dependency_links.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       48 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/requires.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       11 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/top_level.txt
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:25.042601 PyAPplus64-1.0.1/tests/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      786 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/tests/test_applus_db.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    13162 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/tests/test_sql_utils.py
```

### Comparing `PyAPplus64-1.0.0/LICENSE` & `PyAPplus64-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.0/PKG-INFO` & `PyAPplus64-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: PyAPplus64
-Version: 1.0.0
-Summary: Verschiedene Hilfsmittel, um mit dem ERP System APplus zu interagieren. Dieses Packet wurde für APplus 6.4 entwickelt, funktioniert vermutlich aber auch mit anderen Versionen.
-Author-email: Thomas Tuerk <kontakt@thomas-tuerk.de>
-Project-URL: homepage, https://www.thomas-tuerk.de/de/pyapplus64
-Project-URL: repository, https://git.thomas-tuerk.de/thtuerk/PyAPplus64
-Project-URL: documentation, https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Other Audience
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyAPplus64
 
 ## Beschreibung 
 Das Paket `PyAPplus64` enthält eine Sammlung von Python Tools für die Interaktion mit dem ERP-System APplus 6.4. 
 Es sollte auch für andere APplus Versionen nützlich sein. 
 
 Zielgruppe sind APplus-Administratoren und Anpassungs-Entwickler. Die Tools erlauben u.a.
@@ -52,20 +35,26 @@
 
 ## Warnung
 
 `PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige 
 Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie 
 `PyAPplus64` daher bitte vorsichtig. 
 
-## Lizenz
+## Installation
+
+PyAPplus64 wurde auf PyPi veröffentlicht. Es lässt sich daher einfach mittel `pip` installieren
 
-`PyAPplus64` wurde unter MIT license veröffentlicht.
+````
+  pip install PyAPplus64
+````
 
 ## Links
 
-- Homepage https://www.thomas-tuerk.de/de/pyapplus64
-- Doku 
-  + PDF https://www.thomas-tuerk.de/assets/PyAPplus64/pyapplus64.pdf
-  + HTML https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html
-- GIT-Repository https://git.thomas-tuerk.de/thtuerk/PyAPplus64
-- PyPI https://pypi.org/project/PyAPplus64/
-  
+- [PyPi](https://pypi.org/project/PyAPplus64/)
+- Doku [PDF](https://www.thomas-tuerk.de/assets/PyAPplus64/pyapplus64.pdf), [HTML](https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html)
+- [GIT-Repository](https://git.thomas-tuerk.de/thtuerk/PyAPplus64)
+- [GitHub](https://github.com/thtuerk/PyAPplus64)
+
+## Lizenz / Mitarbeit
+
+Ich habe PyAPplus64 unter MIT License veröffentlicht. Diese Lizenz gibt Ihnen weitreichende Rechte für die Nutzung von PyAPplus64, auch im kommerziellen Kontext. Ich bitte aber dringend darum, Ihre Änderungen, Erweiterungen und Fehlerkorrekturen auch anderen zur Verfügung zu stellen. Dafür können Sie die üblichen Methoden auf Github nutzen oder mir ([Thomas Türk](mailto:kontakt@thomas-tuerk.de)) eine eMail mit den Änderungen schicken.
+
```

### Comparing `PyAPplus64-1.0.0/README.md` & `PyAPplus64-1.0.1/docs/build/html/_sources/beschreibung.rst.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# PyAPplus64
+Beschreibung
+============
 
-## Beschreibung 
 Das Paket `PyAPplus64` enthält eine Sammlung von Python Tools für die Interaktion mit dem ERP-System APplus 6.4. 
 Es sollte auch für andere APplus Versionen nützlich sein. 
 
-Zielgruppe sind APplus-Administratoren und Anpassungs-Entwickler. Die Tools erlauben u.a.
+Zielgruppe sind APplus-Administratoren und Anpassungs-Entwickler. `PyAPplus64` erlaubt u.a.
 
-- einfacher Zugriff auf SOAP-Schnittstelle des App-Servers
+- einfacher Zugriff auf SOAP-Schnittstelle des APP-Servers
    + damit Zugriff auf SysConfig
-   + Zugriff auf Tools `nextNumber` für Erzeugung der nächsten Nummer für ein Business-Object
+   + Zugriff auf Tools wie z.B. `nextNumber` für Erzeugung der nächsten Nummer für ein Business-Object
    + ...   
 - Zugriff auf APplus DB per direktem DB-Zugriff und mittels SOAP
-   + automatischer Aufruf von `completeSQL`, um per App-Server SQL-Statements um z.B. Mandanten erweitern zu lassen
+   + automatischer Aufruf von `completeSQL`, um per AppServer SQL-Statements um z.B. Mandanten erweitern zu lassen
    + Tools für einfache Benutzung von `useXML`, d.h. für das Einfügen, Löschen und Ändern von Datensätzen
      mit Hilfe des APP-Servers. Genau wie bei Änderungen an Datensätzen über die Web-Oberfläche und im Gegensatz 
      zum direkten Zugriff über die Datenbank werden dabei evtl. zusätzliche 
      Checks ausgeführt, bestimmte Felder automatisch gesetzt oder bestimmte Aktionen angestoßen. 
 - das Duplizieren von Datensätzen
    + zu kopierende Felder aus XML-Definitionen werden ausgewertet
    + Abhängige Objekte können einfach ebenfalls mit-kopiert werden
@@ -29,26 +29,14 @@
    + einfache Wrapper um andere Libraries, spart aber Zeit
 - ...
 
 In `PyAPplus64` wurden die Features (vielleicht leicht verallgemeinert)
 implementiert, die ich für konkrete Aufgabenstellungen benötigte. Ich gehe davon
 aus, dass im Laufe der Zeit weitere Features hinzukommen.
 
-## Warnung
+Warnung
+-------
 
 `PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige 
 Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie 
-`PyAPplus64` daher bitte vorsichtig. 
+`PyAPplus64` daher bitte vorsichtig. Zudem kann ich leider nicht garantieren, dass `PyAPplus64` fehlerfrei ist. 
 
-## Lizenz
-
-`PyAPplus64` wurde unter MIT license veröffentlicht.
-
-## Links
-
-- Homepage https://www.thomas-tuerk.de/de/pyapplus64
-- Doku 
-  + PDF https://www.thomas-tuerk.de/assets/PyAPplus64/pyapplus64.pdf
-  + HTML https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html
-- GIT-Repository https://git.thomas-tuerk.de/thtuerk/PyAPplus64
-- PyPI https://pypi.org/project/PyAPplus64/
-
```

### Comparing `PyAPplus64-1.0.0/docs/Makefile` & `PyAPplus64-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.0/docs/build/html/_sources/abhaengigkeiten.rst.txt` & `PyAPplus64-1.0.1/docs/build/html/_sources/abhaengigkeiten.rst.txt`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.0/docs/build/html/_sources/anwendungen.rst.txt` & `PyAPplus64-1.0.1/docs/build/html/_sources/anwendungen.rst.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Artikeln (angezeigt als `Bild` in `ArtikelRec.aspx`), für die Datei, auf die
 verwiesen wird, nicht im Dateisystem existiert. Diese fehlenden Dateien werden
 ausgegeben und das Feld `DOCUMENTS` gelöscht. Das Löschen erfolgt dabei über 
 `useXML`, so dass die Felder `UPDDATE` und `UPDUSER` korrekt gesetzt werden.
 
 .. literalinclude:: ../../examples/check_dokumente.py
    :language: python
+   :lines: 9-
    :linenos:
 
 Man kann alle Python Bibliotheken nutzen. Als Erweiterung wäre es in obigem Script 
 zum Beispiel einfach möglich, alle BMP-Bilder zu suchen, nach PNG zu konvertieren 
 und den DB-Eintrag anzupassen.
 
 
@@ -37,14 +38,15 @@
 werden, bietet sich evtl. Python an. 
 
 Folgendes Script erzeugt zum Beispiel eine Excel-Tabelle, mit einer Übersicht,
 welche Materialen wie oft für Artikel benutzt werden:
 
 .. literalinclude:: ../../examples/adhoc_report.py
    :language: python
+   :lines: 9-
    :linenos:
 
 Dieses kurze Script nutzt Standard-Pandas Methoden zur Erzeugung der Excel-Datei. Allerdings
 sind diese Methoden in den Aufrufen von `pandasReadSql` und `exportToExcel` gekapselt,
 so dass der Aufruf sehr einfach ist. Zudem ist es sehr einfach, die Verbindung zur Datenbank
 und zum APP-Server mittels der YAML-Konfigdatei herzustellen. Bei diesem 
 Aufruf kann optional ein Nutzer und eine Umgebung übergeben werden, die die Standard-Werte aus 
@@ -52,15 +54,15 @@
 der für die Umgebung korrekte Mandant automatisch verwendet wird.
 
 
 
 Anbindung eigener Tools
 -----------------------
 
-Ursprünglich wurde `PyAPplus64` für die Anbindung einer APplus-Anpassung geschrieben. Dieses ist 
+Ursprünglich wurde `PyAPplus64` für die Anbindung einer APplus-Anpassung geschrieben. Diese Anpassung ist 
 als Windows-Service auf einem eigenen Rechner installiert und überwacht dort ein bestimmtes Verzeichnis.
 Bei Änderungen an Dateien in diesem Verzeichnis (Hinzufügen, Ändern, Löschen) werden die Dateien verarbeitet
 und die Ergebnisse an APplus gemeldet. Dafür werden DB-Operationen aber auch SOAP-Calls benutzt.
 Ebenso wird auf die SysConf zugegriffen.
 
 Viele solcher Anpassungen lassen sich gut und sinnvoll im App-Server einrichten und als Job regelmäßig aufrufen. 
 Im konkreten Fall wird jedoch für die Verarbeitung der Dateien viel Rechenzeit benötigt. Dies würde dadurch
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_sources/beschreibung.rst.txt` & `PyAPplus64-1.0.1/docs/source/beschreibung.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,11 +34,9 @@
 aus, dass im Laufe der Zeit weitere Features hinzukommen.
 
 Warnung
 -------
 
 `PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige 
 Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie 
-`PyAPplus64` daher bitte vorsichtig. Zudem kann ich leider nicht garantieren, dass `PyAPplus` fehlerfrei ist. 
-
-
+`PyAPplus64` daher bitte vorsichtig. Zudem kann ich leider nicht garantieren, dass `PyAPplus64` fehlerfrei ist.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_sources/examples.rst.txt` & `PyAPplus64-1.0.1/docs/build/html/_sources/examples.rst.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,42 +9,53 @@
 Viele Scripte teilen sich Einstellungen. Beispielsweise greifen fast alle Scripte irgendwie auf APplus zu und benötigen Informationen,
 mit welchem APP-Server, welchem Web-Server und welcher Datenbank sie sich verbinden sollen. Solche Informationen, insbesondere die Passwörter, werden nicht in  
 jedem Script gespeichert, sondern nur in den Config-Dateien. Es bietet sich wohl meist an, 3 Konfigdateien zu erstellen, je eine für 
 das Deploy-, das Test- und das Prod-System. Ein Beispiel ist im Unterverzeichnis ``examples/applus-server.yaml`` zu finden.
 
 .. literalinclude:: ../../examples/applus-server.yaml
    :language: yaml
+   :lines: 9-
    :linenos:
    
 Damit nicht in jedem Script immer wieder neu die Konfig-Dateien ausgewählt werden müssen, werden die Konfigs für 
-das Prod-, Test- und Deploy-System in ``examples/applus_configs.py`` hinterlegt. Diese wird in allen Scripten importiert,
+das Prod-, Test- und Deploy-System in ``examples/applus_configs.py`` hinterlegt. Diese Datei wird in allen Scripten importiert,
 so dass das Config-Verzeichnis und die darin enthaltenen Configs einfach zur Verfügung stehen.
 
 .. literalinclude:: ../../examples/applus_configs.py
    :language: python
+   :lines: 9-
    :linenos:
 
    
+``read_settings.py``
+-----------------------
+Einfaches Beispiel für Auslesen der SysConf und bestimmter Einstellungen.
+
+.. literalinclude:: ../../examples/read_settings.py
+   :language: python
+   :lines: 9-
+   :linenos:
+
 ``check_dokumente.py``
 -----------------------
 Einfaches Beispiel für lesenden und schreibenden Zugriff auf APplus Datenbank.
 
 .. literalinclude:: ../../examples/check_dokumente.py
    :language: python
-   :lines: 6-
+   :lines: 9-
    :linenos:
 
 
 ``adhoc_report.py``
 -------------------
 Sehr einfaches Beispiel zur Erstellung einer Excel-Tabelle aus einer SQL-Abfrage.
 
 .. literalinclude:: ../../examples/adhoc_report.py
    :language: python
-   :lines: 7-
+   :lines: 9-
    :linenos:
 
 
 ``mengenabweichung.py``
 -----------------------
 Etwas komplizierteres Beispiel zur Erstellung einer Excel-Datei aus SQL-Abfragen.
 
@@ -56,18 +67,18 @@
 ``mengenabweichung_gui.py``
 ---------------------------
 Beispiel für eine sehr einfache GUI, die die Eingabe einfacher Parameter erlaubt.
 Die GUI wird um die Erzeugung von Excel-Dateien mit Mengenabweichungen gebaut.
 
 .. literalinclude:: ../../examples/mengenabweichung_gui.pyw
    :language: python
-   :lines: 7-
+   :lines: 9-
    :linenos:
 
 ``copy_artikel.py``
 -----------------------
 Beispiel, wie Artikel inklusive Arbeitsplan und Stückliste dupliziert werden kann.
 
 .. literalinclude:: ../../examples/copy_artikel.py
    :language: python
-   :lines: 21-
+   :lines: 22-
    :linenos:
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_sources/generated/PyAPplus64.rst.txt` & `PyAPplus64-1.0.1/docs/build/html/_sources/generated/PyAPplus64.rst.txt`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/base-stemmer.js` & `PyAPplus64-1.0.1/docs/build/html/_static/base-stemmer.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,7 @@
-/*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
- *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
- *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
-
 /**@constructor*/
 BaseStemmer = function() {
     this.setCurrent = function(value) {
         this.current = value;
         this.cursor = 0;
         this.limit = this.current.length;
         this.limit_backward = 0;
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/basic.css` & `PyAPplus64-1.0.1/docs/build/html/_static/basic.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 /*
-Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
-
-This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
-
-Use of this source code is governed by an MIT-style
-license that can be found in the LICENSE file or at
-https://opensource.org/licenses/MIT.*/
+ * basic.css
+ * ~~~~~~~~~
+ *
+ * Sphinx stylesheet -- basic theme.
+ *
+ * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :license: BSD, see LICENSE for details.
+ *
+ */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
     clear: both;
 }
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/doctools.js` & `PyAPplus64-1.0.1/docs/build/html/_static/doctools.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,17 @@
 /*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
+ * doctools.js
+ * ~~~~~~~~~~~
  *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
+ * Sphinx JavaScript utilities for all documentation.
  *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
+ * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :license: BSD, see LICENSE for details.
+ *
+ */
 
 /**
  * select a different prefix for underscore
  */
 $u = _.noConflict();
 
 /**
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/german-stemmer.js` & `PyAPplus64-1.0.1/docs/build/html/_static/german-stemmer.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,7 @@
-/*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
- *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
- *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
-
 // Generated by Snowball 2.1.0 - https://snowballstem.org/
 
 /**@constructor*/
 GermanStemmer = function() {
     var base = new BaseStemmer();
     /** @const */
     var a_0 = [
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/jquery.js` & `PyAPplus64-1.0.1/docs/build/html/_static/jquery.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,18 @@
-/*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
+/*!
+ * jQuery JavaScript Library v3.6.0
+ * https://jquery.com/
  *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
+ * Includes Sizzle.js
+ * https://sizzlejs.com/
  *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
+ * Copyright OpenJS Foundation and other contributors
+ * Released under the MIT license
+ * https://jquery.org/license
+ */
 (function(global, factory) {
 
     "use strict";
 
     if (typeof module === "object" && typeof module.exports === "object") {
 
         // For CommonJS and CommonJS-like environments where a proper `window`
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/language_data.js` & `PyAPplus64-1.0.1/docs/build/html/_static/language_data.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,18 @@
 /*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
+ * language_data.js
+ * ~~~~~~~~~~~~~~~~
  *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
+ * This script contains the language-specific data used by searchtools.js,
+ * namely the list of stopwords, stemmer, scorer and splitter.
  *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
+ * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :license: BSD, see LICENSE for details.
+ *
+ */
 
 var stopwords = ["aber", "alle", "allem", "allen", "aller", "alles", "als", "also", "am", "an", "ander", "andere", "anderem", "anderen", "anderer", "anderes", "anderm", "andern", "anderr", "anders", "auch", "auf", "aus", "bei", "bin", "bis", "bist", "da", "damit", "dann", "das", "dasselbe", "dazu", "da\u00df", "dein", "deine", "deinem", "deinen", "deiner", "deines", "dem", "demselben", "den", "denn", "denselben", "der", "derer", "derselbe", "derselben", "des", "desselben", "dessen", "dich", "die", "dies", "diese", "dieselbe", "dieselben", "diesem", "diesen", "dieser", "dieses", "dir", "doch", "dort", "du", "durch", "ein", "eine", "einem", "einen", "einer", "eines", "einig", "einige", "einigem", "einigen", "einiger", "einiges", "einmal", "er", "es", "etwas", "euch", "euer", "eure", "eurem", "euren", "eurer", "eures", "f\u00fcr", "gegen", "gewesen", "hab", "habe", "haben", "hat", "hatte", "hatten", "hier", "hin", "hinter", "ich", "ihm", "ihn", "ihnen", "ihr", "ihre", "ihrem", "ihren", "ihrer", "ihres", "im", "in", "indem", "ins", "ist", "jede", "jedem", "jeden", "jeder", "jedes", "jene", "jenem", "jenen", "jener", "jenes", "jetzt", "kann", "kein", "keine", "keinem", "keinen", "keiner", "keines", "k\u00f6nnen", "k\u00f6nnte", "machen", "man", "manche", "manchem", "manchen", "mancher", "manches", "mein", "meine", "meinem", "meinen", "meiner", "meines", "mich", "mir", "mit", "muss", "musste", "nach", "nicht", "nichts", "noch", "nun", "nur", "ob", "oder", "ohne", "sehr", "sein", "seine", "seinem", "seinen", "seiner", "seines", "selbst", "sich", "sie", "sind", "so", "solche", "solchem", "solchen", "solcher", "solches", "soll", "sollte", "sondern", "sonst", "um", "und", "uns", "unse", "unsem", "unsen", "unser", "unses", "unter", "viel", "vom", "von", "vor", "war", "waren", "warst", "was", "weg", "weil", "weiter", "welche", "welchem", "welchen", "welcher", "welches", "wenn", "werde", "werden", "wie", "wieder", "will", "wir", "wird", "wirst", "wo", "wollen", "wollte", "w\u00e4hrend", "w\u00fcrde", "w\u00fcrden", "zu", "zum", "zur", "zwar", "zwischen", "\u00fcber"];
 
 
 /* Non-minified version is copied as a separate JS file, is available */
 BaseStemmer = function() {
     this.setCurrent = function(r) {
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/nature.css` & `PyAPplus64-1.0.1/docs/build/html/_static/nature.css`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 /*
-Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
-
-This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
-
-Use of this source code is governed by an MIT-style
-license that can be found in the LICENSE file or at
-https://opensource.org/licenses/MIT.*/
+ * nature.css_t
+ * ~~~~~~~~~~~~
+ *
+ * Sphinx stylesheet -- nature theme.
+ *
+ * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :license: BSD, see LICENSE for details.
+ *
+ */
 
 @import url("basic.css");
 
 /* -- page layout ----------------------------------------------------------- */
 
 body {
     font-family: Arial, sans-serif;
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/pygments.css` & `PyAPplus64-1.0.1/docs/build/html/_static/pygments.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-/*
-Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
-
-This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
-
-Use of this source code is governed by an MIT-style
-license that can be found in the LICENSE file or at
-https://opensource.org/licenses/MIT.*/
 pre { line-height: 125%; }
 td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 .highlight .hll { background-color: #ffffcc }
 .highlight { background: #f8f8f8; }
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/searchtools.js` & `PyAPplus64-1.0.1/docs/build/html/_static/searchtools.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,17 @@
 /*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
+ * searchtools.js
+ * ~~~~~~~~~~~~~~~~
  *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
+ * Sphinx JavaScript utilities for the full-text search.
  *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
+ * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :license: BSD, see LICENSE for details.
+ *
+ */
 
 if (!Scorer) {
     /**
      * Simple result scoring code.
      */
     var Scorer = {
         // Implement the following function to further tweak the score for each result
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/translations.js` & `PyAPplus64-1.0.1/docs/build/html/_static/translations.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,7 @@
-/*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
- *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
- *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
 Documentation.addTranslations({
     "locale": "de",
     "messages": {
         "%(filename)s &#8212; %(docstitle)s": "",
         "&#169; <a href=\"%(path)s\">Copyright</a> %(copyright)s.": "",
         "&#169; Copyright %(copyright)s.": "",
         ", in ": ", in ",
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/_static/underscore.js` & `PyAPplus64-1.0.1/docs/build/html/_static/underscore.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,7 @@
-/*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
- *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
- *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
 (function(global, factory) {
     typeof exports === 'object' && typeof module !== 'undefined' ? module.exports = factory() :
         typeof define === 'function' && define.amd ? define('underscore', factory) :
         (global = typeof globalThis !== 'undefined' ? globalThis : global || self, (function() {
             var current = global._;
             var exports = global._ = factory();
             exports.noConflict = function() {
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/abhaengigkeiten.html` & `PyAPplus64-1.0.1/docs/build/html/abhaengigkeiten.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>Abhängigkeiten &#8212; PyAPplus64  Dokumentation</title>
+    <title>Abhängigkeiten &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/translations.js"></script>
@@ -38,15 +30,15 @@
              >Module</a> |</li>
         <li class="right" >
           <a href="examples.html" title="Beispiele"
              accesskey="N">weiter</a> |</li>
         <li class="right" >
           <a href="anwendungen.html" title="typische Anwendungsfälle"
              accesskey="P">zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Abhängigkeiten</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -145,15 +137,15 @@
              >Module</a> |</li>
         <li class="right" >
           <a href="examples.html" title="Beispiele"
              >weiter</a> |</li>
         <li class="right" >
           <a href="anwendungen.html" title="typische Anwendungsfälle"
              >zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Abhängigkeiten</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 
 
 **** Navigation ****
     * Index
     * Module |
     * weiter |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * AbhÃ¤ngigkeiten
 ****** AbhÃ¤ngigkeitenÂ¶ ******
 ***** pyodbcÂ¶ *****
 FÃ¼r die Datenbankverbindung wird pyodbc (python -m pip install pyodbc)
 verwendet. Der passende ODBC Treiber, MS SQL Server 2012 Native Client, wird
 zusÃ¤tzlich benÃ¶tigt. Dieser kann von Microsoft bezogen werden.
 
@@ -56,10 +56,10 @@
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
     * weiter |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * AbhÃ¤ngigkeiten
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/anwendungen.html` & `PyAPplus64-1.0.1/docs/build/html/anwendungen.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>typische Anwendungsfälle &#8212; PyAPplus64  Dokumentation</title>
+    <title>typische Anwendungsfälle &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/translations.js"></script>
@@ -38,15 +30,15 @@
              >Module</a> |</li>
         <li class="right" >
           <a href="abhaengigkeiten.html" title="Abhängigkeiten"
              accesskey="N">weiter</a> |</li>
         <li class="right" >
           <a href="beschreibung.html" title="Beschreibung"
              accesskey="P">zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">typische Anwendungsfälle</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -61,42 +53,43 @@
 Ich habe dies vor allem für Wartungsarbeiten an Anpassungstabellen, die für eigene Erweiterungen
 entwickelt wurden, genutzt.</p>
 <p>Als triviales Beispiel sucht folgender Code alle <cite>DOCUMENTS</cite> Einträge in
 Artikeln (angezeigt als <cite>Bild</cite> in <cite>ArtikelRec.aspx</cite>), für die Datei, auf die
 verwiesen wird, nicht im Dateisystem existiert. Diese fehlenden Dateien werden
 ausgegeben und das Feld <cite>DOCUMENTS</cite> gelöscht. Das Löschen erfolgt dabei über
 <cite>useXML</cite>, so dass die Felder <cite>UPDDATE</cite> und <cite>UPDUSER</cite> korrekt gesetzt werden.</p>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="c1">#</span>
-<span class="linenos"> 2</span><span class="c1"># Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)</span>
-<span class="linenos"> 3</span><span class="c1">#</span>
-<span class="linenos"> 4</span><span class="c1"># This file is part of PyAPplus64.</span>
-<span class="linenos"> 5</span><span class="c1">#</span>
-<span class="linenos"> 6</span><span class="kn">import</span> <span class="nn">pathlib</span>
-<span class="linenos"> 7</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
-<span class="linenos"> 8</span><span class="kn">import</span> <span class="nn">applus_configs</span>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">pathlib</span>
+<span class="linenos"> 2</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
+<span class="linenos"> 3</span><span class="kn">import</span> <span class="nn">applus_configs</span>
+<span class="linenos"> 4</span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Optional</span>
+<span class="linenos"> 5</span>
+<span class="linenos"> 6</span>
+<span class="linenos"> 7</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">updateDB</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">docDir</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos"> 8</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span>
 <span class="linenos"> 9</span>
-<span class="linenos">10</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span> <span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">docDir</span><span class="p">:</span><span class="nb">str</span><span class="p">,</span> <span class="n">updateDB</span><span class="p">:</span><span class="nb">bool</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos">11</span>  <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span> 
+<span class="linenos">10</span>    <span class="k">if</span> <span class="n">docDir</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">11</span>        <span class="n">docDir</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getInstallPathWebServer</span><span class="p">()</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="s2">&quot;DocLib&quot;</span><span class="p">))</span>
 <span class="linenos">12</span>
-<span class="linenos">13</span>  <span class="n">sql</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">);</span>
-<span class="linenos">14</span>  <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;ARTIKEL&quot;</span><span class="p">,</span> <span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">);</span>
-<span class="linenos">15</span>  <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addConditionFieldStringNotEmpty</span><span class="p">(</span><span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">);</span>
+<span class="linenos">13</span>    <span class="n">sql</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">)</span>
+<span class="linenos">14</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;ARTIKEL&quot;</span><span class="p">,</span> <span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">)</span>
+<span class="linenos">15</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addConditionFieldStringNotEmpty</span><span class="p">(</span><span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">)</span>
 <span class="linenos">16</span>
-<span class="linenos">17</span>  <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">server</span><span class="o">.</span><span class="n">dbQueryAll</span><span class="p">(</span><span class="n">sql</span><span class="p">):</span>
-<span class="linenos">18</span>    <span class="n">doc</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">docDir</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">DOCUMENTS</span><span class="p">);</span>
-<span class="linenos">19</span>    <span class="k">if</span> <span class="ow">not</span> <span class="n">doc</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-<span class="linenos">20</span>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Bild &#39;</span><span class="si">{}</span><span class="s2">&#39; für Artikel &#39;</span><span class="si">{}</span><span class="s2">&#39; nicht gefunden&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">doc</span><span class="p">,</span> <span class="n">row</span><span class="o">.</span><span class="n">ARTIKEL</span><span class="p">))</span>
-<span class="linenos">21</span>        
-<span class="linenos">22</span>        <span class="k">if</span> <span class="n">updateDB</span><span class="p">:</span>
-<span class="linenos">23</span>              <span class="n">upd</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">mkUseXMLRowUpdate</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">,</span> <span class="n">row</span><span class="o">.</span><span class="n">ID</span><span class="p">);</span>
-<span class="linenos">24</span>              <span class="n">upd</span><span class="o">.</span><span class="n">addField</span><span class="p">(</span><span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">,</span> <span class="kc">None</span><span class="p">);</span>
-<span class="linenos">25</span>              <span class="n">upd</span><span class="o">.</span><span class="n">update</span><span class="p">();</span>
+<span class="linenos">17</span>    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">server</span><span class="o">.</span><span class="n">dbQueryAll</span><span class="p">(</span><span class="n">sql</span><span class="p">):</span>
+<span class="linenos">18</span>        <span class="n">doc</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">docDir</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">DOCUMENTS</span><span class="p">)</span>
+<span class="linenos">19</span>        <span class="k">if</span> <span class="ow">not</span> <span class="n">doc</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+<span class="linenos">20</span>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Bild &#39;</span><span class="si">{}</span><span class="s2">&#39; für Artikel &#39;</span><span class="si">{}</span><span class="s2">&#39; nicht gefunden&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">doc</span><span class="p">,</span> <span class="n">row</span><span class="o">.</span><span class="n">ARTIKEL</span><span class="p">))</span>
+<span class="linenos">21</span>
+<span class="linenos">22</span>            <span class="k">if</span> <span class="n">updateDB</span><span class="p">:</span>
+<span class="linenos">23</span>                <span class="n">upd</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">mkUseXMLRowUpdate</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">,</span> <span class="n">row</span><span class="o">.</span><span class="n">ID</span><span class="p">)</span>
+<span class="linenos">24</span>                <span class="n">upd</span><span class="o">.</span><span class="n">addField</span><span class="p">(</span><span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+<span class="linenos">25</span>                <span class="n">upd</span><span class="o">.</span><span class="n">update</span><span class="p">()</span>
 <span class="linenos">26</span>
-<span class="linenos">27</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-<span class="linenos">28</span>  <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="s2">&quot;somedir</span><span class="se">\\</span><span class="s2">WebServer</span><span class="se">\\</span><span class="s2">DocLib&quot;</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+<span class="linenos">27</span>
+<span class="linenos">28</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">29</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
 </pre></div>
 </div>
 <p>Man kann alle Python Bibliotheken nutzen. Als Erweiterung wäre es in obigem Script
 zum Beispiel einfach möglich, alle BMP-Bilder zu suchen, nach PNG zu konvertieren
 und den DB-Eintrag anzupassen.</p>
 </section>
 <section id="ad-hoc-reports">
@@ -106,61 +99,56 @@
 <p>Für ad-hoc Reports, die nur sehr selten oder sogar nur einmal benutzt werden, ist die
 Erstellung eines Jasper-Reports und die Einbindung in APplus jedoch zu zeitaufwändig.
 Teilweise genügen die Ergebnisse einer SQL-Abfrage, die direkt im MS SQL Server abgesetzt
 werden kann. Wird es etwas komplizierter oder sollen die Ergebnisse noch etwas verarbeitet
 werden, bietet sich evtl. Python an.</p>
 <p>Folgendes Script erzeugt zum Beispiel eine Excel-Tabelle, mit einer Übersicht,
 welche Materialen wie oft für Artikel benutzt werden:</p>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="c1">#</span>
-<span class="linenos"> 2</span><span class="c1"># Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)</span>
-<span class="linenos"> 3</span><span class="c1">#</span>
-<span class="linenos"> 4</span><span class="c1"># This file is part of PyAPplus64.</span>
-<span class="linenos"> 5</span><span class="c1">#</span>
-<span class="linenos"> 6</span>
-<span class="linenos"> 7</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
-<span class="linenos"> 8</span><span class="kn">import</span> <span class="nn">applus_configs</span>
-<span class="linenos"> 9</span><span class="kn">import</span> <span class="nn">pathlib</span>
-<span class="linenos">10</span>
-<span class="linenos">11</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span> <span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">outfile</span> <span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos">12</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span> 
-<span class="linenos">13</span>
-<span class="linenos">14</span>    <span class="c1"># Einfache SQL-Anfrage </span>
-<span class="linenos">15</span>    <span class="n">sql1</span> <span class="o">=</span> <span class="p">(</span><span class="s2">&quot;select Material, count(*) as Anzahl from ARTIKEL &quot;</span>
-<span class="linenos">16</span>            <span class="s2">&quot;group by MATERIAL having MATERIAL is not null &quot;</span>
-<span class="linenos">17</span>            <span class="s2">&quot;order by Anzahl desc&quot;</span><span class="p">)</span>
-<span class="linenos">18</span>    <span class="n">df1</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql1</span><span class="p">)</span>
-<span class="linenos">19</span>
-<span class="linenos">20</span>    <span class="c1"># Sql Select-Statements können auch über SqlStatementSelect zusammengebaut</span>
-<span class="linenos">21</span>    <span class="c1"># werden. Die ist bei vielen, komplizierten Bedingungen teilweise hilfreich.</span>
-<span class="linenos">22</span>    <span class="n">sql2</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">)</span>        
-<span class="linenos">23</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;Material&quot;</span><span class="p">,</span> <span class="s2">&quot;count(*) as Anzahl&quot;</span><span class="p">)</span>
-<span class="linenos">24</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">addGroupBy</span><span class="p">(</span><span class="s2">&quot;MATERIAL&quot;</span><span class="p">)</span>
-<span class="linenos">25</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">having</span><span class="o">.</span><span class="n">addConditionFieldIsNotNull</span><span class="p">(</span><span class="s2">&quot;MATERIAL&quot;</span><span class="p">)</span>
-<span class="linenos">26</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">order</span> <span class="o">=</span> <span class="s2">&quot;Anzahl desc&quot;</span>
-<span class="linenos">27</span>    <span class="n">df2</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql2</span><span class="p">)</span>
-<span class="linenos">28</span>
-<span class="linenos">29</span>    <span class="c1"># Ausgabe als Excel mit 2 Blättern</span>
-<span class="linenos">30</span>    <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">exportToExcel</span><span class="p">(</span><span class="n">outfile</span><span class="p">,</span> <span class="p">[(</span><span class="n">df1</span><span class="p">,</span> <span class="s2">&quot;Materialien&quot;</span><span class="p">),</span> <span class="p">(</span><span class="n">df2</span><span class="p">,</span> <span class="s2">&quot;Materialien 2&quot;</span><span class="p">)],</span> <span class="n">addTable</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-<span class="linenos">31</span>
-<span class="linenos">32</span>
-<span class="linenos">33</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-<span class="linenos">34</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="s2">&quot;myout.xlsx&quot;</span><span class="p">)</span>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
+<span class="linenos"> 2</span><span class="kn">import</span> <span class="nn">applus_configs</span>
+<span class="linenos"> 3</span><span class="kn">import</span> <span class="nn">pathlib</span>
+<span class="linenos"> 4</span>
+<span class="linenos"> 5</span>
+<span class="linenos"> 6</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">outfile</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos"> 7</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span>
+<span class="linenos"> 8</span>
+<span class="linenos"> 9</span>    <span class="c1"># Einfache SQL-Anfrage</span>
+<span class="linenos">10</span>    <span class="n">sql1</span> <span class="o">=</span> <span class="p">(</span><span class="s2">&quot;select Material, count(*) as Anzahl from ARTIKEL &quot;</span>
+<span class="linenos">11</span>            <span class="s2">&quot;group by MATERIAL having MATERIAL is not null &quot;</span>
+<span class="linenos">12</span>            <span class="s2">&quot;order by Anzahl desc&quot;</span><span class="p">)</span>
+<span class="linenos">13</span>    <span class="n">df1</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql1</span><span class="p">)</span>
+<span class="linenos">14</span>
+<span class="linenos">15</span>    <span class="c1"># Sql Select-Statements können auch über SqlStatementSelect zusammengebaut</span>
+<span class="linenos">16</span>    <span class="c1"># werden. Die ist bei vielen, komplizierten Bedingungen teilweise hilfreich.</span>
+<span class="linenos">17</span>    <span class="n">sql2</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">)</span>
+<span class="linenos">18</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;Material&quot;</span><span class="p">,</span> <span class="s2">&quot;count(*) as Anzahl&quot;</span><span class="p">)</span>
+<span class="linenos">19</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">addGroupBy</span><span class="p">(</span><span class="s2">&quot;MATERIAL&quot;</span><span class="p">)</span>
+<span class="linenos">20</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">having</span><span class="o">.</span><span class="n">addConditionFieldIsNotNull</span><span class="p">(</span><span class="s2">&quot;MATERIAL&quot;</span><span class="p">)</span>
+<span class="linenos">21</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">order</span> <span class="o">=</span> <span class="s2">&quot;Anzahl desc&quot;</span>
+<span class="linenos">22</span>    <span class="n">df2</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql2</span><span class="p">)</span>
+<span class="linenos">23</span>
+<span class="linenos">24</span>    <span class="c1"># Ausgabe als Excel mit 2 Blättern</span>
+<span class="linenos">25</span>    <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">exportToExcel</span><span class="p">(</span><span class="n">outfile</span><span class="p">,</span> <span class="p">[(</span><span class="n">df1</span><span class="p">,</span> <span class="s2">&quot;Materialien&quot;</span><span class="p">),</span> <span class="p">(</span><span class="n">df2</span><span class="p">,</span> <span class="s2">&quot;Materialien 2&quot;</span><span class="p">)],</span> <span class="n">addTable</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+<span class="linenos">26</span>
+<span class="linenos">27</span>
+<span class="linenos">28</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">29</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="s2">&quot;myout.xlsx&quot;</span><span class="p">)</span>
 </pre></div>
 </div>
 <p>Dieses kurze Script nutzt Standard-Pandas Methoden zur Erzeugung der Excel-Datei. Allerdings
 sind diese Methoden in den Aufrufen von <cite>pandasReadSql</cite> und <cite>exportToExcel</cite> gekapselt,
 so dass der Aufruf sehr einfach ist. Zudem ist es sehr einfach, die Verbindung zur Datenbank
 und zum APP-Server mittels der YAML-Konfigdatei herzustellen. Bei diesem
 Aufruf kann optional ein Nutzer und eine Umgebung übergeben werden, die die Standard-Werte aus
 der YAML-Datei überschreiben. <cite>pandasReadSql</cite> nutzt intern <cite>completeSQL</cite>, so dass
 der für die Umgebung korrekte Mandant automatisch verwendet wird.</p>
 </section>
 <section id="anbindung-eigener-tools">
 <h2>Anbindung eigener Tools<a class="headerlink" href="#anbindung-eigener-tools" title="Link zu dieser Überschrift">¶</a></h2>
-<p>Ursprünglich wurde <cite>PyAPplus64</cite> für die Anbindung einer APplus-Anpassung geschrieben. Dieses ist
+<p>Ursprünglich wurde <cite>PyAPplus64</cite> für die Anbindung einer APplus-Anpassung geschrieben. Diese Anpassung ist
 als Windows-Service auf einem eigenen Rechner installiert und überwacht dort ein bestimmtes Verzeichnis.
 Bei Änderungen an Dateien in diesem Verzeichnis (Hinzufügen, Ändern, Löschen) werden die Dateien verarbeitet
 und die Ergebnisse an APplus gemeldet. Dafür werden DB-Operationen aber auch SOAP-Calls benutzt.
 Ebenso wird auf die SysConf zugegriffen.</p>
 <p>Viele solcher Anpassungen lassen sich gut und sinnvoll im App-Server einrichten und als Job regelmäßig aufrufen.
 Im konkreten Fall wird jedoch für die Verarbeitung der Dateien viel Rechenzeit benötigt. Dies würde dadurch
 verschlimmert, dass die Dateien nicht auf der gleichen Maschine wie der App-Server liegen und somit
@@ -245,15 +233,15 @@
              >Module</a> |</li>
         <li class="right" >
           <a href="abhaengigkeiten.html" title="Abhängigkeiten"
              >weiter</a> |</li>
         <li class="right" >
           <a href="beschreibung.html" title="Beschreibung"
              >zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">typische Anwendungsfälle</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -6,57 +6,59 @@
 
 
 **** Navigation ****
     * Index
     * Module |
     * weiter |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * typische AnwendungsfÃ¤lle
 ****** typische AnwendungsfÃ¤lleÂ¶ ******
 ***** einfache Admin-AufgabenÂ¶ *****
 Selten auftretende Admin-Aufgaben lassen sich gut mittels Python-Scripten
 automatisieren. Es ist sehr einfach mÃ¶glich, auf die DB, aber auch auf SOAP-
 Schnittstelle zuzugreifen. Ich habe dies vor allem fÃ¼r Wartungsarbeiten an
 Anpassungstabellen, die fÃ¼r eigene Erweiterungen entwickelt wurden, genutzt.
 Als triviales Beispiel sucht folgender Code alleDOCUMENTSEintrÃ¤ge in Artikeln
 (angezeigt alsBildinArtikelRec.aspx), fÃ¼r die Datei, auf die verwiesen wird,
 nicht im Dateisystem existiert. Diese fehlenden Dateien werden ausgegeben und
 das FeldDOCUMENTSgelÃ¶scht. Das LÃ¶schen erfolgt dabei Ã¼beruseXML, so dass die
 FelderUPDDATEundUPDUSERkorrekt gesetzt werden.
- 1#
- 2# Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
- 3#
- 4# This file is part of PyAPplus64.
- 5#
- 6import pathlib
- 7import PyAPplus64
- 8import applus_configs
+ 1import pathlib
+ 2import PyAPplus64
+ 3import applus_configs
+ 4from typing import Optional
+ 5
+ 6
+ 7def main(confFile: pathlib.Path, updateDB: bool, docDir: Optional[str] =
+None) -> None:
+ 8    server = PyAPplus64.applus.applusFromConfigFile(confFile)
  9
-10def main(confFile : pathlib.Path, docDir:str, updateDB:bool) -> None:
-11  server = PyAPplus64.applus.applusFromConfigFile(confFile)
+10    if docDir is None:
+11        docDir = str(server.scripttool.getInstallPathWebServer().joinpath
+("DocLib"))
 12
-13  sql = PyAPplus64.sql_utils.SqlStatementSelect("ARTIKEL");
-14  sql.addFields("ID", "ARTIKEL", "DOCUMENTS");
-15  sql.where.addConditionFieldStringNotEmpty("DOCUMENTS");
+13    sql = PyAPplus64.sql_utils.SqlStatementSelect("ARTIKEL")
+14    sql.addFields("ID", "ARTIKEL", "DOCUMENTS")
+15    sql.where.addConditionFieldStringNotEmpty("DOCUMENTS")
 16
-17  for row in server.dbQueryAll(sql):
-18    doc = pathlib.Path(docDir + row.DOCUMENTS);
-19    if not doc.exists():
-20        print("Bild '{}' fÃ¼r Artikel '{}' nicht gefunden".format(doc,
+17    for row in server.dbQueryAll(sql):
+18        doc = pathlib.Path(docDir + row.DOCUMENTS)
+19        if not doc.exists():
+20            print("Bild '{}' fÃ¼r Artikel '{}' nicht gefunden".format(doc,
 row.ARTIKEL))
 21
-22        if updateDB:
-23              upd = server.mkUseXMLRowUpdate("ARTIKEL", row.ID);
-24              upd.addField("DOCUMENTS", None);
-25              upd.update();
+22            if updateDB:
+23                upd = server.mkUseXMLRowUpdate("ARTIKEL", row.ID)
+24                upd.addField("DOCUMENTS", None)
+25                upd.update()
 26
-27if __name__ == "__main__":
-28  main(applus_configs.serverConfYamlTest, "somedir\\WebServer\\DocLib",
-False)
+27
+28if __name__ == "__main__":
+29    main(applus_configs.serverConfYamlTest, False)
 Man kann alle Python Bibliotheken nutzen. Als Erweiterung wÃ¤re es in obigem
 Script zum Beispiel einfach mÃ¶glich, alle BMP-Bilder zu suchen, nach PNG zu
 konvertieren und den DB-Eintrag anzupassen.
 
 ***** Ad-hoc ReportsÂ¶ *****
 APplus erlaubt es mittels Jasper-Reports, flexible und schÃ¶ne Reports zu
 erzeugen. Dies funktioniert gut und ist fÃ¼r regelmÃ¤Ãig benutzte Reports sehr
@@ -64,63 +66,58 @@
 FÃ¼r ad-hoc Reports, die nur sehr selten oder sogar nur einmal benutzt werden,
 ist die Erstellung eines Jasper-Reports und die Einbindung in APplus jedoch zu
 zeitaufwÃ¤ndig. Teilweise genÃ¼gen die Ergebnisse einer SQL-Abfrage, die direkt
 im MS SQL Server abgesetzt werden kann. Wird es etwas komplizierter oder sollen
 die Ergebnisse noch etwas verarbeitet werden, bietet sich evtl. Python an.
 Folgendes Script erzeugt zum Beispiel eine Excel-Tabelle, mit einer Ãbersicht,
 welche Materialen wie oft fÃ¼r Artikel benutzt werden:
- 1#
- 2# Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
- 3#
- 4# This file is part of PyAPplus64.
- 5#
- 6
- 7import PyAPplus64
- 8import applus_configs
- 9import pathlib
-10
-11def main(confFile : pathlib.Path, outfile : str) -> None:
-12    server = PyAPplus64.applus.applusFromConfigFile(confFile)
-13
-14    # Einfache SQL-Anfrage
-15    sql1 = ("select Material, count(*) as Anzahl from ARTIKEL "
-16            "group by MATERIAL having MATERIAL is not null "
-17            "order by Anzahl desc")
-18    df1 = PyAPplus64.pandas.pandasReadSql(server, sql1)
-19
-20    # Sql Select-Statements kÃ¶nnen auch Ã¼ber SqlStatementSelect
+ 1import PyAPplus64
+ 2import applus_configs
+ 3import pathlib
+ 4
+ 5
+ 6def main(confFile: pathlib.Path, outfile: str) -> None:
+ 7    server = PyAPplus64.applus.applusFromConfigFile(confFile)
+ 8
+ 9    # Einfache SQL-Anfrage
+10    sql1 = ("select Material, count(*) as Anzahl from ARTIKEL "
+11            "group by MATERIAL having MATERIAL is not null "
+12            "order by Anzahl desc")
+13    df1 = PyAPplus64.pandas.pandasReadSql(server, sql1)
+14
+15    # Sql Select-Statements kÃ¶nnen auch Ã¼ber SqlStatementSelect
 zusammengebaut
-21    # werden. Die ist bei vielen, komplizierten Bedingungen teilweise
+16    # werden. Die ist bei vielen, komplizierten Bedingungen teilweise
 hilfreich.
-22    sql2 = PyAPplus64.SqlStatementSelect("ARTIKEL")
-23    sql2.addFields("Material", "count(*) as Anzahl")
-24    sql2.addGroupBy("MATERIAL")
-25    sql2.having.addConditionFieldIsNotNull("MATERIAL")
-26    sql2.order = "Anzahl desc"
-27    df2 = PyAPplus64.pandas.pandasReadSql(server, sql2)
-28
-29    # Ausgabe als Excel mit 2 BlÃ¤ttern
-30    PyAPplus64.pandas.exportToExcel(outfile, [(df1, "Materialien"), (df2,
+17    sql2 = PyAPplus64.SqlStatementSelect("ARTIKEL")
+18    sql2.addFields("Material", "count(*) as Anzahl")
+19    sql2.addGroupBy("MATERIAL")
+20    sql2.having.addConditionFieldIsNotNull("MATERIAL")
+21    sql2.order = "Anzahl desc"
+22    df2 = PyAPplus64.pandas.pandasReadSql(server, sql2)
+23
+24    # Ausgabe als Excel mit 2 BlÃ¤ttern
+25    PyAPplus64.pandas.exportToExcel(outfile, [(df1, "Materialien"), (df2,
 "Materialien 2")], addTable=True)
-31
-32
-33if __name__ == "__main__":
-34    main(applus_configs.serverConfYamlTest, "myout.xlsx")
+26
+27
+28if __name__ == "__main__":
+29    main(applus_configs.serverConfYamlTest, "myout.xlsx")
 Dieses kurze Script nutzt Standard-Pandas Methoden zur Erzeugung der Excel-
 Datei. Allerdings sind diese Methoden in den Aufrufen
 vonpandasReadSqlundexportToExcelgekapselt, so dass der Aufruf sehr einfach ist.
 Zudem ist es sehr einfach, die Verbindung zur Datenbank und zum APP-Server
 mittels der YAML-Konfigdatei herzustellen. Bei diesem Aufruf kann optional ein
 Nutzer und eine Umgebung Ã¼bergeben werden, die die Standard-Werte aus der
 YAML-Datei Ã¼berschreiben.pandasReadSqlnutzt interncompleteSQL, so dass der
 fÃ¼r die Umgebung korrekte Mandant automatisch verwendet wird.
 
 ***** Anbindung eigener ToolsÂ¶ *****
 UrsprÃ¼nglich wurdePyAPplus64fÃ¼r die Anbindung einer APplus-Anpassung
-geschrieben. Dieses ist als Windows-Service auf einem eigenen Rechner
+geschrieben. Diese Anpassung ist als Windows-Service auf einem eigenen Rechner
 installiert und Ã¼berwacht dort ein bestimmtes Verzeichnis. Bei Ãnderungen an
 Dateien in diesem Verzeichnis (HinzufÃ¼gen, Ãndern, LÃ¶schen) werden die
 Dateien verarbeitet und die Ergebnisse an APplus gemeldet. DafÃ¼r werden DB-
 Operationen aber auch SOAP-Calls benutzt. Ebenso wird auf die SysConf
 zugegriffen.
 Viele solcher Anpassungen lassen sich gut und sinnvoll im App-Server einrichten
 und als Job regelmÃ¤Ãig aufrufen. Im konkreten Fall wird jedoch fÃ¼r die
@@ -161,10 +158,10 @@
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
     * weiter |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * typische AnwendungsfÃ¤lle
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/beschreibung.html` & `PyAPplus64-1.0.1/docs/build/html/beschreibung.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>Beschreibung &#8212; PyAPplus64  Dokumentation</title>
+    <title>Beschreibung &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/translations.js"></script>
@@ -38,15 +30,15 @@
              >Module</a> |</li>
         <li class="right" >
           <a href="anwendungen.html" title="typische Anwendungsfälle"
              accesskey="N">weiter</a> |</li>
         <li class="right" >
           <a href="index.html" title="PyAPplus64 Dokumentation"
              accesskey="P">zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Beschreibung</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -104,15 +96,15 @@
 <p>In <cite>PyAPplus64</cite> wurden die Features (vielleicht leicht verallgemeinert)
 implementiert, die ich für konkrete Aufgabenstellungen benötigte. Ich gehe davon
 aus, dass im Laufe der Zeit weitere Features hinzukommen.</p>
 <section id="warnung">
 <h2>Warnung<a class="headerlink" href="#warnung" title="Link zu dieser Überschrift">¶</a></h2>
 <p><cite>PyAPplus64</cite> erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige
 Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie
-<cite>PyAPplus64</cite> daher bitte vorsichtig. Zudem kann ich leider nicht garantieren, dass <cite>PyAPplus</cite> fehlerfrei ist.</p>
+<cite>PyAPplus64</cite> daher bitte vorsichtig. Zudem kann ich leider nicht garantieren, dass <cite>PyAPplus64</cite> fehlerfrei ist.</p>
 </section>
 </section>
 
 
             <div class="clearer"></div>
           </div>
         </div>
@@ -165,15 +157,15 @@
              >Module</a> |</li>
         <li class="right" >
           <a href="anwendungen.html" title="typische Anwendungsfälle"
              >weiter</a> |</li>
         <li class="right" >
           <a href="index.html" title="PyAPplus64 Dokumentation"
              >zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Beschreibung</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 
 
 **** Navigation ****
     * Index
     * Module |
     * weiter |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Beschreibung
 ****** BeschreibungÂ¶ ******
 Das PaketPyAPplus64enthÃ¤lt eine Sammlung von Python Tools fÃ¼r die Interaktion
 mit dem ERP-System APplus 6.4. Es sollte auch fÃ¼r andere APplus Versionen
 nÃ¼tzlich sein.
 Zielgruppe sind APplus-Administratoren und Anpassungs-
 Entwickler.PyAPplus64erlaubt u.a.
@@ -51,15 +51,15 @@
 InPyAPplus64wurden die Features (vielleicht leicht verallgemeinert)
 implementiert, die ich fÃ¼r konkrete Aufgabenstellungen benÃ¶tigte. Ich gehe
 davon aus, dass im Laufe der Zeit weitere Features hinzukommen.
 ***** WarnungÂ¶ *****
 PyAPplus64erlaubt den schreibenden Zugriff auf die APplus Datenbank und
 beliebige Aufrufe von SOAP-Methoden. UnsachgemÃ¤Ãe Nutzung kann Ihre Daten
 zerstÃ¶ren. Benutzen SiePyAPplus64daher bitte vorsichtig. Zudem kann ich leider
-nicht garantieren, dassPyAPplusfehlerfrei ist.
+nicht garantieren, dassPyAPplus64fehlerfrei ist.
 
 **** Inhaltsverzeichnis ****
     * Beschreibung
           o Warnung
 *** Vorheriges Thema ***
 PyAPplus64_Dokumentation
 *** NÃ¤chstes Thema ***
@@ -69,10 +69,10 @@
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
     * weiter |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Beschreibung
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/examples.html` & `PyAPplus64-1.0.1/docs/build/html/examples.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>Beispiele &#8212; PyAPplus64  Dokumentation</title>
+    <title>Beispiele &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/translations.js"></script>
@@ -38,15 +30,15 @@
              >Module</a> |</li>
         <li class="right" >
           <a href="generated/PyAPplus64.html" title="PyAPplus64 package"
              accesskey="N">weiter</a> |</li>
         <li class="right" >
           <a href="abhaengigkeiten.html" title="Abhängigkeiten"
              accesskey="P">zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Beispiele</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -78,406 +70,487 @@
 <span class="linenos">15</span><span class="nt">  db </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;APplusProd6&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
 <span class="linenos">16</span><span class="nt">  user </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;SA&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
 <span class="linenos">17</span><span class="nt">  password </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;your-db-password&quot;</span><span class="w"></span>
 <span class="linenos">18</span><span class="p p-Indicator">}</span><span class="w"></span>
 </pre></div>
 </div>
 <p>Damit nicht in jedem Script immer wieder neu die Konfig-Dateien ausgewählt werden müssen, werden die Konfigs für
-das Prod-, Test- und Deploy-System in <code class="docutils literal notranslate"><span class="pre">examples/applus_configs.py</span></code> hinterlegt. Diese wird in allen Scripten importiert,
+das Prod-, Test- und Deploy-System in <code class="docutils literal notranslate"><span class="pre">examples/applus_configs.py</span></code> hinterlegt. Diese Datei wird in allen Scripten importiert,
 so dass das Config-Verzeichnis und die darin enthaltenen Configs einfach zur Verfügung stehen.</p>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos">1</span><span class="kn">import</span> <span class="nn">pathlib</span>
 <span class="linenos">2</span>
 <span class="linenos">3</span><span class="n">basedir</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span>
 <span class="linenos">4</span><span class="n">configdir</span> <span class="o">=</span> <span class="n">basedir</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="s2">&quot;config&quot;</span><span class="p">)</span>
 <span class="linenos">5</span>
 <span class="linenos">6</span><span class="n">serverConfYamlDeploy</span> <span class="o">=</span> <span class="n">configdir</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="s2">&quot;applus-server-deploy.yaml&quot;</span><span class="p">)</span>
 <span class="linenos">7</span><span class="n">serverConfYamlTest</span> <span class="o">=</span> <span class="n">configdir</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="s2">&quot;applus-server-test.yaml&quot;</span><span class="p">)</span>
 <span class="linenos">8</span><span class="n">serverConfYamlProd</span> <span class="o">=</span> <span class="n">configdir</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="s2">&quot;applus-server-prod.yaml&quot;</span><span class="p">)</span>
-<span class="linenos">9</span>
+</pre></div>
+</div>
+</section>
+<section id="read-settings-py">
+<h2><code class="docutils literal notranslate"><span class="pre">read_settings.py</span></code><a class="headerlink" href="#read-settings-py" title="Link zu dieser Überschrift">¶</a></h2>
+<p>Einfaches Beispiel für Auslesen der SysConf und bestimmter Einstellungen.</p>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="c1"># Einfaches Script, das verschiedene Werte des Servers ausliest.</span>
+<span class="linenos"> 2</span><span class="c1"># Dies sind SysConfig-Einstellungen, aber auch der aktuelle Mandant,</span>
+<span class="linenos"> 3</span><span class="c1"># Systemnamen, ...</span>
+<span class="linenos"> 4</span>
+<span class="linenos"> 5</span><span class="kn">import</span> <span class="nn">pathlib</span>
+<span class="linenos"> 6</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
+<span class="linenos"> 7</span><span class="kn">import</span> <span class="nn">applus_configs</span>
+<span class="linenos"> 8</span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Optional</span><span class="p">,</span> <span class="n">Union</span>
+<span class="linenos"> 9</span>
+<span class="linenos">10</span>
+<span class="linenos">11</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">],</span> <span class="n">user</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">env</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">12</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">,</span> <span class="n">user</span><span class="o">=</span><span class="n">user</span><span class="p">,</span> <span class="n">env</span><span class="o">=</span><span class="n">env</span><span class="p">)</span>
+<span class="linenos">13</span>
+<span class="linenos">14</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n\n</span><span class="s2">SysConf Lookups:&quot;</span><span class="p">)</span>
+<span class="linenos">15</span>
+<span class="linenos">16</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  Default Auftragsart:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">sysconf</span><span class="o">.</span><span class="n">getString</span><span class="p">(</span><span class="s2">&quot;STAMM&quot;</span><span class="p">,</span> <span class="s2">&quot;DEFAULTAUFTRAGSART&quot;</span><span class="p">))</span>
+<span class="linenos">17</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  Auftragsarten:&quot;</span><span class="p">)</span>
+<span class="linenos">18</span>    <span class="n">arten</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">sysconf</span><span class="o">.</span><span class="n">getList</span><span class="p">(</span><span class="s2">&quot;STAMM&quot;</span><span class="p">,</span> <span class="s2">&quot;AUFTRAGSART&quot;</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span><span class="p">)</span>
+<span class="linenos">19</span>    <span class="k">if</span> <span class="ow">not</span> <span class="n">arten</span><span class="p">:</span>
+<span class="linenos">20</span>        <span class="n">arten</span> <span class="o">=</span> <span class="p">[]</span>
+<span class="linenos">21</span>    <span class="k">for</span> <span class="n">a</span> <span class="ow">in</span> <span class="n">arten</span><span class="p">:</span>
+<span class="linenos">22</span>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    - &quot;</span> <span class="o">+</span> <span class="n">a</span><span class="p">)</span>
+<span class="linenos">23</span>
+<span class="linenos">24</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  Firmen-Nr. automatisch vergeben:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">sysconf</span><span class="o">.</span><span class="n">getBoolean</span><span class="p">(</span><span class="s2">&quot;STAMM&quot;</span><span class="p">,</span> <span class="s2">&quot;FIRMAAUTOMATIK&quot;</span><span class="p">))</span>
+<span class="linenos">25</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  Anzahl Artikelstellen:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">sysconf</span><span class="o">.</span><span class="n">getInt</span><span class="p">(</span><span class="s2">&quot;STAMM&quot;</span><span class="p">,</span> <span class="s2">&quot;ARTKLASSIFNRLAENGE&quot;</span><span class="p">))</span>
+<span class="linenos">26</span>
+<span class="linenos">27</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n\n</span><span class="s2">ScriptTool:&quot;</span><span class="p">)</span>
+<span class="linenos">28</span>
+<span class="linenos">29</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  CurrentDate:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getCurrentDate</span><span class="p">())</span>
+<span class="linenos">30</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  CurrentTime:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getCurrentTime</span><span class="p">())</span>
+<span class="linenos">31</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  CurrentDateTime:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getCurrentDateTime</span><span class="p">())</span>
+<span class="linenos">32</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  LoginName:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getLoginName</span><span class="p">())</span>
+<span class="linenos">33</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  UserName:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getUserName</span><span class="p">())</span>
+<span class="linenos">34</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  UserFullName:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getUserFullName</span><span class="p">())</span>
+<span class="linenos">35</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  SystemName:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getSystemName</span><span class="p">())</span>
+<span class="linenos">36</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  Mandant:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getMandant</span><span class="p">())</span>
+<span class="linenos">37</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  MandantName:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getMandantName</span><span class="p">())</span>
+<span class="linenos">38</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  InstallPath:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getInstallPath</span><span class="p">())</span>
+<span class="linenos">39</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  InstallPathAppServer:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getInstallPathAppServer</span><span class="p">())</span>
+<span class="linenos">40</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  InstallPathWebServer:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getInstallPathWebServer</span><span class="p">())</span>
+<span class="linenos">41</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  ServerInfo - Version:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getServerInfo</span><span class="p">()</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;version&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">text</span><span class="p">)</span>
+<span class="linenos">42</span>
+<span class="linenos">43</span>
+<span class="linenos">44</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">45</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">)</span>
 </pre></div>
 </div>
 </section>
 <section id="check-dokumente-py">
 <h2><code class="docutils literal notranslate"><span class="pre">check_dokumente.py</span></code><a class="headerlink" href="#check-dokumente-py" title="Link zu dieser Überschrift">¶</a></h2>
 <p>Einfaches Beispiel für lesenden und schreibenden Zugriff auf APplus Datenbank.</p>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">pathlib</span>
 <span class="linenos"> 2</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
 <span class="linenos"> 3</span><span class="kn">import</span> <span class="nn">applus_configs</span>
-<span class="linenos"> 4</span>
-<span class="linenos"> 5</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span> <span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">docDir</span><span class="p">:</span><span class="nb">str</span><span class="p">,</span> <span class="n">updateDB</span><span class="p">:</span><span class="nb">bool</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos"> 6</span>  <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span> 
-<span class="linenos"> 7</span>
-<span class="linenos"> 8</span>  <span class="n">sql</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">);</span>
-<span class="linenos"> 9</span>  <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;ARTIKEL&quot;</span><span class="p">,</span> <span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">);</span>
-<span class="linenos">10</span>  <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addConditionFieldStringNotEmpty</span><span class="p">(</span><span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">);</span>
-<span class="linenos">11</span>
-<span class="linenos">12</span>  <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">server</span><span class="o">.</span><span class="n">dbQueryAll</span><span class="p">(</span><span class="n">sql</span><span class="p">):</span>
-<span class="linenos">13</span>    <span class="n">doc</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">docDir</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">DOCUMENTS</span><span class="p">);</span>
-<span class="linenos">14</span>    <span class="k">if</span> <span class="ow">not</span> <span class="n">doc</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-<span class="linenos">15</span>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Bild &#39;</span><span class="si">{}</span><span class="s2">&#39; für Artikel &#39;</span><span class="si">{}</span><span class="s2">&#39; nicht gefunden&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">doc</span><span class="p">,</span> <span class="n">row</span><span class="o">.</span><span class="n">ARTIKEL</span><span class="p">))</span>
-<span class="linenos">16</span>        
-<span class="linenos">17</span>        <span class="k">if</span> <span class="n">updateDB</span><span class="p">:</span>
-<span class="linenos">18</span>              <span class="n">upd</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">mkUseXMLRowUpdate</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">,</span> <span class="n">row</span><span class="o">.</span><span class="n">ID</span><span class="p">);</span>
-<span class="linenos">19</span>              <span class="n">upd</span><span class="o">.</span><span class="n">addField</span><span class="p">(</span><span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">,</span> <span class="kc">None</span><span class="p">);</span>
-<span class="linenos">20</span>              <span class="n">upd</span><span class="o">.</span><span class="n">update</span><span class="p">();</span>
+<span class="linenos"> 4</span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Optional</span>
+<span class="linenos"> 5</span>
+<span class="linenos"> 6</span>
+<span class="linenos"> 7</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">updateDB</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">docDir</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos"> 8</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span>
+<span class="linenos"> 9</span>
+<span class="linenos">10</span>    <span class="k">if</span> <span class="n">docDir</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">11</span>        <span class="n">docDir</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getInstallPathWebServer</span><span class="p">()</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="s2">&quot;DocLib&quot;</span><span class="p">))</span>
+<span class="linenos">12</span>
+<span class="linenos">13</span>    <span class="n">sql</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">)</span>
+<span class="linenos">14</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;ARTIKEL&quot;</span><span class="p">,</span> <span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">)</span>
+<span class="linenos">15</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addConditionFieldStringNotEmpty</span><span class="p">(</span><span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">)</span>
+<span class="linenos">16</span>
+<span class="linenos">17</span>    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">server</span><span class="o">.</span><span class="n">dbQueryAll</span><span class="p">(</span><span class="n">sql</span><span class="p">):</span>
+<span class="linenos">18</span>        <span class="n">doc</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">docDir</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">DOCUMENTS</span><span class="p">)</span>
+<span class="linenos">19</span>        <span class="k">if</span> <span class="ow">not</span> <span class="n">doc</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+<span class="linenos">20</span>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Bild &#39;</span><span class="si">{}</span><span class="s2">&#39; für Artikel &#39;</span><span class="si">{}</span><span class="s2">&#39; nicht gefunden&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">doc</span><span class="p">,</span> <span class="n">row</span><span class="o">.</span><span class="n">ARTIKEL</span><span class="p">))</span>
 <span class="linenos">21</span>
-<span class="linenos">22</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-<span class="linenos">23</span>  <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="s2">&quot;somedir</span><span class="se">\\</span><span class="s2">WebServer</span><span class="se">\\</span><span class="s2">DocLib&quot;</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+<span class="linenos">22</span>            <span class="k">if</span> <span class="n">updateDB</span><span class="p">:</span>
+<span class="linenos">23</span>                <span class="n">upd</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">mkUseXMLRowUpdate</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">,</span> <span class="n">row</span><span class="o">.</span><span class="n">ID</span><span class="p">)</span>
+<span class="linenos">24</span>                <span class="n">upd</span><span class="o">.</span><span class="n">addField</span><span class="p">(</span><span class="s2">&quot;DOCUMENTS&quot;</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+<span class="linenos">25</span>                <span class="n">upd</span><span class="o">.</span><span class="n">update</span><span class="p">()</span>
+<span class="linenos">26</span>
+<span class="linenos">27</span>
+<span class="linenos">28</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">29</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
 </pre></div>
 </div>
 </section>
 <section id="adhoc-report-py">
 <h2><code class="docutils literal notranslate"><span class="pre">adhoc_report.py</span></code><a class="headerlink" href="#adhoc-report-py" title="Link zu dieser Überschrift">¶</a></h2>
 <p>Sehr einfaches Beispiel zur Erstellung einer Excel-Tabelle aus einer SQL-Abfrage.</p>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
 <span class="linenos"> 2</span><span class="kn">import</span> <span class="nn">applus_configs</span>
 <span class="linenos"> 3</span><span class="kn">import</span> <span class="nn">pathlib</span>
 <span class="linenos"> 4</span>
-<span class="linenos"> 5</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span> <span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">outfile</span> <span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos"> 6</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span> 
-<span class="linenos"> 7</span>
-<span class="linenos"> 8</span>    <span class="c1"># Einfache SQL-Anfrage </span>
-<span class="linenos"> 9</span>    <span class="n">sql1</span> <span class="o">=</span> <span class="p">(</span><span class="s2">&quot;select Material, count(*) as Anzahl from ARTIKEL &quot;</span>
-<span class="linenos">10</span>            <span class="s2">&quot;group by MATERIAL having MATERIAL is not null &quot;</span>
-<span class="linenos">11</span>            <span class="s2">&quot;order by Anzahl desc&quot;</span><span class="p">)</span>
-<span class="linenos">12</span>    <span class="n">df1</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql1</span><span class="p">)</span>
-<span class="linenos">13</span>
-<span class="linenos">14</span>    <span class="c1"># Sql Select-Statements können auch über SqlStatementSelect zusammengebaut</span>
-<span class="linenos">15</span>    <span class="c1"># werden. Die ist bei vielen, komplizierten Bedingungen teilweise hilfreich.</span>
-<span class="linenos">16</span>    <span class="n">sql2</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">)</span>        
-<span class="linenos">17</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;Material&quot;</span><span class="p">,</span> <span class="s2">&quot;count(*) as Anzahl&quot;</span><span class="p">)</span>
-<span class="linenos">18</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">addGroupBy</span><span class="p">(</span><span class="s2">&quot;MATERIAL&quot;</span><span class="p">)</span>
-<span class="linenos">19</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">having</span><span class="o">.</span><span class="n">addConditionFieldIsNotNull</span><span class="p">(</span><span class="s2">&quot;MATERIAL&quot;</span><span class="p">)</span>
-<span class="linenos">20</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">order</span> <span class="o">=</span> <span class="s2">&quot;Anzahl desc&quot;</span>
-<span class="linenos">21</span>    <span class="n">df2</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql2</span><span class="p">)</span>
-<span class="linenos">22</span>
-<span class="linenos">23</span>    <span class="c1"># Ausgabe als Excel mit 2 Blättern</span>
-<span class="linenos">24</span>    <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">exportToExcel</span><span class="p">(</span><span class="n">outfile</span><span class="p">,</span> <span class="p">[(</span><span class="n">df1</span><span class="p">,</span> <span class="s2">&quot;Materialien&quot;</span><span class="p">),</span> <span class="p">(</span><span class="n">df2</span><span class="p">,</span> <span class="s2">&quot;Materialien 2&quot;</span><span class="p">)],</span> <span class="n">addTable</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-<span class="linenos">25</span>
+<span class="linenos"> 5</span>
+<span class="linenos"> 6</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">outfile</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos"> 7</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span>
+<span class="linenos"> 8</span>
+<span class="linenos"> 9</span>    <span class="c1"># Einfache SQL-Anfrage</span>
+<span class="linenos">10</span>    <span class="n">sql1</span> <span class="o">=</span> <span class="p">(</span><span class="s2">&quot;select Material, count(*) as Anzahl from ARTIKEL &quot;</span>
+<span class="linenos">11</span>            <span class="s2">&quot;group by MATERIAL having MATERIAL is not null &quot;</span>
+<span class="linenos">12</span>            <span class="s2">&quot;order by Anzahl desc&quot;</span><span class="p">)</span>
+<span class="linenos">13</span>    <span class="n">df1</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql1</span><span class="p">)</span>
+<span class="linenos">14</span>
+<span class="linenos">15</span>    <span class="c1"># Sql Select-Statements können auch über SqlStatementSelect zusammengebaut</span>
+<span class="linenos">16</span>    <span class="c1"># werden. Die ist bei vielen, komplizierten Bedingungen teilweise hilfreich.</span>
+<span class="linenos">17</span>    <span class="n">sql2</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;ARTIKEL&quot;</span><span class="p">)</span>
+<span class="linenos">18</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;Material&quot;</span><span class="p">,</span> <span class="s2">&quot;count(*) as Anzahl&quot;</span><span class="p">)</span>
+<span class="linenos">19</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">addGroupBy</span><span class="p">(</span><span class="s2">&quot;MATERIAL&quot;</span><span class="p">)</span>
+<span class="linenos">20</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">having</span><span class="o">.</span><span class="n">addConditionFieldIsNotNull</span><span class="p">(</span><span class="s2">&quot;MATERIAL&quot;</span><span class="p">)</span>
+<span class="linenos">21</span>    <span class="n">sql2</span><span class="o">.</span><span class="n">order</span> <span class="o">=</span> <span class="s2">&quot;Anzahl desc&quot;</span>
+<span class="linenos">22</span>    <span class="n">df2</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql2</span><span class="p">)</span>
+<span class="linenos">23</span>
+<span class="linenos">24</span>    <span class="c1"># Ausgabe als Excel mit 2 Blättern</span>
+<span class="linenos">25</span>    <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">exportToExcel</span><span class="p">(</span><span class="n">outfile</span><span class="p">,</span> <span class="p">[(</span><span class="n">df1</span><span class="p">,</span> <span class="s2">&quot;Materialien&quot;</span><span class="p">),</span> <span class="p">(</span><span class="n">df2</span><span class="p">,</span> <span class="s2">&quot;Materialien 2&quot;</span><span class="p">)],</span> <span class="n">addTable</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
 <span class="linenos">26</span>
-<span class="linenos">27</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-<span class="linenos">28</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="s2">&quot;myout.xlsx&quot;</span><span class="p">)</span>
+<span class="linenos">27</span>
+<span class="linenos">28</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">29</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="s2">&quot;myout.xlsx&quot;</span><span class="p">)</span>
 </pre></div>
 </div>
 </section>
 <section id="mengenabweichung-py">
 <h2><code class="docutils literal notranslate"><span class="pre">mengenabweichung.py</span></code><a class="headerlink" href="#mengenabweichung-py" title="Link zu dieser Überschrift">¶</a></h2>
 <p>Etwas komplizierteres Beispiel zur Erstellung einer Excel-Datei aus SQL-Abfragen.</p>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos">  1</span><span class="kn">import</span> <span class="nn">datetime</span>
-<span class="linenos">  2</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
-<span class="linenos">  3</span><span class="kn">import</span> <span class="nn">applus_configs</span>
-<span class="linenos">  4</span><span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span> <span class="c1"># type: ignore</span>
-<span class="linenos">  5</span><span class="kn">import</span> <span class="nn">pathlib</span>
-<span class="linenos">  6</span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="o">*</span>
-<span class="linenos">  7</span>
-<span class="linenos">  8</span><span class="k">def</span> <span class="nf">ladeAlleWerkstattauftragMengenabweichungen</span><span class="p">(</span>
-<span class="linenos">  9</span>        <span class="n">server</span><span class="p">:</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> 
-<span class="linenos"> 10</span>        <span class="n">cond</span><span class="p">:</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlCondition</span><span class="o">|</span><span class="nb">str</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-<span class="linenos"> 11</span>    <span class="n">sql</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;WAUFTRAG w&quot;</span><span class="p">);</span>
-<span class="linenos"> 12</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addLeftJoin</span><span class="p">(</span><span class="s2">&quot;personal p&quot;</span><span class="p">,</span> <span class="s2">&quot;w.UPDUSER = p.PERSONAL&quot;</span><span class="p">)</span>
-<span class="linenos"> 13</span>
-<span class="linenos"> 14</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFieldsTable</span><span class="p">(</span><span class="s2">&quot;w&quot;</span><span class="p">,</span> <span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;BAUFTRAG&quot;</span><span class="p">,</span> <span class="s2">&quot;POSITION&quot;</span><span class="p">)</span>
-<span class="linenos"> 15</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG&quot;</span><span class="p">)</span>
-<span class="linenos"> 16</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFieldsTable</span><span class="p">(</span><span class="s2">&quot;w&quot;</span><span class="p">,</span> <span class="s2">&quot;MENGE&quot;</span><span class="p">,</span> <span class="s2">&quot;MENGE_IST&quot;</span><span class="p">,</span> 
-<span class="linenos"> 17</span>                       <span class="s2">&quot;APLAN as ARTIKEL&quot;</span><span class="p">,</span> <span class="s2">&quot;NAME as ARTIKELNAME&quot;</span><span class="p">)</span>
-<span class="linenos"> 18</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;w.UPDDATE&quot;</span><span class="p">,</span> <span class="s2">&quot;p.NAME as UPDNAME&quot;</span><span class="p">)</span>
-<span class="linenos"> 19</span>
-<span class="linenos"> 20</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addConditionFieldGe</span><span class="p">(</span><span class="s2">&quot;w.STATUS&quot;</span><span class="p">,</span> <span class="mi">5</span><span class="p">)</span>
-<span class="linenos"> 21</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addCondition</span><span class="p">(</span><span class="s2">&quot;abs(w.MENGE-w.MENGE_IST) &gt; 0.001&quot;</span><span class="p">)</span>    
-<span class="linenos"> 22</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addCondition</span><span class="p">(</span><span class="n">cond</span><span class="p">)</span>
-<span class="linenos"> 23</span>    <span class="n">sql</span><span class="o">.</span><span class="n">order</span><span class="o">=</span><span class="s2">&quot;w.UPDDATE&quot;</span>
-<span class="linenos"> 24</span>    <span class="n">dfOrg</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql</span><span class="p">);</span>
-<span class="linenos"> 25</span>
-<span class="linenos"> 26</span>    <span class="c1"># Add Links</span>
-<span class="linenos"> 27</span>    <span class="n">df</span> <span class="o">=</span> <span class="n">dfOrg</span><span class="o">.</span><span class="n">copy</span><span class="p">();</span>
-<span class="linenos"> 28</span>    <span class="n">df</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;ID&quot;</span><span class="p">]);</span>
-<span class="linenos"> 29</span>    <span class="c1"># df = df[[&#39;POSITION&#39;, &#39;BAUFTRAG&#39;, &#39;MENGE&#39;]] # reorder / filter columns</span>
-<span class="linenos"> 30</span>
-<span class="linenos"> 31</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;POSITION&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span><span class="n">dfOrg</span><span class="p">,</span> 
-<span class="linenos"> 32</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">POSITION</span><span class="p">,</span> 
-<span class="linenos"> 33</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkWauftrag</span><span class="p">(</span>
-<span class="linenos"> 34</span>                            <span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span> <span class="n">accessid</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">ID</span><span class="p">))</span>
-<span class="linenos"> 35</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;BAUFTRAG&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span><span class="n">dfOrg</span><span class="p">,</span> 
-<span class="linenos"> 36</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span> 
-<span class="linenos"> 37</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkBauftrag</span><span class="p">(</span><span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">))</span>
-<span class="linenos"> 38</span>
-<span class="linenos"> 39</span>    <span class="n">colNames</span> <span class="o">=</span> <span class="p">{</span>
-<span class="linenos"> 40</span>        <span class="s2">&quot;BAUFTRAG&quot;</span> <span class="p">:</span> <span class="s2">&quot;Betriebsauftrag&quot;</span><span class="p">,</span>
-<span class="linenos"> 41</span>        <span class="s2">&quot;POSITION&quot;</span> <span class="p">:</span> <span class="s2">&quot;Pos&quot;</span><span class="p">,</span>
-<span class="linenos"> 42</span>        <span class="s2">&quot;MENGENABWEICHUNG&quot;</span> <span class="p">:</span> <span class="s2">&quot;Mengenabweichung&quot;</span><span class="p">,</span>
-<span class="linenos"> 43</span>        <span class="s2">&quot;MENGE&quot;</span> <span class="p">:</span> <span class="s2">&quot;Menge&quot;</span><span class="p">,</span>
-<span class="linenos"> 44</span>        <span class="s2">&quot;MENGE_IST&quot;</span> <span class="p">:</span> <span class="s2">&quot;Menge-Ist&quot;</span><span class="p">,</span>
-<span class="linenos"> 45</span>        <span class="s2">&quot;ARTIKEL&quot;</span> <span class="p">:</span> <span class="s2">&quot;Artikel&quot;</span><span class="p">,</span>
-<span class="linenos"> 46</span>        <span class="s2">&quot;ARTIKELNAME&quot;</span> <span class="p">:</span> <span class="s2">&quot;Artikel-Name&quot;</span><span class="p">,</span>
-<span class="linenos"> 47</span>        <span class="s2">&quot;UPDDATE&quot;</span> <span class="p">:</span> <span class="s2">&quot;geändert am&quot;</span><span class="p">,</span>
-<span class="linenos"> 48</span>        <span class="s2">&quot;UPDNAME&quot;</span> <span class="p">:</span> <span class="s2">&quot;geändert von&quot;</span>
-<span class="linenos"> 49</span>    <span class="p">}</span>
-<span class="linenos"> 50</span>    <span class="n">df</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="n">colNames</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">);</span>
-<span class="linenos"> 51</span>
-<span class="linenos"> 52</span>    <span class="k">return</span> <span class="n">df</span>
-<span class="linenos"> 53</span>
-<span class="linenos"> 54</span>
-<span class="linenos"> 55</span><span class="k">def</span> <span class="nf">ladeAlleWerkstattauftragPosMengenabweichungen</span><span class="p">(</span>
-<span class="linenos"> 56</span>        <span class="n">server</span> <span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> 
-<span class="linenos"> 57</span>        <span class="n">cond</span><span class="p">:</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlCondition</span><span class="o">|</span><span class="nb">str</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-<span class="linenos"> 58</span>    <span class="n">sql</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;WAUFTRAGPOS w&quot;</span><span class="p">);</span>
-<span class="linenos"> 59</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addLeftJoin</span><span class="p">(</span><span class="s2">&quot;personal p&quot;</span><span class="p">,</span> <span class="s2">&quot;w.UPDUSER = p.PERSONAL&quot;</span><span class="p">)</span>
-<span class="linenos"> 60</span>
-<span class="linenos"> 61</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFieldsTable</span><span class="p">(</span><span class="s2">&quot;w&quot;</span><span class="p">,</span> <span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;BAUFTRAG&quot;</span><span class="p">,</span> <span class="s2">&quot;POSITION&quot;</span><span class="p">,</span> <span class="s2">&quot;AG&quot;</span><span class="p">)</span>
-<span class="linenos"> 62</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG&quot;</span><span class="p">)</span>
-<span class="linenos"> 63</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFieldsTable</span><span class="p">(</span><span class="s2">&quot;w&quot;</span><span class="p">,</span> <span class="s2">&quot;MENGE&quot;</span><span class="p">,</span> <span class="s2">&quot;MENGE_IST&quot;</span><span class="p">,</span> <span class="s2">&quot;APLAN as ARTIKEL&quot;</span><span class="p">)</span>
-<span class="linenos"> 64</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;w.UPDDATE&quot;</span><span class="p">,</span> <span class="s2">&quot;p.NAME as UPDNAME&quot;</span><span class="p">)</span>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos">  1</span><span class="c1"># Erzeugt Excel-Tabellen mit Werkstattaufträgen und Werkstattauftragspositionen mit Mengenabweichungen</span>
+<span class="linenos">  2</span>
+<span class="linenos">  3</span><span class="kn">import</span> <span class="nn">datetime</span>
+<span class="linenos">  4</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
+<span class="linenos">  5</span><span class="kn">import</span> <span class="nn">applus_configs</span>
+<span class="linenos">  6</span><span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>  <span class="c1"># type: ignore</span>
+<span class="linenos">  7</span><span class="kn">import</span> <span class="nn">pathlib</span>
+<span class="linenos">  8</span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Tuple</span><span class="p">,</span> <span class="n">Union</span><span class="p">,</span> <span class="n">Optional</span>
+<span class="linenos">  9</span>
+<span class="linenos"> 10</span>
+<span class="linenos"> 11</span><span class="k">def</span> <span class="nf">ladeAlleWerkstattauftragMengenabweichungen</span><span class="p">(</span>
+<span class="linenos"> 12</span>        <span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span>
+<span class="linenos"> 13</span>        <span class="n">cond</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlCondition</span><span class="p">,</span> <span class="nb">str</span><span class="p">,</span> <span class="kc">None</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+<span class="linenos"> 14</span>    <span class="n">sql</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;WAUFTRAG w&quot;</span><span class="p">)</span>
+<span class="linenos"> 15</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addLeftJoin</span><span class="p">(</span><span class="s2">&quot;personal p&quot;</span><span class="p">,</span> <span class="s2">&quot;w.UPDUSER = p.PERSONAL&quot;</span><span class="p">)</span>
+<span class="linenos"> 16</span>
+<span class="linenos"> 17</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFieldsTable</span><span class="p">(</span><span class="s2">&quot;w&quot;</span><span class="p">,</span> <span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;BAUFTRAG&quot;</span><span class="p">,</span> <span class="s2">&quot;POSITION&quot;</span><span class="p">)</span>
+<span class="linenos"> 18</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG&quot;</span><span class="p">)</span>
+<span class="linenos"> 19</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFieldsTable</span><span class="p">(</span><span class="s2">&quot;w&quot;</span><span class="p">,</span> <span class="s2">&quot;MENGE&quot;</span><span class="p">,</span> <span class="s2">&quot;MENGE_IST&quot;</span><span class="p">,</span>
+<span class="linenos"> 20</span>                       <span class="s2">&quot;APLAN as ARTIKEL&quot;</span><span class="p">,</span> <span class="s2">&quot;NAME as ARTIKELNAME&quot;</span><span class="p">)</span>
+<span class="linenos"> 21</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;w.UPDDATE&quot;</span><span class="p">,</span> <span class="s2">&quot;p.NAME as UPDNAME&quot;</span><span class="p">)</span>
+<span class="linenos"> 22</span>
+<span class="linenos"> 23</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addConditionFieldGe</span><span class="p">(</span><span class="s2">&quot;w.STATUS&quot;</span><span class="p">,</span> <span class="mi">5</span><span class="p">)</span>
+<span class="linenos"> 24</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addCondition</span><span class="p">(</span><span class="s2">&quot;abs(w.MENGE-w.MENGE_IST) &gt; 0.001&quot;</span><span class="p">)</span>
+<span class="linenos"> 25</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addCondition</span><span class="p">(</span><span class="n">cond</span><span class="p">)</span>
+<span class="linenos"> 26</span>    <span class="n">sql</span><span class="o">.</span><span class="n">order</span> <span class="o">=</span> <span class="s2">&quot;w.UPDDATE&quot;</span>
+<span class="linenos"> 27</span>    <span class="n">dfOrg</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql</span><span class="p">)</span>
+<span class="linenos"> 28</span>
+<span class="linenos"> 29</span>    <span class="c1"># Add Links</span>
+<span class="linenos"> 30</span>    <span class="n">df</span> <span class="o">=</span> <span class="n">dfOrg</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span>
+<span class="linenos"> 31</span>    <span class="n">df</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;ID&quot;</span><span class="p">])</span>
+<span class="linenos"> 32</span>    <span class="c1"># df = df[[&#39;POSITION&#39;, &#39;BAUFTRAG&#39;, &#39;MENGE&#39;]] # reorder / filter columns</span>
+<span class="linenos"> 33</span>
+<span class="linenos"> 34</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;POSITION&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span>
+<span class="linenos"> 35</span>                        <span class="n">dfOrg</span><span class="p">,</span>
+<span class="linenos"> 36</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">POSITION</span><span class="p">,</span>
+<span class="linenos"> 37</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkWauftrag</span><span class="p">(</span>
+<span class="linenos"> 38</span>                            <span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span> <span class="n">accessid</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">ID</span><span class="p">))</span>
+<span class="linenos"> 39</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;BAUFTRAG&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span>
+<span class="linenos"> 40</span>                        <span class="n">dfOrg</span><span class="p">,</span>
+<span class="linenos"> 41</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span>
+<span class="linenos"> 42</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkBauftrag</span><span class="p">(</span><span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">))</span>
+<span class="linenos"> 43</span>
+<span class="linenos"> 44</span>    <span class="n">colNames</span> <span class="o">=</span> <span class="p">{</span>
+<span class="linenos"> 45</span>        <span class="s2">&quot;BAUFTRAG&quot;</span><span class="p">:</span> <span class="s2">&quot;Betriebsauftrag&quot;</span><span class="p">,</span>
+<span class="linenos"> 46</span>        <span class="s2">&quot;POSITION&quot;</span><span class="p">:</span> <span class="s2">&quot;Pos&quot;</span><span class="p">,</span>
+<span class="linenos"> 47</span>        <span class="s2">&quot;MENGENABWEICHUNG&quot;</span><span class="p">:</span> <span class="s2">&quot;Mengenabweichung&quot;</span><span class="p">,</span>
+<span class="linenos"> 48</span>        <span class="s2">&quot;MENGE&quot;</span><span class="p">:</span> <span class="s2">&quot;Menge&quot;</span><span class="p">,</span>
+<span class="linenos"> 49</span>        <span class="s2">&quot;MENGE_IST&quot;</span><span class="p">:</span> <span class="s2">&quot;Menge-Ist&quot;</span><span class="p">,</span>
+<span class="linenos"> 50</span>        <span class="s2">&quot;ARTIKEL&quot;</span><span class="p">:</span> <span class="s2">&quot;Artikel&quot;</span><span class="p">,</span>
+<span class="linenos"> 51</span>        <span class="s2">&quot;ARTIKELNAME&quot;</span><span class="p">:</span> <span class="s2">&quot;Artikel-Name&quot;</span><span class="p">,</span>
+<span class="linenos"> 52</span>        <span class="s2">&quot;UPDDATE&quot;</span><span class="p">:</span> <span class="s2">&quot;geändert am&quot;</span><span class="p">,</span>
+<span class="linenos"> 53</span>        <span class="s2">&quot;UPDNAME&quot;</span><span class="p">:</span> <span class="s2">&quot;geändert von&quot;</span>
+<span class="linenos"> 54</span>    <span class="p">}</span>
+<span class="linenos"> 55</span>    <span class="n">df</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="n">colNames</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+<span class="linenos"> 56</span>
+<span class="linenos"> 57</span>    <span class="k">return</span> <span class="n">df</span>
+<span class="linenos"> 58</span>
+<span class="linenos"> 59</span>
+<span class="linenos"> 60</span><span class="k">def</span> <span class="nf">ladeAlleWerkstattauftragPosMengenabweichungen</span><span class="p">(</span>
+<span class="linenos"> 61</span>        <span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span>
+<span class="linenos"> 62</span>        <span class="n">cond</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlCondition</span><span class="p">,</span> <span class="nb">str</span><span class="p">,</span> <span class="kc">None</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+<span class="linenos"> 63</span>    <span class="n">sql</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlStatementSelect</span><span class="p">(</span><span class="s2">&quot;WAUFTRAGPOS w&quot;</span><span class="p">)</span>
+<span class="linenos"> 64</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addLeftJoin</span><span class="p">(</span><span class="s2">&quot;personal p&quot;</span><span class="p">,</span> <span class="s2">&quot;w.UPDUSER = p.PERSONAL&quot;</span><span class="p">)</span>
 <span class="linenos"> 65</span>
-<span class="linenos"> 66</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addConditionFieldEq</span><span class="p">(</span><span class="s2">&quot;w.STATUS&quot;</span><span class="p">,</span> <span class="mi">4</span><span class="p">)</span>
-<span class="linenos"> 67</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addCondition</span><span class="p">(</span><span class="s2">&quot;abs(w.MENGE-w.MENGE_IST) &gt; 0.001&quot;</span><span class="p">)</span>    
-<span class="linenos"> 68</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addCondition</span><span class="p">(</span><span class="n">cond</span><span class="p">)</span>
-<span class="linenos"> 69</span>    <span class="n">sql</span><span class="o">.</span><span class="n">order</span><span class="o">=</span><span class="s2">&quot;w.UPDDATE&quot;</span>
+<span class="linenos"> 66</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFieldsTable</span><span class="p">(</span><span class="s2">&quot;w&quot;</span><span class="p">,</span> <span class="s2">&quot;ID&quot;</span><span class="p">,</span> <span class="s2">&quot;BAUFTRAG&quot;</span><span class="p">,</span> <span class="s2">&quot;POSITION&quot;</span><span class="p">,</span> <span class="s2">&quot;AG&quot;</span><span class="p">)</span>
+<span class="linenos"> 67</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG&quot;</span><span class="p">)</span>
+<span class="linenos"> 68</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFieldsTable</span><span class="p">(</span><span class="s2">&quot;w&quot;</span><span class="p">,</span> <span class="s2">&quot;MENGE&quot;</span><span class="p">,</span> <span class="s2">&quot;MENGE_IST&quot;</span><span class="p">,</span> <span class="s2">&quot;APLAN as ARTIKEL&quot;</span><span class="p">)</span>
+<span class="linenos"> 69</span>    <span class="n">sql</span><span class="o">.</span><span class="n">addFields</span><span class="p">(</span><span class="s2">&quot;w.UPDDATE&quot;</span><span class="p">,</span> <span class="s2">&quot;p.NAME as UPDNAME&quot;</span><span class="p">)</span>
 <span class="linenos"> 70</span>
-<span class="linenos"> 71</span>    <span class="n">dfOrg</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql</span><span class="p">);</span>
-<span class="linenos"> 72</span>
-<span class="linenos"> 73</span>    <span class="c1"># Add Links</span>
-<span class="linenos"> 74</span>    <span class="n">df</span> <span class="o">=</span> <span class="n">dfOrg</span><span class="o">.</span><span class="n">copy</span><span class="p">();</span>
-<span class="linenos"> 75</span>    <span class="n">df</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;ID&quot;</span><span class="p">]);</span>
-<span class="linenos"> 76</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;POSITION&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span><span class="n">dfOrg</span><span class="p">,</span> 
-<span class="linenos"> 77</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">POSITION</span><span class="p">,</span> 
-<span class="linenos"> 78</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkWauftrag</span><span class="p">(</span>
-<span class="linenos"> 79</span>                            <span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span> <span class="n">accessid</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">ID</span><span class="p">))</span>
-<span class="linenos"> 80</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;BAUFTRAG&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span><span class="n">dfOrg</span><span class="p">,</span> 
-<span class="linenos"> 81</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span> 
-<span class="linenos"> 82</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkBauftrag</span><span class="p">(</span><span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">))</span>
-<span class="linenos"> 83</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;AG&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span><span class="n">dfOrg</span><span class="p">,</span> 
-<span class="linenos"> 84</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">AG</span><span class="p">,</span> 
-<span class="linenos"> 85</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkWauftragPos</span><span class="p">(</span>
-<span class="linenos"> 86</span>                            <span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span> <span class="n">position</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">POSITION</span><span class="p">,</span> <span class="n">accessid</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">ID</span><span class="p">))</span>
-<span class="linenos"> 87</span>    
-<span class="linenos"> 88</span>    <span class="c1"># Demo zum Hinzufügen einer berechneten Spalte</span>
-<span class="linenos"> 89</span>    <span class="c1"># df[&#39;BAUFPOSAG&#39;] = PyAPplus64.pandas.mkDataframeColumn(dfOrg, </span>
-<span class="linenos"> 90</span>    <span class="c1">#                     lambda r: &quot;{}.{} AG {}&quot;.format(r.BAUFTRAG, r.POSITION, r.AG))</span>
-<span class="linenos"> 91</span>
-<span class="linenos"> 92</span>    <span class="c1"># Rename Columns</span>
-<span class="linenos"> 93</span>    <span class="n">colNames</span> <span class="o">=</span> <span class="p">{</span>
-<span class="linenos"> 94</span>        <span class="s2">&quot;BAUFTRAG&quot;</span> <span class="p">:</span> <span class="s2">&quot;Betriebsauftrag&quot;</span><span class="p">,</span>
-<span class="linenos"> 95</span>        <span class="s2">&quot;POSITION&quot;</span> <span class="p">:</span> <span class="s2">&quot;Pos&quot;</span><span class="p">,</span>
-<span class="linenos"> 96</span>        <span class="s2">&quot;AG&quot;</span> <span class="p">:</span> <span class="s2">&quot;AG&quot;</span><span class="p">,</span>
-<span class="linenos"> 97</span>        <span class="s2">&quot;MENGENABWEICHUNG&quot;</span> <span class="p">:</span> <span class="s2">&quot;Mengenabweichung&quot;</span><span class="p">,</span>
-<span class="linenos"> 98</span>        <span class="s2">&quot;MENGE&quot;</span> <span class="p">:</span> <span class="s2">&quot;Menge&quot;</span><span class="p">,</span>
-<span class="linenos"> 99</span>        <span class="s2">&quot;MENGE_IST&quot;</span> <span class="p">:</span> <span class="s2">&quot;Menge-Ist&quot;</span><span class="p">,</span>
-<span class="linenos">100</span>        <span class="s2">&quot;ARTIKEL&quot;</span> <span class="p">:</span> <span class="s2">&quot;Artikel&quot;</span><span class="p">,</span>
-<span class="linenos">101</span>        <span class="s2">&quot;UPDDATE&quot;</span> <span class="p">:</span> <span class="s2">&quot;geändert am&quot;</span><span class="p">,</span>
-<span class="linenos">102</span>        <span class="s2">&quot;UPDNAME&quot;</span> <span class="p">:</span> <span class="s2">&quot;geändert von&quot;</span>
-<span class="linenos">103</span>    <span class="p">}</span>
-<span class="linenos">104</span>    <span class="n">df</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="n">colNames</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">);</span>
-<span class="linenos">105</span>    <span class="k">return</span> <span class="n">df</span>
-<span class="linenos">106</span>
-<span class="linenos">107</span><span class="k">def</span> <span class="nf">computeInYearMonthCond</span><span class="p">(</span><span class="n">field</span> <span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">year</span><span class="p">:</span><span class="nb">int</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> 
-<span class="linenos">108</span>                           <span class="n">month</span><span class="p">:</span><span class="nb">int</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlCondition</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos">109</span>    <span class="k">if</span> <span class="ow">not</span> <span class="p">(</span><span class="n">year</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">):</span> 
-<span class="linenos">110</span>        <span class="k">if</span> <span class="n">month</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos">111</span>            <span class="k">return</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlConditionDateTimeFieldInYear</span><span class="p">(</span><span class="n">field</span><span class="p">,</span> <span class="n">year</span><span class="p">)</span>
-<span class="linenos">112</span>        <span class="k">else</span><span class="p">:</span>
-<span class="linenos">113</span>            <span class="k">return</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlConditionDateTimeFieldInMonth</span><span class="p">(</span><span class="n">field</span><span class="p">,</span> <span class="n">year</span><span class="p">,</span> <span class="n">month</span><span class="p">)</span>
-<span class="linenos">114</span>    <span class="k">else</span><span class="p">:</span>
-<span class="linenos">115</span>        <span class="k">return</span> <span class="kc">None</span>
-<span class="linenos">116</span>
-<span class="linenos">117</span><span class="k">def</span> <span class="nf">computeFileName</span><span class="p">(</span><span class="n">year</span><span class="p">:</span><span class="nb">int</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">month</span><span class="p">:</span><span class="nb">int</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-<span class="linenos">118</span>    <span class="k">if</span> <span class="n">year</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span> 
-<span class="linenos">119</span>        <span class="k">return</span> <span class="s1">&#39;mengenabweichungen-all.xlsx&#39;</span><span class="p">;</span>
-<span class="linenos">120</span>    <span class="k">else</span><span class="p">:</span>
-<span class="linenos">121</span>        <span class="k">if</span> <span class="n">month</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos">122</span>            <span class="k">return</span> <span class="s1">&#39;mengenabweichungen-</span><span class="si">{:04d}</span><span class="s1">.xlsx&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">year</span><span class="p">);</span>
-<span class="linenos">123</span>        <span class="k">else</span><span class="p">:</span>
-<span class="linenos">124</span>            <span class="k">return</span> <span class="s1">&#39;mengenabweichungen-</span><span class="si">{:04d}</span><span class="s1">-</span><span class="si">{:02d}</span><span class="s1">.xlsx&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">year</span><span class="p">,</span> <span class="n">month</span><span class="p">);</span>
+<span class="linenos"> 71</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addConditionFieldEq</span><span class="p">(</span><span class="s2">&quot;w.STATUS&quot;</span><span class="p">,</span> <span class="mi">4</span><span class="p">)</span>
+<span class="linenos"> 72</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addCondition</span><span class="p">(</span><span class="s2">&quot;abs(w.MENGE-w.MENGE_IST) &gt; 0.001&quot;</span><span class="p">)</span>
+<span class="linenos"> 73</span>    <span class="n">sql</span><span class="o">.</span><span class="n">where</span><span class="o">.</span><span class="n">addCondition</span><span class="p">(</span><span class="n">cond</span><span class="p">)</span>
+<span class="linenos"> 74</span>    <span class="n">sql</span><span class="o">.</span><span class="n">order</span> <span class="o">=</span> <span class="s2">&quot;w.UPDDATE&quot;</span>
+<span class="linenos"> 75</span>
+<span class="linenos"> 76</span>    <span class="n">dfOrg</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">pandasReadSql</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">sql</span><span class="p">)</span>
+<span class="linenos"> 77</span>
+<span class="linenos"> 78</span>    <span class="c1"># Add Links</span>
+<span class="linenos"> 79</span>    <span class="n">df</span> <span class="o">=</span> <span class="n">dfOrg</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span>
+<span class="linenos"> 80</span>    <span class="n">df</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;ID&quot;</span><span class="p">])</span>
+<span class="linenos"> 81</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;POSITION&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span>
+<span class="linenos"> 82</span>                        <span class="n">dfOrg</span><span class="p">,</span>
+<span class="linenos"> 83</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">POSITION</span><span class="p">,</span>
+<span class="linenos"> 84</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkWauftrag</span><span class="p">(</span>
+<span class="linenos"> 85</span>                            <span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span> <span class="n">accessid</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">ID</span><span class="p">))</span>
+<span class="linenos"> 86</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;BAUFTRAG&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span>
+<span class="linenos"> 87</span>                        <span class="n">dfOrg</span><span class="p">,</span>
+<span class="linenos"> 88</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span>
+<span class="linenos"> 89</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkBauftrag</span><span class="p">(</span><span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">))</span>
+<span class="linenos"> 90</span>    <span class="n">df</span><span class="p">[</span><span class="s1">&#39;AG&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">mkHyperlinkDataframeColumn</span><span class="p">(</span>
+<span class="linenos"> 91</span>                        <span class="n">dfOrg</span><span class="p">,</span>
+<span class="linenos"> 92</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">r</span><span class="o">.</span><span class="n">AG</span><span class="p">,</span>
+<span class="linenos"> 93</span>                        <span class="k">lambda</span> <span class="n">r</span><span class="p">:</span> <span class="n">server</span><span class="o">.</span><span class="n">makeWebLinkWauftragPos</span><span class="p">(</span>
+<span class="linenos"> 94</span>                            <span class="n">bauftrag</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">BAUFTRAG</span><span class="p">,</span> <span class="n">position</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">POSITION</span><span class="p">,</span> <span class="n">accessid</span><span class="o">=</span><span class="n">r</span><span class="o">.</span><span class="n">ID</span><span class="p">))</span>
+<span class="linenos"> 95</span>
+<span class="linenos"> 96</span>    <span class="c1"># Demo zum Hinzufügen einer berechneten Spalte</span>
+<span class="linenos"> 97</span>    <span class="c1"># df[&#39;BAUFPOSAG&#39;] = PyAPplus64.pandas.mkDataframeColumn(dfOrg,</span>
+<span class="linenos"> 98</span>    <span class="c1">#                     lambda r: &quot;{}.{} AG {}&quot;.format(r.BAUFTRAG, r.POSITION, r.AG))</span>
+<span class="linenos"> 99</span>
+<span class="linenos">100</span>    <span class="c1"># Rename Columns</span>
+<span class="linenos">101</span>    <span class="n">colNames</span> <span class="o">=</span> <span class="p">{</span>
+<span class="linenos">102</span>        <span class="s2">&quot;BAUFTRAG&quot;</span><span class="p">:</span> <span class="s2">&quot;Betriebsauftrag&quot;</span><span class="p">,</span>
+<span class="linenos">103</span>        <span class="s2">&quot;POSITION&quot;</span><span class="p">:</span> <span class="s2">&quot;Pos&quot;</span><span class="p">,</span>
+<span class="linenos">104</span>        <span class="s2">&quot;AG&quot;</span><span class="p">:</span> <span class="s2">&quot;AG&quot;</span><span class="p">,</span>
+<span class="linenos">105</span>        <span class="s2">&quot;MENGENABWEICHUNG&quot;</span><span class="p">:</span> <span class="s2">&quot;Mengenabweichung&quot;</span><span class="p">,</span>
+<span class="linenos">106</span>        <span class="s2">&quot;MENGE&quot;</span><span class="p">:</span> <span class="s2">&quot;Menge&quot;</span><span class="p">,</span>
+<span class="linenos">107</span>        <span class="s2">&quot;MENGE_IST&quot;</span><span class="p">:</span> <span class="s2">&quot;Menge-Ist&quot;</span><span class="p">,</span>
+<span class="linenos">108</span>        <span class="s2">&quot;ARTIKEL&quot;</span><span class="p">:</span> <span class="s2">&quot;Artikel&quot;</span><span class="p">,</span>
+<span class="linenos">109</span>        <span class="s2">&quot;UPDDATE&quot;</span><span class="p">:</span> <span class="s2">&quot;geändert am&quot;</span><span class="p">,</span>
+<span class="linenos">110</span>        <span class="s2">&quot;UPDNAME&quot;</span><span class="p">:</span> <span class="s2">&quot;geändert von&quot;</span>
+<span class="linenos">111</span>    <span class="p">}</span>
+<span class="linenos">112</span>    <span class="n">df</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="n">colNames</span><span class="p">,</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+<span class="linenos">113</span>    <span class="k">return</span> <span class="n">df</span>
+<span class="linenos">114</span>
+<span class="linenos">115</span>
+<span class="linenos">116</span><span class="k">def</span> <span class="nf">computeInYearMonthCond</span><span class="p">(</span><span class="n">field</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">year</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+<span class="linenos">117</span>                           <span class="n">month</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Optional</span><span class="p">[</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlCondition</span><span class="p">]:</span>
+<span class="linenos">118</span>    <span class="k">if</span> <span class="ow">not</span> <span class="p">(</span><span class="n">year</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">):</span>
+<span class="linenos">119</span>        <span class="k">if</span> <span class="n">month</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">120</span>            <span class="k">return</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlConditionDateTimeFieldInYear</span><span class="p">(</span><span class="n">field</span><span class="p">,</span> <span class="n">year</span><span class="p">)</span>
+<span class="linenos">121</span>        <span class="k">else</span><span class="p">:</span>
+<span class="linenos">122</span>            <span class="k">return</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlConditionDateTimeFieldInMonth</span><span class="p">(</span><span class="n">field</span><span class="p">,</span> <span class="n">year</span><span class="p">,</span> <span class="n">month</span><span class="p">)</span>
+<span class="linenos">123</span>    <span class="k">else</span><span class="p">:</span>
+<span class="linenos">124</span>        <span class="k">return</span> <span class="kc">None</span>
 <span class="linenos">125</span>
-<span class="linenos">126</span><span class="k">def</span> <span class="nf">_exportInternal</span><span class="p">(</span><span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> <span class="n">fn</span><span class="p">:</span><span class="nb">str</span><span class="p">,</span> 
-<span class="linenos">127</span>                    <span class="n">cond</span><span class="p">:</span><span class="n">Union</span><span class="p">[</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlCondition</span><span class="p">,</span> <span class="nb">str</span><span class="p">,</span> <span class="kc">None</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-<span class="linenos">128</span>    <span class="n">df1</span> <span class="o">=</span> <span class="n">ladeAlleWerkstattauftragMengenabweichungen</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">cond</span><span class="p">)</span>
-<span class="linenos">129</span>    <span class="n">df2</span> <span class="o">=</span> <span class="n">ladeAlleWerkstattauftragPosMengenabweichungen</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">cond</span><span class="p">)</span>
-<span class="linenos">130</span>    <span class="nb">print</span> <span class="p">(</span><span class="s2">&quot;erzeuge &quot;</span> <span class="o">+</span> <span class="n">fn</span><span class="p">);</span>
-<span class="linenos">131</span>    <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">exportToExcel</span><span class="p">(</span><span class="n">fn</span><span class="p">,</span> <span class="p">[(</span><span class="n">df1</span><span class="p">,</span> <span class="s2">&quot;WAuftrag&quot;</span><span class="p">),</span> <span class="p">(</span><span class="n">df2</span><span class="p">,</span> <span class="s2">&quot;WAuftrag-Pos&quot;</span><span class="p">)],</span> <span class="n">addTable</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-<span class="linenos">132</span>    <span class="k">return</span> <span class="nb">len</span><span class="p">(</span><span class="n">df1</span><span class="o">.</span><span class="n">index</span><span class="p">)</span> <span class="o">+</span> <span class="nb">len</span><span class="p">(</span><span class="n">df2</span><span class="o">.</span><span class="n">index</span><span class="p">)</span>
-<span class="linenos">133</span>
-<span class="linenos">134</span><span class="k">def</span> <span class="nf">exportVonBis</span><span class="p">(</span><span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> <span class="n">fn</span><span class="p">:</span><span class="nb">str</span><span class="p">,</span> 
-<span class="linenos">135</span>                 <span class="n">von</span><span class="p">:</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">|</span><span class="kc">None</span><span class="p">,</span> <span class="n">bis</span><span class="p">:</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">|</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-<span class="linenos">136</span>  <span class="n">cond</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlConditionDateTimeFieldInRange</span><span class="p">(</span><span class="s2">&quot;w.UPDDATE&quot;</span><span class="p">,</span> <span class="n">von</span><span class="p">,</span> <span class="n">bis</span><span class="p">)</span>
-<span class="linenos">137</span>  <span class="k">return</span> <span class="n">_exportInternal</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">fn</span><span class="p">,</span> <span class="n">cond</span><span class="p">)</span>
-<span class="linenos">138</span>
-<span class="linenos">139</span><span class="k">def</span> <span class="nf">exportYearMonth</span><span class="p">(</span><span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> 
-<span class="linenos">140</span>                    <span class="n">year</span><span class="p">:</span><span class="nb">int</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">month</span><span class="p">:</span><span class="nb">int</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-<span class="linenos">141</span>    <span class="n">cond</span><span class="o">=</span><span class="n">computeInYearMonthCond</span><span class="p">(</span><span class="s2">&quot;w.UPDDATE&quot;</span><span class="p">,</span> <span class="n">year</span><span class="o">=</span><span class="n">year</span><span class="p">,</span> <span class="n">month</span><span class="o">=</span><span class="n">month</span><span class="p">)</span>
-<span class="linenos">142</span>    <span class="n">fn</span> <span class="o">=</span> <span class="n">computeFileName</span><span class="p">(</span><span class="n">year</span><span class="o">=</span><span class="n">year</span><span class="p">,</span> <span class="n">month</span><span class="o">=</span><span class="n">month</span><span class="p">)</span>
-<span class="linenos">143</span>    <span class="k">return</span> <span class="n">_exportInternal</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">fn</span><span class="p">,</span> <span class="n">cond</span><span class="p">)</span>
+<span class="linenos">126</span>
+<span class="linenos">127</span><span class="k">def</span> <span class="nf">computeFileName</span><span class="p">(</span><span class="n">year</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">month</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+<span class="linenos">128</span>    <span class="k">if</span> <span class="n">year</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">129</span>        <span class="k">return</span> <span class="s1">&#39;mengenabweichungen-all.xlsx&#39;</span>
+<span class="linenos">130</span>    <span class="k">else</span><span class="p">:</span>
+<span class="linenos">131</span>        <span class="k">if</span> <span class="n">month</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">132</span>            <span class="k">return</span> <span class="s1">&#39;mengenabweichungen-</span><span class="si">{:04d}</span><span class="s1">.xlsx&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">year</span><span class="p">)</span>
+<span class="linenos">133</span>        <span class="k">else</span><span class="p">:</span>
+<span class="linenos">134</span>            <span class="k">return</span> <span class="s1">&#39;mengenabweichungen-</span><span class="si">{:04d}</span><span class="s1">-</span><span class="si">{:02d}</span><span class="s1">.xlsx&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">year</span><span class="p">,</span> <span class="n">month</span><span class="p">)</span>
+<span class="linenos">135</span>
+<span class="linenos">136</span>
+<span class="linenos">137</span><span class="k">def</span> <span class="nf">_exportInternal</span><span class="p">(</span><span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> <span class="n">fn</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+<span class="linenos">138</span>                    <span class="n">cond</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">SqlCondition</span><span class="p">,</span> <span class="nb">str</span><span class="p">,</span> <span class="kc">None</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+<span class="linenos">139</span>    <span class="n">df1</span> <span class="o">=</span> <span class="n">ladeAlleWerkstattauftragMengenabweichungen</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">cond</span><span class="p">)</span>
+<span class="linenos">140</span>    <span class="n">df2</span> <span class="o">=</span> <span class="n">ladeAlleWerkstattauftragPosMengenabweichungen</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">cond</span><span class="p">)</span>
+<span class="linenos">141</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;erzeuge &quot;</span> <span class="o">+</span> <span class="n">fn</span><span class="p">)</span>
+<span class="linenos">142</span>    <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">pandas</span><span class="o">.</span><span class="n">exportToExcel</span><span class="p">(</span><span class="n">fn</span><span class="p">,</span> <span class="p">[(</span><span class="n">df1</span><span class="p">,</span> <span class="s2">&quot;WAuftrag&quot;</span><span class="p">),</span> <span class="p">(</span><span class="n">df2</span><span class="p">,</span> <span class="s2">&quot;WAuftrag-Pos&quot;</span><span class="p">)],</span> <span class="n">addTable</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+<span class="linenos">143</span>    <span class="k">return</span> <span class="nb">len</span><span class="p">(</span><span class="n">df1</span><span class="o">.</span><span class="n">index</span><span class="p">)</span> <span class="o">+</span> <span class="nb">len</span><span class="p">(</span><span class="n">df2</span><span class="o">.</span><span class="n">index</span><span class="p">)</span>
 <span class="linenos">144</span>
-<span class="linenos">145</span><span class="k">def</span> <span class="nf">computePreviousMonthYear</span><span class="p">(</span><span class="n">cyear</span> <span class="p">:</span> <span class="nb">int</span><span class="p">,</span> <span class="n">cmonth</span> <span class="p">:</span><span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
-<span class="linenos">146</span>    <span class="k">if</span> <span class="n">cmonth</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-<span class="linenos">147</span>        <span class="k">return</span> <span class="p">(</span><span class="n">cyear</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="mi">12</span><span class="p">)</span>
-<span class="linenos">148</span>    <span class="k">else</span><span class="p">:</span>
-<span class="linenos">149</span>        <span class="k">return</span> <span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="o">-</span><span class="mi">1</span><span class="p">);</span>
+<span class="linenos">145</span>
+<span class="linenos">146</span><span class="k">def</span> <span class="nf">exportVonBis</span><span class="p">(</span><span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> <span class="n">fn</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+<span class="linenos">147</span>                 <span class="n">von</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">],</span> <span class="n">bis</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+<span class="linenos">148</span>    <span class="n">cond</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">sql_utils</span><span class="o">.</span><span class="n">SqlConditionDateTimeFieldInRange</span><span class="p">(</span><span class="s2">&quot;w.UPDDATE&quot;</span><span class="p">,</span> <span class="n">von</span><span class="p">,</span> <span class="n">bis</span><span class="p">)</span>
+<span class="linenos">149</span>    <span class="k">return</span> <span class="n">_exportInternal</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">fn</span><span class="p">,</span> <span class="n">cond</span><span class="p">)</span>
 <span class="linenos">150</span>
-<span class="linenos">151</span><span class="k">def</span> <span class="nf">computeNextMonthYear</span><span class="p">(</span><span class="n">cyear</span> <span class="p">:</span> <span class="nb">int</span><span class="p">,</span> <span class="n">cmonth</span> <span class="p">:</span><span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
-<span class="linenos">152</span>    <span class="k">if</span> <span class="n">cmonth</span> <span class="o">==</span> <span class="mi">12</span><span class="p">:</span>
-<span class="linenos">153</span>        <span class="k">return</span> <span class="p">(</span><span class="n">cyear</span><span class="o">+</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
-<span class="linenos">154</span>    <span class="k">else</span><span class="p">:</span>
-<span class="linenos">155</span>        <span class="k">return</span> <span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="o">+</span><span class="mi">1</span><span class="p">);</span>
-<span class="linenos">156</span>
-<span class="linenos">157</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span> <span class="p">:</span> <span class="nb">str</span><span class="o">|</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">user</span><span class="p">:</span><span class="nb">str</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">env</span><span class="p">:</span><span class="nb">str</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos">158</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">,</span> <span class="n">user</span><span class="o">=</span><span class="n">user</span><span class="p">,</span> <span class="n">env</span><span class="o">=</span><span class="n">env</span><span class="p">)</span> 
-<span class="linenos">159</span>    
-<span class="linenos">160</span>    <span class="n">now</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">date</span><span class="o">.</span><span class="n">today</span><span class="p">()</span>
-<span class="linenos">161</span>    <span class="p">(</span><span class="n">cmonth</span><span class="p">,</span> <span class="n">cyear</span><span class="p">)</span> <span class="o">=</span> <span class="p">(</span><span class="n">now</span><span class="o">.</span><span class="n">month</span><span class="p">,</span> <span class="n">now</span><span class="o">.</span><span class="n">year</span><span class="p">)</span>
-<span class="linenos">162</span>    <span class="p">(</span><span class="n">pyear</span><span class="p">,</span> <span class="n">pmonth</span><span class="p">)</span> <span class="o">=</span> <span class="n">computePreviousMonthYear</span><span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">);</span>
-<span class="linenos">163</span>    
-<span class="linenos">164</span>    <span class="c1"># Ausgaben    </span>
-<span class="linenos">165</span>    <span class="n">exportYearMonth</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">)</span> <span class="c1"># Aktueller Monat</span>
-<span class="linenos">166</span>    <span class="n">exportYearMonth</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">pyear</span><span class="p">,</span> <span class="n">pmonth</span><span class="p">)</span> <span class="c1"># Vorheriger Monat</span>
-<span class="linenos">167</span>    <span class="c1"># export(cyear) # aktuelles Jahr</span>
-<span class="linenos">168</span>    <span class="c1"># export(cyear-1) # letztes Jahr</span>
-<span class="linenos">169</span>    <span class="c1"># export() # alles</span>
-<span class="linenos">170</span>
-<span class="linenos">171</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-<span class="linenos">172</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">)</span>
+<span class="linenos">151</span>
+<span class="linenos">152</span><span class="k">def</span> <span class="nf">exportYearMonth</span><span class="p">(</span><span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span>
+<span class="linenos">153</span>                    <span class="n">year</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">month</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+<span class="linenos">154</span>    <span class="n">cond</span> <span class="o">=</span> <span class="n">computeInYearMonthCond</span><span class="p">(</span><span class="s2">&quot;w.UPDDATE&quot;</span><span class="p">,</span> <span class="n">year</span><span class="o">=</span><span class="n">year</span><span class="p">,</span> <span class="n">month</span><span class="o">=</span><span class="n">month</span><span class="p">)</span>
+<span class="linenos">155</span>    <span class="n">fn</span> <span class="o">=</span> <span class="n">computeFileName</span><span class="p">(</span><span class="n">year</span><span class="o">=</span><span class="n">year</span><span class="p">,</span> <span class="n">month</span><span class="o">=</span><span class="n">month</span><span class="p">)</span>
+<span class="linenos">156</span>    <span class="k">return</span> <span class="n">_exportInternal</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">fn</span><span class="p">,</span> <span class="n">cond</span><span class="p">)</span>
+<span class="linenos">157</span>
+<span class="linenos">158</span>
+<span class="linenos">159</span><span class="k">def</span> <span class="nf">computePreviousMonthYear</span><span class="p">(</span><span class="n">cyear</span><span class="p">:</span> <span class="nb">int</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
+<span class="linenos">160</span>    <span class="k">if</span> <span class="n">cmonth</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+<span class="linenos">161</span>        <span class="k">return</span> <span class="p">(</span><span class="n">cyear</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="mi">12</span><span class="p">)</span>
+<span class="linenos">162</span>    <span class="k">else</span><span class="p">:</span>
+<span class="linenos">163</span>        <span class="k">return</span> <span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="o">-</span><span class="mi">1</span><span class="p">)</span>
+<span class="linenos">164</span>
+<span class="linenos">165</span>
+<span class="linenos">166</span><span class="k">def</span> <span class="nf">computeNextMonthYear</span><span class="p">(</span><span class="n">cyear</span><span class="p">:</span> <span class="nb">int</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
+<span class="linenos">167</span>    <span class="k">if</span> <span class="n">cmonth</span> <span class="o">==</span> <span class="mi">12</span><span class="p">:</span>
+<span class="linenos">168</span>        <span class="k">return</span> <span class="p">(</span><span class="n">cyear</span><span class="o">+</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
+<span class="linenos">169</span>    <span class="k">else</span><span class="p">:</span>
+<span class="linenos">170</span>        <span class="k">return</span> <span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="o">+</span><span class="mi">1</span><span class="p">)</span>
+<span class="linenos">171</span>
+<span class="linenos">172</span>
+<span class="linenos">173</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">],</span> <span class="n">user</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">env</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">174</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">,</span> <span class="n">user</span><span class="o">=</span><span class="n">user</span><span class="p">,</span> <span class="n">env</span><span class="o">=</span><span class="n">env</span><span class="p">)</span>
+<span class="linenos">175</span>
+<span class="linenos">176</span>    <span class="n">now</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">date</span><span class="o">.</span><span class="n">today</span><span class="p">()</span>
+<span class="linenos">177</span>    <span class="p">(</span><span class="n">cmonth</span><span class="p">,</span> <span class="n">cyear</span><span class="p">)</span> <span class="o">=</span> <span class="p">(</span><span class="n">now</span><span class="o">.</span><span class="n">month</span><span class="p">,</span> <span class="n">now</span><span class="o">.</span><span class="n">year</span><span class="p">)</span>
+<span class="linenos">178</span>    <span class="p">(</span><span class="n">pyear</span><span class="p">,</span> <span class="n">pmonth</span><span class="p">)</span> <span class="o">=</span> <span class="n">computePreviousMonthYear</span><span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">)</span>
+<span class="linenos">179</span>
+<span class="linenos">180</span>    <span class="c1"># Ausgaben</span>
+<span class="linenos">181</span>    <span class="n">exportYearMonth</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">)</span>  <span class="c1"># Aktueller Monat</span>
+<span class="linenos">182</span>    <span class="n">exportYearMonth</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">pyear</span><span class="p">,</span> <span class="n">pmonth</span><span class="p">)</span>  <span class="c1"># Vorheriger Monat</span>
+<span class="linenos">183</span>    <span class="c1"># export(cyear) # aktuelles Jahr</span>
+<span class="linenos">184</span>    <span class="c1"># export(cyear-1) # letztes Jahr</span>
+<span class="linenos">185</span>    <span class="c1"># export() # alles</span>
+<span class="linenos">186</span>
+<span class="linenos">187</span>
+<span class="linenos">188</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">189</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">)</span>
 </pre></div>
 </div>
 </section>
 <section id="mengenabweichung-gui-py">
 <h2><code class="docutils literal notranslate"><span class="pre">mengenabweichung_gui.py</span></code><a class="headerlink" href="#mengenabweichung-gui-py" title="Link zu dieser Überschrift">¶</a></h2>
 <p>Beispiel für eine sehr einfache GUI, die die Eingabe einfacher Parameter erlaubt.
 Die GUI wird um die Erzeugung von Excel-Dateien mit Mengenabweichungen gebaut.</p>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">PySimpleGUI</span> <span class="k">as</span> <span class="nn">sg</span> <span class="c1"># type: ignore</span>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">PySimpleGUI</span> <span class="k">as</span> <span class="nn">sg</span>  <span class="c1"># type: ignore</span>
 <span class="linenos"> 2</span><span class="kn">import</span> <span class="nn">mengenabweichung</span>
 <span class="linenos"> 3</span><span class="kn">import</span> <span class="nn">datetime</span>
 <span class="linenos"> 4</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
 <span class="linenos"> 5</span><span class="kn">import</span> <span class="nn">applus_configs</span>
 <span class="linenos"> 6</span><span class="kn">import</span> <span class="nn">pathlib</span>
-<span class="linenos"> 7</span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="o">*</span>
+<span class="linenos"> 7</span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Tuple</span><span class="p">,</span> <span class="n">Optional</span><span class="p">,</span> <span class="n">Union</span>
 <span class="linenos"> 8</span>
-<span class="linenos"> 9</span><span class="k">def</span> <span class="nf">parseDate</span> <span class="p">(</span><span class="n">dateS</span><span class="p">:</span><span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Tuple</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">|</span><span class="kc">None</span><span class="p">,</span> <span class="nb">bool</span><span class="p">]:</span>
-<span class="linenos">10</span>    <span class="k">if</span> <span class="n">dateS</span> <span class="ow">is</span> <span class="kc">None</span> <span class="ow">or</span> <span class="n">dateS</span> <span class="o">==</span> <span class="s1">&#39;&#39;</span><span class="p">:</span>
-<span class="linenos">11</span>        <span class="k">return</span> <span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-<span class="linenos">12</span>    <span class="k">else</span><span class="p">:</span>
-<span class="linenos">13</span>        <span class="k">try</span><span class="p">:</span>
-<span class="linenos">14</span>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">strptime</span><span class="p">(</span><span class="n">dateS</span><span class="p">,</span> <span class="s1">&#39;</span><span class="si">%d</span><span class="s1">.%m.%Y&#39;</span><span class="p">),</span> <span class="kc">True</span><span class="p">)</span>
-<span class="linenos">15</span>        <span class="k">except</span><span class="p">:</span>
-<span class="linenos">16</span>            <span class="n">sg</span><span class="o">.</span><span class="n">popup_error</span><span class="p">(</span><span class="s2">&quot;Fehler beim Parsen des Datums &#39;</span><span class="si">{}</span><span class="s2">&#39;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">dateS</span><span class="p">))</span>
-<span class="linenos">17</span>            <span class="k">return</span> <span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-<span class="linenos">18</span>
-<span class="linenos">19</span><span class="k">def</span> <span class="nf">createFile</span><span class="p">(</span><span class="n">server</span><span class="p">:</span><span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> <span class="n">fileS</span><span class="p">:</span><span class="nb">str</span><span class="p">,</span> <span class="n">vonS</span><span class="p">:</span><span class="nb">str</span><span class="p">,</span> <span class="n">bisS</span><span class="p">:</span><span class="nb">str</span><span class="p">)</span><span class="o">-&gt;</span><span class="kc">None</span><span class="p">:</span>    
-<span class="linenos">20</span>    <span class="p">(</span><span class="n">von</span><span class="p">,</span> <span class="n">vonOK</span><span class="p">)</span> <span class="o">=</span> <span class="n">parseDate</span><span class="p">(</span><span class="n">vonS</span><span class="p">)</span>
-<span class="linenos">21</span>    <span class="k">if</span> <span class="ow">not</span> <span class="n">vonOK</span><span class="p">:</span> <span class="k">return</span>
-<span class="linenos">22</span>    
-<span class="linenos">23</span>    <span class="p">(</span><span class="n">bis</span><span class="p">,</span> <span class="n">bisOK</span><span class="p">)</span> <span class="o">=</span> <span class="n">parseDate</span><span class="p">(</span><span class="n">bisS</span><span class="p">)</span>
-<span class="linenos">24</span>    <span class="k">if</span> <span class="ow">not</span> <span class="n">bisOK</span><span class="p">:</span> <span class="k">return</span>
+<span class="linenos"> 9</span>
+<span class="linenos">10</span><span class="k">def</span> <span class="nf">parseDate</span><span class="p">(</span><span class="n">dateS</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Tuple</span><span class="p">[</span><span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">],</span> <span class="nb">bool</span><span class="p">]:</span>
+<span class="linenos">11</span>    <span class="k">if</span> <span class="n">dateS</span> <span class="ow">is</span> <span class="kc">None</span> <span class="ow">or</span> <span class="n">dateS</span> <span class="o">==</span> <span class="s1">&#39;&#39;</span><span class="p">:</span>
+<span class="linenos">12</span>        <span class="k">return</span> <span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+<span class="linenos">13</span>    <span class="k">else</span><span class="p">:</span>
+<span class="linenos">14</span>        <span class="k">try</span><span class="p">:</span>
+<span class="linenos">15</span>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">strptime</span><span class="p">(</span><span class="n">dateS</span><span class="p">,</span> <span class="s1">&#39;</span><span class="si">%d</span><span class="s1">.%m.%Y&#39;</span><span class="p">),</span> <span class="kc">True</span><span class="p">)</span>
+<span class="linenos">16</span>        <span class="k">except</span><span class="p">:</span>
+<span class="linenos">17</span>            <span class="n">sg</span><span class="o">.</span><span class="n">popup_error</span><span class="p">(</span><span class="s2">&quot;Fehler beim Parsen des Datums &#39;</span><span class="si">{}</span><span class="s2">&#39;&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">dateS</span><span class="p">))</span>
+<span class="linenos">18</span>            <span class="k">return</span> <span class="p">(</span><span class="kc">None</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+<span class="linenos">19</span>
+<span class="linenos">20</span>
+<span class="linenos">21</span><span class="k">def</span> <span class="nf">createFile</span><span class="p">(</span><span class="n">server</span><span class="p">:</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">APplusServer</span><span class="p">,</span> <span class="n">fileS</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">vonS</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">bisS</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">22</span>    <span class="p">(</span><span class="n">von</span><span class="p">,</span> <span class="n">vonOK</span><span class="p">)</span> <span class="o">=</span> <span class="n">parseDate</span><span class="p">(</span><span class="n">vonS</span><span class="p">)</span>
+<span class="linenos">23</span>    <span class="k">if</span> <span class="ow">not</span> <span class="n">vonOK</span><span class="p">:</span>
+<span class="linenos">24</span>        <span class="k">return</span>
 <span class="linenos">25</span>
-<span class="linenos">26</span>    <span class="k">if</span> <span class="p">(</span><span class="n">fileS</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">)</span> <span class="ow">or</span> <span class="n">fileS</span> <span class="o">==</span> <span class="s1">&#39;&#39;</span><span class="p">:</span> 
-<span class="linenos">27</span>        <span class="n">sg</span><span class="o">.</span><span class="n">popup_error</span><span class="p">(</span><span class="s2">&quot;Es wurde keine Ausgabedatei ausgewählt.&quot;</span><span class="p">)</span>
+<span class="linenos">26</span>    <span class="p">(</span><span class="n">bis</span><span class="p">,</span> <span class="n">bisOK</span><span class="p">)</span> <span class="o">=</span> <span class="n">parseDate</span><span class="p">(</span><span class="n">bisS</span><span class="p">)</span>
+<span class="linenos">27</span>    <span class="k">if</span> <span class="ow">not</span> <span class="n">bisOK</span><span class="p">:</span>
 <span class="linenos">28</span>        <span class="k">return</span>
-<span class="linenos">29</span>    <span class="k">else</span><span class="p">:</span>
-<span class="linenos">30</span>        <span class="n">file</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">fileS</span><span class="p">)</span>
-<span class="linenos">31</span>
-<span class="linenos">32</span>    <span class="n">c</span> <span class="o">=</span> <span class="n">mengenabweichung</span><span class="o">.</span><span class="n">exportVonBis</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">file</span><span class="o">.</span><span class="n">as_posix</span><span class="p">(),</span> <span class="n">von</span><span class="p">,</span> <span class="n">bis</span><span class="p">)</span>
-<span class="linenos">33</span>    <span class="n">sg</span><span class="o">.</span><span class="n">popup_ok</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{}</span><span class="s2"> Datensätze erfolgreich in Datei &#39;</span><span class="si">{}</span><span class="s2">&#39; geschrieben.&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">c</span><span class="p">,</span> <span class="n">file</span><span class="p">))</span>
-<span class="linenos">34</span>
+<span class="linenos">29</span>
+<span class="linenos">30</span>    <span class="k">if</span> <span class="p">(</span><span class="n">fileS</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">)</span> <span class="ow">or</span> <span class="n">fileS</span> <span class="o">==</span> <span class="s1">&#39;&#39;</span><span class="p">:</span>
+<span class="linenos">31</span>        <span class="n">sg</span><span class="o">.</span><span class="n">popup_error</span><span class="p">(</span><span class="s2">&quot;Es wurde keine Ausgabedatei ausgewählt.&quot;</span><span class="p">)</span>
+<span class="linenos">32</span>        <span class="k">return</span>
+<span class="linenos">33</span>    <span class="k">else</span><span class="p">:</span>
+<span class="linenos">34</span>        <span class="n">file</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">fileS</span><span class="p">)</span>
 <span class="linenos">35</span>
-<span class="linenos">36</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span> <span class="p">:</span> <span class="nb">str</span><span class="o">|</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">user</span><span class="p">:</span><span class="nb">str</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">env</span><span class="p">:</span><span class="nb">str</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos">37</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">,</span> <span class="n">user</span><span class="o">=</span><span class="n">user</span><span class="p">,</span> <span class="n">env</span><span class="o">=</span><span class="n">env</span><span class="p">)</span> 
+<span class="linenos">36</span>    <span class="n">c</span> <span class="o">=</span> <span class="n">mengenabweichung</span><span class="o">.</span><span class="n">exportVonBis</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">file</span><span class="o">.</span><span class="n">as_posix</span><span class="p">(),</span> <span class="n">von</span><span class="p">,</span> <span class="n">bis</span><span class="p">)</span>
+<span class="linenos">37</span>    <span class="n">sg</span><span class="o">.</span><span class="n">popup_ok</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{}</span><span class="s2"> Datensätze erfolgreich in Datei &#39;</span><span class="si">{}</span><span class="s2">&#39; geschrieben.&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">c</span><span class="p">,</span> <span class="n">file</span><span class="p">))</span>
 <span class="linenos">38</span>
-<span class="linenos">39</span>    <span class="n">layout</span> <span class="o">=</span> <span class="p">[</span>
-<span class="linenos">40</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Text</span><span class="p">((</span><span class="s1">&#39;Bitte geben Sie an, für welchen Zeitraum die &#39;</span>
-<span class="linenos">41</span>                  <span class="s1">&#39;Mengenabweichungen ausgegeben werden sollen:&#39;</span><span class="p">))],</span>
-<span class="linenos">42</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Text</span><span class="p">(</span><span class="s1">&#39;Von (einschließlich)&#39;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span><span class="mi">1</span><span class="p">)),</span> <span class="n">sg</span><span class="o">.</span><span class="n">InputText</span><span class="p">(</span><span class="n">key</span><span class="o">=</span><span class="s1">&#39;Von&#39;</span><span class="p">),</span>
-<span class="linenos">43</span>         <span class="n">sg</span><span class="o">.</span><span class="n">CalendarButton</span><span class="p">(</span><span class="s2">&quot;Kalender&quot;</span><span class="p">,</span> <span class="n">close_when_date_chosen</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> 
-<span class="linenos">44</span>                           <span class="n">target</span><span class="o">=</span><span class="s2">&quot;Von&quot;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;</span><span class="si">%d</span><span class="s1">.%m.%Y&#39;</span><span class="p">)],</span>
-<span class="linenos">45</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Text</span><span class="p">(</span><span class="s1">&#39;Bis (ausschließlich)&#39;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span><span class="mi">1</span><span class="p">)),</span> <span class="n">sg</span><span class="o">.</span><span class="n">InputText</span><span class="p">(</span><span class="n">key</span><span class="o">=</span><span class="s1">&#39;Bis&#39;</span><span class="p">),</span>
-<span class="linenos">46</span>         <span class="n">sg</span><span class="o">.</span><span class="n">CalendarButton</span><span class="p">(</span><span class="s2">&quot;Kalender&quot;</span><span class="p">,</span> <span class="n">close_when_date_chosen</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> 
-<span class="linenos">47</span>                           <span class="n">target</span><span class="o">=</span><span class="s2">&quot;Bis&quot;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;</span><span class="si">%d</span><span class="s1">.%m.%Y&#39;</span><span class="p">)],</span>
-<span class="linenos">48</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Text</span><span class="p">(</span><span class="s1">&#39;Ausgabedatei&#39;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span><span class="mi">1</span><span class="p">)),</span> <span class="n">sg</span><span class="o">.</span><span class="n">InputText</span><span class="p">(</span><span class="n">key</span><span class="o">=</span><span class="s1">&#39;File&#39;</span><span class="p">),</span>
-<span class="linenos">49</span>        <span class="n">sg</span><span class="o">.</span><span class="n">FileSaveAs</span><span class="p">(</span><span class="n">button_text</span><span class="o">=</span><span class="s2">&quot;wählen&quot;</span><span class="p">,</span> <span class="n">target</span><span class="o">=</span><span class="s2">&quot;File&quot;</span><span class="p">,</span> 
-<span class="linenos">50</span>                      <span class="n">file_types</span> <span class="o">=</span> <span class="p">((</span><span class="s1">&#39;Excel Files&#39;</span><span class="p">,</span> <span class="s1">&#39;*.xlsx&#39;</span><span class="p">),),</span> 
-<span class="linenos">51</span>                      <span class="n">default_extension</span> <span class="o">=</span> <span class="s2">&quot;.xlsx&quot;</span><span class="p">)],</span>
-<span class="linenos">52</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Aktueller Monat&quot;</span><span class="p">),</span> <span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Letzter Monat&quot;</span><span class="p">),</span> 
-<span class="linenos">53</span>         <span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Aktuelles Jahr&quot;</span><span class="p">),</span> <span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Letztes Jahr&quot;</span><span class="p">)],</span>
-<span class="linenos">54</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Speichern&quot;</span><span class="p">),</span> <span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Beenden&quot;</span><span class="p">)]</span>
-<span class="linenos">55</span>    <span class="p">]</span>
-<span class="linenos">56</span>
-<span class="linenos">57</span>    <span class="n">systemName</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getSystemName</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot;/&quot;</span> <span class="o">+</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getMandant</span><span class="p">()</span>
-<span class="linenos">58</span>    <span class="n">window</span> <span class="o">=</span> <span class="n">sg</span><span class="o">.</span><span class="n">Window</span><span class="p">(</span><span class="s2">&quot;Mengenabweichung &quot;</span> <span class="o">+</span> <span class="n">systemName</span><span class="p">,</span> <span class="n">layout</span><span class="p">)</span>
-<span class="linenos">59</span>    <span class="n">now</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">date</span><span class="o">.</span><span class="n">today</span><span class="p">()</span>
-<span class="linenos">60</span>    <span class="p">(</span><span class="n">cmonth</span><span class="p">,</span> <span class="n">cyear</span><span class="p">)</span> <span class="o">=</span> <span class="p">(</span><span class="n">now</span><span class="o">.</span><span class="n">month</span><span class="p">,</span> <span class="n">now</span><span class="o">.</span><span class="n">year</span><span class="p">)</span>
-<span class="linenos">61</span>    <span class="p">(</span><span class="n">pyear</span><span class="p">,</span> <span class="n">pmonth</span><span class="p">)</span> <span class="o">=</span> <span class="n">mengenabweichung</span><span class="o">.</span><span class="n">computePreviousMonthYear</span><span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">);</span>
-<span class="linenos">62</span>    <span class="p">(</span><span class="n">nyear</span><span class="p">,</span> <span class="n">nmonth</span><span class="p">)</span> <span class="o">=</span> <span class="n">mengenabweichung</span><span class="o">.</span><span class="n">computeNextMonthYear</span><span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">);</span>
-<span class="linenos">63</span>
-<span class="linenos">64</span>    <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-<span class="linenos">65</span>        <span class="n">event</span><span class="p">,</span> <span class="n">values</span> <span class="o">=</span> <span class="n">window</span><span class="o">.</span><span class="n">read</span><span class="p">()</span>
-<span class="linenos">66</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="n">sg</span><span class="o">.</span><span class="n">WIN_CLOSED</span> <span class="ow">or</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Beenden&#39;</span><span class="p">:</span>
-<span class="linenos">67</span>            <span class="k">break</span>
-<span class="linenos">68</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Aktueller Monat&#39;</span><span class="p">:</span>
-<span class="linenos">69</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Von&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.</span><span class="si">{:02d}</span><span class="s2">.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cmonth</span><span class="p">,</span> <span class="n">cyear</span><span class="p">));</span>
-<span class="linenos">70</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Bis&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.</span><span class="si">{:02d}</span><span class="s2">.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">nmonth</span><span class="p">,</span> <span class="n">nyear</span><span class="p">));</span>
-<span class="linenos">71</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Letzter Monat&#39;</span><span class="p">:</span>
-<span class="linenos">72</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Von&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.</span><span class="si">{:02d}</span><span class="s2">.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">pmonth</span><span class="p">,</span> <span class="n">pyear</span><span class="p">));</span>
-<span class="linenos">73</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Bis&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.</span><span class="si">{:02d}</span><span class="s2">.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cmonth</span><span class="p">,</span> <span class="n">cyear</span><span class="p">));</span>
-<span class="linenos">74</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Aktuelles Jahr&#39;</span><span class="p">:</span>
-<span class="linenos">75</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Von&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.01.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cyear</span><span class="p">));</span>
-<span class="linenos">76</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Bis&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.01.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cyear</span><span class="o">+</span><span class="mi">1</span><span class="p">));</span>
-<span class="linenos">77</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Letztes Jahr&#39;</span><span class="p">:</span>
-<span class="linenos">78</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Von&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.01.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cyear</span><span class="o">-</span><span class="mi">1</span><span class="p">));</span>
-<span class="linenos">79</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Bis&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.01.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cyear</span><span class="p">));</span>
-<span class="linenos">80</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Speichern&#39;</span><span class="p">:</span>
-<span class="linenos">81</span>            <span class="k">try</span><span class="p">:</span>
-<span class="linenos">82</span>                <span class="n">createFile</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">values</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;File&#39;</span><span class="p">,</span> <span class="kc">None</span><span class="p">),</span> 
-<span class="linenos">83</span>                           <span class="n">values</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;Von&#39;</span><span class="p">,</span> <span class="kc">None</span><span class="p">),</span> <span class="n">values</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;Bis&#39;</span><span class="p">,</span> <span class="kc">None</span><span class="p">))</span>
-<span class="linenos">84</span>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-<span class="linenos">85</span>                <span class="n">sg</span><span class="o">.</span><span class="n">popup_error_with_traceback</span><span class="p">(</span><span class="s2">&quot;Beim Erzeugen der Excel-Datei trat ein Fehler auf:&quot;</span><span class="p">,</span> <span class="n">e</span><span class="p">);</span>
-<span class="linenos">86</span>
-<span class="linenos">87</span>    <span class="n">window</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-<span class="linenos">88</span>
-<span class="linenos">89</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-<span class="linenos">90</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlProd</span><span class="p">)</span>
+<span class="linenos">39</span>
+<span class="linenos">40</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">],</span> <span class="n">user</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">env</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">41</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">,</span> <span class="n">user</span><span class="o">=</span><span class="n">user</span><span class="p">,</span> <span class="n">env</span><span class="o">=</span><span class="n">env</span><span class="p">)</span>
+<span class="linenos">42</span>
+<span class="linenos">43</span>    <span class="n">layout</span> <span class="o">=</span> <span class="p">[</span>
+<span class="linenos">44</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Text</span><span class="p">((</span><span class="s1">&#39;Bitte geben Sie an, für welchen Zeitraum die &#39;</span>
+<span class="linenos">45</span>                  <span class="s1">&#39;Mengenabweichungen ausgegeben werden sollen:&#39;</span><span class="p">))],</span>
+<span class="linenos">46</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Text</span><span class="p">(</span><span class="s1">&#39;Von (einschließlich)&#39;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">1</span><span class="p">)),</span> <span class="n">sg</span><span class="o">.</span><span class="n">InputText</span><span class="p">(</span><span class="n">key</span><span class="o">=</span><span class="s1">&#39;Von&#39;</span><span class="p">),</span>
+<span class="linenos">47</span>         <span class="n">sg</span><span class="o">.</span><span class="n">CalendarButton</span><span class="p">(</span><span class="s2">&quot;Kalender&quot;</span><span class="p">,</span> <span class="n">close_when_date_chosen</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+<span class="linenos">48</span>                           <span class="n">target</span><span class="o">=</span><span class="s2">&quot;Von&quot;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;</span><span class="si">%d</span><span class="s1">.%m.%Y&#39;</span><span class="p">)],</span>
+<span class="linenos">49</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Text</span><span class="p">(</span><span class="s1">&#39;Bis (ausschließlich)&#39;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">1</span><span class="p">)),</span> <span class="n">sg</span><span class="o">.</span><span class="n">InputText</span><span class="p">(</span><span class="n">key</span><span class="o">=</span><span class="s1">&#39;Bis&#39;</span><span class="p">),</span>
+<span class="linenos">50</span>         <span class="n">sg</span><span class="o">.</span><span class="n">CalendarButton</span><span class="p">(</span><span class="s2">&quot;Kalender&quot;</span><span class="p">,</span> <span class="n">close_when_date_chosen</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+<span class="linenos">51</span>                           <span class="n">target</span><span class="o">=</span><span class="s2">&quot;Bis&quot;</span><span class="p">,</span> <span class="nb">format</span><span class="o">=</span><span class="s1">&#39;</span><span class="si">%d</span><span class="s1">.%m.%Y&#39;</span><span class="p">)],</span>
+<span class="linenos">52</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Text</span><span class="p">(</span><span class="s1">&#39;Ausgabedatei&#39;</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">1</span><span class="p">)),</span> <span class="n">sg</span><span class="o">.</span><span class="n">InputText</span><span class="p">(</span><span class="n">key</span><span class="o">=</span><span class="s1">&#39;File&#39;</span><span class="p">),</span>
+<span class="linenos">53</span>         <span class="n">sg</span><span class="o">.</span><span class="n">FileSaveAs</span><span class="p">(</span><span class="n">button_text</span><span class="o">=</span><span class="s2">&quot;wählen&quot;</span><span class="p">,</span>
+<span class="linenos">54</span>                       <span class="n">target</span><span class="o">=</span><span class="s2">&quot;File&quot;</span><span class="p">,</span>
+<span class="linenos">55</span>                       <span class="n">file_types</span><span class="o">=</span><span class="p">((</span><span class="s1">&#39;Excel Files&#39;</span><span class="p">,</span> <span class="s1">&#39;*.xlsx&#39;</span><span class="p">),),</span>
+<span class="linenos">56</span>                       <span class="n">default_extension</span><span class="o">=</span><span class="s2">&quot;.xlsx&quot;</span><span class="p">)],</span>
+<span class="linenos">57</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Aktueller Monat&quot;</span><span class="p">),</span> <span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Letzter Monat&quot;</span><span class="p">),</span>
+<span class="linenos">58</span>         <span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Aktuelles Jahr&quot;</span><span class="p">),</span> <span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Letztes Jahr&quot;</span><span class="p">)],</span>
+<span class="linenos">59</span>        <span class="p">[</span><span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Speichern&quot;</span><span class="p">),</span> <span class="n">sg</span><span class="o">.</span><span class="n">Button</span><span class="p">(</span><span class="s2">&quot;Beenden&quot;</span><span class="p">)]</span>
+<span class="linenos">60</span>    <span class="p">]</span>
+<span class="linenos">61</span>
+<span class="linenos">62</span>    <span class="n">systemName</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getSystemName</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot;/&quot;</span> <span class="o">+</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getMandant</span><span class="p">()</span>
+<span class="linenos">63</span>    <span class="n">window</span> <span class="o">=</span> <span class="n">sg</span><span class="o">.</span><span class="n">Window</span><span class="p">(</span><span class="s2">&quot;Mengenabweichung &quot;</span> <span class="o">+</span> <span class="n">systemName</span><span class="p">,</span> <span class="n">layout</span><span class="p">)</span>
+<span class="linenos">64</span>    <span class="n">now</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">date</span><span class="o">.</span><span class="n">today</span><span class="p">()</span>
+<span class="linenos">65</span>    <span class="p">(</span><span class="n">cmonth</span><span class="p">,</span> <span class="n">cyear</span><span class="p">)</span> <span class="o">=</span> <span class="p">(</span><span class="n">now</span><span class="o">.</span><span class="n">month</span><span class="p">,</span> <span class="n">now</span><span class="o">.</span><span class="n">year</span><span class="p">)</span>
+<span class="linenos">66</span>    <span class="p">(</span><span class="n">pyear</span><span class="p">,</span> <span class="n">pmonth</span><span class="p">)</span> <span class="o">=</span> <span class="n">mengenabweichung</span><span class="o">.</span><span class="n">computePreviousMonthYear</span><span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">)</span>
+<span class="linenos">67</span>    <span class="p">(</span><span class="n">nyear</span><span class="p">,</span> <span class="n">nmonth</span><span class="p">)</span> <span class="o">=</span> <span class="n">mengenabweichung</span><span class="o">.</span><span class="n">computeNextMonthYear</span><span class="p">(</span><span class="n">cyear</span><span class="p">,</span> <span class="n">cmonth</span><span class="p">)</span>
+<span class="linenos">68</span>
+<span class="linenos">69</span>    <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+<span class="linenos">70</span>        <span class="n">event</span><span class="p">,</span> <span class="n">values</span> <span class="o">=</span> <span class="n">window</span><span class="o">.</span><span class="n">read</span><span class="p">()</span>
+<span class="linenos">71</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="n">sg</span><span class="o">.</span><span class="n">WIN_CLOSED</span> <span class="ow">or</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Beenden&#39;</span><span class="p">:</span>
+<span class="linenos">72</span>            <span class="k">break</span>
+<span class="linenos">73</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Aktueller Monat&#39;</span><span class="p">:</span>
+<span class="linenos">74</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Von&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.</span><span class="si">{:02d}</span><span class="s2">.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cmonth</span><span class="p">,</span> <span class="n">cyear</span><span class="p">))</span>
+<span class="linenos">75</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Bis&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.</span><span class="si">{:02d}</span><span class="s2">.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">nmonth</span><span class="p">,</span> <span class="n">nyear</span><span class="p">))</span>
+<span class="linenos">76</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Letzter Monat&#39;</span><span class="p">:</span>
+<span class="linenos">77</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Von&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.</span><span class="si">{:02d}</span><span class="s2">.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">pmonth</span><span class="p">,</span> <span class="n">pyear</span><span class="p">))</span>
+<span class="linenos">78</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Bis&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.</span><span class="si">{:02d}</span><span class="s2">.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cmonth</span><span class="p">,</span> <span class="n">cyear</span><span class="p">))</span>
+<span class="linenos">79</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Aktuelles Jahr&#39;</span><span class="p">:</span>
+<span class="linenos">80</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Von&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.01.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cyear</span><span class="p">))</span>
+<span class="linenos">81</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Bis&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.01.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cyear</span><span class="o">+</span><span class="mi">1</span><span class="p">))</span>
+<span class="linenos">82</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Letztes Jahr&#39;</span><span class="p">:</span>
+<span class="linenos">83</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Von&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.01.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cyear</span><span class="o">-</span><span class="mi">1</span><span class="p">))</span>
+<span class="linenos">84</span>            <span class="n">window</span><span class="p">[</span><span class="s1">&#39;Bis&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">value</span><span class="o">=</span><span class="s2">&quot;01.01.</span><span class="si">{:04d}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">cyear</span><span class="p">))</span>
+<span class="linenos">85</span>        <span class="k">if</span> <span class="n">event</span> <span class="o">==</span> <span class="s1">&#39;Speichern&#39;</span><span class="p">:</span>
+<span class="linenos">86</span>            <span class="k">try</span><span class="p">:</span>
+<span class="linenos">87</span>                <span class="n">createFile</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">values</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;File&#39;</span><span class="p">,</span> <span class="kc">None</span><span class="p">),</span>
+<span class="linenos">88</span>                           <span class="n">values</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;Von&#39;</span><span class="p">,</span> <span class="kc">None</span><span class="p">),</span> <span class="n">values</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;Bis&#39;</span><span class="p">,</span> <span class="kc">None</span><span class="p">))</span>
+<span class="linenos">89</span>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+<span class="linenos">90</span>                <span class="n">sg</span><span class="o">.</span><span class="n">popup_error_with_traceback</span><span class="p">(</span><span class="s2">&quot;Beim Erzeugen der Excel-Datei trat ein Fehler auf:&quot;</span><span class="p">,</span> <span class="n">e</span><span class="p">)</span>
+<span class="linenos">91</span>
+<span class="linenos">92</span>    <span class="n">window</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
+<span class="linenos">93</span>
+<span class="linenos">94</span>
+<span class="linenos">95</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">96</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlProd</span><span class="p">)</span>
 </pre></div>
 </div>
 </section>
 <section id="copy-artikel-py">
 <h2><code class="docutils literal notranslate"><span class="pre">copy_artikel.py</span></code><a class="headerlink" href="#copy-artikel-py" title="Link zu dieser Überschrift">¶</a></h2>
 <p>Beispiel, wie Artikel inklusive Arbeitsplan und Stückliste dupliziert werden kann.</p>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
-<span class="linenos"> 2</span><span class="kn">import</span> <span class="nn">applus_configs</span>
-<span class="linenos"> 3</span><span class="kn">import</span> <span class="nn">logging</span>
-<span class="linenos"> 4</span><span class="kn">import</span> <span class="nn">yaml</span> 
-<span class="linenos"> 5</span>
-<span class="linenos"> 6</span>
-<span class="linenos"> 7</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">artikel</span><span class="p">:</span><span class="nb">str</span><span class="p">,</span> <span class="n">artikelNeu</span><span class="p">:</span><span class="nb">str</span><span class="o">|</span><span class="kc">None</span><span class="o">=</span><span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
-<span class="linenos"> 8</span>    <span class="c1"># Server verbinden</span>
-<span class="linenos"> 9</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span> 
-<span class="linenos">10</span>
-<span class="linenos">11</span>    <span class="c1"># DuplicateBusinessObject für Artikel erstellen</span>
-<span class="linenos">12</span>    <span class="n">dArt</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">duplicate</span><span class="o">.</span><span class="n">loadDBDuplicateArtikel</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">artikel</span><span class="p">);</span>
-<span class="linenos">13</span>
-<span class="linenos">14</span>    <span class="c1"># DuplicateBusinessObject zur Demonstration in YAML konvertieren und zurück</span>
-<span class="linenos">15</span>    <span class="n">dArtYaml</span> <span class="o">=</span> <span class="n">yaml</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">dArt</span><span class="p">);</span>
-<span class="linenos">16</span>    <span class="nb">print</span><span class="p">(</span><span class="n">dArtYaml</span><span class="p">);</span>
-<span class="linenos">17</span>    <span class="n">dArt2</span> <span class="o">=</span> <span class="n">yaml</span><span class="o">.</span><span class="n">load</span><span class="p">(</span><span class="n">dArtYaml</span><span class="p">,</span> <span class="n">Loader</span><span class="o">=</span><span class="n">yaml</span><span class="o">.</span><span class="n">UnsafeLoader</span><span class="p">)</span>
-<span class="linenos">18</span>
-<span class="linenos">19</span>    <span class="c1"># Neue Artikel-Nummer bestimmen und DuplicateBusinessObject in DB schreiben</span>
-<span class="linenos">20</span>    <span class="c1"># Man könnte hier genauso gut einen anderen Server verwenden</span>
-<span class="linenos">21</span>    <span class="k">if</span> <span class="p">(</span><span class="n">artikelNeu</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">):</span>
-<span class="linenos">22</span>        <span class="n">artikelNeu</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">nextNumber</span><span class="p">(</span><span class="s2">&quot;Artikel&quot;</span><span class="p">)</span>
-<span class="linenos">23</span>
-<span class="linenos">24</span>    <span class="k">if</span> <span class="ow">not</span> <span class="p">(</span><span class="n">dArt</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">):</span>
-<span class="linenos">25</span>        <span class="n">dArt</span><span class="o">.</span><span class="n">setFields</span><span class="p">({</span><span class="s2">&quot;artikel&quot;</span> <span class="p">:</span> <span class="n">artikelNeu</span><span class="p">})</span>
-<span class="linenos">26</span>        <span class="n">res</span> <span class="o">=</span> <span class="n">dArt</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">server</span><span class="p">);</span>
-<span class="linenos">27</span>        <span class="nb">print</span><span class="p">(</span><span class="n">res</span><span class="p">);</span>
-<span class="linenos">28</span>
-<span class="linenos">29</span>
-<span class="linenos">30</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-<span class="linenos">31</span>    <span class="c1"># Logger Einrichten</span>
-<span class="linenos">32</span>    <span class="n">logging</span><span class="o">.</span><span class="n">basicConfig</span><span class="p">(</span><span class="n">level</span><span class="o">=</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span> 
-<span class="linenos">33</span>    <span class="c1"># logger = logging.getLogger(&quot;PyAPplus64.applus_db&quot;);</span>
-<span class="linenos">34</span>    <span class="c1"># logger.setLevel(logging.ERROR)</span>
-<span class="linenos">35</span>
-<span class="linenos">36</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="s2">&quot;my-artikel&quot;</span><span class="p">,</span> <span class="n">artikelNeu</span><span class="o">=</span><span class="s2">&quot;my-artikel-copy&quot;</span><span class="p">)</span>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">pathlib</span>
+<span class="linenos"> 2</span><span class="kn">import</span> <span class="nn">PyAPplus64</span>
+<span class="linenos"> 3</span><span class="kn">import</span> <span class="nn">applus_configs</span>
+<span class="linenos"> 4</span><span class="kn">import</span> <span class="nn">logging</span>
+<span class="linenos"> 5</span><span class="kn">import</span> <span class="nn">yaml</span>
+<span class="linenos"> 6</span><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Optional</span>
+<span class="linenos"> 7</span>
+<span class="linenos"> 8</span>
+<span class="linenos"> 9</span><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">confFile</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="n">artikel</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">artikelNeu</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+<span class="linenos">10</span>    <span class="c1"># Server verbinden</span>
+<span class="linenos">11</span>    <span class="n">server</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">applus</span><span class="o">.</span><span class="n">applusFromConfigFile</span><span class="p">(</span><span class="n">confFile</span><span class="p">)</span>
+<span class="linenos">12</span>
+<span class="linenos">13</span>    <span class="c1"># DuplicateBusinessObject für Artikel erstellen</span>
+<span class="linenos">14</span>    <span class="n">dArt</span> <span class="o">=</span> <span class="n">PyAPplus64</span><span class="o">.</span><span class="n">duplicate</span><span class="o">.</span><span class="n">loadDBDuplicateArtikel</span><span class="p">(</span><span class="n">server</span><span class="p">,</span> <span class="n">artikel</span><span class="p">)</span>
+<span class="linenos">15</span>
+<span class="linenos">16</span>    <span class="c1"># DuplicateBusinessObject zur Demonstration in YAML konvertieren und zurück</span>
+<span class="linenos">17</span>    <span class="n">dArtYaml</span> <span class="o">=</span> <span class="n">yaml</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">dArt</span><span class="p">)</span>
+<span class="linenos">18</span>    <span class="nb">print</span><span class="p">(</span><span class="n">dArtYaml</span><span class="p">)</span>
+<span class="linenos">19</span>    <span class="n">dArt2</span> <span class="o">=</span> <span class="n">yaml</span><span class="o">.</span><span class="n">load</span><span class="p">(</span><span class="n">dArtYaml</span><span class="p">,</span> <span class="n">Loader</span><span class="o">=</span><span class="n">yaml</span><span class="o">.</span><span class="n">UnsafeLoader</span><span class="p">)</span>
+<span class="linenos">20</span>
+<span class="linenos">21</span>    <span class="c1"># Neue Artikel-Nummer bestimmen und DuplicateBusinessObject in DB schreiben</span>
+<span class="linenos">22</span>    <span class="c1"># Man könnte hier genauso gut einen anderen Server verwenden</span>
+<span class="linenos">23</span>    <span class="k">if</span> <span class="p">(</span><span class="n">artikelNeu</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">):</span>
+<span class="linenos">24</span>        <span class="n">artikelNeu</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">nextNumber</span><span class="p">(</span><span class="s2">&quot;Artikel&quot;</span><span class="p">)</span>
+<span class="linenos">25</span>
+<span class="linenos">26</span>    <span class="k">if</span> <span class="ow">not</span> <span class="p">(</span><span class="n">dArt</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">):</span>
+<span class="linenos">27</span>        <span class="n">dArt</span><span class="o">.</span><span class="n">setFields</span><span class="p">({</span><span class="s2">&quot;artikel&quot;</span><span class="p">:</span> <span class="n">artikelNeu</span><span class="p">})</span>
+<span class="linenos">28</span>        <span class="n">res</span> <span class="o">=</span> <span class="n">dArt</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">server</span><span class="p">)</span>
+<span class="linenos">29</span>        <span class="nb">print</span><span class="p">(</span><span class="n">res</span><span class="p">)</span>
+<span class="linenos">30</span>
+<span class="linenos">31</span>
+<span class="linenos">32</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">33</span>    <span class="c1"># Logger Einrichten</span>
+<span class="linenos">34</span>    <span class="n">logging</span><span class="o">.</span><span class="n">basicConfig</span><span class="p">(</span><span class="n">level</span><span class="o">=</span><span class="n">logging</span><span class="o">.</span><span class="n">INFO</span><span class="p">)</span>
+<span class="linenos">35</span>    <span class="c1"># logger = logging.getLogger(&quot;PyAPplus64.applus_db&quot;);</span>
+<span class="linenos">36</span>    <span class="c1"># logger.setLevel(logging.ERROR)</span>
 <span class="linenos">37</span>
+<span class="linenos">38</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">,</span> <span class="s2">&quot;my-artikel&quot;</span><span class="p">,</span> <span class="n">artikelNeu</span><span class="o">=</span><span class="s2">&quot;my-artikel-copy&quot;</span><span class="p">)</span>
 </pre></div>
 </div>
 </section>
 </section>
 
 
             <div class="clearer"></div>
@@ -486,14 +559,15 @@
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h3><a href="index.html">Inhaltsverzeichnis</a></h3>
   <ul>
 <li><a class="reference internal" href="#">Beispiele</a><ul>
 <li><a class="reference internal" href="#config-dateien">Config-Dateien</a></li>
+<li><a class="reference internal" href="#read-settings-py"><code class="docutils literal notranslate"><span class="pre">read_settings.py</span></code></a></li>
 <li><a class="reference internal" href="#check-dokumente-py"><code class="docutils literal notranslate"><span class="pre">check_dokumente.py</span></code></a></li>
 <li><a class="reference internal" href="#adhoc-report-py"><code class="docutils literal notranslate"><span class="pre">adhoc_report.py</span></code></a></li>
 <li><a class="reference internal" href="#mengenabweichung-py"><code class="docutils literal notranslate"><span class="pre">mengenabweichung.py</span></code></a></li>
 <li><a class="reference internal" href="#mengenabweichung-gui-py"><code class="docutils literal notranslate"><span class="pre">mengenabweichung_gui.py</span></code></a></li>
 <li><a class="reference internal" href="#copy-artikel-py"><code class="docutils literal notranslate"><span class="pre">copy_artikel.py</span></code></a></li>
 </ul>
 </li>
@@ -537,15 +611,15 @@
              >Module</a> |</li>
         <li class="right" >
           <a href="generated/PyAPplus64.html" title="PyAPplus64 package"
              >weiter</a> |</li>
         <li class="right" >
           <a href="abhaengigkeiten.html" title="Abhängigkeiten"
              >zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Beispiele</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 
 
 **** Navigation ****
     * Index
     * Module |
     * weiter |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Beispiele
 ****** BeispieleÂ¶ ******
 Im Verzeichnis examples finden sich Python Dateien, die die Verwendung
 vonPyAPplus64demonstrieren.
 ***** Config-DateienÂ¶ *****
 Viele Scripte teilen sich Einstellungen. Beispielsweise greifen fast alle
 Scripte irgendwie auf APplus zu und benÃ¶tigen Informationen, mit welchem APP-
@@ -40,434 +40,526 @@
 14  server : "some-server",
 15  db : "APplusProd6",
 16  user : "SA",
 17  password : "your-db-password"
 18}
 Damit nicht in jedem Script immer wieder neu die Konfig-Dateien ausgewÃ¤hlt
 werden mÃ¼ssen, werden die Konfigs fÃ¼r das Prod-, Test- und Deploy-System in
-examples/applus_configs.py hinterlegt. Diese wird in allen Scripten importiert,
-so dass das Config-Verzeichnis und die darin enthaltenen Configs einfach zur
-VerfÃ¼gung stehen.
+examples/applus_configs.py hinterlegt. Diese Datei wird in allen Scripten
+importiert, so dass das Config-Verzeichnis und die darin enthaltenen Configs
+einfach zur VerfÃ¼gung stehen.
 1import pathlib
 2
 3basedir = pathlib.Path(__file__)
 4configdir = basedir.joinpath("config")
 5
 6serverConfYamlDeploy = configdir.joinpath("applus-server-deploy.yaml")
 7serverConfYamlTest = configdir.joinpath("applus-server-test.yaml")
 8serverConfYamlProd = configdir.joinpath("applus-server-prod.yaml")
-9
+
+***** read_settings.pyÂ¶ *****
+Einfaches Beispiel fÃ¼r Auslesen der SysConf und bestimmter Einstellungen.
+ 1# Einfaches Script, das verschiedene Werte des Servers ausliest.
+ 2# Dies sind SysConfig-Einstellungen, aber auch der aktuelle Mandant,
+ 3# Systemnamen, ...
+ 4
+ 5import pathlib
+ 6import PyAPplus64
+ 7import applus_configs
+ 8from typing import Optional, Union
+ 9
+10
+11def main(confFile: Union[str, pathlib.Path], user: Optional[str] = None, env:
+Optional[str] = None) -> None:
+12    server = PyAPplus64.applusFromConfigFile(confFile, user=user, env=env)
+13
+14    print("\n\nSysConf Lookups:")
+15
+16    print("  Default Auftragsart:", server.sysconf.getString("STAMM",
+"DEFAULTAUFTRAGSART"))
+17    print("  Auftragsarten:")
+18    arten = server.sysconf.getList("STAMM", "AUFTRAGSART", sep='\n')
+19    if not arten:
+20        arten = []
+21    for a in arten:
+22        print("    - " + a)
+23
+24    print("  Firmen-Nr. automatisch vergeben:", server.sysconf.getBoolean
+("STAMM", "FIRMAAUTOMATIK"))
+25    print("  Anzahl Artikelstellen:", server.sysconf.getInt("STAMM",
+"ARTKLASSIFNRLAENGE"))
+26
+27    print("\n\nScriptTool:")
+28
+29    print("  CurrentDate:", server.scripttool.getCurrentDate())
+30    print("  CurrentTime:", server.scripttool.getCurrentTime())
+31    print("  CurrentDateTime:", server.scripttool.getCurrentDateTime())
+32    print("  LoginName:", server.scripttool.getLoginName())
+33    print("  UserName:", server.scripttool.getUserName())
+34    print("  UserFullName:", server.scripttool.getUserFullName())
+35    print("  SystemName:", server.scripttool.getSystemName())
+36    print("  Mandant:", server.scripttool.getMandant())
+37    print("  MandantName:", server.scripttool.getMandantName())
+38    print("  InstallPath:", server.scripttool.getInstallPath())
+39    print("  InstallPathAppServer:",
+server.scripttool.getInstallPathAppServer())
+40    print("  InstallPathWebServer:",
+server.scripttool.getInstallPathWebServer())
+41    print("  ServerInfo - Version:", server.scripttool.getServerInfo().find
+("version").text)
+42
+43
+44if __name__ == "__main__":
+45    main(applus_configs.serverConfYamlTest)
 
 ***** check_dokumente.pyÂ¶ *****
 Einfaches Beispiel fÃ¼r lesenden und schreibenden Zugriff auf APplus Datenbank.
  1import pathlib
  2import PyAPplus64
  3import applus_configs
- 4
- 5def main(confFile : pathlib.Path, docDir:str, updateDB:bool) -> None:
- 6  server = PyAPplus64.applus.applusFromConfigFile(confFile)
- 7
- 8  sql = PyAPplus64.sql_utils.SqlStatementSelect("ARTIKEL");
- 9  sql.addFields("ID", "ARTIKEL", "DOCUMENTS");
-10  sql.where.addConditionFieldStringNotEmpty("DOCUMENTS");
-11
-12  for row in server.dbQueryAll(sql):
-13    doc = pathlib.Path(docDir + row.DOCUMENTS);
-14    if not doc.exists():
-15        print("Bild '{}' fÃ¼r Artikel '{}' nicht gefunden".format(doc,
-row.ARTIKEL))
+ 4from typing import Optional
+ 5
+ 6
+ 7def main(confFile: pathlib.Path, updateDB: bool, docDir: Optional[str] =
+None) -> None:
+ 8    server = PyAPplus64.applus.applusFromConfigFile(confFile)
+ 9
+10    if docDir is None:
+11        docDir = str(server.scripttool.getInstallPathWebServer().joinpath
+("DocLib"))
+12
+13    sql = PyAPplus64.sql_utils.SqlStatementSelect("ARTIKEL")
+14    sql.addFields("ID", "ARTIKEL", "DOCUMENTS")
+15    sql.where.addConditionFieldStringNotEmpty("DOCUMENTS")
 16
-17        if updateDB:
-18              upd = server.mkUseXMLRowUpdate("ARTIKEL", row.ID);
-19              upd.addField("DOCUMENTS", None);
-20              upd.update();
+17    for row in server.dbQueryAll(sql):
+18        doc = pathlib.Path(docDir + row.DOCUMENTS)
+19        if not doc.exists():
+20            print("Bild '{}' fÃ¼r Artikel '{}' nicht gefunden".format(doc,
+row.ARTIKEL))
 21
-22if __name__ == "__main__":
-23  main(applus_configs.serverConfYamlTest, "somedir\\WebServer\\DocLib",
-False)
+22            if updateDB:
+23                upd = server.mkUseXMLRowUpdate("ARTIKEL", row.ID)
+24                upd.addField("DOCUMENTS", None)
+25                upd.update()
+26
+27
+28if __name__ == "__main__":
+29    main(applus_configs.serverConfYamlTest, False)
 
 ***** adhoc_report.pyÂ¶ *****
 Sehr einfaches Beispiel zur Erstellung einer Excel-Tabelle aus einer SQL-
 Abfrage.
  1import PyAPplus64
  2import applus_configs
  3import pathlib
  4
- 5def main(confFile : pathlib.Path, outfile : str) -> None:
- 6    server = PyAPplus64.applus.applusFromConfigFile(confFile)
- 7
- 8    # Einfache SQL-Anfrage
- 9    sql1 = ("select Material, count(*) as Anzahl from ARTIKEL "
-10            "group by MATERIAL having MATERIAL is not null "
-11            "order by Anzahl desc")
-12    df1 = PyAPplus64.pandas.pandasReadSql(server, sql1)
-13
-14    # Sql Select-Statements kÃ¶nnen auch Ã¼ber SqlStatementSelect
+ 5
+ 6def main(confFile: pathlib.Path, outfile: str) -> None:
+ 7    server = PyAPplus64.applus.applusFromConfigFile(confFile)
+ 8
+ 9    # Einfache SQL-Anfrage
+10    sql1 = ("select Material, count(*) as Anzahl from ARTIKEL "
+11            "group by MATERIAL having MATERIAL is not null "
+12            "order by Anzahl desc")
+13    df1 = PyAPplus64.pandas.pandasReadSql(server, sql1)
+14
+15    # Sql Select-Statements kÃ¶nnen auch Ã¼ber SqlStatementSelect
 zusammengebaut
-15    # werden. Die ist bei vielen, komplizierten Bedingungen teilweise
+16    # werden. Die ist bei vielen, komplizierten Bedingungen teilweise
 hilfreich.
-16    sql2 = PyAPplus64.SqlStatementSelect("ARTIKEL")
-17    sql2.addFields("Material", "count(*) as Anzahl")
-18    sql2.addGroupBy("MATERIAL")
-19    sql2.having.addConditionFieldIsNotNull("MATERIAL")
-20    sql2.order = "Anzahl desc"
-21    df2 = PyAPplus64.pandas.pandasReadSql(server, sql2)
-22
-23    # Ausgabe als Excel mit 2 BlÃ¤ttern
-24    PyAPplus64.pandas.exportToExcel(outfile, [(df1, "Materialien"), (df2,
+17    sql2 = PyAPplus64.SqlStatementSelect("ARTIKEL")
+18    sql2.addFields("Material", "count(*) as Anzahl")
+19    sql2.addGroupBy("MATERIAL")
+20    sql2.having.addConditionFieldIsNotNull("MATERIAL")
+21    sql2.order = "Anzahl desc"
+22    df2 = PyAPplus64.pandas.pandasReadSql(server, sql2)
+23
+24    # Ausgabe als Excel mit 2 BlÃ¤ttern
+25    PyAPplus64.pandas.exportToExcel(outfile, [(df1, "Materialien"), (df2,
 "Materialien 2")], addTable=True)
-25
 26
-27if __name__ == "__main__":
-28    main(applus_configs.serverConfYamlTest, "myout.xlsx")
+27
+28if __name__ == "__main__":
+29    main(applus_configs.serverConfYamlTest, "myout.xlsx")
 
 ***** mengenabweichung.pyÂ¶ *****
 Etwas komplizierteres Beispiel zur Erstellung einer Excel-Datei aus SQL-
 Abfragen.
-  1import datetime
-  2import PyAPplus64
-  3import applus_configs
-  4import pandas as pd # type: ignore
-  5import pathlib
-  6from typing import *
-  7
-  8def ladeAlleWerkstattauftragMengenabweichungen(
-  9        server:PyAPplus64.APplusServer,
- 10        cond:PyAPplus64.SqlCondition|str|None=None) -> pd.DataFrame:
- 11    sql = PyAPplus64.sql_utils.SqlStatementSelect("WAUFTRAG w");
- 12    sql.addLeftJoin("personal p", "w.UPDUSER = p.PERSONAL")
- 13
- 14    sql.addFieldsTable("w", "ID", "BAUFTRAG", "POSITION")
- 15    sql.addFields("(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG")
- 16    sql.addFieldsTable("w", "MENGE", "MENGE_IST",
- 17                       "APLAN as ARTIKEL", "NAME as ARTIKELNAME")
- 18    sql.addFields("w.UPDDATE", "p.NAME as UPDNAME")
- 19
- 20    sql.where.addConditionFieldGe("w.STATUS", 5)
- 21    sql.where.addCondition("abs(w.MENGE-w.MENGE_IST) > 0.001")
- 22    sql.where.addCondition(cond)
- 23    sql.order="w.UPDDATE"
- 24    dfOrg = PyAPplus64.pandas.pandasReadSql(server, sql);
- 25
- 26    # Add Links
- 27    df = dfOrg.copy();
- 28    df = df.drop(columns=["ID"]);
- 29    # df = df[['POSITION', 'BAUFTRAG', 'MENGE']] # reorder / filter columns
- 30
- 31    df['POSITION'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg,
- 32                        lambda r: r.POSITION,
- 33                        lambda r: server.makeWebLinkWauftrag(
- 34                            bauftrag=r.BAUFTRAG, accessid=r.ID))
- 35    df['BAUFTRAG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg,
- 36                        lambda r: r.BAUFTRAG,
- 37                        lambda r: server.makeWebLinkBauftrag
+  1# Erzeugt Excel-Tabellen mit WerkstattauftrÃ¤gen und
+Werkstattauftragspositionen mit Mengenabweichungen
+  2
+  3import datetime
+  4import PyAPplus64
+  5import applus_configs
+  6import pandas as pd  # type: ignore
+  7import pathlib
+  8from typing import Tuple, Union, Optional
+  9
+ 10
+ 11def ladeAlleWerkstattauftragMengenabweichungen(
+ 12        server: PyAPplus64.APplusServer,
+ 13        cond: Union[PyAPplus64.SqlCondition, str, None] = None) -
+> pd.DataFrame:
+ 14    sql = PyAPplus64.sql_utils.SqlStatementSelect("WAUFTRAG w")
+ 15    sql.addLeftJoin("personal p", "w.UPDUSER = p.PERSONAL")
+ 16
+ 17    sql.addFieldsTable("w", "ID", "BAUFTRAG", "POSITION")
+ 18    sql.addFields("(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG")
+ 19    sql.addFieldsTable("w", "MENGE", "MENGE_IST",
+ 20                       "APLAN as ARTIKEL", "NAME as ARTIKELNAME")
+ 21    sql.addFields("w.UPDDATE", "p.NAME as UPDNAME")
+ 22
+ 23    sql.where.addConditionFieldGe("w.STATUS", 5)
+ 24    sql.where.addCondition("abs(w.MENGE-w.MENGE_IST) > 0.001")
+ 25    sql.where.addCondition(cond)
+ 26    sql.order = "w.UPDDATE"
+ 27    dfOrg = PyAPplus64.pandas.pandasReadSql(server, sql)
+ 28
+ 29    # Add Links
+ 30    df = dfOrg.copy()
+ 31    df = df.drop(columns=["ID"])
+ 32    # df = df[['POSITION', 'BAUFTRAG', 'MENGE']] # reorder / filter columns
+ 33
+ 34    df['POSITION'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+ 35                        dfOrg,
+ 36                        lambda r: r.POSITION,
+ 37                        lambda r: server.makeWebLinkWauftrag(
+ 38                            bauftrag=r.BAUFTRAG, accessid=r.ID))
+ 39    df['BAUFTRAG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+ 40                        dfOrg,
+ 41                        lambda r: r.BAUFTRAG,
+ 42                        lambda r: server.makeWebLinkBauftrag
 (bauftrag=r.BAUFTRAG))
- 38
- 39    colNames = {
- 40        "BAUFTRAG" : "Betriebsauftrag",
- 41        "POSITION" : "Pos",
- 42        "MENGENABWEICHUNG" : "Mengenabweichung",
- 43        "MENGE" : "Menge",
- 44        "MENGE_IST" : "Menge-Ist",
- 45        "ARTIKEL" : "Artikel",
- 46        "ARTIKELNAME" : "Artikel-Name",
- 47        "UPDDATE" : "geÃ¤ndert am",
- 48        "UPDNAME" : "geÃ¤ndert von"
- 49    }
- 50    df.rename(columns=colNames, inplace=True);
- 51
- 52    return df
- 53
- 54
- 55def ladeAlleWerkstattauftragPosMengenabweichungen(
- 56        server : PyAPplus64.APplusServer,
- 57        cond:PyAPplus64.SqlCondition|str|None=None) -> pd.DataFrame:
- 58    sql = PyAPplus64.sql_utils.SqlStatementSelect("WAUFTRAGPOS w");
- 59    sql.addLeftJoin("personal p", "w.UPDUSER = p.PERSONAL")
- 60
- 61    sql.addFieldsTable("w", "ID", "BAUFTRAG", "POSITION", "AG")
- 62    sql.addFields("(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG")
- 63    sql.addFieldsTable("w", "MENGE", "MENGE_IST", "APLAN as ARTIKEL")
- 64    sql.addFields("w.UPDDATE", "p.NAME as UPDNAME")
+ 43
+ 44    colNames = {
+ 45        "BAUFTRAG": "Betriebsauftrag",
+ 46        "POSITION": "Pos",
+ 47        "MENGENABWEICHUNG": "Mengenabweichung",
+ 48        "MENGE": "Menge",
+ 49        "MENGE_IST": "Menge-Ist",
+ 50        "ARTIKEL": "Artikel",
+ 51        "ARTIKELNAME": "Artikel-Name",
+ 52        "UPDDATE": "geÃ¤ndert am",
+ 53        "UPDNAME": "geÃ¤ndert von"
+ 54    }
+ 55    df.rename(columns=colNames, inplace=True)
+ 56
+ 57    return df
+ 58
+ 59
+ 60def ladeAlleWerkstattauftragPosMengenabweichungen(
+ 61        server: PyAPplus64.APplusServer,
+ 62        cond: Union[PyAPplus64.SqlCondition, str, None] = None) -
+> pd.DataFrame:
+ 63    sql = PyAPplus64.sql_utils.SqlStatementSelect("WAUFTRAGPOS w")
+ 64    sql.addLeftJoin("personal p", "w.UPDUSER = p.PERSONAL")
  65
- 66    sql.where.addConditionFieldEq("w.STATUS", 4)
- 67    sql.where.addCondition("abs(w.MENGE-w.MENGE_IST) > 0.001")
- 68    sql.where.addCondition(cond)
- 69    sql.order="w.UPDDATE"
+ 66    sql.addFieldsTable("w", "ID", "BAUFTRAG", "POSITION", "AG")
+ 67    sql.addFields("(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG")
+ 68    sql.addFieldsTable("w", "MENGE", "MENGE_IST", "APLAN as ARTIKEL")
+ 69    sql.addFields("w.UPDDATE", "p.NAME as UPDNAME")
  70
- 71    dfOrg = PyAPplus64.pandas.pandasReadSql(server, sql);
- 72
- 73    # Add Links
- 74    df = dfOrg.copy();
- 75    df = df.drop(columns=["ID"]);
- 76    df['POSITION'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg,
- 77                        lambda r: r.POSITION,
- 78                        lambda r: server.makeWebLinkWauftrag(
- 79                            bauftrag=r.BAUFTRAG, accessid=r.ID))
- 80    df['BAUFTRAG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg,
- 81                        lambda r: r.BAUFTRAG,
- 82                        lambda r: server.makeWebLinkBauftrag
+ 71    sql.where.addConditionFieldEq("w.STATUS", 4)
+ 72    sql.where.addCondition("abs(w.MENGE-w.MENGE_IST) > 0.001")
+ 73    sql.where.addCondition(cond)
+ 74    sql.order = "w.UPDDATE"
+ 75
+ 76    dfOrg = PyAPplus64.pandas.pandasReadSql(server, sql)
+ 77
+ 78    # Add Links
+ 79    df = dfOrg.copy()
+ 80    df = df.drop(columns=["ID"])
+ 81    df['POSITION'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+ 82                        dfOrg,
+ 83                        lambda r: r.POSITION,
+ 84                        lambda r: server.makeWebLinkWauftrag(
+ 85                            bauftrag=r.BAUFTRAG, accessid=r.ID))
+ 86    df['BAUFTRAG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+ 87                        dfOrg,
+ 88                        lambda r: r.BAUFTRAG,
+ 89                        lambda r: server.makeWebLinkBauftrag
 (bauftrag=r.BAUFTRAG))
- 83    df['AG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg,
- 84                        lambda r: r.AG,
- 85                        lambda r: server.makeWebLinkWauftragPos(
- 86                            bauftrag=r.BAUFTRAG, position=r.POSITION,
+ 90    df['AG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+ 91                        dfOrg,
+ 92                        lambda r: r.AG,
+ 93                        lambda r: server.makeWebLinkWauftragPos(
+ 94                            bauftrag=r.BAUFTRAG, position=r.POSITION,
 accessid=r.ID))
- 87
- 88    # Demo zum HinzufÃ¼gen einer berechneten Spalte
- 89    # df['BAUFPOSAG'] = PyAPplus64.pandas.mkDataframeColumn(dfOrg,
- 90    #                     lambda r: "{}.{} AG {}".format(r.BAUFTRAG,
+ 95
+ 96    # Demo zum HinzufÃ¼gen einer berechneten Spalte
+ 97    # df['BAUFPOSAG'] = PyAPplus64.pandas.mkDataframeColumn(dfOrg,
+ 98    #                     lambda r: "{}.{} AG {}".format(r.BAUFTRAG,
 r.POSITION, r.AG))
- 91
- 92    # Rename Columns
- 93    colNames = {
- 94        "BAUFTRAG" : "Betriebsauftrag",
- 95        "POSITION" : "Pos",
- 96        "AG" : "AG",
- 97        "MENGENABWEICHUNG" : "Mengenabweichung",
- 98        "MENGE" : "Menge",
- 99        "MENGE_IST" : "Menge-Ist",
-100        "ARTIKEL" : "Artikel",
-101        "UPDDATE" : "geÃ¤ndert am",
-102        "UPDNAME" : "geÃ¤ndert von"
-103    }
-104    df.rename(columns=colNames, inplace=True);
-105    return df
-106
-107def computeInYearMonthCond(field : str, year:int|None=None,
-108                           month:int|None=None) -> PyAPplus64.SqlCondition |
-None:
-109    if not (year is None):
-110        if month is None:
-111            return PyAPplus64.sql_utils.SqlConditionDateTimeFieldInYear
+ 99
+100    # Rename Columns
+101    colNames = {
+102        "BAUFTRAG": "Betriebsauftrag",
+103        "POSITION": "Pos",
+104        "AG": "AG",
+105        "MENGENABWEICHUNG": "Mengenabweichung",
+106        "MENGE": "Menge",
+107        "MENGE_IST": "Menge-Ist",
+108        "ARTIKEL": "Artikel",
+109        "UPDDATE": "geÃ¤ndert am",
+110        "UPDNAME": "geÃ¤ndert von"
+111    }
+112    df.rename(columns=colNames, inplace=True)
+113    return df
+114
+115
+116def computeInYearMonthCond(field: str, year: Optional[int] = None,
+117                           month: Optional[int] = None) -> Optional
+[PyAPplus64.SqlCondition]:
+118    if not (year is None):
+119        if month is None:
+120            return PyAPplus64.sql_utils.SqlConditionDateTimeFieldInYear
 (field, year)
-112        else:
-113            return PyAPplus64.sql_utils.SqlConditionDateTimeFieldInMonth
+121        else:
+122            return PyAPplus64.sql_utils.SqlConditionDateTimeFieldInMonth
 (field, year, month)
-114    else:
-115        return None
-116
-117def computeFileName(year:int|None=None, month:int|None=None) -> str:
-118    if year is None:
-119        return 'mengenabweichungen-all.xlsx';
-120    else:
-121        if month is None:
-122            return 'mengenabweichungen-{:04d}.xlsx'.format(year);
-123        else:
-124            return 'mengenabweichungen-{:04d}-{:02d}.xlsx'.format(year,
-month);
+123    else:
+124        return None
 125
-126def _exportInternal(server: PyAPplus64.APplusServer, fn:str,
-127                    cond:Union[PyAPplus64.SqlCondition, str, None]) -> int:
-128    df1 = ladeAlleWerkstattauftragMengenabweichungen(server, cond)
-129    df2 = ladeAlleWerkstattauftragPosMengenabweichungen(server, cond)
-130    print ("erzeuge " + fn);
-131    PyAPplus64.pandas.exportToExcel(fn, [(df1, "WAuftrag"), (df2, "WAuftrag-
+126
+127def computeFileName(year: Optional[int] = None, month: Optional[int] = None)
+-> str:
+128    if year is None:
+129        return 'mengenabweichungen-all.xlsx'
+130    else:
+131        if month is None:
+132            return 'mengenabweichungen-{:04d}.xlsx'.format(year)
+133        else:
+134            return 'mengenabweichungen-{:04d}-{:02d}.xlsx'.format(year,
+month)
+135
+136
+137def _exportInternal(server: PyAPplus64.APplusServer, fn: str,
+138                    cond: Union[PyAPplus64.SqlCondition, str, None]) -> int:
+139    df1 = ladeAlleWerkstattauftragMengenabweichungen(server, cond)
+140    df2 = ladeAlleWerkstattauftragPosMengenabweichungen(server, cond)
+141    print("erzeuge " + fn)
+142    PyAPplus64.pandas.exportToExcel(fn, [(df1, "WAuftrag"), (df2, "WAuftrag-
 Pos")], addTable=True)
-132    return len(df1.index) + len(df2.index)
-133
-134def exportVonBis(server: PyAPplus64.APplusServer, fn:str,
-135                 von:datetime.datetime|None, bis:datetime.datetime|None) -
-> int:
-136  cond = PyAPplus64.sql_utils.SqlConditionDateTimeFieldInRange("w.UPDDATE",
-von, bis)
-137  return _exportInternal(server, fn, cond)
-138
-139def exportYearMonth(server: PyAPplus64.APplusServer,
-140                    year:int|None=None, month:int|None=None) -> int:
-141    cond=computeInYearMonthCond("w.UPDDATE", year=year, month=month)
-142    fn = computeFileName(year=year, month=month)
-143    return _exportInternal(server, fn, cond)
+143    return len(df1.index) + len(df2.index)
 144
-145def computePreviousMonthYear(cyear : int, cmonth :int) -> Tuple[int, int]:
-146    if cmonth == 1:
-147        return (cyear-1, 12)
-148    else:
-149        return (cyear, cmonth-1);
+145
+146def exportVonBis(server: PyAPplus64.APplusServer, fn: str,
+147                 von: Optional[datetime.datetime], bis: Optional
+[datetime.datetime]) -> int:
+148    cond = PyAPplus64.sql_utils.SqlConditionDateTimeFieldInRange
+("w.UPDDATE", von, bis)
+149    return _exportInternal(server, fn, cond)
 150
-151def computeNextMonthYear(cyear : int, cmonth :int) -> Tuple[int, int]:
-152    if cmonth == 12:
-153        return (cyear+1, 1)
-154    else:
-155        return (cyear, cmonth+1);
-156
-157def main(confFile : str|pathlib.Path, user:str|None=None, env:str|None=None)
--> None:
-158    server = PyAPplus64.applusFromConfigFile(confFile, user=user, env=env)
-159
-160    now = datetime.date.today()
-161    (cmonth, cyear) = (now.month, now.year)
-162    (pyear, pmonth) = computePreviousMonthYear(cyear, cmonth);
-163
-164    # Ausgaben
-165    exportYearMonth(server, cyear, cmonth) # Aktueller Monat
-166    exportYearMonth(server, pyear, pmonth) # Vorheriger Monat
-167    # export(cyear) # aktuelles Jahr
-168    # export(cyear-1) # letztes Jahr
-169    # export() # alles
-170
-171if __name__ == "__main__":
-172    main(applus_configs.serverConfYamlTest)
+151
+152def exportYearMonth(server: PyAPplus64.APplusServer,
+153                    year: Optional[int] = None, month: Optional[int] = None)
+-> int:
+154    cond = computeInYearMonthCond("w.UPDDATE", year=year, month=month)
+155    fn = computeFileName(year=year, month=month)
+156    return _exportInternal(server, fn, cond)
+157
+158
+159def computePreviousMonthYear(cyear: int, cmonth: int) -> Tuple[int, int]:
+160    if cmonth == 1:
+161        return (cyear-1, 12)
+162    else:
+163        return (cyear, cmonth-1)
+164
+165
+166def computeNextMonthYear(cyear: int, cmonth: int) -> Tuple[int, int]:
+167    if cmonth == 12:
+168        return (cyear+1, 1)
+169    else:
+170        return (cyear, cmonth+1)
+171
+172
+173def main(confFile: Union[str, pathlib.Path], user: Optional[str] = None,
+env: Optional[str] = None) -> None:
+174    server = PyAPplus64.applusFromConfigFile(confFile, user=user, env=env)
+175
+176    now = datetime.date.today()
+177    (cmonth, cyear) = (now.month, now.year)
+178    (pyear, pmonth) = computePreviousMonthYear(cyear, cmonth)
+179
+180    # Ausgaben
+181    exportYearMonth(server, cyear, cmonth)  # Aktueller Monat
+182    exportYearMonth(server, pyear, pmonth)  # Vorheriger Monat
+183    # export(cyear) # aktuelles Jahr
+184    # export(cyear-1) # letztes Jahr
+185    # export() # alles
+186
+187
+188if __name__ == "__main__":
+189    main(applus_configs.serverConfYamlTest)
 
 ***** mengenabweichung_gui.pyÂ¶ *****
 Beispiel fÃ¼r eine sehr einfache GUI, die die Eingabe einfacher Parameter
 erlaubt. Die GUI wird um die Erzeugung von Excel-Dateien mit Mengenabweichungen
 gebaut.
- 1import PySimpleGUI as sg # type: ignore
+ 1import PySimpleGUI as sg  # type: ignore
  2import mengenabweichung
  3import datetime
  4import PyAPplus64
  5import applus_configs
  6import pathlib
- 7from typing import *
+ 7from typing import Tuple, Optional, Union
  8
- 9def parseDate (dateS:str) -> Tuple[datetime.datetime|None, bool]:
-10    if dateS is None or dateS == '':
-11        return (None, True)
-12    else:
-13        try:
-14            return (datetime.datetime.strptime(dateS, '%d.%m.%Y'), True)
-15        except:
-16            sg.popup_error("Fehler beim Parsen des Datums '{}'".format
+ 9
+10def parseDate(dateS: str) -> Tuple[Optional[datetime.datetime], bool]:
+11    if dateS is None or dateS == '':
+12        return (None, True)
+13    else:
+14        try:
+15            return (datetime.datetime.strptime(dateS, '%d.%m.%Y'), True)
+16        except:
+17            sg.popup_error("Fehler beim Parsen des Datums '{}'".format
 (dateS))
-17            return (None, False)
-18
-19def createFile(server:PyAPplus64.APplusServer, fileS:str, vonS:str, bisS:
-str)->None:
-20    (von, vonOK) = parseDate(vonS)
-21    if not vonOK: return
-22
-23    (bis, bisOK) = parseDate(bisS)
-24    if not bisOK: return
+18            return (None, False)
+19
+20
+21def createFile(server: PyAPplus64.APplusServer, fileS: str, vonS: str, bisS:
+str) -> None:
+22    (von, vonOK) = parseDate(vonS)
+23    if not vonOK:
+24        return
 25
-26    if (fileS is None) or fileS == '':
-27        sg.popup_error("Es wurde keine Ausgabedatei ausgewÃ¤hlt.")
+26    (bis, bisOK) = parseDate(bisS)
+27    if not bisOK:
 28        return
-29    else:
-30        file = pathlib.Path(fileS)
-31
-32    c = mengenabweichung.exportVonBis(server, file.as_posix(), von, bis)
-33    sg.popup_ok("{} DatensÃ¤tze erfolgreich in Datei '{}'
-geschrieben.".format(c, file))
-34
+29
+30    if (fileS is None) or fileS == '':
+31        sg.popup_error("Es wurde keine Ausgabedatei ausgewÃ¤hlt.")
+32        return
+33    else:
+34        file = pathlib.Path(fileS)
 35
-36def main(confFile : str|pathlib.Path, user:str|None=None, env:str|None=None)
--> None:
-37    server = PyAPplus64.applusFromConfigFile(confFile, user=user, env=env)
+36    c = mengenabweichung.exportVonBis(server, file.as_posix(), von, bis)
+37    sg.popup_ok("{} DatensÃ¤tze erfolgreich in Datei '{}'
+geschrieben.".format(c, file))
 38
-39    layout = [
-40        [sg.Text(('Bitte geben Sie an, fÃ¼r welchen Zeitraum die '
-41                  'Mengenabweichungen ausgegeben werden sollen:'))],
-42        [sg.Text('Von (einschlieÃlich)', size=(15,1)), sg.InputText
+39
+40def main(confFile: Union[str, pathlib.Path], user: Optional[str] = None, env:
+Optional[str] = None) -> None:
+41    server = PyAPplus64.applusFromConfigFile(confFile, user=user, env=env)
+42
+43    layout = [
+44        [sg.Text(('Bitte geben Sie an, fÃ¼r welchen Zeitraum die '
+45                  'Mengenabweichungen ausgegeben werden sollen:'))],
+46        [sg.Text('Von (einschlieÃlich)', size=(15, 1)), sg.InputText
 (key='Von'),
-43         sg.CalendarButton("Kalender", close_when_date_chosen=True,
-44                           target="Von", format='%d.%m.%Y')],
-45        [sg.Text('Bis (ausschlieÃlich)', size=(15,1)), sg.InputText
+47         sg.CalendarButton("Kalender", close_when_date_chosen=True,
+48                           target="Von", format='%d.%m.%Y')],
+49        [sg.Text('Bis (ausschlieÃlich)', size=(15, 1)), sg.InputText
 (key='Bis'),
-46         sg.CalendarButton("Kalender", close_when_date_chosen=True,
-47                           target="Bis", format='%d.%m.%Y')],
-48        [sg.Text('Ausgabedatei', size=(15,1)), sg.InputText(key='File'),
-49        sg.FileSaveAs(button_text="wÃ¤hlen", target="File",
-50                      file_types = (('Excel Files', '*.xlsx'),),
-51                      default_extension = ".xlsx")],
-52        [sg.Button("Aktueller Monat"), sg.Button("Letzter Monat"),
-53         sg.Button("Aktuelles Jahr"), sg.Button("Letztes Jahr")],
-54        [sg.Button("Speichern"), sg.Button("Beenden")]
-55    ]
-56
-57    systemName = server.scripttool.getSystemName() + "/" +
+50         sg.CalendarButton("Kalender", close_when_date_chosen=True,
+51                           target="Bis", format='%d.%m.%Y')],
+52        [sg.Text('Ausgabedatei', size=(15, 1)), sg.InputText(key='File'),
+53         sg.FileSaveAs(button_text="wÃ¤hlen",
+54                       target="File",
+55                       file_types=(('Excel Files', '*.xlsx'),),
+56                       default_extension=".xlsx")],
+57        [sg.Button("Aktueller Monat"), sg.Button("Letzter Monat"),
+58         sg.Button("Aktuelles Jahr"), sg.Button("Letztes Jahr")],
+59        [sg.Button("Speichern"), sg.Button("Beenden")]
+60    ]
+61
+62    systemName = server.scripttool.getSystemName() + "/" +
 server.scripttool.getMandant()
-58    window = sg.Window("Mengenabweichung " + systemName, layout)
-59    now = datetime.date.today()
-60    (cmonth, cyear) = (now.month, now.year)
-61    (pyear, pmonth) = mengenabweichung.computePreviousMonthYear(cyear,
-cmonth);
-62    (nyear, nmonth) = mengenabweichung.computeNextMonthYear(cyear, cmonth);
-63
-64    while True:
-65        event, values = window.read()
-66        if event == sg.WIN_CLOSED or event == 'Beenden':
-67            break
-68        if event == 'Aktueller Monat':
-69            window['Von'].update(value="01.{:02d}.{:04d}".format(cmonth,
-cyear));
-70            window['Bis'].update(value="01.{:02d}.{:04d}".format(nmonth,
-nyear));
-71        if event == 'Letzter Monat':
-72            window['Von'].update(value="01.{:02d}.{:04d}".format(pmonth,
-pyear));
-73            window['Bis'].update(value="01.{:02d}.{:04d}".format(cmonth,
-cyear));
-74        if event == 'Aktuelles Jahr':
-75            window['Von'].update(value="01.01.{:04d}".format(cyear));
-76            window['Bis'].update(value="01.01.{:04d}".format(cyear+1));
-77        if event == 'Letztes Jahr':
-78            window['Von'].update(value="01.01.{:04d}".format(cyear-1));
-79            window['Bis'].update(value="01.01.{:04d}".format(cyear));
-80        if event == 'Speichern':
-81            try:
-82                createFile(server, values.get('File', None),
-83                           values.get('Von', None), values.get('Bis', None))
-84            except Exception as e:
-85                sg.popup_error_with_traceback("Beim Erzeugen der Excel-Datei
-trat ein Fehler auf:", e);
-86
-87    window.close()
-88
-89if __name__ == "__main__":
-90    main(applus_configs.serverConfYamlProd)
+63    window = sg.Window("Mengenabweichung " + systemName, layout)
+64    now = datetime.date.today()
+65    (cmonth, cyear) = (now.month, now.year)
+66    (pyear, pmonth) = mengenabweichung.computePreviousMonthYear(cyear,
+cmonth)
+67    (nyear, nmonth) = mengenabweichung.computeNextMonthYear(cyear, cmonth)
+68
+69    while True:
+70        event, values = window.read()
+71        if event == sg.WIN_CLOSED or event == 'Beenden':
+72            break
+73        if event == 'Aktueller Monat':
+74            window['Von'].update(value="01.{:02d}.{:04d}".format(cmonth,
+cyear))
+75            window['Bis'].update(value="01.{:02d}.{:04d}".format(nmonth,
+nyear))
+76        if event == 'Letzter Monat':
+77            window['Von'].update(value="01.{:02d}.{:04d}".format(pmonth,
+pyear))
+78            window['Bis'].update(value="01.{:02d}.{:04d}".format(cmonth,
+cyear))
+79        if event == 'Aktuelles Jahr':
+80            window['Von'].update(value="01.01.{:04d}".format(cyear))
+81            window['Bis'].update(value="01.01.{:04d}".format(cyear+1))
+82        if event == 'Letztes Jahr':
+83            window['Von'].update(value="01.01.{:04d}".format(cyear-1))
+84            window['Bis'].update(value="01.01.{:04d}".format(cyear))
+85        if event == 'Speichern':
+86            try:
+87                createFile(server, values.get('File', None),
+88                           values.get('Von', None), values.get('Bis', None))
+89            except Exception as e:
+90                sg.popup_error_with_traceback("Beim Erzeugen der Excel-Datei
+trat ein Fehler auf:", e)
+91
+92    window.close()
+93
+94
+95if __name__ == "__main__":
+96    main(applus_configs.serverConfYamlProd)
 
 ***** copy_artikel.pyÂ¶ *****
 Beispiel, wie Artikel inklusive Arbeitsplan und StÃ¼ckliste dupliziert werden
 kann.
- 1import PyAPplus64
- 2import applus_configs
- 3import logging
- 4import yaml
- 5
- 6
- 7def main(confFile:pathlib.Path, artikel:str, artikelNeu:str|None=None) -
-> None:
- 8    # Server verbinden
- 9    server = PyAPplus64.applus.applusFromConfigFile(confFile)
-10
-11    # DuplicateBusinessObject fÃ¼r Artikel erstellen
-12    dArt = PyAPplus64.duplicate.loadDBDuplicateArtikel(server, artikel);
-13
-14    # DuplicateBusinessObject zur Demonstration in YAML konvertieren und
+ 1import pathlib
+ 2import PyAPplus64
+ 3import applus_configs
+ 4import logging
+ 5import yaml
+ 6from typing import Optional
+ 7
+ 8
+ 9def main(confFile: pathlib.Path, artikel: str, artikelNeu: Optional[str] =
+None) -> None:
+10    # Server verbinden
+11    server = PyAPplus64.applus.applusFromConfigFile(confFile)
+12
+13    # DuplicateBusinessObject fÃ¼r Artikel erstellen
+14    dArt = PyAPplus64.duplicate.loadDBDuplicateArtikel(server, artikel)
+15
+16    # DuplicateBusinessObject zur Demonstration in YAML konvertieren und
 zurÃ¼ck
-15    dArtYaml = yaml.dump(dArt);
-16    print(dArtYaml);
-17    dArt2 = yaml.load(dArtYaml, Loader=yaml.UnsafeLoader)
-18
-19    # Neue Artikel-Nummer bestimmen und DuplicateBusinessObject in DB
+17    dArtYaml = yaml.dump(dArt)
+18    print(dArtYaml)
+19    dArt2 = yaml.load(dArtYaml, Loader=yaml.UnsafeLoader)
+20
+21    # Neue Artikel-Nummer bestimmen und DuplicateBusinessObject in DB
 schreiben
-20    # Man kÃ¶nnte hier genauso gut einen anderen Server verwenden
-21    if (artikelNeu is None):
-22        artikelNeu = server.nextNumber("Artikel")
-23
-24    if not (dArt is None):
-25        dArt.setFields({"artikel" : artikelNeu})
-26        res = dArt.insert(server);
-27        print(res);
-28
-29
-30if __name__ == "__main__":
-31    # Logger Einrichten
-32    logging.basicConfig(level=logging.INFO)
-33    # logger = logging.getLogger("PyAPplus64.applus_db");
-34    # logger.setLevel(logging.ERROR)
-35
-36    main(applus_configs.serverConfYamlTest, "my-artikel", artikelNeu="my-
-artikel-copy")
+22    # Man kÃ¶nnte hier genauso gut einen anderen Server verwenden
+23    if (artikelNeu is None):
+24        artikelNeu = server.nextNumber("Artikel")
+25
+26    if not (dArt is None):
+27        dArt.setFields({"artikel": artikelNeu})
+28        res = dArt.insert(server)
+29        print(res)
+30
+31
+32if __name__ == "__main__":
+33    # Logger Einrichten
+34    logging.basicConfig(level=logging.INFO)
+35    # logger = logging.getLogger("PyAPplus64.applus_db");
+36    # logger.setLevel(logging.ERROR)
 37
+38    main(applus_configs.serverConfYamlTest, "my-artikel", artikelNeu="my-
+artikel-copy")
 
 **** Inhaltsverzeichnis ****
     * Beispiele
           o Config-Dateien
+          o read_settings.py
           o check_dokumente.py
           o adhoc_report.py
           o mengenabweichung.py
           o mengenabweichung_gui.py
           o copy_artikel.py
 *** Vorheriges Thema ***
 AbhÃ¤ngigkeiten
@@ -478,10 +570,10 @@
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
     * weiter |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Beispiele
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/generated/PyAPplus64.html` & `PyAPplus64-1.0.1/docs/build/html/generated/PyAPplus64.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>PyAPplus64 package &#8212; PyAPplus64  Dokumentation</title>
+    <title>PyAPplus64 package &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/jquery.js"></script>
     <script src="../_static/underscore.js"></script>
     <script src="../_static/doctools.js"></script>
     <script src="../_static/translations.js"></script>
@@ -34,15 +26,15 @@
              accesskey="I">Index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python-Modulindex"
              >Module</a> |</li>
         <li class="right" >
           <a href="../examples.html" title="Beispiele"
              accesskey="P">zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">PyAPplus64 package</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1817,27 +1809,27 @@
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionTrue</span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionTrue" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#PyAPplus64.sql_utils.SqlConditionPrepared" title="PyAPplus64.sql_utils.SqlConditionPrepared"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyAPplus64.sql_utils.SqlConditionPrepared</span></code></a></p>
 <p>True-Bedingung</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlDate">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlDate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">d</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.date</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">4,</span> <span class="pre">28,</span> <span class="pre">10,</span> <span class="pre">50,</span> <span class="pre">34,</span> <span class="pre">308109)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlDate" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlDate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">d</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.date</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">6,</span> <span class="pre">22,</span> <span class="pre">11,</span> <span class="pre">50,</span> <span class="pre">888219)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlDate" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Wrapper um DateTime, die die Formatierung erleichtern</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><p><strong>d</strong> (<em>Union</em><em>[</em><em>datetime.datetime</em><em>, </em><em>datetime.date</em><em>]</em>) – das Datum</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlDateTime">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlDateTime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dt</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.date</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">4,</span> <span class="pre">28,</span> <span class="pre">10,</span> <span class="pre">50,</span> <span class="pre">34,</span> <span class="pre">308099)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlDateTime" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlDateTime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dt</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.date</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">6,</span> <span class="pre">22,</span> <span class="pre">11,</span> <span class="pre">50,</span> <span class="pre">888210)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlDateTime" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Wrapper um DateTime, die die Formatierung erleichtern</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><p><strong>dt</strong> (<em>Union</em><em>[</em><em>datetime.datetime</em><em>, </em><em>datetime.date</em><em>]</em>) – der Zeitpunkt</p>
 </dd>
 </dl>
@@ -2041,15 +2033,15 @@
 <dd><p>die Bedingung, Default ist True</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlTime">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlTime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">t</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">4,</span> <span class="pre">28,</span> <span class="pre">10,</span> <span class="pre">50,</span> <span class="pre">34,</span> <span class="pre">308116)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlTime" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlTime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">t</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">6,</span> <span class="pre">22,</span> <span class="pre">11,</span> <span class="pre">50,</span> <span class="pre">888223)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlTime" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Wrapper um DateTime, die die Formatierung erleichtern</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><p><strong>t</strong> (<em>Union</em><em>[</em><em>datetime.datetime</em><em>, </em><em>datetime.time</em><em>]</em>) – die Zeit</p>
 </dd>
 </dl>
@@ -2217,15 +2209,15 @@
              >Index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python-Modulindex"
              >Module</a> |</li>
         <li class="right" >
           <a href="../examples.html" title="Beispiele"
              >zurück</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">PyAPplus64 package</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 **** Navigation ****
     * Index
     * Module |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * PyAPplus64 package
 ****** PyAPplus64 packageÂ¶ ******
 ***** SubmodulesÂ¶ *****
 
 ***** PyAPplus64.applus moduleÂ¶ *****
   classPyAPplus64.applus.APplusServer(db_settings:
   PyAPplus64.applus_db.APplusDBSettings, server_settings:
@@ -998,21 +998,21 @@
         Parameter
                 * field (str) â das Feld
                 * value (str) â der Wert
   classPyAPplus64.sql_utils.SqlConditionTrueÂ¶
       Bases: PyAPplus64.sql_utils.SqlConditionPrepared
       True-Bedingung
   classPyAPplus64.sql_utils.SqlDate(d: Union[datetime.datetime, datetime.date]
-  = datetime.datetime(2023, 4, 28, 10, 50, 34, 308109))Â¶
+  = datetime.datetime(2023, 5, 6, 22, 11, 50, 888219))Â¶
       Bases: object
       Wrapper um DateTime, die die Formatierung erleichtern
         Parameter
             d (Union[datetime.datetime,datetime.date]) â das Datum
   classPyAPplus64.sql_utils.SqlDateTime(dt: Union[datetime.datetime,
-  datetime.date] = datetime.datetime(2023, 4, 28, 10, 50, 34, 308099))Â¶
+  datetime.date] = datetime.datetime(2023, 5, 6, 22, 11, 50, 888210))Â¶
       Bases: object
       Wrapper um DateTime, die die Formatierung erleichtern
         Parameter
             dt (Union[datetime.datetime,datetime.date]) â der Zeitpunkt
   classPyAPplus64.sql_utils.SqlField(fn: str)Â¶
       Bases: object
       Wrapper um SQL Feldnamen, die die Formatierung erleichtern
@@ -1100,15 +1100,15 @@
         table: strÂ¶
             die Tabelle
         top: intÂ¶
             wie viele DatensÃ¤tze auswÃ¤hlen? 0 fÃ¼r alle
         where: PyAPplus64.sql_utils.SqlConditionListÂ¶
             die Bedingung, Default ist True
   classPyAPplus64.sql_utils.SqlTime(t: Union[datetime.datetime, datetime.time]
-  = datetime.datetime(2023, 4, 28, 10, 50, 34, 308116))Â¶
+  = datetime.datetime(2023, 5, 6, 22, 11, 50, 888223))Â¶
       Bases: object
       Wrapper um DateTime, die die Formatierung erleichtern
         Parameter
             t (Union[datetime.datetime,datetime.time]) â die Zeit
   PyAPplus64.sql_utils.SqlValueÂ¶
       Union-Type aller unterstÃ¼tzter SQL-Werte
       alias of Union[str, int, float, PyAPplus64.sql_utils.SqlParam,
@@ -1183,10 +1183,10 @@
     * Quellcode_anzeigen
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
     * zurÃ¼ck |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * PyAPplus64 package
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/genindex.html` & `PyAPplus64-1.0.1/docs/build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Stichwortverzeichnis &#8212; PyAPplus64  Dokumentation</title>
+    <title>Stichwortverzeichnis &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/translations.js"></script>
@@ -29,15 +21,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="Stichwortverzeichnis"
              accesskey="I">Index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python-Modulindex"
              >Module</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Stichwortverzeichnis</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -806,15 +798,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="Stichwortverzeichnis"
              >Index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python-Modulindex"
              >Module</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Stichwortverzeichnis</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 **** Navigation ****
     * Index
     * Module |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Stichwortverzeichnis
 ****** Stichwortverzeichnis ******
 A | C | D | E | F | G | H | I | J | L | M | N | O | P | R | S | T | U | W | X
 ***** A *****
     * add()_(Methode_von
       PyAPplus64.applus_db.DBTableIDs)           * addDependentBusinessObject()_(Methode_von
     * addCondition()_(Methode_von                  PyAPplus64.duplicate.DuplicateBusinessObject)
@@ -293,10 +293,10 @@
 ***** X *****
     * XMLDefinition_(Klasse_in_PyAPplus64.applus_scripttool)
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Stichwortverzeichnis
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/index.html` & `PyAPplus64-1.0.1/docs/build/html/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>PyAPplus64 Dokumentation &#8212; PyAPplus64  Dokumentation</title>
+    <title>PyAPplus64 Dokumentation &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/translations.js"></script>
@@ -34,15 +26,15 @@
              accesskey="I">Index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python-Modulindex"
              >Module</a> |</li>
         <li class="right" >
           <a href="beschreibung.html" title="Beschreibung"
              accesskey="N">weiter</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">PyAPplus64 Dokumentation</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -100,15 +92,15 @@
              >Index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python-Modulindex"
              >Module</a> |</li>
         <li class="right" >
           <a href="beschreibung.html" title="Beschreibung"
              >weiter</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">PyAPplus64 Dokumentation</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 **** Navigation ****
     * Index
     * Module |
     * weiter |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * PyAPplus64 Dokumentation
 ****** PyAPplus64 DokumentationÂ¶ ******
     * Beschreibung
     * typische_AnwendungsfÃ¤lle
     * AbhÃ¤ngigkeiten
     * Beispiele
     * PyAPplus64_package
@@ -22,10 +22,10 @@
     * Quellcode_anzeigen
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
     * weiter |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * PyAPplus64 Dokumentation
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/objects.inv` & `PyAPplus64-1.0.1/docs/build/html/objects.inv`

 * *Files 2% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: PyAPplus64
-# Version: 
+# Version: 1.0.1
 # The remainder of this file is compressed using zlib.
 
 PyAPplus64 py:module 0 generated/PyAPplus64.html#module-$ -
 PyAPplus64.applus py:module 0 generated/PyAPplus64.html#module-$ -
 PyAPplus64.applus.APplusServer py:class 1 generated/PyAPplus64.html#$ -
 PyAPplus64.applus.APplusServer.completeSQL py:method 1 generated/PyAPplus64.html#$ -
 PyAPplus64.applus.APplusServer.dbQuery py:method 1 generated/PyAPplus64.html#$ -
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/py-modindex.html` & `PyAPplus64-1.0.1/docs/build/html/py-modindex.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python-Modulindex &#8212; PyAPplus64  Dokumentation</title>
+    <title>Python-Modulindex &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/translations.js"></script>
@@ -32,15 +24,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="Stichwortverzeichnis"
              accesskey="I">Index</a></li>
         <li class="right" >
           <a href="#" title="Python-Modulindex"
              >Module</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python-Modulindex</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -141,15 +133,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="Stichwortverzeichnis"
              >Index</a></li>
         <li class="right" >
           <a href="#" title="Python-Modulindex"
              >Module</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python-Modulindex</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 **** Navigation ****
     * Index
     * Module |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Python-Modulindex
 ****** Python-Modulindex ******
 p
      
     p
 [-] PyAPplus64
         PyAPplus64.applus
@@ -24,10 +24,10 @@
         PyAPplus64.sql_utils
         PyAPplus64.utils
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Python-Modulindex
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/search.html` & `PyAPplus64-1.0.1/docs/build/html/search.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-<!--
--- Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
---
--- This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
---
--- Use of this source code is governed by an MIT-style
--- license that can be found in the LICENSE file or at
--- https://opensource.org/licenses/MIT.-->
 
 <!DOCTYPE html>
 
 <html lang="de">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Suche &#8212; PyAPplus64  Dokumentation</title>
+    <title>Suche &#8212; PyAPplus64 1.0.1 Dokumentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -35,15 +27,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="Stichwortverzeichnis"
              accesskey="I">Index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python-Modulindex"
              >Module</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Suche</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -94,15 +86,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="Stichwortverzeichnis"
              >Index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python-Modulindex"
              >Module</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64  Dokumentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyAPplus64 1.0.1 Dokumentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Suche</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2023, Thomas Tuerk.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.3.2.
     </div>
```

#### html2text {}

```diff
@@ -2,19 +2,19 @@
 
 
 
 
 **** Navigation ****
     * Index
     * Module |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Suche
 ****** Suche ******
 Bitte aktivieren Sie JavaScript, wenn Sie die Suchfunktion nutzen wollen.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [suchen]
 **** Navigation ****
     * Index
     * Module |
-    * PyAPplus64_Dokumentation »
+    * PyAPplus64_1.0.1_Dokumentation »
     * Suche
 © Copyright 2023, Thomas Tuerk. Created using Sphinx 4.3.2.
```

### Comparing `PyAPplus64-1.0.0/docs/build/html/searchindex.js` & `PyAPplus64-1.0.1/docs/build/html/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,7 @@
-/*
- * Copyright (c) 2023 Thomas Tuerk (kontakt@thomas-tuerk.de)
- *
- * This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
- *
- * Use of this source code is governed by an MIT-style
- * license that can be found in the LICENSE file or at
- * https://opensource.org/licenses/MIT. */
 Search.setIndex({
     docnames: ["abhaengigkeiten", "anwendungen", "beschreibung", "examples", "generated/PyAPplus64", "index"],
     envversion: {
         "sphinx.domains.c": 2,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 4,
@@ -335,35 +327,62 @@
     terms: {
         "0": [3, 4],
         "001": 3,
         "01": 3,
         "02d": 3,
         "04d": 3,
         "1": [3, 4],
-        "10": 4,
+        "11": 4,
         "12": 3,
+        "14": [],
         "15": 3,
+        "17": [],
+        "18": [],
         "2": [0, 1, 3],
         "2012": 0,
-        "2023": [1, 4],
+        "2023": 4,
         "2037": 3,
-        "23": [],
-        "28": 4,
+        "22": 4,
+        "24": [],
+        "247492": [],
+        "247501": [],
+        "247507": [],
+        "27": [],
+        "29": [],
         "3": 3,
-        "308099": 4,
-        "308109": 4,
-        "308116": 4,
-        "34": 4,
-        "386330": [],
-        "386341": [],
-        "386348": [],
-        "4": [2, 3, 4],
-        "5": 3,
+        "4": [2, 3],
+        "45": [],
+        "46": [],
+        "48": [],
+        "5": [3, 4],
         "50": 4,
-        "6": 2,
+        "51": [],
+        "533586": [],
+        "533594": [],
+        "533598": [],
+        "58": [],
+        "6": [2, 4],
+        "734716": [],
+        "734722": [],
+        "734726": [],
+        "746273": [],
+        "746286": [],
+        "746292": [],
+        "80523": [],
+        "80533": [],
+        "80538": [],
+        "873776": [],
+        "873786": [],
+        "873790": [],
+        "888210": 4,
+        "888219": 4,
+        "888223": 4,
+        "917696": [],
+        "917703": [],
+        "917707": [],
         "\u00c4nderung": 4,
         "\u00c4nderungen": [1, 2, 4],
         "boolean": 4,
         "break": 3,
         "class": 4,
         "default": [3, 4],
         "do": 4,
@@ -373,44 +392,45 @@
         "if": [1, 3],
         "import": [1, 3],
         "int": [0, 1, 3, 4],
         "m\u00fcssen": [3, 4],
         "n\u00e4chsten": 2,
         "null": [1, 3, 4],
         "return": [3, 4],
-        "this": 1,
+        "this": [],
         "true": [1, 3, 4],
         "try": 3,
         "w\u00e4re": 1,
         "w\u00e4ren": 1,
         Als: [1, 4],
         Auch: 4,
         Bei: [1, 4],
         Bis: 3,
         Da: 4,
         Damit: [3, 4],
         Das: [1, 2, 4],
         Dazu: 4,
         Der: [0, 4],
         Die: [0, 1, 3, 4],
-        Dies: [1, 4],
+        Dies: [1, 3, 4],
         Diese: [0, 1, 3, 4],
         Dieser: [0, 4],
         Dieses: [1, 4],
         Ein: [3, 4],
         Eine: 4,
         Einige: 4,
         Es: [1, 2, 3, 4],
         Etwas: 3,
         Hier: 4,
         Ich: [1, 2],
         Ihre: 2,
         Im: [1, 3, 4],
         In: [2, 4],
         Ist: [3, 4],
+        MIT: [],
         Man: [1, 3],
         Nach: 1,
         Sehr: 3,
         Sie: [0, 2, 3],
         So: 4,
         Sollen: 0,
         Viele: [1, 3],
@@ -423,15 +443,15 @@
         Zum: 4,
         __file__: 3,
         __main__: [1, 3],
         __name__: [1, 3],
         _bas: 4,
         _exportinternal: 3,
         _typing: 4,
-        a: [2, 4],
+        a: [2, 3, 4],
         ab: 4,
         abfrag: [1, 2, 3],
         abgeles: 4,
         abgesetzt: 1,
         abhang: [2, 4, 5],
         abs: 3,
         abstrakt: 4,
@@ -518,57 +538,64 @@
         apply: 4,
         appserv: [2, 3, 4],
         appserverport: 4,
         arbeit: 4,
         arbeitsplan: [2, 3, 4],
         arbeitsplanposition: 4,
         arg: 4,
-        art: 4,
+        art: [3, 4],
         artikel: [1, 3, 4],
         artikeldefinition: 4,
         artikeln: [1, 2],
         artikelnam: 3,
         artikelneu: 3,
         artikelrec: 1,
+        artikelstell: 3,
+        artklassifnrlaeng: 3,
         as: [1, 3],
         as_posix: 3,
         asol: 3,
         aspx: 1,
+        at: [],
         attribut: [2, 4],
         aufgabenstell: 2,
         aufgeruf: 4,
         aufruf: [0, 1, 2, 4],
         auftrag: 4,
+        auftragsart: 3,
         auftret: [1, 4],
         ausdruck: 4,
         ausgab: [1, 3],
         ausgabedatei: 3,
         ausgeb: 4,
         ausgefeilt: 4,
         ausgefuhrt: [2, 4],
         ausgegeb: [1, 3],
         ausgeschloss: 4,
         ausgewahlt: [3, 4],
         ausgewertet: 2,
+        ausles: 3,
+        ausli: 3,
         ausschliess: [3, 4],
         auswahl: 4,
         auszuwahl: 4,
-        automat: [1, 2, 4],
+        automat: [1, 2, 3, 4],
         automatisi: 1,
         automatisiert: [0, 4],
         b: [2, 4],
         bas: 4,
         basedir: 3,
         baseurl: [3, 4],
         basi: 4,
         basicconf: 3,
         bat: 0,
         bau: 4,
         baufposag: 3,
         bauftrag: 3,
+        be: [],
         beding: [1, 3, 4],
         beend: 3,
         beginn: 4,
         beim: [3, 4],
         beinhaltet: 4,
         beispiel: [1, 2, 4, 5],
         beispielsweis: [1, 2, 3],
@@ -582,15 +609,15 @@
         berechn: 4,
         berechnet: [3, 4],
         bereit: 4,
         beschreib: 5,
         besitz: 4,
         besond: 4,
         bestimm: 3,
-        bestimmt: [1, 2, 4],
+        bestimmt: [1, 2, 3, 4],
         betriebsauftrag: 3,
         bevorzug: 4,
         bezieh: 4,
         bezog: 0,
         bibliothek: 1,
         bietet: [1, 3],
         bild: [1, 3],
@@ -605,19 +632,20 @@
         business: [2, 4],
         businessobject: 4,
         businessobjekt: 4,
         button: 3,
         button_text: 3,
         by: [1, 3],
         byt: 4,
-        c: [1, 3],
+        c: 3,
         cach: 4,
         calendarbutton: 3,
         call: 1,
         callabl: 4,
+        can: [],
         charset: 4,
         check: [2, 4],
         checkdirexist: 4,
         checkexist: 4,
         checkfieldset: 4,
         checkfieldsset: 4,
         checkfileexist: 4,
@@ -642,19 +670,22 @@
         config: [0, 1, 4],
         configdir: 3,
         connect: 4,
         connection: 4,
         connector: 4,
         containsonlyallowedchar: 4,
         copy: 3,
-        copyright: 1,
+        copyright: [],
         cor: 4,
         count: [1, 3],
         createfil: 3,
         createsqlalchemyengin: 4,
+        currentdat: 3,
+        currentdatetim: 3,
+        currenttim: 3,
         cyear: 3,
         d: [1, 2, 3, 4],
         dabei: [1, 2, 4],
         dadurch: 1,
         dafur: [1, 4],
         dah: 2,
         danach: 4,
@@ -689,17 +720,18 @@
         dbquery: 4,
         dbqueryall: [1, 3, 4],
         dbquerysinglerow: 4,
         dbquerysinglerowdict: 4,
         dbquerysinglevalu: 4,
         dbserv: 3,
         dbtableid: 4,
-        de: 1,
+        de: [],
         def: [1, 3],
         default_extension: 3,
+        defaultauftragsart: 3,
         definition: [2, 4],
         defintion: 4,
         delet: 4,
         demo: 3,
         demonstration: 3,
         demonstri: 3,
         demonstriert: 1,
@@ -783,15 +815,15 @@
         erstell: [1, 2, 3, 4],
         erstellt: 4,
         erweit: 2,
         erweiter: 1,
         erweiternd: 4,
         erweitert: 4,
         erzeug: [1, 2, 3, 4],
-        erzeugt: [0, 1, 4],
+        erzeugt: [0, 1, 3, 4],
         et: 4,
         etre: 4,
         eulaend: 1,
         event: 3,
         evtl: [0, 1, 2, 4],
         exampl: 3,
         excel: [0, 1, 2, 3, 4],
@@ -822,35 +854,38 @@
         feldnam: 4,
         fest: 4,
         field1: 4,
         field2: 4,
         field: [3, 4],
         fieldsnotcopied: 4,
         fieldstocopyfortablecach: 4,
-        fil: [1, 3],
+        fil: 3,
         file_typ: 3,
         filedescriptororpath: 4,
         filenam: 4,
         filesaveas: 3,
         filt: 3,
         find: [0, 3],
         findet: 0,
+        firm: 3,
+        firmaautomat: 3,
         fix: 4,
         flag: 4,
         flexibl: 1,
         fn: [3, 4],
         folgend: 1,
         forc: 4,
         form: 4,
         format: [1, 3],
         formatdatetimeforapplus: 4,
         formatier: 4,
         formatiert: 4,
         formatsqlvalu: 4,
         formatsqlvaluestring: 4,
+        found: [],
         fram: 4,
         from: [1, 3],
         fugt: 4,
         fuhrt: 4,
         funktion: 4,
         funktioniert: [1, 4],
         fur: [0, 1, 2, 3, 4],
@@ -882,48 +917,53 @@
         geschickt: 4,
         geschrieb: [0, 1, 3],
         gesetzt: [1, 2, 4],
         gespeichert: [2, 3, 4],
         gestellt: 4,
         gesucht: 4,
         get: 3,
-        getboolean: 4,
+        getboolean: [3, 4],
         getclient: [1, 4],
         getcompletesql: 4,
         getcondition: 4,
         getconnectionstring: 4,
-        getcurrentdat: 4,
-        getcurrentdatetim: 4,
-        getcurrenttim: 4,
+        getcurrentdat: [3, 4],
+        getcurrentdatetim: [3, 4],
+        getcurrenttim: [3, 4],
         getdoubl: 4,
         getduplicat: 4,
         getfield: 4,
         getfieldstocopyfortabl: 4,
-        getint: 4,
+        getinstallpath: 3,
+        getinstallpathappserv: 3,
+        getinstallpathwebserv: [1, 3],
+        getint: [3, 4],
         getjoin: 4,
-        getlist: [1, 4],
+        getlist: [1, 3, 4],
         getlogg: 3,
-        getloginnam: 4,
+        getloginnam: [3, 4],
         getmandant: [3, 4],
-        getmandantnam: 4,
+        getmandantnam: [3, 4],
         getrennt: 4,
+        getserverinfo: 3,
         getsql: 4,
-        getstring: [1, 4],
+        getstring: [1, 3, 4],
         getsystemnam: [3, 4],
         gettabl: 4,
         gettablefield: 4,
         getuniquefieldsoftabl: 4,
-        getuserfullnam: 4,
-        getusernam: 4,
+        getuserfullnam: [3, 4],
+        getusernam: [3, 4],
         getxmldefinition: 4,
         getxmldefinitionobj: 4,
         getxmldefinitionstring: 4,
         geworf: 4,
         gibt: 4,
         gleich: [1, 4],
+        governed: [],
         greif: 3,
         group: [1, 3],
         groupby: 4,
         gruppiert: 4,
         gui: 3,
         guid: 4,
         gut: [1, 3],
@@ -947,14 +987,15 @@
         hinzu: [1, 4],
         hinzufug: [1, 3],
         hinzugefugt: [1, 4],
         hinzukomm: 2,
         hochkomma: 4,
         html: 0,
         http: 3,
+        https: [],
         hyperlink: 4,
         id: [1, 3, 4],
         id_a: 4,
         ids: 4,
         ignor: 3,
         imm: [3, 4],
         implementier: 1,
@@ -973,14 +1014,17 @@
         inputtext: 3,
         insbesond: 3,
         insdat: 4,
         insert: [3, 4],
         inspiziert: 4,
         install: 0,
         installiert: [0, 1],
+        installpath: 3,
+        installpathappserv: 3,
+        installpathwebserv: 3,
         insus: 4,
         interaktion: 2,
         interessant: [1, 4],
         interfac: 4,
         io: 4,
         irgendwi: 3,
         is: [1, 3, 4],
@@ -991,30 +1035,30 @@
         jahr: [3, 4],
         jasp: 1,
         je: [3, 4],
         jed: [3, 4],
         jedoch: [1, 4],
         job: 1,
         join: 4,
-        joinpath: 3,
+        joinpath: [1, 3],
         jointyp: 4,
         kalend: 3,
         key: 3,
         klass: 4,
         knot: 4,
         komfortabl: 4,
         kommt: 1,
         kompliziert: [1, 3],
         konfig: 3,
         konfigdatei: [1, 3],
         konfiguriert: 4,
         konkret: [1, 2],
         konn: [0, 1, 2, 3, 4],
         konnt: [3, 4],
-        kontakt: 1,
+        kontakt: [],
         konverti: [1, 3],
         konvertiert: 4,
         kopi: [2, 4],
         kopier: [2, 4],
         kopiert: [2, 4],
         korrekt: 1,
         kurz: 1,
@@ -1035,14 +1079,15 @@
         leid: 2,
         len: 3,
         lesend: [1, 3],
         letzt: 3,
         level: [3, 4],
         librari: 2,
         library: 0,
+        licens: [],
         liefert: 4,
         lieg: 1,
         liegt: 4,
         link: [3, 4],
         list: 4,
         listenelement: 4,
         load: 3,
@@ -1050,14 +1095,16 @@
         loaddbduplicateartikel: [3, 4],
         loaddbduplicatebusinessobject: 4,
         loaddbduplicatebusinessobjectsimplecond: 4,
         loaddbduplicatebusinessobjectssimplecond: 4,
         loaddbduplicatestueli: 4,
         logg: 3,
         logging: 3,
+        loginnam: 3,
+        lookups: 3,
         losch: [1, 2, 4],
         loschend: 4,
         lxml: 4,
         m: [0, 3],
         main: [1, 3],
         mak: 0,
         makelink: 4,
@@ -1066,14 +1113,15 @@
         makeweblink: 4,
         makeweblinkbauftrag: [3, 4],
         makeweblinkwauftrag: [3, 4],
         makeweblinkwauftragpos: [3, 4],
         manag: 3,
         mandant: [1, 2, 3, 4],
         mandanteninformation: 4,
+        mandantnam: 3,
         maschin: 1,
         maskiert: 4,
         material: [1, 3],
         materiali: [1, 3],
         maximal: 4,
         md5: 4,
         mehr: 4,
@@ -1094,14 +1142,15 @@
         moglich: [1, 2, 4],
         monat: [3, 4],
         month: [3, 4],
         ms: [0, 1],
         my: [1, 3],
         myland: 1,
         myout: [1, 3],
+        n: 3,
         nachd: 4,
         nachschlag: 4,
         nachtrag: 4,
         nam: [3, 4],
         nativ: 0,
         negation: 4,
         negier: 4,
@@ -1117,14 +1166,17 @@
         normalisedbfield: 4,
         normalisedbfieldlist: 4,
         normalisedbfieldset: 4,
         normalisiert: 4,
         not: [1, 3],
         notig: [1, 4],
         now: 3,
+        nr: 3,
+        nscripttool: 3,
+        nsysconf: 3,
         numm: [2, 3, 4],
         nutz: 1,
         nutzlich: 2,
         nutzt: 1,
         nutzung: [2, 4],
         nyear: 3,
         o: 0,
@@ -1132,24 +1184,26 @@
         ober: 4,
         oberflach: 2,
         obig: 1,
         obj: 4,
         object: [2, 4],
         objekt: [2, 4],
         odbc: [0, 4],
-        of: [1, 4],
+        of: 4,
         oft: [1, 4],
         ohn: [1, 4],
         on: 4,
         onlycopied: 4,
         op: 4,
+        opensourc: [],
         operation: [1, 4],
-        optional: [1, 4],
+        optional: [1, 3, 4],
         or: [3, 4],
         ord: [1, 3, 4],
+        org: [],
         original: 4,
         originalspalt: 4,
         outfil: [1, 3],
         p2applus64: 1,
         p2cor: 4,
         p2syst: 1,
         p: [3, 4],
@@ -1160,15 +1214,15 @@
         pandas: [1, 2, 3],
         pandasreadsql: [1, 3, 4],
         paramet: [3, 4],
         parent: 4,
         pars: 3,
         parsedat: 3,
         parst: 4,
-        part: 1,
+        part: [],
         passend: [0, 4],
         password: [3, 4],
         passwort: 3,
         path: [1, 3, 4],
         pathlib: [1, 3, 4],
         pathlik: 4,
         pd: [3, 4],
@@ -1189,15 +1243,14 @@
         prod: [2, 3],
         project: 3,
         properti: 4,
         pruf: 4,
         pruft: 4,
         punkt: 4,
         pyapplus64: [0, 1, 2, 3],
-        pyapplus: 2,
         pyear: 3,
         pyodbc: 4,
         pysimplegui: 3,
         python: [0, 1, 2, 3],
         query: 4,
         r: 3,
         raw: 4,
@@ -1238,28 +1291,30 @@
         schnittstell: [1, 2, 4],
         schon: [1, 4],
         schreib: 3,
         schreibarbeit: 4,
         schreibend: [1, 2, 3],
         schreibt: 4,
         script: [1, 3],
-        scripttool: [3, 4],
+        scripttool: [1, 3, 4],
+        see: [],
         selb: 4,
         select: [1, 3, 4],
         selektiert: 4,
         selt: 1,
-        sep: 4,
+        sep: [3, 4],
         sequenc: 4,
         seri: 4,
         serv: [0, 1, 2, 3, 4],
         server_conn: [1, 4],
         server_setting: 4,
         serverconfyamldeploy: 3,
         serverconfyamlprod: 3,
         serverconfyamlt: [1, 3],
+        serverinfo: 3,
         servic: [1, 4],
         set: 4,
         setfield: [3, 4],
         setlevel: 3,
         setting: 4,
         settop: 4,
         setzend: 4,
@@ -1274,15 +1329,15 @@
         siz: 3,
         soap: [0, 1, 2],
         sogar: 1,
         solch: [1, 3, 4],
         sollen: [1, 3, 4],
         sollt: [0, 2, 4],
         som: 3,
-        somedir: [1, 3],
+        somedir: [],
         somit: 1,
         sond: [3, 4],
         sortier: 4,
         sourc: 0,
         sowi: 4,
         spalt: [3, 4],
         spart: 2,
@@ -1337,63 +1392,66 @@
         sqlparam: 4,
         sqls: 4,
         sqlstatement: 4,
         sqlstatementselect: [1, 3, 4],
         sqltim: 4,
         sqlvalu: 4,
         src: 0,
-        stamm: 1,
+        stamm: [1, 3],
         standard: [1, 4],
         statement: [1, 2, 3, 4],
         statisch: 4,
         statt: 4,
         status: 3,
         steh: 3,
         stellt: 4,
         str: [1, 3, 4],
         string: 4,
         strptim: 3,
         struktur: 0,
         stucklist: [2, 3, 4],
         stueli: 4,
+        styl: [],
         sub: 4,
         such: 1,
         sucht: 1,
         sys: 1,
-        sysconf: [1, 2, 4],
+        sysconf: [1, 2, 3, 4],
         syst: [2, 3, 4],
         system: 2,
         systemnam: 3,
         t: [0, 4],
         tabell: [1, 3, 4],
         tabl: 4,
         tag: 4,
         target: 3,
         teil: 3,
         teilweis: [1, 3],
         test: 3,
         text: [3, 4],
-        thomas: 1,
+        that: [],
+        the: [],
+        thomas: [],
         tim: 4,
         timestamp: 4,
         timestamp_a: 4,
         today: 3,
         tool: [2, 4],
         top: 4,
         toprettyxml: 4,
         transaktion: 4,
         trat: 3,
         treib: 0,
         trivial: 1,
         ts: 4,
-        tuerk: 1,
+        tuerk: [],
         tupeln: 4,
         tupl: [3, 4],
         typ: [3, 4],
-        typing: 3,
+        typing: [1, 3],
         typisch: [4, 5],
         u: [2, 4],
         uber: [1, 2, 3, 4],
         ubergeb: [1, 4],
         ubernehm: 4,
         ubernomm: 4,
         uberschreib: 1,
@@ -1417,16 +1475,19 @@
         updat: [1, 3, 4],
         updatedb: [1, 3],
         updateorinsert: 4,
         upddat: [1, 3, 4],
         updnam: 3,
         updus: [1, 3, 4],
         ursprung: 1,
+        use: [],
         usecach: 4,
         user: [3, 4],
+        userfullnam: 3,
+        usernam: 3,
         usexml: [1, 2, 4],
         usexmlrow: 4,
         usexmlrowdelet: 4,
         usexmlrowinsert: 4,
         usexmlrowinsertorupdat: 4,
         usexmlrowupdat: 4,
         v1: 4,
@@ -1438,19 +1499,21 @@
         verallgemeinert: 2,
         verarbeit: 1,
         verarbeitet: 1,
         verbind: [1, 3, 4],
         verbindet: 4,
         verbund: 4,
         verfug: [3, 4],
+        vergeb: 3,
         vergleich: 4,
         vergleichsoperator: 4,
         verglich: 4,
+        verschied: 3,
         verschlimmert: 1,
-        version: [2, 4],
+        version: [2, 3, 4],
         vervollstand: 4,
         vervollstandigt: 4,
         verwend: [3, 4],
         verwendet: [0, 1, 4],
         verwies: 1,
         verzeichnis: [0, 1, 3, 4],
         viele: [1, 4],
@@ -1467,33 +1530,36 @@
         wahl: 3,
         wartungsarbeit: 1,
         wauftrag: 3,
         wauftragpos: 3,
         web: [2, 3, 4],
         web_setting: 4,
         weboberflach: 4,
-        webserv: [1, 3],
+        webserv: 3,
         weit: [2, 4],
         welch: [1, 3, 4],
         werd: [0, 1, 2, 3, 4],
-        wert: [1, 4],
+        werkstattauftrag: 3,
+        werkstattauftragsposition: 3,
+        wert: [1, 3, 4],
         wher: [1, 3, 4],
         whil: 3,
         wied: [3, 4],
         wiederum: 4,
         win_closed: 3,
         window: 3,
         windows: 1,
         wirklich: [3, 4],
         wohl: 3,
         wortlich: 4,
         wrapp: [2, 4],
         writeexcelbuff: 4,
         wsdl: 4,
         wurd: [1, 2, 3, 4],
+        www: [],
         xlsx: [1, 3],
         xlsxwrit: 2,
         xml: [2, 4],
         xmldefinition: 4,
         xmlrow: 4,
         y: 3,
         yaml: [1, 3],
@@ -1565,14 +1631,15 @@
         modul: 4,
         packag: 4,
         pandas: [0, 4],
         py: 3,
         pyapplus64: [4, 5],
         pyodbc: 0,
         pyyaml: 0,
+        read_setting: 3,
         report: 1,
         sphinx: 0,
         sql_util: 4,
         sqlalchemy: 0,
         submodul: 4,
         tool: 1,
         typisch: 1,
```

### Comparing `PyAPplus64-1.0.0/docs/make.bat` & `PyAPplus64-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.0/docs/source/abhaengigkeiten.rst` & `PyAPplus64-1.0.1/docs/source/abhaengigkeiten.rst`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.0/docs/source/anwendungen.rst` & `PyAPplus64-1.0.1/docs/source/anwendungen.rst`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Artikeln (angezeigt als `Bild` in `ArtikelRec.aspx`), für die Datei, auf die
 verwiesen wird, nicht im Dateisystem existiert. Diese fehlenden Dateien werden
 ausgegeben und das Feld `DOCUMENTS` gelöscht. Das Löschen erfolgt dabei über 
 `useXML`, so dass die Felder `UPDDATE` und `UPDUSER` korrekt gesetzt werden.
 
 .. literalinclude:: ../../examples/check_dokumente.py
    :language: python
+   :lines: 9-
    :linenos:
 
 Man kann alle Python Bibliotheken nutzen. Als Erweiterung wäre es in obigem Script 
 zum Beispiel einfach möglich, alle BMP-Bilder zu suchen, nach PNG zu konvertieren 
 und den DB-Eintrag anzupassen.
 
 
@@ -37,14 +38,15 @@
 werden, bietet sich evtl. Python an. 
 
 Folgendes Script erzeugt zum Beispiel eine Excel-Tabelle, mit einer Übersicht,
 welche Materialen wie oft für Artikel benutzt werden:
 
 .. literalinclude:: ../../examples/adhoc_report.py
    :language: python
+   :lines: 9-
    :linenos:
 
 Dieses kurze Script nutzt Standard-Pandas Methoden zur Erzeugung der Excel-Datei. Allerdings
 sind diese Methoden in den Aufrufen von `pandasReadSql` und `exportToExcel` gekapselt,
 so dass der Aufruf sehr einfach ist. Zudem ist es sehr einfach, die Verbindung zur Datenbank
 und zum APP-Server mittels der YAML-Konfigdatei herzustellen. Bei diesem 
 Aufruf kann optional ein Nutzer und eine Umgebung übergeben werden, die die Standard-Werte aus 
@@ -52,15 +54,15 @@
 der für die Umgebung korrekte Mandant automatisch verwendet wird.
 
 
 
 Anbindung eigener Tools
 -----------------------
 
-Ursprünglich wurde `PyAPplus64` für die Anbindung einer APplus-Anpassung geschrieben. Dieses ist 
+Ursprünglich wurde `PyAPplus64` für die Anbindung einer APplus-Anpassung geschrieben. Diese Anpassung ist 
 als Windows-Service auf einem eigenen Rechner installiert und überwacht dort ein bestimmtes Verzeichnis.
 Bei Änderungen an Dateien in diesem Verzeichnis (Hinzufügen, Ändern, Löschen) werden die Dateien verarbeitet
 und die Ergebnisse an APplus gemeldet. Dafür werden DB-Operationen aber auch SOAP-Calls benutzt.
 Ebenso wird auf die SysConf zugegriffen.
 
 Viele solcher Anpassungen lassen sich gut und sinnvoll im App-Server einrichten und als Job regelmäßig aufrufen. 
 Im konkreten Fall wird jedoch für die Verarbeitung der Dateien viel Rechenzeit benötigt. Dies würde dadurch
```

### Comparing `PyAPplus64-1.0.0/docs/source/conf.py` & `PyAPplus64-1.0.1/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'PyAPplus64'
 copyright = '2023, Thomas Tuerk'
 author = 'Thomas Tuerk'
+version = '1.0.1'
+release = '1.0.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
-    'sphinx.ext.autodoc',    
+    'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
 ]
 
 templates_path = ['_templates']
-exclude_patterns = [] # type: ignore
+exclude_patterns = []  # type: ignore
 
 language = 'de'
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'nature'
@@ -49,8 +51,8 @@
 
     # Additional stuff for the LaTeX preamble.
     # 'preamble': PREAMBLE
 }
 
 autodoc_type_aliases = {
     'SqlValue': 'SqlValue'
-}
+}
```

### Comparing `PyAPplus64-1.0.0/docs/source/examples.rst` & `PyAPplus64-1.0.1/docs/source/examples.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,42 +9,53 @@
 Viele Scripte teilen sich Einstellungen. Beispielsweise greifen fast alle Scripte irgendwie auf APplus zu und benötigen Informationen,
 mit welchem APP-Server, welchem Web-Server und welcher Datenbank sie sich verbinden sollen. Solche Informationen, insbesondere die Passwörter, werden nicht in  
 jedem Script gespeichert, sondern nur in den Config-Dateien. Es bietet sich wohl meist an, 3 Konfigdateien zu erstellen, je eine für 
 das Deploy-, das Test- und das Prod-System. Ein Beispiel ist im Unterverzeichnis ``examples/applus-server.yaml`` zu finden.
 
 .. literalinclude:: ../../examples/applus-server.yaml
    :language: yaml
+   :lines: 9-
    :linenos:
    
 Damit nicht in jedem Script immer wieder neu die Konfig-Dateien ausgewählt werden müssen, werden die Konfigs für 
-das Prod-, Test- und Deploy-System in ``examples/applus_configs.py`` hinterlegt. Diese wird in allen Scripten importiert,
+das Prod-, Test- und Deploy-System in ``examples/applus_configs.py`` hinterlegt. Diese Datei wird in allen Scripten importiert,
 so dass das Config-Verzeichnis und die darin enthaltenen Configs einfach zur Verfügung stehen.
 
 .. literalinclude:: ../../examples/applus_configs.py
    :language: python
+   :lines: 9-
    :linenos:
 
    
+``read_settings.py``
+-----------------------
+Einfaches Beispiel für Auslesen der SysConf und bestimmter Einstellungen.
+
+.. literalinclude:: ../../examples/read_settings.py
+   :language: python
+   :lines: 9-
+   :linenos:
+
 ``check_dokumente.py``
 -----------------------
 Einfaches Beispiel für lesenden und schreibenden Zugriff auf APplus Datenbank.
 
 .. literalinclude:: ../../examples/check_dokumente.py
    :language: python
-   :lines: 6-
+   :lines: 9-
    :linenos:
 
 
 ``adhoc_report.py``
 -------------------
 Sehr einfaches Beispiel zur Erstellung einer Excel-Tabelle aus einer SQL-Abfrage.
 
 .. literalinclude:: ../../examples/adhoc_report.py
    :language: python
-   :lines: 7-
+   :lines: 9-
    :linenos:
 
 
 ``mengenabweichung.py``
 -----------------------
 Etwas komplizierteres Beispiel zur Erstellung einer Excel-Datei aus SQL-Abfragen.
 
@@ -56,18 +67,18 @@
 ``mengenabweichung_gui.py``
 ---------------------------
 Beispiel für eine sehr einfache GUI, die die Eingabe einfacher Parameter erlaubt.
 Die GUI wird um die Erzeugung von Excel-Dateien mit Mengenabweichungen gebaut.
 
 .. literalinclude:: ../../examples/mengenabweichung_gui.pyw
    :language: python
-   :lines: 7-
+   :lines: 9-
    :linenos:
 
 ``copy_artikel.py``
 -----------------------
 Beispiel, wie Artikel inklusive Arbeitsplan und Stückliste dupliziert werden kann.
 
 .. literalinclude:: ../../examples/copy_artikel.py
    :language: python
-   :lines: 21-
+   :lines: 22-
    :linenos:
```

### Comparing `PyAPplus64-1.0.0/examples/adhoc_report.py` & `PyAPplus64-1.0.1/examples/adhoc_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
 import PyAPplus64
 import applus_configs
 import pathlib
 
-def main(confFile : pathlib.Path, outfile : str) -> None:
-    server = PyAPplus64.applus.applusFromConfigFile(confFile) 
 
-    # Einfache SQL-Anfrage 
+def main(confFile: pathlib.Path, outfile: str) -> None:
+    server = PyAPplus64.applus.applusFromConfigFile(confFile)
+
+    # Einfache SQL-Anfrage
     sql1 = ("select Material, count(*) as Anzahl from ARTIKEL "
             "group by MATERIAL having MATERIAL is not null "
             "order by Anzahl desc")
     df1 = PyAPplus64.pandas.pandasReadSql(server, sql1)
 
     # Sql Select-Statements können auch über SqlStatementSelect zusammengebaut
     # werden. Die ist bei vielen, komplizierten Bedingungen teilweise hilfreich.
-    sql2 = PyAPplus64.SqlStatementSelect("ARTIKEL")        
+    sql2 = PyAPplus64.SqlStatementSelect("ARTIKEL")
     sql2.addFields("Material", "count(*) as Anzahl")
     sql2.addGroupBy("MATERIAL")
     sql2.having.addConditionFieldIsNotNull("MATERIAL")
     sql2.order = "Anzahl desc"
     df2 = PyAPplus64.pandas.pandasReadSql(server, sql2)
 
     # Ausgabe als Excel mit 2 Blättern
     PyAPplus64.pandas.exportToExcel(outfile, [(df1, "Materialien"), (df2, "Materialien 2")], addTable=True)
 
 
 if __name__ == "__main__":
-    main(applus_configs.serverConfYamlTest, "myout.xlsx")
+    main(applus_configs.serverConfYamlTest, "myout.xlsx")
```

### Comparing `PyAPplus64-1.0.0/examples/applus-server.yaml` & `PyAPplus64-1.0.1/examples/applus-server.yaml`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.0/examples/check_dokumente.py` & `PyAPplus64-1.0.1/examples/check_dokumente.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
 import pathlib
 import PyAPplus64
 import applus_configs
+from typing import Optional
 
-def main(confFile : pathlib.Path, docDir:str, updateDB:bool) -> None:
-  server = PyAPplus64.applus.applusFromConfigFile(confFile) 
 
-  sql = PyAPplus64.sql_utils.SqlStatementSelect("ARTIKEL");
-  sql.addFields("ID", "ARTIKEL", "DOCUMENTS");
-  sql.where.addConditionFieldStringNotEmpty("DOCUMENTS");
-
-  for row in server.dbQueryAll(sql):
-    doc = pathlib.Path(docDir + row.DOCUMENTS);
-    if not doc.exists():
-        print("Bild '{}' für Artikel '{}' nicht gefunden".format(doc, row.ARTIKEL))
-        
-        if updateDB:
-              upd = server.mkUseXMLRowUpdate("ARTIKEL", row.ID);
-              upd.addField("DOCUMENTS", None);
-              upd.update();
+def main(confFile: pathlib.Path, updateDB: bool, docDir: Optional[str] = None) -> None:
+    server = PyAPplus64.applus.applusFromConfigFile(confFile)
+
+    if docDir is None:
+        docDir = str(server.scripttool.getInstallPathWebServer().joinpath("DocLib"))
+
+    sql = PyAPplus64.sql_utils.SqlStatementSelect("ARTIKEL")
+    sql.addFields("ID", "ARTIKEL", "DOCUMENTS")
+    sql.where.addConditionFieldStringNotEmpty("DOCUMENTS")
+
+    for row in server.dbQueryAll(sql):
+        doc = pathlib.Path(docDir + row.DOCUMENTS)
+        if not doc.exists():
+            print("Bild '{}' für Artikel '{}' nicht gefunden".format(doc, row.ARTIKEL))
+
+            if updateDB:
+                upd = server.mkUseXMLRowUpdate("ARTIKEL", row.ID)
+                upd.addField("DOCUMENTS", None)
+                upd.update()
+
 
 if __name__ == "__main__":
-  main(applus_configs.serverConfYamlTest, "somedir\\WebServer\\DocLib", False)
+    main(applus_configs.serverConfYamlTest, False)
```

### Comparing `PyAPplus64-1.0.0/examples/copy_artikel.py` & `PyAPplus64-1.0.1/examples/copy_artikel.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,49 +11,49 @@
 # Dies ist sowohl in der gleichen DB als auch in anderen DBs möglich.
 # So kann z.B. ein einzelner Artikel aus Test in Prod kopiert werden.
 # Ebenso ist es möglich, die Daten in einer Datei zwischenzuspeichern und
 # später irgendwo anders einzuspielen.
 #
 # Dies ist für Administrationszwecke gedacht. Anwendungsbeispiel wäre,
 # dass ein Artikel mit langem Arbeitsplan und Stückliste im Test-System erstellt wird.
-# Viele der Positionen enthalten Nachauflöse-Scripte, die im Test-System 
+# Viele der Positionen enthalten Nachauflöse-Scripte, die im Test-System
 # getestet werden. Diese vielen Scripte per Hand zu kopieren ist aufwändig
 # und Fehleranfällig und kann mit solchen Admin-Scripten automatisiert werden.
 
 import pathlib
 import PyAPplus64
 import applus_configs
 import logging
-import yaml 
+import yaml
+from typing import Optional
 
 
-def main(confFile:pathlib.Path, artikel:str, artikelNeu:str|None=None) -> None:
+def main(confFile: pathlib.Path, artikel: str, artikelNeu: Optional[str] = None) -> None:
     # Server verbinden
-    server = PyAPplus64.applus.applusFromConfigFile(confFile) 
+    server = PyAPplus64.applus.applusFromConfigFile(confFile)
 
     # DuplicateBusinessObject für Artikel erstellen
-    dArt = PyAPplus64.duplicate.loadDBDuplicateArtikel(server, artikel);
+    dArt = PyAPplus64.duplicate.loadDBDuplicateArtikel(server, artikel)
 
     # DuplicateBusinessObject zur Demonstration in YAML konvertieren und zurück
-    dArtYaml = yaml.dump(dArt);
-    print(dArtYaml);
+    dArtYaml = yaml.dump(dArt)
+    print(dArtYaml)
     dArt2 = yaml.load(dArtYaml, Loader=yaml.UnsafeLoader)
 
     # Neue Artikel-Nummer bestimmen und DuplicateBusinessObject in DB schreiben
     # Man könnte hier genauso gut einen anderen Server verwenden
     if (artikelNeu is None):
         artikelNeu = server.nextNumber("Artikel")
 
     if not (dArt is None):
-        dArt.setFields({"artikel" : artikelNeu})
-        res = dArt.insert(server);
-        print(res);
+        dArt.setFields({"artikel": artikelNeu})
+        res = dArt.insert(server)
+        print(res)
 
 
 if __name__ == "__main__":
     # Logger Einrichten
-    logging.basicConfig(level=logging.INFO) 
+    logging.basicConfig(level=logging.INFO)
     # logger = logging.getLogger("PyAPplus64.applus_db");
     # logger.setLevel(logging.ERROR)
 
     main(applus_configs.serverConfYamlTest, "my-artikel", artikelNeu="my-artikel-copy")
-
```

### Comparing `PyAPplus64-1.0.0/examples/mengenabweichung.py` & `PyAPplus64-1.0.1/examples/mengenabweichung.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,176 +7,191 @@
 # https://opensource.org/licenses/MIT.
 
 # Erzeugt Excel-Tabellen mit Werkstattaufträgen und Werkstattauftragspositionen mit Mengenabweichungen
 
 import datetime
 import PyAPplus64
 import applus_configs
-import pandas as pd # type: ignore
+import pandas as pd  # type: ignore
 import pathlib
-from typing import *
+from typing import Tuple, Union, Optional
+
 
 def ladeAlleWerkstattauftragMengenabweichungen(
-        server:PyAPplus64.APplusServer, 
-        cond:PyAPplus64.SqlCondition|str|None=None) -> pd.DataFrame:
-    sql = PyAPplus64.sql_utils.SqlStatementSelect("WAUFTRAG w");
+        server: PyAPplus64.APplusServer,
+        cond: Union[PyAPplus64.SqlCondition, str, None] = None) -> pd.DataFrame:
+    sql = PyAPplus64.sql_utils.SqlStatementSelect("WAUFTRAG w")
     sql.addLeftJoin("personal p", "w.UPDUSER = p.PERSONAL")
 
     sql.addFieldsTable("w", "ID", "BAUFTRAG", "POSITION")
     sql.addFields("(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG")
-    sql.addFieldsTable("w", "MENGE", "MENGE_IST", 
+    sql.addFieldsTable("w", "MENGE", "MENGE_IST",
                        "APLAN as ARTIKEL", "NAME as ARTIKELNAME")
     sql.addFields("w.UPDDATE", "p.NAME as UPDNAME")
 
     sql.where.addConditionFieldGe("w.STATUS", 5)
-    sql.where.addCondition("abs(w.MENGE-w.MENGE_IST) > 0.001")    
+    sql.where.addCondition("abs(w.MENGE-w.MENGE_IST) > 0.001")
     sql.where.addCondition(cond)
-    sql.order="w.UPDDATE"
-    dfOrg = PyAPplus64.pandas.pandasReadSql(server, sql);
+    sql.order = "w.UPDDATE"
+    dfOrg = PyAPplus64.pandas.pandasReadSql(server, sql)
 
     # Add Links
-    df = dfOrg.copy();
-    df = df.drop(columns=["ID"]);
+    df = dfOrg.copy()
+    df = df.drop(columns=["ID"])
     # df = df[['POSITION', 'BAUFTRAG', 'MENGE']] # reorder / filter columns
 
-    df['POSITION'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg, 
-                        lambda r: r.POSITION, 
+    df['POSITION'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+                        dfOrg,
+                        lambda r: r.POSITION,
                         lambda r: server.makeWebLinkWauftrag(
                             bauftrag=r.BAUFTRAG, accessid=r.ID))
-    df['BAUFTRAG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg, 
-                        lambda r: r.BAUFTRAG, 
+    df['BAUFTRAG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+                        dfOrg,
+                        lambda r: r.BAUFTRAG,
                         lambda r: server.makeWebLinkBauftrag(bauftrag=r.BAUFTRAG))
 
     colNames = {
-        "BAUFTRAG" : "Betriebsauftrag",
-        "POSITION" : "Pos",
-        "MENGENABWEICHUNG" : "Mengenabweichung",
-        "MENGE" : "Menge",
-        "MENGE_IST" : "Menge-Ist",
-        "ARTIKEL" : "Artikel",
-        "ARTIKELNAME" : "Artikel-Name",
-        "UPDDATE" : "geändert am",
-        "UPDNAME" : "geändert von"
+        "BAUFTRAG": "Betriebsauftrag",
+        "POSITION": "Pos",
+        "MENGENABWEICHUNG": "Mengenabweichung",
+        "MENGE": "Menge",
+        "MENGE_IST": "Menge-Ist",
+        "ARTIKEL": "Artikel",
+        "ARTIKELNAME": "Artikel-Name",
+        "UPDDATE": "geändert am",
+        "UPDNAME": "geändert von"
     }
-    df.rename(columns=colNames, inplace=True);
+    df.rename(columns=colNames, inplace=True)
 
     return df
 
 
 def ladeAlleWerkstattauftragPosMengenabweichungen(
-        server : PyAPplus64.APplusServer, 
-        cond:PyAPplus64.SqlCondition|str|None=None) -> pd.DataFrame:
-    sql = PyAPplus64.sql_utils.SqlStatementSelect("WAUFTRAGPOS w");
+        server: PyAPplus64.APplusServer,
+        cond: Union[PyAPplus64.SqlCondition, str, None] = None) -> pd.DataFrame:
+    sql = PyAPplus64.sql_utils.SqlStatementSelect("WAUFTRAGPOS w")
     sql.addLeftJoin("personal p", "w.UPDUSER = p.PERSONAL")
 
     sql.addFieldsTable("w", "ID", "BAUFTRAG", "POSITION", "AG")
     sql.addFields("(w.MENGE-w.MENGE_IST) as MENGENABWEICHUNG")
     sql.addFieldsTable("w", "MENGE", "MENGE_IST", "APLAN as ARTIKEL")
     sql.addFields("w.UPDDATE", "p.NAME as UPDNAME")
 
     sql.where.addConditionFieldEq("w.STATUS", 4)
-    sql.where.addCondition("abs(w.MENGE-w.MENGE_IST) > 0.001")    
+    sql.where.addCondition("abs(w.MENGE-w.MENGE_IST) > 0.001")
     sql.where.addCondition(cond)
-    sql.order="w.UPDDATE"
+    sql.order = "w.UPDDATE"
 
-    dfOrg = PyAPplus64.pandas.pandasReadSql(server, sql);
+    dfOrg = PyAPplus64.pandas.pandasReadSql(server, sql)
 
     # Add Links
-    df = dfOrg.copy();
-    df = df.drop(columns=["ID"]);
-    df['POSITION'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg, 
-                        lambda r: r.POSITION, 
+    df = dfOrg.copy()
+    df = df.drop(columns=["ID"])
+    df['POSITION'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+                        dfOrg,
+                        lambda r: r.POSITION,
                         lambda r: server.makeWebLinkWauftrag(
                             bauftrag=r.BAUFTRAG, accessid=r.ID))
-    df['BAUFTRAG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg, 
-                        lambda r: r.BAUFTRAG, 
+    df['BAUFTRAG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+                        dfOrg,
+                        lambda r: r.BAUFTRAG,
                         lambda r: server.makeWebLinkBauftrag(bauftrag=r.BAUFTRAG))
-    df['AG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(dfOrg, 
-                        lambda r: r.AG, 
+    df['AG'] = PyAPplus64.pandas.mkHyperlinkDataframeColumn(
+                        dfOrg,
+                        lambda r: r.AG,
                         lambda r: server.makeWebLinkWauftragPos(
                             bauftrag=r.BAUFTRAG, position=r.POSITION, accessid=r.ID))
-    
+
     # Demo zum Hinzufügen einer berechneten Spalte
-    # df['BAUFPOSAG'] = PyAPplus64.pandas.mkDataframeColumn(dfOrg, 
+    # df['BAUFPOSAG'] = PyAPplus64.pandas.mkDataframeColumn(dfOrg,
     #                     lambda r: "{}.{} AG {}".format(r.BAUFTRAG, r.POSITION, r.AG))
 
     # Rename Columns
     colNames = {
-        "BAUFTRAG" : "Betriebsauftrag",
-        "POSITION" : "Pos",
-        "AG" : "AG",
-        "MENGENABWEICHUNG" : "Mengenabweichung",
-        "MENGE" : "Menge",
-        "MENGE_IST" : "Menge-Ist",
-        "ARTIKEL" : "Artikel",
-        "UPDDATE" : "geändert am",
-        "UPDNAME" : "geändert von"
+        "BAUFTRAG": "Betriebsauftrag",
+        "POSITION": "Pos",
+        "AG": "AG",
+        "MENGENABWEICHUNG": "Mengenabweichung",
+        "MENGE": "Menge",
+        "MENGE_IST": "Menge-Ist",
+        "ARTIKEL": "Artikel",
+        "UPDDATE": "geändert am",
+        "UPDNAME": "geändert von"
     }
-    df.rename(columns=colNames, inplace=True);
+    df.rename(columns=colNames, inplace=True)
     return df
 
-def computeInYearMonthCond(field : str, year:int|None=None, 
-                           month:int|None=None) -> PyAPplus64.SqlCondition | None:
-    if not (year is None): 
+
+def computeInYearMonthCond(field: str, year: Optional[int] = None,
+                           month: Optional[int] = None) -> Optional[PyAPplus64.SqlCondition]:
+    if not (year is None):
         if month is None:
             return PyAPplus64.sql_utils.SqlConditionDateTimeFieldInYear(field, year)
         else:
             return PyAPplus64.sql_utils.SqlConditionDateTimeFieldInMonth(field, year, month)
     else:
         return None
 
-def computeFileName(year:int|None=None, month:int|None=None) -> str:
-    if year is None: 
-        return 'mengenabweichungen-all.xlsx';
+
+def computeFileName(year: Optional[int] = None, month: Optional[int] = None) -> str:
+    if year is None:
+        return 'mengenabweichungen-all.xlsx'
     else:
         if month is None:
-            return 'mengenabweichungen-{:04d}.xlsx'.format(year);
+            return 'mengenabweichungen-{:04d}.xlsx'.format(year)
         else:
-            return 'mengenabweichungen-{:04d}-{:02d}.xlsx'.format(year, month);
+            return 'mengenabweichungen-{:04d}-{:02d}.xlsx'.format(year, month)
 
-def _exportInternal(server: PyAPplus64.APplusServer, fn:str, 
-                    cond:Union[PyAPplus64.SqlCondition, str, None]) -> int:
+
+def _exportInternal(server: PyAPplus64.APplusServer, fn: str,
+                    cond: Union[PyAPplus64.SqlCondition, str, None]) -> int:
     df1 = ladeAlleWerkstattauftragMengenabweichungen(server, cond)
     df2 = ladeAlleWerkstattauftragPosMengenabweichungen(server, cond)
-    print ("erzeuge " + fn);
+    print("erzeuge " + fn)
     PyAPplus64.pandas.exportToExcel(fn, [(df1, "WAuftrag"), (df2, "WAuftrag-Pos")], addTable=True)
     return len(df1.index) + len(df2.index)
 
-def exportVonBis(server: PyAPplus64.APplusServer, fn:str, 
-                 von:datetime.datetime|None, bis:datetime.datetime|None) -> int:
-  cond = PyAPplus64.sql_utils.SqlConditionDateTimeFieldInRange("w.UPDDATE", von, bis)
-  return _exportInternal(server, fn, cond)
-
-def exportYearMonth(server: PyAPplus64.APplusServer, 
-                    year:int|None=None, month:int|None=None) -> int:
-    cond=computeInYearMonthCond("w.UPDDATE", year=year, month=month)
+
+def exportVonBis(server: PyAPplus64.APplusServer, fn: str,
+                 von: Optional[datetime.datetime], bis: Optional[datetime.datetime]) -> int:
+    cond = PyAPplus64.sql_utils.SqlConditionDateTimeFieldInRange("w.UPDDATE", von, bis)
+    return _exportInternal(server, fn, cond)
+
+
+def exportYearMonth(server: PyAPplus64.APplusServer,
+                    year: Optional[int] = None, month: Optional[int] = None) -> int:
+    cond = computeInYearMonthCond("w.UPDDATE", year=year, month=month)
     fn = computeFileName(year=year, month=month)
     return _exportInternal(server, fn, cond)
 
-def computePreviousMonthYear(cyear : int, cmonth :int) -> Tuple[int, int]:
+
+def computePreviousMonthYear(cyear: int, cmonth: int) -> Tuple[int, int]:
     if cmonth == 1:
         return (cyear-1, 12)
     else:
-        return (cyear, cmonth-1);
+        return (cyear, cmonth-1)
 
-def computeNextMonthYear(cyear : int, cmonth :int) -> Tuple[int, int]:
+
+def computeNextMonthYear(cyear: int, cmonth: int) -> Tuple[int, int]:
     if cmonth == 12:
         return (cyear+1, 1)
     else:
-        return (cyear, cmonth+1);
+        return (cyear, cmonth+1)
+
+
+def main(confFile: Union[str, pathlib.Path], user: Optional[str] = None, env: Optional[str] = None) -> None:
+    server = PyAPplus64.applusFromConfigFile(confFile, user=user, env=env)
 
-def main(confFile : str|pathlib.Path, user:str|None=None, env:str|None=None) -> None:
-    server = PyAPplus64.applusFromConfigFile(confFile, user=user, env=env) 
-    
     now = datetime.date.today()
     (cmonth, cyear) = (now.month, now.year)
-    (pyear, pmonth) = computePreviousMonthYear(cyear, cmonth);
-    
-    # Ausgaben    
-    exportYearMonth(server, cyear, cmonth) # Aktueller Monat
-    exportYearMonth(server, pyear, pmonth) # Vorheriger Monat
+    (pyear, pmonth) = computePreviousMonthYear(cyear, cmonth)
+
+    # Ausgaben
+    exportYearMonth(server, cyear, cmonth)  # Aktueller Monat
+    exportYearMonth(server, pyear, pmonth)  # Vorheriger Monat
     # export(cyear) # aktuelles Jahr
     # export(cyear-1) # letztes Jahr
     # export() # alles
 
+
 if __name__ == "__main__":
     main(applus_configs.serverConfYamlTest)
```

### Comparing `PyAPplus64-1.0.0/pyproject.toml` & `PyAPplus64-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyAPplus64"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Thomas Tuerk", email="kontakt@thomas-tuerk.de" },
 ]
 description = "Verschiedene Hilfsmittel, um mit dem ERP System APplus zu interagieren. Dieses Packet wurde für APplus 6.4 entwickelt, funktioniert vermutlich aber auch mit anderen Versionen."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/__init__.py` & `PyAPplus64-1.0.1/src/PyAPplus64/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
     SqlStatement,
     SqlStatementSelect
 )
 
 try:
     from . import pandas
 except:
-    pass
+    pass
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/applus.py` & `PyAPplus64-1.0.1/src/PyAPplus64/applus.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,286 +2,282 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
-
 from . import applus_db
 from . import applus_server
 from . import applus_sysconf
 from . import applus_scripttool
 from . import applus_usexml
 from . import sql_utils
 import yaml
 import urllib.parse
 from zeep import Client
-import pyodbc # type: ignore
-from typing import *
+import pyodbc  # type: ignore
+from typing import TYPE_CHECKING, Optional, Any, Callable, Dict, Sequence, Set, List
 
 if TYPE_CHECKING:
     from _typeshed import FileDescriptorOrPath
 
 
-
 class APplusServer:
     """
     Verbindung zu einem APplus DB und App Server mit Hilfsfunktionen für den komfortablen Zugriff.
-    
+
     :param db_settings: die Einstellungen für die Verbindung mit der Datenbank
     :type db_settings: APplusDBSettings
     :param server_settings: die Einstellungen für die Verbindung mit dem APplus App Server
     :type server_settings: APplusAppServerSettings
     :param web_settings: die Einstellungen für die Verbindung mit dem APplus Web Server
     :type web_settings: APplusWebServerSettings
     """
-    def __init__(self, db_settings : applus_db.APplusDBSettings, server_settings : applus_server.APplusAppServerSettings, web_settings : applus_server.APplusWebServerSettings):
+    def __init__(self,
+                 db_settings: applus_db.APplusDBSettings,
+                 server_settings: applus_server.APplusAppServerSettings,
+                 web_settings: applus_server.APplusWebServerSettings):
 
-        self.db_settings : applus_db.APplusDBSettings = db_settings
+        self.db_settings: applus_db.APplusDBSettings = db_settings
         """Die Einstellungen für die Datenbankverbindung"""
 
-        self.web_settings : applus_server.APplusWebServerSettings = web_settings
+        self.web_settings: applus_server.APplusWebServerSettings = web_settings
         """Die Einstellungen für die Datenbankverbindung"""
 
-        self.db_conn = db_settings.connect()        
+        self.db_conn = db_settings.connect()
         """
         Eine pyodbc-Connection zur APplus DB. Diese muss genutzt werden, wenn mehrere Operationen in einer Transaktion
-        genutzt werden sollen. Ansonsten sind die Hilfsmethoden wie :meth:`APplusServer.dbQuery` zu bevorzugen. 
+        genutzt werden sollen. Ansonsten sind die Hilfsmethoden wie :meth:`APplusServer.dbQuery` zu bevorzugen.
         Diese Connection kann in Verbindung mit den Funktionen aus :mod:`PyAPplus64.applus_db` genutzt werden.
         """
 
-
-        self.server_conn :  applus_server.APplusServerConnection = applus_server.APplusServerConnection(server_settings);
+        self.server_conn: applus_server.APplusServerConnection = applus_server.APplusServerConnection(server_settings)
         """erlaubt den Zugriff auf den AppServer"""
-        
-        self.sysconf : applus_sysconf.APplusSysConf = applus_sysconf.APplusSysConf(self);
+
+        self.sysconf: applus_sysconf.APplusSysConf = applus_sysconf.APplusSysConf(self)
         """erlaubt den Zugriff auf die Sysconfig"""
 
-        self.scripttool : applus_scripttool.APplusScriptTool = applus_scripttool.APplusScriptTool(self);
+        self.scripttool: applus_scripttool.APplusScriptTool = applus_scripttool.APplusScriptTool(self)
         """erlaubt den einfachen Zugriff auf Funktionen des ScriptTools"""
 
-        self.client_table = self.server_conn.getClient("p2core","Table");
-        self.client_xml = self.server_conn.getClient("p2core","XML");
+        self.client_table = self.server_conn.getClient("p2core", "Table")
+        self.client_xml = self.server_conn.getClient("p2core", "XML")
         self.client_nummer = self.server_conn.getClient("p2system", "Nummer")
 
     def reconnectDB(self) -> None:
         try:
-            self.db_conn.close() 
+            self.db_conn.close()
         except:
             pass
         self.db_conn = self.db_settings.connect()
 
-    def completeSQL(self, sql : sql_utils.SqlStatement, raw:bool=False) -> str:
+    def completeSQL(self, sql: sql_utils.SqlStatement, raw: bool = False) -> str:
         """
         Vervollständigt das SQL-Statement. Es wird z.B. der Mandant hinzugefügt.
-            
+
         :param sql: das SQL Statement
         :type sql: sql_utils.SqlStatement
         :param raw: soll completeSQL ausgeführt werden? Falls True, wird die Eingabe zurückgeliefert
         :type raw: boolean
         :return: das vervollständigte SQL-Statement
         :rtype: str
         """
         if raw:
             return str(sql)
         else:
-            return self.client_table.service.getCompleteSQL(sql);
+            return self.client_table.service.getCompleteSQL(sql)
 
-    def dbQueryAll(self, sql : sql_utils.SqlStatement, *args:Any, raw:bool=False, 
-                   apply:Optional[Callable[[pyodbc.Row],Any]]=None) -> Any:
-        """Führt eine SQL Query aus und liefert alle Zeilen zurück. Das SQL wird zunächst 
+    def dbQueryAll(self, sql: sql_utils.SqlStatement, *args: Any, raw: bool = False,
+                   apply: Optional[Callable[[pyodbc.Row], Any]] = None) -> Any:
+        """Führt eine SQL Query aus und liefert alle Zeilen zurück. Das SQL wird zunächst
            vom Server angepasst, so dass z.B. Mandanteninformation hinzugefügt werden."""
-        sqlC = self.completeSQL(sql, raw=raw);
+        sqlC = self.completeSQL(sql, raw=raw)
         return applus_db.rawQueryAll(self.db_conn, sqlC, *args, apply=apply)
 
-    def dbQuerySingleValues(self, sql : sql_utils.SqlStatement, *args:Any, raw:bool=False) -> Sequence[Any]:
+    def dbQuerySingleValues(self, sql: sql_utils.SqlStatement, *args: Any, raw: bool = False) -> Sequence[Any]:
         """Führt eine SQL Query aus, die nur eine Spalte zurückliefern soll."""
         return self.dbQueryAll(sql, *args, raw=raw, apply=lambda r: r[0])
 
-    def dbQuery(self, sql : sql_utils.SqlStatement, f : Callable[[pyodbc.Row], None], *args : Any, raw:bool=False) -> None:
-        """Führt eine SQL Query aus und führt für jede Zeile die übergeben Funktion aus. 
+    def dbQuery(self, sql: sql_utils.SqlStatement, f: Callable[[pyodbc.Row], None], *args: Any, raw: bool = False) -> None:
+        """Führt eine SQL Query aus und führt für jede Zeile die übergeben Funktion aus.
            Das SQL wird zunächst vom Server angepasst, so dass z.B. Mandanteninformation hinzugefügt werden."""
-        sqlC = self.completeSQL(sql, raw=raw);
+        sqlC = self.completeSQL(sql, raw=raw)
         applus_db.rawQuery(self.db_conn, sqlC, f, *args)
 
-    def dbQuerySingleRow(self, sql:sql_utils.SqlStatement, *args:Any, raw:bool=False) -> Optional[pyodbc.Row]:
+    def dbQuerySingleRow(self, sql: sql_utils.SqlStatement, *args: Any, raw: bool = False) -> Optional[pyodbc.Row]:
         """Führt eine SQL Query aus, die maximal eine Zeile zurückliefern soll. Diese Zeile wird geliefert."""
-        sqlC = self.completeSQL(sql, raw=raw);
+        sqlC = self.completeSQL(sql, raw=raw)
         return applus_db.rawQuerySingleRow(self.db_conn, sqlC, *args)
 
-    def dbQuerySingleRowDict(self, sql:sql_utils.SqlStatement, *args:Any, raw:bool=False) -> Optional[Dict[str, Any]]:
-        """Führt eine SQL Query aus, die maximal eine Zeile zurückliefern soll. 
+    def dbQuerySingleRowDict(self, sql: sql_utils.SqlStatement, *args: Any, raw: bool = False) -> Optional[Dict[str, Any]]:
+        """Führt eine SQL Query aus, die maximal eine Zeile zurückliefern soll.
            Diese Zeile wird als Dictionary geliefert."""
-        row = self.dbQuerySingleRow(sql, *args, raw=raw);
+        row = self.dbQuerySingleRow(sql, *args, raw=raw)
         if row:
-            return applus_db.row_to_dict(row);
+            return applus_db.row_to_dict(row)
         else:
             return None
 
-    def dbQuerySingleValue(self, sql:sql_utils.SqlStatement, *args:Any, raw:bool=False) -> Any:
-        """Führt eine SQL Query aus, die maximal einen Wert zurückliefern soll. 
+    def dbQuerySingleValue(self, sql: sql_utils.SqlStatement, *args: Any, raw: bool = False) -> Any:
+        """Führt eine SQL Query aus, die maximal einen Wert zurückliefern soll.
            Dieser Wert oder None wird geliefert."""
-        sqlC = self.completeSQL(sql, raw=raw);
+        sqlC = self.completeSQL(sql, raw=raw)
         return applus_db.rawQuerySingleValue(self.db_conn, sqlC, *args)
 
-    def isDBTableKnown(self, table : str) -> bool:
+    def isDBTableKnown(self, table: str) -> bool:
         """Prüft, ob eine Tabelle im System bekannt ist"""
         sql = "select count(*) from SYS.TABLES T where T.NAME=?"
-        c = self.dbQuerySingleValue(sql, table);
+        c = self.dbQuerySingleValue(sql, table)
         return (c > 0)
 
-    def getClient(self, package : str, name : str) -> Client:
+    def getClient(self, package: str, name: str) -> Client:
         """Erzeugt einen zeep - Client.
            Mittels dieses Clients kann die WSDL Schnittstelle angesprochen werden.
-           Wird als *package* "p2core" und als *name* "Table" verwendet und der 
+           Wird als *package* "p2core" und als *name* "Table" verwendet und der
            resultierende client "client" genannt, dann kann
            z.B. mittels "client.service.getCompleteSQL(sql)" vom AppServer ein Vervollständigen
            des SQLs angefordert werden.
 
            :param package: das Packet, z.B. "p2core"
            :type package: str
            :param name: der Name im Packet, z.B. "Table"
            :type package: string
            :return: den Client
            :rtype: Client
            """
-        return self.server_conn.getClient(package, name);
+        return self.server_conn.getClient(package, name)
 
-    def getTableFields(self, table:str, isComputed:Optional[bool]=None) -> Set[str]:
+    def getTableFields(self, table: str, isComputed: Optional[bool] = None) -> Set[str]:
         """
         Liefert die Namen aller Felder einer Tabelle.
 
         :param table: Name der Tabelle
         :param isComputed: wenn gesetzt, werden nur die Felder geliefert, die berechnet werden oder nicht berechnet werden
         :return: Liste aller Feld-Namen
         :rtype: {str}
         """
         sql = sql_utils.SqlStatementSelect("SYS.TABLES T")
-        join = sql.addInnerJoin("SYS.COLUMNS C");
+        join = sql.addInnerJoin("SYS.COLUMNS C")
         join.on.addConditionFieldsEq("T.Object_ID", "C.Object_ID")
-        if not (isComputed == None):
-            join.on.addConditionFieldEq("c.is_computed", isComputed)        
+        if not (isComputed is None):
+            join.on.addConditionFieldEq("c.is_computed", isComputed)
         sql.addFields("C.NAME")
 
         sql.where.addConditionFieldEq("t.name", sql_utils.SqlParam())
-        return sql_utils.normaliseDBfieldSet(self.dbQueryAll(sql, table, apply=lambda r : r.NAME));
+        return sql_utils.normaliseDBfieldSet(self.dbQueryAll(sql, table, apply=lambda r: r.NAME))
 
-    def getUniqueFieldsOfTable(self, table : str) -> Dict[str, List[str]]:     
+    def getUniqueFieldsOfTable(self, table: str) -> Dict[str, List[str]]:
         """
-        Liefert alle Spalten einer Tabelle, die eindeutig sein müssen. 
-        Diese werden als Dictionary gruppiert nach Index-Namen geliefert. 
-        Jeder Eintrag enthält eine Liste von Feldern, die zusammen eindeutig sein 
+        Liefert alle Spalten einer Tabelle, die eindeutig sein müssen.
+        Diese werden als Dictionary gruppiert nach Index-Namen geliefert.
+        Jeder Eintrag enthält eine Liste von Feldern, die zusammen eindeutig sein
         müssen.
         """
         return applus_db.getUniqueFieldsOfTable(self.db_conn, table)
 
+    def useXML(self, xml: str) -> Any:
+        """Ruft ``p2core.xml.usexml`` auf. Wird meist durch ein ``UseXMLRow-Objekt`` aufgerufen."""
+        return self.client_xml.service.useXML(xml)
 
-    def useXML(self, xml : str) -> Any:
-        """Ruft ``p2core.xml.usexml`` auf. Wird meist durch ein ``UseXMLRow-Objekt`` aufgerufen."""        
-        return self.client_xml.service.useXML(xml);
-
-
-    def mkUseXMLRowInsert(self, table : str) -> applus_usexml.UseXmlRowInsert:
+    def mkUseXMLRowInsert(self, table: str) -> applus_usexml.UseXmlRowInsert:
         """
         Erzeugt ein Objekt zum Einfügen eines neuen DB-Eintrags.
-        
+
         :param table: DB-Tabelle in die eingefügt werden soll
         :type table: str
         :return: das XmlRow-Objekt
         :rtype: applus_usexml.UseXmlRowInsert
         """
 
         return applus_usexml.UseXmlRowInsert(self, table)
 
-    def mkUseXMLRowUpdate(self, table : str, id : int) -> applus_usexml.UseXmlRowUpdate:
+    def mkUseXMLRowUpdate(self, table: str, id: int) -> applus_usexml.UseXmlRowUpdate:
         return applus_usexml.UseXmlRowUpdate(self, table, id)
 
-    def mkUseXMLRowInsertOrUpdate(self, table : str) -> applus_usexml.UseXmlRowInsertOrUpdate:
+    def mkUseXMLRowInsertOrUpdate(self, table: str) -> applus_usexml.UseXmlRowInsertOrUpdate:
         """
         Erzeugt ein Objekt zum Einfügen oder Updaten eines DB-Eintrags.
-        
+
         :param table: DB-Tabelle in die eingefügt werden soll
         :type table: string
         :return: das XmlRow-Objekt
         :rtype: applus_usexml.UseXmlRowInsertOrUpdate
         """
 
         return applus_usexml.UseXmlRowInsertOrUpdate(self, table)
 
+    def mkUseXMLRowDelete(self, table: str, id: int) -> applus_usexml.UseXmlRowDelete:
+        return applus_usexml.UseXmlRowDelete(self, table, id)
 
-    def mkUseXMLRowDelete(self, table:str, id:int) -> applus_usexml.UseXmlRowDelete :
-        return applus_usexml.UseXmlRowDelete(self, table, id)        
-
-    def execUseXMLRowDelete(self, table:str, id:int) -> None:
+    def execUseXMLRowDelete(self, table: str, id: int) -> None:
         delRow = self.mkUseXMLRowDelete(table, id)
-        delRow.delete();
+        delRow.delete()
 
-    def nextNumber(self, obj : str) -> str:
+    def nextNumber(self, obj: str) -> str:
         """
         Erstellt eine neue Nummer für das Objekt und legt diese Nummer zurück.
         """
         return self.client_nummer.service.nextNumber(obj)
 
-    def makeWebLink(self, base : str, **kwargs : Any) -> str :
+    def makeWebLink(self, base: str, **kwargs: Any) -> str:
         if not self.web_settings.baseurl:
-            raise Exception("keine Webserver-BaseURL gesetzt");
-        
-        url = str(self.web_settings.baseurl) + base;
+            raise Exception("keine Webserver-BaseURL gesetzt")
+
+        url = str(self.web_settings.baseurl) + base
         firstArg = True
         for arg, argv in kwargs.items():
-            if not (argv == None):
+            if not (argv is None):
                 if firstArg:
-                    firstArg = False;
+                    firstArg = False
                     url += "?"
                 else:
                     url += "&"
                 url += arg + "=" + urllib.parse.quote(str(argv))
-        return url;
+        return url
 
-    def makeWebLinkWauftragPos(self, **kwargs : Any) -> str:
-        return self.makeWebLink("wp/wauftragPosRec.aspx", **kwargs);
+    def makeWebLinkWauftragPos(self, **kwargs: Any) -> str:
+        return self.makeWebLink("wp/wauftragPosRec.aspx", **kwargs)
 
-    def makeWebLinkWauftrag(self, **kwargs : Any) -> str :
-        return self.makeWebLink("wp/wauftragRec.aspx", **kwargs);
+    def makeWebLinkWauftrag(self, **kwargs: Any) -> str:
+        return self.makeWebLink("wp/wauftragRec.aspx", **kwargs)
 
-    def makeWebLinkBauftrag(self, **kwargs : Any) -> str :
-        return self.makeWebLink("wp/bauftragRec.aspx", **kwargs);
+    def makeWebLinkBauftrag(self, **kwargs: Any) -> str:
+        return self.makeWebLink("wp/bauftragRec.aspx", **kwargs)
 
 
-
-def applusFromConfigDict(yamlDict:Dict[str, Any], user:Optional[str]=None, env:Optional[str]=None) -> APplusServer:
+def applusFromConfigDict(yamlDict: Dict[str, Any], user: Optional[str] = None, env: Optional[str] = None) -> APplusServer:
     """Läd Einstellungen aus einer Config und erzeugt daraus ein APplus-Objekt"""
-    if user is None or user=='':
-        user = yamlDict["appserver"]["user"]        
-    if env is None or env=='':
-        env = yamlDict["appserver"]["env"]        
+    if user is None or user == '':
+        user = yamlDict["appserver"]["user"]
+    if env is None or env == '':
+        env = yamlDict["appserver"]["env"]
     app_server = applus_server.APplusAppServerSettings(
-        appserver=yamlDict["appserver"]["server"], 
-        appserverPort=yamlDict["appserver"]["port"], 
-        user=user, # type: ignore
+        appserver=yamlDict["appserver"]["server"],
+        appserverPort=yamlDict["appserver"]["port"],
+        user=user,  # type: ignore
         env=env)
     web_server = applus_server.APplusWebServerSettings(
         baseurl=yamlDict.get("webserver", {}).get("baseurl", None)
     )
     dbparams = applus_db.APplusDBSettings(
-        server=yamlDict["dbserver"]["server"], 
+        server=yamlDict["dbserver"]["server"],
         database=yamlDict["dbserver"]["db"],
-        user=yamlDict["dbserver"]["user"], 
-        password=yamlDict["dbserver"]["password"]);
-    return APplusServer(dbparams, app_server, web_server);
+        user=yamlDict["dbserver"]["user"],
+        password=yamlDict["dbserver"]["password"])
+    return APplusServer(dbparams, app_server, web_server)
+
 
-def applusFromConfigFile(yamlfile : 'FileDescriptorOrPath', 
-                         user:Optional[str]=None, env:Optional[str]=None) -> APplusServer:
+def applusFromConfigFile(yamlfile: 'FileDescriptorOrPath',
+                         user: Optional[str] = None, env: Optional[str] = None) -> APplusServer:
     """Läd Einstellungen aus einer Config-Datei und erzeugt daraus ein APplus-Objekt"""
     yamlDict = {}
     with open(yamlfile, "r") as stream:
         yamlDict = yaml.safe_load(stream)
 
     return applusFromConfigDict(yamlDict, user=user, env=env)
 
-def applusFromConfig(yamlString : str, user:Optional[str]=None, env:Optional[str]=None) -> APplusServer:
+
+def applusFromConfig(yamlString: str, user: Optional[str] = None, env: Optional[str] = None) -> APplusServer:
     """Läd Einstellungen aus einer Config-Datei und erzeugt daraus ein APplus-Objekt"""
     yamlDict = yaml.safe_load(yamlString)
     return applusFromConfigDict(yamlDict, user=user, env=env)
-
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/applus_db.py` & `PyAPplus64-1.0.1/src/PyAPplus64/applus_db.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,170 +2,171 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
-
-import pyodbc # type: ignore
+import pyodbc  # type: ignore
 import logging
 from .sql_utils import SqlStatement
 from . import sql_utils
-from typing import *
+from typing import List, Dict, Set, Any, Optional, Callable, Sequence
+
 
+logger = logging.getLogger(__name__)
 
-logger = logging.getLogger(__name__);
 
 class APplusDBSettings:
     """
     Einstellungen, mit welcher DB sich verbunden werden soll.
     """
-    
-    def __init__(self, server : str, database : str, user : str, password : str):
+
+    def __init__(self, server: str, database: str, user: str, password: str):
         self.server = server
-        self.database = database;
+        self.database = database
         self.user = user
         self.password = password
 
-
     def getConnectionString(self) -> str:
         """Liefert den ODBC Connection-String für die Verbindung.
         :return: den Connection-String
         """
         return ("Driver={SQL Server Native Client 11.0};"
                 "Server="+self.server+";"
                 "Database="+self.database+";"
                 "UID="+self.user+";"
-                "PWD="+self.password + ";")    
+                "PWD="+self.password + ";")
 
     def connect(self) -> pyodbc.Connection:
         """Stellt eine neue Verbindung her und liefert diese zurück.
         """
         return pyodbc.connect(self.getConnectionString())
 
 
-
-def row_to_dict(row : pyodbc.Row) -> Dict[str, Any]:
+def row_to_dict(row: pyodbc.Row) -> Dict[str, Any]:
     """Konvertiert eine Zeile in ein Dictionary"""
     return dict(zip([t[0] for t in row.cursor_description], row))
 
-def _logSQLWithArgs(sql : SqlStatement, *args : Any) -> None:
+
+def _logSQLWithArgs(sql: SqlStatement, *args: Any) -> None:
     if args:
         logger.debug("executing '{}' with args {}".format(str(sql), str(args)))
     else:
         logger.debug("executing '{}'".format(str(sql)))
 
+
 def rawQueryAll(
-        cnxn : pyodbc.Connection,
-        sql : SqlStatement, 
-        *args : Any, 
-        apply : Optional[Callable[[pyodbc.Row], Any]]=None) -> Sequence[Any]:
+        cnxn: pyodbc.Connection,
+        sql: SqlStatement,
+        *args: Any,
+        apply: Optional[Callable[[pyodbc.Row], Any]] = None) -> Sequence[Any]:
     """
     Führt eine SQL Query direkt aus und liefert alle Zeilen zurück.
     Wenn apply gesetzt ist, wird die Funktion auf jeder Zeile ausgeführt und das Ergebnis ausgeben, die nicht None sind.
     """
     _logSQLWithArgs(sql, *args)
     with cnxn.cursor() as cursor:
         cursor.execute(str(sql), *args)
 
-        rows = cursor.fetchall();
+        rows = cursor.fetchall()
         if apply is None:
             return rows
         else:
             res = []
             for r in rows:
                 rr = apply(r)
-                if not (rr == None):
+                if not (rr is None):
                     res.append(rr)
             return res
 
-def rawQuery(cnxn : pyodbc.Connection, sql : sql_utils.SqlStatement, f : Callable[[pyodbc.Row], None], *args : Any) -> None:
+
+def rawQuery(cnxn: pyodbc.Connection, sql: sql_utils.SqlStatement, f: Callable[[pyodbc.Row], None], *args: Any) -> None:
     """Führt eine SQL Query direkt aus und führt für jede Zeile die übergeben Funktion aus."""
     _logSQLWithArgs(sql, *args)
     with cnxn.cursor() as cursor:
         cursor.execute(str(sql), *args)
         for row in cursor:
-            f(row);
+            f(row)
 
-def rawQuerySingleRow(cnxn : pyodbc.Connection, sql : SqlStatement, *args : Any) -> Optional[pyodbc.Row]:
+
+def rawQuerySingleRow(cnxn: pyodbc.Connection, sql: SqlStatement, *args: Any) -> Optional[pyodbc.Row]:
     """Führt eine SQL Query direkt aus, die maximal eine Zeile zurückliefern soll. Diese Zeile wird geliefert."""
     _logSQLWithArgs(sql, *args)
     with cnxn.cursor() as cursor:
         cursor.execute(str(sql), *args)
-        return cursor.fetchone();
+        return cursor.fetchone()
+
 
-def rawQuerySingleValue(cnxn : pyodbc.Connection, sql : SqlStatement, *args : Any) -> Any:
+def rawQuerySingleValue(cnxn: pyodbc.Connection, sql: SqlStatement, *args: Any) -> Any:
     """Führt eine SQL Query direkt aus, die maximal einen Wert zurückliefern soll. Dieser Wert oder None wird geliefert."""
     _logSQLWithArgs(sql, *args)
     with cnxn.cursor() as cursor:
         cursor.execute(str(sql), *args)
-        row = cursor.fetchone();
+        row = cursor.fetchone()
         if row:
-            return row[0];
+            return row[0]
         else:
-            return None;
+            return None
 
-def getUniqueFieldsOfTable(cnxn : pyodbc.Connection, table : str) -> Dict[str, List[str]] :     
+
+def getUniqueFieldsOfTable(cnxn: pyodbc.Connection, table: str) -> Dict[str, List[str]]:
     """
-    Liefert alle Spalten einer Tabelle, die eindeutig sein müssen. 
-    Diese werden als Dictionary gruppiert nach Index-Namen geliefert. 
-    Jeder Eintrag enthält eine Liste von Feldern, die zusammen eindeutig sein 
+    Liefert alle Spalten einer Tabelle, die eindeutig sein müssen.
+    Diese werden als Dictionary gruppiert nach Index-Namen geliefert.
+    Jeder Eintrag enthält eine Liste von Feldern, die zusammen eindeutig sein
     müssen.
     """
 
     sql = sql_utils.SqlStatementSelect("sys.indexes AS i")
     join = sql.addInnerJoin("sys.index_columns AS ic")
     join.on.addCondition("i.OBJECT_ID = ic.OBJECT_ID")
     join.on.addCondition("i.index_id = ic.index_id")
     sql.where.addConditionFieldEq("OBJECT_NAME(ic.OBJECT_ID)", table)
     sql.where.addConditionFieldEq("i.is_unique", True)
     sql.addFields("i.name AS INDEX_NAME", "COL_NAME(ic.OBJECT_ID,ic.column_id) AS COL")
     _logSQLWithArgs(sql)
 
-    indices : Dict[str, List[str]] = {}
+    indices: Dict[str, List[str]] = {}
     with cnxn.cursor() as cursor:
         cursor.execute(str(sql))
         for row in cursor:
             cols = indices.get(row.INDEX_NAME, [])
             cols.append(sql_utils.normaliseDBfield(row.COL))
             indices[row.INDEX_NAME] = cols
     return indices
 
 
 class DBTableIDs():
     """Klasse, die Mengen von IDs gruppiert nach Tabellen speichert"""
-    
+
     def __init__(self) -> None:
-        self.data : Dict[str, Set[int]]= {}
+        self.data: Dict[str, Set[int]] = {}
 
-    def add(self, table:str, *ids : int) -> None:
+    def add(self, table: str, *ids: int) -> None:
         """
         fügt Eintrag hinzu
-        
+
         :param table: die Tabelle
         :type table: str
         :param id: die ID
         """
         table = table.upper()
         if not (table in self.data):
-            self.data[table] = set(ids);            
+            self.data[table] = set(ids)
         else:
             self.data[table].update(ids)
 
-    def getTable(self, table : str) -> Set[int]:
+    def getTable(self, table: str) -> Set[int]:
         """
         Liefert die Menge der IDs für eine bestimmte Tabelle.
 
         :param table: die Tabelle
         :type table: str
-        :return: die IDs        
+        :return: die IDs
         """
 
         table = table.upper()
         return self.data.get(table, set())
 
     def __str__(self) -> str:
         return str(self.data)
-
-
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/applus_scripttool.py` & `PyAPplus64-1.0.1/src/PyAPplus64/applus_scripttool.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,65 +2,65 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
-
 from .applus import APplusServer
 from . import sql_utils
-import lxml.etree as ET # type: ignore
-from typing import *
+import lxml.etree as ET  # type: ignore
+from typing import Optional, Tuple, Set
+import pathlib
+
 
 class XMLDefinition:
     """Repräsentation eines XML-Dokuments"""
 
-    def __init__(self, root : ET.Element) -> None:
-        self.root : ET.Element = root
+    def __init__(self, root: ET.Element) -> None:
+        self.root: ET.Element = root
         """das Root-Element, repräsentiert "object" aus Datei."""
 
     def __str__(self) -> str:
-        return ET.tostring(self.root, encoding = "unicode")
+        return ET.tostring(self.root, encoding="unicode")
 
     def getDuplicate(self) -> Tuple[Set[str], bool]:
         """
         Extrahiert alle Properties, die für Duplizieren konfiguriert sind.
         Zudem wird ein Flag geliefert, ob diese Properties ein oder ausgeschlossen werden sollen.
         :return: Tuple aus allen Properties und ob dies aus- (True) oder ein-(False) zuschließen sind.
         :rtype: Tuple[Set[str], bool]
         """
-        res : Set[str] = set()
-        excl = True;
+        res: Set[str] = set()
+        excl = True
         dupl = self.root.find("duplicate")
         if (dupl is None):
-            return (res, excl);
+            return (res, excl)
 
         exclS = dupl.get("type", default="exclude")
         excl = exclS.casefold() == "exclude"
 
         for e in dupl.findall("{ref}property"):
             v = e.get("ref")
             if not (v is None):
                 res.add(sql_utils.normaliseDBfield(str(v)))
-        
+
         return (res, excl)
 
 
 class APplusScriptTool:
     """
     Zugriff auf AppServer ScriptTool
 
     :param server: die Verbindung zum Server
     :type server: APplusServerConnection
 
     """
-    
-    def __init__(self, server : APplusServer) -> None:
+
+    def __init__(self, server: APplusServer) -> None:
         self.client = server.getClient("p2script", "ScriptTool")
 
     def getCurrentDate(self) -> str:
         return self.client.service.getCurrentDate()
 
     def getCurrentTime(self) -> str:
         return self.client.service.getCurrentTime()
@@ -72,77 +72,112 @@
         return self.client.service.getLoginName()
 
     def getUserName(self) -> str:
         return self.client.service.getUserName()
 
     def getUserFullName(self) -> str:
         return self.client.service.getUserFullName()
-        
+
     def getSystemName(self) -> str:
         return self.client.service.getSystemName()
 
-    def getXMLDefinitionString(self, obj:str, mandant:str="") -> str:
+    def getInstallPath(self) -> str:
+        """
+        Liefert den Installionspfad des Appservers
+        """
+        return self.client.service.getInstallPath()
+
+    def getInstallPathAppServer(self) -> pathlib.Path:
+        """
+        Liefert den Installionspfad des Appservers als PathLib-Path
+        """
+        return pathlib.Path(self.getInstallPath())
+
+    def getInstallPathWebServer(self) -> pathlib.Path:
+        """
+        Liefert den Installionspfad des Webservers als PathLib-Path
+        """
+        return self.getInstallPathAppServer().parents[0].joinpath("WebServer")
+
+    def getXMLDefinitionString(self, obj: str, mandant: str = "") -> str:
         """
         Läd die XML-Defintion als String vom APPServer. Auch wenn kein XML-Dokument im Dateisystem gefunden wird,
         wird ein String zurückgeliefert, der einen leeren Top-"Object" Knoten enthält. Für gefundene XML-Dokumente
-        gibt es zusätzlich einen Top-"MD5"-Knoten. 
-        
+        gibt es zusätzlich einen Top-"MD5"-Knoten.
+
         :param obj: das Objekt, dessen Definition zu laden ist, "Artikel" läd z.B. "ArtikelDefinition.xml"
         :type obj: str
         :param mandant: der Mandant, dessen XML-Doku geladen werden soll, wenn "" wird der Standard-Mandant verwendet
         :type mandant: str optional
         :return: das gefundene XML-Dokument als String
-        :rtype: str 
+        :rtype: str
         """
         return self.client.service.getXMLDefinition2(obj, "")
 
-    def getXMLDefinition(self, obj:str, mandant:str="", checkFileExists:bool=False) -> Optional[ET.Element]:
+    def getXMLDefinition(self, obj: str, mandant: str = "", checkFileExists: bool = False) -> Optional[ET.Element]:
         """
         Läd die XML-Definition als String vom APPServer. und parst das XML in ein minidom-Dokument.
-        
+
         :param obj: das Objekt, dessen Definition zu laden ist, "Artikel" läd z.B. "ArtikelDefinition.xml"
         :type obj: str
         :param mandant: der Mandant, dessen XML-Doku geladen werden soll, wenn "" wird der Standard-Mandant verwendet
         :type mandant: str optional
-        :return: das gefundene und mittels ElementTree geparste XML-Dokument
+        :return: das gefundene und geparste XML-Dokument
         :rtype: ET.Element
         """
         return ET.fromstring(self.getXMLDefinitionString(obj, mandant=mandant))
 
-    def getXMLDefinitionObj(self, obj:str, mandant:str="") -> Optional[XMLDefinition]:
+    def getXMLDefinitionObj(self, obj: str, mandant: str = "") -> Optional[XMLDefinition]:
         """
-        Benutzt getXMLDefinitionObj und liefert den Top-Level "Object" Knoten zurück, falls zusätzlich 
+        Benutzt getXMLDefinitionObj und liefert den Top-Level "Object" Knoten zurück, falls zusätzlich
         ein MD5 Knoten existiert, also falls das Dokument wirklich vom Dateisystem geladen werden konnte.
         Ansonten wird None geliefert.
 
         :param obj: das Objekt, dess Definition zu laden ist, "Artikel" läd z.B. "ArtikelDefinition.xml"
         :type obj: str
         :param mandant: der Mandant, dessen XML-Doku geladen werden soll, wenn "" wird der Standard-Mandant verwendet
         :type mandant: str optional
-        :return: das gefundene und mittels ElementTree geparste XML-Dokument
+        :return: das gefundene und geparste XML-Dokument
         :rtype: Optional[XMLDefinition]
         """
-        e = self.getXMLDefinition(obj, mandant=mandant);
+        e = self.getXMLDefinition(obj, mandant=mandant)
         if e is None:
             return None
 
         if e.find("md5") is None:
-            return None;
+            return None
 
         o = e.find("object")
         if o is None:
             return None
         else:
-            return XMLDefinition(o);
-
+            return XMLDefinition(o)
 
     def getMandant(self) -> str:
         """
         Liefert den aktuellen Mandanten
         """
         return self.client.service.getCurrentClientProperty("MANDANTID")
 
     def getMandantName(self) -> str:
         """
         Liefert den Namen des aktuellen Mandanten
         """
         return self.client.service.getCurrentClientProperty("NAME")
+
+    def getServerInfoString(self) -> str:
+        """
+        Liefert Informationen zum Server als String. Dieser String repräsentiert ein XML Dokument.
+
+        :return: das XML-Dokument als String
+        :rtype: str
+        """
+        return self.client.service.getP2plusServerInfo()
+
+    def getServerInfo(self) -> Optional[ET.Element]:
+        """
+        Liefert Informationen zum Server als ein XML Dokument.
+
+        :return: das gefundene und geparste XML-Dokument
+        :rtype: ET.Element
+        """
+        return ET.fromstring(self.getServerInfoString())
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/applus_server.py` & `PyAPplus64-1.0.1/src/PyAPplus64/applus_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,86 +2,85 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
-
-from requests import Session # type: ignore
+from requests import Session  # type: ignore
 from requests.auth import HTTPBasicAuth  # type: ignore # or HTTPDigestAuth, or OAuth1, etc.
 from zeep import Client
 from zeep.transports import Transport
 from zeep.cache import SqliteCache
 from typing import Optional, Dict
 
 
 class APplusAppServerSettings:
     """
     Einstellungen, mit welchem APplus App-Server sich verbunden werden soll.
     """
-    
-    def __init__(self, appserver : str, appserverPort : int, user : str, env : Optional[str] = None):
+
+    def __init__(self, appserver: str, appserverPort: int, user: str, env: Optional[str] = None):
         self.appserver = appserver
         self.appserverPort = appserverPort
         self.user = user
         self.env = env
 
+
 class APplusWebServerSettings:
     """
     Einstellungen, mit welchem APplus Web-Server sich verbunden werden soll.
     """
-    
-    def __init__(self, baseurl:Optional[str]=None):
-        self.baseurl : Optional[str] = baseurl;
-        try:        
+
+    def __init__(self, baseurl: Optional[str] = None):
+        self.baseurl: Optional[str] = baseurl
+        try:
             assert (isinstance(self.baseurl, str))
-            if not (self.baseurl == None) and not (self.baseurl[-1] == "/"):
-                self.baseurl = self.baseurl + "/";
+            if not (self.baseurl is None) and not (self.baseurl[-1] == "/"):
+                self.baseurl = self.baseurl + "/"
         except:
             pass
 
 
 class APplusServerConnection:
     """Verbindung zu einem APplus APP-Server
 
     :param settings: die Einstellungen für die Verbindung mit dem APplus Server
     :type settings: APplusAppServerSettings
     """
-    def __init__(self, settings : APplusAppServerSettings) -> None:
-        userEnv = settings.user;
+    def __init__(self, settings: APplusAppServerSettings) -> None:
+        userEnv = settings.user
         if (settings.env):
             userEnv += "|" + settings.env
 
         session = Session()
         session.auth = HTTPBasicAuth(userEnv, "")
 
         self.transport = Transport(cache=SqliteCache(), session=session)
         # self.transport = Transport(session=session)
-        self.clientCache : Dict[str, Client] = {}
-        self.settings=settings;
-        self.appserverUrl = "http://" + settings.appserver + ":" + str(settings.appserverPort) + "/";
+        self.clientCache: Dict[str, Client] = {}
+        self.settings = settings
+        self.appserverUrl = "http://" + settings.appserver + ":" + str(settings.appserverPort) + "/"
 
-    def getClient(self, package : str, name : str) -> Client:
+    def getClient(self, package: str, name: str) -> Client:
         """Erzeugt einen zeep - Client.
            Mittels dieses Clients kann die WSDL Schnittstelle angesprochen werden.
-           Wird als *package* "p2core" und als *name* "Table" verwendet und der 
+           Wird als *package* "p2core" und als *name* "Table" verwendet und der
            resultierende client "client" genannt, dann kann
            z.B. mittels "client.service.getCompleteSQL(sql)" vom AppServer ein Vervollständigen
            des SQLs angefordert werden.
 
            :param package: das Packet, z.B. "p2core"
            :type package: str
            :param name: der Name im Packet, z.B. "Table"
            :type package: string
            :return: den Client
            :rtype: Client
            """
-        url = package+"/"+name;
+        url = package+"/"+name
         try:
-            return self.clientCache[url];
+            return self.clientCache[url]
         except:
             fullClientUrl = self.appserverUrl + url + ".jws?wsdl"
             client = Client(fullClientUrl, transport=self.transport)
-            self.clientCache[url] = client;
-            return client;
+            self.clientCache[url] = client
+            return client
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/applus_sysconf.py` & `PyAPplus64-1.0.1/src/PyAPplus64/applus_sysconf.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,58 +2,56 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
+from typing import TYPE_CHECKING, Optional, Dict, Any, Callable, Sequence
 
-from typing import *
-
-if TYPE_CHECKING: 
+if TYPE_CHECKING:
     from .applus import APplusServer
 
 
 class APplusSysConf:
     """
     SysConf Zugriff mit Cache über AppServer
 
     :param server: die Verbindung zum Server
     :type server: APplusServer
 
     """
-    
-    def __init__(self, server : 'APplusServer') -> None:
+
+    def __init__(self, server: 'APplusServer') -> None:
         self.client = server.getClient("p2system", "SysConf")
-        self.cache : Dict[str, type] = {}
+        self.cache: Dict[str, type] = {}
 
     def clearCache(self) -> None:
-        self.cache = {};
+        self.cache = {}
 
-    def _getGeneral(self, ty:str, f : Callable[[str, str], Any], module:str, name:str, useCache:bool) -> Any:
-        cacheKey = module + "/" + name + "/" + ty;
+    def _getGeneral(self, ty: str, f: Callable[[str, str], Any], module: str, name: str, useCache: bool) -> Any:
+        cacheKey = module + "/" + name + "/" + ty
         if useCache and cacheKey in self.cache:
             return self.cache[cacheKey]
         else:
-            v = f(module, name);
-            self.cache[cacheKey] = v;
-            return v;
+            v = f(module, name)
+            self.cache[cacheKey] = v
+            return v
 
-    def getString(self, module:str, name:str, useCache:bool=True) -> str:
-        return self._getGeneral("string", self.client.service.getString, module, name, useCache);
+    def getString(self, module: str, name: str, useCache: bool = True) -> str:
+        return self._getGeneral("string", self.client.service.getString, module, name, useCache)
 
-    def getInt(self, module:str, name:str, useCache:bool=True) -> int:
-        return self._getGeneral("int", self.client.service.getInt, module, name, useCache);
+    def getInt(self, module: str, name: str, useCache: bool = True) -> int:
+        return self._getGeneral("int", self.client.service.getInt, module, name, useCache)
 
-    def getDouble(self, module:str, name:str, useCache:bool=True) -> float:
-        return self._getGeneral("double", self.client.service.getDouble, module, name, useCache);
+    def getDouble(self, module: str, name: str, useCache: bool = True) -> float:
+        return self._getGeneral("double", self.client.service.getDouble, module, name, useCache)
 
-    def getBoolean(self, module:str, name:str, useCache:bool=True) -> bool:
-        return self._getGeneral("boolean", self.client.service.getBoolean, module, name, useCache);
+    def getBoolean(self, module: str, name: str, useCache: bool = True) -> bool:
+        return self._getGeneral("boolean", self.client.service.getBoolean, module, name, useCache)
 
-    def getList(self, module : str, name:str, useCache:bool=True, sep:str=",") -> Optional[Sequence[str]]:
-        s = self.getString(module, name, useCache=useCache);
-        if (s == None or s == ""): 
+    def getList(self, module: str, name: str, useCache: bool = True, sep: str = ",") -> Optional[Sequence[str]]:
+        s = self.getString(module, name, useCache=useCache)
+        if (s is None or s == ""):
             return None
 
-        return s.split(sep);
+        return s.split(sep)
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/applus_usexml.py` & `PyAPplus64-1.0.1/src/PyAPplus64/applus_usexml.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,334 +2,324 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
-
-import lxml.etree as ET # type: ignore
+import lxml.etree as ET  # type: ignore
 from . import sql_utils
 import datetime
-from typing import *
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
-if TYPE_CHECKING: 
+if TYPE_CHECKING:
     from .applus import APplusServer
 
 
-
-def _formatValueForXMLRow(v : Any) -> str:
+def _formatValueForXMLRow(v: Any) -> str:
     """Hilfsfunktion zum Formatieren eines Wertes für XML"""
     if (v is None):
-        return "";
+        return ""
     if isinstance(v, (int, float)):
-        return str(v);
+        return str(v)
     elif isinstance(v, str):
-        return v;
+        return v
     elif isinstance(v, datetime.datetime):
         return v.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
     elif isinstance(v, datetime.date):
         return v.strftime("%Y-%m-%d")
     elif isinstance(v, datetime.time):
         return v.strftime("%H:%M:%S.%f")[:-3]
     else:
         return str(v)
 
 
 class UseXmlRow:
     """
-    Klasse, die eine XML-Datei erzeugen kann, die mittels p2core.useXML 
+    Klasse, die eine XML-Datei erzeugen kann, die mittels p2core.useXML
     genutzt werden kann. Damit ist es möglich APplus BusinessObjekte zu
     erzeugen, ändern und zu löschen. Im Gegensatz zu direkten DB-Zugriffen,
     werden diese Anfragen über den APP-Server ausgeführt. Dabei werden
     die von der Weboberfläche bekannten Checks und Änderungen ausgeführt.
     Als sehr einfaches Beispiel wird z.B. INSDATE oder UPDDATE automatisch gesetzt.
     Interessanter sind automatische Änderungen und Checks.
 
-    Bei der Benutzung wird zunächst ein Objekt erzeugt, dann evtl. 
-    mittels :meth:`addField` Felder hinzugefügt und schließlich mittels 
-    :meth:`exec` an den AppServer übergeben. 
+    Bei der Benutzung wird zunächst ein Objekt erzeugt, dann evtl.
+    mittels :meth:`addField` Felder hinzugefügt und schließlich mittels
+    :meth:`exec` an den AppServer übergeben.
     Normalerweise sollte die Klasse nicht direkt, sondern über Unterklassen
     für das Einfügen, Ändern oder Löschen benutzt werden.
 
-    :param applus: Verbindung zu APplus 
+    :param applus: Verbindung zu APplus
     :type applus: APplusServer
     :param table: die Tabelle
     :type table: str
     :param cmd: cmd-attribut der row, also ob es sich um ein Update, ein Insert oder ein Delete handelt
     :type cmd: str
     """
 
-    def __init__(self, applus : 'APplusServer', table : str, cmd : str) -> None:
+    def __init__(self, applus: 'APplusServer', table: str, cmd: str) -> None:
         self.applus = applus
         self.table = table
         self.cmd = cmd
-        self.fields : Dict[str, Any] = {}
+        self.fields: Dict[str, Any] = {}
 
     def __str__(self) -> str:
-        return self.toprettyxml() 
+        return self.toprettyxml()
 
-    def _buildXML(self) -> ET.Element :
+    def _buildXML(self) -> ET.Element:
         """Hilfsfunktion, die das eigentliche XML baut"""
-        row = ET.Element("row", cmd=self.cmd, table=self.table, nsmap={ "dt" : "urn:schemas-microsoft-com:datatypes"});
+        row = ET.Element("row", cmd=self.cmd, table=self.table, nsmap={"dt": "urn:schemas-microsoft-com:datatypes"})
 
         for name, value in self.fields.items():
             child = ET.Element(name)
             child.text = _formatValueForXMLRow(value)
             row.append(child)
 
         return row
 
-
-    def toprettyxml(self)->str:
+    def toprettyxml(self) -> str:
         """
-        Gibt das formatierte XML aus. Dieses kann per useXML an den AppServer übergeben werden. 
+        Gibt das formatierte XML aus. Dieses kann per useXML an den AppServer übergeben werden.
         Dies wird mittels :meth:`exec` automatisiert.
         """
-        return ET.tostring(self._buildXML(), encoding = "unicode", pretty_print=True)
+        return ET.tostring(self._buildXML(), encoding="unicode", pretty_print=True)
 
-    def getField(self, name:str) -> Any:
+    def getField(self, name: str) -> Any:
         """Liefert den Wert eines gesetzten Feldes"""
 
-        if name is None: 
+        if name is None:
             return None
-        name = sql_utils.normaliseDBfield(name);
+        name = sql_utils.normaliseDBfield(name)
 
         if name in self.fields:
             return self.fields[name]
         elif name == "MANDANT":
             return self.applus.scripttool.getMandant()
         else:
             return None
 
-    def checkFieldSet(self, name:Optional[str]) -> bool:
+    def checkFieldSet(self, name: Optional[str]) -> bool:
         """Prüft, ob ein Feld gesetzt wurde"""
-        if name is None: 
+        if name is None:
             return False
         name = sql_utils.normaliseDBfield(name)
         return (name in self.fields) or (name == "MANDANT")
 
-    def checkFieldsSet(self, *names : str) -> bool:
+    def checkFieldsSet(self, *names: str) -> bool:
         """Prüft, ob alle übergebenen Felder gesetzt sind"""
         for n in names:
             if not (self.checkFieldSet(n)):
                 return False
         return True
 
-    def addField(self, name:str|None, value:Any) -> None:
+    def addField(self, name: Optional[str], value: Any) -> None:
         """
         Fügt ein Feld zum Row-Node hinzu.
 
         :param name: das Feld
         :type name: string
         :param value: Wert des Feldes
         """
-        if name is None: 
+        if name is None:
             return
-    
-        self.fields[sql_utils.normaliseDBfield(name)] = value
 
+        self.fields[sql_utils.normaliseDBfield(name)] = value
 
-    def addTimestampField(self, id:int, ts:Optional[bytes]=None) -> None:
+    def addTimestampField(self, id: int, ts: Optional[bytes] = None) -> None:
         """
-        Fügt ein Timestamp-Feld hinzu. Wird kein Timestamp übergeben, wird mittels der ID der aktuelle 
+        Fügt ein Timestamp-Feld hinzu. Wird kein Timestamp übergeben, wird mittels der ID der aktuelle
         Timestamp aus der DB geladen. Dabei kann ein Fehler auftreten.
         Ein Timestamp-Feld ist für Updates und das Löschen nötig um sicherzustellen, dass die richtige
         Version des Objekts geändert oder gelöscht wird. Wird z.B. ein Objekt aus der DB geladen, inspiziert
         und sollen dann Änderungen gespeichert werden, so sollte der Timestamp des Ladens übergeben werden.
         So wird sichergestellt, dass nicht ein anderer User zwischenzeitlich Änderungen vornahm. Ist dies
         der Fall, wird dann bei "exec" eine Exception geworfen.
 
-        :param id: DB-id des Objektes dessen Timestamp hinzugefügt werden soll   
+        :param id: DB-id des Objektes dessen Timestamp hinzugefügt werden soll
         :type id: string
         :param ts: Fester Timestamp der verwendet werden soll, wenn None wird der Timestamp aus der DB geladen.
         :type ts: bytes
         """
         if ts is None:
-            ts = self.applus.dbQuerySingleValue("select timestamp from " + self.table + " where id = ?", id);
+            ts = self.applus.dbQuerySingleValue("select timestamp from " + self.table + " where id = ?", id)
         if ts:
-            self.addField("timestamp", ts.hex());
+            self.addField("timestamp", ts.hex())
         else:
             raise Exception("kein Eintrag in Tabelle '" + self.table + " mit ID " + str(id) + " gefunden")
 
-
-    def addTimestampIDFields(self, id:int, ts:Optional[bytes]=None) -> None:
+    def addTimestampIDFields(self, id: int, ts: Optional[bytes] = None) -> None:
         """
-        Fügt ein Timestamp-Feld sowie ein Feld id hinzu. Wird kein Timestamp übergeben, wird mittels der ID der aktuelle 
+        Fügt ein Timestamp-Feld sowie ein Feld id hinzu. Wird kein Timestamp übergeben, wird mittels der ID der aktuelle
         Timestamp aus der DB geladen. Dabei kann ein Fehler auftreten. Intern wird :meth:`addTimestampField` benutzt.
 
-        :param id: DB-id des Objektes dessen Timestamp hinzugefügt werden soll   
+        :param id: DB-id des Objektes dessen Timestamp hinzugefügt werden soll
         :type id: string
         :param ts: Fester Timestamp der verwendet werden soll, wenn None wird der Timestamp aus der DB geladen.
         :type ts: bytes
         """
         self.addField("id", id)
-        self.addTimestampField(id, ts=ts);
+        self.addTimestampField(id, ts=ts)
 
     def exec(self) -> Any:
         """
         Führt die UseXmlRow mittels useXML aus. Je nach Art der Zeile wird etwas zurückgeliefert oder nicht.
         In jedem Fall kann eine Exception geworfen werden.
         """
-        return self.applus.useXML(self.toprettyxml());
+        return self.applus.useXML(self.toprettyxml())
 
 
 class UseXmlRowInsert(UseXmlRow):
     """
     Klasse, die eine XML-Datei für das Einfügen eines neuen Datensatzes erzeugen kann.
 
-    :param applus: Verbindung zu APplus 
+    :param applus: Verbindung zu APplus
     :type applus: APplusServer
     :param table: die Tabelle
     :type table: string
     """
 
-    def __init__(self, applus:'APplusServer', table:str) -> None:
-        super().__init__(applus, table, "insert");
-    
+    def __init__(self, applus: 'APplusServer', table: str) -> None:
+        super().__init__(applus, table, "insert")
+
     def insert(self) -> int:
         """
         Führt das insert aus. Entweder wird dabei eine Exception geworfen oder die ID des neuen Eintrags zurückgegeben.
         Dies ist eine Umbenennung von :meth:`exec`.
         """
-        return super().exec();
+        return super().exec()
 
 
 class UseXmlRowDelete(UseXmlRow):
     """
     Klasse, die eine XML-Datei für das Löschen eines neuen Datensatzes erzeugen kann.
     Die Felder `id` und `timestamp` werden automatisch gesetzt.
     Dies sind die einzigen Felder, die gesetzt werden sollten.
 
-    :param applus: Verbindung zu APplus 
+    :param applus: Verbindung zu APplus
     :type applus: APplusServer
     :param table: die Tabelle
     :type table: string
     :param id: die zu löschende ID
     :type id: int
     :param ts: wenn gesetzt, wird dieser Timestamp verwendet, sonst der aktuelle aus der DB
     :type ts: bytes optional
     """
 
-    def __init__(self, applus:'APplusServer', table:str, id:int, ts:Optional[bytes]=None) -> None:
-        super().__init__(applus, table, "delete");
-        self.addTimestampIDFields(id, ts=ts);
+    def __init__(self, applus: 'APplusServer', table: str, id: int, ts: Optional[bytes] = None) -> None:
+        super().__init__(applus, table, "delete")
+        self.addTimestampIDFields(id, ts=ts)
 
-    
     def delete(self) -> None:
         """
         Führt das delete aus. Evtl. wird dabei eine Exception geworfen.
         Dies ist eine Umbenennung von :meth:`exec`.
         """
-        super().exec();        
+        super().exec()
 
 
 class UseXmlRowUpdate(UseXmlRow):
     """
     Klasse, die eine XML-Datei für das Ändern eines neuen Datensatzes, erzeugen kann.
     Die Felder `id` und `timestamp` werden automatisch gesetzt.
 
-    :param applus: Verbindung zu APplus 
+    :param applus: Verbindung zu APplus
     :type applus: APplusServer
     :param table: die Tabelle
     :type table: string
     :param id: die ID des zu ändernden Datensatzes
     :type id: int
     :param ts: wenn gesetzt, wird dieser Timestamp verwendet, sonst der aktuelle aus der DB
     :type ts: bytes optional
     """
 
-    def __init__(self, applus : 'APplusServer', table : str, id : int, ts:Optional[bytes]=None) -> None:
-        super().__init__(applus, table, "update");
-        self.addTimestampIDFields(id, ts=ts);
+    def __init__(self, applus: 'APplusServer', table: str, id: int, ts: Optional[bytes] = None) -> None:
+        super().__init__(applus, table, "update")
+        self.addTimestampIDFields(id, ts=ts)
 
-    
     def update(self) -> None:
         """
         Führt das update aus. Evtl. wird dabei eine Exception geworfen.
         Dies ist eine Umbenennung von :meth:`exec`.
         """
-        super().exec();        
-
+        super().exec()
 
 
 class UseXmlRowInsertOrUpdate(UseXmlRow):
     """
     Klasse, die eine XML-Datei für das Einfügen oder Ändern eines neuen Datensatzes, erzeugen kann.
     Die Methode `checkExists` erlaubt es zu prüfen, ob ein Objekt bereits existiert. Dafür werden die
     gesetzten Felder mit den Feldern aus eindeutigen Indices verglichen. Existiert ein Objekt bereits, wird
-    ein Update ausgeführt, ansonsten ein Insert. Bei Updates werden die Felder `id` und `timestamp` 
+    ein Update ausgeführt, ansonsten ein Insert. Bei Updates werden die Felder `id` und `timestamp`
     automatisch gesetzt.
 
-    :param applus: Verbindung zu APplus 
+    :param applus: Verbindung zu APplus
     :type applus: APplusServer
     :param table: die Tabelle
     :type table: string
     """
 
-    def __init__(self, applus : 'APplusServer', table : str) -> None:
-        super().__init__(applus, table, "");
+    def __init__(self, applus: 'APplusServer', table: str) -> None:
+        super().__init__(applus, table, "")
 
-    
-    def checkExists(self) -> int|None:
+    def checkExists(self) -> Optional[int]:
         """
-        Prüft, ob der Datensatz bereits in der DB existiert. 
+        Prüft, ob der Datensatz bereits in der DB existiert.
         Ist dies der Fall, wird die ID geliefert, sonst None
         """
 
         # Baue Bedingung
-        cond = sql_utils.SqlConditionOr();
+        cond = sql_utils.SqlConditionOr()
         for idx, fs in self.applus.getUniqueFieldsOfTable(self.table).items():
             if (self.checkFieldsSet(*fs)):
-                condIdx = sql_utils.SqlConditionAnd();
+                condIdx = sql_utils.SqlConditionAnd()
                 for f in fs:
                     condIdx.addConditionFieldEq(f, self.getField(f))
                 cond.addCondition(condIdx)
-        
+
         sql = sql_utils.SqlStatementSelect(self.table, "id")
         sql.where = cond
         return self.applus.dbQuerySingleValue(sql)
 
     def insert(self) -> int:
         """Führt ein Insert aus. Existiert das Objekt bereits, wird eine Exception geworfen."""
 
-        r = UseXmlRowInsert(self.applus, self.table)            
+        r = UseXmlRowInsert(self.applus, self.table)
         for k, v in self.fields.items():
             r.addField(k, v)
-        return r.insert();
+        return r.insert()
 
-    def update(self, id:Optional[int]=None, ts:Optional[bytes]=None) -> int:
+    def update(self, id: Optional[int] = None, ts: Optional[bytes] = None) -> int:
         """Führt ein Update aus. Falls ID oder Timestamp nicht übergeben werden, wird
         nach einem passenden Objekt gesucht. Existiert das Objekt nicht, wird eine Exception geworfen."""
 
         if id is None:
             id = self.checkExists()
 
         if id is None:
             raise Exception("Update nicht möglich, da kein Objekt für Update gefunden.")
-        
-        r = UseXmlRowUpdate(self.applus, self.table, id, ts=ts)            
+
+        r = UseXmlRowUpdate(self.applus, self.table, id, ts=ts)
         for k, v in self.fields.items():
             r.addField(k, v)
-        r.update();
+        r.update()
         return id
 
-    def exec(self) -> int:   
+    def exec(self) -> int:
         """
         Führt entweder ein Update oder ein Insert durch. Dies hängt davon ab, ob das Objekt bereits in
         der DB existiert. In jedem Fall wird die ID des erzeugten oder geänderten Objekts geliefert.
         """
 
-        id = self.checkExists();
-        if id == None:
+        id = self.checkExists()
+        if id is None:
             return self.insert()
-        else:            
+        else:
             return self.update(id=id)
 
     def updateOrInsert(self) -> int:
         """
         Führt das update oder das insert aus. Evtl. wird dabei eine Exception geworfen.
         Dies ist eine Umbenennung von :meth:`exec`.
         Es wird die ID des Eintrages geliefert
         """
-        return self.exec();        
+        return self.exec()
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/duplicate.py` & `PyAPplus64-1.0.1/src/PyAPplus64/duplicate.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,570 +2,562 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
-
 """
 Dupliziert ein oder mehrere APplus Business-Objekte
 """
 
 from . import sql_utils
 from . import applus_db
 from . import applus_usexml
 from .applus import APplusServer
-import pyodbc # type: ignore
+import pyodbc  # type: ignore
 import traceback
 import logging
-from typing import *
+from typing import List, Set, Optional, Dict, Tuple, Sequence, Any, Union
 
-logger = logging.getLogger(__name__);
+logger = logging.getLogger(__name__)
 
 noCopyFields = sql_utils.normaliseDBfieldSet({"INSUSER", "UPDDATE", "TIMESTAMP", "MANDANT", "GUID", "ID", "TIMESTAMP_A", "INSDATE", "ID_A", "UPDUSER"})
 """Menge von Feld-Namen, die nie kopiert werden sollen."""
 
 
-def getFieldsToCopyForTable(server : APplusServer, table : str, force:bool=True) -> Set[str]:
+def getFieldsToCopyForTable(server: APplusServer, table: str, force: bool = True) -> Set[str]:
     """
     Bestimmt die für eine Tabelle zu kopierenden Spalten. Dazu wird in den XML-Definitionen geschaut.
-    Ist dort 'include' hinterlegt, werden diese Spalten verwendet. Ansonsten alle nicht generierten Spalten, 
+    Ist dort 'include' hinterlegt, werden diese Spalten verwendet. Ansonsten alle nicht generierten Spalten,
     ohne die 'exclude' Spalten. In jedem Fall werden Spalten wie "ID", die nie kopiert werden sollten, entfernt.
     """
 
     xmlDefs = server.scripttool.getXMLDefinitionObj(table)
-    fields : Set[str]
+    fields: Set[str]
     if (xmlDefs is None):
         if not force:
-            raise Exception ("Keine XML-Definitionen für '{}' gefunden".format(table));
+            raise Exception("Keine XML-Definitionen für '{}' gefunden".format(table))
         (fields, excl) = (set(), True)
-    else: 
+    else:
         (fields, excl) = xmlDefs.getDuplicate()
-    if not excl: 
+    if not excl:
         return fields.difference(noCopyFields)
 
     allFields = server.getTableFields(table, isComputed=False)
-    return allFields.difference(fields).difference(noCopyFields);
-
+    return allFields.difference(fields).difference(noCopyFields)
 
 
 class FieldsToCopyForTableCache():
     """
     Cache für welche Felder für welche Tabelle kopiert werden sollen
     """
-    
-    def __init__(self, server : APplusServer) -> None:
+
+    def __init__(self, server: APplusServer) -> None:
         self.server = server
-        self.cache : Dict[str, Set[str]]= {}
+        self.cache: Dict[str, Set[str]] = {}
 
-    def getFieldsToCopyForTable(self, table : str) -> Set[str]:
+    def getFieldsToCopyForTable(self, table: str) -> Set[str]:
         """
         Bestimmt die für eine Tabelle zu kopierenden Spalten. Dazu wird in den XML-Definitionen geschaut.
-        Ist dort 'include' hinterlegt, werden diese Spalten verwendet. Ansonsten alle nicht generierten Spalten, 
+        Ist dort 'include' hinterlegt, werden diese Spalten verwendet. Ansonsten alle nicht generierten Spalten,
         ohne die 'exclude' Spalten. In jedem Fall werden Spalten wie "ID", die nie kopiert werden sollten, entfernt.
         """
         if (table is None):
             return None
-        
+
         t = table.upper()
         fs = self.cache.get(t, None)
         if not (fs is None):
             return fs
         else:
             fs = getFieldsToCopyForTable(self.server, t)
             self.cache[t] = fs
             return fs
 
 
-def initFieldsToCopyForTableCacheIfNeeded(server : APplusServer, cache : Optional[FieldsToCopyForTableCache]) -> FieldsToCopyForTableCache:
+def initFieldsToCopyForTableCacheIfNeeded(server: APplusServer, cache: Optional[FieldsToCopyForTableCache]) -> FieldsToCopyForTableCache:
     """
     Hilfsfunktion, die einen Cache erzeugt, falls dies noch nicht geschehen ist.
     """
     if cache is None:
         return FieldsToCopyForTableCache(server)
     else:
-        return cache;
+        return cache
 
 
 class DuplicateBusinessObject():
     """
     Klasse, die alle Daten zu einem BusinessObject speichert und zum Duplizieren dieses Objektes dient.
     Dies beinhaltet Daten zu abhängigen Objekten sowie die Beziehung zu diesen Objekten. Zu einem Artikel
     wird z.B. der Arbeitsplan gespeichert, der wiederum Arbeitsplanpositionen enthält. Als Beziehung ist u.a.
     hinterlegt, dass das Feld "APLAN" der Arbeitsplans dem Feld "ARTIKEL" des Artikels entsprechen muss und dass
-    "APLAN" aus den Positionen, "APLAN" aus dem APlan entsprichen muss. So kann beim Duplizieren ein 
+    "APLAN" aus den Positionen, "APLAN" aus dem APlan entsprichen muss. So kann beim Duplizieren ein
     anderer Name des Artikels gesetzt werden und automatisch die Felder der abhängigen Objekte angepasst werden.
     Einige Felder der Beziehung sind dabei statisch, d.h. können direkt aus den zu speichernden Daten abgelesen werden.
-    Andere Felder sind dynamisch, d.h. das Parent-Objekt muss in der DB angelegt werden, damit ein solcher dynamischer Wert erstellt 
+    Andere Felder sind dynamisch, d.h. das Parent-Objekt muss in der DB angelegt werden, damit ein solcher dynamischer Wert erstellt
     und geladen werden kann. Ein typisches Beispiel für ein dynamisches Feld ist "GUID".
     """
 
-    def __init__(self, table : str, fields : Dict[str, Any], fieldsNotCopied:Dict[str, Any]={}, allowUpdate:bool=False) -> None:
+    def __init__(self, table: str, fields: Dict[str, Any], fieldsNotCopied: Dict[str, Any] = {}, allowUpdate: bool = False) -> None:
         self.table = table
         """für welche Tabelle ist das BusinessObject"""
 
-        self.fields = fields        
+        self.fields = fields
         """die Daten"""
 
         self.fieldsNotCopied = fieldsNotCopied
         """Datenfelder, die im Original vorhanden sind, aber nicht kopiert werden sollen"""
-    
-        self.dependentObjs : List[Dict[str, Any]] = []
+
+        self.dependentObjs: List[Dict[str, Any]] = []
         """Abhängige Objekte"""
 
         self.allowUpdate = allowUpdate
         """Erlaube Updates statt Fehlern, wenn Objekt schon in DB existiert"""
 
-    def addDependentBusinessObject(self, dObj : Optional['DuplicateBusinessObject'], *args : Tuple[str, str]) -> None:
+    def addDependentBusinessObject(self, dObj: Optional['DuplicateBusinessObject'], *args: Tuple[str, str]) -> None:
         """
         Fügt ein neues Unterobjekt zum DuplicateBusinessObject hinzu.
         Dabei handelt es sich selbst um ein DuplicateBusinessObject, das zusammen mit dem
-        Parent-Objekt dupliziert werden sollen. Zum Beispiel sollen zu einem 
+        Parent-Objekt dupliziert werden sollen. Zum Beispiel sollen zu einem
         Auftrag auch die Positionen dupliziert werden.
         Zusätzlich zum Objekt selbst können mehrere (keine, eine oder viele)
         Paare von Feldern übergeben werden. Ein Paar ("pf", "sf") verbindet das
         Feld "pf" des Parent-Objekts mit dem Feld "sf" des Sub-Objekts. So ist es möglich,
         Werte des Parent-Objekts zu ändern und diese Änderungen für Sub-Objekte zu übernehmen.
         Üblicherweise muss zum Beispiel die Nummer des Hauptobjekts geändert werden. Die
         gleiche Änderung ist für alle abhängigen  Objekte nötig, damit die neuen Objekte sich auf das
         Parent-Objekt beziehen.
 
         :param dObj: das Unter-Objekt
         :type dObj: DuplicateBusinessObject
         :param args: Liste von Tupeln, die Parent- und Sub-Objekt-Felder miteinander verbinden
         """
         if (dObj is None):
-            return 
+            return
 
-        args2= {}
+        args2 = {}
         for f1, f2 in args:
             args2[sql_utils.normaliseDBfield(f1)] = sql_utils.normaliseDBfield(f2)
-        
+
         self.dependentObjs.append({
-                "dependentObj" : dObj,
-                "connection" : args2
+                "dependentObj": dObj,
+                "connection": args2
             })
 
-    def getField(self, field:str, onlyCopied:bool=False) -> Any:
+    def getField(self, field: str, onlyCopied: bool = False) -> Any:
         """
-        Schlägt den Wert eines Feldes nach. Wenn onlyCopied gesetzt ist, werden nur Felder zurückgeliefert, die auch kopiert 
+        Schlägt den Wert eines Feldes nach. Wenn onlyCopied gesetzt ist, werden nur Felder zurückgeliefert, die auch kopiert
         werden sollen.
         """
 
         f = sql_utils.normaliseDBfield(field)
         if (f in self.fields):
             return self.fields[f]
 
         if (not onlyCopied) and (f in self.fieldsNotCopied):
             return self.fieldsNotCopied[f]
-        
+
         return None
 
-    def insert(self, server : APplusServer) -> applus_db.DBTableIDs:
+    def insert(self, server: APplusServer) -> applus_db.DBTableIDs:
         """
         Fügt alle Objekte zur DB hinzu. Es wird die Menge der IDs der erzeugten
         Objekte gruppiert nach Tabellen erzeugt. Falls ein Datensatz schon
         existiert, wird dieser entweder aktualisiert oder eine Fehlermeldung
         geworfen. Geliefert wird die Menge aller Eingefügten Objekte mit ihrer ID.
         """
-        
+
         res = applus_db.DBTableIDs()
 
-        def insertDO(do : 'DuplicateBusinessObject') -> Optional[int]:
+        def insertDO(do: 'DuplicateBusinessObject') -> Optional[int]:
             nonlocal res
-            insertRow : applus_usexml.UseXmlRow
-            if do.allowUpdate:                
-                insertRow = server.mkUseXMLRowInsertOrUpdate(do.table);
+            insertRow: applus_usexml.UseXmlRow
+            if do.allowUpdate:
+                insertRow = server.mkUseXMLRowInsertOrUpdate(do.table)
             else:
-                insertRow = server.mkUseXMLRowInsert(do.table);
+                insertRow = server.mkUseXMLRowInsert(do.table)
 
             for f, v in do.fields.items():
                 insertRow.addField(f, v)
-            
+
             try:
                 id = insertRow.exec()
                 res.add(do.table, id)
                 return id
             except:
-                msg = traceback.format_exc();
+                msg = traceback.format_exc()
                 logger.error("Exception inserting BusinessObjekt: %s\n%s", str(insertRow), msg)
                 return None
 
-        def insertDep(do : 'DuplicateBusinessObject', doID : int, so : 'DuplicateBusinessObject', connect : Dict[str,str]) -> None:
+        def insertDep(do: 'DuplicateBusinessObject', doID: int, so: 'DuplicateBusinessObject', connect: Dict[str, str]) -> None:
             nonlocal res
 
             # Abbruch, wenn do nicht eingefügt wurde
             if (doID is None):
                 return
 
             # copy known fields of connect
             connectMissing = {}
             for fd, fs in connect.items():
                 if fd in do.fields:
                     so.fields[fs] = do.fields[fd]
                 else:
                     connectMissing[fd] = fs
-            
+
             # load missing fields from DB
             if len(connectMissing) > 0:
-                sql = sql_utils.SqlStatementSelect(do.table);
+                sql = sql_utils.SqlStatementSelect(do.table)
                 sql.where.addConditionFieldEq("id", doID)
                 for fd in connectMissing:
                     sql.addFields(fd)
 
                 rd = server.dbQuerySingleRowDict(sql)
                 if not (rd is None):
                     for fd, fs in connectMissing.items():
                         so.fields[fs] = rd[fd]
 
             # real insert
             id = insertDO(so)
             if not (id is None):
                 insertDeps(so, id)
 
-
-        def insertDeps(do : 'DuplicateBusinessObject', doID : int) -> None:
+        def insertDeps(do: 'DuplicateBusinessObject', doID: int) -> None:
             for so in do.dependentObjs:
                 insertDep(do, doID, so["dependentObj"], so["connection"])
-        
+
         topID = insertDO(self)
         if not (topID is None):
             insertDeps(self, topID)
 
         return res
 
-
-    def setFields(self, upds : Dict[str, Any]) -> None:
+    def setFields(self, upds: Dict[str, Any]) -> None:
         """
         Setzt Felder des DuplicateBusinessObjektes und falls nötig seiner Unterobjekte.
         So kann zum Beispiel die Nummer vor dem Speichern geändert werden.
 
         :param upds: Dictionary mit zu setzenden Werten
         """
 
-        def setFieldsInternal(dobj : 'DuplicateBusinessObject', upds : Dict[str, Any]) -> None:
+        def setFieldsInternal(dobj: 'DuplicateBusinessObject', upds: Dict[str, Any]) -> None:
             # setze alle Felder des Hauptobjekts
             for f, v in upds.items():
                 dobj.fields[f] = v
-            
+
             # verarbeite alle Subobjekte
             for su in dobj.dependentObjs:
                 subupds = {}
                 for fp, fs in su["connection"].items():
                     if fp in upds:
                         subupds[fs] = upds[fp]
                 setFieldsInternal(su["dependentObj"], subupds)
-            
 
-        updsNorm : Dict[str, Any] = {}
+        updsNorm: Dict[str, Any] = {}
         for f, v in upds.items():
             updsNorm[sql_utils.normaliseDBfield(f)] = v
         setFieldsInternal(self, updsNorm)
 
 
-
 def _loadDBDuplicateBusinessObjectDict(
-        server : APplusServer, 
-        table : str, 
-        row : pyodbc.Row, 
-        cache:Optional[FieldsToCopyForTableCache]=None, 
-        allowUpdate:bool=False) -> Optional[DuplicateBusinessObject]:
+        server: APplusServer,
+        table: str,
+        row: pyodbc.Row,
+        cache: Optional[FieldsToCopyForTableCache] = None,
+        allowUpdate: bool = False) -> Optional[DuplicateBusinessObject]:
     """
     Hilfsfunktion, die ein DuplicateBusinessObjekt erstellt. Die Daten stammen aus
     einer PyOdbc Zeile. So ist es möglich, mit nur einem SQL-Statement,
-    mehrere DuplicateBusinessObjekte zu erstellen. 
+    mehrere DuplicateBusinessObjekte zu erstellen.
 
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :param table: Tabelle für das neue DuplicateBusinessObjekt
     :param row: die Daten als PyODBC Zeile
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :return: das neue DuplicateBusinessObject
     """
-    table = table.upper();
+    table = table.upper()
 
     def getFieldsToCopy() -> Set[str]:
         if cache is None:
             return getFieldsToCopyForTable(server, table)
-        else: 
+        else:
             return cache.getFieldsToCopyForTable(table)
-        
 
     def getFields() -> Tuple[Dict[str, Any], Dict[str, Any]]:
         ftc = getFieldsToCopy()
-        fields = {}   
+        fields = {}
         fieldsNotCopied = {}
         for f, v in applus_db.row_to_dict(row).items():
-            f = sql_utils.normaliseDBfield(f);
+            f = sql_utils.normaliseDBfield(f)
             if f in ftc:
                 fields[f] = v
             else:
                 fieldsNotCopied[f] = v
         return (fields, fieldsNotCopied)
 
-    
     if (row is None):
         return None
 
-    (fields, fieldsNotCopied) = getFields()   
+    (fields, fieldsNotCopied) = getFields()
     return DuplicateBusinessObject(table, fields, fieldsNotCopied=fieldsNotCopied, allowUpdate=allowUpdate)
 
 
 def loadDBDuplicateBusinessObject(
-        server : APplusServer, 
-        table : str, 
-        cond : sql_utils.SqlCondition, 
-        cache : Optional[FieldsToCopyForTableCache]=None, 
-        allowUpdate : bool = False) -> Optional[DuplicateBusinessObject]:
+        server: APplusServer,
+        table: str,
+        cond: sql_utils.SqlCondition,
+        cache: Optional[FieldsToCopyForTableCache] = None,
+        allowUpdate: bool = False) -> Optional[DuplicateBusinessObject]:
     """
     Läd ein einzelnes DuplicateBusinessObjekt aus der DB. Die Bedingung sollte dabei
-    einen eindeutigen Datensatz auswählen. Werden mehrere zurückgeliefert, wird ein 
+    einen eindeutigen Datensatz auswählen. Werden mehrere zurückgeliefert, wird ein
     zufälliger ausgewählt. Wird kein Datensatz gefunden, wird None geliefert.
 
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :type server: APplusServer
     :param table: Tabelle für das neue DuplicateBusinessObjekt
     :type table: str
     :param cond: SQL-Bedingung zur Auswahl eines Objektes
     :type cond: sql_utils.SqlCondition
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :type cache: Optional[FieldsToCopyForTableCache]
     :param allowUpdate: ist Update statt Insert erlaubt?
     :type allowUpdate: bool
     :return: das neue DuplicateBusinessObject
     :rtype: Optional[DuplicateBusinessObject]
     """
-    table = table.upper();
+    table = table.upper()
 
-    def getRow() -> pyodbc.Row:    
+    def getRow() -> pyodbc.Row:
         sql = sql_utils.SqlStatementSelect(table)
         sql.setTop(1)
-        sql.where.addCondition(cond);
+        sql.where.addCondition(cond)
         return server.dbQuerySingleRow(sql)
 
-    return _loadDBDuplicateBusinessObjectDict(server, table, getRow(), cache=cache, allowUpdate=allowUpdate);
+    return _loadDBDuplicateBusinessObjectDict(server, table, getRow(), cache=cache, allowUpdate=allowUpdate)
+
 
 def loadDBDuplicateBusinessObjectSimpleCond(
-        server : APplusServer, 
-        table : str, 
-        field : str, 
-        value : Optional[Union[sql_utils.SqlValue, bool]], 
-        cache : Optional[FieldsToCopyForTableCache]=None, 
-        allowUpdate : bool = False) -> Optional[DuplicateBusinessObject]:              
+        server: APplusServer,
+        table: str,
+        field: str,
+        value: Union[sql_utils.SqlValue, bool, None],
+        cache: Optional[FieldsToCopyForTableCache] = None,
+        allowUpdate: bool = False) -> Optional[DuplicateBusinessObject]:
     """
     Wrapper für loadDBDuplicateBusinessObject, das eine einfache Bedingung benutzt,
     bei der ein Feld einen bestimmten Wert haben muss.
 
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :type server: APplusServer
     :param table: Tabelle für das neue DuplicateBusinessObjekt
     :type table: str
     :param field: Feld für Bedingung
     :type field: str
     :param value: Wert des Feldes für Bedingung
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :type cache: Optional[FieldsToCopyForTableCache]
     :return: das neue DuplicateBusinessObject
     :rtype: Optional[DuplicateBusinessObject]
     """
     cond = sql_utils.SqlConditionFieldEq(field, value)
     return loadDBDuplicateBusinessObject(server, table, cond, cache=cache, allowUpdate=allowUpdate)
-    
+
 
 def loadDBDuplicateBusinessObjects(
-        server : APplusServer, 
-        table : str, 
-        cond : sql_utils.SqlCondition, 
-        cache : Optional[FieldsToCopyForTableCache]=None, 
-        allowUpdate : bool = False) -> Sequence[DuplicateBusinessObject]:
+        server: APplusServer,
+        table: str,
+        cond: sql_utils.SqlCondition,
+        cache: Optional[FieldsToCopyForTableCache] = None,
+        allowUpdate: bool = False) -> Sequence[DuplicateBusinessObject]:
     """
     Läd eine Liste von DuplicateBusinessObjekten aus der DB. Die Bedingung kann mehrere Datensätze auswählen.
 
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :type server: APplusServer
     :param table: Tabelle für das neue DuplicateBusinessObjekt
     :type table: str
     :param cond: SQL-Bedingung zur Auswahl eines Objektes
     :type cond: sql_utils.SqlCondition
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :type cache: Optional[FieldsToCopyForTableCache]
     :return: Liste der neuen DuplicateBusinessObjects
     :rtype: Sequence[DuplicateBusinessObject]
     """
     table = table.upper()
     cache = initFieldsToCopyForTableCacheIfNeeded(server, cache)
 
-    def processRow(r : pyodbc.Row) -> Optional[DuplicateBusinessObject]:
-        return _loadDBDuplicateBusinessObjectDict(server, table, r, cache=cache, allowUpdate=allowUpdate)        
-    
+    def processRow(r: pyodbc.Row) -> Optional[DuplicateBusinessObject]:
+        return _loadDBDuplicateBusinessObjectDict(server, table, r, cache=cache, allowUpdate=allowUpdate)
+
     sql = sql_utils.SqlStatementSelect(table)
     sql.where.addCondition(cond)
     return server.dbQueryAll(sql, apply=processRow)
-    
+
+
 def loadDBDuplicateBusinessObjectsSimpleCond(
-        server : APplusServer, 
-        table : str, 
-        field : str, 
-        value : Optional[Union[sql_utils.SqlValue, bool]], 
-        cache : Optional[FieldsToCopyForTableCache]=None, 
-        allowUpdate : bool = False) -> Sequence[DuplicateBusinessObject]:
+        server: APplusServer,
+        table: str,
+        field: str,
+        value: Union[sql_utils.SqlValue, bool, None],
+        cache: Optional[FieldsToCopyForTableCache] = None,
+        allowUpdate: bool = False) -> Sequence[DuplicateBusinessObject]:
     """
     Wrapper für loadDBDuplicateBusinessObjects, das eine einfache Bedingung benutzt,
     bei der ein Feld einen bestimmten Wert haben muss.
 
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :type server: APplusServer
     :param table: Tabelle für das neue DuplicateBusinessObjekt
     :type table: str
     :param field: Feld für Bedingung
     :param value: Wert des Feldes für Bedingung
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :type cache: Optional[FieldsToCopyForTableCache]
     :return: Liste der neuen DuplicateBusinessObjects
     :rtype: Sequence[DuplicateBusinessObject]
     """
     cond = sql_utils.SqlConditionFieldEq(field, value)
     return loadDBDuplicateBusinessObjects(server, table, cond, cache=cache, allowUpdate=allowUpdate)
-    
+
 
 # Im Laufe der Zeit sollten load-Funktionen für verschiedene BusinessObjekte
 # erstellt werden. Dies erfolgt immer, wenn eine solche Funktion wirklich
 # benutzt werden soll
 
 def loadDBDuplicateAPlan(
-        server : APplusServer, 
-        aplan : str, 
-        cache:Optional[FieldsToCopyForTableCache]=None) -> Optional[DuplicateBusinessObject]:
+        server: APplusServer,
+        aplan: str,
+        cache: Optional[FieldsToCopyForTableCache] = None) -> Optional[DuplicateBusinessObject]:
     """
-    Erstelle DuplicateBusinessObject für einzelnen Arbeitsplan. 
-    
+    Erstelle DuplicateBusinessObject für einzelnen Arbeitsplan.
+
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :type server: APplusServer
     :param aplan: Aplan, der kopiert werden soll.
     :type aplan: str
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :type cache: Optional[FieldsToCopyForTableCache]
     :return: das neue DuplicateBusinessObject
     :rtype: DuplicateBusinessObject
     """
 
-    cache = initFieldsToCopyForTableCacheIfNeeded(server, cache);
+    cache = initFieldsToCopyForTableCacheIfNeeded(server, cache)
     boMain = loadDBDuplicateBusinessObjectSimpleCond(server, "aplan", "APLAN", aplan, cache=cache)
     if boMain is None:
         return None
 
     for so in loadDBDuplicateBusinessObjectsSimpleCond(server, "aplanpos", "APLAN", aplan, cache=cache):
         boMain.addDependentBusinessObject(so, ("aplan", "aplan"))
-    
+
     return boMain
 
 
-def loadDBDuplicateStueli(server : APplusServer, stueli : str, cache:Optional[FieldsToCopyForTableCache]=None) -> Optional[DuplicateBusinessObject]:
+def loadDBDuplicateStueli(server: APplusServer, stueli: str, cache: Optional[FieldsToCopyForTableCache] = None) -> Optional[DuplicateBusinessObject]:
     """
-    Erstelle DuplicateBusinessObject für einzelne Stückliste. 
-    
+    Erstelle DuplicateBusinessObject für einzelne Stückliste.
+
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :type server: APplusServer
     :param stueli: Stückliste, die kopiert werden soll.
     :type stueli: str
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :type cache: Optional[FieldsToCopyForTableCache]
     :return: das neue DuplicateBusinessObject
     :rtype: Optional[DuplicateBusinessObject]
     """
 
-    cache = initFieldsToCopyForTableCacheIfNeeded(server, cache);
+    cache = initFieldsToCopyForTableCacheIfNeeded(server, cache)
     boMain = loadDBDuplicateBusinessObjectSimpleCond(server, "stueli", "stueli", stueli, cache=cache)
     if boMain is None:
         return None
 
     for so in loadDBDuplicateBusinessObjectsSimpleCond(server, "stuelipos", "stueli", stueli, cache=cache):
         boMain.addDependentBusinessObject(so, ("stueli", "stueli"))
-    
+
     return boMain
 
+
 def addSachgruppeDependentObjects(
-        do : DuplicateBusinessObject, 
-        server : APplusServer, 
-        cache:Optional[FieldsToCopyForTableCache]=None) -> None:
+        do: DuplicateBusinessObject,
+        server: APplusServer,
+        cache: Optional[FieldsToCopyForTableCache] = None) -> None:
     """
     Fügt Unterobjekte hinzu, die die Sachgruppenwerte kopieren.
 
     :param do: zu erweiterndes DuplicateBusinessObject
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :type server: APplusServer
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :type cache: Optional[FieldsToCopyForTableCache]
     """
 
-    cache = initFieldsToCopyForTableCacheIfNeeded(server, cache);
+    cache = initFieldsToCopyForTableCacheIfNeeded(server, cache)
     klasse = do.fields.get(sql_utils.normaliseDBfield("SACHGRUPPENKLASSE"), None)
-    if (klasse == None):
+    if (klasse is None):
         # keine Klasse gesetzt, nichts zu kopieren
-        return 
+        return
 
     # bestimme alle Gruppen
     def loadGruppen() -> Sequence[str]:
         sql = sql_utils.SqlStatementSelect("sachgruppenklassepos", "sachgruppe")
         sql.where.addConditionFieldEq("sachgruppenklasse", klasse)
         sql.where.addConditionFieldEq("tabelle", do.table)
         return server.dbQueryAll(sql, apply=lambda r: r.sachgruppe)
 
-    gruppen = loadGruppen();
+    gruppen = loadGruppen()
 
     # Gruppe bearbeiten
     def processGruppen() -> None:
         cond = sql_utils.SqlConditionAnd()
         cond.addConditionFieldEq("tabelle", do.table)
         cond.addConditionFieldEq("instanzguid", do.getField("guid"))
         cond.addConditionFieldEq("sachgruppenklasse", klasse)
         cond.addConditionFieldIn("sachgruppe", gruppen)
         cond.addConditionFieldStringNotEmpty("wert")
 
         for so in loadDBDuplicateBusinessObjects(server, "sachwert", cond, cache=cache, allowUpdate=True):
             do.addDependentBusinessObject(so, ("guid", "instanzguid"))
 
-
     processGruppen()
-    
 
 
 def loadDBDuplicateArtikel(
-        server : APplusServer, 
-        artikel : str, 
-        cache:Optional[FieldsToCopyForTableCache]=None,
-        dupAplan:bool=True, 
-        dupStueli:bool=True) -> Optional[DuplicateBusinessObject]:
+        server: APplusServer,
+        artikel: str,
+        cache: Optional[FieldsToCopyForTableCache] = None,
+        dupAplan: bool = True,
+        dupStueli: bool = True) -> Optional[DuplicateBusinessObject]:
 
     """
-    Erstelle DuplicateBusinessObject für einzelnen Artikel. 
-    
+    Erstelle DuplicateBusinessObject für einzelnen Artikel.
+
     :param server: Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder
     :type server: APplusServer
     :param artikel: Artikel, der kopiert werden soll
     :type artikel: str
-    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen 
+    :param cache: Cache, so dass benötigte Felder nicht immer wieder neu berechnet werden müssen
     :type cache: Optional[FieldsToCopyForTableCache]
     :param dupAplan: Arbeitsplan duplizieren?
     :type dupAplan: bool optional
     :param dupStueli: Stückliste duplizieren?
     :type dupStueli: bool optional
     :return: das neue DuplicateBusinessObject
     :rtype: DuplicateBusinessObject
     """
 
-    cache = initFieldsToCopyForTableCacheIfNeeded(server, cache);
+    cache = initFieldsToCopyForTableCacheIfNeeded(server, cache)
     boArt = loadDBDuplicateBusinessObjectSimpleCond(server, "artikel", "ARTIKEL", artikel, cache=cache)
     if boArt is None:
         return None
     addSachgruppeDependentObjects(boArt, server, cache=cache)
 
     if dupAplan:
         boAplan = loadDBDuplicateAPlan(server, artikel, cache=cache)
         boArt.addDependentBusinessObject(boAplan, ("artikel", "aplan"))
-    
+
     if dupStueli:
         boStueli = loadDBDuplicateStueli(server, artikel, cache=cache)
         boArt.addDependentBusinessObject(boStueli, ("artikel", "stueli"))
 
     return boArt
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/pandas.py` & `PyAPplus64-1.0.1/src/PyAPplus64/pandas.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,128 +4,125 @@
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
 """Pandas Interface für PyAPplus64."""
 
-from typing import Annotated as Ann
-import pandas as pd # type: ignore
-from pandas._typing import AggFuncType, FilePath, WriteExcelBuffer # type: ignore
+import pandas as pd    # type: ignore
+from pandas._typing import AggFuncType, FilePath, WriteExcelBuffer    # type: ignore
 import sqlalchemy
 import traceback
 from .applus import APplusServer
 from .applus import sql_utils
-from typing import *
+from typing import Optional, Callable, Sequence, Tuple, Any, Union
 
 
-def createSqlAlchemyEngine(server : APplusServer) -> sqlalchemy.Engine:
+def createSqlAlchemyEngine(server: APplusServer) -> sqlalchemy.Engine:
     """Erzeugt eine SqlAlchemy-Engine für die Verbindung zur DB."""
     return sqlalchemy.create_engine(sqlalchemy.engine.URL.create("mssql+pyodbc", query={"odbc_connect": server.db_settings.getConnectionString()}))
 
 
 def pandasReadSql(
-        server : APplusServer, 
-        sql : sql_utils.SqlStatement, 
-        raw:bool=False, 
-        engine:Optional[sqlalchemy.Engine]=None) -> pd.DataFrame:    
+        server: APplusServer,
+        sql: sql_utils.SqlStatement,
+        raw: bool = False,
+        engine: Optional[sqlalchemy.Engine] = None) -> pd.DataFrame:
     """Wrapper für pd.read_sql für sqlalchemy-engine.
-    
+
     :param server: APplusServer für Datenbankverbindung und complete-SQL
     :type server: APplusServer
     :param sql: das SQL-statement
     """
 
     if engine is None:
-        engine = createSqlAlchemyEngine(server);
+        engine = createSqlAlchemyEngine(server)
     with engine.connect() as conn:
         return pd.read_sql(sqlalchemy.text(server.completeSQL(sql, raw=raw)), conn)
 
 
-def _createHyperLinkGeneral(genOrg : Callable[[], str|int|float], genLink: Callable[[], str]) -> str|int|float:
+def _createHyperLinkGeneral(genOrg: Callable[[], Union[str, int, float]], genLink: Callable[[], str]) -> Union[str, int, float]:
     """
     Hilfsfunktion zum Generieren eines Excel-Links.
-    
-    :param genLink: Funktion, die  Parameter aufgerufen wird und einen Link generiert    
+
+    :param genLink: Funktion, die  Parameter aufgerufen wird und einen Link generiert
     """
-    org:str|int|float=""
-    org2:str|int|float
-    try:           
-        org = genOrg();
+    org: Union[str, int, float] = ""
+    org2: Union[str, int, float]
+    try:
+        org = genOrg()
         if not org:
             return org
-        else :
+        else:
             if isinstance(org, (int, float)):
-                org2 = org;
+                org2 = org
             else:
-                org2 = "\""  + str(org).replace("\"", "\"\"") + "\""
+                org2 = "\"" + str(org).replace("\"", "\"\"") + "\""
 
             return "=HYPERLINK(\"{}\", {})".format(genLink(), org2)
     except:
-        msg = traceback.format_exc();
-        print ("Exception: {}".format(msg))
+        msg = traceback.format_exc()
+        print("Exception: {}".format(msg))
         return org
 
 
-def mkDataframeColumn(df : pd.DataFrame, makeValue : AggFuncType) -> pd.Series:    
+def mkDataframeColumn(df: pd.DataFrame, makeValue: AggFuncType) -> pd.Series:
     """
     Erzeugt für alle Zeilen eines Dataframes eine neuen Wert. Dies wird benutzt, um eine Spalte zu berechnen.
     Diese kann eine Originalspalte ersetzen, oder neu hinzugefügt werden.
-    
+
     :param df: der Dataframe
     :param makeValue: Funktion, die eine Zeile als Parameter bekommt und den neuen Wert berechnet
     """
-    def mkValueWrapper(r): # type: ignore
+    def mkValueWrapper(r):  # type: ignore
         try:
             return makeValue(r)
         except:
-            msg = traceback.format_exc();
-            print ("Exception: {}".format(msg))
+            msg = traceback.format_exc()
+            print("Exception: {}".format(msg))
             return ""
 
     if (len(df.index) > 0):
         return df.apply(mkValueWrapper, axis=1)
     else:
-        return df.apply(lambda r: "", axis=1);
+        return df.apply(lambda r: "", axis=1)
 
 
-def mkHyperlinkDataframeColumn(df : pd.DataFrame, makeOrig : AggFuncType, makeLink : Callable[[Any], str]) -> pd.Series :    
+def mkHyperlinkDataframeColumn(df: pd.DataFrame, makeOrig: AggFuncType, makeLink: Callable[[Any], str]) -> pd.Series:
     """
     Erzeugt für alle Zeilen eines Dataframes einen Hyperlink. Dies wird benutzt, um eine Spalte mit einem Hyperlink zu berechnen.
     Diese kann eine Originalspalte ersetzen, oder neu hinzugefügt werden.
-    
+
     :param df: der Dataframe
     :param makeOrig: Funktion, die eine Zeile als Parameter bekommt und den Wert berechnet, der angezeigt werden soll
     :param makeLink: Funktion, die eine Zeile als Parameter bekommt und den Link berechnet
     """
     if (len(df.index) > 0):
-        return df.apply(lambda r: _createHyperLinkGeneral(lambda : makeOrig(r), lambda : makeLink(r)), axis=1)
+        return df.apply(lambda r: _createHyperLinkGeneral(lambda: makeOrig(r), lambda: makeLink(r)), axis=1)
     else:
-        return df.apply(lambda r: "", axis=1);
+        return df.apply(lambda r: "", axis=1)
 
 
 def exportToExcel(
-        filename:FilePath | WriteExcelBuffer | pd.ExcelWriter, 
-        dfs : Sequence[Tuple[pd.DataFrame, str]], 
-        addTable:bool=True) -> None:
+        filename: Union[FilePath, WriteExcelBuffer, pd.ExcelWriter],
+        dfs: Sequence[Tuple[pd.DataFrame, str]],
+        addTable: bool = True) -> None:
     """
     Schreibt eine Menge von Dataframes in eine Excel-Tabelle
-    
-    :param filename: Name der Excel-Datei 
+
+    :param filename: Name der Excel-Datei
     :param dfs: Liste von Tupeln aus DataFrames und Namen von Sheets.
     """
-    with pd.ExcelWriter(filename, engine='xlsxwriter') as writer:  
+    with pd.ExcelWriter(filename, engine='xlsxwriter') as writer:
         for (df, name) in dfs:
             df.to_excel(writer, sheet_name=name, index=False, header=True)
             ws = writer.sheets[name]
 
             # Table
             if addTable:
                 (max_row, max_col) = df.shape
                 if max_row > 0 and max_col > 0:
                     column_settings = [{'header': column} for column in df.columns]
                     ws.add_table(0, 0, max_row, max_col - 1, {'columns': column_settings})
 
             # Spaltenbreiten anpassen
-            ws.autofit();
-
-
+            ws.autofit()
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/sql_utils.py` & `PyAPplus64-1.0.1/src/PyAPplus64/sql_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
 """
 Diese Datei enthält Funktionen für den Bau von SQL Statements, besonders
 SELECT-Statements. Es gibt viel ausgefeiltere Methoden für die Erstellung von
 SQL Statements. APplus benötigt jedoch die Statements als Strings, die dann an
 APplus für Änderungen und erst danach an die DB geschickt werden. Dies erschwert
 die Nutzung von Tools wie SqlAlchemy.
 
@@ -18,317 +17,338 @@
 gestellt. PyODBC erlaubt Parameter (dargestellt als '?') in SQL Statements, die
 dann beim Aufruf gefüllt werden. Dies funktioniert auch im Zusammenspiel mit
 APplus. Oft ist es sinnvoll, solche Parameter zu verwenden.
 """
 
 from __future__ import annotations
 import datetime
-from typing import *
+from typing import Set, Sequence, Union, Optional, cast, List
 
-def normaliseDBfield(f : str) -> str:
+
+def normaliseDBfield(f: str) -> str:
     """Normalisiert die Darstellung eines DB-Feldes"""
-    return str(f).upper();
+    return str(f).upper()
+
 
-def normaliseDBfieldSet(s : Set[str]) -> Set[str]:
+def normaliseDBfieldSet(s: Set[str]) -> Set[str]:
     """Normalisiert eine Menge von DB-Feldern"""
     return {normaliseDBfield(f) for f in s}
 
-def normaliseDBfieldList(l : Sequence[str]) -> Sequence[str]:
+
+def normaliseDBfieldList(fields: Sequence[str]) -> Sequence[str]:
     """Normalisiert eine Menge von DB-Feldern"""
-    return [normaliseDBfield(f) for f in l]
+    return [normaliseDBfield(f) for f in fields]
 
 
 class SqlField():
     """
     Wrapper um SQL Feldnamen, die die Formatierung erleichtern
-    
+
     :param fn: der Feldname
     :type fn: str
     """
-    def __init__(self, fn : str):
-        self.field = normaliseDBfield(fn);
+    def __init__(self, fn: str):
+        self.field = normaliseDBfield(fn)
 
     def __str__(self) -> str:
-        return self.field;
+        return self.field
+
 
 class SqlFixed():
     """
     Wrapper um Strings, die ohne Änderung in SQL übernommen werden
-    
+
     :param s: der string
     :type s: str
     """
-    def __init__(self, s : str):
-        self.s = str(s);
+    def __init__(self, s: str):
+        self.s = str(s)
 
     def __str__(self) -> str:
-        return self.s;
+        return self.s
+
 
 class SqlDateTime():
     """
     Wrapper um DateTime, die die Formatierung erleichtern
 
     :param dt: der Zeitpunkt
     :type dt: Union[datetime.datetime, datetime.date]
     """
-    def __init__(self, dt:Union[datetime.datetime, datetime.date]=datetime.datetime.now()) -> None:        
-        self.value = dt;
+    def __init__(self, dt: Union[datetime.datetime, datetime.date] = datetime.datetime.now()) -> None:
+        self.value = dt
 
     def __str__(self) -> str:
-        # %f formatiert mit 6 Stellen, also microseconds. Es werden aber nur 
+        # %f formatiert mit 6 Stellen, also microseconds. Es werden aber nur
         # 3 Stellen unterstützt, daher werden 3 weggeworfen.
         return self.value.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3]
 
+
 class SqlDate():
     """
     Wrapper um DateTime, die die Formatierung erleichtern
 
     :param d: das Datum
     :type d: Union[datetime.datetime, datetime.date]
     """
-    def __init__(self, d:Union[datetime.datetime, datetime.date]=datetime.datetime.now()) -> None:        
-        self.value = d;
+    def __init__(self, d: Union[datetime.datetime, datetime.date] = datetime.datetime.now()) -> None:
+        self.value = d
 
     def __str__(self) -> str:
-        return self.value.strftime("%Y%m%d");
+        return self.value.strftime("%Y%m%d")
+
 
 class SqlTime():
     """
     Wrapper um DateTime, die die Formatierung erleichtern
 
     :param t: die Zeit
     :type t: Union[datetime.datetime, datetime.time]
     """
-    def __init__(self, t:Union[datetime.datetime, datetime.time]=datetime.datetime.now()) -> None:        
+    def __init__(self, t: Union[datetime.datetime, datetime.time] = datetime.datetime.now()) -> None:
         self.value = t
 
     def __str__(self) -> str:
         return self.value.strftime("%H:%M:%S.%f")[:-3]
 
+
 class SqlParam():
     """Hilfsklasse, für einen Parameter (?)"""
     def __init__(self) -> None:
-        pass 
+        pass
 
     def __str__(self) -> str:
         return "?"
 
+
 sqlParam = SqlParam()
 """Da SqlParam keinen Zustand hat, reicht ein einzelner statischer Wert"""
 
-def formatSqlValueString(s:str) -> str:
+
+def formatSqlValueString(s: str) -> str:
     """
-    Formatiert einen String für ein Sql-Statement. Der String wird in "'" eingeschlossen 
+    Formatiert einen String für ein Sql-Statement. Der String wird in "'" eingeschlossen
     und Hochkomma im Text maskiert.
 
     :param s: der String
     :type s: str
     :return: der formatierte String
     :rtype: str
     """
 
-    if (s is None): 
-        return "''";
+    if (s is None):
+        return "''"
 
-    return "'" + str(s).replace("'", "''") + "'";
+    return "'" + str(s).replace("'", "''") + "'"
 
 
-SqlValue : TypeAlias = Union[str, int, float, SqlParam, SqlField, SqlFixed, SqlDate, SqlDateTime, datetime.datetime, datetime.date, datetime.time]
+SqlValue = Union[str, int, float, SqlParam, SqlField, SqlFixed, SqlDate, SqlDateTime, datetime.datetime, datetime.date, datetime.time]
 """Union-Type aller unterstützter SQL-Werte"""
 
-def formatSqlValue(v : SqlValue) -> str:
+
+def formatSqlValue(v: SqlValue) -> str:
     """
     Formatiert einen Wert für SQL. Je nachdem um welchen Typ es sich handelt, werden andere Formatierungen verwendet.
 
     :param v: der Wert
     :type v: SqlValue
     :return: der formatierte Wert
     :rtype: str
     """
 
-    if (v == None):
-        raise Exception("formatSqlValue: null not supported");
+    if v is None:
+        raise Exception("formatSqlValue: null not supported")
 
     if isinstance(v, (int, float, SqlField)):
-        return str(v);
+        return str(v)
     elif isinstance(v, str):
-        return formatSqlValueString(v);
+        return formatSqlValueString(v)
     elif isinstance(v, datetime.datetime):
-        return "'" + str(SqlDateTime(v)) + "'";
+        return "'" + str(SqlDateTime(v)) + "'"
     elif isinstance(v, datetime.date):
-        return "'" + str(SqlDate(v)) + "'";
+        return "'" + str(SqlDate(v)) + "'"
     elif isinstance(v, datetime.time):
-        return "'" + str(SqlTime(v)) + "'";
+        return "'" + str(SqlTime(v)) + "'"
     elif isinstance(v, (SqlDateTime, SqlDate, SqlTime)):
-        return "'" + str(v) + "'";
+        return "'" + str(v) + "'"
     elif isinstance(v, (SqlParam, SqlFixed)):
-        return str(v);
+        return str(v)
     else:
-        raise Exception("formatSqlValue: unsupported type {}".format(type(v)));
+        raise Exception("formatSqlValue: unsupported type {}".format(type(v)))
+
 
 class SqlCondition():
     """Eine abstrakte Sql-Bedingung. Unterklassen erledigen die eigentliche Arbeit."""
-    
+
     def getCondition(self) -> str:
         """
         Liefert die Bedingung als String
-        
-        :return: die Bedingung 
+
+        :return: die Bedingung
         :rtype: str
-        """ 
-        raise Exception("Not implemented");
+        """
+        raise Exception("Not implemented")
 
     def __str__(self) -> str:
-        return self.getCondition();
+        return self.getCondition()
 
 
 class SqlConditionPrepared(SqlCondition):
     """Eine einfache Sql-Bedingung, die immer einen festen String zurückgibt."""
 
-    def __init__(self, cond : Union[SqlCondition, str]):
-        self.cond = str(cond);
+    def __init__(self, cond: Union[SqlCondition, str]):
+        self.cond = str(cond)
 
     def getCondition(self) -> str:
-        return self.cond;
+        return self.cond
+
 
 class SqlConditionTrue(SqlConditionPrepared):
     """True-Bedingung"""
 
     def __init__(self) -> None:
         super().__init__("(1=1)")
 
+
 class SqlConditionFalse(SqlConditionPrepared):
     """False-Bedingung"""
 
     def __init__(self) -> None:
         super().__init__("(1=0)")
 
+
 class SqlConditionBool(SqlConditionPrepared):
     """Fixe True-oder-False Bedingung"""
 
-    def __init__(self, b : bool):
+    def __init__(self, b: bool):
         if b:
             super().__init__(SqlConditionTrue())
         else:
             super().__init__(SqlConditionFalse())
 
+
 class SqlConditionNot(SqlCondition):
     """
     Negation einer anderen Bedingung
 
     :param cond: die zu negierende Bedingung
-    :type cond: SqlCondition    
+    :type cond: SqlCondition
     """
 
-    def __init__(self, cond : SqlCondition):
-        self.cond = cond;
+    def __init__(self, cond: SqlCondition):
+        self.cond = cond
 
     def getCondition(self) -> str:
-        return "(not {})".format(self.cond.getCondition());
+        return "(not {})".format(self.cond.getCondition())
 
 
 class SqlConditionIsNull(SqlConditionPrepared):
     """
     Wert soll null sein
 
     :param v: das Feld
     :type v: SqlValue
     """
 
-    def __init__(self, v : SqlValue):
+    def __init__(self, v: SqlValue):
         super().__init__("({} is null)".format(formatSqlValue(v)))
 
+
 class SqlConditionFieldIsNull(SqlConditionIsNull):
-    def __init__(self, field : str):
+    def __init__(self, field: str):
         super().__init__(SqlField(field))
 
+
 class SqlConditionIsNotNull(SqlConditionPrepared):
     """
     Wert soll nicht null sein
 
     :param v: der Wert
     :type v: SqlValue
     """
 
-    def __init__(self, v : SqlValue):
+    def __init__(self, v: SqlValue):
         super().__init__("({} is not null)".format(formatSqlValue(v)))
 
+
 class SqlConditionFieldIsNotNull(SqlConditionIsNotNull):
-    def __init__(self, field : str):
+    def __init__(self, field: str):
         super().__init__(SqlField(field))
-    
+
+
 class SqlConditionStringStartsWith(SqlConditionPrepared):
     """
     Feld soll mit einem bestimmten String beginnen
 
     :param field: das Feld
     :type field: str
     :param value: der Wert
     :type value: str
     """
 
-    def __init__(self, field : str, value : str):
-        cond = "";
+    def __init__(self, field: str, value: str):
+        cond = ""
         if value:
-            cond="(left({}, {}) = {})".format(normaliseDBfield(field), len(value), formatSqlValueString(value));
+            cond = "(left({}, {}) = {})".format(normaliseDBfield(field), len(value), formatSqlValueString(value))
         else:
-            cond = "(1=1)"        
+            cond = "(1=1)"
         super().__init__(cond)
 
 
 class SqlConditionFieldStringNotEmpty(SqlConditionPrepared):
     """
     Feld soll nicht den leeren String oder null enthalten.
     Der Ausdruck wird wörtlich übernommen.
 
     :param field: das Feld
     :type field: str
     """
 
-    def __init__(self, field : str):
-        field = normaliseDBfield(field);
-        cond="({} is not null and {} != '')".format(field, field);
+    def __init__(self, field: str):
+        field = normaliseDBfield(field)
+        cond = "({} is not null and {} != '')".format(field, field)
         super().__init__(cond)
 
 
 class SqlConditionIn(SqlConditionPrepared):
-    """    
+    """
     Bedingung der Form 'v in ...'
 
-    :param value: der Wert, kann unterschiedliche Typen besitzen    
+    :param value: der Wert, kann unterschiedliche Typen besitzen
     :type value: SqlValue
     :param values: die erlaubten Werte
     :type values: Sequence[SqlValue]
     """
-    def __init__(self, value : SqlValue, values : Sequence[SqlValue]):
+    def __init__(self, value: SqlValue, values: Sequence[SqlValue]):
         valuesLen = len(values)
-        if (valuesLen == 0):            
-            cond : Union[SqlCondition, str] = SqlConditionFalse()
+        if (valuesLen == 0):
+            cond: Union[SqlCondition, str] = SqlConditionFalse()
         elif (valuesLen == 1):
             cond = SqlConditionEq(value, values[0])
         else:
             valuesS = formatSqlValue(values[0])
             for i in range(1, valuesLen):
                 valuesS += ", " + formatSqlValue(values[i])
             cond = "({} in ({}))".format(formatSqlValue(value), valuesS)
         super().__init__(cond)
- 
+
+
 class SqlConditionFieldIn(SqlConditionIn):
-    def __init__(self, field:str, values : Sequence[SqlValue]):
+    def __init__(self, field: str, values: Sequence[SqlValue]):
         super().__init__(SqlField(field), values)
 
 
 class SqlConditionEq(SqlConditionPrepared):
-    """    
+    """
     Bedingung der Form 'v1 is null', 'v2 is null', 'v1 = v2', '(1=1)' oder '(0=1)'
 
-    :param value1: der Wert, kann unterschiedliche Typen besitzen    
-    :param value2: der Wert, kann unterschiedliche Typen besitzen    
+    :param value1: der Wert, kann unterschiedliche Typen besitzen
+    :param value2: der Wert, kann unterschiedliche Typen besitzen
     """
-    def __init__(self, value1 : Optional[Union[SqlValue, bool]], value2 : Optional[Union[SqlValue, bool]]):
+    def __init__(self, value1: Union[SqlValue, bool, None], value2: Union[SqlValue, bool, None]):
         cond: Union[SqlCondition, str]
         if (value1 is None) and (value2 is None):
             cond = SqlConditionTrue()
         elif (value1 is None) and not (value2 is None):
             if (isinstance(value2, bool)):
                 cond = SqlConditionFalse()
             else:
@@ -336,478 +356,494 @@
         elif not (value1 is None) and (value2 is None):
             if (isinstance(value1, bool)):
                 cond = SqlConditionFalse()
             else:
                 cond = SqlConditionIsNull(value1)
         else:
             if isinstance(value1, bool) and isinstance(value2, bool):
-                cond = SqlConditionBool(value1 == value2);
+                cond = SqlConditionBool(value1 == value2)
             elif isinstance(value1, bool) and not isinstance(value2, bool):
                 value2 = cast(SqlValue, value2)
                 if value1:
                     cond = "({} = 1)".format(formatSqlValue(value2))
                 else:
-                    cond = "({} = 0 OR {} is null)".format(formatSqlValue(value2), formatSqlValue(value2));
+                    cond = "({} = 0 OR {} is null)".format(formatSqlValue(value2), formatSqlValue(value2))
             elif not isinstance(value1, bool) and isinstance(value2, bool):
                 value1 = cast(SqlValue, value1)
                 if value2:
                     cond = "({} = 1)".format(formatSqlValue(value1))
                 else:
                     cond = "({} = 0 OR {} is null)".format(formatSqlValue(value1), formatSqlValue(value1))
             else:
                 value1 = cast(SqlValue, value1)
                 value2 = cast(SqlValue, value2)
-                cond = "({} = {})".format(formatSqlValue(value1), formatSqlValue(value2));
+                cond = "({} = {})".format(formatSqlValue(value1), formatSqlValue(value2))
         super().__init__(cond)
 
 
 class SqlConditionBinComp(SqlConditionPrepared):
-    """    
+    """
     Bedingung der Form 'value1 op value2'
 
     :param op: der Vergleichsoperator
     :type op: str
-    :param value1: der Wert, kann unterschiedliche Typen besitzen    
+    :param value1: der Wert, kann unterschiedliche Typen besitzen
     :type value1: SqlValue
-    :param value2: der Wert, kann unterschiedliche Typen besitzen    
+    :param value2: der Wert, kann unterschiedliche Typen besitzen
     :type value2: SqlValue
     """
-    def __init__(self, op : str, value1 : SqlValue, value2 : SqlValue):
-        if not(value1) or not(value2):
+    def __init__(self, op: str, value1: SqlValue, value2: SqlValue):
+        if not value1 or not value2:
             raise Exception("SqlConditionBinComp: value not provided")
 
-        cond = "({} {} {})".format(formatSqlValue(value1), op, formatSqlValue(value2));
+        cond = "({} {} {})".format(formatSqlValue(value1), op, formatSqlValue(value2))
         super().__init__(cond)
 
 
 class SqlConditionLt(SqlConditionBinComp):
-    """    
+    """
     Bedingung der Form 'value1 < value2'
 
-    :param value1: der Wert, kann unterschiedliche Typen besitzen    
-    :param value2: der Wert, kann unterschiedliche Typen besitzen    
+    :param value1: der Wert, kann unterschiedliche Typen besitzen
+    :param value2: der Wert, kann unterschiedliche Typen besitzen
     """
-    def __init__(self, value1 : SqlValue, value2 : SqlValue):
-       super().__init__("<", value1, value2)
+    def __init__(self, value1: SqlValue, value2: SqlValue):
+        super().__init__("<", value1, value2)
+
 
 class SqlConditionLe(SqlConditionBinComp):
-    """    
+    """
     Bedingung der Form 'value1 <= value2'
 
-    :param value1: der Wert, kann unterschiedliche Typen besitzen    
-    :param value2: der Wert, kann unterschiedliche Typen besitzen    
+    :param value1: der Wert, kann unterschiedliche Typen besitzen
+    :param value2: der Wert, kann unterschiedliche Typen besitzen
     """
-    def __init__(self, value1 : SqlValue, value2 : SqlValue):
-       super().__init__("<=", value1, value2)
+    def __init__(self, value1: SqlValue, value2: SqlValue):
+        super().__init__("<=", value1, value2)
+
 
 class SqlConditionGt(SqlConditionBinComp):
-    """    
+    """
     Bedingung der Form 'value1 > value2'
 
-    :param value1: der Wert, kann unterschiedliche Typen besitzen    
-    :param value2: der Wert, kann unterschiedliche Typen besitzen    
+    :param value1: der Wert, kann unterschiedliche Typen besitzen
+    :param value2: der Wert, kann unterschiedliche Typen besitzen
     """
-    def __init__(self, value1 : SqlValue, value2 : SqlValue):
-       super().__init__(">", value1, value2)
+    def __init__(self, value1: SqlValue, value2: SqlValue):
+        super().__init__(">", value1, value2)
+
 
 class SqlConditionGe(SqlConditionBinComp):
-    """    
+    """
     Bedingung der Form 'value1 >= value2'
 
-    :param value1: der Wert, kann unterschiedliche Typen besitzen    
-    :param value2: der Wert, kann unterschiedliche Typen besitzen    
+    :param value1: der Wert, kann unterschiedliche Typen besitzen
+    :param value2: der Wert, kann unterschiedliche Typen besitzen
     """
-    def __init__(self, value1 : SqlValue, value2 : SqlValue):
-       super().__init__(">=", value1, value2)
+    def __init__(self, value1: SqlValue, value2: SqlValue):
+        super().__init__(">=", value1, value2)
 
 
 class SqlConditionFieldEq(SqlConditionEq):
-    def __init__(self, field : str, value : Optional[Union[SqlValue, bool]]):
+    def __init__(self, field: str, value: Union[SqlValue, bool, None]):
         super().__init__(SqlField(field), value)
 
+
 class SqlConditionFieldLt(SqlConditionLt):
-    def __init__(self, field : str, value : SqlValue):
+    def __init__(self, field: str, value: SqlValue):
         super().__init__(SqlField(field), value)
 
+
 class SqlConditionFieldLe(SqlConditionLe):
-    def __init__(self, field : str, value : SqlValue):
+    def __init__(self, field: str, value: SqlValue):
         super().__init__(SqlField(field), value)
 
+
 class SqlConditionFieldGt(SqlConditionGt):
-    def __init__(self, field : str, value : SqlValue):
+    def __init__(self, field: str, value: SqlValue):
         super().__init__(SqlField(field), value)
 
+
 class SqlConditionFieldGe(SqlConditionGe):
-    def __init__(self, field : str, value : SqlValue):
+    def __init__(self, field: str, value: SqlValue):
         super().__init__(SqlField(field), value)
-  
+
+
 class SqlConditionList(SqlCondition):
     """
     Eine SQL Bedingung, die sich aus einer Liste anderer Bedingungen zusammensetzen.
     Dies kann eine "AND" oder eine "OR" Liste sein.
-    
+
     :param connector: wie werden Listenelemente verbunden (AND oder OR)
-    :type connector: str 
+    :type connector: str
     :param emptyCond: Rückgabewert für leere Liste
     :type emptyCond: str
     """
 
-    def __init__(self, connector : str, emptyCond : str):
-        self.connector : str = connector;
-        self.emptyCond : str = emptyCond;
-        self.elems : List[SqlCondition] = []
-    
-    def addCondition(self, cond : SqlCondition | str | None) -> None:
+    def __init__(self, connector: str, emptyCond: str):
+        self.connector: str = connector
+        self.emptyCond: str = emptyCond
+        self.elems: List[SqlCondition] = []
+
+    def addCondition(self, cond: Union[SqlCondition, str, None]) -> None:
         if (cond is None):
             return
         if not (isinstance(cond, SqlCondition)):
-            cond = SqlConditionPrepared("("+str(cond)+")");
-        self.elems.append(cond);
+            cond = SqlConditionPrepared("("+str(cond)+")")
+        self.elems.append(cond)
 
-    def addConditions(self, *conds : SqlCondition | str | None) -> None:
+    def addConditions(self, *conds: Union[SqlCondition, str, None]) -> None:
         for cond in conds:
             self.addCondition(cond)
 
-    def addConditionFieldStringNotEmpty(self, field : str) -> None:
-        self.addCondition(SqlConditionFieldStringNotEmpty(field));
+    def addConditionFieldStringNotEmpty(self, field: str) -> None:
+        self.addCondition(SqlConditionFieldStringNotEmpty(field))
 
-    def addConditionFieldIn(self, field : str, values : Sequence[SqlValue]) -> None:
-        self.addCondition(SqlConditionFieldIn(field, values));
+    def addConditionFieldIn(self, field: str, values: Sequence[SqlValue]) -> None:
+        self.addCondition(SqlConditionFieldIn(field, values))
 
-    def addConditionFieldEq(self, field : str, value : Optional[Union[SqlValue, bool]]) -> None:
-        self.addCondition(SqlConditionFieldEq(field, value));
+    def addConditionFieldEq(self, field: str, value: Union[SqlValue, bool, None]) -> None:
+        self.addCondition(SqlConditionFieldEq(field, value))
 
-    def addConditionFieldsEq(self, field1 : str, field2 : str) -> None:
-        self.addCondition(SqlConditionEq(SqlField(field1), SqlField(field2)));
+    def addConditionFieldsEq(self, field1: str, field2: str) -> None:
+        self.addCondition(SqlConditionEq(SqlField(field1), SqlField(field2)))
 
-    def addConditionEq(self, value1 : Optional[Union[SqlValue, bool]], value2 : Optional[Union[SqlValue, bool]]) -> None:
-        self.addCondition(SqlConditionEq(value1, value2));
+    def addConditionEq(self, value1: Union[SqlValue, bool, None], value2: Union[SqlValue, bool, None]) -> None:
+        self.addCondition(SqlConditionEq(value1, value2))
 
-    def addConditionGe(self, value1 : SqlValue, value2 : SqlValue) -> None:
-        self.addCondition(SqlConditionGe(value1, value2));
+    def addConditionGe(self, value1: SqlValue, value2: SqlValue) -> None:
+        self.addCondition(SqlConditionGe(value1, value2))
 
-    def addConditionFieldGe(self, field : str, value : SqlValue) -> None:
-        self.addCondition(SqlConditionGe(SqlField(field), value));
+    def addConditionFieldGe(self, field: str, value: SqlValue) -> None:
+        self.addCondition(SqlConditionGe(SqlField(field), value))
 
-    def addConditionFieldsGe(self, field1 : str, field2 : str) -> None:
-        self.addCondition(SqlConditionGe(SqlField(field1), SqlField(field2)));
+    def addConditionFieldsGe(self, field1: str, field2: str) -> None:
+        self.addCondition(SqlConditionGe(SqlField(field1), SqlField(field2)))
 
-    def addConditionLe(self, value1 : SqlValue, value2 : SqlValue) -> None:
-        self.addCondition(SqlConditionLe(value1, value2));
+    def addConditionLe(self, value1: SqlValue, value2: SqlValue) -> None:
+        self.addCondition(SqlConditionLe(value1, value2))
 
-    def addConditionFieldLe(self, field : str, value : SqlValue) -> None:
-        self.addCondition(SqlConditionLe(SqlField(field), value));
+    def addConditionFieldLe(self, field: str, value: SqlValue) -> None:
+        self.addCondition(SqlConditionLe(SqlField(field), value))
 
-    def addConditionFieldsLe(self, field1 : str, field2 : str) -> None:
-        self.addCondition(SqlConditionLe(SqlField(field1), SqlField(field2)));
+    def addConditionFieldsLe(self, field1: str, field2: str) -> None:
+        self.addCondition(SqlConditionLe(SqlField(field1), SqlField(field2)))
 
-    def addConditionGt(self, value1 : SqlValue, value2 : SqlValue) -> None:
-        self.addCondition(SqlConditionGt(value1, value2));
+    def addConditionGt(self, value1: SqlValue, value2: SqlValue) -> None:
+        self.addCondition(SqlConditionGt(value1, value2))
 
-    def addConditionFieldGt(self, field : str, value : SqlValue) -> None:
-        self.addCondition(SqlConditionGt(SqlField(field), value));
+    def addConditionFieldGt(self, field: str, value: SqlValue) -> None:
+        self.addCondition(SqlConditionGt(SqlField(field), value))
 
-    def addConditionFieldsGt(self, field1 : str, field2 : str) -> None:
-        self.addCondition(SqlConditionGt(SqlField(field1), SqlField(field2)));
+    def addConditionFieldsGt(self, field1: str, field2: str) -> None:
+        self.addCondition(SqlConditionGt(SqlField(field1), SqlField(field2)))
 
-    def addConditionLt(self, value1 : SqlValue, value2 : SqlValue) -> None:
-        self.addCondition(SqlConditionLt(value1, value2));
+    def addConditionLt(self, value1: SqlValue, value2: SqlValue) -> None:
+        self.addCondition(SqlConditionLt(value1, value2))
 
-    def addConditionFieldLt(self, field : str, value : SqlValue) -> None:
-        self.addCondition(SqlConditionLt(SqlField(field), value));
+    def addConditionFieldLt(self, field: str, value: SqlValue) -> None:
+        self.addCondition(SqlConditionLt(SqlField(field), value))
 
-    def addConditionFieldsLt(self, field1 : str, field2 : str) -> None:
-        self.addCondition(SqlConditionLt(SqlField(field1), SqlField(field2)));
+    def addConditionFieldsLt(self, field1: str, field2: str) -> None:
+        self.addCondition(SqlConditionLt(SqlField(field1), SqlField(field2)))
 
-    def addConditionFieldIsNull(self, field : str) -> None:
-        self.addCondition(SqlConditionFieldIsNull(field));
+    def addConditionFieldIsNull(self, field: str) -> None:
+        self.addCondition(SqlConditionFieldIsNull(field))
 
-    def addConditionFieldIsNotNull(self, field : str) -> None:
-        self.addCondition(SqlConditionFieldIsNotNull(field));
+    def addConditionFieldIsNotNull(self, field: str) -> None:
+        self.addCondition(SqlConditionFieldIsNotNull(field))
 
     def isEmpty(self) -> bool:
-        return not(self.elems);
+        return not self.elems
 
     def getCondition(self) -> str:
-        match (len(self.elems)):
-            case 0:
-                return self.emptyCond;
-            case 1:
-                return self.elems[0].getCondition();
-            case l:
-                res = "(" + self.elems[0].getCondition();
-                for i in range(1, l):
-                    res += " {} {}".format(self.connector, self.elems[i].getCondition())
-                res += ")";
-                return res;
+        elemLen = len(self.elems)
+        if elemLen == 0:
+            return self.emptyCond
+        elif elemLen == 1:
+            return self.elems[0].getCondition()
+        else:
+            res = "(" + self.elems[0].getCondition()
+            for i in range(1, elemLen):
+                res += " {} {}".format(self.connector, self.elems[i].getCondition())
+            res += ")"
+            return res
 
 
 class SqlConditionDateTimeFieldInRange(SqlConditionPrepared):
-    """    
+    """
     Liegt Datetime in einem bestimmten Zeitraum?
 
     :param field: das Feld
     :type field: str
     :param datetimeVon: der untere Wert (einschließlich), None erlaubt beliebige Zeiten
     :param datetimeBis: der obere Wert (ausschließlich), None erlaubt beliebige Zeiten
     """
-    def __init__(self, field : str, datetimeVon : datetime.datetime|None, datetimeBis : datetime.datetime|None):
+    def __init__(self, field: str, datetimeVon: Optional[datetime.datetime], datetimeBis: Optional[datetime.datetime]):
         cond = SqlConditionAnd()
         if not (datetimeVon is None):
             cond.addConditionFieldGe(field, datetimeVon)
         if not (datetimeBis is None):
             cond.addConditionFieldLt(field, datetimeBis)
         super().__init__(str(cond))
 
+
 class SqlConditionDateTimeFieldInMonth(SqlConditionPrepared):
-    """    
+    """
     Liegt Datetime in einem bestimmten Monat?
 
     :param field: das Feld
     :type field: string
     :param year: das Jahr
     :param month: der Monat
     """
-    def __init__(self, field : str, year : int, month : int):
+    def __init__(self, field: str, year: int, month: int):
         if month == 12:
-            nyear=year+1
-            nmonth=1;
+            nyear = year+1
+            nmonth = 1
         else:
-            nyear=year
-            nmonth=month+1;
-        cond = SqlConditionDateTimeFieldInRange(field, 
-                  datetime.datetime(year=year, month=month, day=1), 
-                  datetime.datetime(year=nyear, month=nmonth, day=1))
+            nyear = year
+            nmonth = month+1
+        cond = SqlConditionDateTimeFieldInRange(
+                   field,
+                   datetime.datetime(year=year, month=month, day=1),
+                   datetime.datetime(year=nyear, month=nmonth, day=1))
         super().__init__(str(cond))
 
+
 class SqlConditionDateTimeFieldInYear(SqlConditionPrepared):
-    """    
+    """
     Liegt Datetime in einem bestimmten Jahr?
 
     :param field: das Feld
     :type field: str
     :param year: das Jahr
     """
-    def __init__(self, field : str, year :int) -> None:
-        nyear=year+1
-        cond = SqlConditionDateTimeFieldInRange(field, 
-                  datetime.datetime(year=year, month=1, day=1), 
-                  datetime.datetime(year=nyear, month=1, day=1))
+    def __init__(self, field: str, year: int) -> None:
+        nyear = year+1
+        cond = SqlConditionDateTimeFieldInRange(
+                   field,
+                   datetime.datetime(year=year, month=1, day=1),
+                   datetime.datetime(year=nyear, month=1, day=1))
         super().__init__(str(cond))
 
+
 class SqlConditionDateTimeFieldInDay(SqlConditionPrepared):
-    """    
+    """
     Liegt Datetime in einem bestimmten Monat?
 
     :param field: das Feld
     :type field: str
     :param year: das Jahr
     :param month: der Monat
     :param day: der Tag
     """
-    def __init__(self, field : str, year : int, month : int, day : int) -> None:
+    def __init__(self, field: str, year: int, month: int, day: int) -> None:
         d = datetime.datetime(year=year, month=month, day=day)
-        cond = SqlConditionDateTimeFieldInRange(field, 
-                d,
-                d + datetime.timedelta(days=1))
+        cond = SqlConditionDateTimeFieldInRange(
+                   field,
+                   d,
+                   d + datetime.timedelta(days=1))
         super().__init__(str(cond))
 
+
 class SqlConditionAnd(SqlConditionList):
-    def __init__(self, *conds : Union[SqlCondition, str]) -> None:
+    def __init__(self, *conds: Union[SqlCondition, str]) -> None:
         super().__init__("AND", "(1=1)")
         self.addConditions(*conds)
 
+
 class SqlConditionOr(SqlConditionList):
-    def __init__(self, *conds : Union[SqlCondition, str]) -> None:
+    def __init__(self, *conds: Union[SqlCondition, str]) -> None:
         super().__init__("OR", "(1=0)")
         self.addConditions(*conds)
 
 
 class SqlJoin():
     """
     Ein abstrakter Sql-Join
 
     :param joinType: Art des Joins, wird in SQL übernommen, z.B. "LEFT JOIN".
     :type joinType: str
     :param table: die Tabelle, die gejoint werden soll
     :type table: str
     :param conds: Bedingungen, die bereits hinzugefügt werden soll. Weitere können über Attribut `on` hinzugefügt werden.
-    
+
     """
-    
-    def __init__(self, joinType : str, table : str, *conds : Union[SqlCondition, str]) -> None:       
+
+    def __init__(self, joinType: str, table: str, *conds: Union[SqlCondition, str]) -> None:
         self.joinType = joinType
         self.table = table
 
-        self.on : SqlConditionAnd = SqlConditionAnd(*conds)
+        self.on: SqlConditionAnd = SqlConditionAnd(*conds)
         """Bedingung des Joins, kann noch nachträglich erweitert werden"""
-        
+
     def getJoin(self) -> str:
         """
-        Liefert den Join als String       
-        """ 
-        return self.joinType + " " + self.table + " ON " + self.on.getCondition();
+        Liefert den Join als String
+        """
+        return self.joinType + " " + self.table + " ON " + self.on.getCondition()
 
     def __str__(self) -> str:
-        return self.getJoin();
+        return self.getJoin()
 
 
 class SqlInnerJoin(SqlJoin):
     """
     Ein Inner-Join.
 
     :param table: die Tabelle, die gejoint werden soll
     :type table: str
     :param conds: Bedingungen, die bereits hinzugefügt werden soll. Weitere können über Attribut `on` hinzugefügt werden.
     """
 
-    def __init__(self, table : str, *conds : Union[SqlCondition, str]) -> None:
+    def __init__(self, table: str, *conds: Union[SqlCondition, str]) -> None:
         super().__init__("INNER JOIN", table, *conds)
 
+
 class SqlLeftJoin(SqlJoin):
     """
     Ein Left-Join.
 
     :param table: die Tabelle, die gejoint werden soll
     :type table: str
     :param conds: Bedingungen, die bereits hinzugefügt werden soll. Weitere können über Attribut `on` hinzugefügt werden.
     """
-    def __init__(self, table : str, *conds : Union[SqlCondition, str]) -> None:
+    def __init__(self, table: str, *conds: Union[SqlCondition, str]) -> None:
         super().__init__("LEFT JOIN", table, *conds)
 
+
 class SqlStatementSelect():
     """
     Klasse, um einfache Select-Statements zu bauen.
 
     :param table: die Haupt-Tabelle
     :type table: str
-    :param fields: kein oder mehrere Felder, die selektiert werden sollen    
+    :param fields: kein oder mehrere Felder, die selektiert werden sollen
     """
 
-    def __init__(self, table : str, *fields : str) -> None:
-        self.table : str = table
+    def __init__(self, table: str, *fields: str) -> None:
+        self.table: str = table
         """die Tabelle"""
-        
-        self.top : int = 0
+
+        self.top: int = 0
         """wie viele Datensätze auswählen? 0 für alle"""
 
-        self.where : SqlConditionList = SqlConditionAnd();
+        self.where: SqlConditionList = SqlConditionAnd()
         """die Bedingung, Default ist True"""
 
-        self.fields : List[str] = []        
+        self.fields: List[str] = []
         """Liste von auszuwählenden Feldern"""
         self.addFields(*fields)
 
-        self.joins : List[SqlJoin|str] = []
+        self.joins: List[Union[SqlJoin, str]] = []
         """Joins mit extra Tabellen"""
 
-        self.groupBy : List[str] = [];
+        self.groupBy: List[str] = []
         """die Bedingung, Default ist True"""
 
-        self.having : SqlConditionList = SqlConditionAnd();
+        self.having: SqlConditionList = SqlConditionAnd()
         """die Bedingung having, Default ist True"""
 
-        self.order : Optional[str] = None
+        self.order: Optional[str] = None
         """Sortierung"""
 
     def __str__(self) -> str:
-        return self.getSql();
+        return self.getSql()
 
-    def addFields(self, *fields : str) -> None:
+    def addFields(self, *fields: str) -> None:
         """Fügt ein oder mehrere Felder, also auszuwählende Werte zu einem SQL-Statement hinzu."""
         for f in fields:
-            if not (f == None):
+            if not (f is None):
                 self.fields.append(f)
 
-    def addGroupBy(self, *fields : str) -> None:
+    def addGroupBy(self, *fields: str) -> None:
         """Fügt ein oder mehrere GroupBy Felder zu einem SQL-Statement hinzu."""
         for f in fields:
-            if not (f == None):
+            if not (f is None):
                 self.groupBy.append(f)
 
-    def setTop(self, t : int) -> None:
+    def setTop(self, t: int) -> None:
         """Wie viele Datensätze sollen maximal zurückgeliefert werden? 0 für alle"""
         self.top = t
 
-    def addFieldsTable(self, table : str, *fields : str) -> None:
+    def addFieldsTable(self, table: str, *fields: str) -> None:
         """
         Fügt ein oder mehrere Felder, die zu einer Tabelle gehören zu einem SQL-Statement hinzu.
         Felder sind Strings. Vor jeden dieser Strings wird die Tabelle mit einem Punkt getrennt gesetzt.
         Dies kann im Vergleich zu 'addFields' Schreibarbeit erleitern.
         """
         for f in fields:
-            if not (f == None):
+            if not (f is None):
                 self.fields.append(table + "." + str(f))
 
-    def addJoin(self, j : SqlJoin|str) -> None:
+    def addJoin(self, j: Union[SqlJoin, str]) -> None:
         """Fügt ein Join zum SQL-Statement hinzu. Beispiel: 'LEFT JOIN personal p ON t.UPDUSER = p.PERSONAL'"""
         self.joins.append(j)
 
-    def addLeftJoin(self, table : str, *conds : Union[SqlCondition, str]) -> SqlLeftJoin:
+    def addLeftJoin(self, table: str, *conds: Union[SqlCondition, str]) -> SqlLeftJoin:
         j = SqlLeftJoin(table, *conds)
         self.addJoin(j)
         return j
 
-    def addInnerJoin(self, table : str, *conds : Union[SqlCondition, str]) ->  SqlInnerJoin:
+    def addInnerJoin(self, table: str, *conds: Union[SqlCondition, str]) -> SqlInnerJoin:
         j = SqlInnerJoin(table, *conds)
         self.addJoin(j)
         return j
 
     def getSql(self) -> str:
         """Liefert das SQL-SELECT-Statement als String"""
         def getFields() -> str:
-            match (len(self.fields)):
-                case 0:
-                    return "*";
-                case 1:
-                    return str(self.fields[0]);
-                case l:
-                    res = str(self.fields[0]);
-                    for i in range(1, l):
-                        res += ", " + str(self.fields[i]);
-                    return res;
+            fieldsLen = len(self.fields)
+            if fieldsLen == 0:
+                return "*"
+            elif fieldsLen == 1:
+                return str(self.fields[0])
+            else:
+                res = str(self.fields[0])
+                for i in range(1, fieldsLen):
+                    res += ", " + str(self.fields[i])
+                return res
 
         def getGroupBy() -> str:
-            match (len(self.groupBy)):
-                case 0:
-                    return "";
-                case l:
-                    res = " GROUP BY " + str(self.fields[0])
-                    for i in range(1, l):
-                        res += ", " + str(self.fields[i]);
-                    if not (self.having.isEmpty()): 
-                        res += " HAVING " + str(self.having)                    
-                    return res;
+            groupByLen = len(self.groupBy)
+            if groupByLen == 0:
+                return ""
+            else:
+                res = " GROUP BY " + str(self.fields[0])
+                for i in range(1, groupByLen):
+                    res += ", " + str(self.fields[i])
+                if not (self.having.isEmpty()):
+                    res += " HAVING " + str(self.having)
+                return res
 
         def getJoins() -> str:
-            match (len(self.joins)):
-                case 0:
-                    return ""
-                case l:
-                    res = "";
-                    for i in range(0, l):
-                        res += " " + str(self.joins[i])
-                    return res
+            if (len(self.joins) == 0):
+                return ""
+            else:
+                res = ""
+                for i in range(0, len(self.joins)):
+                    res += " " + str(self.joins[i])
+                return res
 
         def getWhere() -> str:
-            if self.where.isEmpty(): 
+            if self.where.isEmpty():
                 return ""
             else:
                 return " WHERE " + str(self.where)
 
         def getOrder() -> str:
-            if self.order == None:
+            if self.order is None:
                 return ""
             else:
                 return " ORDER BY " + str(self.order)
-        
+
         def getTop() -> str:
             if self.top <= 0:
                 return ""
             else:
                 return "TOP " + str(self.top) + " "
 
-        return "SELECT " + getTop() + getFields() + " FROM " + self.table + getJoins() + getWhere() + getGroupBy() + getOrder();
-
+        return "SELECT " + getTop() + getFields() + " FROM " + self.table + getJoins() + getWhere() + getGroupBy() + getOrder()
 
-SqlStatement : TypeAlias = Union [SqlStatementSelect, str]
 
+SqlStatement = Union[SqlStatementSelect, str]
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64/utils.py` & `PyAPplus64-1.0.1/src/PyAPplus64/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,55 +2,55 @@
 #
 # This file is part of PyAPplus64 (see https://www.thomas-tuerk.de/de/pyapplus64).
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
-#-*- coding: utf-8 -*-
-
 import pathlib
 import datetime
-from typing import *
+from typing import Set, Union
+
 
-def checkDirExists(dir : Union[str, pathlib.Path]) -> pathlib.Path:    
+def checkDirExists(dir: Union[str, pathlib.Path]) -> pathlib.Path:
     """Prüft, ob ein Verzeichnis existiert. Ist dies nicht möglich, wird eine Exception geworfen.
 
     :param dir: das Verzeichnis
     :type dir: Union[str, pathlib.Path]
     :return: den normalisierten Pfad
     :rtype: pathlib.Path
     """
 
     if not (isinstance(dir, pathlib.Path)):
         dir = pathlib.Path(str(dir))
 
     dir = dir.resolve()
     if not (dir.exists()):
-        raise Exception("Verzeichnis '" + str(dir) + "' nicht gefunden");
-        
+        raise Exception("Verzeichnis '" + str(dir) + "' nicht gefunden")
+
     if not (dir.is_dir()):
-        raise Exception("'" + str(dir) + "' ist kein Verzeichnis");
-    return dir;
+        raise Exception("'" + str(dir) + "' ist kein Verzeichnis")
+    return dir
 
 
-def formatDateTimeForAPplus(v : Union[datetime.datetime, datetime.date, datetime.time]) -> str:
+def formatDateTimeForAPplus(v: Union[datetime.datetime, datetime.date, datetime.time]) -> str:
     """Formatiert ein Datum oder eine Uhrzeit für APplus"""
-    if (v == None):
-        return "";
+    if v is None:
+        return ""
     elif isinstance(v, str):
-        return v;
+        return v
     elif isinstance(v, datetime.datetime):
         return v.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
     elif isinstance(v, datetime.date):
         return v.strftime("%Y-%m-%d")
     elif isinstance(v, datetime.time):
         return v.strftime("%H:%M:%S.%f")[:-3]
     else:
         return str(v)
-   
-def containsOnlyAllowedChars(charset : Set[str], s : str) -> bool:
+
+
+def containsOnlyAllowedChars(charset: Set[str], s: str) -> bool:
     """Enthält ein String nur erlaubte Zeichen?"""
     for c in s:
-        if not (c in charset): 
+        if not (c in charset):
             return False
     return True
```

### Comparing `PyAPplus64-1.0.0/src/PyAPplus64.egg-info/SOURCES.txt` & `PyAPplus64-1.0.1/src/PyAPplus64.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.0/tests/test_sql_utils.py` & `PyAPplus64-1.0.1/tests/test_sql_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,292 +5,358 @@
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
 from PyAPplus64 import sql_utils
 import datetime
 
-def test_normaliseDBField1() -> None:    
+
+def test_normaliseDBField1() -> None:
     assert (sql_utils.normaliseDBfield("aAa") == "AAA")
     assert (sql_utils.normaliseDBfield("a#Aa") == "A#AA")
     assert (sql_utils.normaliseDBfield("2") == "2")
 
-def test_normaliseDBFieldSet() -> None:    
+
+def test_normaliseDBFieldSet() -> None:
     assert (sql_utils.normaliseDBfieldSet(set()) == set())
     assert (sql_utils.normaliseDBfieldSet({"aAa", "b", "c", "2"}) == {"2", "AAA", "B", "C"})
 
-def test_normaliseDBFieldList() -> None:    
+
+def test_normaliseDBFieldList() -> None:
     assert (sql_utils.normaliseDBfieldList([]) == [])
     assert (sql_utils.normaliseDBfieldList(["aAa", "b", "c", "2"]) == ["AAA", "B", "C", "2"])
 
+
 def test_SqlField1() -> None:
     assert (str(sql_utils.SqlField("abc")) == "ABC")
 
+
 def test_SqlField2() -> None:
     assert (str(sql_utils.SqlField("t.abc")) == "T.ABC")
 
+
 def test_SqlParam() -> None:
     assert (str(sql_utils.sqlParam) == "?")
 
+
 def test_SqlDateTime() -> None:
     dt = datetime.datetime(year=2023, month=1, day=12, hour=9, minute=59, second=12, microsecond=2344)
     assert (str(sql_utils.SqlDateTime(dt)) == "2023-01-12T09:59:12.002")
 
+
 def test_SqlDate() -> None:
     dt = datetime.datetime(year=2023, month=1, day=12, hour=9, minute=59, second=12, microsecond=2344)
     assert (str(sql_utils.SqlDate(dt)) == "20230112")
 
+
 def test_formatSqlValueString1() -> None:
-    assert(sql_utils.formatSqlValueString("") == "''");
+    assert (sql_utils.formatSqlValueString("") == "''")
+
 
 def test_formatSqlValueString2() -> None:
-    assert(sql_utils.formatSqlValueString("abc") == "'abc'");
+    assert (sql_utils.formatSqlValueString("abc") == "'abc'")
+
 
 def test_formatSqlValueString3() -> None:
-    assert(sql_utils.formatSqlValueString("a b c") == "'a b c'");
+    assert (sql_utils.formatSqlValueString("a b c") == "'a b c'")
+
 
 def test_formatSqlValueString4() -> None:
-    assert(sql_utils.formatSqlValueString("a \"b\" c") == "'a \"b\" c'");    
+    assert (sql_utils.formatSqlValueString("a \"b\" c") == "'a \"b\" c'")
+
 
 def test_formatSqlValueString5() -> None:
-    assert(sql_utils.formatSqlValueString("a 'b'\nc") == "'a ''b''\nc'");        
+    assert (sql_utils.formatSqlValueString("a 'b'\nc") == "'a ''b''\nc'")
+
 
 def test_formatSqlValue1() -> None:
-    assert(sql_utils.formatSqlValue(2) == "2");        
+    assert (sql_utils.formatSqlValue(2) == "2")
+
 
 def test_formatSqlValue2() -> None:
-    assert(sql_utils.formatSqlValue(2.4) == "2.4");        
+    assert (sql_utils.formatSqlValue(2.4) == "2.4")
+
 
 def test_formatSqlValue3() -> None:
-    assert(sql_utils.formatSqlValue("AA") == "'AA'");        
+    assert (sql_utils.formatSqlValue("AA") == "'AA'")
+
 
 def test_formatSqlValue4() -> None:
-    assert(sql_utils.formatSqlValue(sql_utils.SqlField("aa")) == "AA");        
+    assert (sql_utils.formatSqlValue(sql_utils.SqlField("aa")) == "AA")
+
 
 def test_formatSqlValue5() -> None:
-    assert(sql_utils.formatSqlValue(0) == "0");        
+    assert (sql_utils.formatSqlValue(0) == "0")
+
 
 def test_formatSqlValue6() -> None:
     dt = datetime.datetime(year=2023, month=1, day=12, hour=9, minute=59, second=12, microsecond=2344)
-    assert(sql_utils.formatSqlValue(sql_utils.SqlDateTime(dt)) == "'2023-01-12T09:59:12.002'");        
+    assert (sql_utils.formatSqlValue(sql_utils.SqlDateTime(dt)) == "'2023-01-12T09:59:12.002'")
+
 
 def test_SqlConditionTrue() -> None:
-    assert(str(sql_utils.SqlConditionTrue()) == "(1=1)");            
+    assert (str(sql_utils.SqlConditionTrue()) == "(1=1)")
+
 
 def test_SqlConditionFalse() -> None:
-    assert(str(sql_utils.SqlConditionFalse()) == "(1=0)");                
+    assert (str(sql_utils.SqlConditionFalse()) == "(1=0)")
+
 
 def test_SqlConditionBool1() -> None:
-    assert(str(sql_utils.SqlConditionBool(True)) == "(1=1)");            
+    assert (str(sql_utils.SqlConditionBool(True)) == "(1=1)")
+
 
 def test_SqlConditionBool2() -> None:
-    assert(str(sql_utils.SqlConditionBool(False)) == "(1=0)");            
+    assert (str(sql_utils.SqlConditionBool(False)) == "(1=0)")
+
 
 def test_SqlConditionIsNull() -> None:
-    cond = sql_utils.SqlConditionIsNull("AA");
-    assert(str(cond) == "('AA' is null)");                
+    cond = sql_utils.SqlConditionIsNull("AA")
+    assert (str(cond) == "('AA' is null)")
+
 
 def test_SqlConditionIsNotNull() -> None:
-    cond = sql_utils.SqlConditionIsNotNull("AA");
-    assert(str(cond) == "('AA' is not null)");                
+    cond = sql_utils.SqlConditionIsNotNull("AA")
+    assert (str(cond) == "('AA' is not null)")
+
 
 def test_SqlConditionNot() -> None:
-    cond1 = sql_utils.SqlConditionIsNull("AA");
-    cond = sql_utils.SqlConditionNot(cond1);
-    assert(str(cond) == "(not ('AA' is null))");                
+    cond1 = sql_utils.SqlConditionIsNull("AA")
+    cond = sql_utils.SqlConditionNot(cond1)
+    assert (str(cond) == "(not ('AA' is null))")
+
 
 def test_SqlConditionStringStartsWith() -> None:
     cond = sql_utils.SqlConditionStringStartsWith("f", "a'an")
-    assert(str(cond) == "(left(F, 4) = 'a''an')");                
+    assert (str(cond) == "(left(F, 4) = 'a''an')")
+
 
 def test_SqlConditionIn1() -> None:
     cond = sql_utils.SqlConditionIn(sql_utils.SqlField("f"), [])
-    assert(str(cond) == "(1=0)");                
+    assert (str(cond) == "(1=0)")
+
 
 def test_SqlConditionIn2() -> None:
     cond = sql_utils.SqlConditionIn(sql_utils.SqlField("f"), ["a"])
-    assert(str(cond) == "(F = 'a')");                
+    assert (str(cond) == "(F = 'a')")
+
 
 def test_SqlConditionIn3() -> None:
     cond = sql_utils.SqlConditionIn(sql_utils.SqlField("f"), ["a", "a'A", "b", "c"])
-    assert(str(cond) == "(F in ('a', 'a''A', 'b', 'c'))");                
+    assert (str(cond) == "(F in ('a', 'a''A', 'b', 'c'))")
+
 
 def test_SqlConditionStringNotEmpty1() -> None:
     cond = sql_utils.SqlConditionFieldStringNotEmpty("f")
-    assert(str(cond) == "(F is not null and F != '')");                
+    assert (str(cond) == "(F is not null and F != '')")
+
 
 def test_SqlConditionEq1() -> None:
     cond = sql_utils.SqlConditionEq("f1", None)
-    assert(str(cond) == "('f1' is null)");                
+    assert (str(cond) == "('f1' is null)")
+
 
 def test_SqlConditionEq2() -> None:
     cond = sql_utils.SqlConditionEq(None, "f1")
-    assert(str(cond) == "('f1' is null)");                
+    assert (str(cond) == "('f1' is null)")
+
 
 def test_SqlConditionEq3() -> None:
     cond = sql_utils.SqlConditionEq(sql_utils.SqlField("f1"), sql_utils.SqlField("f2"))
-    assert(str(cond) == "(F1 = F2)");                
+    assert (str(cond) == "(F1 = F2)")
+
 
 def test_SqlConditionEq4() -> None:
     cond = sql_utils.SqlConditionEq(sql_utils.SqlField("f1"), "aa'a")
-    assert(str(cond) == "(F1 = 'aa''a')");                
+    assert (str(cond) == "(F1 = 'aa''a')")
+
 
 def test_SqlConditionEq5() -> None:
     cond = sql_utils.SqlConditionEq(sql_utils.SqlField("f1"), 2)
-    assert(str(cond) == "(F1 = 2)");                
+    assert (str(cond) == "(F1 = 2)")
+
 
 def test_SqlConditionEq6() -> None:
     cond = sql_utils.SqlConditionEq(sql_utils.SqlField("f1"), True)
-    assert(str(cond) == "(F1 = 1)");                
+    assert (str(cond) == "(F1 = 1)")
+
 
 def test_SqlConditionEq7() -> None:
     cond = sql_utils.SqlConditionEq(sql_utils.SqlField("f1"), False)
-    assert(str(cond) == "(F1 = 0 OR F1 is null)");                
+    assert (str(cond) == "(F1 = 0 OR F1 is null)")
+
 
 def test_SqlConditionEq8() -> None:
     cond = sql_utils.SqlConditionEq(True, sql_utils.SqlField("f1"))
-    assert(str(cond) == "(F1 = 1)");                
+    assert (str(cond) == "(F1 = 1)")
+
 
 def test_SqlConditionEq9() -> None:
     cond = sql_utils.SqlConditionEq(False, sql_utils.SqlField("f1"))
-    assert(str(cond) == "(F1 = 0 OR F1 is null)");                
+    assert (str(cond) == "(F1 = 0 OR F1 is null)")
+
 
 def test_SqlConditionEq10() -> None:
     cond = sql_utils.SqlConditionEq(False, True)
-    assert(str(cond) == "(1=0)");                
+    assert (str(cond) == "(1=0)")
+
 
 def test_SqlConditionEq11() -> None:
     cond = sql_utils.SqlConditionEq(True, True)
-    assert(str(cond) == "(1=1)");                
+    assert (str(cond) == "(1=1)")
+
 
 def test_SqlConditionFieldEq1() -> None:
     cond = sql_utils.SqlConditionFieldEq("f1", None)
-    assert(str(cond) == "(F1 is null)");                
+    assert (str(cond) == "(F1 is null)")
+
 
 def test_SqlConditionFieldEq2() -> None:
     cond = sql_utils.SqlConditionFieldEq("f1", sql_utils.SqlField("f2"))
-    assert(str(cond) == "(F1 = F2)");                
+    assert (str(cond) == "(F1 = F2)")
+
 
 def test_SqlConditionFieldEq3() -> None:
     cond = sql_utils.SqlConditionFieldEq("f1", "aa'a")
-    assert(str(cond) == "(F1 = 'aa''a')");                
+    assert (str(cond) == "(F1 = 'aa''a')")
+
 
 def test_SqlConditionFieldEq4() -> None:
     cond = sql_utils.SqlConditionFieldEq("f1", 2)
-    assert(str(cond) == "(F1 = 2)");                
+    assert (str(cond) == "(F1 = 2)")
+
 
 def test_SqlConditionFieldEq5() -> None:
     cond = sql_utils.SqlConditionFieldEq("f1", sql_utils.sqlParam)
-    assert(str(cond) == "(F1 = ?)");                
+    assert (str(cond) == "(F1 = ?)")
+
 
 def test_SqlConditionLt1() -> None:
     cond = sql_utils.SqlConditionLt(sql_utils.SqlField("f"), sql_utils.SqlDate(datetime.date(year=2022, month=12, day=12)))
-    assert(str(cond) == "(F < '20221212')");                
+    assert (str(cond) == "(F < '20221212')")
+
 
 def test_SqlConditionLt2() -> None:
     cond = sql_utils.SqlConditionLt(2, sql_utils.SqlField("f"))
-    assert(str(cond) == "(2 < F)");                
+    assert (str(cond) == "(2 < F)")
+
 
 def test_SqlConditionGt1() -> None:
     cond = sql_utils.SqlConditionGt(sql_utils.SqlField("f"), sql_utils.SqlDate(datetime.date(year=2022, month=12, day=12)))
-    assert(str(cond) == "(F > '20221212')");                
+    assert (str(cond) == "(F > '20221212')")
+
 
 def test_SqlConditionGt2() -> None:
     cond = sql_utils.SqlConditionGt(2, sql_utils.SqlField("f"))
-    assert(str(cond) == "(2 > F)");                
+    assert (str(cond) == "(2 > F)")
+
 
 def test_SqlConditionLe1() -> None:
     cond = sql_utils.SqlConditionLe(sql_utils.SqlField("f"), sql_utils.SqlDate(datetime.date(year=2022, month=12, day=12)))
-    assert(str(cond) == "(F <= '20221212')");                
+    assert (str(cond) == "(F <= '20221212')")
+
 
 def test_SqlConditionLe2() -> None:
     cond = sql_utils.SqlConditionLe(2, sql_utils.SqlField("f"))
-    assert(str(cond) == "(2 <= F)");                
+    assert (str(cond) == "(2 <= F)")
+
 
 def test_SqlConditionGe1() -> None:
     cond = sql_utils.SqlConditionGe(sql_utils.SqlField("f"), sql_utils.SqlDate(datetime.date(year=2022, month=12, day=12)))
-    assert(str(cond) == "(F >= '20221212')");                
+    assert (str(cond) == "(F >= '20221212')")
+
 
 def test_SqlConditionGe2() -> None:
     cond = sql_utils.SqlConditionGe(2, sql_utils.SqlField("f"))
-    assert(str(cond) == "(2 >= F)");                
+    assert (str(cond) == "(2 >= F)")
+
 
 def test_SqlConditionFieldLt1() -> None:
     cond = sql_utils.SqlConditionFieldLt("f", sql_utils.SqlDate(datetime.date(year=2022, month=12, day=12)))
-    assert(str(cond) == "(F < '20221212')");                
+    assert (str(cond) == "(F < '20221212')")
+
 
 def test_SqlConditionFieldLe1() -> None:
     cond = sql_utils.SqlConditionFieldLe("f", sql_utils.SqlDate(datetime.date(year=2022, month=12, day=12)))
-    assert(str(cond) == "(F <= '20221212')");                
+    assert (str(cond) == "(F <= '20221212')")
+
 
 def test_SqlConditionFieldGt1() -> None:
     cond = sql_utils.SqlConditionFieldGt("f", sql_utils.SqlDate(datetime.date(year=2022, month=12, day=12)))
-    assert(str(cond) == "(F > '20221212')");                
+    assert (str(cond) == "(F > '20221212')")
+
 
 def test_SqlConditionFieldGe1() -> None:
     cond = sql_utils.SqlConditionFieldGe("f", sql_utils.SqlDate(datetime.date(year=2022, month=12, day=12)))
-    assert(str(cond) == "(F >= '20221212')");                
+    assert (str(cond) == "(F >= '20221212')")
 
 
 def test_SqlConditionAnd1() -> None:
-    conj = sql_utils.SqlConditionAnd();
-    assert(str(conj) == "(1=1)");                
+    conj = sql_utils.SqlConditionAnd()
+    assert (str(conj) == "(1=1)")
+
 
 def test_SqlConditionAnd2() -> None:
-    cond1 = sql_utils.SqlConditionPrepared("cond1");
-    conj = sql_utils.SqlConditionAnd();
+    cond1 = sql_utils.SqlConditionPrepared("cond1")
+    conj = sql_utils.SqlConditionAnd()
     conj.addCondition(cond1)
-    assert(str(conj) == "cond1");     
+    assert (str(conj) == "cond1")
+
 
 def test_SqlConditionAnd3() -> None:
-    cond1 = sql_utils.SqlConditionPrepared("cond1");
-    cond2 = sql_utils.SqlConditionPrepared("cond2");
-    conj = sql_utils.SqlConditionAnd();
+    cond1 = sql_utils.SqlConditionPrepared("cond1")
+    cond2 = sql_utils.SqlConditionPrepared("cond2")
+    conj = sql_utils.SqlConditionAnd()
     conj.addCondition(cond1)
     conj.addCondition(cond2)
-    assert(str(conj) == "(cond1 AND cond2)");     
+    assert (str(conj) == "(cond1 AND cond2)")
+
 
 def test_SqlConditionAnd4() -> None:
-    cond1 = sql_utils.SqlConditionPrepared("cond1");
-    cond2 = sql_utils.SqlConditionPrepared("cond2");
-    cond3 = sql_utils.SqlConditionPrepared("cond3");
-    conj = sql_utils.SqlConditionAnd();
+    cond1 = sql_utils.SqlConditionPrepared("cond1")
+    cond2 = sql_utils.SqlConditionPrepared("cond2")
+    cond3 = sql_utils.SqlConditionPrepared("cond3")
+    conj = sql_utils.SqlConditionAnd()
     conj.addCondition(cond1)
     conj.addCondition(cond2)
     conj.addCondition(cond3)
-    assert(str(conj) == "(cond1 AND cond2 AND cond3)");     
+    assert (str(conj) == "(cond1 AND cond2 AND cond3)")
 
 
 def test_SqlConditionOr1() -> None:
-    conj = sql_utils.SqlConditionOr();
-    assert(str(conj) == "(1=0)");                
+    conj = sql_utils.SqlConditionOr()
+    assert (str(conj) == "(1=0)")
+
 
 def test_SqlConditionOr2() -> None:
-    cond1 = sql_utils.SqlConditionPrepared("cond1");
-    conj = sql_utils.SqlConditionOr();
+    cond1 = sql_utils.SqlConditionPrepared("cond1")
+    conj = sql_utils.SqlConditionOr()
     conj.addCondition(cond1)
-    assert(str(conj) == "cond1");     
+    assert (str(conj) == "cond1")
+
 
 def test_SqlConditionOr3() -> None:
-    cond1 = sql_utils.SqlConditionPrepared("cond1");
-    cond2 = sql_utils.SqlConditionPrepared("cond2");
-    conj = sql_utils.SqlConditionOr();
+    cond1 = sql_utils.SqlConditionPrepared("cond1")
+    cond2 = sql_utils.SqlConditionPrepared("cond2")
+    conj = sql_utils.SqlConditionOr()
     conj.addCondition(cond1)
     conj.addCondition(cond2)
-    assert(str(conj) == "(cond1 OR cond2)");     
+    assert (str(conj) == "(cond1 OR cond2)")
+
 
 def test_SqlConditionOr4() -> None:
-    cond1 = sql_utils.SqlConditionPrepared("cond1");
-    cond2 = sql_utils.SqlConditionPrepared("cond2");
-    cond3 = sql_utils.SqlConditionPrepared("cond3");
-    conj = sql_utils.SqlConditionOr();
+    cond1 = sql_utils.SqlConditionPrepared("cond1")
+    cond2 = sql_utils.SqlConditionPrepared("cond2")
+    cond3 = sql_utils.SqlConditionPrepared("cond3")
+    conj = sql_utils.SqlConditionOr()
     conj.addCondition(cond1)
     conj.addCondition(cond2)
     conj.addCondition(cond3)
-    assert(str(conj) == "(cond1 OR cond2 OR cond3)");     
+    assert (str(conj) == "(cond1 OR cond2 OR cond3)")
+
 
 def test_SqlStatementSelect1() -> None:
     sql = sql_utils.SqlStatementSelect("tabelle t")
     assert (str(sql) == "SELECT * FROM tabelle t")
 
     sql.setTop(10)
     assert (str(sql) == "SELECT TOP 10 * FROM tabelle t")
@@ -319,33 +385,36 @@
     sql = sql_utils.SqlStatementSelect("t1")
     sql.addJoin("left join t2 on cond2")
     assert (str(sql) == "SELECT * FROM t1 left join t2 on cond2")
 
     sql.addJoin("left join t3 on cond3")
     assert (str(sql) == "SELECT * FROM t1 left join t2 on cond2 left join t3 on cond3")
 
+
 def test_SqlStatementSelect4() -> None:
     sql = sql_utils.SqlStatementSelect("t")
     sql.where.addCondition("cond1")
     assert (str(sql) == "SELECT * FROM t WHERE (cond1)")
 
     sql.where.addCondition("cond2")
     assert (str(sql) == "SELECT * FROM t WHERE ((cond1) AND (cond2))")
 
+
 def test_SqlStatementSelect5() -> None:
     sql = sql_utils.SqlStatementSelect("t")
-    cond = sql_utils.SqlConditionOr();
+    cond = sql_utils.SqlConditionOr()
     sql.where.addCondition(cond)
     cond.addCondition("cond1")
     assert (str(sql) == "SELECT * FROM t WHERE (cond1)")
 
     cond.addCondition("cond2")
     assert (str(sql) == "SELECT * FROM t WHERE ((cond1) OR (cond2))")
 
+
 def test_SqlStatementSelect6() -> None:
     sql = sql_utils.SqlStatementSelect("t")
-    sql.where = sql_utils.SqlConditionOr();
+    sql.where = sql_utils.SqlConditionOr()
     sql.where.addCondition("cond1")
     assert (str(sql) == "SELECT * FROM t WHERE (cond1)")
 
     sql.where.addCondition("cond2")
     assert (str(sql) == "SELECT * FROM t WHERE ((cond1) OR (cond2))")
```

