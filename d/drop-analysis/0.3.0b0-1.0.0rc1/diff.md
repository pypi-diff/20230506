# Comparing `tmp/drop_analysis-0.3.0b0.tar.gz` & `tmp/drop-analysis-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drop_analysis-0.3.0b0.tar", last modified: Tue Feb 15 09:42:46 2022, max compression
+gzip compressed data, was "drop-analysis-1.0.0rc1.tar", last modified: Fri May  5 21:25:18 2023, max compression
```

## Comparing `drop_analysis-0.3.0b0.tar` & `drop-analysis-1.0.0rc1.tar`

### file list

```diff
@@ -1,53 +1,74 @@
-drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2022-02-15 09:42:46.490011 drop_analysis-0.3.0b0/
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     1098 2022-01-16 15:07:59.000000 drop_analysis-0.3.0b0/.gitignore
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    35141 2018-11-24 15:33:18.000000 drop_analysis-0.3.0b0/LICENSE
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      375 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/MANIFEST.in
-drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2022-02-15 09:42:46.380012 drop_analysis-0.3.0b0/Old scripts/
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     6541 2020-09-28 20:44:26.000000 drop_analysis-0.3.0b0/Old scripts/GUI_sessile_drop_analysis.py
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     9848 2020-09-28 20:44:26.000000 drop_analysis-0.3.0b0/Old scripts/contact_angle_analysis_function.py
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     3334 2020-10-16 16:58:12.000000 drop_analysis-0.3.0b0/Old scripts/edge_detection.py
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     8681 2020-09-28 20:44:26.000000 drop_analysis-0.3.0b0/Old scripts/sessile_drop_analysis.py
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     4311 2022-02-15 09:42:46.490011 drop_analysis-0.3.0b0/PKG-INFO
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     3961 2022-01-26 23:55:33.000000 drop_analysis-0.3.0b0/README.md
-drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2022-02-15 09:42:46.380012 drop_analysis-0.3.0b0/Sample/
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)  2673786 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/Sample/Sample.avi
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)   210685 2020-10-10 23:32:47.000000 drop_analysis-0.3.0b0/Screenshot.png
-drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2022-02-15 09:42:46.428012 drop_analysis-0.3.0b0/docs/
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      634 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/docs/Makefile
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)     2336 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/docs/conf.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      273 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/docs/index.rst
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      760 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/docs/make.bat
-drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2022-02-15 09:42:46.480012 drop_analysis-0.3.0b0/drop_analysis/
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     9255 2022-01-19 22:24:23.000000 drop_analysis-0.3.0b0/drop_analysis/FrameSupply.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)    10169 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/Mainwindow.ui
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)     7504 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/Settings.ui
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)       46 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/__init__.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      264 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/__main__.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      207 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/config.toml
-drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2022-02-15 09:42:46.484012 drop_analysis-0.3.0b0/drop_analysis/data/
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      245 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/data/README.rst
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)        2 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/data/__init__.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)     1807 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/data/common_resolutions.csv
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)    68146 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/data/icon.ico
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)   194564 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/data/icon.xcf
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)     7259 2022-01-26 23:20:22.000000 drop_analysis-0.3.0b0/drop_analysis/edge_analysis.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)     3383 2022-01-16 14:43:30.000000 drop_analysis-0.3.0b0/drop_analysis/edge_detection.py
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    17705 2022-01-26 23:22:13.000000 drop_analysis-0.3.0b0/drop_analysis/gui.py
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)      817 2022-01-19 22:24:23.000000 drop_analysis-0.3.0b0/drop_analysis/otsu.py
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     6283 2022-01-26 23:17:12.000000 drop_analysis-0.3.0b0/drop_analysis/settings.py
-drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2022-02-15 09:42:46.490011 drop_analysis-0.3.0b0/drop_analysis/tests/
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)       44 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/drop_analysis/tests/__init__.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      347 2022-02-15 09:42:45.000000 drop_analysis-0.3.0b0/drop_analysis/version.py
-drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2022-02-15 09:42:46.480012 drop_analysis-0.3.0b0/drop_analysis.egg-info/
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     4311 2022-02-15 09:42:46.000000 drop_analysis-0.3.0b0/drop_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     1116 2022-02-15 09:42:46.000000 drop_analysis-0.3.0b0/drop_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)        1 2022-02-15 09:42:46.000000 drop_analysis-0.3.0b0/drop_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)       62 2022-02-15 09:42:46.000000 drop_analysis-0.3.0b0/drop_analysis.egg-info/entry_points.txt
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)        1 2022-01-20 22:40:58.000000 drop_analysis-0.3.0b0/drop_analysis.egg-info/not-zip-safe
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)      151 2022-02-15 09:42:46.000000 drop_analysis-0.3.0b0/drop_analysis.egg-info/requires.txt
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)       14 2022-02-15 09:42:46.000000 drop_analysis-0.3.0b0/drop_analysis.egg-info/top_level.txt
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)       79 2022-01-19 22:24:23.000000 drop_analysis-0.3.0b0/pyinst_entrypoint.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)      134 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/pyproject.toml
--rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     1541 2022-02-15 09:42:46.491011 drop_analysis-0.3.0b0/setup.cfg
--rwxrwxr-x   0 mathijs   (1000) mathijs   (1000)      600 2022-01-21 10:33:45.000000 drop_analysis-0.3.0b0/setup.py
--rw-r--r--   0 mathijs   (1000) mathijs   (1000)     1316 2021-04-13 22:39:14.000000 drop_analysis-0.3.0b0/tox.ini
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.648861 drop-analysis-1.0.0rc1/
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     1136 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/.gitignore
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    35141 2018-11-24 15:33:18.000000 drop-analysis-1.0.0rc1/LICENSE
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)      375 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/MANIFEST.in
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.644861 drop-analysis-1.0.0rc1/Old scripts/
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     6541 2020-09-28 20:44:26.000000 drop-analysis-1.0.0rc1/Old scripts/GUI_sessile_drop_analysis.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     9848 2020-09-28 20:44:26.000000 drop-analysis-1.0.0rc1/Old scripts/contact_angle_analysis_function.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     3334 2020-10-16 16:58:12.000000 drop-analysis-1.0.0rc1/Old scripts/edge_detection.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     8681 2020-09-28 20:44:26.000000 drop-analysis-1.0.0rc1/Old scripts/sessile_drop_analysis.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    45156 2023-05-05 21:25:18.649861 drop-analysis-1.0.0rc1/PKG-INFO
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     3981 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/README.md
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.644861 drop-analysis-1.0.0rc1/Sample/
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)  2673786 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/Sample/Sample.avi
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)   210685 2020-10-10 23:32:47.000000 drop-analysis-1.0.0rc1/Screenshot.png
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.646861 drop-analysis-1.0.0rc1/docs/
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)   117784 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/Analysis_running.png
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    40449 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/Camera_settings.png
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    30515 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/Edge_detection_setting.png
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    37814 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/Just_launched.png
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)      634 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/docs/Makefile
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    76399 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/Opened_video_file.png
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    77364 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/Placed_baseline.png
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    32724 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/Sessile_drop_settings.png
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    77728 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/Use_200_pixels.png
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.646861 drop-analysis-1.0.0rc1/docs/_static/
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    68146 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/_static/html_favicon.ico
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     3125 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/conf.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)      567 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/contact.md
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)      566 2023-03-26 21:54:50.000000 drop-analysis-1.0.0rc1/docs/contact.md.backup
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     1223 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/index.rst
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)      539 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/install.md
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)      760 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/docs/make.bat
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     7519 2023-03-26 23:14:24.000000 drop-analysis-1.0.0rc1/docs/usage.md
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     7519 2023-03-26 15:25:45.000000 drop-analysis-1.0.0rc1/docs/usage.md.backup
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.647861 drop-analysis-1.0.0rc1/drop_analysis/
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     7950 2023-03-27 19:24:53.000000 drop-analysis-1.0.0rc1/drop_analysis/About.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     9058 2023-03-27 19:24:45.000000 drop-analysis-1.0.0rc1/drop_analysis/About.ui
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     9255 2023-05-05 20:52:37.000000 drop-analysis-1.0.0rc1/drop_analysis/FrameSupply.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     3379 2023-03-27 14:37:16.000000 drop-analysis-1.0.0rc1/drop_analysis/Help.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     3313 2023-03-27 19:45:03.000000 drop-analysis-1.0.0rc1/drop_analysis/Help.ui
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    10616 2023-05-05 20:52:37.000000 drop-analysis-1.0.0rc1/drop_analysis/Mainwindow.ui
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)      245 2023-03-26 12:18:41.000000 drop-analysis-1.0.0rc1/drop_analysis/README.rst
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     7504 2023-05-05 20:52:37.000000 drop-analysis-1.0.0rc1/drop_analysis/Settings.ui
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)       46 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/drop_analysis/__init__.py
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)      264 2022-06-03 13:38:46.000000 drop-analysis-1.0.0rc1/drop_analysis/__main__.py
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)      207 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/drop_analysis/config.toml
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.648861 drop-analysis-1.0.0rc1/drop_analysis/data/
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)      245 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/drop_analysis/data/README.rst
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)        2 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/drop_analysis/data/__init__.py
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)     1807 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/drop_analysis/data/common_resolutions.csv
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)    68146 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/drop_analysis/data/icon.ico
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)   194564 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/drop_analysis/data/icon.xcf
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     8991 2023-03-26 23:15:29.000000 drop-analysis-1.0.0rc1/drop_analysis/edge_analysis.py
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)     3401 2023-03-27 14:44:25.000000 drop-analysis-1.0.0rc1/drop_analysis/edge_detection.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    20381 2023-05-05 20:52:37.000000 drop-analysis-1.0.0rc1/drop_analysis/gui.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     1254 2023-03-26 12:18:41.000000 drop-analysis-1.0.0rc1/drop_analysis/otsu.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     6283 2023-05-05 20:52:37.000000 drop-analysis-1.0.0rc1/drop_analysis/settings.py
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.648861 drop-analysis-1.0.0rc1/drop_analysis/tests/
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)       44 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/drop_analysis/tests/__init__.py
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)      348 2023-05-05 21:25:18.000000 drop-analysis-1.0.0rc1/drop_analysis/version.py
+drwxrwxr-x   0 mathijs   (1000) mathijs   (1000)        0 2023-05-05 21:25:18.648861 drop-analysis-1.0.0rc1/drop_analysis.egg-info/
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)    45156 2023-05-05 21:25:18.000000 drop-analysis-1.0.0rc1/drop_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     1586 2023-05-05 21:25:18.000000 drop-analysis-1.0.0rc1/drop_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)        1 2023-05-05 21:25:18.000000 drop-analysis-1.0.0rc1/drop_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)       62 2023-05-05 21:25:18.000000 drop-analysis-1.0.0rc1/drop_analysis.egg-info/entry_points.txt
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)        1 2022-01-20 22:40:58.000000 drop-analysis-1.0.0rc1/drop_analysis.egg-info/not-zip-safe
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)      151 2023-05-05 21:25:18.000000 drop-analysis-1.0.0rc1/drop_analysis.egg-info/requires.txt
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)       14 2023-05-05 21:25:18.000000 drop-analysis-1.0.0rc1/drop_analysis.egg-info/top_level.txt
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)       79 2022-01-19 22:24:23.000000 drop-analysis-1.0.0rc1/pyinst_entrypoint.py
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)      693 2023-03-08 23:49:53.000000 drop-analysis-1.0.0rc1/pynsist_installer.cfg
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)      693 2023-05-05 21:23:00.000000 drop-analysis-1.0.0rc1/pyproject.toml
+-rw-rw-r--   0 mathijs   (1000) mathijs   (1000)     1522 2023-05-05 21:25:18.649861 drop-analysis-1.0.0rc1/setup.cfg
+-rwxrwxr-x   0 mathijs   (1000) mathijs   (1000)      600 2022-01-21 10:33:45.000000 drop-analysis-1.0.0rc1/setup.py
+-rw-r--r--   0 mathijs   (1000) mathijs   (1000)     1316 2021-04-13 22:39:14.000000 drop-analysis-1.0.0rc1/tox.ini
```

### Comparing `drop_analysis-0.3.0b0/.gitignore` & `drop-analysis-1.0.0rc1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+.vscode/
 Sample/
 Dockerfile
 buffer/
