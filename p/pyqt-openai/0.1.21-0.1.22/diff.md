# Comparing `tmp/pyqt-openai-0.1.21.tar.gz` & `tmp/pyqt-openai-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-openai-0.1.21.tar", last modified: Fri May  5 23:52:03 2023, max compression
+gzip compressed data, was "pyqt-openai-0.1.22.tar", last modified: Sat May  6 01:35:17 2023, max compression
```

## Comparing `pyqt-openai-0.1.21.tar` & `pyqt-openai-0.1.22.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.314478 pyqt-openai-0.1.21/
--rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.21/LICENSE
--rw-rw-rw-   0        0        0     5104 2023-05-05 23:52:03.312481 pyqt-openai-0.1.21/PKG-INFO
--rw-rw-rw-   0        0        0     4710 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.093038 pyqt-openai-0.1.21/pyqt_openai/
--rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/__init__.py
--rw-rw-rw-   0        0        0     6738 2023-04-09 06:45:06.000000 pyqt-openai-0.1.21/pyqt_openai/a.py
--rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/apiData.py
--rw-rw-rw-   0        0        0     6771 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/chatWidget.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/circleProfileImage.py
--rw-rw-rw-   0        0        0     8132 2023-04-08 11:47:46.000000 pyqt-openai-0.1.21/pyqt_openai/clickableTooltip.py
--rw-rw-rw-   0        0        0     5072 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/convListWidget.py
--rw-rw-rw-   0        0        0     7583 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/customizeDialog.py
-drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.159860 pyqt-openai-0.1.21/pyqt_openai/ico/
--rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.21/pyqt_openai/ico/__init__.py
--rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/add.svg
--rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.21/pyqt_openai/ico/close.svg
--rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/ico/customize.svg
--rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/delete.svg
--rw-rw-rw-   0        0        0      654 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/download.svg
--rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/help.svg
--rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.21/pyqt_openai/ico/openai.svg
--rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/ico/prompt.svg
--rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/search.svg
--rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/setting.svg
--rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.21/pyqt_openai/ico/sidebar.svg
--rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.21/pyqt_openai/ico/stackontop.svg
--rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/ico/user.svg
--rw-rw-rw-   0        0        0     1383 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/inputDialog.py
--rw-rw-rw-   0        0        0     3768 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/leftSideBar.py
--rw-rw-rw-   0        0        0    22515 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/main.py
--rw-rw-rw-   0        0        0     1788 2023-04-08 11:47:46.000000 pyqt-openai-0.1.21/pyqt_openai/modelTable.py
--rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.21/pyqt_openai/notifier.py
-drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.193285 pyqt-openai-0.1.21/pyqt_openai/prompt/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/prompt/__init__.py
--rw-rw-rw-   0        0        0     1721 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/prompt/promptGeneratorWidget.py
--rw-rw-rw-   0        0        0     1574 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/prompt/propPage.py
--rw-rw-rw-   0        0        0     3351 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/prompt/templatePage.py
-drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.247142 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/
--rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/__init__.py
--rw-rw-rw-   0        0        0     2220 2023-05-05 02:57:06.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
--rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/chatPage.py
--rw-rw-rw-   0        0        0    11101 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/completionPage.py
--rw-rw-rw-   0        0        0     1623 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/imagePage.py
--rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/searchBar.py
--rw-rw-rw-   0        0        0    21685 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/sqlite.py
--rw-rw-rw-   0        0        0     5931 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/svgButton.py
--rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.21/pyqt_openai/svgLabel.py
-drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.275074 pyqt-openai-0.1.21/pyqt_openai/test/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/test/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/test/htmlformat.py
--rw-rw-rw-   0        0        0     1280 2023-04-23 09:02:45.000000 pyqt-openai-0.1.21/pyqt_openai/test/rightSideBarTab.py
-drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.310487 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/
--rw-rw-rw-   0        0        0        0 2023-05-05 07:22:12.000000 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/__init__.py
--rw-rw-rw-   0        0        0      722 2023-05-05 12:31:35.000000 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/delete_model.py
--rw-rw-rw-   0        0        0     2559 2023-05-05 07:22:36.000000 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/make_model.py
--rw-rw-rw-   0        0        0      433 2023-05-05 08:36:36.000000 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/using_model.py
-drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.129975 pyqt-openai-0.1.21/pyqt_openai.egg-info/
--rw-rw-rw-   0        0        0     5104 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1656 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 23:52:03.314478 pyqt-openai-0.1.21/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-05-05 23:45:36.000000 pyqt-openai-0.1.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.406271 pyqt-openai-0.1.22/
+-rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.22/LICENSE
+-rw-rw-rw-   0        0        0     5482 2023-05-06 01:35:17.405270 pyqt-openai-0.1.22/PKG-INFO
+-rw-rw-rw-   0        0        0     5082 2023-05-06 01:32:51.000000 pyqt-openai-0.1.22/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.303224 pyqt-openai-0.1.22/pyqt_openai/
+-rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/__init__.py
+-rw-rw-rw-   0        0        0     6738 2023-04-09 06:45:06.000000 pyqt-openai-0.1.22/pyqt_openai/a.py
+-rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/apiData.py
+-rw-rw-rw-   0        0        0     6771 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/chatWidget.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.22/pyqt_openai/circleProfileImage.py
+-rw-rw-rw-   0        0        0     8132 2023-04-08 11:47:46.000000 pyqt-openai-0.1.22/pyqt_openai/clickableTooltip.py
+-rw-rw-rw-   0        0        0     5072 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/convListWidget.py
+-rw-rw-rw-   0        0        0     7627 2023-05-06 01:32:51.000000 pyqt-openai-0.1.22/pyqt_openai/customizeDialog.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.365059 pyqt-openai-0.1.22/pyqt_openai/ico/
+-rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.22/pyqt_openai/ico/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/add.svg
+-rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.22/pyqt_openai/ico/close.svg
+-rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.22/pyqt_openai/ico/customize.svg
+-rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/delete.svg
+-rw-rw-rw-   0        0        0      654 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/download.svg
+-rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/help.svg
+-rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.22/pyqt_openai/ico/openai.svg
+-rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/ico/prompt.svg
+-rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/search.svg
+-rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/ico/setting.svg
+-rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.22/pyqt_openai/ico/sidebar.svg
+-rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.22/pyqt_openai/ico/stackontop.svg
+-rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.22/pyqt_openai/ico/user.svg
+-rw-rw-rw-   0        0        0     1383 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/inputDialog.py
+-rw-rw-rw-   0        0        0     3768 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/leftSideBar.py
+-rw-rw-rw-   0        0        0    22532 2023-05-06 01:32:51.000000 pyqt-openai-0.1.22/pyqt_openai/main.py
+-rw-rw-rw-   0        0        0     1788 2023-04-08 11:47:46.000000 pyqt-openai-0.1.22/pyqt_openai/modelTable.py
+-rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.22/pyqt_openai/notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.374035 pyqt-openai-0.1.22/pyqt_openai/prompt/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/prompt/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/prompt/promptGeneratorWidget.py
+-rw-rw-rw-   0        0        0     1574 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/prompt/propPage.py
+-rw-rw-rw-   0        0        0     3351 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/prompt/templatePage.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.386317 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/
+-rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/__init__.py
+-rw-rw-rw-   0        0        0     2220 2023-05-05 02:57:06.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
+-rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/chatPage.py
+-rw-rw-rw-   0        0        0    11101 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/completionPage.py
+-rw-rw-rw-   0        0        0     1623 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/right_sidebar/imagePage.py
+-rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/searchBar.py
+-rw-rw-rw-   0        0        0    21685 2023-05-06 01:32:51.000000 pyqt-openai-0.1.22/pyqt_openai/sqlite.py
+-rw-rw-rw-   0        0        0     5931 2023-04-22 00:05:31.000000 pyqt-openai-0.1.22/pyqt_openai/svgButton.py
+-rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.22/pyqt_openai/svgLabel.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.393302 pyqt-openai-0.1.22/pyqt_openai/test/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/test/__init__.py
+-rw-rw-rw-   0        0        0     1425 2023-05-06 00:44:23.000000 pyqt-openai-0.1.22/pyqt_openai/test/dialog.py
+-rw-rw-rw-   0        0        0     1773 2023-05-05 02:56:55.000000 pyqt-openai-0.1.22/pyqt_openai/test/htmlformat.py
+-rw-rw-rw-   0        0        0     1280 2023-04-23 09:02:45.000000 pyqt-openai-0.1.22/pyqt_openai/test/rightSideBarTab.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.403276 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/
+-rw-rw-rw-   0        0        0        0 2023-05-05 07:22:12.000000 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-05-05 12:31:35.000000 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/delete_model.py
+-rw-rw-rw-   0        0        0     2559 2023-05-05 07:22:36.000000 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/make_model.py
+-rw-rw-rw-   0        0        0      433 2023-05-05 08:36:36.000000 pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/using_model.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:35:17.336141 pyqt-openai-0.1.22/pyqt_openai.egg-info/
+-rw-rw-rw-   0        0        0     5482 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1683 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 01:35:17.000000 pyqt-openai-0.1.22/pyqt_openai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 01:35:17.406271 pyqt-openai-0.1.22/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-05-06 01:33:10.000000 pyqt-openai-0.1.22/setup.py
```

### Comparing `pyqt-openai-0.1.21/LICENSE` & `pyqt-openai-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/PKG-INFO` & `pyqt-openai-0.1.22/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.21
+Version: 0.1.22
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -37,24 +37,30 @@
 
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 Some of the features are still being tested.
 
