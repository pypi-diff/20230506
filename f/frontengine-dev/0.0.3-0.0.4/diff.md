# Comparing `tmp/frontengine_dev-0.0.3.tar.gz` & `tmp/frontengine_dev-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontengine_dev-0.0.3.tar", last modified: Sat May  6 11:04:55 2023, max compression
+gzip compressed data, was "frontengine_dev-0.0.4.tar", last modified: Sat May  6 11:28:12 2023, max compression
```

## Comparing `frontengine_dev-0.0.3.tar` & `frontengine_dev-0.0.4.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.575431 frontengine_dev-0.0.3/
--rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine_dev-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1418 2023-05-06 11:04:55.573437 frontengine_dev-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine_dev-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.311139 frontengine_dev-0.0.3/frontengine/
--rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine_dev-0.0.3/frontengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.313133 frontengine_dev-0.0.3/frontengine/show/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.3/frontengine/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.316125 frontengine_dev-0.0.3/frontengine/show/gif/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.3/frontengine/show/gif/__init__.py
--rw-rw-rw-   0        0        0     1749 2023-05-06 09:15:04.000000 frontengine_dev-0.0.3/frontengine/show/gif/paint_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.321111 frontengine_dev-0.0.3/frontengine/show/image/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.3/frontengine/show/image/__init__.py
--rw-rw-rw-   0        0        0     1318 2023-05-06 09:15:04.000000 frontengine_dev-0.0.3/frontengine/show/image/paint_image.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.329091 frontengine_dev-0.0.3/frontengine/show/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.3/frontengine/show/sound_player/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-05-06 09:15:04.000000 frontengine_dev-0.0.3/frontengine/show/sound_player/sound_effect.py
--rw-rw-rw-   0        0        0     1489 2023-05-06 09:15:04.000000 frontengine_dev-0.0.3/frontengine/show/sound_player/sound_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.338065 frontengine_dev-0.0.3/frontengine/show/text/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.3/frontengine/show/text/__init__.py
--rw-rw-rw-   0        0        0     1310 2023-05-06 09:15:04.000000 frontengine_dev-0.0.3/frontengine/show/text/draw_text.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.345048 frontengine_dev-0.0.3/frontengine/show/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.3/frontengine/show/video/__init__.py
--rw-rw-rw-   0        0        0     1729 2023-05-06 09:15:04.000000 frontengine_dev-0.0.3/frontengine/show/video/video_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.349037 frontengine_dev-0.0.3/frontengine/show/web/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.3/frontengine/show/web/__init__.py
--rw-rw-rw-   0        0        0      666 2023-05-06 09:15:04.000000 frontengine_dev-0.0.3/frontengine/show/web/webview.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.353027 frontengine_dev-0.0.3/frontengine/ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.3/frontengine/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.359010 frontengine_dev-0.0.3/frontengine/ui/main/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.3/frontengine/ui/main/__init__.py
--rw-rw-rw-   0        0        0     2117 2023-05-06 09:57:23.000000 frontengine_dev-0.0.3/frontengine/ui/main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.362999 frontengine_dev-0.0.3/frontengine/ui/setting/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/ui/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.365991 frontengine_dev-0.0.3/frontengine/ui/setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/ui/setting/gif/__init__.py
--rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine_dev-0.0.3/frontengine/ui/setting/gif/gif_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.369980 frontengine_dev-0.0.3/frontengine/ui/setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/ui/setting/image/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine_dev-0.0.3/frontengine/ui/setting/image/image_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.373971 frontengine_dev-0.0.3/frontengine/ui/setting/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/ui/setting/sound_player/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine_dev-0.0.3/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.378957 frontengine_dev-0.0.3/frontengine/ui/setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/ui/setting/text/__init__.py
--rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine_dev-0.0.3/frontengine/ui/setting/text/text_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.381950 frontengine_dev-0.0.3/frontengine/ui/setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/ui/setting/video/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine_dev-0.0.3/frontengine/ui/setting/video/video_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.389927 frontengine_dev-0.0.3/frontengine/ui/setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/ui/setting/web/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine_dev-0.0.3/frontengine/ui/setting/web/web_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.391921 frontengine_dev-0.0.3/frontengine/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.3/frontengine/user_setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.395912 frontengine_dev-0.0.3/frontengine/user_setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.3/frontengine/user_setting/gif/__init__.py
--rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine_dev-0.0.3/frontengine/user_setting/gif/gif_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.399900 frontengine_dev-0.0.3/frontengine/user_setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.3/frontengine/user_setting/image/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine_dev-0.0.3/frontengine/user_setting/image/image_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.404888 frontengine_dev-0.0.3/frontengine/user_setting/sound/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.3/frontengine/user_setting/sound/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine_dev-0.0.3/frontengine/user_setting/sound/sound_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.407880 frontengine_dev-0.0.3/frontengine/user_setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.3/frontengine/user_setting/text/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine_dev-0.0.3/frontengine/user_setting/text/text_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.413863 frontengine_dev-0.0.3/frontengine/user_setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.3/frontengine/user_setting/video/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine_dev-0.0.3/frontengine/user_setting/video/video_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.419848 frontengine_dev-0.0.3/frontengine/user_setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.3/frontengine/user_setting/web/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine_dev-0.0.3/frontengine/user_setting/web/web_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.423837 frontengine_dev-0.0.3/frontengine/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.3/frontengine/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.465724 frontengine_dev-0.0.3/frontengine/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.473703 frontengine_dev-0.0.3/frontengine/utils/file/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.480685 frontengine_dev-0.0.3/frontengine/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.490657 frontengine_dev-0.0.3/frontengine/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.494648 frontengine_dev-0.0.3/frontengine/utils/json/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.500632 frontengine_dev-0.0.3/frontengine/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine_dev-0.0.3/frontengine/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:04:55.570446 frontengine_dev-0.0.3/frontengine_dev.egg-info/
--rw-rw-rw-   0        0        0     1418 2023-05-06 11:04:55.000000 frontengine_dev-0.0.3/frontengine_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2514 2023-05-06 11:04:55.000000 frontengine_dev-0.0.3/frontengine_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:04:55.000000 frontengine_dev-0.0.3/frontengine_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 11:04:55.000000 frontengine_dev-0.0.3/frontengine_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 11:04:55.000000 frontengine_dev-0.0.3/frontengine_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1142 2023-05-06 11:04:36.000000 frontengine_dev-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 11:04:55.576429 frontengine_dev-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.166468 frontengine_dev-0.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine_dev-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1418 2023-05-06 11:28:12.164473 frontengine_dev-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine_dev-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.841337 frontengine_dev-0.0.4/frontengine/
+-rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine_dev-0.0.4/frontengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.845328 frontengine_dev-0.0.4/frontengine/show/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.4/frontengine/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.849316 frontengine_dev-0.0.4/frontengine/show/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.4/frontengine/show/gif/__init__.py
+-rw-rw-rw-   0        0        0     1749 2023-05-06 09:15:04.000000 frontengine_dev-0.0.4/frontengine/show/gif/paint_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.853305 frontengine_dev-0.0.4/frontengine/show/image/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.4/frontengine/show/image/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-05-06 09:15:04.000000 frontengine_dev-0.0.4/frontengine/show/image/paint_image.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.863279 frontengine_dev-0.0.4/frontengine/show/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.4/frontengine/show/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-05-06 09:15:04.000000 frontengine_dev-0.0.4/frontengine/show/sound_player/sound_effect.py
+-rw-rw-rw-   0        0        0     1489 2023-05-06 09:15:04.000000 frontengine_dev-0.0.4/frontengine/show/sound_player/sound_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.870260 frontengine_dev-0.0.4/frontengine/show/text/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.4/frontengine/show/text/__init__.py
+-rw-rw-rw-   0        0        0     1310 2023-05-06 09:15:04.000000 frontengine_dev-0.0.4/frontengine/show/text/draw_text.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.875247 frontengine_dev-0.0.4/frontengine/show/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.4/frontengine/show/video/__init__.py
+-rw-rw-rw-   0        0        0     1729 2023-05-06 09:15:04.000000 frontengine_dev-0.0.4/frontengine/show/video/video_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.881231 frontengine_dev-0.0.4/frontengine/show/web/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.4/frontengine/show/web/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-05-06 09:15:04.000000 frontengine_dev-0.0.4/frontengine/show/web/webview.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.883226 frontengine_dev-0.0.4/frontengine/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.4/frontengine/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.888212 frontengine_dev-0.0.4/frontengine/ui/main/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.4/frontengine/ui/main/__init__.py
+-rw-rw-rw-   0        0        0     2093 2023-05-06 11:27:46.000000 frontengine_dev-0.0.4/frontengine/ui/main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.891204 frontengine_dev-0.0.4/frontengine/ui/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/ui/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.895194 frontengine_dev-0.0.4/frontengine/ui/setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/ui/setting/gif/__init__.py
+-rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine_dev-0.0.4/frontengine/ui/setting/gif/gif_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.900179 frontengine_dev-0.0.4/frontengine/ui/setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/ui/setting/image/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine_dev-0.0.4/frontengine/ui/setting/image/image_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.908160 frontengine_dev-0.0.4/frontengine/ui/setting/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/ui/setting/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine_dev-0.0.4/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:11.972985 frontengine_dev-0.0.4/frontengine/ui/setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/ui/setting/text/__init__.py
+-rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine_dev-0.0.4/frontengine/ui/setting/text/text_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.032829 frontengine_dev-0.0.4/frontengine/ui/setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/ui/setting/video/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine_dev-0.0.4/frontengine/ui/setting/video/video_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.040804 frontengine_dev-0.0.4/frontengine/ui/setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/ui/setting/web/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine_dev-0.0.4/frontengine/ui/setting/web/web_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.043797 frontengine_dev-0.0.4/frontengine/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.4/frontengine/user_setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.050777 frontengine_dev-0.0.4/frontengine/user_setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.4/frontengine/user_setting/gif/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine_dev-0.0.4/frontengine/user_setting/gif/gif_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.073716 frontengine_dev-0.0.4/frontengine/user_setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.4/frontengine/user_setting/image/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine_dev-0.0.4/frontengine/user_setting/image/image_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.078705 frontengine_dev-0.0.4/frontengine/user_setting/sound/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.4/frontengine/user_setting/sound/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine_dev-0.0.4/frontengine/user_setting/sound/sound_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.082692 frontengine_dev-0.0.4/frontengine/user_setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.4/frontengine/user_setting/text/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine_dev-0.0.4/frontengine/user_setting/text/text_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.087678 frontengine_dev-0.0.4/frontengine/user_setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.4/frontengine/user_setting/video/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine_dev-0.0.4/frontengine/user_setting/video/video_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.091668 frontengine_dev-0.0.4/frontengine/user_setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.4/frontengine/user_setting/web/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine_dev-0.0.4/frontengine/user_setting/web/web_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.094660 frontengine_dev-0.0.4/frontengine/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.4/frontengine/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.105632 frontengine_dev-0.0.4/frontengine/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.107625 frontengine_dev-0.0.4/frontengine/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.111615 frontengine_dev-0.0.4/frontengine/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.118597 frontengine_dev-0.0.4/frontengine/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.123583 frontengine_dev-0.0.4/frontengine/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.128569 frontengine_dev-0.0.4/frontengine/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine_dev-0.0.4/frontengine/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:28:12.162479 frontengine_dev-0.0.4/frontengine_dev.egg-info/
+-rw-rw-rw-   0        0        0     1418 2023-05-06 11:28:11.000000 frontengine_dev-0.0.4/frontengine_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2514 2023-05-06 11:28:11.000000 frontengine_dev-0.0.4/frontengine_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:28:11.000000 frontengine_dev-0.0.4/frontengine_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 11:28:11.000000 frontengine_dev-0.0.4/frontengine_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 11:28:11.000000 frontengine_dev-0.0.4/frontengine_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1142 2023-05-06 11:27:46.000000 frontengine_dev-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:28:12.166468 frontengine_dev-0.0.4/setup.cfg
```

### Comparing `frontengine_dev-0.0.3/LICENSE` & `frontengine_dev-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/PKG-INFO` & `frontengine_dev-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine_dev
-Version: 0.0.3
+Version: 0.0.4
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine_dev-0.0.3/README.md` & `frontengine_dev-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/show/gif/paint_gif.py` & `frontengine_dev-0.0.4/frontengine/show/gif/paint_gif.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/show/image/paint_image.py` & `frontengine_dev-0.0.4/frontengine/show/image/paint_image.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/show/sound_player/sound_effect.py` & `frontengine_dev-0.0.4/frontengine/show/sound_player/sound_effect.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/show/sound_player/sound_player.py` & `frontengine_dev-0.0.4/frontengine/show/sound_player/sound_player.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/show/text/draw_text.py` & `frontengine_dev-0.0.4/frontengine/show/text/draw_text.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/show/video/video_player.py` & `frontengine_dev-0.0.4/frontengine/show/video/video_player.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/show/web/webview.py` & `frontengine_dev-0.0.4/frontengine/show/web/webview.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/ui/main/main_ui.py` & `frontengine_dev-0.0.4/frontengine/ui/main/main_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,9 +45,7 @@
 def start_front_engine():
     new_editor = QApplication(sys.argv)
     window = FrontEngineMainUI()
     apply_stylesheet(new_editor, theme='dark_amber.xml')
     window.showMaximized()
     sys.exit(new_editor.exec())
 