+*.build/
+*.dist/
+*.md.backup
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `drop_analysis-0.3.0b0/LICENSE` & `drop-analysis-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/Old scripts/GUI_sessile_drop_analysis.py` & `drop-analysis-1.0.0rc1/Old scripts/GUI_sessile_drop_analysis.py`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/Old scripts/contact_angle_analysis_function.py` & `drop-analysis-1.0.0rc1/Old scripts/contact_angle_analysis_function.py`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/Old scripts/edge_detection.py` & `drop-analysis-1.0.0rc1/Old scripts/edge_detection.py`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/Old scripts/sessile_drop_analysis.py` & `drop-analysis-1.0.0rc1/Old scripts/sessile_drop_analysis.py`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/PKG-INFO` & `drop-analysis-1.0.0rc1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,23 @@
-Metadata-Version: 2.1
-Name: drop_analysis
-Version: 0.3.0b0
-Summary: A program to capture and analyze images of droplets
-Home-page: https://github.com/mvgorcum/Sessile.drop.analysis
-Author: Mathijs van Gorcum
-Author-email: mathijs@vgorcum.com
-License: GNU GPL v3+
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Provides-Extra: test
-License-File: LICENSE
-
 # Python sessile drop analysis
 [![Element Android Matrix room #Sessile.Drop.Analysis:matrix.vgorcum.com](https://img.shields.io/matrix/Sessile.Drop.Analysis:matrix.vgorcum.com.svg?label=%23Sessile.Drop.Analysis:matrix.vgorcum.com&logo=matrix&server_fqdn=matrix.org)](https://matrix.to/#/#Sessile.Drop.Analysis:matrix.vgorcum.com)
 
 Made by Mathijs van Gorcum during his PhD at the Physics of Fluids group of the University of Twente.
 
+For the user documentation go to [drop-analysis.com](https://drop-analysis.com).
+
 Python program to analyze sessile drops by measuring contact angle, drop volume and contact line position (as function of time or framenumber).  
 This program can capture images or movies from a camera or import image sequences (in the form of an movie file, a tiffstack or a single image) and measures the contact angle, drop volume and the contact line position.  
 The program assumes an image of a drop on the surface, where the drop is dark, and the background is light.
 A crop (to increase calculation speed, and cut off any irrelevant parts) and a baseline must be set on the view of the image. The Edgepixels to fit setting increases the amount of pixels up from the baseline used to measure the contact angle and contact line position.  
 We use a subpixel edge detection, either fast (with a linear interpolation between two pixels around the edge) or slow and more precise (by fitting an error function around the edge). To find the contact line position and the contact angle the detected edge is fitted with a configurable order polynomial fit, and the slope of the baseline is also used to calculate the contact angles. Note that the drop volume assume cylindrical symmetry and if there is a needle present, the volume of the needle is added for as much as it is in view of the crop.
 
 ## Screenshot
 
-![](https://github.com/mvgorcum/Sessile.drop.analysis/blob/master/Screenshot.png)
+![](Screenshot.png)
 
 ## Install and running
 This program has an installer for windows available in the [releases assets on github](https://github.com/mvgorcum/Sessile.drop.analysis/releases), or is installable from pypi.org with `pip install drop-analysis`.
 
 To install the program from source run `pip install .` in the sessile.drop.analysis folder. To run the program after installing simply run drop_analysis in the terminal.
 
 ## Prerequisites
@@ -47,9 +36,7 @@
 
 ## Contributing
 Feel free to send pull requests, critique my awful code or point out any issues.
 
 ## License
 This project is licensed under the GPLv3 license - see the [LICENSE](https://github.com/mvgorcum/Sessile.drop.analysis/blob/master/LICENSE) file for details.  
 This means the software can be freely used, for private, academic, or commercial purposes. If this program is distributed you are required to use a compatible open source license and must share the sourcecode of your version.
-
-
```

