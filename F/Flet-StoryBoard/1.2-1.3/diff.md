# Comparing `tmp/Flet StoryBoard-1.2.tar.gz` & `tmp/Flet StoryBoard-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flet StoryBoard-1.2.tar", last modified: Tue Apr 25 19:00:51 2023, max compression
+gzip compressed data, was "Flet StoryBoard-1.3.tar", last modified: Sat May  6 16:21:39 2023, max compression
```

## Comparing `Flet StoryBoard-1.2.tar` & `Flet StoryBoard-1.3.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.284163 Flet StoryBoard-1.2/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.277438 Flet StoryBoard-1.2/Flet_StoryBoard/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.279202 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:35.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8326 2023-04-23 11:23:40.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/edit_subwidgets_engin.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8400 2023-04-23 09:53:37.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/edit_widget_engine.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4927 2023-04-24 14:04:07.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/suggesting_engine.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2892 2023-04-25 13:53:41.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Engines/viewer_engine.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.280197 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:59.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3030 2023-04-21 16:25:25.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/color_picker.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      977 2023-04-25 13:40:50.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/create_storyboard.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      702 2023-04-22 11:06:35.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/get_url_icon.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2857 2023-04-22 13:53:33.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/list_picker.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      118 2023-04-20 11:35:46.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/page_info.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1754 2023-04-25 14:14:21.000000 Flet StoryBoard-1.2/Flet_StoryBoard/Tools/storyboard_class.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.280480 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1117 2023-04-24 11:25:41.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/All.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:18.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.282220 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:25.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2836 2023-04-24 10:12:52.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1966 2023-04-24 13:07:17.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/image.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2954 2023-04-23 15:09:29.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/label.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2077 2023-04-22 15:19:21.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/markdown.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2592 2023-04-24 11:23:12.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/navigator.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3514 2023-04-23 15:22:36.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/open_url.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1696 2023-04-23 15:09:43.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/padding.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2919 2023-04-24 08:30:46.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/paragraph.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7286 2023-04-23 15:54:32.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/row.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4927 2023-04-24 10:03:48.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/textfield.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2782 2023-04-23 19:24:28.000000 Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/title.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       92 2023-04-22 14:25:13.000000 Flet StoryBoard-1.2/Flet_StoryBoard/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1615 2023-04-25 18:59:57.000000 Flet StoryBoard-1.2/Flet_StoryBoard/edit.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1170 2023-04-24 11:12:41.000000 Flet StoryBoard-1.2/Flet_StoryBoard/load_storyboard.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.282871 Flet StoryBoard-1.2/Flet_StoryBoard/pages/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.283125 Flet StoryBoard-1.2/Flet_StoryBoard/pages/Settings/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 13:38:01.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/Settings/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2028 2023-04-25 14:10:15.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/Settings/pages.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:41.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     9938 2023-04-24 13:56:02.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/create_new_file.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     9941 2023-04-25 14:10:02.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/main_page.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6535 2023-04-25 13:54:52.000000 Flet StoryBoard-1.2/Flet_StoryBoard/pages/settings.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.283597 Flet StoryBoard-1.2/Flet_StoryBoard/sections/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:49.000000 Flet StoryBoard-1.2/Flet_StoryBoard/sections/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      623 2023-04-23 08:24:47.000000 Flet StoryBoard-1.2/Flet_StoryBoard/sections/edit_section.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2033 2023-04-24 08:50:35.000000 Flet StoryBoard-1.2/Flet_StoryBoard/sections/left_section.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-24 10:23:00.000000 Flet StoryBoard-1.2/Flet_StoryBoard/sections/preview_section.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.283811 Flet StoryBoard-1.2/Flet_StoryBoard/ui_toolkit/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:08.000000 Flet StoryBoard-1.2/Flet_StoryBoard/ui_toolkit/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      784 2023-04-22 17:35:05.000000 Flet StoryBoard-1.2/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-25 19:00:51.278188 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      431 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1879 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       21 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-25 19:00:51.000000 Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 Flet StoryBoard-1.2/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       24 2023-02-14 13:25:28.000000 Flet StoryBoard-1.2/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      431 2023-04-25 19:00:51.284023 Flet StoryBoard-1.2/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     2487 2023-04-24 14:34:26.000000 Flet StoryBoard-1.2/README.md
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 Flet StoryBoard-1.2/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-25 19:00:51.284205 Flet StoryBoard-1.2/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      592 2023-04-25 19:00:21.000000 Flet StoryBoard-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.694544 Flet StoryBoard-1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.682544 Flet StoryBoard-1.3/Flet_StoryBoard/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/edit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.686544 Flet StoryBoard-1.3/Flet_StoryBoard/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/edit_subwidgets_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/edit_widget_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/suggesting_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/engines/viewer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/load_storyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.686544 Flet StoryBoard-1.3/Flet_StoryBoard/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.686544 Flet StoryBoard-1.3/Flet_StoryBoard/pages/Settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/Settings/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/create_new_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/main_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pages/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/pyodide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.690544 Flet StoryBoard-1.3/Flet_StoryBoard/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/sections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/sections/edit_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/sections/left_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/sections/preview_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.690544 Flet StoryBoard-1.3/Flet_StoryBoard/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/create_storyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/get_url_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/list_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/page_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/tools/storyboard_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.690544 Flet StoryBoard-1.3/Flet_StoryBoard/ui_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/ui_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.690544 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/All.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.694544 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/textfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/title.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:21:39.682544 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 16:21:39.000000 Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 16:21:39.694544 Flet StoryBoard-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:21:39.694544 Flet StoryBoard-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-06 16:21:28.000000 Flet StoryBoard-1.3/setup.py
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/Engines/edit_subwidgets_engin.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/engines/edit_widget_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,222 @@
 import flet
 
-from ..WIDGETS.All import all_widgets
-from ..Tools.color_picker import colorPicker
-from ..Tools.list_picker import ListPopup
-
-# main_widget_mother_class: is the widgets mother like row or column.
-class editSubWidgetsEngine:
-    def __init__(self, main_class, main_widget_mother_class, section_view:flet.Column, widget_number) -> None:
+from ..widgets.All import all_widgets
+from ..tools.color_picker import ColorPicker
+from ..tools.list_picker import ListPopup
+
+
+class EditWidgetsEngine:
+    def __init__(self, main_class, section_view: flet.Column, widget_number) -> None:
         self.main_class = main_class
-        self.main_widget_mother_class = main_widget_mother_class
         self.section_view = section_view
         self.widget_number = widget_number
 
+        self.current_page_name = self.main_class.current_page_name
         self.all_fields = {}
-        
+
         self.show_edit_tools()
-    
-    def show_edit_tools (self):
-        #? Update the viewerEngine.
-        self.main_class.preview_section.update_preview(self.main_class.current_page_name)
 
-        #? Start..
+    def show_edit_tools(self):
         self.section_view.clean()
-        content = self.main_widget_mother_class.template["widgets"]
-        class_name = content[self.widget_number]["widget_class_name"]
-        widget_content = content[self.widget_number]
+        content = self.main_class.dict_content
+        class_name = content["pages"][self.current_page_name]["widgets"][self.widget_number]["widget_class_name"]
+        widget_content = content["pages"][self.current_page_name]["widgets"][self.widget_number]
 
         if class_name not in all_widgets:
-            #? if widget not found.
-            self.section_view.controls.append(flet.Row([flet.Text(f"There is no supported\nwidget named '{class_name}'.", color="white")]))
+            # if widget not found.
+            self.section_view.controls.append(
+                flet.Row(
+                    [flet.Text(f"There is no supported\nwidget named '{class_name}'.", color=flet.colors.WHITE)]
+                )
+            )
             return
-        
+
         the_class = all_widgets[class_name]["class"]
-        the_class = the_class(self.main_class, self.main_widget_mother_class.preview_section, widget_number=self.widget_number)
+        the_class = the_class(
+            self.main_class,
+            self.main_class.preview_section.main_view,
+            widget_number=self.widget_number
+        )
         default_args = the_class.args
-        
-        title = flet.Text(f"Edit {class_name}", size=25, weight="bold", color="white")
+
+        title = flet.Text(f"Edit {class_name}", size=25, weight=flet.FontWeight.BOLD, color=flet.colors.WHITE)
         self.section_view.controls.append(title)
 
         for t in widget_content["properties"]:
             prop_name = t
             prop_value = widget_content["properties"][t]
-            if prop_name not in default_args: print("Error while load widget properties in edit engine."); self.section_view.clean(); return
+            if prop_name not in default_args:
+                print("Error while load widget properties in edit engine.")
+                self.section_view.clean()
+                return
             prop_type = default_args[prop_name]["type"]
-            
-            #* This statments bellow is for adding the fields for edit a widget.
-            if type(prop_type()) == type(str()):
-                tf = flet.TextField(width=160, bgcolor="white", color="black", label=prop_name)
+
+            # These statements below are for adding the fields for edit a widget.
+            if isinstance(prop_type(), str):
+                tf = flet.TextField(width=160, bgcolor=flet.colors.WHITE, color=flet.colors.BLACK, label=prop_name)
                 tf.value = prop_value