+I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b>
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
-* support GPT-4
-* you can save the conversation history with sqlite database
+* conversation management
+  * add & delete conversations
+  * save conversations
+  * rename conversation
+  * everything above is saved in an SQLite database file named conv.db.
+* support GPT-4 and every other models below GPT3
 * support prompt generator
 * support image generation with DALL-E
-* you can test any models, including gpt3.5
 * you can run this in background application
+  * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.21 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.22 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot. Even though this
@@ -12,27 +12,32 @@
 for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
 nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
 generation feature available since v0.0.16. You can see the detail in official
 OpenAI site. Currently this feature is very basic now. This is using sqlite as
 a database. You can select the model at the right side bar. An internet
 connection is required. ## Contact You can join pyqt-openai's Discord_Server to
 have a conversation about it or AI-related stuff ð ## Note Some of the
-features are still being tested. ## Feature * basically this is desktop
-application version of ChatGPT * text streaming (enable by default, you can
-disable it) * AI remembers past conversation * support GPT-4 * you can save the
-conversation history with sqlite database * support prompt generator * support
-image generation with DALL-E * you can test any models, including gpt3.5 * you
-can run this in background application * you can make window stack on top or
-control its transparency ## Requirements * qtpy - the package allowing you to
-write code that works with both PyQt and PySide * PyQt5 >= 5.14 or PySide6 *
-openai ## Preview This is using GPT-3.5 turbo model by default. ### Homepage !
-[image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-
-2b8f-483b-9271-b78ab8a1eb73.png) You have to write your openai api key inside
-the red box. see [How to play](#how-to-play) ### Overview ![image](https://
-user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
+features are still being tested. I recommend to install sqlite management
+software. It's not necessary to run this app (obviously), but it's good
+practice to manage database about conversation history with AI and to know how
+this works. ## Feature * basically this is desktop application version of
+ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
+past conversation * conversation management * add & delete conversations * save
+conversations * rename conversation * everything above is saved in an SQLite
+database file named conv.db. * support GPT-4 and every other models below GPT3
+* support prompt generator * support image generation with DALL-E * you can run
+this in background application * notification will pop up when response is
+generated * you can make window stack on top or control its transparency ##
+Requirements * qtpy - the package allowing you to write code that works with
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
+using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
+images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-
+b78ab8a1eb73.png) You have to write your openai api key inside the red box. see
+[How to play](#how-to-play) ### Overview ![image](https://user-
+images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
 e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
 user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
 7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
 Generator https://user-images.githubusercontent.com/55078043/236584481-
 b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
 lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
```

### Comparing `pyqt-openai-0.1.21/README.md` & `pyqt-openai-0.1.22/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -25,24 +25,30 @@
 
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 Some of the features are still being tested.
 
+I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b>
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
-* support GPT-4
-* you can save the conversation history with sqlite database
+* conversation management
+  * add & delete conversations
+  * save conversations
+  * rename conversation
+  * everything above is saved in an SQLite database file named conv.db.
+* support GPT-4 and every other models below GPT3
 * support prompt generator
 * support image generation with DALL-E
-* you can test any models, including gpt3.5
 * you can run this in background application
+  * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
```

#### html2text {}

```diff
@@ -9,27 +9,32 @@
 for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
 nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
 generation feature available since v0.0.16. You can see the detail in official
 OpenAI site. Currently this feature is very basic now. This is using sqlite as
 a database. You can select the model at the right side bar. An internet
 connection is required. ## Contact You can join pyqt-openai's Discord_Server to
 have a conversation about it or AI-related stuff ð ## Note Some of the
-features are still being tested. ## Feature * basically this is desktop
-application version of ChatGPT * text streaming (enable by default, you can
-disable it) * AI remembers past conversation * support GPT-4 * you can save the
-conversation history with sqlite database * support prompt generator * support
-image generation with DALL-E * you can test any models, including gpt3.5 * you
-can run this in background application * you can make window stack on top or
-control its transparency ## Requirements * qtpy - the package allowing you to
-write code that works with both PyQt and PySide * PyQt5 >= 5.14 or PySide6 *
-openai ## Preview This is using GPT-3.5 turbo model by default. ### Homepage !
-[image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-
-2b8f-483b-9271-b78ab8a1eb73.png) You have to write your openai api key inside
-the red box. see [How to play](#how-to-play) ### Overview ![image](https://
-user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
+features are still being tested. I recommend to install sqlite management
+software. It's not necessary to run this app (obviously), but it's good
+practice to manage database about conversation history with AI and to know how
+this works. ## Feature * basically this is desktop application version of
+ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
+past conversation * conversation management * add & delete conversations * save
+conversations * rename conversation * everything above is saved in an SQLite
+database file named conv.db. * support GPT-4 and every other models below GPT3
+* support prompt generator * support image generation with DALL-E * you can run
+this in background application * notification will pop up when response is
+generated * you can make window stack on top or control its transparency ##
+Requirements * qtpy - the package allowing you to write code that works with
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
+using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
+images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-
+b78ab8a1eb73.png) You have to write your openai api key inside the red box. see
+[How to play](#how-to-play) ### Overview ![image](https://user-
+images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
 e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
 user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
 7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
 Generator https://user-images.githubusercontent.com/55078043/236584481-
 b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
 lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
```

### Comparing `pyqt-openai-0.1.21/pyqt_openai/a.py` & `pyqt-openai-0.1.22/pyqt_openai/a.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/apiData.py` & `pyqt-openai-0.1.22/pyqt_openai/apiData.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/chatWidget.py` & `pyqt-openai-0.1.22/pyqt_openai/chatWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/circleProfileImage.py` & `pyqt-openai-0.1.22/pyqt_openai/circleProfileImage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/clickableTooltip.py` & `pyqt-openai-0.1.22/pyqt_openai/clickableTooltip.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/convListWidget.py` & `pyqt-openai-0.1.22/pyqt_openai/convListWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/customizeDialog.py` & `pyqt-openai-0.1.22/pyqt_openai/customizeDialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,26 +155,26 @@
     def setAsDirectory(self, f: bool):
         self.__directory = f
 
     def isForDirectory(self) -> bool:
         return self.__directory
 
 class CustomizeDialog(QDialog):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.__initVal()
         self.__initUi()
 
     def __initVal(self):
         pass
 
     def __initUi(self):
         self.setWindowTitle('Customize (working)')
         self.setWindowIcon(QIcon('ico/openai.svg'))
-        self.setWindowFlags(Qt.WindowCloseButtonHint)
+        self.setWindowFlags(Qt.Window | Qt.WindowCloseButtonHint)
 
         homePageGraphicsView = SingleImageGraphicsView()
 
         userImage = RoundedImage()
         userImage.setMaximumSize(24, 24)
         userImage.setImage('ico/user.svg')
         AIImage = RoundedImage()
```

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/close.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/close.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/customize.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/customize.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/download.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/download.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/help.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/help.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/openai.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/openai.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/search.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/search.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/setting.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/setting.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/stackontop.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/stackontop.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/ico/user.svg` & `pyqt-openai-0.1.22/pyqt_openai/ico/user.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/inputDialog.py` & `pyqt-openai-0.1.22/pyqt_openai/inputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/leftSideBar.py` & `pyqt-openai-0.1.22/pyqt_openai/leftSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/main.py` & `pyqt-openai-0.1.22/pyqt_openai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,15 +435,15 @@
             if self.__remember_past_conv:
                 convs = []
                 with open('conv.json', 'r') as f:
                     for line in f:
                         conv = json.loads(line.strip())
                         convs.append(conv)
             # TODO refactoring
-            if info_dict['engine'] in ['gpt-3.5-turbo', 'gpt-3.5-turbo-0301']:
+            if info_dict['engine'] in ['gpt-3.5-turbo', 'gpt-3.5-turbo-0301', 'gpt-4']:
                 # "assistant" below is for making the AI remember the last question
                 openai_arg = {
                     'model': info_dict['engine'],
                     'messages': [
                         {"role": "system", "content": info_dict['system']},
                         {"role": "assistant", "content": self.__browser.getAllText()},
                         {"role": "user", "content": self.__lineEdit.toPlainText()},
@@ -493,25 +493,25 @@
         if f:
             self.setWindowFlags(self.windowFlags() | Qt.WindowStaysOnTopHint)
         else:
             self.setWindowFlags(self.windowFlags() & ~Qt.WindowStaysOnTopHint)
         self.show()
 
     def __executeCustomizeDialog(self):
-        dialog = CustomizeDialog()
+        dialog = CustomizeDialog(self)
         reply = dialog.exec()
         if reply == QDialog.Accepted:
             pass
 
     def __setTransparency(self, v):
         self.setWindowOpacity(v / 100)
 
     def closeEvent(self, e):
         message = 'The window has been closed. Would you like to continue running this app in the background?'
-        closeMessageBox = QMessageBox()
+        closeMessageBox = QMessageBox(self)
         closeMessageBox.setWindowTitle('Wait!')
         closeMessageBox.setText(message)
         closeMessageBox.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
         reply = closeMessageBox.exec()
         # Yes
         if reply == 16384:
             e.accept()
```

### Comparing `pyqt-openai-0.1.21/pyqt_openai/modelTable.py` & `pyqt-openai-0.1.22/pyqt_openai/modelTable.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/notifier.py` & `pyqt-openai-0.1.22/pyqt_openai/notifier.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/prompt/promptGeneratorWidget.py` & `pyqt-openai-0.1.22/pyqt_openai/prompt/promptGeneratorWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/prompt/propPage.py` & `pyqt-openai-0.1.22/pyqt_openai/prompt/propPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/prompt/templatePage.py` & `pyqt-openai-0.1.22/pyqt_openai/prompt/templatePage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/right_sidebar/aiPlaygroundWidget.py` & `pyqt-openai-0.1.22/pyqt_openai/right_sidebar/aiPlaygroundWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/right_sidebar/chatPage.py` & `pyqt-openai-0.1.22/pyqt_openai/right_sidebar/chatPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/right_sidebar/completionPage.py` & `pyqt-openai-0.1.22/pyqt_openai/right_sidebar/completionPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/right_sidebar/imagePage.py` & `pyqt-openai-0.1.22/pyqt_openai/right_sidebar/imagePage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/searchBar.py` & `pyqt-openai-0.1.22/pyqt_openai/searchBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/sqlite.py` & `pyqt-openai-0.1.22/pyqt_openai/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 if isinstance(self.__chat_default_value[col], str):
                     d_value = f'"{d_value}"' if len(self.__chat_default_value[col].split()) > 0 else d_value
                 self.__c.execute(f"ALTER TABLE {self.__info_tb_nm} ADD COLUMN {col} DEFAULT {d_value}")
         else:
             self.__c.execute(f'''CREATE TABLE {self.__info_tb_nm}
                                      (id INTEGER PRIMARY KEY,
                                       engine VARCHAR(50) DEFAULT '{self.__chat_default_value['engine']}',
-                                      engine TEXT DEFAULT '{self.__chat_default_value['system']}',
+                                      system TEXT DEFAULT '{self.__chat_default_value['system']}',
                                       temperature INTEGER DEFAULT {self.__chat_default_value['temperature']},
                                       max_tokens INTEGER DEFAULT {self.__chat_default_value['max_tokens']},
                                       top_p INTEGER DEFAULT {self.__chat_default_value['top_p']},
                                       frequency_penalty INTEGER DEFAULT {self.__chat_default_value['frequency_penalty']},
                                       presence_penalty INTEGER DEFAULT {self.__chat_default_value['presence_penalty']},
                                       stream BOOL DEFAULT {self.__chat_default_value['stream']},
```

### Comparing `pyqt-openai-0.1.21/pyqt_openai/svgButton.py` & `pyqt-openai-0.1.22/pyqt_openai/svgButton.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/svgLabel.py` & `pyqt-openai-0.1.22/pyqt_openai/svgLabel.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/test/htmlformat.py` & `pyqt-openai-0.1.22/pyqt_openai/test/htmlformat.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/test/rightSideBarTab.py` & `pyqt-openai-0.1.22/pyqt_openai/test/rightSideBarTab.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/delete_model.py` & `pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/delete_model.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/make_model.py` & `pyqt-openai-0.1.22/pyqt_openai/test/stable_diffusion/make_model.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.21/pyqt_openai.egg-info/PKG-INFO` & `pyqt-openai-0.1.22/pyqt_openai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.21
+Version: 0.1.22
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -37,24 +37,30 @@
 
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 Some of the features are still being tested.
 
+I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
+
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b>
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
-* support GPT-4
-* you can save the conversation history with sqlite database
+* conversation management
+  * add & delete conversations
+  * save conversations
+  * rename conversation
+  * everything above is saved in an SQLite database file named conv.db.
+* support GPT-4 and every other models below GPT3
 * support prompt generator
 * support image generation with DALL-E
-* you can test any models, including gpt3.5
 * you can run this in background application
+  * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.21 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.22 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot. Even though this
@@ -12,27 +12,32 @@
 for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
 nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
 generation feature available since v0.0.16. You can see the detail in official
 OpenAI site. Currently this feature is very basic now. This is using sqlite as
 a database. You can select the model at the right side bar. An internet
 connection is required. ## Contact You can join pyqt-openai's Discord_Server to
 have a conversation about it or AI-related stuff ð ## Note Some of the
-features are still being tested. ## Feature * basically this is desktop
-application version of ChatGPT * text streaming (enable by default, you can
-disable it) * AI remembers past conversation * support GPT-4 * you can save the
-conversation history with sqlite database * support prompt generator * support
-image generation with DALL-E * you can test any models, including gpt3.5 * you
-can run this in background application * you can make window stack on top or
-control its transparency ## Requirements * qtpy - the package allowing you to
-write code that works with both PyQt and PySide * PyQt5 >= 5.14 or PySide6 *
-openai ## Preview This is using GPT-3.5 turbo model by default. ### Homepage !
-[image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-
-2b8f-483b-9271-b78ab8a1eb73.png) You have to write your openai api key inside
-the red box. see [How to play](#how-to-play) ### Overview ![image](https://
-user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
+features are still being tested. I recommend to install sqlite management
+software. It's not necessary to run this app (obviously), but it's good
+practice to manage database about conversation history with AI and to know how
+this works. ## Feature * basically this is desktop application version of
+ChatGPT * text streaming (enable by default, you can disable it) * AI remembers
+past conversation * conversation management * add & delete conversations * save
+conversations * rename conversation * everything above is saved in an SQLite
+database file named conv.db. * support GPT-4 and every other models below GPT3
+* support prompt generator * support image generation with DALL-E * you can run
+this in background application * notification will pop up when response is
+generated * you can make window stack on top or control its transparency ##
+Requirements * qtpy - the package allowing you to write code that works with
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
+using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
+images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-
+b78ab8a1eb73.png) You have to write your openai api key inside the red box. see
+[How to play](#how-to-play) ### Overview ![image](https://user-
+images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
 e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
 user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
 7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
 55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
 Generator https://user-images.githubusercontent.com/55078043/236584481-
 b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
 lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
```

### Comparing `pyqt-openai-0.1.21/pyqt_openai.egg-info/SOURCES.txt` & `pyqt-openai-0.1.22/pyqt_openai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,14 @@
 pyqt_openai/prompt/templatePage.py
 pyqt_openai/right_sidebar/__init__.py
 pyqt_openai/right_sidebar/aiPlaygroundWidget.py
 pyqt_openai/right_sidebar/chatPage.py
 pyqt_openai/right_sidebar/completionPage.py
 pyqt_openai/right_sidebar/imagePage.py
 pyqt_openai/test/__init__.py
+pyqt_openai/test/dialog.py
 pyqt_openai/test/htmlformat.py
 pyqt_openai/test/rightSideBarTab.py
 pyqt_openai/test/stable_diffusion/__init__.py
 pyqt_openai/test/stable_diffusion/delete_model.py
 pyqt_openai/test/stable_diffusion/make_model.py
 pyqt_openai/test/stable_diffusion/using_model.py
```

### Comparing `pyqt-openai-0.1.21/setup.py` & `pyqt-openai-0.1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-openai',
-    version='0.1.21',
+    version='0.1.22',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
     package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'help.svg', 'customize.svg', 'user.svg',
                                       'sidebar.svg', 'prompt.svg', 'download.svg', 'stackontop.svg',
                                       'add.svg', 'delete.svg', 'setting.svg', 'search.svg']},
```