### Comparing `drop_analysis-0.3.0b0/Sample/Sample.avi` & `drop-analysis-1.0.0rc1/Sample/Sample.avi`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/Screenshot.png` & `drop-analysis-1.0.0rc1/Screenshot.png`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/docs/Makefile` & `drop-analysis-1.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/docs/conf.py` & `drop-analysis-1.0.0rc1/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
 
 # -- Project information -----------------------------------------------------
 
-project = 'sessile_drop_analysis'
-copyright = '2021, Mathijs van Gorcum'
+project = 'drop-analysis'
+copyright = '2023, Mathijs van Gorcum'
 author = 'Mathijs van Gorcum'
 
 # The full version, including alpha/beta/rc tags
-from sessile_drop_analysis import __version__
+from drop_analysis import __version__
 release = __version__
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -30,39 +30,72 @@
     'sphinx.ext.inheritance_diagram',
     'sphinx.ext.viewcode',
     'sphinx.ext.napoleon',
     'sphinx.ext.doctest',
     'sphinx.ext.mathjax',
     'sphinx_automodapi.automodapi',
     'sphinx_automodapi.smart_resolver',
+    "sphinx_favicon",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
-source_suffix = '.rst'
+source_suffix = {
+    '.rst': 'restructuredtext',
+    '.md': 'markdown',
+}
 
 # The master toctree document.
 master_doc = 'index'
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {'https://docs.python.org/': None}
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'alabaster'
+html_theme = 'sphinx_book_theme'
+
+html_static_path = ["_static"]
+
+favicons = [
+    {"href": "html_favicon.ico"},]
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
+
+# for MarkdownParser
+from sphinx_markdown_parser.parser import MarkdownParser
+
+def setup(app):
+    app.add_source_suffix('.md', 'markdown')
+    app.add_source_parser(MarkdownParser)
+    app.add_config_value('markdown_parser_config', {
+        'auto_toc_tree_section': 'Content',
+        'enable_auto_doc_ref': True,
+        'enable_auto_toc_tree': True,
+        'enable_eval_rst': True,
+        'enable_inline_math': True,
+        'extensions': [
+            'extra',
+            'nl2br',
+            'sane_lists',
+            'smarty',
+            'toc',
+            'wikilinks',
+            'pymdownx.arithmatex',
+        ],
+    }, True)
+
```

### Comparing `drop_analysis-0.3.0b0/docs/make.bat` & `drop-analysis-1.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/drop_analysis/FrameSupply.py` & `drop-analysis-1.0.0rc1/drop_analysis/FrameSupply.py`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/drop_analysis/Mainwindow.ui` & `drop-analysis-1.0.0rc1/drop_analysis/Mainwindow.ui`

 * *Files 2% similar despite different names*