-                self.section_view.controls.append(flet.Row([tf], alignment="center"))
+                self.section_view.controls.append(flet.Row([tf], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = tf
                 if "multi_line" in default_args[prop_name]:
                     tf.multiline = True
-            elif type(prop_type()) == type(int()):
+
+            elif isinstance(prop_type(), int):
                 slid = flet.Slider(min=0, max=500, divisions=500, label="{value}", width=160)
                 slid.value = int(prop_value)
-                self.section_view.controls.append(flet.Row([flet.Text(f"{prop_name}:", color="white", width=150)], alignment="center"))
-                self.section_view.controls.append(flet.Row([slid], alignment="center"))
+                self.section_view.controls.append(
+                    flet.Row(
+                        [
+                            flet.Text(
+                                f"{prop_name}:",
+                                color=flet.colors.WHITE,
+                                width=150
+                            )
+                        ], alignment=flet.MainAxisAlignment.CENTER
+                    )
+                )
+                self.section_view.controls.append(
+                    flet.Row(
+                        [slid],
+                        alignment=flet.MainAxisAlignment.CENTER
+                    )
+                )
                 self.all_fields[prop_name] = slid
-            elif type(prop_type()) == type(bool()):
+
+            elif isinstance(prop_type(), bool):
                 tog = flet.Switch()
                 tog.value = prop_value
-                self.section_view.controls.append(flet.Row([flet.Text(f"{prop_name}",color="white", size=13), tog], alignment="center", spacing=25))
+                self.section_view.controls.append(
+                    flet.Row([flet.Text(f"{prop_name}", color=flet.colors.WHITE, size=13), tog],
+                             alignment=flet.MainAxisAlignment.CENTER, spacing=25))
                 self.all_fields[prop_name] = tog
-            elif type(prop_type()) == type(colorPicker()):
+
+            elif type(prop_type()) == type(ColorPicker()):
                 self.section_view.controls.append(flet.Text(""))
-                colp = colorPicker(self.section_view, title_name=prop_name, drop_width=120, selected_color=prop_value, add_it=False)
-                self.section_view.controls.append(flet.Row([colp.v], alignment="center"))
+                colp = ColorPicker(self.section_view, selected_color=prop_value, add_it=False, title_name=prop_name,
+                                   drop_width=120)
+                self.section_view.controls.append(flet.Row([colp.v], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = colp
-            elif type(prop_type()) == type(list()):
+
+            elif isinstance(prop_type(), list):
                 dr = flet.Dropdown(width=160, label=prop_name)
                 for i in default_args[prop_name]["options"]:
                     dr.options.append(flet.dropdown.Option(f"{i}"))
                 dr.value = prop_value
-                self.section_view.controls.append(flet.Row([dr], alignment="center"))
+                self.section_view.controls.append(flet.Row([dr], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = dr
+
             elif type(prop_type()) == type(ListPopup()):
                 lp = ListPopup(default_args[prop_name]["options"], self.main_class, prop_value, prop_name)
-                self.section_view.controls.append(flet.Row([lp.self_ui], alignment="center"))
+                self.section_view.controls.append(flet.Row([lp.self_ui], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = lp
-        
 
-        #* This button bellow for widgets that support sub-widgets.
+        # This button below for widgets that support sub-widgets.
         if hasattr(the_class, "support_sub_widgets"):
             add_sub_widget_button = flet.TextButton("Add sub-widget", on_click=the_class.widgets_to_add_in)
-            self.section_view.controls.append(flet.Row([add_sub_widget_button], alignment="center"))
-
-        
-
-        #* This slider bellow is for rearrange the widget on the page.
-        rearrange_slider = flet.Slider(min=0, max=len(content), 
-        value=self.widget_number, label="{value}", width=160, divisions=len(content))
-        self.section_view.controls.append(flet.Row([flet.Text(f"reArrange:", color="white", width=150)], alignment="center"))
-        self.section_view.controls.append(flet.Row([rearrange_slider], alignment="center"))
+            self.section_view.controls.append(
+                flet.Row(
+                    [add_sub_widget_button],
+                    alignment=flet.MainAxisAlignment.CENTER
+                )
+            )
+
+        # This slider bellow is for rearrange the widget on the page.
+        rearrange_slider = flet.Slider(
+            min=0,
+            max=len(content["pages"][self.current_page_name]["widgets"]),
+            value=self.widget_number,
+            label="{value}",
+            width=160,
+            divisions=len(content["pages"][self.current_page_name]["widgets"])
+        )
+        self.section_view.controls.append(
+            flet.Row(
+                [flet.Text(f"reArrange:", color=flet.colors.WHITE, width=150)],
+                alignment=flet.MainAxisAlignment.CENTER
+            )
+        )
+        self.section_view.controls.append(flet.Row([rearrange_slider], alignment=flet.MainAxisAlignment.CENTER))
         self.rearrange_slider = rearrange_slider
-        
+
         self.section_view.controls.append(flet.Text("\n"))
-        #* Down bellow is for done_button and delete_btn.
-        done_button = flet.ElevatedButton("Done", bgcolor="white", color="black", width=150, height=40, on_click=self.done_edit)
-        self.section_view.controls.append(flet.Row([done_button], alignment="center"))
-
-        delete_button = flet.TextButton(content=flet.Text("delete", color="red", size=13), on_click=self.delete_widget)
-        self.section_view.controls.append(flet.Row([delete_button], alignment="center"))
-    
-    def done_edit (self, *args):
+        # Down bellow is for done_button and delete_btn.
+        done_button = flet.ElevatedButton(
+            "Done",
+            bgcolor=flet.colors.WHITE,
+            color=flet.colors.BLACK,
+            width=150,
+            height=40,
+            on_click=self.done_edit
+        )
+        self.section_view.controls.append(
+            flet.Row(
+                [done_button],
+                alignment=flet.MainAxisAlignment.CENTER
+            )
+        )
+
+        delete_button = flet.TextButton(
+            content=flet.Text("delete", color=flet.colors.RED, size=13),
+            on_click=self.delete_widget
+        )
+        self.section_view.controls.append(
+            flet.Row(
+                [delete_button],
+                alignment=flet.MainAxisAlignment.CENTER
+            )
+        )
+
+    def done_edit(self, *args):
         new_widget_properties_dict = {}
         for P in self.all_fields:
             new_widget_properties_dict[P] = self.all_fields[P].value
-        
 
         if int(self.widget_number) == int(self.rearrange_slider.value):
-            #? If the widget arrange is the same.
-            self.main_widget_mother_class.template["widgets"][self.widget_number]["properties"].update(new_widget_properties_dict)
+            # If the widget arrange is the same.
+            self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number][
+                "properties"].update(new_widget_properties_dict)
         else:
-            #? If the widget arrange is NOT the same.
-            if int(self.rearrange_slider.value) >= int(len(self.main_widget_mother_class.template["widgets"])):
-                self.main_widget_mother_class.template["widgets"][self.widget_number]["properties"].update(new_widget_properties_dict)
-                copy_of_content = self.main_widget_mother_class.template["widgets"][self.widget_number]
-                del self.main_widget_mother_class.template["widgets"][self.widget_number]
-                
-                self.main_widget_mother_class.template["widgets"].append(copy_of_content)
+            # If the widget arrange is NOT the same.
+            if int(self.rearrange_slider.value) >= int(
+                    len(self.main_class.dict_content["pages"][self.main_class.current_page_name]["widgets"])):
+                self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number][
+                    "properties"].update(new_widget_properties_dict)
+                copy_of_content = self.main_class.dict_content["pages"][self.current_page_name]["widgets"][
+                    self.widget_number]
+                del self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]
 
-                self.widget_number = int(len(self.main_widget_mother_class.template["widgets"])-1)
+                self.main_class.dict_content["pages"][self.current_page_name]["widgets"].append(copy_of_content)
+
+                self.widget_number = int(
+                    len(self.main_class.dict_content["pages"][self.current_page_name]["widgets"]) - 1)
             else:
-                self.main_widget_mother_class.template["widgets"][self.widget_number]["properties"].update(new_widget_properties_dict)
-                copy_of_content = self.main_widget_mother_class.template["widgets"][self.widget_number]
-                
-                self.main_widget_mother_class.template["widgets"][int(self.rearrange_slider.value)] = copy_of_content
-                del self.main_widget_mother_class.template["widgets"][self.widget_number]
+                self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number][
+                    "properties"].update(new_widget_properties_dict)
+                copy_of_content = self.main_class.dict_content["pages"][self.current_page_name]["widgets"][
+                    self.widget_number]
+
+                self.main_class.dict_content["pages"][self.current_page_name]["widgets"][
+                    int(self.rearrange_slider.value)] = copy_of_content
+                del self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]
 
                 self.widget_number = int(self.rearrange_slider.value)
 
-        
-        #? Update the viewer engine to see the edit changes.
-        self.main_widget_mother_class.update_preview()
+        # Update the viewer engine to see the edit changes.
         self.main_class.preview_section.update_preview(self.main_class.current_page_name)
         self.main_class.page.update()
 
-        #? ReOpen the editor again
-        editSubWidgetsEngine(main_class=self.main_class, main_widget_mother_class=self.main_widget_mother_class, section_view=self.section_view, widget_number=self.widget_number)
+        # ReOpen the editor again
+        EditWidgetsEngine(
+            main_class=self.main_class,
+            section_view=self.section_view,
+            widget_number=self.widget_number
+        )
         self.main_class.page.update()
 
-    def delete_widget (self, *args):
-        del self.main_widget_mother_class.template["widgets"][self.widget_number]
+    def delete_widget(self, *args):
+        del self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]
         self.section_view.clean()
 
-        #? Update the viewer engine to see the edit changes.
+        # Update the viewer engine to see the edit changes.
         self.main_class.preview_section.update_preview(self.main_class.current_page_name)
-        self.main_class.page.update()
+        self.main_class.page.update()
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/Engines/edit_widget_engine.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/engines/edit_subwidgets_engine.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,145 +1,211 @@
 import flet
 
-from ..WIDGETS.All import all_widgets
-from ..Tools.color_picker import colorPicker
-from ..Tools.list_picker import ListPopup
+from ..widgets.All import all_widgets
+from ..tools.color_picker import ColorPicker
+from ..tools.list_picker import ListPopup
 
 
-class editWidgetsEngine:
-    def __init__(self, main_class, section_view:flet.Column, widget_number) -> None:
+# main_widget_mother_class: is the widgets mother like row or column.
+class EditSubWidgetsEngine:
+    def __init__(self, main_class, main_widget_mother_class, section_view: flet.Column, widget_number) -> None:
         self.main_class = main_class
+        self.main_widget_mother_class = main_widget_mother_class
         self.section_view = section_view
         self.widget_number = widget_number
 
-        self.current_page_name = self.main_class.current_page_name
         self.all_fields = {}
 
         self.show_edit_tools()
-    
-    def show_edit_tools (self):
+
+    def show_edit_tools(self):
+        # Update the ViewerEngine.
+        self.main_class.preview_section.update_preview(self.main_class.current_page_name)
+
+        # start
         self.section_view.clean()
-        content = self.main_class.dict_content
-        class_name = content["pages"][self.current_page_name]["widgets"][self.widget_number]["widget_class_name"]
-        widget_content = content["pages"][self.current_page_name]["widgets"][self.widget_number]
+        content = self.main_widget_mother_class.template["widgets"]
+        class_name = content[self.widget_number]["widget_class_name"]
+        widget_content = content[self.widget_number]
 
+        # widget not found
         if class_name not in all_widgets:
-            #? if widget not found.
-            self.section_view.controls.append(flet.Row([flet.Text(f"There is no supported\nwidget named '{class_name}'.", color="white")]))
+            self.section_view.controls.append(
+                flet.Row(
+                    [
+                        flet.Text(
+                            f"There is no supported\nwidget named '{class_name}'.",
+                            color=flet.colors.WHITE
+                        )
+                    ]
+                )
+            )
             return
-        
+
         the_class = all_widgets[class_name]["class"]
-        the_class = the_class(self.main_class, self.main_class.preview_section.main_view, widget_number=self.widget_number)
+        the_class = the_class(
+            self.main_class,
+            self.main_widget_mother_class.preview_section,
+            widget_number=self.widget_number
+        )
         default_args = the_class.args
-        
-        title = flet.Text(f"Edit {class_name}", size=25, weight="bold", color="white")
+
+        title = flet.Text(f"Edit {class_name}", size=25, weight=flet.FontWeight.BOLD, color=flet.colors.WHITE)
         self.section_view.controls.append(title)
 
         for t in widget_content["properties"]:
             prop_name = t
             prop_value = widget_content["properties"][t]
-            if prop_name not in default_args: print("Error while load widget properties in edit engine."); self.section_view.clean(); return
+            if prop_name not in default_args:
+                print("Error while load widget properties in edit engine.")
+                self.section_view.clean()
+                return
             prop_type = default_args[prop_name]["type"]
-            
-            #* This statments bellow is for adding the fields for edit a widget.
-            if type(prop_type()) == type(str()):
-                tf = flet.TextField(width=160, bgcolor="white", color="black", label=prop_name)
+
+            # This statement below is for adding the fields for edit a widget.
+            if isinstance(prop_type(), str):
+                tf = flet.TextField(width=160, bgcolor=flet.colors.WHITE, color=flet.colors.BLACK, label=prop_name)
                 tf.value = prop_value
-                self.section_view.controls.append(flet.Row([tf], alignment="center"))
+                self.section_view.controls.append(flet.Row([tf], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = tf
                 if "multi_line" in default_args[prop_name]:
                     tf.multiline = True
-            elif type(prop_type()) == type(int()):
+
+            elif isinstance(prop_type(), int):
                 slid = flet.Slider(min=0, max=500, divisions=500, label="{value}", width=160)
                 slid.value = int(prop_value)
-                self.section_view.controls.append(flet.Row([flet.Text(f"{prop_name}:", color="white", width=150)], alignment="center"))
-                self.section_view.controls.append(flet.Row([slid], alignment="center"))
+                self.section_view.controls.append(
+                    flet.Row(
+                        [flet.Text(f"{prop_name}:", color=flet.colors.WHITE, width=150)],
+                        alignment=flet.MainAxisAlignment.CENTER
+                    )
+                )
+                self.section_view.controls.append(flet.Row([slid], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = slid
-            elif type(prop_type()) == type(bool()):
+
+            elif isinstance(prop_type(), bool):
                 tog = flet.Switch()
                 tog.value = prop_value
-                self.section_view.controls.append(flet.Row([flet.Text(f"{prop_name}",color="white", size=13), tog], alignment="center", spacing=25))
+                self.section_view.controls.append(
+                    flet.Row([flet.Text(f"{prop_name}", color=flet.colors.WHITE, size=13), tog],
+                             alignment=flet.MainAxisAlignment.CENTER, spacing=25))
                 self.all_fields[prop_name] = tog
-            elif type(prop_type()) == type(colorPicker()):
+
+            elif type(prop_type()) == type(ColorPicker()):
                 self.section_view.controls.append(flet.Text(""))
-                colp = colorPicker(self.section_view, title_name=prop_name, drop_width=120, selected_color=prop_value, add_it=False)
-                self.section_view.controls.append(flet.Row([colp.v], alignment="center"))
+                colp = ColorPicker(
+                    self.section_view,
+                    selected_color=prop_value,
+                    add_it=False,
+                    title_name=prop_name,
+                    drop_width=120
+                )
+                self.section_view.controls.append(flet.Row([colp.v], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = colp
-            elif type(prop_type()) == type(list()):
+
+            elif isinstance(prop_type(), list):
                 dr = flet.Dropdown(width=160, label=prop_name)
                 for i in default_args[prop_name]["options"]:
                     dr.options.append(flet.dropdown.Option(f"{i}"))
                 dr.value = prop_value
-                self.section_view.controls.append(flet.Row([dr], alignment="center"))
+                self.section_view.controls.append(flet.Row([dr], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = dr
+
             elif type(prop_type()) == type(ListPopup()):
                 lp = ListPopup(default_args[prop_name]["options"], self.main_class, prop_value, prop_name)
-                self.section_view.controls.append(flet.Row([lp.self_ui], alignment="center"))
+                self.section_view.controls.append(flet.Row([lp.self_ui], alignment=flet.MainAxisAlignment.CENTER))
                 self.all_fields[prop_name] = lp
-        
 
-        #* This button bellow for widgets that support sub-widgets.
+        # This button below for widgets that support sub-widgets.
         if hasattr(the_class, "support_sub_widgets"):
             add_sub_widget_button = flet.TextButton("Add sub-widget", on_click=the_class.widgets_to_add_in)
-            self.section_view.controls.append(flet.Row([add_sub_widget_button], alignment="center"))
+            self.section_view.controls.append(
+                flet.Row([add_sub_widget_button], alignment=flet.MainAxisAlignment.CENTER))
 
-        
-
-        #* This slider bellow is for rearrange the widget on the page.
-        rearrange_slider = flet.Slider(min=0, max=len(content["pages"][self.current_page_name]["widgets"]), 
-        value=self.widget_number, label="{value}", width=160, divisions=len(content["pages"][self.current_page_name]["widgets"]))
-        self.section_view.controls.append(flet.Row([flet.Text(f"reArrange:", color="white", width=150)], alignment="center"))
-        self.section_view.controls.append(flet.Row([rearrange_slider], alignment="center"))
+        # This slider below is for rearranging the widget on the page.
+        rearrange_slider = flet.Slider(
+            min=0,
+            max=len(content),
+            value=self.widget_number,
+            label="{value}",
+            width=160,
+            divisions=len(content)
+        )
+        self.section_view.controls.append(
+            flet.Row([flet.Text(f"reArrange:", color=flet.colors.WHITE, width=150)],
+                     alignment=flet.MainAxisAlignment.CENTER))
+        self.section_view.controls.append(flet.Row([rearrange_slider], alignment=flet.MainAxisAlignment.CENTER))
         self.rearrange_slider = rearrange_slider
-        
+
         self.section_view.controls.append(flet.Text("\n"))
-        #* Down bellow is for done_button and delete_btn.
-        done_button = flet.ElevatedButton("Done", bgcolor="white", color="black", width=150, height=40, on_click=self.done_edit)
-        self.section_view.controls.append(flet.Row([done_button], alignment="center"))
-
-        delete_button = flet.TextButton(content=flet.Text("delete", color="red", size=13), on_click=self.delete_widget)
-        self.section_view.controls.append(flet.Row([delete_button], alignment="center"))
-    
-    def done_edit (self, *args):
+        # Down bellow is for done_button and delete_btn.
+        done_button = flet.ElevatedButton(
+            "Done",
+            bgcolor=flet.colors.WHITE,
+            color=flet.colors.BLACK,
+            width=150,
+            height=40,
+            on_click=self.done_edit
+        )
+        self.section_view.controls.append(flet.Row([done_button], alignment=flet.MainAxisAlignment.CENTER))
+
+        delete_button = flet.TextButton(
+            content=flet.Text(
+                "delete",
+                color=flet.colors.RED,
+                size=13
+            ),
+            on_click=self.delete_widget
+        )
+        self.section_view.controls.append(flet.Row([delete_button], alignment=flet.MainAxisAlignment.CENTER))
+
+    def done_edit(self, *args):
         new_widget_properties_dict = {}
         for P in self.all_fields:
             new_widget_properties_dict[P] = self.all_fields[P].value
-        
 
         if int(self.widget_number) == int(self.rearrange_slider.value):
-            #? If the widget arrange is the same.
-            self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]["properties"].update(new_widget_properties_dict)
+            # If the widget arrange is the same.
+            self.main_widget_mother_class.template["widgets"][self.widget_number]["properties"].update(
+                new_widget_properties_dict)
         else:
-            #? If the widget arrange is NOT the same.
-            if int(self.rearrange_slider.value) >= int(len(self.main_class.dict_content["pages"][self.main_class.current_page_name]["widgets"])):
-                self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]["properties"].update(new_widget_properties_dict)
-                copy_of_content = self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]
-                del self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]
-                
-                self.main_class.dict_content["pages"][self.current_page_name]["widgets"].append(copy_of_content)
+            # If the widget arrange is NOT the same.
+            if int(self.rearrange_slider.value) >= int(len(self.main_widget_mother_class.template["widgets"])):
+                self.main_widget_mother_class.template["widgets"][self.widget_number]["properties"].update(
+                    new_widget_properties_dict)
+                copy_of_content = self.main_widget_mother_class.template["widgets"][self.widget_number]
+                del self.main_widget_mother_class.template["widgets"][self.widget_number]
+
+                self.main_widget_mother_class.template["widgets"].append(copy_of_content)
 
-                self.widget_number = int(len(self.main_class.dict_content["pages"][self.current_page_name]["widgets"])-1)
+                self.widget_number = int(len(self.main_widget_mother_class.template["widgets"]) - 1)
             else:
-                self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]["properties"].update(new_widget_properties_dict)
-                copy_of_content = self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]
-                
-                self.main_class.dict_content["pages"][self.current_page_name]["widgets"][int(self.rearrange_slider.value)] = copy_of_content
-                del self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]
+                self.main_widget_mother_class.template["widgets"][self.widget_number]["properties"].update(
+                    new_widget_properties_dict)
+                copy_of_content = self.main_widget_mother_class.template["widgets"][self.widget_number]
+
+                self.main_widget_mother_class.template["widgets"][int(self.rearrange_slider.value)] = copy_of_content
+                del self.main_widget_mother_class.template["widgets"][self.widget_number]
 
                 self.widget_number = int(self.rearrange_slider.value)
 
-        
-        #? Update the viewer engine to see the edit changes.
+        # Update the viewer engine to see the edit changes.
+        self.main_widget_mother_class.update_preview()
         self.main_class.preview_section.update_preview(self.main_class.current_page_name)
         self.main_class.page.update()
 
-        #? ReOpen the editor again
-        editWidgetsEngine(main_class=self.main_class, section_view=self.section_view, widget_number=self.widget_number)
+        # Reopen the editor again
+        EditSubWidgetsEngine(
+            main_class=self.main_class,
+            main_widget_mother_class=self.main_widget_mother_class,
+            section_view=self.section_view,
+            widget_number=self.widget_number
+        )
         self.main_class.page.update()
 
-    def delete_widget (self, *args):
-        del self.main_class.dict_content["pages"][self.current_page_name]["widgets"][self.widget_number]
+    def delete_widget(self, *args):
+        del self.main_widget_mother_class.template["widgets"][self.widget_number]
         self.section_view.clean()
 
-        #? Update the viewer engine to see the edit changes.
+        # Update the ViewerEngine to see the edit changes.
         self.main_class.preview_section.update_preview(self.main_class.current_page_name)
-        self.main_class.page.update()
+        self.main_class.page.update()
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/Engines/suggesting_engine.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/engines/suggesting_engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,161 @@
 import json
 import flet
 import random
 import os
 import requests
 
+
 class SuggestingEngine:
     def __init__(self, main_class):
         self.main_class = main_class
 
-        self.main_col = flet.Column(width=self.main_class.left_section.main_container.width, 
-        height=self.main_class.left_section.main_container.height, scroll=True)
+        self.main_col = flet.Column(
+            width=self.main_class.left_section.main_container.width,
+            height=self.main_class.left_section.main_container.height,
+            # issue: True is not a valid value for the scroll mode. Use flet.SCROLL_MODE
+            scroll=True
+        )
 
     def push_new_suggestion(self):
         settings = self.main_class.dict_content["storyboard_settings"]
         applied = settings["storyboard_suggestions"]
-        if applied == False: return # if `storyboard suggestions` is off.
-        # -----------------------------------------------------------------------
-        suggestions_rules_name = self.main_class.dict_content["pages"][self.main_class.current_page_name]["settings"]["suggestions_rules"]
-        if suggestions_rules_name == "none": return
-        #? Get the rules file
+
+        # if `storyboard suggestions` is off.
+        if not applied:
+            return
+
+        suggestions_rules_name = self.main_class.dict_content["pages"][self.main_class.current_page_name]["settings"][
+            "suggestions_rules"]
+
+        if suggestions_rules_name == "none":
+            return
+
+        # Get the rules file
         if not os.path.isdir("rules"):
             os.mkdir("rules")
-        
+
         if not os.path.isfile(f"rules/{suggestions_rules_name}.json"):
             all_rules = requests.get("https://raw.githubusercontent.com/SKbarbon/Flet_StoryBoard/main/rules/all.json").text
             all_rules = json.loads(all_rules)
-            if suggestions_rules_name not in all_rules["all_rules"]: return
+
+            if suggestions_rules_name not in all_rules["all_rules"]:
+                return
             else:
                 rf = requests.get(all_rules["all_rules"][suggestions_rules_name]).text
                 open(f"rules/{suggestions_rules_name}.json", "w+", encoding="utf-8").write(rf)
-        
+
         rules_file = json.loads(open(f"rules/{suggestions_rules_name}.json", encoding="utf-8").read())
 
-        #? step1: Get current widgets.
+        # step1: Get current widgets.
         current_widgets = list(self.main_class.dict_content["pages"][self.main_class.current_page_name]["widgets"])
 
-        #? step2: Count classes on widgets.
+        # step2: Count classes on widgets.
         classes_in_widgets = {}
         for c in current_widgets:
             if c["widget_class_name"] not in classes_in_widgets:
                 classes_in_widgets[c["widget_class_name"]] = 1
             else:
                 classes_in_widgets[c["widget_class_name"]] = classes_in_widgets[c["widget_class_name"]] + 1
-        
 
-        #? step3: Search for the correct case on the rules file.
+        # step3: Search for the correct case on the rules file.
         for rule in rules_file["rules"]:
             if rule["case"] == classes_in_widgets:
                 self.change_left_section_into_suggestion(rule["sugs"])
                 break
-    
 
-    def change_left_section_into_suggestion (self, suggestions):
-        def go_back (e):
+    def change_left_section_into_suggestion(self, suggestions):
+        def go_back(e):
             if last_on_section == self.main_col:
                 self.main_class.left_section.show_all_widgets()
             else:
                 self.main_class.left_section.show_new_content(last_on_section)
-        
-        main_clo = self.main_col
-        main_clo.controls.clear()
-        
+
+        main_col = self.main_col
+        main_col.controls.clear()
+
         back_btn = flet.TextButton("< Back", on_click=go_back)
-        main_clo.controls.append(back_btn)
+        main_col.controls.append(back_btn)
 
-        title = flet.Text("Suggestions ✨", weight="bold", size=22, color="white")
-        main_clo.controls.append(title)
+        title = flet.Text("Suggestions ✨", weight=flet.FontWeight.BOLD, size=22, color=flet.colors.WHITE)
+        main_col.controls.append(title)
 
-        main_clo.controls.append(flet.Row([flet.Text("", color="white", size=13)], alignment="center"))
+        main_col.controls.append(
+            flet.Row(
+                [flet.Text("", color=flet.colors.WHITE, size=13)],
+                alignment=flet.MainAxisAlignment.CENTER
+            )
+        )
 
         for sug in suggestions:
             sc = self.suggestion_card(sug, go_back)
-            main_clo.controls.append(flet.Row([sc], alignment="center"))
+            main_col.controls.append(
+                flet.Row(
+                    [sc],
+                    alignment=flet.MainAxisAlignment.CENTER
+                )
+            )
 
         last_on_section = self.main_class.left_section.main_container
         self.main_class.left_section.show_new_content(self.main_col)
 
-    def suggestion_card (self, suggestion_dict, go_back_function):
-        def add_widget (e):
+    def suggestion_card(self, suggestion_dict, go_back_function):
+        def add_widget(e):
             go_back_function(e)
             w = self.main_class.add_new_widget(suggestion_dict["class"])
             w.update(suggestion_dict["props"])
             self.main_class.preview_section.update_preview(self.main_class.current_page_name)
-            self.main_class.edit_a_widget(len(self.main_class.dict_content["pages"][self.main_class.current_page_name]["widgets"])-1)
+            self.main_class.edit_a_widget(len(self.main_class.dict_content["pages"][self.main_class.current_page_name]["widgets"]) - 1)
             self.main_class.page.update()
-        # -----
-        colors = ["white", "#F5DEE5", "yellow"]
-        card_container = flet.Container(bgcolor=random.choice(colors), width=170, height=225, border_radius=13)
-        collumn = flet.Column()
-        card_container.content = collumn
+
+        colors = [flet.colors.WHITE, "#F5DEE5", flet.colors.YELLOW]
+
+        card_container = flet.Container(
+            bgcolor=random.choice(colors),
+            width=170,
+            height=225,
+            border_radius=13
+        )
+        column = flet.Column()
+        card_container.content = column
 
         class_name = suggestion_dict["class"]
         why_to_add = suggestion_dict["about"]
 
-        title = flet.Text(value=f"\n   {class_name}", size=23, weight="bold", color="black", width=card_container.width)
-        collumn.controls.append(title)
-
-        about = flet.Text(value=f"{why_to_add}", size=13, color="black", width=card_container.width-37, height=90)
-        collumn.controls.append(flet.Row([about], alignment="center"))
+        title = flet.Text(
+            value=f"\n   {class_name}",
+            size=23,
+            weight=flet.FontWeight.BOLD,
+            color=flet.colors.BLACK,
+            width=card_container.width
+        )
+        about = flet.Text(
+            value=f"{why_to_add}",
+            size=13,
+            color=flet.colors.BLACK,
+            width=card_container.width - 37,
+            height=90
+        )
+        apply_button = flet.Container(
+            flet.Row(
+                [flet.Text("Add", color="white")],
+                alignment=flet.MainAxisAlignment.CENTER
+            ),
+            bgcolor=flet.colors.BLACK,
+            width=card_container.width - 15,
+            height=40,
+            border_radius=13,
+            on_click=add_widget
+        )
+
+        column.controls.append(title)
+        column.controls.append(flet.Row([about], alignment=flet.MainAxisAlignment.CENTER))
+        column.controls.append(
+            flet.Row(
+                [apply_button],
+                alignment=flet.MainAxisAlignment.CENTER
+            )
+        )
 
-        apply_button = flet.Container(flet.Row([
-            flet.Text("Add", color="white")
-        ], alignment="center"), bgcolor="black", width=card_container.width-15, height=40, border_radius=13, on_click=add_widget)
-        collumn.controls.append(flet.Row([apply_button], alignment="center"))
+        # issue: column is not updated: column.update()
 
-        return card_container
+        return card_container
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/Engines/viewer_engine.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/engines/viewer_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from flet import Page, Container
 import flet
 
-from ..WIDGETS.All import all_widgets
+from ..widgets.All import all_widgets
 
 
 class viewerEngine:
     def __init__ (self, main_class, content_dict:dict, page_name, parent_view, widgets_parent_view, development=True):
         """
         This is the engine of preview.
         parent_view -> is the Container in the develop case, and Page in the production case
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/color_picker.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/tools/color_picker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,105 @@
 from flet import Container, Row, Column
 import flet
 
 
 def none(*args):
     pass
 
-class colorPicker:
 
-    def __init__(self, mainview=None, selected_color="white", on_choose_color=none, add_it=True, title_name="select color", drop_width=200, color_prev_width=50) -> None:
-        if mainview == None: return
+class ColorPicker:
+
+    def __init__(
+            self,
+            main_view=None,
+            selected_color="white",
+            on_choose_color=none,
+            add_it=True,
+            title_name="select color",
+            drop_width=200,
+            color_prev_width=50
+    ) -> None:
+
+        if main_view is None:
+            return
         self.__all_colors = ["None", "white", "black", "pink", "red", "green", "yellow", "blue", "hex-color"]
 
         self.drop_width = drop_width
         self.on_choose_color = on_choose_color
-        self.mainview = mainview
+        self.main_view = main_view
         self.selected_color = selected_color
 
         v = Container()
         self.v = v
 
-        main_dropdown = flet.Dropdown(width=drop_width, value=selected_color, label=title_name, on_change=self.on_choose)
+        main_dropdown = flet.Dropdown(width=drop_width, value=selected_color, label=title_name,
+                                      on_change=self.on_choose)
         for i in self.__all_colors:
             main_dropdown.options.append(flet.dropdown.Option(i))
         self.mainDropdown = main_dropdown
 
-        color_preview = flet.Container(width=color_prev_width, height=50, bgcolor=self.selected_color, border_radius=8, border=flet.border.all(0.1, "white"))
+        color_preview = flet.Container(width=color_prev_width, height=50, bgcolor=self.selected_color, border_radius=8,
+                                       border=flet.border.all(0.1, "white"))
         self.color_preview = color_preview
 
-        main_row = Row(controls=[
-            main_dropdown,
-            color_preview
-        ])
+        main_row = Row(
+            controls=[
+                main_dropdown,
+                color_preview
+            ]
+        )
         self.main_row = main_row
 
         v.content = main_row
         if add_it:
-            mainview.controls.append(v)
-    
+            main_view.controls.append(v)
 
-    def on_choose (self, me):
-        def on_change_color (me):
+    def on_choose(self, me):
+        def on_change_color(me):
             tfc.value = str(tfc.value).replace(" ", "")
             tfc.update()
             if tfc.value != "#":
                 new_color_selected = tfc.value
                 self.selected_color = tfc.value
                 self.color_preview.bgcolor = tfc.value
                 self.on_choose_color(tfc.value)
             self.v.update()
-        
-        def back_to_orig (me):
+
+        def back_to_orig(me):
             self.color_preview.on_click = None
             self.selected_color = "white"
             self.mainDropdown.value = self.selected_color
             self.color_preview.bgcolor = self.selected_color
             self.main_row.controls[0] = self.mainDropdown
             self.v.update()
 
         new_color_selected = me.control.value
-        tfc = flet.TextField(label="hex-color", value="#0", width=self.drop_width, on_change=on_change_color, on_submit=on_change_color)
+        tfc = flet.TextField(
+            label="hex-color",
+            value="#0",
+            width=self.drop_width,
+            on_change=on_change_color,
+            on_submit=on_change_color
+        )
 
         if str(new_color_selected) == "hex-color":
             self.main_row.controls[0] = tfc
             self.color_preview.on_click = back_to_orig
         elif str(new_color_selected) == "None":
             self.color_preview.bgcolor = None
             self.selected_color = None
             self.on_choose_color(new_color_selected)
         else:
             self.color_preview.bgcolor = new_color_selected
             self.selected_color = new_color_selected
             self.on_choose_color(new_color_selected)
-        
+
         self.v.update()
-    
+
     def update(self):
         self.mainDropdown.value = self.selected_color
         self.color_preview.bgcolor = self.selected_color
         self.v.update()
-    
 
     @property
-    def value (self):
-        return self.selected_color
+    def value(self):
+        return self.selected_color
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/create_storyboard.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/tools/create_storyboard.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import json
 
 
-def Create_StoryBoard (file_name, template="default", storyboard_suggestions=False, main_page_suggestions_rules="none"):
+def Create_StoryBoard(file_name, template="default", storyboard_suggestions=False, main_page_suggestions_rules="none"):
     if template == "default":
-        storyboard_defualt_template = {
-            "storyboard_settings" : {
-                "template" : "default",
-                "storyboard_suggestions" : storyboard_suggestions,
-                "allow_scroll" : False
+        storyboard_default_template = {
+            "storyboard_settings": {
+                "template": "default",
+                "storyboard_suggestions": storyboard_suggestions,
+                "allow_scroll": False
             },
-            "pages" : {
-                "main" : {
-                    "settings" : {
-                        "bgcolor" : "black",
-                        "suggestions_rules" : f"{main_page_suggestions_rules}"
+            "pages": {
+                "main": {
+                    "settings": {
+                        "bgcolor": "black",
+                        "suggestions_rules": f"{main_page_suggestions_rules}"
                     },
-                    "widgets" : [
-                        
+                    "widgets": [
+
                     ]
                 }
             }
         }
 
-
         file = open(f"{file_name}.fletsb", "w+", encoding="utf-8")
-        file.write(json.dumps(storyboard_defualt_template))
+        file.write(json.dumps(storyboard_default_template))
         return True
     else:
-        print("External templates are nor supported yet.")
+        print("External templates are nor supported yet.")
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/get_url_icon.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/tools/get_url_icon.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import requests
 import urllib3
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-def get_site_favicon (url):
-	response = requests.get(url, verify=False)
-	soup = BeautifulSoup(response.text, 'html.parser')
-	favicon_link = soup.find('link', rel='icon') or soup.find('link', rel='shortcut icon') or soup.find('link', rel='apple-touch-icon')
-	try:
-		favicon_url = favicon_link['href']
-		if str(favicon_url).startswith("http"):
-			return f"{favicon_url}"
-		else:
-			return f"{url}/{favicon_url}"
-	except:
-		return None
+
+def get_site_favicon(url):
+    response = requests.get(url, verify=False)
+    soup = BeautifulSoup(response.text, 'html.parser')
+    favicon_link = soup.find('link', rel='icon') or soup.find('link', rel='shortcut icon') or soup.find('link', rel='apple-touch-icon')
+    try:
+        favicon_url = favicon_link['href']
+        if str(favicon_url).startswith("http"):
+            return f"{favicon_url}"
+        else:
+            return f"{url}/{favicon_url}"
+    except:
+        return None
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/Tools/list_picker.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/tools/list_picker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,90 @@
 import flet
 
+
 class ListPopup:
-    def __init__ (self, the_list=None, main_class=None, default_choice=None, title=None):
-        if the_list == None: return
-        import random
+    def __init__(self, the_list=None, main_class=None, default_choice=None, title=None):
+        if the_list is None:
+            return
 
         self.title = title
-        self.page : flet.Page = main_class.page
+        self.page: flet.Page = main_class.page
         self.main_class = main_class
         self.self_ui = flet.TextButton(f"{title}: f{default_choice}", on_click=self.show_popup)
         self.the_list = the_list
         self.__selected = default_choice
 
-    
-    def show_popup (self, *args):
-        def on_search (e):
+    def show_popup(self, *args):
+        def on_search(e):
             for i in self.all_list_choices:
                 col.controls.remove(i)
+
             self.all_list_choices = []
+
             if search_field.value == "":
                 for icon in self.the_list:
                     name = str(icon)
-                    if name.startswith("__"): pass
+                    if name.startswith("__"):
+                        pass
                     else:
                         self.all_list_choices.append(self.generate_new(name, col))
                 col.update()
                 return
+
             self.all_list_choices = []
             self.all_list_choices.clear()
             s = str(search_field.value).lower()
+
             for i in self.the_list:
                 name = str(i)
                 if str(i).lower().startswith(s):
                     self.all_list_choices.append(self.generate_new(name, col))
             col.update()
-        
-        # ---
-        page : flet.Page = self.main_class.page
+
+        page: flet.Page = self.main_class.page
+
+        cont = flet.Container(bgcolor=flet.colors.BLACK, border_radius=12)
+        loading_text = flet.Text("Loading..", color=flet.colors.WHITE)
+        cont.content = flet.Row([loading_text], alignment=flet.MainAxisAlignment.CENTER, height=100)
+
         page.dialog = flet.AlertDialog()
-        cont = flet.Container(bgcolor="black", border_radius=12)
-        loading_text = flet.Text("Loading..", color="white")
-        cont.content = flet.Row([loading_text], alignment="center", height=100)
         page.dialog.content = cont
-
         page.dialog.open = True
         page.update()
 
         col = flet.ListView(width=450, height=500)
-        col.controls.append(flet.Text("Choose one:", color="white", size=28, weight="bold"))
+        col.controls.append(flet.Text("Choose one:", color="white", size=28, weight=flet.FontWeight.BOLD))
 
         search_field = flet.TextField(label="Search", on_change=on_search)
         col.controls.append(search_field)
-        
+
         self.all_list_choices = []
         for icon in self.the_list:
             name = str(icon)
-            if name.startswith("__"): pass
+            if name.startswith("__"):
+                pass
             else:
                 self.all_list_choices.append(self.generate_new(name, col))
 
         cont.content = col
         page.update()
-    
-    def generate_new (self, value_name, col):
+
+    def generate_new(self, value_name, col):
         def on_choose(e):
             self.self_ui.text = f"{self.title}: f{value_name}"
             self.__selected = value_name
             self.page.dialog.open = False
             self.page.update()
-        
-        r = flet.Row([flet.Icon(value_name, size=22, color="white"), flet.Text(f"{value_name}", color="white")])
+
+        r = flet.Row(
+            [
+                flet.Icon(value_name, size=22, color=flet.colors.WHITE),
+                flet.Text(f"{value_name}", color=flet.colors.WHITE)
+            ]
+        )
         cc = flet.Container(content=r, on_click=on_choose)
         col.controls.append(cc)
         return cc
-    
-    
+
     @property
-    def value (self):
-        return self.__selected
+    def value(self):
+        return self.__selected
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/button.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/button.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,75 @@
 import flet
-from ...Tools.color_picker import colorPicker
+from ...tools.color_picker import ColorPicker
 
 
-class Button (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+class Button(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
         self.self_object = flet.ElevatedButton(on_click=self.on_button_click)
 
-        #? all args
+        # all args
         self.args = {
-            "text" : {"type":str, "default_value":"click me"},
-            "function name" : {"type":str, "default_value":""},
-            "text_color" : {"type":colorPicker, "default_value":"black"},
-            "bgcolor" : {"type":colorPicker, "default_value":"white"},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"},
-            "width" : {"type":int, "default_value":95},
-            "height" : {"type":int, "default_value":40},
-            "hide" : {"type":bool, "default_value":False}
+            "text": {"type": str, "default_value": "click me"},
+            "function name": {"type": str, "default_value": ""},
+            "text_color": {"type": ColorPicker, "default_value": "black"},
+            "bgcolor": {"type": ColorPicker, "default_value": "white"},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
+            "width": {"type": int, "default_value": 95},
+            "height": {"type": int, "default_value": 40},
+            "hide": {"type": bool, "default_value": False}
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Button",
-            "properties" : {}
+            "widget_class_name": "Button",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
+    def update(self, new_props: dict = None):
         t = self.self_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
-        
 
         t.text = props["text"]
         t.color = props["text_color"]
         t.bgcolor = props["bgcolor"]
         t.width = props["width"]
         t.height = props["height"]
         t.visible = props["hide"] == False
-        
-        if self.self_object.page != None:
+
+        if self.self_object.page is not None:
             self.self_object.update()
 
-    
-    def on_button_click (self, event):
+    def on_button_click(self, event):
         if self.main_class.development_mode:
             return
         else:
             props = self.template["properties"]
-            if props["function name"] == "": return
+            if props["function name"] == "":
+                return
 
             if props["function name"] in self.main_class.storyboard_class.functions:
                 self.main_class.storyboard_class.functions[props["function name"]]()
             else:
                 fn = props["function name"]
                 print(f"Pass error: There is not function found called {fn}")
-    
 
-    def return_widget (self):
+    def return_widget(self):
         props = self.template["properties"]
-        if self.main_class.development_mode == True: self.self_object.disabled = True
+        if self.main_class.development_mode:
+            self.self_object.disabled = True
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
+            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/image.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/label.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,84 @@
 import flet
-from ...Tools.color_picker import colorPicker
+from ...tools.color_picker import ColorPicker
+from ...tools.list_picker import ListPopup
 
-class Image (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+
+class Label(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
-        self.self_object = flet.Image(fit=flet.ImageFit.COVER)
+        self.self_object = flet.Row()
+        self.title_object = flet.Text()
+        self.icon_object = flet.Icon()
+
+        self.self_object.controls.append(self.icon_object)
+        self.self_object.controls.append(self.title_object)
+
+        # all args
+        all_icons = []
+        for icon in flet.icons.__dict__:
+            name = str(icon)
+            if name.startswith("__"):
+                pass
+            else:
+                all_icons.append(name)
 
-        #? all args
         self.args = {
-            "src" : {"type":str, "default_value":"https://picsum.photos/id/237/200/300"},
-            "width" : {"type":int, "default_value":150},
-            "height" : {"type":int, "default_value":150},
-            "border_radius" : {"type":int, "default_value":75},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"},
+            "title": {"type": str, "default_value": "Just me and coffee"},
+            "icon": {"type": ListPopup, "options": all_icons, "default_value": "EMOJI_FOOD_BEVERAGE_ROUNDED"},
+            "title_color": {"type": ColorPicker, "default_value": "white"},
+            "icon_color": {"type": ColorPicker, "default_value": "white"},
+            "title_size": {"type": int, "default_value": 18},
+            "icon_size": {"type": int, "default_value": 18},
+            "spacing": {"type": int, "default_value": 15},
+            "title_bold": {"type": int, "default_value": True},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"}
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Image",
-            "properties" : {}
+            "widget_class_name": "Label",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
-        img = self.self_object
+    def update(self, new_props: dict = None):
+        r = self.self_object
+        t = self.title_object
+        I = self.icon_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
 
-        img.src = props["src"]
-        img.width = props["width"]
-        img.height = props["height"]
-        img.border_radius = props["border_radius"]        
-        
-        if self.self_object.page != None:
+        r.spacing = props["spacing"]
+
+        t.value = props["title"]
+        t.color = props["title_color"]
+        t.size = props["title_size"]
+
+        if props["title_bold"]:
+            t.weight = "bold"
+        else:
+            t.weight = "normal"
+
+        I.name = props["icon"]
+        I.color = props["icon_color"]
+        I.size = props["icon_size"]
+
+        if self.self_object.page is not None:
             self.self_object.update()
-        
 
-    def return_widget (self):
+    def return_widget(self):
         props = self.template["properties"]
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
+            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/label.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/title.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,73 @@
 import flet
-from ...Tools.color_picker import colorPicker
-from ...Tools.list_picker import ListPopup
+from ...tools.color_picker import ColorPicker
 
 
-class Label (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+class Title(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
-        self.self_object = flet.Row()
-        self.title_object = flet.Text()
-        self.icon_object = flet.Icon()
-
-        self.self_object.controls.append(self.icon_object)
-        self.self_object.controls.append(self.title_object)
-
-        #? all args
-        all_icons = []
-        for icon in flet.icons.__dict__:
-            name = str(icon)
-            if name.startswith("__"): pass
-            else:
-                all_icons.append(name)
+        self.self_object = flet.Text("")
+
+        # all args
         self.args = {
-            "title" : {"type":str, "default_value":"Just me and coffee"},
-            "icon" : {"type":ListPopup, "options":all_icons, "default_value":"EMOJI_FOOD_BEVERAGE_ROUNDED"},
-            "title_color" : {"type":colorPicker, "default_value":"white"},
-            "icon_color" : {"type":colorPicker, "default_value":"white"},
-            "title_size" : {"type":int, "default_value":18},
-            "icon_size" : {"type":int, "default_value":18},
-            "spacing" : {"type":int, "default_value":15},
-            "title_bold" : {"type":int, "default_value":True},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"}
+            "title": {"type": str, "default_value": "myTitle"},
+            "title_color": {"type": ColorPicker, "default_value": "white"},
+            "size": {"type": int, "default_value": 23},
+            "width": {"type": int, "default_value": 350},
+            "italic": {"type": bool, "default_value": False},
+            "bold": {"type": bool, "default_value": True},
+            "hide": {"type": bool, "default_value": False},
+            "expand": {"type": bool, "default_value": False},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
+            "text_align": {"type": list, "options": ["left", "center", "right"], "default_value": "left"}
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Label",
-            "properties" : {}
+            "widget_class_name": "Title",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
-        r = self.self_object
-        t = self.title_object
-        I = self.icon_object
+    def update(self, new_props: dict = None):
+        t = self.self_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
 
-        r.spacing = props["spacing"]
-
         t.value = props["title"]
+        t.size = props["size"]
         t.color = props["title_color"]
-        t.size = props["title_size"]
-        if props["title_bold"]:
+        t.width = props["width"]
+        t.expand = props["expand"]
+        t.italic = props["italic"]
+        t.visible = props["hide"] == False
+        if str(props["text_align"]).lower() == "left":
+            t.text_align = flet.TextAlign.LEFT
+        elif str(props["text_align"]).lower() == "center":
+            t.text_align = flet.TextAlign.CENTER
+        elif str(props["text_align"]).lower() == "right":
+            t.text_align = flet.TextAlign.RIGHT
+
+        if props["bold"]:
             t.weight = "bold"
         else:
             t.weight = "normal"
-        
-        I.name = props["icon"]
-        I.color = props["icon_color"]
-        I.size = props["icon_size"]
-        
-        
-        if self.self_object.page != None:
+
+        if self.self_object.page is not None:
             self.self_object.update()
-        
 
-    def return_widget (self):
+    def return_widget(self):
         props = self.template["properties"]
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
+            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/markdown.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/markdown.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 import flet
-from ...Tools.color_picker import colorPicker
 
-class Markdown (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+
+class Markdown(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
-        self.self_object = flet.Markdown(selectable=True, extension_set="gitHubWeb", 
-        code_style=flet.TextStyle(font_family="Roboto Mono", color="blue"))
+        self.self_object = flet.Markdown(
+            selectable=True,
+            extension_set=flet.MarkdownExtensionSet.GITHUB_WEB,
+            code_style=flet.TextStyle(font_family="Roboto Mono", color="blue")
+        )
 
-        #? all args
+        # all args
         self.args = {
-            "content" : {"type":str, "default_value":"", "multi_line":True},
-            "code_theme" : {"type":list, "options":["a11y-dark", "arta", "atom-one-dark", "dark", "default"], "default_value":"default"},
-            "width" : {"type":int, "default_value":150},
-            "height" : {"type":int, "default_value":150},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"left"}
+            "content": {"type": str, "default_value": "", "multi_line": True},
+            "code_theme": {"type": list, "options": ["a11y-dark", "arta", "atom-one-dark", "dark", "default"],
+                           "default_value": "default"},
+            "width": {"type": int, "default_value": 150},
+            "height": {"type": int, "default_value": 150},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "left"}
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Markdown",
-            "properties" : {}
+            "widget_class_name": "Markdown",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
+    def update(self, new_props: dict = None):
         m = self.self_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
 
-        
         m.value = props["content"]
         m.width = props["width"]
         m.height = props["height"]
-        
-        if self.self_object.page != None:
+
+        if self.self_object.page is not None:
             self.self_object.update()
-        
 
-    def return_widget (self):
+    def return_widget(self):
         props = self.template["properties"]
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
+            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/navigator.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/navigator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 import flet
-from ...Tools.color_picker import colorPicker
+from ...tools.color_picker import ColorPicker
 
 
-class Navigator (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+class Navigator(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
         self.self_object = flet.ElevatedButton(on_click=self.on_button_click)
 
-        #? all args
+        # all args
         all_pages = []
         for i in self.main_class.dict_content["pages"]:
             all_pages.append(i)
         self.args = {
-            "text" : {"type":str, "default_value":"click me"},
-            "page name" : {"type":list, "options":all_pages, "default_value":"main"},
-            "width" : {"type":int, "default_value":150},
-            "height" : {"type":int, "default_value":45},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"},
-            "bgcolor" : {"type":colorPicker, "default_value":"black"},
-            "text_color" : {"type":colorPicker, "default_value":"blue"}
+            "text": {"type": str, "default_value": "click me"},
+            "page name": {"type": list, "options": all_pages, "default_value": "main"},
+            "width": {"type": int, "default_value": 150},
+            "height": {"type": int, "default_value": 45},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
+            "bgcolor": {"type": ColorPicker, "default_value": "black"},
+            "text_color": {"type": ColorPicker, "default_value": "blue"}
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Navigator",
-            "properties" : {}
+            "widget_class_name": "Navigator",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
+    def update(self, new_props: dict = None):
         t = self.self_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
-        
 
         t.text = props["text"]
         t.color = props["text_color"]
         t.bgcolor = props["bgcolor"]
         t.width = props["width"]
         t.height = props["height"]
-        
-        if self.self_object.page != None:
+
+        if self.self_object.page is not None:
             self.self_object.update()
 
-    
-    def on_button_click (self, event):
+    def on_button_click(self, event):
         if self.main_class.development_mode:
             return
         else:
             props = self.template["properties"]
             self.main_class.storyboard_class.navigate_to_page(props["page name"])
-    
 
-    def return_widget (self):
+    def return_widget(self):
         props = self.template["properties"]
-        if self.main_class.development_mode == True: self.self_object.disabled = True
+        if self.main_class.development_mode:
+            self.self_object.disabled = True
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
+            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/open_url.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/open_url.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 import flet
-import threading
-from ...Tools.color_picker import colorPicker
-from ...Tools.list_picker import ListPopup
+from ...tools.color_picker import ColorPicker
+from ...tools.list_picker import ListPopup
 
-class Open_Url (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+
+class Open_Url(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
         self.self_object = flet.Container(on_click=self.open_url)
         self.url_text = flet.Text()
         self.url_icon = flet.Icon(size=12)
-        self.self_object.content = flet.Row([self.url_icon, self.url_text], alignment="center")
+        self.self_object.content = flet.Row([self.url_icon, self.url_text], alignment=flet.MainAxisAlignment.CENTER)
 
-        #? all args
+        # all args
         all_icons = []
         for icon in flet.icons.__dict__:
             name = str(icon)
-            if name.startswith("__"): pass
+            if name.startswith("__"):
+                pass
             else:
                 all_icons.append(name)
+
         self.args = {
-            "text" : {"type":str, "default_value":"example url"},
-            "url" : {"type":str, "default_value":"https://example.com"},
-            "link icon" : {"type":ListPopup, "options":all_icons, "default_value":"INSERT_LINK_OUTLINED"},
-            "text_color" : {"type":colorPicker, "default_value":"blue"},
-            "icon_color" : {"type":colorPicker, "default_value":"blue"},
-            "bgcolor" : {"type":colorPicker, "default_value":"black"},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"},
-            "width" : {"type":int, "default_value":130},
-            "height" : {"type":int, "default_value":30},
-            "text_size" : {"type":int, "default_value":15},
-            "icon_size" : {"type":int, "default_value":15},
-            "border_radius" : {"type":int, "default_value":10},
-            "hide" : {"type":bool, "default_value":False}
+            "text": {"type": str, "default_value": "example url"},
+            "url": {"type": str, "default_value": "https://example.com"},
+            "link icon": {"type": ListPopup, "options": all_icons, "default_value": "INSERT_LINK_OUTLINED"},
+            "text_color": {"type": ColorPicker, "default_value": "blue"},
+            "icon_color": {"type": ColorPicker, "default_value": "blue"},
+            "bgcolor": {"type": ColorPicker, "default_value": "black"},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
+            "width": {"type": int, "default_value": 130},
+            "height": {"type": int, "default_value": 30},
+            "text_size": {"type": int, "default_value": 15},
+            "icon_size": {"type": int, "default_value": 15},
+            "border_radius": {"type": int, "default_value": 10},
+            "hide": {"type": bool, "default_value": False}
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Open Url",
-            "properties" : {}
+            "widget_class_name": "Open Url",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
+    def update(self, new_props: dict = None):
         c = self.self_object
         t = self.url_text
         ii = self.url_icon
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
 
-
         url = props["url"]
         c.tooltip = f"open '{url}'"
         c.width = props["width"]
         c.bgcolor = props["bgcolor"]
         c.border_radius = props["border_radius"]
         c.height = props["height"]
         c.visible = props["hide"] == False
@@ -70,24 +70,24 @@
         t.color = props["text_color"]
         t.text_align = props["text_color"]
         t.size = props["text_size"]
 
         ii.name = props["link icon"]
         ii.color = props["icon_color"]
         ii.size = props["icon_size"]
-        if self.self_object.page != None:
+        if self.self_object.page is not None:
             self.self_object.update()
-        
 
-    def open_url (self, event):
+    def open_url(self, event):
         if self.main_class.development_mode: return
         url = self.template["properties"]["url"]
         event.control.page.launch_url(url)
 
-    def return_widget (self):
+    def return_widget(self):
         props = self.template["properties"]
         if props["alignment"] == "left":
             return flet.Row([flet.Text("   "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment="right")
+            # issue: right is not a valid value
+            return flet.Row([self.self_object, flet.Text("    ")], alignment="right")
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/padding.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import flet
-from ...Tools.color_picker import colorPicker
 
-class Padding (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+
+class Image(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
-        self.self_object = flet.Text("")
-
+        self.self_object = flet.Image(fit=flet.ImageFit.COVER)
 
-        #? all args
+        # all args
         self.args = {
-            "width" : {"type":int, "default_value":50},
-            "height" : {"type":int, "default_value":50},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"}
+            "src": {"type": str, "default_value": "https://picsum.photos/id/237/200/300"},
+            "width": {"type": int, "default_value": 150},
+            "height": {"type": int, "default_value": 150},
+            "border_radius": {"type": int, "default_value": 75},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Padding",
-            "properties" : {}
+            "widget_class_name": "Image",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
-        p = self.self_object
+    def update(self, new_props: dict = None):
+        img = self.self_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
 
-        p.width = props["width"]
-        p.height = props["height"]
-        
-        if self.self_object.page != None:
+        img.src = props["src"]
+        img.width = props["width"]
+        img.height = props["height"]
+        img.border_radius = props["border_radius"]
+
+        if self.self_object.page is not None:
             self.self_object.update()
-        
 
-    def return_widget (self):
+    def return_widget(self):
         props = self.template["properties"]
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
+            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/paragraph.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/paragraph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 import flet
-from ...Tools.color_picker import colorPicker
+from ...tools.color_picker import ColorPicker
 
-class Paragraph (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+
+class Paragraph(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
         self.self_object = flet.Text("")
 
-        #? all args
+        # all args
         self.args = {
-            "text" : {"type":str, "default_value":"dude,\nThere is no one who loves pain itself, who seeks after it and wants to have it, simply because it is pain 🙃...", "multi_line":True},
-            "text_color" : {"type":colorPicker, "default_value":"white"},
-            "size" : {"type":int, "default_value":16},
-            "width" : {"type":int, "default_value":300},
-            "italic" : {"type":bool, "default_value":False},
-            "bold" : {"type":bool, "default_value":False},
-            "hide" : {"type":bool, "default_value":False},
-            "expand" : {"type":bool, "default_value":False},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"},
-            "text_align" : {"type":list, "options":["left", "center", "right"], "default_value" : "left"}
+            "text": {"type": str,
+                     "default_value": "dude,\nThere is no one who loves pain itself, who seeks after it and wants to have it, simply because it is pain 🙃...",
+                     "multi_line": True},
+            "text_color": {"type": ColorPicker, "default_value": "white"},
+            "size": {"type": int, "default_value": 16},
+            "width": {"type": int, "default_value": 300},
+            "italic": {"type": bool, "default_value": False},
+            "bold": {"type": bool, "default_value": False},
+            "hide": {"type": bool, "default_value": False},
+            "expand": {"type": bool, "default_value": False},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
+            "text_align": {"type": list, "options": ["left", "center", "right"], "default_value": "left"}
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Paragraph",
-            "properties" : {}
+            "widget_class_name": "Paragraph",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
+    def update(self, new_props: dict = None):
         t = self.self_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
 
         t.value = props["text"]
         t.size = props["size"]
         t.color = props["text_color"]
         t.width = props["width"]
         t.expand = props["expand"]
         t.italic = props["italic"]
         t.visible = props["hide"] == False
+
         if str(props["text_align"]).lower() == "left":
             t.text_align = flet.TextAlign.LEFT
         elif str(props["text_align"]).lower() == "center":
             t.text_align = flet.TextAlign.CENTER
         elif str(props["text_align"]).lower() == "right":
             t.text_align = flet.TextAlign.RIGHT
 
-        if props["bold"] == True:
+        if props["bold"]:
             t.weight = "bold"
         else:
             t.weight = "normal"
-        
-        if self.self_object.page != None:
+
+        if self.self_object.page is not None:
             self.self_object.update()
-        
 
-    def return_widget (self):
+    def return_widget(self):
         props = self.template["properties"]
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
+            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/row.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/row.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,183 +1,188 @@
-from flet import Column, Row, Container
 import flet
-from ...Tools.color_picker import colorPicker
 from ...ui_toolkit.widget_browser_frame import Widget_Browse_Frame
 
-class Row (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+
+class Row(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
         self.self_object = flet.Row()
 
-        self.widget_number = kwrds["widget_number"]
+        self.widget_number = kwargs["widget_number"]
 
-        #? Row Special args.
+        # Row Special args.
         self.dont_border_subs = True
         self.last_added = None
         self.support_sub_widgets = True
 
-        if main_class.development_mode == True:
+        if main_class.development_mode:
             self.development_mode = True
         else:
             self.development_mode = False
 
-        #? all args
+        # all args
         self.args = {
-            "width" : {"type":int, "default_value":23},
-            "height" : {"type":int, "default_value":150},
-            "hide" : {"type":bool, "default_value":False},
-            "scroll" : {"type":bool, "default_value":False},
-            "auto_scroll_to_end" : {"type":bool, "default_value":True},
-            "expand" : {"type":bool, "default_value":True},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"},
-            "sub_widgets_alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"},
+            "width": {"type": int, "default_value": 23},
+            "height": {"type": int, "default_value": 150},
+            "hide": {"type": bool, "default_value": False},
+            "scroll": {"type": bool, "default_value": False},
+            "auto_scroll_to_end": {"type": bool, "default_value": True},
+            "expand": {"type": bool, "default_value": True},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
+            "sub_widgets_alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "Row",
-            "properties" : {},
-            "widgets" : []
+            "widget_class_name": "Row",
+            "properties": {},
+            "widgets": []
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None, new_sub_widgets:dict=None):
+    def update(self, new_props: dict = None, new_sub_widgets: dict = None):
         r = self.self_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
-        
-        if new_sub_widgets != None:
+
+        if new_sub_widgets is not None:
             for w in new_sub_widgets:
                 self.template["widgets"].append(w)
 
-        
         r.width = props["width"]
         r.height = props["height"]
         r.visible = props["hide"] == False
         r.expand = props["expand"]
         r.scroll = props["scroll"]
         r.alignment = props["sub_widgets_alignment"]
         r.auto_scroll = props["auto_scroll_to_end"]
-        
-        if self.self_object.page != None:
+
+        if self.self_object.page is not None:
             self.self_object.update()
-        
+
         self.update_preview()
-    
 
-    #? Row Tools
-    def widgets_to_add_in (self, *args):
+    # Row tools
+    def widgets_to_add_in(self, *args):
+        """To show all widgets that are available to add to the row."""
         for i in args:
             i.control.visible = False
             i.control.update()
-        """
-        To show all widgets that are available to add to the row.
-        """
+
         def go_back(*e):
             self.main_class.left_section.show_new_content(copy_of_last_container)
-            if self.last_added != None:
-                if self.last_added.page == None:
+            if self.last_added is not None:
+                if self.last_added.page is None:
                     self.last_added.border = None
                     self.main_class.page.update()
                 else:
                     self.last_added.border = None
                     self.last_added.update()
             self.main_class.on_page_resize()
             for i in args:
                 i.control.visible = True
                 i.control.update()
-        
-        # ----
+
         page = self.main_class.page
-        #* This is the default section.
-        
-        col = Column(scroll=True)
+        # This is the default section.
+
+        # issue: scroll has not attribute True
+        col = flet.Column(scroll=True)
         col.controls.append(flet.TextButton("< Back", on_click=go_back))
-        title = flet.Text("Widgets in row", size=25, weight="bold", color="white")
+        title = flet.Text("Widgets in row", size=25, weight=flet.FontWeight.BOLD, color="white")
         col.controls.append(title)
         all_widgets = self.main_class.all_widgets
         for wid in all_widgets:
             w = Widget_Browse_Frame(wid, all_widgets[wid], self.add_new_widget, self.main_class.current_page_name)
             col.controls.append(w)
-        
 
-        main_container = Container(bgcolor=page.bgcolor, width=page.width/4, height=page.height)
-        main_container.content = col
+        main_container = flet.Container(
+            content=col,
+            bgcolor=page.bgcolor,
+            width=page.width / 4,
+            height=page.height
+        )
+
         copy_of_last_container = self.main_class.left_section.self_ui.content
         self.main_class.left_section.show_new_content(main_container)
         self.main_class.on_page_resize()
         self.main_class.page.update()
-    
-    def add_new_widget (self, widget_name, page_name):
-        """
-        To add the widget, and open the edit to edit this new sub-widget.
-        """
+
+    def add_new_widget(self, widget_name, page_name):
+        """To add the widget, and open the edit to edit this new sub-widget."""
         self.dont_border_subs = False
         all_widgets = self.main_class.all_widgets
         widget_class = all_widgets[widget_name]["class"]
-        widget_class = widget_class(self, self.preview_section, widget_number=len(self.template["widgets"])-1, is_a_sub=True)
-        
-    
+        widget_class = widget_class(
+            self, self.preview_section,
+            widget_number=len(self.template["widgets"]) - 1,
+            is_a_sub=True
+        )
+
         self.template["widgets"].append(widget_class.template)
         self.main_class.dict_content["pages"][self.main_class.current_page_name]["widgets"][self.widget_number]["widgets"] = self.template["widgets"]
 
         self.update_preview()
         editSubWidgetsEngine = self.main_class._editSubWidgetsEngine
-        editSubWidgetsEngine = editSubWidgetsEngine(self.main_class, self, self.main_class.edit_section.main_column, len(self.template["widgets"])-1)
+        editSubWidgetsEngine = editSubWidgetsEngine(
+            self.main_class,
+            self,
+            self.main_class.edit_section.main_column,
+            len(self.template["widgets"]) - 1
+        )
         self.main_class.page.update()
-    
 
     def update_preview(self):
         all_widgets = self.main_class.all_widgets
         self.preview_section.controls.clear()
         sub_widgets = self.template["widgets"]
         num = 0
+
         for widget in sub_widgets:
             if widget["widget_class_name"] in all_widgets:
                 widget_class = all_widgets[widget["widget_class_name"]]["class"]
                 widget_class = widget_class(self.main_class, self.preview_section)
                 if hasattr(widget_class, "support_sub_widgets"):
                     widget_class.update(widget["properties"], widget["widgets"])
                 else:
                     widget_class.update(widget["properties"])
                 if self.development_mode:
                     self.create_development_container(widget_class.return_widget(), num)
                 else:
                     self.preview_section.controls.append(widget_class.return_widget())
             num = num + 1
-        
+
         self.main_class.page.update()
 
     @property
-    def preview_section (self):
+    def preview_section(self):
         return self.self_object
-    
-    def return_widget (self):
+
+    def return_widget(self):
         props = self.template["properties"]
-        # return self.self_object
+
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
             return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER, spacing=0)
         else:
             return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.MainAxisAlignment.END)
-    
-    def create_development_container (self, cls, widget_number):
-        if self.last_added == None:
+
+    def create_development_container(self, cls, widget_number):
+        if self.last_added is None:
             c = flet.Container(cls, border_radius=8, border=flet.border.all(2, flet.colors.YELLOW_300))
             self.last_added = c
         else:
             self.last_added.border = None
             c = flet.Container(cls, border_radius=8, border=flet.border.all(2, flet.colors.YELLOW_300))
             self.last_added = c
-        
+
         self.preview_section.controls.append(c)
-        return c
+        return c
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/WIDGETS/widgets/textfield.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/widgets/widgets/textfield.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,125 @@
 import flet
-from ...Tools.color_picker import colorPicker
+from ...tools.color_picker import ColorPicker
 
 
-class TextField (object):
-    def __init__(self, main_class, parent, *args, **kwrds) -> None:
+class TextField(object):
+    def __init__(self, main_class, parent, *args, **kwargs) -> None:
         self.parent = parent
         self.main_class = main_class
-        self.self_object = flet.TextField(on_focus=self.on_start_type, on_change=self.on_change_text, on_submit=self.on_end_type, 
-        selection_color="black", cursor_color="black", focused_color="color")
+        self.self_object = flet.TextField(
+            on_focus=self.on_start_type,
+            on_change=self.on_change_text,
+            on_submit=self.on_end_type,
+            selection_color=flet.colors.BLACK,
+            cursor_color=flet.colors.BLACK,
+            # issue: focused_color can't have value "color"
+            focused_color="color"
+        )
 
-        #? all args
+        # all args
         self.args = {
-            "text" : {"type":str, "default_value":""},
-            "label" : {"type":str, "default_value":"text.."},
-            "hint_text" : {"type":str, "default_value":"text.."},
-            "can_reveal_password" : {"type":bool, "default_value":True},
-            "password" : {"type":bool, "default_value":False},
-            "width" : {"type":int, "default_value":200},
-            "height" : {"type":int, "default_value":65},
-            "border_radius" : {"type":int, "default_value":12},
-            "bgcolor" : {"type":colorPicker, "default_value":"white"},
-            "color" : {"type":colorPicker, "default_value":"black"},
-            "alignment" : {"type":list, "options":["left", "center", "right"], "default_value":"center"},
-            "on start" : {"type":str, "default_value":""},
-            "on change" : {"type":str, "default_value":""},
-            "on end" : {"type":str, "default_value":""},
-            "point name" : {"type":str, "default_value":""}
+            "text": {"type": str, "default_value": ""},
+            "label": {"type": str, "default_value": "text.."},
+            "hint_text": {"type": str, "default_value": "text.."},
+            "can_reveal_password": {"type": bool, "default_value": True},
+            "password": {"type": bool, "default_value": False},
+            "width": {"type": int, "default_value": 200},
+            "height": {"type": int, "default_value": 65},
+            "border_radius": {"type": int, "default_value": 12},
+            "bgcolor": {"type": ColorPicker, "default_value": "white"},
+            "color": {"type": ColorPicker, "default_value": "black"},
+            "alignment": {"type": list, "options": ["left", "center", "right"], "default_value": "center"},
+            "on start": {"type": str, "default_value": ""},
+            "on change": {"type": str, "default_value": ""},
+            "on end": {"type": str, "default_value": ""},
+            "point name": {"type": str, "default_value": ""}
         }
 
-        #? Template dict
-        #* This is where the widget data will be stored.
+        # Template dict
+        # This is where the widget data will be stored.
         self.template = {
-            "widget_class_name" : "TextField",
-            "properties" : {}
+            "widget_class_name": "TextField",
+            "properties": {}
         }
         for p in self.args:
             self.template["properties"][p] = self.args[p]["default_value"]
-        
+
         self.update()
 
-    
-    def update (self, new_props:dict=None):
+    def update(self, new_props: dict = None):
         tf = self.self_object
         props = self.template["properties"]
-        
-        if new_props != None:
+
+        if new_props is not None:
             for i in new_props:
                 self.template["properties"][i] = new_props[i]
-        
 
         tf.value = props["text"]
         tf.label = props["label"]
         tf.hint_text = props["hint_text"]
         tf.password = props["password"]
         tf.can_reveal_password = props["can_reveal_password"]
         tf.width = props["width"]
         tf.height = props["height"]
         tf.bgcolor = props["bgcolor"]
         tf.color = props["color"]
         tf.border_radius = props["border_radius"]
-        
-        if self.self_object.page != None:
+
+        if self.self_object.page is not None:
             self.self_object.update()
 
-    
-    def on_start_type (self, event):
+    def on_start_type(self, event):
         if self.main_class.development_mode:
             return
         else:
             props = self.template["properties"]
-            if props["on start"] == "": return
+            if props["on start"] == "":
+                return
 
             if props["on start"] in self.main_class.storyboard_class.functions:
                 self.main_class.storyboard_class.functions[props["on start"]]()
             else:
                 fn = props["on start"]
                 print(f"Pass error: There is not function found called {fn}")
-    
-    def on_change_text (self, event):
+
+    def on_change_text(self, event):
         if self.main_class.development_mode:
             return
         else:
             props = self.template["properties"]
             if props["point name"] != "":
                 self.main_class.storyboard_class.points[props["point name"]] = str(self.self_object.value)
-            if props["on change"] == "": return
+            if props["on change"] == "":
+                return
 
             if props["on change"] in self.main_class.storyboard_class.functions:
                 self.main_class.storyboard_class.functions[props["on change"]](self.self_object.value)
             else:
                 fn = props["on change"]
                 print(f"Pass error: There is not function found called {fn}")
-    
-    def on_end_type (self, event):
+
+    def on_end_type(self, event):
         if self.main_class.development_mode:
             return
         else:
             props = self.template["properties"]
             if props["point name"] != "":
                 self.main_class.storyboard_class.points[props["point name"]] = str(self.self_object.value)
             if props["on end"] == "": return
 
             if props["on end"] in self.main_class.storyboard_class.functions:
                 self.main_class.storyboard_class.functions[props["on end"]](self.self_object.value)
             else:
                 fn = props["on end"]
                 print(f"Pass error: There is not function found called {fn}")
-    
 
-    def return_widget (self):
-        if self.main_class.development_mode == True: self.self_object.disabled = True
+    def return_widget(self):
+        if self.main_class.development_mode:
+            self.self_object.disabled = True
         props = self.template["properties"]
         if props["alignment"] == "left":
             return flet.Row([flet.Text("    "), self.self_object])
         elif props["alignment"] == "center":
-            return flet.Row([self.self_object], alignment="center")
+            return flet.Row([self.self_object], alignment=flet.MainAxisAlignment.CENTER)
         else:
-            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
+            return flet.Row([self.self_object, flet.Text("    ")], alignment=flet.alignment.center_right)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/edit.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/edit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 from .pages.create_new_file import CreateNewFile
 from .pages.main_page import mainPage
 import sys
 import os
 import flet
 
-
 cmd_args = sys.argv
 debug_mode = False
 if "--debug" in cmd_args:
     debug_mode = True
 
+
 class manage_edit:
     def __init__(self) -> None:
         self.cmd_args = sys.argv
         self.file_name = None
         flet.app(target=self.CNF)
-        if self.file_name == None: 
-            if debug_mode: print("Debug alert: Unexpected exit, no errors."); sys.exit("Exit.")
+
+        if self.file_name is None and debug_mode:
+            print("Debug alert: Unexpected exit, no errors.")
+            sys.exit("Exit.")
+
         if not str(self.file_name).endswith(".fletsb"):
             self.file_name = str(self.file_name) + ".fletsb"
-        
-        if debug_mode: print("Debug alert: About to run the editor.")
+
+        if debug_mode:
+            print("Debug alert: About to run the editor.")
+
         mainPage(self.file_name)
-    
-    def CNF (self, page):
+
+    def CNF(self, page):
         CreateNewFile(page, manage_class=self)
 
 
 if len(cmd_args) == 1:
-    #? To create a new file.
-    if debug_mode: print("Debug alert: About to show the 'CreateNewFile' window.")
+    # To create a new file.
+    if debug_mode:
+        print("Debug alert: About to show the 'CreateNewFile' window.")
     manage_edit()
 else:
-    #? To edit a exist File.
+    # To edit an existing File.
     full_path = ""
     for i in range(1, len(cmd_args)):
         if full_path == "":
             full_path = full_path + cmd_args[i]
         else:
             full_path = full_path + " " + cmd_args[i]
+
     full_path = full_path.replace(" --debug", "")
     full_path = full_path.replace("--debug", "")
+
     if os.path.isfile(full_path):
-        if debug_mode: print("Debug alert: About to run the editor.")
+        if debug_mode:
+            print("Debug alert: About to run the editor.")
         mainPage(full_path)
     else:
         print(f"Warning: File not found '{full_path}', so create a new one.")
-        if debug_mode: print("Debug alert: About to show the 'CreateNewFile' window.")
-        manage_edit()
+        if debug_mode:
+            print("Debug alert: About to show the 'CreateNewFile' window.")
+        manage_edit()
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/pages/Settings/pages.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/pages/Settings/pages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,70 @@
-from flet import *
 import flet
 
-from ...Tools.color_picker import colorPicker
+from ...tools.color_picker import ColorPicker
 
-def page_settings_page (settings_class):
-    def allow_scrolling (e):
+
+def page_settings_page(settings_class):
+    def allow_scrolling(e):
         settings_class.main_class.dict_content["storyboard_settings"]["allow_scroll"] = e.control.value
-        page : flet.Page = settings_class.page
-        page.snack_bar = flet.SnackBar(flet.Text(f"Done! But this is not saved, you must go click 'Save' on the editor."))
-        page.snack_bar.open = True
+        page: flet.Page = settings_class.page
+        page.show_snack_bar(
+            flet.SnackBar(
+                flet.Text(f"Done! But this is not saved, you must go click 'Save' on the editor."),
+                open=True
+            )
+        )
         settings_class.main_class.preview_section.update_preview()
         page.update()
 
-    def on_change_bgcolor (color):
+    def on_change_bgcolor(color):
         settings_class.main_class.dict_content["pages"][current_page_name]["settings"]["bgcolor"] = color
-        page : flet.Page = settings_class.page
-        page.snack_bar = flet.SnackBar(flet.Text(f"Done! But this is not saved, you must go click 'Save' on the editor."))
-        page.snack_bar.open = True
+        page: flet.Page = settings_class.page
+        page.show_snack_bar(
+            flet.SnackBar(
+                flet.Text(f"Done! But this is not saved, you must go click 'Save' on the editor."),
+                open=True
+            )
+        )
         settings_class.main_class.preview_section.update_preview()
         page.update()
 
     v = settings_class.page_viewing_section
     v.clean()
 
     current_page_name = settings_class.main_class.current_page_name
-    title = flet.Text(f"\n   Pages - {current_page_name}", color="white", weight="bold", size=28)
+    title = flet.Text(
+        f"\n   Pages - {current_page_name}",
+        color=flet.colors.WHITE,
+        weight=flet.FontWeight.BOLD,
+        size=28
+    )
     v.controls.append(title)
 
     if "allow_scroll" not in settings_class.main_class.dict_content["storyboard_settings"]:
         settings_class.main_class.dict_content["storyboard_settings"]["allow_scroll"] = False
-    Allow_Scrolling = flet.Row([
-        flet.Text("Allow scrolling", color="white", width=300),
-        flet.Switch(on_change=allow_scrolling,
-        value=settings_class.main_class.dict_content["storyboard_settings"]["allow_scroll"])
-    ], alignment="center")
-    v.controls.append(Allow_Scrolling)
-
-    cp = colorPicker(v, settings_class.main_class.dict_content["pages"][current_page_name]["settings"]["bgcolor"], 
-    on_choose_color=on_change_bgcolor, title_name="bgcolor", add_it=False)
-    v.controls.append(flet.Container(flet.Row([cp.v], alignment="center"), bgcolor="black"))
 
-    v.update()
+    row_allow_scrolling = flet.Row(
+        [
+            flet.Text("Allow scrolling", color="white", width=300),
+            flet.Switch(
+                on_change=allow_scrolling,
+                value=settings_class.main_class.dict_content["storyboard_settings"]["allow_scroll"]
+            )
+        ],
+        alignment=flet.MainAxisAlignment.CENTER
+    )
+    v.controls.append(row_allow_scrolling)
+
+    cp = ColorPicker(v, settings_class.main_class.dict_content["pages"][current_page_name]["settings"]["bgcolor"],
+                     on_choose_color=on_change_bgcolor, add_it=False, title_name="bgcolor")
+    v.controls.append(
+        flet.Container(
+            flet.Row(
+                [cp.v],
+                alignment=flet.MainAxisAlignment.CENTER
+            ),
+            bgcolor=flet.colors.BLACK
+        )
+    )
+
+    v.update()
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/pages/create_new_file.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/pages/create_new_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,247 +1,283 @@
 import flet
 import time
 import os
 import json
 import requests
 
-from ..Tools.create_storyboard import Create_StoryBoard
+from ..tools.create_storyboard import Create_StoryBoard
 
 
 class CreateNewFile:
-    def __init__ (self, page:flet.Page, manage_class):
+    def __init__(self, page: flet.Page, manage_class):
         page.window_resizable = False
         page.update()
         page.window_center()
 
-        #? Set page prop
-        page.bgcolor = "black"
-        
-        #? Setup Content's mother.
+        # Set page prop
+        page.bgcolor = flet.colors.BLACK
+
+        # Setup Content's mother.
         self.manage_class = manage_class
         self.page = page
-        self.mother = flet.AnimatedSwitcher(expand=True, content=flet.Text(""), 
-        transition=flet.AnimatedSwitcherTransition.FADE, duration=500, reverse_duration=250, switch_in_curve=flet.AnimationCurve.EASE_IN)
+        self.mother = flet.AnimatedSwitcher(
+            expand=True,
+            content=flet.Text(""),
+            transition=flet.AnimatedSwitcherTransition.FADE,
+            duration=500,
+            reverse_duration=250,
+            switch_in_curve=flet.AnimationCurve.EASE_IN
+        )
         page.add(self.mother)
-        
+
         time.sleep(0.3)
-        #? Run the first page.
+        # Run the first page.
         self.page_one()
-    
-    def page_one (self):
+
+    def page_one(self):
         page = self.page
         mother = self.mother
         main_column = flet.Column()
         mother.content = main_column
 
         main_column.controls.append(flet.Text("\n\n"))
 
-        Title1 = flet.Text("\n        Let's imagine 😃,\n        What if there is a ...", color="white", size=36, weight="bold")
-        main_column.controls.append(Title1)
+        title_1 = flet.Text(
+            "\n        Let's imagine 😃,\n        What if there is a ...",
+            color=flet.colors.WHITE,
+            size=36,
+            weight=flet.FontWeight.BOLD
+        )
+        describe = flet.Text(
+            "                  Everything start from the imagine skill.\n                  With Flet_StoryBoard you will make the impossible ✨.\n",
+            color=flet.colors.WHITE60,
+            size=15
+        )
+        next_button = flet.Container(
+            flet.Row(
+                [flet.Text("Start", color=flet.colors.BLACK)],
+                alignment=flet.MainAxisAlignment.CENTER
+            ),
+            bgcolor=flet.colors.WHITE,
+            width=100,
+            height=35,
+            border_radius=11,
+            on_click=self.page_two
+        )
 
-        describe = flet.Text("                  Everything start from the imagine skill.\n                  With Flet_StoryBoard you will make the impossible ✨.\n",
-        color=flet.colors.WHITE60, size=15)
+        main_column.controls.append(title_1)
         main_column.controls.append(describe)
-
-        next_button = flet.Container(flet.Row([flet.Text("Start", color="black")], alignment="center"), 
-        bgcolor="white", width=100, height=35, border_radius=11, on_click=self.page_two)
-        main_column.controls.append(flet.Column([flet.Row([next_button], alignment="END")], alignment="END", expand=True))
+        main_column.controls.append(
+            flet.Column(
+                [
+                    flet.Row(
+                        [next_button],
+                        alignment=flet.MainAxisAlignment.END
+                    )
+                ],
+                alignment=flet.MainAxisAlignment.END,
+                expand=True
+            )
+        )
 
         page.update()
-    
-    def page_two (self, *args):
-        def on_type (event):
+
+    def page_two(self, *args):
+        def on_type(event):
             if event.control.value == "":
                 next_button.tooltip = "You must pick a name."
                 next_button.disabled = True
                 next_button.update()
             else:
                 next_button.tooltip = "Click to generate the file."
                 next_button.disabled = False
                 page.title = "Flet StoryBoard - " + str(event.control.value)
                 if os.path.isfile(f"{page.title}.fletsb"):
                     page.title = page.title + " | Warning: File name exist"
                 page.update()
                 self.file_name = str(event.control.value)
-        
+
         page = self.page
         mother = self.mother
         main_column = flet.Column()
         mother.content = main_column
 
         main_column.controls.append(flet.Text("\n\n"))
 
-        Title1 = flet.Text("\n        Hey sir 🎩,\n        What is the name ?", color="white", size=36, weight="bold")
+        Title1 = flet.Text("\n        Hey sir 🎩,\n        What is the name ?", color=flet.colors.WHITE, size=36, weight="bold")
         main_column.controls.append(Title1)
 
-        describe = flet.Text("                  Lets choose a name of our UI.\n                  This name is the same as StoryBoad file name!.\n",
-        color=flet.colors.WHITE60, size=15)
+        describe = flet.Text(
+            "                  Lets choose a name of our UI.\n                  This name is the same as StoryBoad file name!.\n",
+            color=flet.colors.WHITE60, size=15)
         main_column.controls.append(describe)
 
-        StoryBoard_Name = flet.TextField(label="UI name", border_color="black", cursor_color="black", 
-        bgcolor="white", border_radius=19, width=350, height=60, on_change=on_type, color="black", on_submit=self.page_three)
+        StoryBoard_Name = flet.TextField(label="UI name", border_color=flet.colors.BLACK, cursor_color=flet.colors.BLACK,
+                                         bgcolor=flet.colors.WHITE, border_radius=19, width=350, height=60, on_change=on_type,
+                                         color=flet.colors.BLACK, on_submit=self.page_three)
         main_column.controls.append(flet.Row([StoryBoard_Name], alignment="center"))
 
-        next_button = flet.Container(flet.Row([flet.Text("Generate", color="black")], alignment="center"), 
-        bgcolor="white", width=100, height=35, border_radius=11, on_click=self.page_three, disabled=True)
-        main_column.controls.append(flet.Column([flet.Row([next_button], alignment="END")], alignment="END", expand=True))
+        next_button = flet.Container(flet.Row([flet.Text("Generate", color=flet.colors.BLACK)], alignment="center"),
+                                     bgcolor=flet.colors.WHITE, width=100, height=35, border_radius=11, on_click=self.page_three,
+                                     disabled=True)
+        main_column.controls.append(
+            flet.Column([flet.Row([next_button], alignment="END")], alignment="END", expand=True))
 
         mother.update()
         page.update()
-    
-    def page_three (self, *args):
+
+    def page_three(self, *args):
         page = self.page
         page.title = page.title
         mother = self.mother
         main_column = flet.Column()
         mother.content = main_column
 
         main_column.controls.append(flet.Text("\n\n"))
 
-        Title1 = flet.Text("\n        Now🪄,\n        Just choose a template!!", color="white", size=36, weight="bold")
+        Title1 = flet.Text("\n        Now🪄,\n        Just choose a template!!", color=flet.colors.WHITE, size=36, weight="bold")
         main_column.controls.append(Title1)
 
-        describe = flet.Text("                  Ok, what is a template ?.\n                  A template is a theme and pre-set page that make it quick to start.\n",
-        color=flet.colors.WHITE60, size=15)
+        describe = flet.Text(
+            "                  Ok, what is a template ?.\n                  A template is a theme and pre-set page that make it quick to start.\n",
+            color=flet.colors.WHITE60, size=15)
         main_column.controls.append(describe)
 
         r = flet.Row([
             self.make_a_template_button(flet.colors.WHITE24, "Blank new - default", "ADD_ROUNDED"),
             self.make_a_template_button(flet.colors.WHITE24, "Import template - soon", "GET_APP_OUTLINED", disable=True)
         ], alignment="center", spacing=15)
         main_column.controls.append(r)
 
         mother.update()
         page.update()
-    
 
-    def page_four (self, *args):
+    def page_four(self, *args):
         page = self.page
         page.title = page.title
         mother = self.mother
         main_column = flet.Column()
         mother.content = main_column
 
         main_column.controls.append(flet.Text("\n\n"))
 
-        Title1 = flet.Text("\n        Wait😄,\n        Building things for you.", color="white", size=36, weight="bold")
+        Title1 = flet.Text("\n        Wait😄,\n        Building things for you.", color=flet.colors.WHITE, size=36, weight="bold")
         main_column.controls.append(Title1)
 
         mother.update()
         page.update()
         time.sleep(1)
         self.apply_suggestion_page()
-    
 
-    def apply_suggestion_page (self, *a):
+    def apply_suggestion_page(self, *a):
         def dont_apply(e):
             Create_StoryBoard(self.file_name, "default", False)
             self.manage_class.file_name = self.file_name
             self.page.window_close()
-        def apply_it (e):
+
+        def apply_it(e):
             self.final_page_with_storyboard_suggest()
 
         page = self.page
         page.vertical_alignment = flet.MainAxisAlignment.CENTER
         page.title = page.title
         mother = self.mother
         main_column = flet.Column()
         mother.content = main_column
         col = main_column
 
         col.controls.append(flet.Row([flet.Text("", height=15)], alignment="center"))
 
-
-        image = flet.Image(src="https://raw.githubusercontent.com/SKbarbon/Flet_StoryBoard/main/assets/IMG_3260.PNG", width=250, height=250)
+        image = flet.Image(src="https://raw.githubusercontent.com/SKbarbon/Flet_StoryBoard/main/assets/IMG_3260.PNG",
+                           width=250, height=250)
         col.controls.append(flet.Row([image], alignment="center"))
 
-        title = flet.Text("Apply StoryBoard suggestions", size=20, weight="bold", color="white")
+        title = flet.Text("Apply StoryBoard suggestions", size=20, weight="bold", color=flet.colors.WHITE)
         col.controls.append(flet.Row([title], alignment="center"))
 
         describe = flet.Text("""
         These are suggestions based on smart rules that help 
         you build your interface by suggesting 
         widgets based on your goal.
-        """, size=13, color="white")
+        """, size=13, color=flet.colors.WHITE)
         col.controls.append(flet.Row([describe], alignment="center"))
 
-        apply_button = flet.ElevatedButton("Apply", bgcolor="white", color="black", width=250, on_click=apply_it)
+        apply_button = flet.ElevatedButton("Apply", bgcolor=flet.colors.WHITE, color=flet.colors.BLACK, width=250, on_click=apply_it)
         col.controls.append(flet.Row([apply_button], alignment="center"))
 
         no_btn = flet.TextButton(content=flet.Text("no thanks", color="red"), on_click=dont_apply)
         col.controls.append(flet.Row([no_btn], alignment="center"))
 
         mother.update()
         page.update()
 
-
-    def final_page_with_storyboard_suggest (self):
-        def apply_and_start (rule_name, rule_install_url):
+    def final_page_with_storyboard_suggest(self):
+        def apply_and_start(rule_name, rule_install_url):
             rules_file_content = requests.get(rule_install_url).text
             if not os.path.isdir("rules"):
                 os.mkdir("rules")
             open(f"rules/{rule_name}.json", "w+", encoding="utf-8").write(str(rules_file_content))
             Create_StoryBoard(self.file_name, "default", True, rule_name)
             self.manage_class.file_name = self.file_name
             self.page.window_close()
+
         # ------
         page = self.page
         page.title = page.title
         mother = self.mother
         main_column = flet.Column()
         mother.content = main_column
         col = main_column
         col.scroll = True
 
         main_column.controls.append(flet.Text("\n\n"))
 
-        Title1 = flet.Text("Choose your case.", color="white", size=36, weight="bold")
+        Title1 = flet.Text("Choose your case.", color=flet.colors.WHITE, size=36, weight="bold")
         main_column.controls.append(flet.Row([Title1], alignment="center"))
         mother.update()
         describe = flet.Text("""
 Choose your 'main' page goal from the 
 options down bellow. This will install the right suggestions rules
 for your main page case.
-        """, size=13, color="white")
+        """, size=13, color=flet.colors.WHITE)
         col.controls.append(flet.Row([describe], alignment="center"))
         mother.update()
 
-        
         all_rules = requests.get("https://raw.githubusercontent.com/SKbarbon/Flet_StoryBoard/main/rules/all.json").text
         all_rules = json.loads(all_rules)
-        
+
         for rule_option in all_rules["all_rules"]:
-            col.controls.append(self.make_a_rule_button_option(rule_option, all_rules["all_rules"][rule_option], apply_and_start))
+            col.controls.append(
+                self.make_a_rule_button_option(rule_option, all_rules["all_rules"][rule_option], apply_and_start))
 
         col.scroll = True
         mother.update()
 
-
-    
-
-    def make_a_template_button (self, bgcolor, name, icon, disable=False):
-        def on_hov (event):
+    def make_a_template_button(self, bgcolor, name, icon, disable=False):
+        def on_hov(event):
             if event.data == "true":
                 event.control.bgcolor = flet.colors.WHITE12
             elif event.data == "false":
                 event.control.bgcolor = flet.colors.WHITE24
                 event.control.update()
             event.control.update()
 
         cc = flet.Column(alignment="center", disabled=disable)
-        c = flet.Container(width=220, height=140, bgcolor=bgcolor, border_radius=10, on_click=self.page_four, on_hover=on_hov)
+        c = flet.Container(width=220, height=140, bgcolor=bgcolor, border_radius=10, on_click=self.page_four,
+                           on_hover=on_hov)
         cc.controls.append(c)
 
-        Icon = flet.Icon(icon, size=20, color="white")
+        Icon = flet.Icon(icon, size=20, color=flet.colors.WHITE)
         c.content = flet.Row([Icon], alignment="center")
-        
-        name_it = flet.Text(name, color="white", size=13, text_align="center")
+
+        name_it = flet.Text(name, color=flet.colors.WHITE, size=13, text_align="center")
         cc.controls.append(flet.Row([name_it], alignment="center"))
 
         return cc
 
-    def make_a_rule_button_option (self, name, url, on_click):
-        def on_choose (e):
+    def make_a_rule_button_option(self, name, url, on_click):
+        def on_choose(e):
             on_click(name, url)
-        b = flet.ElevatedButton(f"{name}", on_click=on_choose, bgcolor="white", color="blacK", width=150, height=45)
 
-        return flet.Row([b], alignment="center")
+        b = flet.ElevatedButton(f"{name}", on_click=on_choose, bgcolor=flet.colors.WHITE, color=flet.colors.BLACK, width=150, height=45)
+
+        return flet.Row([b], alignment="center")
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/pages/main_page.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/pages/main_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #! This is the editing page of a storyboard.
 from flet import Page, Row, Text
-from ..WIDGETS.All import all_widgets
+from ..widgets.All import all_widgets
 import flet
 import os
 import json
 import time
 import requests
 
 
 #* local imports
 from ..sections.left_section import leftSection
-from ..sections.preview_section import previewSection
+from ..sections.preview_section import PreviewSection
 from ..sections.edit_section import editSection
-from ..Engines.edit_widget_engine import editWidgetsEngine
-from ..Engines.edit_subwidgets_engin import editSubWidgetsEngine
-from ..Engines.suggesting_engine import SuggestingEngine
-from ..WIDGETS.All import all_widgets
+from ..engines.edit_widget_engine import EditWidgetsEngine
+from ..engines.edit_subwidgets_engine import EditSubWidgetsEngine
+from ..engines.suggesting_engine import SuggestingEngine
+from ..widgets.All import all_widgets
 from ..pages.settings import SettingsPage
 
 
 class mainPage:
     def __init__(self, file_path):
         if not os.path.isfile(file_path):
             raise FileExistsError(f"There is no Flet StoryBoard on path '{file_path}' .")
@@ -28,16 +28,16 @@
         self.current_page_name = "main"
         self.file_path = file_path
         self.development_mode = True
         self.dict_content = json.loads(open(file_path, encoding="utf-8").read())
 
         #? Copy of classes
         self.all_widgets = all_widgets
-        self._editWidgetsEngine = editWidgetsEngine
-        self._editSubWidgetsEngine = editSubWidgetsEngine
+        self._editWidgetsEngine = EditWidgetsEngine
+        self._editSubWidgetsEngine = EditSubWidgetsEngine
 
         #? Run the app
         flet.app(target=self.app)
 
     def app (self, page:Page):
         page.title = f"Flet StoryBoard - {self.file_path}"
         page.spacing = 0
@@ -54,15 +54,15 @@
 
         # The main row
         self.main_row = Row(scroll=False)
         page.add(self.main_row)
 
         #? append the sections
         self.left_section = leftSection(page, self, self.main_row)
-        self.preview_section = previewSection(page, self, self.main_row)
+        self.preview_section = PreviewSection(page, self, self.main_row)
         self.edit_section = editSection(page, self, self.main_row)
 
         #? Set finals of page.
         page.on_resize = self.on_page_resize
         page.on_keyboard_event = self.manage_keyboard_commands
 
 
@@ -174,15 +174,15 @@
         page.snack_bar.open = True
         page.update()
     
 
     def add_new_widget (self, widget_name, page_name=None):
         widget_number = len(self.dict_content["pages"][self.current_page_name]["widgets"])-1
         widget_class = all_widgets[widget_name]["class"]
-        widget_class = widget_class(self, self.preview_section.main_view_collumn, widget_number=widget_number)
+        widget_class = widget_class(self, self.preview_section.main_view_column, widget_number=widget_number)
         
         self.dict_content["pages"][self.current_page_name]["widgets"].append(widget_class.template)
         
         self.preview_section.update_preview(self.current_page_name)
         self.page.update()
 
         self.edit_a_widget(len(self.dict_content["pages"][self.current_page_name]["widgets"])-1)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/pages/settings.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/pages/settings.py`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/sections/edit_section.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/sections/edit_section.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from flet import Column, Page, Row
 import flet
 
-from ..Engines.edit_widget_engine import editWidgetsEngine
+from ..engines.edit_widget_engine import EditWidgetsEngine
 
 
 class editSection:
     def __init__(self, page:Page, main_class, main_row:Row) -> None:
         self.page : Page = page
         self.main_class = main_class
         self.main_row : Row = main_row
 
         self.main_column = Column(width=page.width/4, height=page.height,scroll=True)
 
         main_row.controls.append(self.main_column)
     
     def edit_widget_using_engine (self, widget_number):
-        ee = editWidgetsEngine(main_class=self.main_class, section_view=self.main_column, widget_number=widget_number)
+        ee = EditWidgetsEngine(main_class=self.main_class, section_view=self.main_column, widget_number=widget_number)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/sections/left_section.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/sections/left_section.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This is the left section part.
 from flet import Page, AnimatedSwitcher, Container, Row, Column
 import flet
 import time
 
-from ..WIDGETS.All import all_widgets
+from ..widgets.All import all_widgets
 from ..ui_toolkit.widget_browser_frame import Widget_Browse_Frame
 
 class leftSection:
     def __init__(self, page:Page, main_class, main_row:Row) -> None:
         self.page : Page = page
         self.main_class = main_class
         self.main_row = main_row
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py` & `Flet StoryBoard-1.3/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import flet
 
 
-
-
-def Widget_Browse_Frame (widget_name, widget_info_dict, on_click, page_name):
-    def action (event):
+def Widget_Browse_Frame(widget_name, widget_info_dict, on_click, page_name):
+    def action(event):
         on_click(widget_name, page_name)
 
-    def on_hover (event):
-        if event.data == "true":
-            event.control.bgcolor = "#474747"
-            event.control.update()
-        else:
-            event.control.bgcolor = "#5C5C5C"
-            event.control.update()
-
-    c = flet.Container(width=170, height=35, bgcolor="#5C5C5C", on_click=action, expand=True, on_hover=on_hover)
-    c.border_radius = 12
-
-    r = flet.Row([
-        flet.Text(" "),
-        flet.Icon(widget_info_dict["icon"], size=18, color="white"),
-        flet.Text(widget_name, size=13, color="white")
-    ], spacing=12)
-    c.content = r
+    def on_hover(event):
+        event.control.bgcolor = "#474747" if event.data == "true" else "#5C5C5C"
+        event.control.update()
+
+    r = flet.Row(
+        [
+            flet.Text(" "),
+            flet.Icon(widget_info_dict["icon"], size=18, color=flet.colors.WHITE),
+            flet.Text(widget_name, size=13, color=flet.colors.WHITE)
+        ],
+        spacing=12
+    )
+
+    c = flet.Container(
+        content=r,
+        width=170,
+        height=35,
+        bgcolor="#5C5C5C",
+        on_click=action,
+        expand=True,
+        on_hover=on_hover,
+        border_radius=12
+    )
 
-    return flet.Row([c], alignment="center")
+    return flet.Row([c], alignment=flet.MainAxisAlignment.CENTER)
```

### Comparing `Flet StoryBoard-1.2/Flet_StoryBoard.egg-info/SOURCES.txt` & `Flet StoryBoard-1.3/Flet_StoryBoard.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,50 +2,51 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 Flet_StoryBoard/__init__.py
 Flet_StoryBoard/edit.py
 Flet_StoryBoard/load_storyboard.py
+Flet_StoryBoard/pyodide.py
 Flet_StoryBoard.egg-info/PKG-INFO
 Flet_StoryBoard.egg-info/SOURCES.txt
 Flet_StoryBoard.egg-info/dependency_links.txt
 Flet_StoryBoard.egg-info/requires.txt
 Flet_StoryBoard.egg-info/top_level.txt
-Flet_StoryBoard/Engines/__init__.py
-Flet_StoryBoard/Engines/edit_subwidgets_engin.py
-Flet_StoryBoard/Engines/edit_widget_engine.py
-Flet_StoryBoard/Engines/suggesting_engine.py
-Flet_StoryBoard/Engines/viewer_engine.py
-Flet_StoryBoard/Tools/__init__.py
-Flet_StoryBoard/Tools/color_picker.py
-Flet_StoryBoard/Tools/create_storyboard.py
-Flet_StoryBoard/Tools/get_url_icon.py
-Flet_StoryBoard/Tools/list_picker.py
-Flet_StoryBoard/Tools/page_info.py
-Flet_StoryBoard/Tools/storyboard_class.py
-Flet_StoryBoard/WIDGETS/All.py
-Flet_StoryBoard/WIDGETS/__init__.py
-Flet_StoryBoard/WIDGETS/widgets/__init__.py
-Flet_StoryBoard/WIDGETS/widgets/button.py
-Flet_StoryBoard/WIDGETS/widgets/image.py
-Flet_StoryBoard/WIDGETS/widgets/label.py
-Flet_StoryBoard/WIDGETS/widgets/markdown.py
-Flet_StoryBoard/WIDGETS/widgets/navigator.py
-Flet_StoryBoard/WIDGETS/widgets/open_url.py
-Flet_StoryBoard/WIDGETS/widgets/padding.py
-Flet_StoryBoard/WIDGETS/widgets/paragraph.py
-Flet_StoryBoard/WIDGETS/widgets/row.py
-Flet_StoryBoard/WIDGETS/widgets/textfield.py
-Flet_StoryBoard/WIDGETS/widgets/title.py
+Flet_StoryBoard/engines/__init__.py
+Flet_StoryBoard/engines/edit_subwidgets_engine.py
+Flet_StoryBoard/engines/edit_widget_engine.py
+Flet_StoryBoard/engines/suggesting_engine.py
+Flet_StoryBoard/engines/viewer_engine.py
 Flet_StoryBoard/pages/__init__.py
 Flet_StoryBoard/pages/create_new_file.py
 Flet_StoryBoard/pages/main_page.py
 Flet_StoryBoard/pages/settings.py
 Flet_StoryBoard/pages/Settings/__init__.py
 Flet_StoryBoard/pages/Settings/pages.py
 Flet_StoryBoard/sections/__init__.py
 Flet_StoryBoard/sections/edit_section.py
 Flet_StoryBoard/sections/left_section.py
 Flet_StoryBoard/sections/preview_section.py
+Flet_StoryBoard/tools/__init__.py
+Flet_StoryBoard/tools/color_picker.py
+Flet_StoryBoard/tools/create_storyboard.py
+Flet_StoryBoard/tools/get_url_icon.py
+Flet_StoryBoard/tools/list_picker.py
+Flet_StoryBoard/tools/page_info.py
+Flet_StoryBoard/tools/storyboard_class.py
 Flet_StoryBoard/ui_toolkit/__init__.py
-Flet_StoryBoard/ui_toolkit/widget_browser_frame.py
+Flet_StoryBoard/ui_toolkit/widget_browser_frame.py
+Flet_StoryBoard/widgets/All.py
+Flet_StoryBoard/widgets/__init__.py
+Flet_StoryBoard/widgets/widgets/__init__.py
+Flet_StoryBoard/widgets/widgets/button.py
+Flet_StoryBoard/widgets/widgets/image.py
+Flet_StoryBoard/widgets/widgets/label.py
+Flet_StoryBoard/widgets/widgets/markdown.py
+Flet_StoryBoard/widgets/widgets/navigator.py
+Flet_StoryBoard/widgets/widgets/open_url.py
+Flet_StoryBoard/widgets/widgets/padding.py
+Flet_StoryBoard/widgets/widgets/paragraph.py
+Flet_StoryBoard/widgets/widgets/row.py
+Flet_StoryBoard/widgets/widgets/textfield.py
+Flet_StoryBoard/widgets/widgets/title.py
```

### Comparing `Flet StoryBoard-1.2/LICENSE` & `Flet StoryBoard-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Flet StoryBoard-1.2/README.md` & `Flet StoryBoard-1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,50 +2,51 @@
 Flet StoryBoard is a python library that have an easy to use tools for building graphical interfaces based on python `flet` library. Powerful interfaces with simple usability.
 You can use these tools with only two main and simple functions!
 
 ## Goal 🏁
 My goal is to allow programmers to focus on the back-end, and build the front-end using just a simple easy-to-use window without any front-end coding require.
 
 ## installation ⬇️
+- Python > 3.7
+
 For install:
 > `pip install Flet-StoryBoard`
 
 for Upgrade:
 > `pip install Flet-StoryBoard --upgrade`
 
-if there was anything wrong, and its not upgrading properly, you should uninstall this package and reinstall it:
+if there was anything wrong, and it's not upgrading properly, you should uninstall this package and reinstall it:
 > `pip uninstall Flet_StoryBoard` To uninstall
 
-## requirements ❗️
-- `flet` python library - it will auto install it if you dont have it-.
-- `requests` python library - it will auto install it if you dont have it-.
-- up than python3.7
+## Little Peek
+
+<img width="1500" alt="Screenshot 2023-04-26 at 12 17 33 PM" src="https://user-images.githubusercontent.com/86029286/234530619-004e0eca-d2b3-47ad-94fe-37ef5ae0fa68.png">
 
-## whats new on `Flet_StoryBoard` `1.0` 🎉
+## What's new on `Flet_StoryBoard` `1.0` 🎉
 - ReSupport custom widgets with flet.
 - Multiple pages support.
 - New Suggestions
 - New way to load the StoryBoard on your app.
-- The ability of add external `flet` controls inside of the StoryBoard.
-- New Feature called `Smart suggestions`. It get your goal then suggest things based on it.
+- The ability to add external `flet` controls inside the StoryBoard.
+- New Feature called `Smart suggestions`. It gets your goal then suggest things based on it.
 - Support templates. A template is a file contain pre-set props for all StoryBoard's widgets, like fonts and default text color. - soon -
 - ReBuild the architecture of the library.
 * Please read the docs to know more about library usage. [docs page](https://github.com/SKbarbon/Flet_StoryBoard/wiki)
 * if there is any another issues not fixed yet, please create an issue here: [issues page](https://github.com/SKbarbon/Flet_StoryBoard/issues)
 
 
 ## usage & examples 🤝
 There is a very simple docs here about library usage.
 [docs page](https://github.com/SKbarbon/Flet_StoryBoard/wiki)
 
 ### create/edit your own StoryBoard
 ```cmd
 python3 -m Flet_StoryBoard.edit myUI.fletsb
 ```
-It will edit the exist one or create a new one if not.
+It will edit the existing one or create a new one if not.
 
 ### load a StoryBoard
 To load your StoryBoard on your app, you can do this example code:
 
 ```python
 from Flet_StoryBoard import LoadStoryBoard, StoryBoard
 
@@ -53,9 +54,9 @@
     pass
 
 LoadStoryBoard(target_function=main, storyboard_file_path="myUI.fletsb")
 ```
 
 To know more about the `StoryBoard` class, follow the [docs page](https://github.com/SKbarbon/Flet_StoryBoard/wiki) .
 
-## comming soon 🔜
-- add custom non-built-in `flet` widgets. like `ColorPicker` and `AudioPlayer` widgets.
+## Coming Soon 🔜
+- add custom non-built-in `flet` widgets. like `ColorPicker` and `AudioPlayer` widgets.
```

### Comparing `Flet StoryBoard-1.2/setup.py` & `Flet StoryBoard-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Flet StoryBoard',
-    version='1.2',
+    version='1.3',
     author='SKbarbon',
     description='A UI-Builder that helps programmers build the front-end without codding it.',
     long_description="https://github.com/SKbarbon/Flet_StoryBoard",
     url='https://github.com/SKbarbon/Flet-StoryBoard',
     install_requires=["flet==0.5.2", "requests"],
     packages=find_packages(),
     classifiers=[
```

