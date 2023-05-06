# Comparing `tmp/datadigitizer-1.2.0.tar.gz` & `tmp/datadigitizer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadigitizer-1.2.0.tar", last modified: Tue Sep 20 18:38:39 2022, max compression
+gzip compressed data, was "datadigitizer-1.2.1.tar", last modified: Sat May  6 05:33:52 2023, max compression
```

## Comparing `datadigitizer-1.2.0.tar` & `datadigitizer-1.2.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.390919 datadigitizer-1.2.0/
--rw-r--r--   0 milan      (501) staff       (20)       61 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/INSTALL.txt
--rw-r--r--   0 milan      (501) staff       (20)    35148 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/LICENSE.txt
--rw-r--r--   0 milan      (501) staff       (20)      528 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/MANIFEST.in
--rw-r--r--   0 milan      (501) staff       (20)     2597 2022-09-20 18:38:39.390543 datadigitizer-1.2.0/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)     1690 2022-09-20 18:33:30.000000 datadigitizer-1.2.0/README.rst
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.278887 datadigitizer-1.2.0/datadigitizer/
--rw-r--r--   0 milan      (501) staff       (20)      748 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/datadigitizer/__init__.py
--rw-r--r--   0 milan      (501) staff       (20)      802 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/datadigitizer/__main__.py
--rw-r--r--   0 milan      (501) staff       (20)    57211 2022-09-20 18:33:30.000000 datadigitizer-1.2.0/datadigitizer/gui.py
--rw-r--r--   0 milan      (501) staff       (20)     2461 2022-09-20 18:35:44.000000 datadigitizer-1.2.0/datadigitizer/icon.png
--rw-r--r--   0 milan      (501) staff       (20)     1212 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/datadigitizer/icon.py
--rw-r--r--   0 milan      (501) staff       (20)     3264 2022-09-20 18:33:30.000000 datadigitizer-1.2.0/datadigitizer/settings.py
--rw-r--r--   0 milan      (501) staff       (20)     4075 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/datadigitizer/tests.py
--rw-r--r--   0 milan      (501) staff       (20)     1264 2022-09-20 18:37:59.000000 datadigitizer-1.2.0/datadigitizer/version.py
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.288545 datadigitizer-1.2.0/datadigitizer.egg-info/
--rw-r--r--   0 milan      (501) staff       (20)     2597 2022-09-20 18:38:38.000000 datadigitizer-1.2.0/datadigitizer.egg-info/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)     1774 2022-09-20 18:38:38.000000 datadigitizer-1.2.0/datadigitizer.egg-info/SOURCES.txt
--rw-r--r--   0 milan      (501) staff       (20)        1 2022-09-20 18:38:38.000000 datadigitizer-1.2.0/datadigitizer.egg-info/dependency_links.txt
--rw-r--r--   0 milan      (501) staff       (20)       44 2022-09-20 18:38:38.000000 datadigitizer-1.2.0/datadigitizer.egg-info/requires.txt
--rw-r--r--   0 milan      (501) staff       (20)       14 2022-09-20 18:38:38.000000 datadigitizer-1.2.0/datadigitizer.egg-info/top_level.txt
--rw-r--r--   0 milan      (501) staff       (20)       43 2022-09-20 18:33:30.000000 datadigitizer-1.2.0/requirements.txt
--rw-r--r--   0 milan      (501) staff       (20)       38 2022-09-20 18:38:39.391051 datadigitizer-1.2.0/setup.cfg
--rw-r--r--   0 milan      (501) staff       (20)     2201 2022-09-20 18:33:30.000000 datadigitizer-1.2.0/setup.py
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.292421 datadigitizer-1.2.0/sphinx/
--rw-r--r--   0 milan      (501) staff       (20)      638 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/Makefile
--rw-r--r--   0 milan      (501) staff       (20)      764 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/make.bat
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.295570 datadigitizer-1.2.0/sphinx/source/
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.299464 datadigitizer-1.2.0/sphinx/source/api/
--rw-r--r--   0 milan      (501) staff       (20)      300 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/api/codedoc.rst
--rw-r--r--   0 milan      (501) staff       (20)      110 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/api/index.rst
--rw-r--r--   0 milan      (501) staff       (20)     5978 2022-06-18 15:53:07.000000 datadigitizer-1.2.0/sphinx/source/conf.py
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.306703 datadigitizer-1.2.0/sphinx/source/getting_started/
--rw-r--r--   0 milan      (501) staff       (20)       85 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/getting_started/index.rst
--rw-r--r--   0 milan      (501) staff       (20)     1724 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/getting_started/introduction.rst
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.352113 datadigitizer-1.2.0/sphinx/source/images/
--rw-r--r--   0 milan      (501) staff       (20)    31585 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/images/tutorial-1-Open_App.png
--rw-r--r--   0 milan      (501) staff       (20)    41448 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/images/tutorial-2-Open_Image.png
--rw-r--r--   0 milan      (501) staff       (20)    41412 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/images/tutorial-3-Position_Axis.png
--rw-r--r--   0 milan      (501) staff       (20)    41454 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/images/tutorial-4-Set_XY_limits.png
--rw-r--r--   0 milan      (501) staff       (20)    49302 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/images/tutorial-5-Set_XY_Values.png
--rw-r--r--   0 milan      (501) staff       (20)    34094 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/images/tutorial-6-DataTable.png
--rw-r--r--   0 milan      (501) staff       (20)    50269 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/images/tutorial-6-Set_Data_Values.png
--rw-r--r--   0 milan      (501) staff       (20)    47844 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/images/tutorial-7-Test_Scale.png
--rw-r--r--   0 milan      (501) staff       (20)      528 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/index.rst
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.383937 datadigitizer-1.2.0/sphinx/source/releases/
--rw-r--r--   0 milan      (501) staff       (20)      907 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.0.0-changelog.rst
--rw-r--r--   0 milan      (501) staff       (20)      256 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.0.0-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      389 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.0.1-changelog.rst
--rw-r--r--   0 milan      (501) staff       (20)      158 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.0.1-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)     1112 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.0.2-changelog.rst
--rw-r--r--   0 milan      (501) staff       (20)      788 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.0.2-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      155 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.1.0-changelog.rst
--rw-r--r--   0 milan      (501) staff       (20)      395 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.1.0-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      155 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.1.1-changelog.rst
--rw-r--r--   0 milan      (501) staff       (20)      232 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/1.1.1-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      154 2022-06-18 15:53:07.000000 datadigitizer-1.2.0/sphinx/source/releases/1.1.2-changelog.rst
--rw-r--r--   0 milan      (501) staff       (20)      232 2022-06-18 15:53:07.000000 datadigitizer-1.2.0/sphinx/source/releases/1.1.2-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      154 2022-09-20 18:33:30.000000 datadigitizer-1.2.0/sphinx/source/releases/1.2.0-changelog.rst
--rw-r--r--   0 milan      (501) staff       (20)      424 2022-09-20 18:33:30.000000 datadigitizer-1.2.0/sphinx/source/releases/1.2.0-notes.rst
--rw-r--r--   0 milan      (501) staff       (20)      222 2022-09-20 18:33:30.000000 datadigitizer-1.2.0/sphinx/source/releases/index.rst
--rw-r--r--   0 milan      (501) staff       (20)      427 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/releases/template.rst
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2022-09-20 18:38:39.388101 datadigitizer-1.2.0/sphinx/source/user_guide/
--rw-r--r--   0 milan      (501) staff       (20)       93 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/user_guide/index.rst
--rw-r--r--   0 milan      (501) staff       (20)     3936 2022-06-17 21:15:50.000000 datadigitizer-1.2.0/sphinx/source/user_guide/tutorial.rst
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:52.075933 datadigitizer-1.2.1/
+-rw-r--r--   0 milan      (501) staff       (20)       61 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/INSTALL.txt
+-rw-r--r--   0 milan      (501) staff       (20)    35148 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/LICENSE.txt
+-rw-r--r--   0 milan      (501) staff       (20)      530 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/MANIFEST.in
+-rw-r--r--   0 milan      (501) staff       (20)     2257 2023-05-06 05:33:52.075025 datadigitizer-1.2.1/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)     1690 2022-09-20 18:33:30.000000 datadigitizer-1.2.1/README.rst
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:51.956743 datadigitizer-1.2.1/datadigitizer/
+-rw-r--r--   0 milan      (501) staff       (20)       48 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/datadigitizer/__init__.py
+-rw-r--r--   0 milan      (501) staff       (20)      162 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/datadigitizer/__main__.py
+-rw-r--r--   0 milan      (501) staff       (20)    56598 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/datadigitizer/gui.py
+-rw-r--r--   0 milan      (501) staff       (20)     2461 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/datadigitizer/icon.png
+-rw-r--r--   0 milan      (501) staff       (20)      512 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/datadigitizer/icon.py
+-rw-r--r--   0 milan      (501) staff       (20)     2564 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/datadigitizer/settings.py
+-rw-r--r--   0 milan      (501) staff       (20)     3375 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/datadigitizer/tests.py
+-rw-r--r--   0 milan      (501) staff       (20)      559 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/datadigitizer/version.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:51.961183 datadigitizer-1.2.1/datadigitizer.egg-info/
+-rw-r--r--   0 milan      (501) staff       (20)     2257 2023-05-06 05:33:51.000000 datadigitizer-1.2.1/datadigitizer.egg-info/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)     1813 2023-05-06 05:33:51.000000 datadigitizer-1.2.1/datadigitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 milan      (501) staff       (20)        1 2023-05-06 05:33:51.000000 datadigitizer-1.2.1/datadigitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 milan      (501) staff       (20)       44 2023-05-06 05:33:51.000000 datadigitizer-1.2.1/datadigitizer.egg-info/requires.txt
+-rw-r--r--   0 milan      (501) staff       (20)       14 2023-05-06 05:33:51.000000 datadigitizer-1.2.1/datadigitizer.egg-info/top_level.txt
+-rw-r--r--   0 milan      (501) staff       (20)       43 2023-05-06 05:06:37.000000 datadigitizer-1.2.1/requirements.txt
+-rw-r--r--   0 milan      (501) staff       (20)       38 2023-05-06 05:33:52.076097 datadigitizer-1.2.1/setup.cfg
+-rw-r--r--   0 milan      (501) staff       (20)     1047 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/setup.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:51.966831 datadigitizer-1.2.1/sphinx/
+-rw-r--r--   0 milan      (501) staff       (20)      700 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/sphinx/Makefile
+-rw-r--r--   0 milan      (501) staff       (20)      764 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/make.bat
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:51.969710 datadigitizer-1.2.1/sphinx/source/
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:51.972710 datadigitizer-1.2.1/sphinx/source/api/
+-rw-r--r--   0 milan      (501) staff       (20)      300 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/api/codedoc.rst
+-rw-r--r--   0 milan      (501) staff       (20)      110 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/api/index.rst
+-rw-r--r--   0 milan      (501) staff       (20)     5978 2022-06-18 15:53:07.000000 datadigitizer-1.2.1/sphinx/source/conf.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:51.983329 datadigitizer-1.2.1/sphinx/source/getting_started/
+-rw-r--r--   0 milan      (501) staff       (20)       85 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/getting_started/index.rst
+-rw-r--r--   0 milan      (501) staff       (20)     1724 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/getting_started/introduction.rst
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:52.016693 datadigitizer-1.2.1/sphinx/source/images/
+-rw-r--r--   0 milan      (501) staff       (20)    31585 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/images/tutorial-1-Open_App.png
+-rw-r--r--   0 milan      (501) staff       (20)    41448 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/images/tutorial-2-Open_Image.png
+-rw-r--r--   0 milan      (501) staff       (20)    41412 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/images/tutorial-3-Position_Axis.png
+-rw-r--r--   0 milan      (501) staff       (20)    41454 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/images/tutorial-4-Set_XY_limits.png
+-rw-r--r--   0 milan      (501) staff       (20)    49302 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/images/tutorial-5-Set_XY_Values.png
+-rw-r--r--   0 milan      (501) staff       (20)    34094 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/images/tutorial-6-DataTable.png
+-rw-r--r--   0 milan      (501) staff       (20)    50269 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/images/tutorial-6-Set_Data_Values.png
+-rw-r--r--   0 milan      (501) staff       (20)    47844 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/images/tutorial-7-Test_Scale.png
+-rw-r--r--   0 milan      (501) staff       (20)      528 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/index.rst
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:52.063117 datadigitizer-1.2.1/sphinx/source/releases/
+-rw-r--r--   0 milan      (501) staff       (20)      907 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.0.0-changelog.rst
+-rw-r--r--   0 milan      (501) staff       (20)      256 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.0.0-notes.rst
+-rw-r--r--   0 milan      (501) staff       (20)      389 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.0.1-changelog.rst
+-rw-r--r--   0 milan      (501) staff       (20)      158 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.0.1-notes.rst
+-rw-r--r--   0 milan      (501) staff       (20)     1112 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.0.2-changelog.rst
+-rw-r--r--   0 milan      (501) staff       (20)      788 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.0.2-notes.rst
+-rw-r--r--   0 milan      (501) staff       (20)      155 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.1.0-changelog.rst
+-rw-r--r--   0 milan      (501) staff       (20)      395 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.1.0-notes.rst
+-rw-r--r--   0 milan      (501) staff       (20)      155 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.1.1-changelog.rst
+-rw-r--r--   0 milan      (501) staff       (20)      232 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/1.1.1-notes.rst
+-rw-r--r--   0 milan      (501) staff       (20)      154 2022-06-18 15:53:07.000000 datadigitizer-1.2.1/sphinx/source/releases/1.1.2-changelog.rst
+-rw-r--r--   0 milan      (501) staff       (20)      232 2022-06-18 15:53:07.000000 datadigitizer-1.2.1/sphinx/source/releases/1.1.2-notes.rst
+-rw-r--r--   0 milan      (501) staff       (20)      154 2022-09-20 18:33:30.000000 datadigitizer-1.2.1/sphinx/source/releases/1.2.0-changelog.rst
+-rw-r--r--   0 milan      (501) staff       (20)      424 2023-02-19 14:02:03.000000 datadigitizer-1.2.1/sphinx/source/releases/1.2.0-notes.rst
+-rw-r--r--   0 milan      (501) staff       (20)      359 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/sphinx/source/releases/1.2.1-notes.rst
+-rw-r--r--   0 milan      (501) staff       (20)      242 2023-05-06 05:33:05.000000 datadigitizer-1.2.1/sphinx/source/releases/index.rst
+-rw-r--r--   0 milan      (501) staff       (20)      427 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/releases/template.rst
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2023-05-06 05:33:52.070234 datadigitizer-1.2.1/sphinx/source/user_guide/
+-rw-r--r--   0 milan      (501) staff       (20)       93 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/user_guide/index.rst
+-rw-r--r--   0 milan      (501) staff       (20)     3936 2022-06-17 21:15:50.000000 datadigitizer-1.2.1/sphinx/source/user_guide/tutorial.rst
```

### Comparing `datadigitizer-1.2.0/LICENSE.txt` & `datadigitizer-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/MANIFEST.in` & `datadigitizer-1.2.1/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Add documentation: I don't use add_data_dir and add_data_file in setup.py
 # since I don't want to include this at installation , only sdist-generated tarballs 