-
-start_front_engine()
```

### Comparing `frontengine_dev-0.0.3/frontengine/ui/setting/gif/gif_setting_ui.py` & `frontengine_dev-0.0.4/frontengine/ui/setting/gif/gif_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/ui/setting/image/image_setting_ui.py` & `frontengine_dev-0.0.4/frontengine/ui/setting/image/image_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/ui/setting/sound_player/sound_player_setting_ui.py` & `frontengine_dev-0.0.4/frontengine/ui/setting/sound_player/sound_player_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/ui/setting/text/text_setting_ui.py` & `frontengine_dev-0.0.4/frontengine/ui/setting/text/text_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/ui/setting/video/video_setting_ui.py` & `frontengine_dev-0.0.4/frontengine/ui/setting/video/video_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/ui/setting/web/web_setting_ui.py` & `frontengine_dev-0.0.4/frontengine/ui/setting/web/web_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/utils/file/open/open_file.py` & `frontengine_dev-0.0.4/frontengine/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/utils/file/save/save_file.py` & `frontengine_dev-0.0.4/frontengine/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/utils/json/json_file.py` & `frontengine_dev-0.0.4/frontengine/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine/utils/json_format/json_process.py` & `frontengine_dev-0.0.4/frontengine/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/frontengine_dev.egg-info/PKG-INFO` & `frontengine_dev-0.0.4/frontengine_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine-dev
-Version: 0.0.3
+Version: 0.0.4
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine_dev-0.0.3/frontengine_dev.egg-info/SOURCES.txt` & `frontengine_dev-0.0.4/frontengine_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.3/pyproject.toml` & `frontengine_dev-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frontengine_dev"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 dependencies = [
     "PySide6",
     "qt-material",
 ]
```

