# Comparing `tmp/frontengine-0.0.1.tar.gz` & `tmp/frontengine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontengine-0.0.1.tar", last modified: Sat May  6 07:15:00 2023, max compression
+gzip compressed data, was "frontengine-0.0.2.tar", last modified: Sat May  6 10:43:37 2023, max compression
```

## Comparing `frontengine-0.0.1.tar` & `frontengine-0.0.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.122466 frontengine-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      733 2023-05-06 07:15:00.120470 frontengine-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-05-06 07:14:06.000000 frontengine-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.936959 frontengine-0.0.1/frontengine/
--rw-rw-rw-   0        0        0      104 2023-05-06 07:06:43.000000 frontengine-0.0.1/frontengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.959898 frontengine-0.0.1/frontengine/show/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.1/frontengine/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.963887 frontengine-0.0.1/frontengine/show/gif/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.1/frontengine/show/gif/__init__.py
--rw-rw-rw-   0        0        0     1661 2023-05-06 05:08:59.000000 frontengine-0.0.1/frontengine/show/gif/paint_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.967876 frontengine-0.0.1/frontengine/show/image/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.1/frontengine/show/image/__init__.py
--rw-rw-rw-   0        0        0     1219 2023-05-05 19:19:14.000000 frontengine-0.0.1/frontengine/show/image/paint_image.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.975856 frontengine-0.0.1/frontengine/show/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.1/frontengine/show/sound_player/__init__.py
--rw-rw-rw-   0        0        0     1194 2023-05-06 06:44:24.000000 frontengine-0.0.1/frontengine/show/sound_player/sound_effect.py
--rw-rw-rw-   0        0        0     1401 2023-05-06 06:44:24.000000 frontengine-0.0.1/frontengine/show/sound_player/sound_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.980842 frontengine-0.0.1/frontengine/show/text/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.1/frontengine/show/text/__init__.py
--rw-rw-rw-   0        0        0     1183 2023-05-06 05:40:15.000000 frontengine-0.0.1/frontengine/show/text/draw_text.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.983834 frontengine-0.0.1/frontengine/show/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.1/frontengine/show/video/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-05-06 07:01:52.000000 frontengine-0.0.1/frontengine/show/video/video_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.988821 frontengine-0.0.1/frontengine/show/web/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.1/frontengine/show/web/__init__.py
--rw-rw-rw-   0        0        0      539 2023-05-06 05:48:20.000000 frontengine-0.0.1/frontengine/show/web/webview.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.992810 frontengine-0.0.1/frontengine/ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.1/frontengine/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.995802 frontengine-0.0.1/frontengine/ui/main/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.1/frontengine/ui/main/__init__.py
--rw-rw-rw-   0        0        0     2681 2023-05-06 07:07:56.000000 frontengine-0.0.1/frontengine/ui/main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.997797 frontengine-0.0.1/frontengine/ui/setting/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/ui/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.001786 frontengine-0.0.1/frontengine/ui/setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/ui/setting/gif/__init__.py
--rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine-0.0.1/frontengine/ui/setting/gif/gif_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.005775 frontengine-0.0.1/frontengine/ui/setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/ui/setting/image/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine-0.0.1/frontengine/ui/setting/image/image_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.018742 frontengine-0.0.1/frontengine/ui/setting/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/ui/setting/sound_player/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine-0.0.1/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.024723 frontengine-0.0.1/frontengine/ui/setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/ui/setting/text/__init__.py
--rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine-0.0.1/frontengine/ui/setting/text/text_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.029713 frontengine-0.0.1/frontengine/ui/setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/ui/setting/video/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine-0.0.1/frontengine/ui/setting/video/video_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.036692 frontengine-0.0.1/frontengine/ui/setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/ui/setting/web/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine-0.0.1/frontengine/ui/setting/web/web_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.041680 frontengine-0.0.1/frontengine/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.1/frontengine/user_setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.045668 frontengine-0.0.1/frontengine/user_setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.1/frontengine/user_setting/gif/__init__.py
--rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine-0.0.1/frontengine/user_setting/gif/gif_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.052650 frontengine-0.0.1/frontengine/user_setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.1/frontengine/user_setting/image/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine-0.0.1/frontengine/user_setting/image/image_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.057637 frontengine-0.0.1/frontengine/user_setting/sound/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.1/frontengine/user_setting/sound/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine-0.0.1/frontengine/user_setting/sound/sound_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.063623 frontengine-0.0.1/frontengine/user_setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.1/frontengine/user_setting/text/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine-0.0.1/frontengine/user_setting/text/text_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.071600 frontengine-0.0.1/frontengine/user_setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.1/frontengine/user_setting/video/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine-0.0.1/frontengine/user_setting/video/video_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.076586 frontengine-0.0.1/frontengine/user_setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.1/frontengine/user_setting/web/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine-0.0.1/frontengine/user_setting/web/web_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.078580 frontengine-0.0.1/frontengine/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.1/frontengine/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.089552 frontengine-0.0.1/frontengine/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.091547 frontengine-0.0.1/frontengine/utils/file/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.095534 frontengine-0.0.1/frontengine/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.104511 frontengine-0.0.1/frontengine/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.111492 frontengine-0.0.1/frontengine/utils/json/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:15:00.117476 frontengine-0.0.1/frontengine/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine-0.0.1/frontengine/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:14:59.957904 frontengine-0.0.1/frontengine.egg-info/
--rw-rw-rw-   0        0        0      733 2023-05-06 07:14:59.000000 frontengine-0.0.1/frontengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2494 2023-05-06 07:14:59.000000 frontengine-0.0.1/frontengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:14:59.000000 frontengine-0.0.1/frontengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 07:14:59.000000 frontengine-0.0.1/frontengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 07:14:59.000000 frontengine-0.0.1/frontengine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-05-06 07:12:09.000000 frontengine-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 07:15:00.122466 frontengine-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.517479 frontengine-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1414 2023-05-06 10:43:37.517479 frontengine-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.446948 frontengine-0.0.2/frontengine/
+-rw-rw-rw-   0        0        0        0 2023-05-06 09:57:23.000000 frontengine-0.0.2/frontengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.459863 frontengine-0.0.2/frontengine/show/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.461858 frontengine-0.0.2/frontengine/show/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/gif/__init__.py
+-rw-rw-rw-   0        0        0     1749 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/gif/paint_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.463853 frontengine-0.0.2/frontengine/show/image/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/image/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/image/paint_image.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.466845 frontengine-0.0.2/frontengine/show/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.2/frontengine/show/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/sound_player/sound_effect.py
+-rw-rw-rw-   0        0        0     1489 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/sound_player/sound_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.468839 frontengine-0.0.2/frontengine/show/text/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/text/__init__.py
+-rw-rw-rw-   0        0        0     1310 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/text/draw_text.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.470833 frontengine-0.0.2/frontengine/show/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/show/video/__init__.py
+-rw-rw-rw-   0        0        0     1729 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/video/video_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.472829 frontengine-0.0.2/frontengine/show/web/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/show/web/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-05-06 09:15:04.000000 frontengine-0.0.2/frontengine/show/web/webview.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.474823 frontengine-0.0.2/frontengine/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.476595 frontengine-0.0.2/frontengine/ui/main/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.2/frontengine/ui/main/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-05-06 09:57:23.000000 frontengine-0.0.2/frontengine/ui/main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.477592 frontengine-0.0.2/frontengine/ui/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.479626 frontengine-0.0.2/frontengine/ui/setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/gif/__init__.py
+-rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine-0.0.2/frontengine/ui/setting/gif/gif_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.481638 frontengine-0.0.2/frontengine/ui/setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/image/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine-0.0.2/frontengine/ui/setting/image/image_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.483575 frontengine-0.0.2/frontengine/ui/setting/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine-0.0.2/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.485609 frontengine-0.0.2/frontengine/ui/setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/text/__init__.py
+-rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine-0.0.2/frontengine/ui/setting/text/text_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.487565 frontengine-0.0.2/frontengine/ui/setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/video/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine-0.0.2/frontengine/ui/setting/video/video_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.489597 frontengine-0.0.2/frontengine/ui/setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/ui/setting/web/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine-0.0.2/frontengine/ui/setting/web/web_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.490557 frontengine-0.0.2/frontengine/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.492552 frontengine-0.0.2/frontengine/user_setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/gif/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine-0.0.2/frontengine/user_setting/gif/gif_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.494547 frontengine-0.0.2/frontengine/user_setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/image/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine-0.0.2/frontengine/user_setting/image/image_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.496542 frontengine-0.0.2/frontengine/user_setting/sound/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/sound/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine-0.0.2/frontengine/user_setting/sound/sound_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.498536 frontengine-0.0.2/frontengine/user_setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/text/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine-0.0.2/frontengine/user_setting/text/text_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.500522 frontengine-0.0.2/frontengine/user_setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/video/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine-0.0.2/frontengine/user_setting/video/video_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.502559 frontengine-0.0.2/frontengine/user_setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.2/frontengine/user_setting/web/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine-0.0.2/frontengine/user_setting/web/web_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.503517 frontengine-0.0.2/frontengine/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.2/frontengine/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.506509 frontengine-0.0.2/frontengine/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.507506 frontengine-0.0.2/frontengine/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.509500 frontengine-0.0.2/frontengine/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.511496 frontengine-0.0.2/frontengine/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.513491 frontengine-0.0.2/frontengine/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.516490 frontengine-0.0.2/frontengine/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine-0.0.2/frontengine/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:43:37.458866 frontengine-0.0.2/frontengine.egg-info/
+-rw-rw-rw-   0        0        0     1414 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2494 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 10:43:37.000000 frontengine-0.0.2/frontengine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1138 2023-05-06 10:43:24.000000 frontengine-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 10:43:37.518476 frontengine-0.0.2/setup.cfg
```

### Comparing `frontengine-0.0.1/LICENSE` & `frontengine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/show/gif/paint_gif.py` & `frontengine-0.0.2/frontengine/show/gif/paint_gif.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
             self.movie.start()
         else:
             message_box = QMessageBox(self)
             message_box.setText("GIF or WEBP error")
             message_box.show()
         # Window setting
         self.setWindowTitle("GIF AND WEBP")