#### Comparing `drop_analysis-0.3.0b0/drop_analysis/Mainwindow.ui` & `drop-analysis-1.0.0rc1/drop_analysis/Mainwindow.ui`

```diff
@@ -263,15 +263,15 @@
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>1280</width>
-          <height>32</height>
+          <height>30</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <widget class="QMenu" name="menuSave">
@@ -289,16 +289,24 @@
       </widget>
       <widget class="QMenu" name="menuEdit">
         <property name="title">
           <string>Edit</string>
         </property>
         <addaction name="actionSettings"/>
       </widget>
+      <widget class="QMenu" name="menuHelp">
+        <property name="title">
+          <string>Help</string>
+        </property>
+        <addaction name="actionHelp"/>
+        <addaction name="actionAbout"/>
+      </widget>
       <addaction name="menuFile"/>
       <addaction name="menuEdit"/>
+      <addaction name="menuHelp"/>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
     <action name="actionNewMeasurement">
       <property name="text">
         <string>New Measurement</string>
       </property>
     </action>
@@ -328,14 +336,24 @@
       </property>
     </action>
     <action name="actionExportVideo">
       <property name="text">
         <string>Export Video</string>
       </property>
     </action>
+    <action name="actionHelp">
+      <property name="text">
+        <string>Help</string>
+      </property>
+    </action>
+    <action name="actionAbout">
+      <property name="text">
+        <string>About</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>PlotWidget</class>
       <extends>QWidget</extends>
       <header location="global">pyqtgraph</header>
       <container>1</container>
```