-recursive-include docs/*
+# recursive-include docs/*
 recursive-include sphinx/source *
 include sphinx/make.bat
 include sphinx/Makefile
 
 
 include INSTALL.txt
 include LICENSE.txt
```

### Comparing `datadigitizer-1.2.0/README.rst` & `datadigitizer-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/datadigitizer/gui.py` & `datadigitizer-1.2.1/datadigitizer/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 r"""
 Main GUI.
-
-Copyright (C) 2020-2021 Milan Skocic.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Author: Milan Skocic <milan.skocic@gmail.com>
 """
 import tkinter as tk
 from tkinter import ttk, messagebox, filedialog
 
 import sys
 import webbrowser
 import pathlib
@@ -401,15 +384,15 @@
         label.grid(row=0, column=0, sticky='nswe')
 
     def _quit(self):
         r"""Close the toplevel window."""
         self.master.focus_set()
         self.destroy()
 
-
+#TODO: Use tkinter treeview instead of array of widgets
 class DataTable(ScrolledFrame):
     r"""Scrolled data table. See __init__.__doc__."""
     def __init__(self, master, **kwargs):
         r"""
         Scrolled data table widget.
 
         Parameters
@@ -1404,16 +1387,16 @@
             self._data_array['y'] = trans.backward(ypix)
             msg = f'{trans.backward_scale}' + ' ' + unit
             self._ax.set_ylabel(msg)
 
             flag = True
             self._refresh()
 
-        except ValueError as e:
-            messagebox.showwarning('Warning', e)
+        except ValueError as err:
+            messagebox.showwarning('Warning', err)
 
         return flag
 
     def _plot_test_data(self):
         r"""
         x and y positions are indicated as matrix indexes: 
         row index x is for y axis and column index y is for x axis
@@ -1445,16 +1428,16 @@
                               which=which)
             ypix = trans.forward(ytest_value)
             flag = True
             i,j = self._xypix_to_ij(xpix, ypix)
             self._add_data(i, j)
             self._refresh()
 
-        except ValueError as e:
-            messagebox.showwarning('Warning', e)
+        except ValueError as err:
+            messagebox.showwarning('Warning', err)
 
         return flag
 
     def _save(self):
         """Save data."""
         _filepath = filedialog.asksaveasfilename(title='Open Plot',
                                                  defaultextension='.txt',
@@ -1510,21 +1493,21 @@
     def _test_loglog(self):
         """Test semi-log scale."""
         self._filepath = test_loglog()
         self._load_image()
 
     def _online_documentation(self):
         """Display online documentation."""
-        b = webbrowser.get()
-        b.open(self.url)
+        browser = webbrowser.get()
+        browser.open(self.url)
 
     def _sources(self):
         """Display sources."""
-        b = webbrowser.get()
-        b.open(self.url_download)
+        browser = webbrowser.get()
+        browser.open(self.url_download)
 
     def stop(self):
         r"""
         Stop the main tk loop.
         """
         if messagebox.askyesno("Exit", "Do you want to quit the application?"):
             section = 'FOLDERS'
```

### Comparing `datadigitizer-1.2.0/datadigitizer/icon.png` & `datadigitizer-1.2.1/datadigitizer/icon.png`

 * *Files 3% similar despite different names*

#### sng

```diff
@@ -2,15 +2,15 @@
 IHDR {
     width: 128; height: 128; bitdepth: 8;
     using color alpha;
 }
 pHYs {xpixels: 2520; ypixels: 2520; per: meter;}  # (64 dpi)
 tEXt {
     keyword: "Software";
-    text: "Matplotlib version3.6.0, https://matplotlib.org/";
+    text: "Matplotlib version3.7.1, https://matplotlib.org/";
 }
 IMAGE {
     pixels hex
 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 
 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 
 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 
 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff
```

### Comparing `datadigitizer-1.2.0/datadigitizer/settings.py` & `datadigitizer-1.2.1/datadigitizer/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 r"""
 Settings module.
-
-Copyright (C) 2020-2021 Milan Skocic.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Author: Milan Skocic <milan.skocic@gmail.com>
 """
 import os
 import configparser
 import re
 from typing import Dict
 from . import version
```

### Comparing `datadigitizer-1.2.0/datadigitizer/tests.py` & `datadigitizer-1.2.1/datadigitizer/tests.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 r"""
 Tests module.
-
-Copyright (C) 2020-2021 Milan Skocic.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Author: Milan Skocic <milan.skocic@gmail.com>
 """
 import pathlib
 import unittest
 import numpy as np
 import matplotlib.pyplot as plt
 from .settings import CFG_FOLDER
```

### Comparing `datadigitizer-1.2.0/datadigitizer.egg-info/SOURCES.txt` & `datadigitizer-1.2.1/datadigitizer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,11 +43,12 @@
 sphinx/source/releases/1.1.0-notes.rst
 sphinx/source/releases/1.1.1-changelog.rst
 sphinx/source/releases/1.1.1-notes.rst
 sphinx/source/releases/1.1.2-changelog.rst
 sphinx/source/releases/1.1.2-notes.rst
 sphinx/source/releases/1.2.0-changelog.rst
 sphinx/source/releases/1.2.0-notes.rst
+sphinx/source/releases/1.2.1-notes.rst
 sphinx/source/releases/index.rst
 sphinx/source/releases/template.rst
 sphinx/source/user_guide/index.rst
 sphinx/source/user_guide/tutorial.rst
```

### Comparing `datadigitizer-1.2.0/sphinx/Makefile` & `datadigitizer-1.2.1/sphinx/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -8,13 +8,17 @@
 SOURCEDIR     = source
 BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
-.PHONY: help Makefile
+.PHONY: help Makefile upload
+
+upload:
+	rm -r ../docs/*
+	cp -r build/html/* ../docs/
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `datadigitizer-1.2.0/sphinx/make.bat` & `datadigitizer-1.2.1/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/conf.py` & `datadigitizer-1.2.1/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/getting_started/introduction.rst` & `datadigitizer-1.2.1/sphinx/source/getting_started/introduction.rst`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/images/tutorial-1-Open_App.png` & `datadigitizer-1.2.1/sphinx/source/images/tutorial-1-Open_App.png`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/images/tutorial-2-Open_Image.png` & `datadigitizer-1.2.1/sphinx/source/images/tutorial-2-Open_Image.png`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/images/tutorial-3-Position_Axis.png` & `datadigitizer-1.2.1/sphinx/source/images/tutorial-3-Position_Axis.png`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/images/tutorial-4-Set_XY_limits.png` & `datadigitizer-1.2.1/sphinx/source/images/tutorial-4-Set_XY_limits.png`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/images/tutorial-5-Set_XY_Values.png` & `datadigitizer-1.2.1/sphinx/source/images/tutorial-5-Set_XY_Values.png`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/images/tutorial-6-DataTable.png` & `datadigitizer-1.2.1/sphinx/source/images/tutorial-6-DataTable.png`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/images/tutorial-6-Set_Data_Values.png` & `datadigitizer-1.2.1/sphinx/source/images/tutorial-6-Set_Data_Values.png`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/images/tutorial-7-Test_Scale.png` & `datadigitizer-1.2.1/sphinx/source/images/tutorial-7-Test_Scale.png`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/index.rst` & `datadigitizer-1.2.1/sphinx/source/index.rst`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/releases/1.0.0-changelog.rst` & `datadigitizer-1.2.1/sphinx/source/releases/1.0.0-changelog.rst`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/releases/1.0.2-changelog.rst` & `datadigitizer-1.2.1/sphinx/source/releases/1.0.2-changelog.rst`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/releases/1.0.2-notes.rst` & `datadigitizer-1.2.1/sphinx/source/releases/1.0.2-notes.rst`

 * *Files identical despite different names*

### Comparing `datadigitizer-1.2.0/sphinx/source/user_guide/tutorial.rst` & `datadigitizer-1.2.1/sphinx/source/user_guide/tutorial.rst`

 * *Files identical despite different names*

