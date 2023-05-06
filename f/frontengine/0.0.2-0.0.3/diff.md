# Comparing `tmp/frontengine-0.0.2.tar.gz` & `tmp/frontengine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontengine-0.0.2.tar", last modified: Sat May  6 10:43:37 2023, max compression
+gzip compressed data, was "frontengine-0.0.3.tar", last modified: Sat May  6 11:03:25 2023, max compression
```

## Comparing `frontengine-0.0.2.tar` & `frontengine-0.0.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.517479 frontengine-0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1414 2023-05-06 10:43:37.517479 frontengine-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.446948 frontengine-0.0.2/frontengine/
--rw-rw-rw-   0        0        0        0 2023-05-06 09:57:23.000000 frontengine-0.0.2/frontengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.459863 frontengine-0.0.2/frontengine/show/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.461858 frontengine-0.0.2/frontengine/show/gif/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/gif/__init__.py
--rw-rw-rw-   0        0        0     1749 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/gif/paint_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.463853 frontengine-0.0.2/frontengine/show/image/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/image/__init__.py
--rw-rw-rw-   0        0        0     1318 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/image/paint_image.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.466845 frontengine-0.0.2/frontengine/show/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.2/frontengine/show/sound_player/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/sound_player/sound_effect.py
--rw-rw-rw-   0        0        0     1489 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/sound_player/sound_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.468839 frontengine-0.0.2/frontengine/show/text/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/text/__init__.py
--rw-rw-rw-   0        0        0     1310 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/text/draw_text.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.470833 frontengine-0.0.2/frontengine/show/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/show/video/__init__.py
--rw-rw-rw-   0        0        0     1729 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/video/video_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.472829 frontengine-0.0.2/frontengine/show/web/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/web/__init__.py
--rw-rw-rw-   0        0        0      666 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/web/webview.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.474823 frontengine-0.0.2/frontengine/ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.476595 frontengine-0.0.2/frontengine/ui/main/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.2/frontengine/ui/main/__init__.py
--rw-rw-rw-   0        0        0     2117 2023-05-06 09:57:23.000000 frontengine-0.0.2/frontengine/ui/main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.477592 frontengine-0.0.2/frontengine/ui/setting/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.479626 frontengine-0.0.2/frontengine/ui/setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/gif/__init__.py
--rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine-0.0.2/frontengine/ui/setting/gif/gif_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.481638 frontengine-0.0.2/frontengine/ui/setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/image/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine-0.0.2/frontengine/ui/setting/image/image_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.483575 frontengine-0.0.2/frontengine/ui/setting/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/sound_player/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine-0.0.2/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.485609 frontengine-0.0.2/frontengine/ui/setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/text/__init__.py
--rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine-0.0.2/frontengine/ui/setting/text/text_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.487565 frontengine-0.0.2/frontengine/ui/setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/video/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine-0.0.2/frontengine/ui/setting/video/video_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.489597 frontengine-0.0.2/frontengine/ui/setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/web/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine-0.0.2/frontengine/ui/setting/web/web_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.490557 frontengine-0.0.2/frontengine/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.492552 frontengine-0.0.2/frontengine/user_setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/gif/__init__.py
--rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine-0.0.2/frontengine/user_setting/gif/gif_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.494547 frontengine-0.0.2/frontengine/user_setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/image/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine-0.0.2/frontengine/user_setting/image/image_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.496542 frontengine-0.0.2/frontengine/user_setting/sound/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/sound/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine-0.0.2/frontengine/user_setting/sound/sound_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.498536 frontengine-0.0.2/frontengine/user_setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/text/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine-0.0.2/frontengine/user_setting/text/text_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.500522 frontengine-0.0.2/frontengine/user_setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/video/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine-0.0.2/frontengine/user_setting/video/video_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.502559 frontengine-0.0.2/frontengine/user_setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/web/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine-0.0.2/frontengine/user_setting/web/web_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.503517 frontengine-0.0.2/frontengine/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.506509 frontengine-0.0.2/frontengine/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.507506 frontengine-0.0.2/frontengine/utils/file/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.509500 frontengine-0.0.2/frontengine/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.511496 frontengine-0.0.2/frontengine/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.513491 frontengine-0.0.2/frontengine/utils/json/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.516490 frontengine-0.0.2/frontengine/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.458866 frontengine-0.0.2/frontengine.egg-info/
--rw-rw-rw-   0        0        0     1414 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2494 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1138 2023-05-06 10:43:24.000000 frontengine-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 10:43:37.518476 frontengine-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.555839 frontengine-0.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1414 2023-05-06 11:03:25.554841 frontengine-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.392276 frontengine-0.0.3/frontengine/
+-rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine-0.0.3/frontengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.431173 frontengine-0.0.3/frontengine/show/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.3/frontengine/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.435163 frontengine-0.0.3/frontengine/show/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.3/frontengine/show/gif/__init__.py
+-rw-rw-rw-   0        0        0     1749 2023-05-06 09:15:04.000000 frontengine-0.0.3/frontengine/show/gif/paint_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.440148 frontengine-0.0.3/frontengine/show/image/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.3/frontengine/show/image/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-05-06 09:15:04.000000 frontengine-0.0.3/frontengine/show/image/paint_image.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.448126 frontengine-0.0.3/frontengine/show/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.3/frontengine/show/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-05-06 09:15:04.000000 frontengine-0.0.3/frontengine/show/sound_player/sound_effect.py
+-rw-rw-rw-   0        0        0     1489 2023-05-06 09:15:04.000000 frontengine-0.0.3/frontengine/show/sound_player/sound_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.452121 frontengine-0.0.3/frontengine/show/text/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.3/frontengine/show/text/__init__.py
+-rw-rw-rw-   0        0        0     1310 2023-05-06 09:15:04.000000 frontengine-0.0.3/frontengine/show/text/draw_text.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.459097 frontengine-0.0.3/frontengine/show/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.3/frontengine/show/video/__init__.py
+-rw-rw-rw-   0        0        0     1729 2023-05-06 09:15:04.000000 frontengine-0.0.3/frontengine/show/video/video_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.462091 frontengine-0.0.3/frontengine/show/web/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.3/frontengine/show/web/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-05-06 09:15:04.000000 frontengine-0.0.3/frontengine/show/web/webview.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.464084 frontengine-0.0.3/frontengine/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.3/frontengine/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.467076 frontengine-0.0.3/frontengine/ui/main/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.3/frontengine/ui/main/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-05-06 09:57:23.000000 frontengine-0.0.3/frontengine/ui/main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.468073 frontengine-0.0.3/frontengine/ui/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/ui/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.473064 frontengine-0.0.3/frontengine/ui/setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/ui/setting/gif/__init__.py
+-rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine-0.0.3/frontengine/ui/setting/gif/gif_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.479048 frontengine-0.0.3/frontengine/ui/setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/ui/setting/image/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine-0.0.3/frontengine/ui/setting/image/image_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.483039 frontengine-0.0.3/frontengine/ui/setting/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/ui/setting/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine-0.0.3/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.488022 frontengine-0.0.3/frontengine/ui/setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/ui/setting/text/__init__.py
+-rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine-0.0.3/frontengine/ui/setting/text/text_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.492010 frontengine-0.0.3/frontengine/ui/setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/ui/setting/video/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine-0.0.3/frontengine/ui/setting/video/video_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.496998 frontengine-0.0.3/frontengine/ui/setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/ui/setting/web/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine-0.0.3/frontengine/ui/setting/web/web_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.500985 frontengine-0.0.3/frontengine/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.3/frontengine/user_setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.505972 frontengine-0.0.3/frontengine/user_setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.3/frontengine/user_setting/gif/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine-0.0.3/frontengine/user_setting/gif/gif_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.509962 frontengine-0.0.3/frontengine/user_setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.3/frontengine/user_setting/image/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine-0.0.3/frontengine/user_setting/image/image_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.513953 frontengine-0.0.3/frontengine/user_setting/sound/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.3/frontengine/user_setting/sound/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine-0.0.3/frontengine/user_setting/sound/sound_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.517940 frontengine-0.0.3/frontengine/user_setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.3/frontengine/user_setting/text/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine-0.0.3/frontengine/user_setting/text/text_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.526916 frontengine-0.0.3/frontengine/user_setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.3/frontengine/user_setting/video/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine-0.0.3/frontengine/user_setting/video/video_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.529908 frontengine-0.0.3/frontengine/user_setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.3/frontengine/user_setting/web/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine-0.0.3/frontengine/user_setting/web/web_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.532901 frontengine-0.0.3/frontengine/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.3/frontengine/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.537889 frontengine-0.0.3/frontengine/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.539881 frontengine-0.0.3/frontengine/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.542874 frontengine-0.0.3/frontengine/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.547861 frontengine-0.0.3/frontengine/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.550852 frontengine-0.0.3/frontengine/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.553844 frontengine-0.0.3/frontengine/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine-0.0.3/frontengine/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:03:25.429179 frontengine-0.0.3/frontengine.egg-info/
+-rw-rw-rw-   0        0        0     1414 2023-05-06 11:03:25.000000 frontengine-0.0.3/frontengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2494 2023-05-06 11:03:25.000000 frontengine-0.0.3/frontengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:03:25.000000 frontengine-0.0.3/frontengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 11:03:25.000000 frontengine-0.0.3/frontengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 11:03:25.000000 frontengine-0.0.3/frontengine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1138 2023-05-06 11:03:04.000000 frontengine-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:03:25.555839 frontengine-0.0.3/setup.cfg
```

### Comparing `frontengine-0.0.2/LICENSE` & `frontengine-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/PKG-INFO` & `frontengine-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine
-Version: 0.0.2
+Version: 0.0.3
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine-0.0.2/README.md` & `frontengine-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/show/gif/paint_gif.py` & `frontengine-0.0.3/frontengine/show/gif/paint_gif.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/show/image/paint_image.py` & `frontengine-0.0.3/frontengine/show/image/paint_image.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/show/sound_player/sound_effect.py` & `frontengine-0.0.3/frontengine/show/sound_player/sound_effect.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/show/sound_player/sound_player.py` & `frontengine-0.0.3/frontengine/show/sound_player/sound_player.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/show/text/draw_text.py` & `frontengine-0.0.3/frontengine/show/text/draw_text.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/show/video/video_player.py` & `frontengine-0.0.3/frontengine/show/video/video_player.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/show/web/webview.py` & `frontengine-0.0.3/frontengine/show/web/webview.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/ui/main/main_ui.py` & `frontengine-0.0.3/frontengine/ui/main/main_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/ui/setting/gif/gif_setting_ui.py` & `frontengine-0.0.3/frontengine/ui/setting/gif/gif_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/ui/setting/image/image_setting_ui.py` & `frontengine-0.0.3/frontengine/ui/setting/image/image_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/ui/setting/sound_player/sound_player_setting_ui.py` & `frontengine-0.0.3/frontengine/ui/setting/sound_player/sound_player_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/ui/setting/text/text_setting_ui.py` & `frontengine-0.0.3/frontengine/ui/setting/text/text_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/ui/setting/video/video_setting_ui.py` & `frontengine-0.0.3/frontengine/ui/setting/video/video_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/ui/setting/web/web_setting_ui.py` & `frontengine-0.0.3/frontengine/ui/setting/web/web_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/utils/file/open/open_file.py` & `frontengine-0.0.3/frontengine/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/utils/file/save/save_file.py` & `frontengine-0.0.3/frontengine/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/utils/json/json_file.py` & `frontengine-0.0.3/frontengine/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine/utils/json_format/json_process.py` & `frontengine-0.0.3/frontengine/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/frontengine.egg-info/PKG-INFO` & `frontengine-0.0.3/frontengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine
-Version: 0.0.2
+Version: 0.0.3
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine-0.0.2/frontengine.egg-info/SOURCES.txt` & `frontengine-0.0.3/frontengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.2/pyproject.toml` & `frontengine-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frontengine"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 dependencies = [
     "PySide6",
     "qt-material",
 ]
```