### Comparing `drop_analysis-0.3.0b0/drop_analysis/Settings.ui` & `drop-analysis-1.0.0rc1/drop_analysis/Settings.ui`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/drop_analysis/data/common_resolutions.csv` & `drop-analysis-1.0.0rc1/drop_analysis/data/common_resolutions.csv`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/drop_analysis/data/icon.ico` & `drop-analysis-1.0.0rc1/docs/_static/html_favicon.ico`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/drop_analysis/data/icon.xcf` & `drop-analysis-1.0.0rc1/drop_analysis/data/icon.xcf`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/drop_analysis/edge_detection.py` & `drop-analysis-1.0.0rc1/drop_analysis/edge_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Created on Tue Dec 20 16:20:35 2016
 
 @author: M.van.Gorcum
 """
 import numpy as np
 import scipy as sp
+from scipy.optimize import least_squares
 
 def subpixel_detection(image,thresh,mode):
     """
     edge detection, allowing for two subpixel detection methods
     """
     erffitsize=np.int(40)
     framesize=image.shape
@@ -48,21 +49,21 @@
     Subpixel detection by fitting an error function on the 'erffitsize' pixels around the detected edge
     """
     def errorfunction(x,xdata,y): #define errorfunction to fit with a least squares fit.
         return x[0]*(1+sp.special.erf(xdata*x[1]+x[2]))+x[3] - y
     if (edgeleft-erffitsize)>=0  and (edgeleft-erffitsize)<=len(imagerow):
         fitparts=np.array(imagerow[range(np.int(edgeleft)-erffitsize,np.int(edgeleft)+erffitsize)]) #take out part of the image around the edge to fit the error function
         guess=(max(fitparts)-min(fitparts))/2,-.22,0,min(fitparts) #initial guess for error function
-        lstsqrsol=sp.optimize.least_squares(errorfunction,guess,args=(np.array(range(-erffitsize,erffitsize)),fitparts)) #least sqaures fit
+        lstsqrsol=least_squares(errorfunction,guess,args=(np.array(range(-erffitsize,erffitsize)),fitparts)) #least sqaures fit
         leftsubpxcorr=-lstsqrsol.x[2]/lstsqrsol.x[1] #add the subpixel correction
     else:
         leftsubpxcorr=0
     if (edgeright-erffitsize)>=0  and (edgeright+erffitsize)<len(imagerow):
         fitparts=np.array(imagerow[range(np.int(edgeright)-erffitsize,np.int(edgeright)+erffitsize)])
         guess=(max(fitparts)-min(fitparts))/2,.22,0,min(fitparts)
-        lstsqrsol=sp.optimize.least_squares(errorfunction,guess,args=(np.array(range(-erffitsize,erffitsize)),fitparts))
+        lstsqrsol=least_squares(errorfunction,guess,args=(np.array(range(-erffitsize,erffitsize)),fitparts))
         rightsubpxcorr=-lstsqrsol.x[2]/lstsqrsol.x[1]
     else:
         rightsubpxcorr=0
     return leftsubpxcorr,rightsubpxcorr
```

### Comparing `drop_analysis-0.3.0b0/drop_analysis/gui.py` & `drop-analysis-1.0.0rc1/drop_analysis/gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 from PyQt5 import QtWidgets, uic, QtGui
 from PyQt5.QtCore import pyqtSignal, Qt
 
 import cv2
 import pyqtgraph as pg
 import sys
 from pathlib import Path
-from .otsu import otsu
+from drop_analysis.otsu import otsu
 import numpy as np
 import pandas as pd
 import threading
 from time import sleep
 from pkg_resources import resource_filename
 import mimetypes
 
-from . import FrameSupply
-from . import settings
-from .edge_detection import subpixel_detection as edgedetection
-from .edge_analysis import analysis
+import drop_analysis.FrameSupply as FrameSupply
+from drop_analysis.settings import settings
+from drop_analysis.edge_detection import subpixel_detection as edgedetection
+from drop_analysis.edge_analysis import analysis
+from drop_analysis.Help import Ui_Help
+from drop_analysis.About import Ui_About
+from drop_analysis import version
 
 pg.setConfigOptions(imageAxisOrder='row-major')
 
+#a dict to map the different files that can be opened to the right framesupply object. 
+#if a new filetype is to be supported, a framesource class needs to be written
+#and the mimetype of said format can then be mapped to said class here.
 filetypemap={'image/tiff':FrameSupply.ImageReader,'image/jpeg':FrameSupply.ImageReader,'image/png':FrameSupply.ImageReader,
              'video/x-msvideo':FrameSupply.OpencvReadVideo,'video/mp4':FrameSupply.OpencvReadVideo,'video/avi':FrameSupply.OpencvReadVideo,
              'application/x-hdf':FrameSupply.Hdf5Reader}
 
 class MainWindow(QtWidgets.QMainWindow):
     updateVideo = pyqtSignal(np.ndarray)
     updateLeftEdge = pyqtSignal(np.ndarray,np.ndarray)
     updateRightEdge = pyqtSignal(np.ndarray,np.ndarray)
     updatePlotLeft = pyqtSignal(np.ndarray,np.ndarray)
     updatePlotRight = pyqtSignal(np.ndarray,np.ndarray)
     updateLeftEdgeFit = pyqtSignal(np.ndarray,np.ndarray)
     updateRightEdgeFit = pyqtSignal(np.ndarray,np.ndarray)
+    updateCenterOfMass = pyqtSignal(list,list)
     updateFrameCount=pyqtSignal(int,int)
     updateFitHeightLine=pyqtSignal(np.ndarray,np.ndarray)
     def __init__(self, *args, **kwargs):
         """
         Initialize the main window, set up all plots, and connect to defined buttons.
         """
         super(MainWindow, self).__init__(*args, **kwargs)
