# Comparing `tmp/pyqt-openai-0.1.2.tar.gz` & `tmp/pyqt-openai-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-openai-0.1.2.tar", last modified: Fri May  5 02:49:50 2023, max compression
+gzip compressed data, was "pyqt-openai-0.1.21.tar", last modified: Fri May  5 23:52:03 2023, max compression
```

## Comparing `pyqt-openai-0.1.2.tar` & `pyqt-openai-0.1.21.tar`

### file list

```diff
@@ -1,56 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.450469 pyqt-openai-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4736 2023-05-05 02:49:50.449469 pyqt-openai-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4351 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.342585 pyqt-openai-0.1.2/pyqt_openai/
--rw-rw-rw-   0        0        0       25 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/__init__.py
--rw-rw-rw-   0        0        0     6738 2023-04-09 06:45:06.000000 pyqt-openai-0.1.2/pyqt_openai/a.py
--rw-rw-rw-   0        0        0     2144 2023-05-05 02:48:09.000000 pyqt-openai-0.1.2/pyqt_openai/apiData.py
--rw-rw-rw-   0        0        0     6771 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/chatWidget.py
--rw-rw-rw-   0        0        0     8132 2023-04-08 11:47:46.000000 pyqt-openai-0.1.2/pyqt_openai/clickableTooltip.py
--rw-rw-rw-   0        0        0     5072 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/convListWidget.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.405931 pyqt-openai-0.1.2/pyqt_openai/ico/
--rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.2/pyqt_openai/ico/__init__.py
--rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/add.svg
--rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.2/pyqt_openai/ico/close.svg
--rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/delete.svg
--rw-rw-rw-   0        0        0      654 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/download.svg
--rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/help.svg
--rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.2/pyqt_openai/ico/openai.svg
--rw-rw-rw-   0        0        0      501 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/ico/prompt.svg
--rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/search.svg
--rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/setting.svg
--rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.2/pyqt_openai/ico/sidebar.svg
--rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.2/pyqt_openai/ico/stackontop.svg
--rw-rw-rw-   0        0        0     1383 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/inputDialog.py
--rw-rw-rw-   0        0        0     3768 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/leftSideBar.py
--rw-rw-rw-   0        0        0    21864 2023-05-05 02:49:02.000000 pyqt-openai-0.1.2/pyqt_openai/main.py
--rw-rw-rw-   0        0        0     1788 2023-04-08 11:47:46.000000 pyqt-openai-0.1.2/pyqt_openai/modelTable.py
--rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.2/pyqt_openai/notifier.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.413224 pyqt-openai-0.1.2/pyqt_openai/prompt/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/prompt/__init__.py
--rw-rw-rw-   0        0        0     1721 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/prompt/promptGeneratorWidget.py
--rw-rw-rw-   0        0        0     1574 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/prompt/propPage.py
--rw-rw-rw-   0        0        0     3351 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/prompt/templatePage.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.428156 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/
--rw-rw-rw-   0        0        0       39 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/__init__.py
--rw-rw-rw-   0        0        0     2220 2023-05-05 00:11:49.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
--rw-rw-rw-   0        0        0     4706 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/chatPage.py
--rw-rw-rw-   0        0        0    11101 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/completionPage.py
--rw-rw-rw-   0        0        0     1623 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/imagePage.py
--rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/searchBar.py
--rw-rw-rw-   0        0        0    21685 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/sqlite.py
--rw-rw-rw-   0        0        0     5931 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/svgButton.py
--rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.2/pyqt_openai/svgLabel.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.447474 pyqt-openai-0.1.2/pyqt_openai/test/
--rw-rw-rw-   0        0        0        0 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/test/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/test/htmlformat.py
--rw-rw-rw-   0        0        0     1280 2023-04-23 09:02:45.000000 pyqt-openai-0.1.2/pyqt_openai/test/rightSideBarTab.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.379999 pyqt-openai-0.1.2/pyqt_openai.egg-info/
--rw-rw-rw-   0        0        0     4736 2023-05-05 02:49:49.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1343 2023-05-05 02:49:50.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 02:49:49.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-05 02:49:49.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 02:49:49.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 02:49:50.450469 pyqt-openai-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      958 2023-05-05 02:31:28.000000 pyqt-openai-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.314478 pyqt-openai-0.1.21/
+-rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.21/LICENSE
+-rw-rw-rw-   0        0        0     5104 2023-05-05 23:52:03.312481 pyqt-openai-0.1.21/PKG-INFO
+-rw-rw-rw-   0        0        0     4710 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.093038 pyqt-openai-0.1.21/pyqt_openai/
+-rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/__init__.py
+-rw-rw-rw-   0        0        0     6738 2023-04-09 06:45:06.000000 pyqt-openai-0.1.21/pyqt_openai/a.py
+-rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/apiData.py
+-rw-rw-rw-   0        0        0     6771 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/chatWidget.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/circleProfileImage.py
+-rw-rw-rw-   0        0        0     8132 2023-04-08 11:47:46.000000 pyqt-openai-0.1.21/pyqt_openai/clickableTooltip.py
+-rw-rw-rw-   0        0        0     5072 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/convListWidget.py
+-rw-rw-rw-   0        0        0     7583 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/customizeDialog.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.159860 pyqt-openai-0.1.21/pyqt_openai/ico/
+-rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.21/pyqt_openai/ico/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/add.svg
+-rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.21/pyqt_openai/ico/close.svg
+-rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/ico/customize.svg
+-rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/delete.svg
+-rw-rw-rw-   0        0        0      654 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/download.svg
+-rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/help.svg
+-rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.21/pyqt_openai/ico/openai.svg
+-rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/ico/prompt.svg
+-rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/search.svg
+-rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/ico/setting.svg
+-rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.21/pyqt_openai/ico/sidebar.svg
+-rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.21/pyqt_openai/ico/stackontop.svg
+-rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/ico/user.svg
+-rw-rw-rw-   0        0        0     1383 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/inputDialog.py
+-rw-rw-rw-   0        0        0     3768 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/leftSideBar.py
+-rw-rw-rw-   0        0        0    22515 2023-05-05 23:44:44.000000 pyqt-openai-0.1.21/pyqt_openai/main.py
+-rw-rw-rw-   0        0        0     1788 2023-04-08 11:47:46.000000 pyqt-openai-0.1.21/pyqt_openai/modelTable.py
+-rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.21/pyqt_openai/notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.193285 pyqt-openai-0.1.21/pyqt_openai/prompt/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/prompt/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/prompt/promptGeneratorWidget.py
+-rw-rw-rw-   0        0        0     1574 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/prompt/propPage.py
+-rw-rw-rw-   0        0        0     3351 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/prompt/templatePage.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.247142 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/
+-rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/__init__.py
+-rw-rw-rw-   0        0        0     2220 2023-05-05 02:57:06.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
+-rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/chatPage.py
+-rw-rw-rw-   0        0        0    11101 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/completionPage.py
+-rw-rw-rw-   0        0        0     1623 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/right_sidebar/imagePage.py
+-rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/searchBar.py
+-rw-rw-rw-   0        0        0    21685 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/sqlite.py
+-rw-rw-rw-   0        0        0     5931 2023-04-22 00:05:31.000000 pyqt-openai-0.1.21/pyqt_openai/svgButton.py
+-rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.21/pyqt_openai/svgLabel.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.275074 pyqt-openai-0.1.21/pyqt_openai/test/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/test/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-05-05 02:56:55.000000 pyqt-openai-0.1.21/pyqt_openai/test/htmlformat.py
+-rw-rw-rw-   0        0        0     1280 2023-04-23 09:02:45.000000 pyqt-openai-0.1.21/pyqt_openai/test/rightSideBarTab.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.310487 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/
+-rw-rw-rw-   0        0        0        0 2023-05-05 07:22:12.000000 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/__init__.py
+-rw-rw-rw-   0        0        0      722 2023-05-05 12:31:35.000000 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/delete_model.py
+-rw-rw-rw-   0        0        0     2559 2023-05-05 07:22:36.000000 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/make_model.py
+-rw-rw-rw-   0        0        0      433 2023-05-05 08:36:36.000000 pyqt-openai-0.1.21/pyqt_openai/test/stable_diffusion/using_model.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:52:03.129975 pyqt-openai-0.1.21/pyqt_openai.egg-info/
+-rw-rw-rw-   0        0        0     5104 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1656 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 23:52:02.000000 pyqt-openai-0.1.21/pyqt_openai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 23:52:03.314478 pyqt-openai-0.1.21/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-05-05 23:45:36.000000 pyqt-openai-0.1.21/setup.py
```

### Comparing `pyqt-openai-0.1.2/LICENSE` & `pyqt-openai-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/PKG-INFO` & `pyqt-openai-0.1.21/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.2
+Version: 0.1.21
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,57 +21,67 @@
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
-The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default.
+The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
 Image generation feature available since v0.0.16. You can see the detail in <a href="https://platform.openai.com/docs/guides/images/introduction">official OpenAI</a> site. Currently this feature is very basic now.
 
 This is using <b>sqlite</b> as a database.
 