+        # Set Icon
+        self.icon_path = Path(os.getcwd() + "/je_driver_icon.ico")
 
     def paintEvent(self, event) -> None:
         current_gif_frame = self.movie.currentPixmap()
         painter = QPainter(self)
         painter.setOpacity(self.opacity)
         painter.drawPixmap(
             QRect(
```

### Comparing `frontengine-0.0.1/frontengine/show/image/paint_image.py` & `frontengine-0.0.2/frontengine/show/image/paint_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from pathlib import Path
 
 from PySide6.QtCore import Qt, QRect
 from PySide6.QtGui import QPainter, QImage
 from PySide6.QtWidgets import QWidget, QMessageBox
 
 
@@ -21,14 +22,16 @@
             message_box = QMessageBox(self)
             message_box.setText("Image Error")
             message_box.show()
         self.opacity = opacity
         self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
         # Window setting
         self.setWindowTitle("Image")
+        # Set Icon
+        self.icon_path = Path(os.getcwd() + "/je_driver_icon.ico")
 
     def paintEvent(self, event) -> None:
         painter = QPainter(self)
         painter.setOpacity(self.opacity)
         painter.drawImage(
             QRect(self.x(), self.y(), self.width(), self.height()),
             self.image)
```

### Comparing `frontengine-0.0.1/frontengine/show/sound_player/sound_effect.py` & `frontengine-0.0.2/frontengine/show/sound_player/sound_effect.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,12 +24,14 @@
             self.sound_player.play()
         else:
             message_box = QMessageBox(self)
             message_box.setText("Sound file error")
             message_box.show()
         # Window setting
         self.setWindowTitle("Sound Wave")
+        # Set Icon
+        self.icon_path = Path(os.getcwd() + "/je_driver_icon.ico")
 
     def close(self):
         super().close()
         self.sound_player.stop()
```

### Comparing `frontengine-0.0.1/frontengine/show/sound_player/sound_player.py` & `frontengine-0.0.2/frontengine/show/sound_player/sound_player.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,11 +27,13 @@
             self.media_player.play()
         else:
             message_box = QMessageBox(self)
             message_box.setText("Sound file error")
             message_box.show()
         # Window setting
         self.setWindowTitle("Sound")
+        # Set Icon
+        self.icon_path = Path(os.getcwd() + "/je_driver_icon.ico")
 
     def close(self):
         super().close()
         self.media_player.stop()
```

### Comparing `frontengine-0.0.1/frontengine/show/text/draw_text.py` & `frontengine-0.0.2/frontengine/show/text/draw_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+from pathlib import Path
+
 from PySide6.QtCore import Qt, QRect
 from PySide6.QtGui import QPainter, QFontDatabase
 from PySide6.QtWidgets import QWidget
 
 
 class TextWidget(QWidget):
 
@@ -14,14 +17,16 @@
         )
         self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
         self.text = text
         self.font_size = font_size
         self.opacity = opacity
         self.draw_font = QFontDatabase.font(self.font().family(), "", self.font_size)
         self.setWindowTitle("Text")
+        # Set Icon
+        self.icon_path = Path(os.getcwd() + "/je_driver_icon.ico")
 
     def paintEvent(self, event) -> None:
         painter = QPainter(self)
         painter.setFont(
             self.draw_font
         )
         painter.setPen(Qt.GlobalColor.black)
```

### Comparing `frontengine-0.0.1/frontengine/show/video/video_player.py` & `frontengine-0.0.2/frontengine/show/video/video_player.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from pathlib import Path
 
 from PySide6.QtCore import Qt, QUrl
 from PySide6.QtMultimedia import QMediaPlayer, QAudioOutput
 from PySide6.QtMultimediaWidgets import QVideoWidget
 from PySide6.QtWidgets import QMessageBox
 
@@ -33,10 +34,12 @@
             self.media_player.audioOutput().setVolume(volume)
             self.media_player.play()
         else:
             message_box = QMessageBox(self)
             message_box.setText("Video error")
             message_box.show()
         self.setWindowTitle("Video")
+        # Set Icon
+        self.icon_path = Path(os.getcwd() + "/je_driver_icon.ico")
 
     def closeEvent(self, event):
         self.media_player.stop()
```

### Comparing `frontengine-0.0.1/frontengine/ui/setting/gif/gif_setting_ui.py` & `frontengine-0.0.2/frontengine/ui/setting/gif/gif_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/ui/setting/image/image_setting_ui.py` & `frontengine-0.0.2/frontengine/ui/setting/image/image_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/ui/setting/sound_player/sound_player_setting_ui.py` & `frontengine-0.0.2/frontengine/ui/setting/sound_player/sound_player_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/ui/setting/text/text_setting_ui.py` & `frontengine-0.0.2/frontengine/ui/setting/text/text_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/ui/setting/video/video_setting_ui.py` & `frontengine-0.0.2/frontengine/ui/setting/video/video_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/ui/setting/web/web_setting_ui.py` & `frontengine-0.0.2/frontengine/ui/setting/web/web_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/utils/file/open/open_file.py` & `frontengine-0.0.2/frontengine/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/utils/file/save/save_file.py` & `frontengine-0.0.2/frontengine/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/utils/json/json_file.py` & `frontengine-0.0.2/frontengine/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine/utils/json_format/json_process.py` & `frontengine-0.0.2/frontengine/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/frontengine.egg-info/SOURCES.txt` & `frontengine-0.0.2/frontengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.1/pyproject.toml` & `frontengine-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frontengine"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 dependencies = [
     "PySide6",
     "qt-material",
 ]
-description = ""
+description = "FrontEngine is a tool allow you set Video or Image or GIF front of all window"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Win32 (MS Windows)",
     "Environment :: MacOS X",
```