@@ -52,21 +59,25 @@
         self.VideoItem = pg.ImageItem()
         self.RootVidPlot.addItem(self.VideoItem)
         self.LeftEdgeFit=pg.PlotCurveItem(pen=pg.mkPen(color='#2ca02c', width=4))
         self.RightEdgeFit=pg.PlotCurveItem(pen=pg.mkPen(color='#d62728', width=4))
         self.LeftEdgeItem=pg.PlotCurveItem(pen=pg.mkPen(color='#ff7f0e', width=2))
         self.RightEdgeItem=pg.PlotCurveItem(pen=pg.mkPen(color='#1f77b4', width=2))
         self.FitHeightLine=pg.PlotCurveItem(pen=pg.mkPen(color='#d62728', width=1,style=Qt.DashLine))
+        self.CenterOfMassItem=pg.ScatterPlotItem(pen='#ff7f0e',brush='#ff7f0e',symbol='o')
 
         self.RootVidPlot.addItem(self.RightEdgeFit)
         self.RootVidPlot.addItem(self.LeftEdgeFit)
         self.RootVidPlot.addItem(self.LeftEdgeItem)
         self.RootVidPlot.addItem(self.RightEdgeItem)
         self.RootVidPlot.addItem(self.FitHeightLine)
+        self.RootVidPlot.addItem(self.CenterOfMassItem)
+
         self.updateVideo.connect(self.VideoItem.setImage)
+        self.updateCenterOfMass.connect(self.CenterOfMassItem.setData)
         self.updateLeftEdgeFit.connect(self.LeftEdgeFit.setData)
         self.updateRightEdgeFit.connect(self.RightEdgeFit.setData)
         self.updateLeftEdge.connect(self.LeftEdgeItem.setData)
         self.updateRightEdge.connect(self.RightEdgeItem.setData)
         self.updateFitHeightLine.connect(self.FitHeightLine.setData)
 
         self.ThetaLeftPlot=pg.ScatterPlotItem(pen='#ff7f0e',brush='#ff7f0e',symbol='o')
@@ -76,68 +87,88 @@
         self.updatePlotRight.connect(self.ThetaRightPlot.setData)
 
         self.BaseLine=pg.LineSegmentROI([(15,90),(100,90)],pen='#d62728')
         self.CropRoi=pg.RectROI([10,10],[110,110],scaleSnap=True)
         self.CropRoi.addScaleHandle([0,0],[1,1])
         self.VideoWidget.addItem(self.CropRoi)
         self.VideoWidget.addItem(self.BaseLine)
+        
 
         self.BaseLine.sigRegionChanged.connect(self._updateFitHeightLine)
         self.actionOpen.triggered.connect(self.openCall)
         self.actionSaveData.triggered.connect(self.SaveResult)
         self.actionSettings.triggered.connect(self.configSettings)
         self.StartStopButton.clicked.connect(self.StartStop)
         self.CameraToggleButton.clicked.connect(self.CameraToggle)
         self.VidRecordButton.clicked.connect(self.recordVid)
         self.VidRecordButton.hide()
         self.actionSaveVideo.triggered.connect(self.SaveVideo)
         self.actionExportVideo.triggered.connect(self.ExportVideo)
 
         self.FrameSource=FrameSupply.FrameSupply()
-        self.MeasurementResult=pd.DataFrame(columns=['thetaleft', 'thetaright', 'contactpointleft','contactpointright','volume','time'])
+        self.MeasurementResult=pd.DataFrame(columns=['thetaleft', 'thetaright', 'contactpointleftx','contactpointlefty','contactpointrightx','contactpointrighty','volume','time'])
 
         self.MaybeSave=False
-        self.settings=settings.settings(self)
+        self.settings=settings(self)
 
         self.kInputSlider.setValue(self.settings.config['sessiledrop']['defaultfitpixels'])
         self.kInputSpinbox.setValue(self.kInputSlider.value())
         self.kInputSlider.valueChanged.connect(lambda: self._updateFitHeightLine('slider'))
         self.kInputSpinbox.valueChanged.connect(lambda: self._updateFitHeightLine('spinbox'))
 
-        self.updateFrameCount.connect(lambda f,n: self.FrameCounterText.setText('Frame: '+str(f)+'/'+str(n)))
+        self.updateFrameCount.connect(lambda f,n: self.FrameCounterText.setText(f'Frame: {str(f)} / {str(n)}'))
+        
+        self.helpwidget=QtWidgets.QDialog()
+        self.helpUI=Ui_Help()
+        self.helpUI.setupUi(self.helpwidget)
+        self.aboutwidget=QtWidgets.QDialog()
+        self.aboutUI=Ui_About()
+        self.aboutUI.setupUi(self.aboutwidget)
+        self.aboutUI.versionLabel.setText(f"Version: {version.__version__}")
+        self.actionHelp.triggered.connect(self.helpwidget.show)
+        self.actionAbout.triggered.connect(self.aboutwidget.show)
 
     def _updateFitHeightLine(self,kset=''):