-You can select other model with the combobox on the sidebar at the right side of the window.
+You can select the model at the right side bar.
 
 An internet connection is required.
 
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 Some of the features are still being tested.
 
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b>
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
+* support GPT-4
 * you can save the conversation history with sqlite database
+* support prompt generator
 * support image generation with DALL-E
 * you can test any models, including gpt3.5
 * you can run this in background application
-* you can make window stack on top or control its transparency 
+* you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 
 ## Preview
 This is using GPT-3.5 turbo model by default.
 
 ### Homepage
-![image](https://user-images.githubusercontent.com/55078043/230718379-d8f85397-74e9-483a-8686-5ce59ead70a3.png)
+![image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-b78ab8a1eb73.png)
 <b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
 
+### Overview
+![image](https://user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-e502a182264d.png)
+
 ### Conversation preview
-#### Image
-![image](https://user-images.githubusercontent.com/55078043/230718925-bc36693b-1ad6-472f-ab08-63517e3a433f.png)
-#### Video
-https://user-images.githubusercontent.com/55078043/230719180-3e665a05-959c-4b49-b693-7046a538630e.mp4
+#### Preview Image
+![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
+#### Preview Video
+https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
+
+### Prompt Generator
+https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
+
+So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
 
 ## How to play
 1. git clone ~
 2. from the root directory, type "cd pyqt_openai"
 3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
@@ -91,24 +101,22 @@
 ```
 python setup.py install
 ```
 
 That will install the openai.
 
 ## TODO list
-* redesign the right side bar
-* prompt generator
-* support MidJourney or Stable Diffusion or both
+* support Stable Diffusion
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
 * save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
 * add the basic example sources of making deep learning model with PyTorch (eventually)
 
 ## See Also
 * <a href="https://learn.microsoft.com/en-us/azure/cognitive-services/openai/overview">Azure OpenAI service</a>
-* <a href="https://openai.com/waitlist/gpt-4-api">join gpt4 waitlist</a>
+* <a href="https://openai.com/waitlist/gpt-4-api">join gpt4 waitlist</a> - i took 1 month to get access from it
 * <a href="https://https://openai.com/waitlist/plugins">join chatgpt plugins waitlist</a>
```

#### html2text {}

```diff
@@ -1,52 +1,56 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.2 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.21 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot. Even though this
 project has become too huge to be called an 'example'. The major advantage of
 this package is that you don't need to know other language aside from Python.
 If you want to study openai with Python-only good old desktop software, this is
 for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
-nearly as functional as ChatGPT) by default. Image generation feature available
-since v0.0.16. You can see the detail in official_OpenAI site. Currently this
-feature is very basic now. This is using sqlite as a database. You can select
-other model with the combobox on the sidebar at the right side of the window.
-An internet connection is required. ## Contact You can join pyqt-openai's
-Discord_Server to have a conversation about it or AI-related stuff ð ## Note
-Some of the features are still being tested. ## Feature * basically this is
-desktop application version of ChatGPT * text streaming (enable by default, you
-can disable it) * AI remembers past conversation * you can save the
-conversation history with sqlite database * support image generation with DALL-
-E * you can test any models, including gpt3.5 * you can run this in background
-application * you can make window stack on top or control its transparency ##
-Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
-using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/230718379-d8f85397-74e9-483a-8686-
-5ce59ead70a3.png) You have to write your openai api key inside the red box. see
-[How to play](#how-to-play) ### Conversation preview #### Image ![image](https:
-//user-images.githubusercontent.com/55078043/230718925-bc36693b-1ad6-472f-ab08-
-63517e3a433f.png) #### Video https://user-images.githubusercontent.com/
-55078043/230719180-3e665a05-959c-4b49-b693-7046a538630e.mp4 ## How to play 1.
-git clone ~ 2. from the root directory, type "cd pyqt_openai" 3. You should put
-your api key in the line edit. You can get it in official_site of openai. Sign
-up and log in before you get it. By the way, this is free trial, not
-permanently free. See this after you have logged in. Be sure, this is a very
-important API key that belongs to you only, so you should remember it and keep
-it secure. 4. python main.py If installation doesn't work, check the
-troubleshooting below. ## Troubleshooting If you see this error while
-installing the openai package ``` subprocess-exited-with-error ``` you can
-shout a curse word and just download the package itself from pypi. Unzip it,
-access the package directory, type ``` python setup.py install ``` That will
-install the openai. ## TODO list * redesign the right side bar * prompt
-generator * support MidJourney or Stable Diffusion or both * show the
-explanation of every model and terms related to AI (e.g. temperature, topp..) *
-save conversation history with other format (xlsx, csv, etc.) * tokenizer *
-highlight the source (optional, eventually) * support multiple language * use
-SQLAlchemy (maybe not) * show reason when the chat input is disabled for some
-reasons * add the basic example sources of making deep learning model with
-PyTorch (eventually) ## See Also * Azure_OpenAI_service * join_gpt4_waitlist *
-join_chatgpt_plugins_waitlist
+nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
+generation feature available since v0.0.16. You can see the detail in official
+OpenAI site. Currently this feature is very basic now. This is using sqlite as
+a database. You can select the model at the right side bar. An internet
+connection is required. ## Contact You can join pyqt-openai's Discord_Server to
+have a conversation about it or AI-related stuff ð ## Note Some of the
+features are still being tested. ## Feature * basically this is desktop
+application version of ChatGPT * text streaming (enable by default, you can
+disable it) * AI remembers past conversation * support GPT-4 * you can save the
+conversation history with sqlite database * support prompt generator * support
+image generation with DALL-E * you can test any models, including gpt3.5 * you
+can run this in background application * you can make window stack on top or
+control its transparency ## Requirements * qtpy - the package allowing you to
+write code that works with both PyQt and PySide * PyQt5 >= 5.14 or PySide6 *
+openai ## Preview This is using GPT-3.5 turbo model by default. ### Homepage !
+[image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-
+2b8f-483b-9271-b78ab8a1eb73.png) You have to write your openai api key inside
+the red box. see [How to play](#how-to-play) ### Overview ![image](https://
+user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
+e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
+user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
+7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
+55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
+Generator https://user-images.githubusercontent.com/55078043/236584481-
+b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
+lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
+~ 2. from the root directory, type "cd pyqt_openai" 3. You should put your api
+key in the line edit. You can get it in official_site of openai. Sign up and
+log in before you get it. By the way, this is free trial, not permanently free.
+See this after you have logged in. Be sure, this is a very important API key
+that belongs to you only, so you should remember it and keep it secure. 4.
+python main.py If installation doesn't work, check the troubleshooting below.
+## Troubleshooting If you see this error while installing the openai package
+``` subprocess-exited-with-error ``` you can shout a curse word and just
+download the package itself from pypi. Unzip it, access the package directory,
+type ``` python setup.py install ``` That will install the openai. ## TODO list
+* support Stable Diffusion * show the explanation of every model and terms
+related to AI (e.g. temperature, topp..) * save conversation history with other
+format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
+eventually) * support multiple language * use SQLAlchemy (maybe not) * show
+reason when the chat input is disabled for some reasons * add the basic example
+sources of making deep learning model with PyTorch (eventually) ## See Also *
+Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
+it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.2/README.md` & `pyqt-openai-0.1.21/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,57 +9,67 @@
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
-The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default.
+The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
 Image generation feature available since v0.0.16. You can see the detail in <a href="https://platform.openai.com/docs/guides/images/introduction">official OpenAI</a> site. Currently this feature is very basic now.
 
 This is using <b>sqlite</b> as a database.
 
-You can select other model with the combobox on the sidebar at the right side of the window.
+You can select the model at the right side bar.
 
 An internet connection is required.
 
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 Some of the features are still being tested.
 
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b>
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
+* support GPT-4
 * you can save the conversation history with sqlite database
+* support prompt generator
 * support image generation with DALL-E
 * you can test any models, including gpt3.5
 * you can run this in background application
-* you can make window stack on top or control its transparency 
+* you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 
 ## Preview
 This is using GPT-3.5 turbo model by default.
 
 ### Homepage
-![image](https://user-images.githubusercontent.com/55078043/230718379-d8f85397-74e9-483a-8686-5ce59ead70a3.png)
+![image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-b78ab8a1eb73.png)
 <b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
 
+### Overview
+![image](https://user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-e502a182264d.png)
+
 ### Conversation preview
-#### Image
-![image](https://user-images.githubusercontent.com/55078043/230718925-bc36693b-1ad6-472f-ab08-63517e3a433f.png)
-#### Video
-https://user-images.githubusercontent.com/55078043/230719180-3e665a05-959c-4b49-b693-7046a538630e.mp4
+#### Preview Image
+![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
+#### Preview Video
+https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
+
+### Prompt Generator
+https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
+
+So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
 
 ## How to play
 1. git clone ~
 2. from the root directory, type "cd pyqt_openai"
 3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
@@ -79,24 +89,22 @@
 ```
 python setup.py install
 ```
 
 That will install the openai.
 
 ## TODO list
-* redesign the right side bar
-* prompt generator
-* support MidJourney or Stable Diffusion or both
+* support Stable Diffusion
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
 * save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
 * add the basic example sources of making deep learning model with PyTorch (eventually)
 
 ## See Also
 * <a href="https://learn.microsoft.com/en-us/azure/cognitive-services/openai/overview">Azure OpenAI service</a>
-* <a href="https://openai.com/waitlist/gpt-4-api">join gpt4 waitlist</a>
+* <a href="https://openai.com/waitlist/gpt-4-api">join gpt4 waitlist</a> - i took 1 month to get access from it
 * <a href="https://https://openai.com/waitlist/plugins">join chatgpt plugins waitlist</a>
```

#### html2text {}

```diff
@@ -3,47 +3,51 @@
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot. Even though this
 project has become too huge to be called an 'example'. The major advantage of
 this package is that you don't need to know other language aside from Python.
 If you want to study openai with Python-only good old desktop software, this is
 for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
-nearly as functional as ChatGPT) by default. Image generation feature available
-since v0.0.16. You can see the detail in official_OpenAI site. Currently this
-feature is very basic now. This is using sqlite as a database. You can select
-other model with the combobox on the sidebar at the right side of the window.
-An internet connection is required. ## Contact You can join pyqt-openai's
-Discord_Server to have a conversation about it or AI-related stuff ð ## Note
-Some of the features are still being tested. ## Feature * basically this is
-desktop application version of ChatGPT * text streaming (enable by default, you
-can disable it) * AI remembers past conversation * you can save the
-conversation history with sqlite database * support image generation with DALL-
-E * you can test any models, including gpt3.5 * you can run this in background
-application * you can make window stack on top or control its transparency ##
-Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
-using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/230718379-d8f85397-74e9-483a-8686-
-5ce59ead70a3.png) You have to write your openai api key inside the red box. see
-[How to play](#how-to-play) ### Conversation preview #### Image ![image](https:
-//user-images.githubusercontent.com/55078043/230718925-bc36693b-1ad6-472f-ab08-
-63517e3a433f.png) #### Video https://user-images.githubusercontent.com/
-55078043/230719180-3e665a05-959c-4b49-b693-7046a538630e.mp4 ## How to play 1.
-git clone ~ 2. from the root directory, type "cd pyqt_openai" 3. You should put
-your api key in the line edit. You can get it in official_site of openai. Sign
-up and log in before you get it. By the way, this is free trial, not
-permanently free. See this after you have logged in. Be sure, this is a very
-important API key that belongs to you only, so you should remember it and keep
-it secure. 4. python main.py If installation doesn't work, check the
-troubleshooting below. ## Troubleshooting If you see this error while
-installing the openai package ``` subprocess-exited-with-error ``` you can
-shout a curse word and just download the package itself from pypi. Unzip it,
-access the package directory, type ``` python setup.py install ``` That will
-install the openai. ## TODO list * redesign the right side bar * prompt
-generator * support MidJourney or Stable Diffusion or both * show the
-explanation of every model and terms related to AI (e.g. temperature, topp..) *
-save conversation history with other format (xlsx, csv, etc.) * tokenizer *
-highlight the source (optional, eventually) * support multiple language * use
-SQLAlchemy (maybe not) * show reason when the chat input is disabled for some
-reasons * add the basic example sources of making deep learning model with
-PyTorch (eventually) ## See Also * Azure_OpenAI_service * join_gpt4_waitlist *
-join_chatgpt_plugins_waitlist
+nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
+generation feature available since v0.0.16. You can see the detail in official
+OpenAI site. Currently this feature is very basic now. This is using sqlite as
+a database. You can select the model at the right side bar. An internet
+connection is required. ## Contact You can join pyqt-openai's Discord_Server to
+have a conversation about it or AI-related stuff ð ## Note Some of the
+features are still being tested. ## Feature * basically this is desktop
+application version of ChatGPT * text streaming (enable by default, you can
+disable it) * AI remembers past conversation * support GPT-4 * you can save the
+conversation history with sqlite database * support prompt generator * support
+image generation with DALL-E * you can test any models, including gpt3.5 * you
+can run this in background application * you can make window stack on top or
+control its transparency ## Requirements * qtpy - the package allowing you to
+write code that works with both PyQt and PySide * PyQt5 >= 5.14 or PySide6 *
+openai ## Preview This is using GPT-3.5 turbo model by default. ### Homepage !
+[image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-
+2b8f-483b-9271-b78ab8a1eb73.png) You have to write your openai api key inside
+the red box. see [How to play](#how-to-play) ### Overview ![image](https://
+user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
+e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
+user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
+7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
+55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
+Generator https://user-images.githubusercontent.com/55078043/236584481-
+b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
+lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
+~ 2. from the root directory, type "cd pyqt_openai" 3. You should put your api
+key in the line edit. You can get it in official_site of openai. Sign up and
+log in before you get it. By the way, this is free trial, not permanently free.
+See this after you have logged in. Be sure, this is a very important API key
+that belongs to you only, so you should remember it and keep it secure. 4.
+python main.py If installation doesn't work, check the troubleshooting below.
+## Troubleshooting If you see this error while installing the openai package
+``` subprocess-exited-with-error ``` you can shout a curse word and just
+download the package itself from pypi. Unzip it, access the package directory,
+type ``` python setup.py install ``` That will install the openai. ## TODO list
+* support Stable Diffusion * show the explanation of every model and terms
+related to AI (e.g. temperature, topp..) * save conversation history with other
+format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
+eventually) * support multiple language * use SQLAlchemy (maybe not) * show
+reason when the chat input is disabled for some reasons * add the basic example
+sources of making deep learning model with PyTorch (eventually) ## See Also *
+Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
+it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.2/pyqt_openai/a.py` & `pyqt-openai-0.1.21/pyqt_openai/a.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/apiData.py` & `pyqt-openai-0.1.21/pyqt_openai/apiData.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/chatWidget.py` & `pyqt-openai-0.1.21/pyqt_openai/chatWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/clickableTooltip.py` & `pyqt-openai-0.1.21/pyqt_openai/clickableTooltip.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/convListWidget.py` & `pyqt-openai-0.1.21/pyqt_openai/convListWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/ico/close.svg` & `pyqt-openai-0.1.21/pyqt_openai/ico/close.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/ico/download.svg` & `pyqt-openai-0.1.21/pyqt_openai/ico/download.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/ico/help.svg` & `pyqt-openai-0.1.21/pyqt_openai/ico/help.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/ico/openai.svg` & `pyqt-openai-0.1.21/pyqt_openai/ico/openai.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/ico/search.svg` & `pyqt-openai-0.1.21/pyqt_openai/ico/search.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/ico/setting.svg` & `pyqt-openai-0.1.21/pyqt_openai/ico/setting.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/ico/stackontop.svg` & `pyqt-openai-0.1.21/pyqt_openai/ico/stackontop.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/inputDialog.py` & `pyqt-openai-0.1.21/pyqt_openai/inputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/leftSideBar.py` & `pyqt-openai-0.1.21/pyqt_openai/leftSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/main.py` & `pyqt-openai-0.1.21/pyqt_openai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 from chatWidget import Prompt, ChatBrowser
 
 from notifier import NotifierWidget
 
 from qtpy.QtCore import Qt, QCoreApplication, QThread, QSettings, QEvent, Signal
 from qtpy.QtGui import QGuiApplication, QFont, QIcon, QColor, QCursor
-from qtpy.QtWidgets import QMainWindow, QApplication, QVBoxLayout, QWidget, QSplitter, QComboBox, QSpinBox, \
+from qtpy.QtWidgets import QMainWindow, QApplication, QVBoxLayout, QWidget, QSplitter, QDialog, QSpinBox, \
     QFileDialog, QToolBar, QWidgetAction, QHBoxLayout, QAction, QMenu, \
     QSystemTrayIcon, QMessageBox, QSizePolicy, QLabel, QListWidgetItem, QLineEdit, QPushButton
 
 from pyqt_openai.apiData import getModelEndpoint
 from pyqt_openai.clickableTooltip import ClickableTooltip
+from pyqt_openai.customizeDialog import CustomizeDialog
 from pyqt_openai.leftSideBar import LeftSideBar
 from pyqt_openai.apiData import ModelData
 from pyqt_openai.prompt.promptGeneratorWidget import PromptGeneratorWidget
 from pyqt_openai.right_sidebar.aiPlaygroundWidget import AIPlaygroundWidget
 from pyqt_openai.svgButton import SvgButton
 from pyqt_openai.sqlite import SqliteDatabase
 
@@ -271,33 +272,40 @@
         self.__stackBtn = SvgButton()
         self.__stackBtn.setIcon('ico/stackontop.svg')
         self.__stackBtn.setCheckable(True)
         self.__stackBtn.toggled.connect(self.__stackToggle)
         self.__stackAction.setDefaultWidget(self.__stackBtn)
         self.__stackBtn.setToolTip('Always On Top')
 
-        self.__sideBarAction = QWidgetAction(self)
+        self.__leftSideBarAction = QWidgetAction(self)
         self.__sideBarBtn = SvgButton()
         self.__sideBarBtn.setIcon('ico/sidebar.svg')
         self.__sideBarBtn.setCheckable(True)
         self.__sideBarBtn.toggled.connect(self.__leftSideBarWidget.setVisible)
-        self.__sideBarAction.setDefaultWidget(self.__sideBarBtn)
+        self.__leftSideBarAction.setDefaultWidget(self.__sideBarBtn)
         self.__sideBarBtn.setToolTip('Chat List')
         self.__sideBarBtn.setChecked(True)
 
         self.__settingAction = QWidgetAction(self)
         self.__settingBtn = SvgButton()
         self.__settingBtn.setIcon('ico/setting.svg')
         self.__settingBtn.toggled.connect(self.__aiPlaygroundWidget.setVisible)
         self.__settingAction.setDefaultWidget(self.__settingBtn)
         self.__settingBtn.setToolTip('Settings')
         self.__settingBtn.setCheckable(True)
         self.__settingBtn.setChecked(True)
         self.__settingBtn.setChecked(False)
 
+        self.__customizeAction = QWidgetAction(self)
+        self.__customizeBtn = SvgButton()
+        self.__customizeBtn.setIcon('ico/customize.svg')
+        self.__customizeBtn.clicked.connect(self.__executeCustomizeDialog)
+        self.__customizeAction.setDefaultWidget(self.__customizeBtn)
+        self.__customizeBtn.setToolTip('Customize (working)')
+
         self.__promptAction = QWidgetAction(self)
         self.__promptBtn = SvgButton()
         self.__promptBtn.setIcon('ico/prompt.svg')
         self.__promptAction.setDefaultWidget(self.__promptBtn)
         self.__promptBtn.toggled.connect(self.__promptGeneratorWidget.setVisible)
         self.__promptBtn.setToolTip('Prompt Generator')
         self.__promptBtn.setCheckable(True)
@@ -347,17 +355,18 @@
         if reason == 3:
             self.show()
 
     def __setToolBar(self):
         toolbar = QToolBar()
         lay = QHBoxLayout()
         toolbar.addAction(self.__stackAction)
-        toolbar.addAction(self.__sideBarAction)
+        toolbar.addAction(self.__leftSideBarAction)
         toolbar.addAction(self.__settingAction)
         toolbar.addAction(self.__promptAction)
+        toolbar.addAction(self.__customizeAction)
         toolbar.addAction(self.__transparentAction)
         toolbar.addAction(self.__apiAction)
         toolbar.setLayout(lay)
         toolbar.setMovable(False)
         self.addToolBar(toolbar)
         # QToolbar's layout can't be set spacing with lay.setSpacing so i've just did this instead
         toolbar.setStyleSheet('QToolBar { spacing: 2px; }')
@@ -483,14 +492,20 @@
     def __stackToggle(self, f):
         if f:
             self.setWindowFlags(self.windowFlags() | Qt.WindowStaysOnTopHint)
         else:
             self.setWindowFlags(self.windowFlags() & ~Qt.WindowStaysOnTopHint)
         self.show()
 
+    def __executeCustomizeDialog(self):
+        dialog = CustomizeDialog()
+        reply = dialog.exec()
+        if reply == QDialog.Accepted:
+            pass
+
     def __setTransparency(self, v):
         self.setWindowOpacity(v / 100)
 
     def closeEvent(self, e):
         message = 'The window has been closed. Would you like to continue running this app in the background?'
         closeMessageBox = QMessageBox()
         closeMessageBox.setWindowTitle('Wait!')
```

### Comparing `pyqt-openai-0.1.2/pyqt_openai/modelTable.py` & `pyqt-openai-0.1.21/pyqt_openai/modelTable.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/notifier.py` & `pyqt-openai-0.1.21/pyqt_openai/notifier.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/prompt/promptGeneratorWidget.py` & `pyqt-openai-0.1.21/pyqt_openai/prompt/promptGeneratorWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/prompt/propPage.py` & `pyqt-openai-0.1.21/pyqt_openai/prompt/propPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/prompt/templatePage.py` & `pyqt-openai-0.1.21/pyqt_openai/prompt/templatePage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/right_sidebar/aiPlaygroundWidget.py` & `pyqt-openai-0.1.21/pyqt_openai/right_sidebar/aiPlaygroundWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/right_sidebar/chatPage.py` & `pyqt-openai-0.1.21/pyqt_openai/right_sidebar/chatPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/right_sidebar/completionPage.py` & `pyqt-openai-0.1.21/pyqt_openai/right_sidebar/completionPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/right_sidebar/imagePage.py` & `pyqt-openai-0.1.21/pyqt_openai/right_sidebar/imagePage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/searchBar.py` & `pyqt-openai-0.1.21/pyqt_openai/searchBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/sqlite.py` & `pyqt-openai-0.1.21/pyqt_openai/sqlite.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/svgButton.py` & `pyqt-openai-0.1.21/pyqt_openai/svgButton.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/svgLabel.py` & `pyqt-openai-0.1.21/pyqt_openai/svgLabel.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/test/htmlformat.py` & `pyqt-openai-0.1.21/pyqt_openai/test/htmlformat.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai/test/rightSideBarTab.py` & `pyqt-openai-0.1.21/pyqt_openai/test/rightSideBarTab.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.2/pyqt_openai.egg-info/PKG-INFO` & `pyqt-openai-0.1.21/pyqt_openai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.2
+Version: 0.1.21
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,57 +21,67 @@
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
-The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default.
+The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
 Image generation feature available since v0.0.16. You can see the detail in <a href="https://platform.openai.com/docs/guides/images/introduction">official OpenAI</a> site. Currently this feature is very basic now.
 
 This is using <b>sqlite</b> as a database.
 
-You can select other model with the combobox on the sidebar at the right side of the window.
+You can select the model at the right side bar.
 
 An internet connection is required.
 
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 Some of the features are still being tested.
 
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b>
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
+* support GPT-4
 * you can save the conversation history with sqlite database
+* support prompt generator
 * support image generation with DALL-E
 * you can test any models, including gpt3.5
 * you can run this in background application
-* you can make window stack on top or control its transparency 
+* you can make window stack on top or control its transparency
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 
 ## Preview
 This is using GPT-3.5 turbo model by default.
 
 ### Homepage
-![image](https://user-images.githubusercontent.com/55078043/230718379-d8f85397-74e9-483a-8686-5ce59ead70a3.png)
+![image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-2b8f-483b-9271-b78ab8a1eb73.png)
 <b>You have to write your openai api key inside the red box.</b> see [How to play](#how-to-play)
 
+### Overview
+![image](https://user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-e502a182264d.png)
+
 ### Conversation preview
-#### Image
-![image](https://user-images.githubusercontent.com/55078043/230718925-bc36693b-1ad6-472f-ab08-63517e3a433f.png)
-#### Video
-https://user-images.githubusercontent.com/55078043/230719180-3e665a05-959c-4b49-b693-7046a538630e.mp4
+#### Preview Image
+![image](https://user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-7daa8e41b525.png)
+#### Preview Video
+https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
+
+### Prompt Generator
+https://user-images.githubusercontent.com/55078043/236584481-b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4
+
+So sorry to weak preview, but i have a lot of idea about this prompt generator! Just wait. 
 
 ## How to play
 1. git clone ~
 2. from the root directory, type "cd pyqt_openai"
 3. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it. <b>By the way, this is free trial, not permanently free. See <a href="https://platform.openai.com/account/billing/overview">this</a> after you have logged in.</b>
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
@@ -91,24 +101,22 @@
 ```
 python setup.py install
 ```
 
 That will install the openai.
 
 ## TODO list
-* redesign the right side bar
-* prompt generator
-* support MidJourney or Stable Diffusion or both
+* support Stable Diffusion
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
 * save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
 * add the basic example sources of making deep learning model with PyTorch (eventually)
 
 ## See Also
 * <a href="https://learn.microsoft.com/en-us/azure/cognitive-services/openai/overview">Azure OpenAI service</a>
-* <a href="https://openai.com/waitlist/gpt-4-api">join gpt4 waitlist</a>
+* <a href="https://openai.com/waitlist/gpt-4-api">join gpt4 waitlist</a> - i took 1 month to get access from it
 * <a href="https://https://openai.com/waitlist/plugins">join chatgpt plugins waitlist</a>
```

#### html2text {}

```diff
@@ -1,52 +1,56 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.2 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.21 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot. Even though this
 project has become too huge to be called an 'example'. The major advantage of
 this package is that you don't need to know other language aside from Python.
 If you want to study openai with Python-only good old desktop software, this is
 for you. The OpenAI model this package uses is the gpt-3.5-turbo model(which is
-nearly as functional as ChatGPT) by default. Image generation feature available
-since v0.0.16. You can see the detail in official_OpenAI site. Currently this
-feature is very basic now. This is using sqlite as a database. You can select
-other model with the combobox on the sidebar at the right side of the window.
-An internet connection is required. ## Contact You can join pyqt-openai's
-Discord_Server to have a conversation about it or AI-related stuff ð ## Note
-Some of the features are still being tested. ## Feature * basically this is
-desktop application version of ChatGPT * text streaming (enable by default, you
-can disable it) * AI remembers past conversation * you can save the
-conversation history with sqlite database * support image generation with DALL-
-E * you can test any models, including gpt3.5 * you can run this in background
-application * you can make window stack on top or control its transparency ##
-Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai ## Preview This is
-using GPT-3.5 turbo model by default. ### Homepage ![image](https://user-
-images.githubusercontent.com/55078043/230718379-d8f85397-74e9-483a-8686-
-5ce59ead70a3.png) You have to write your openai api key inside the red box. see
-[How to play](#how-to-play) ### Conversation preview #### Image ![image](https:
-//user-images.githubusercontent.com/55078043/230718925-bc36693b-1ad6-472f-ab08-
-63517e3a433f.png) #### Video https://user-images.githubusercontent.com/
-55078043/230719180-3e665a05-959c-4b49-b693-7046a538630e.mp4 ## How to play 1.
-git clone ~ 2. from the root directory, type "cd pyqt_openai" 3. You should put
-your api key in the line edit. You can get it in official_site of openai. Sign
-up and log in before you get it. By the way, this is free trial, not
-permanently free. See this after you have logged in. Be sure, this is a very
-important API key that belongs to you only, so you should remember it and keep
-it secure. 4. python main.py If installation doesn't work, check the
-troubleshooting below. ## Troubleshooting If you see this error while
-installing the openai package ``` subprocess-exited-with-error ``` you can
-shout a curse word and just download the package itself from pypi. Unzip it,
-access the package directory, type ``` python setup.py install ``` That will
-install the openai. ## TODO list * redesign the right side bar * prompt
-generator * support MidJourney or Stable Diffusion or both * show the
-explanation of every model and terms related to AI (e.g. temperature, topp..) *
-save conversation history with other format (xlsx, csv, etc.) * tokenizer *
-highlight the source (optional, eventually) * support multiple language * use
-SQLAlchemy (maybe not) * show reason when the chat input is disabled for some
-reasons * add the basic example sources of making deep learning model with
-PyTorch (eventually) ## See Also * Azure_OpenAI_service * join_gpt4_waitlist *
-join_chatgpt_plugins_waitlist
+nearly as functional as ChatGPT) by default. You can use gpt-4 as well. Image
+generation feature available since v0.0.16. You can see the detail in official
+OpenAI site. Currently this feature is very basic now. This is using sqlite as
+a database. You can select the model at the right side bar. An internet
+connection is required. ## Contact You can join pyqt-openai's Discord_Server to
+have a conversation about it or AI-related stuff ð ## Note Some of the
+features are still being tested. ## Feature * basically this is desktop
+application version of ChatGPT * text streaming (enable by default, you can
+disable it) * AI remembers past conversation * support GPT-4 * you can save the
+conversation history with sqlite database * support prompt generator * support
+image generation with DALL-E * you can test any models, including gpt3.5 * you
+can run this in background application * you can make window stack on top or
+control its transparency ## Requirements * qtpy - the package allowing you to
+write code that works with both PyQt and PySide * PyQt5 >= 5.14 or PySide6 *
+openai ## Preview This is using GPT-3.5 turbo model by default. ### Homepage !
+[image](https://user-images.githubusercontent.com/55078043/236583808-f43403f7-
+2b8f-483b-9271-b78ab8a1eb73.png) You have to write your openai api key inside
+the red box. see [How to play](#how-to-play) ### Overview ![image](https://
+user-images.githubusercontent.com/55078043/236584269-99c76ea5-4cec-44f7-8283-
+e502a182264d.png) ### Conversation preview #### Preview Image ![image](https://
+user-images.githubusercontent.com/55078043/236583716-a18b30b0-7b67-412e-b633-
+7daa8e41b525.png) #### Preview Video https://user-images.githubusercontent.com/
+55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
+Generator https://user-images.githubusercontent.com/55078043/236584481-
+b7bb5246-6bf4-4343-ba6c-a343bb11cda7.mp4 So sorry to weak preview, but i have a
+lot of idea about this prompt generator! Just wait. ## How to play 1. git clone
+~ 2. from the root directory, type "cd pyqt_openai" 3. You should put your api
+key in the line edit. You can get it in official_site of openai. Sign up and
+log in before you get it. By the way, this is free trial, not permanently free.
+See this after you have logged in. Be sure, this is a very important API key
+that belongs to you only, so you should remember it and keep it secure. 4.
+python main.py If installation doesn't work, check the troubleshooting below.
+## Troubleshooting If you see this error while installing the openai package
+``` subprocess-exited-with-error ``` you can shout a curse word and just
+download the package itself from pypi. Unzip it, access the package directory,
+type ``` python setup.py install ``` That will install the openai. ## TODO list
+* support Stable Diffusion * show the explanation of every model and terms
+related to AI (e.g. temperature, topp..) * save conversation history with other
+format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
+eventually) * support multiple language * use SQLAlchemy (maybe not) * show
+reason when the chat input is disabled for some reasons * add the basic example
+sources of making deep learning model with PyTorch (eventually) ## See Also *
+Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
+it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.2/pyqt_openai.egg-info/SOURCES.txt` & `pyqt-openai-0.1.21/pyqt_openai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 README.md
 setup.py
 pyqt_openai/__init__.py
 pyqt_openai/a.py
 pyqt_openai/apiData.py
 pyqt_openai/chatWidget.py
+pyqt_openai/circleProfileImage.py
 pyqt_openai/clickableTooltip.py
 pyqt_openai/convListWidget.py
+pyqt_openai/customizeDialog.py
 pyqt_openai/inputDialog.py
 pyqt_openai/leftSideBar.py
 pyqt_openai/main.py
 pyqt_openai/modelTable.py
 pyqt_openai/notifier.py
 pyqt_openai/searchBar.py
 pyqt_openai/sqlite.py
@@ -20,28 +22,34 @@
 pyqt_openai.egg-info/SOURCES.txt
 pyqt_openai.egg-info/dependency_links.txt
 pyqt_openai.egg-info/requires.txt
 pyqt_openai.egg-info/top_level.txt
 pyqt_openai/ico/__init__.py
 pyqt_openai/ico/add.svg
 pyqt_openai/ico/close.svg
+pyqt_openai/ico/customize.svg
 pyqt_openai/ico/delete.svg
 pyqt_openai/ico/download.svg
 pyqt_openai/ico/help.svg
 pyqt_openai/ico/openai.svg
 pyqt_openai/ico/prompt.svg
 pyqt_openai/ico/search.svg
 pyqt_openai/ico/setting.svg
 pyqt_openai/ico/sidebar.svg
 pyqt_openai/ico/stackontop.svg
+pyqt_openai/ico/user.svg
 pyqt_openai/prompt/__init__.py
 pyqt_openai/prompt/promptGeneratorWidget.py
 pyqt_openai/prompt/propPage.py
 pyqt_openai/prompt/templatePage.py
 pyqt_openai/right_sidebar/__init__.py
 pyqt_openai/right_sidebar/aiPlaygroundWidget.py
 pyqt_openai/right_sidebar/chatPage.py
 pyqt_openai/right_sidebar/completionPage.py
 pyqt_openai/right_sidebar/imagePage.py
 pyqt_openai/test/__init__.py
 pyqt_openai/test/htmlformat.py
-pyqt_openai/test/rightSideBarTab.py
+pyqt_openai/test/rightSideBarTab.py
+pyqt_openai/test/stable_diffusion/__init__.py
+pyqt_openai/test/stable_diffusion/delete_model.py
+pyqt_openai/test/stable_diffusion/make_model.py
+pyqt_openai/test/stable_diffusion/using_model.py
```

### Comparing `pyqt-openai-0.1.2/setup.py` & `pyqt-openai-0.1.21/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-openai',
-    version='0.1.2',
+    version='0.1.21',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
-    package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'help.svg', 'sidebar.svg', 'prompt.svg', 'download.svg', 'stackontop.svg', 'add.svg', 'delete.svg', 'setting.svg', 'search.svg']},
+    package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'help.svg', 'customize.svg', 'user.svg',
+                                      'sidebar.svg', 'prompt.svg', 'download.svg', 'stackontop.svg',
+                                      'add.svg', 'delete.svg', 'setting.svg', 'search.svg']},
     description='PyQt OpenAI example',
     url='https://github.com/yjg30737/pyqt-openai.git',
     long_description_content_type='text/markdown',
     long_description=long_description,
     install_requires=[
         'PyQt5>=5.14',
         'PySide6',
```