+        """This sets the amount of pixels to use for the fit, and we want the slider and the input spinbox to show the same value"""
         if kset=='slider':
             self.kInputSpinbox.setValue(self.kInputSlider.value())
         elif kset=='spinbox':
             self.kInputSlider.setValue(self.kInputSpinbox.value())
         _,basearray=self.BaseLine.getArrayRegion(self.VideoItem.image, self.VideoItem, returnSlice=False, returnMappedCoords=True)
         baseinput=[[basearray[0,0],basearray[1,0]-self.kInputSpinbox.value()],[basearray[0,-1],basearray[1,-1]-self.kInputSpinbox.value()]]
         plotlinex=np.array([basearray[0,0],basearray[0,-1]])
         plotliney=np.array([basearray[1,0]-self.kInputSpinbox.value(),basearray[1,-1]-self.kInputSpinbox.value()])
         self.updateFitHeightLine.emit(plotlinex,plotliney)
 
         
     def closeEvent(self, event):
         if self.FrameSource.is_running:
             self.FrameSource.stop()
+        if self.MaybeSave:
+            savepopup=QtWidgets.QMessageBox()
+            savepopup.setText('Unsaved analysis data.')
+            savepopup.setInformativeText("Do you want to save your data?")
+            savepopup.setStandardButtons(QtWidgets.QMessageBox.Save | QtWidgets.QMessageBox.Discard)
+            reply=savepopup.exec_()
+            if reply == QtWidgets.QMessageBox.Save:
+                self.SaveResult()
 
     def recordVid(self):
         if self.VidRecordButton.isChecked():
             self.FrameSource.record=True
         else:
             self.FrameSource.record=False
 
 
     def openCall(self):
         if self.FrameSource.is_running:
             self.FrameSource.stop()
         VideoFile, _ = QtWidgets.QFileDialog.getOpenFileName(self,'Open file')
         mimetype=mimetypes.guess_type(VideoFile)[0]
-        self.MeasurementResult=pd.DataFrame(columns=['thetaleft', 'thetaright', 'contactpointleft','contactpointright','volume','time'])
+        self.MeasurementResult=pd.DataFrame(columns=['thetaleft', 'thetaright', 'contactpointleftx','contactpointlefty','contactpointrightx','contactpointrighty','volume','time'])
         self.PlotItem.clear()
         if mimetype is None or not any(mimetype in key for key in filetypemap):
             errorpopup=QtWidgets.QMessageBox()
             errorpopup.setText('Unkown filetype')
             errorpopup.setStandardButtons(QtWidgets.QMessageBox.Ok)
             errorpopup.exec_()
         else:
@@ -146,15 +177,14 @@
             FrameWidth,FrameHeight=self.FrameSource.getframesize()
             self.CropRoi.setPos([FrameWidth*.1,FrameHeight*.1])
             self.CropRoi.setSize([FrameWidth*.8,FrameHeight*.8])
             self.BaseLine.setPos([FrameWidth*.2,FrameHeight*.7])
             firstframe,_=self.FrameSource.getfirstframe()
             self.VideoItem.setImage(firstframe,autoRange=True)
 
-
     def StartStop(self):
         if self.StartStopButton.isChecked():
             self.StartStopButton.setText('Stop Measurement')
             self.PlotItem.setLabel('left',text='Contact angle [°]')
             if self.FrameSource.gotcapturetime:
                 self.PlotItem.setLabel('bottom',text='Time [s]')
             else:
@@ -182,15 +212,15 @@
             self.FrameSource.start()
             FrameWidth,FrameHeight=self.FrameSource.getframesize()
             self.CropRoi.setPos([FrameWidth*.1,FrameHeight*.1])
             self.CropRoi.setSize([FrameWidth*.8,FrameHeight*.8])
             self.BaseLine.setPos([FrameWidth*.2,FrameHeight*.7])
             CameraThread = threading.Thread(target=self.CameraCapture)
             CameraThread.start()
-            self.MeasurementResult=pd.DataFrame(columns=['thetaleft', 'thetaright', 'contactpointleft','contactpointright','volume','time'])
+            self.MeasurementResult=pd.DataFrame(columns=['thetaleft', 'thetaright', 'contactpointleftx','contactpointlefty','contactpointrightx','contactpointrighty','volume','centroidx','centroidy','time'])
             self.PlotItem.clear()
         else:
 
             self.VidRecordButton.hide()
 
     def CameraCapture(self):
         while self.CameraToggleButton.isChecked():
@@ -201,14 +231,21 @@
                 if not np.all(org_frame==-1):
                     self.updateVideo.emit(org_frame)
                 else:
                     sleep(0.001)
         self.FrameSource.stop()
 
     def RunAnalysis(self):
+        """
+        This runs the actual analysis, note that we will want to run this in a seperate thread to not lock up the camera and/or UI.
+        First we start by grabbing the frames from the framesupply object
+        Then we grab the crop and baseline from the pyqtgraph window as set by the user and crop the image
+        If it's a color image, make it grayscale and send the image off for edge detection with the edgedetection.py function
+        The resulting edge is then sent off for analysis, returning the contact line position and angles
+        """
         while self.StartStopButton.isChecked():
             org_frame,framecaptime = self.FrameSource.getnextframe()
             if not np.all(org_frame==-1):
                 #get crop and save coordinate transformation
                 self.updateVideo.emit(org_frame)
                 cropcoords=self.CropRoi.getArraySlice(org_frame, self.VideoItem, returnSlice=False)
                 verticalCropOffset=0.5+cropcoords[0][0][0]
@@ -228,29 +265,31 @@
                     gray = np.asarray(cropped)
                 thresh=otsu(gray)
                 CroppedEdgeLeft,CroppedEdgeRight=edgedetection(gray,thresh,self.settings.config['edgedetection']['subpixelscheme'])
                 EdgeLeft=CroppedEdgeLeft+horizontalCropOffset
                 EdgeRight=CroppedEdgeRight+horizontalCropOffset
                 results, debuginfo = analysis(EdgeLeft,EdgeRight,base,cropped.shape,k=self.kInputSpinbox.value(),PO=self.settings.config['sessiledrop']['polyfitorder'],fittype=self.settings.config['sessiledrop']['fittype'])
                 results.update({'time':framecaptime})
-                self.MeasurementResult=self.MeasurementResult.append(results,ignore_index=True)
+                results['centroidy']=results['centroidy']+verticalCropOffset #TODO: this is ugly and needs fixing
+                self.MeasurementResult=pd.concat((self.MeasurementResult,pd.DataFrame(results,index=[0])),ignore_index=True)
                 if self.FrameSource.gotcapturetime:
                     plottime=self.MeasurementResult['time']-self.MeasurementResult.iloc[0]['time']
                     #convert from nanoseconds to seconds
                     plottime=plottime.to_numpy().astype('float')*10**-9
                 else:
                     plottime=self.MeasurementResult['time'].to_numpy()
                 plotleft=self.MeasurementResult['thetaleft'].to_numpy()
                 plotright=self.MeasurementResult['thetaright'].to_numpy()
                 self.updateLeftEdge.emit(EdgeLeft,np.arange(0,len(EdgeLeft))+verticalCropOffset)
                 self.updateRightEdge.emit(EdgeRight,np.arange(0,len(EdgeRight))+verticalCropOffset)
                 self.updatePlotLeft.emit(plottime,plotleft)
                 self.updatePlotRight.emit(plottime,plotright)
                 self.updateLeftEdgeFit.emit(debuginfo['leftfit'][0,:],verticalCropOffset+debuginfo['leftfit'][1,:])
                 self.updateRightEdgeFit.emit(debuginfo['rightfit'][0,:],verticalCropOffset+debuginfo['rightfit'][1,:])
+                self.updateCenterOfMass.emit([results['centroidx']],[results['centroidy']])
                 self.MaybeSave=True
                 self.updateFrameCount.emit(self.FrameSource.framenumber,self.FrameSource.nframes)
             else:
                 sleep(0.001)
             if (not self.FrameSource.is_running and len(self.FrameSource.framebuffer)<1):
                 break
 
@@ -336,8 +375,7 @@
             progress.setValue(totalframes)
             writer.release()
         else:
             errorpopup=QtWidgets.QMessageBox()
             errorpopup.setText("Can't export video while recording is running")
             errorpopup.setStandardButtons(QtWidgets.QMessageBox.Ok)
             errorpopup.exec_()
-
```

### Comparing `drop_analysis-0.3.0b0/drop_analysis/settings.py` & `drop-analysis-1.0.0rc1/drop_analysis/settings.py`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/drop_analysis.egg-info/SOURCES.txt` & `drop-analysis-1.0.0rc1/drop_analysis.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 Screenshot.png
 pyinst_entrypoint.py
+pynsist_installer.cfg
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 Old scripts/GUI_sessile_drop_analysis.py
 Old scripts/contact_angle_analysis_function.py
 Old scripts/edge_detection.py
 Old scripts/sessile_drop_analysis.py
 Sample/Sample.avi
+docs/Analysis_running.png
+docs/Camera_settings.png
+docs/Edge_detection_setting.png
+docs/Just_launched.png
 docs/Makefile
+docs/Opened_video_file.png
+docs/Placed_baseline.png
+docs/Sessile_drop_settings.png
+docs/Use_200_pixels.png
 docs/conf.py
+docs/contact.md
+docs/contact.md.backup
 docs/index.rst
+docs/install.md
 docs/make.bat
+docs/usage.md
+docs/usage.md.backup
+docs/_static/html_favicon.ico
+drop_analysis/About.py
+drop_analysis/About.ui
 drop_analysis/FrameSupply.py
+drop_analysis/Help.py
+drop_analysis/Help.ui
 drop_analysis/Mainwindow.ui
+drop_analysis/README.rst
 drop_analysis/Settings.ui
 drop_analysis/__init__.py
 drop_analysis/__main__.py
 drop_analysis/config.toml
 drop_analysis/edge_analysis.py
 drop_analysis/edge_detection.py
 drop_analysis/gui.py
```

### Comparing `drop_analysis-0.3.0b0/setup.cfg` & `drop-analysis-1.0.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = drop_analysis
 author = Mathijs van Gorcum
-author_email = mathijs@vgorcum.com
+author_email = dropanalysis@vgorcum.com
 license = GNU GPL v3+
 license_file = LICENSE
-url = https://github.com/mvgorcum/Sessile.drop.analysis
+url = https://drop-analysis.com
 description = A program to capture and analyze images of droplets
 long_description = file: README.md
 Description-Content-Type = text/markdown
 
 [options]
 zip_safe = False
 packages = find:
```

### Comparing `drop_analysis-0.3.0b0/setup.py` & `drop-analysis-1.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `drop_analysis-0.3.0b0/tox.ini` & `drop-analysis-1.0.0rc1/tox.ini`

 * *Files identical despite different names*

