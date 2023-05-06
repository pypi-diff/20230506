# Comparing `tmp/frontengine_dev-0.0.6.tar.gz` & `tmp/frontengine_dev-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontengine_dev-0.0.6.tar", last modified: Sat May  6 12:05:39 2023, max compression
+gzip compressed data, was "frontengine_dev-0.0.7.tar", last modified: Sat May  6 12:49:48 2023, max compression
```

## Comparing `frontengine_dev-0.0.6.tar` & `frontengine_dev-0.0.7.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.473641 frontengine_dev-0.0.6/
--rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine_dev-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1418 2023-05-06 12:05:39.471646 frontengine_dev-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine_dev-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.141993 frontengine_dev-0.0.6/frontengine/
--rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine_dev-0.0.6/frontengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.144983 frontengine_dev-0.0.6/frontengine/show/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.6/frontengine/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.149978 frontengine_dev-0.0.6/frontengine/show/gif/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.6/frontengine/show/gif/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-05-06 11:59:16.000000 frontengine_dev-0.0.6/frontengine/show/gif/paint_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.154959 frontengine_dev-0.0.6/frontengine/show/image/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.6/frontengine/show/image/__init__.py
--rw-rw-rw-   0        0        0     1549 2023-05-06 11:59:16.000000 frontengine_dev-0.0.6/frontengine/show/image/paint_image.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.161939 frontengine_dev-0.0.6/frontengine/show/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.6/frontengine/show/sound_player/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-05-06 11:59:16.000000 frontengine_dev-0.0.6/frontengine/show/sound_player/sound_effect.py
--rw-rw-rw-   0        0        0     1720 2023-05-06 11:59:16.000000 frontengine_dev-0.0.6/frontengine/show/sound_player/sound_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.166925 frontengine_dev-0.0.6/frontengine/show/text/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.6/frontengine/show/text/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-05-06 11:59:16.000000 frontengine_dev-0.0.6/frontengine/show/text/draw_text.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.173910 frontengine_dev-0.0.6/frontengine/show/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.6/frontengine/show/video/__init__.py
--rw-rw-rw-   0        0        0     1962 2023-05-06 11:59:16.000000 frontengine_dev-0.0.6/frontengine/show/video/video_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.177895 frontengine_dev-0.0.6/frontengine/show/web/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.6/frontengine/show/web/__init__.py
--rw-rw-rw-   0        0        0      897 2023-05-06 11:59:16.000000 frontengine_dev-0.0.6/frontengine/show/web/webview.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.181889 frontengine_dev-0.0.6/frontengine/ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.6/frontengine/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.187869 frontengine_dev-0.0.6/frontengine/ui/main/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.6/frontengine/ui/main/__init__.py
--rw-rw-rw-   0        0        0     2598 2023-05-06 11:59:16.000000 frontengine_dev-0.0.6/frontengine/ui/main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.190863 frontengine_dev-0.0.6/frontengine/ui/setting/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/ui/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.194851 frontengine_dev-0.0.6/frontengine/ui/setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/ui/setting/gif/__init__.py
--rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine_dev-0.0.6/frontengine/ui/setting/gif/gif_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.202342 frontengine_dev-0.0.6/frontengine/ui/setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/ui/setting/image/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine_dev-0.0.6/frontengine/ui/setting/image/image_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.215310 frontengine_dev-0.0.6/frontengine/ui/setting/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/ui/setting/sound_player/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine_dev-0.0.6/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.246230 frontengine_dev-0.0.6/frontengine/ui/setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/ui/setting/text/__init__.py
--rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine_dev-0.0.6/frontengine/ui/setting/text/text_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.261184 frontengine_dev-0.0.6/frontengine/ui/setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/ui/setting/video/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine_dev-0.0.6/frontengine/ui/setting/video/video_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.285121 frontengine_dev-0.0.6/frontengine/ui/setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/ui/setting/web/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine_dev-0.0.6/frontengine/ui/setting/web/web_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.307577 frontengine_dev-0.0.6/frontengine/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.6/frontengine/user_setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.318546 frontengine_dev-0.0.6/frontengine/user_setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.6/frontengine/user_setting/gif/__init__.py
--rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine_dev-0.0.6/frontengine/user_setting/gif/gif_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.331508 frontengine_dev-0.0.6/frontengine/user_setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.6/frontengine/user_setting/image/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine_dev-0.0.6/frontengine/user_setting/image/image_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.337492 frontengine_dev-0.0.6/frontengine/user_setting/sound/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.6/frontengine/user_setting/sound/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine_dev-0.0.6/frontengine/user_setting/sound/sound_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.348463 frontengine_dev-0.0.6/frontengine/user_setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.6/frontengine/user_setting/text/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine_dev-0.0.6/frontengine/user_setting/text/text_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.360433 frontengine_dev-0.0.6/frontengine/user_setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.6/frontengine/user_setting/video/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine_dev-0.0.6/frontengine/user_setting/video/video_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.372399 frontengine_dev-0.0.6/frontengine/user_setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.6/frontengine/user_setting/web/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine_dev-0.0.6/frontengine/user_setting/web/web_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.382372 frontengine_dev-0.0.6/frontengine/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.6/frontengine/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.390351 frontengine_dev-0.0.6/frontengine/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.393344 frontengine_dev-0.0.6/frontengine/utils/file/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.405828 frontengine_dev-0.0.6/frontengine/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.418786 frontengine_dev-0.0.6/frontengine/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.428759 frontengine_dev-0.0.6/frontengine/utils/json/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.436743 frontengine_dev-0.0.6/frontengine/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine_dev-0.0.6/frontengine/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:05:39.468655 frontengine_dev-0.0.6/frontengine_dev.egg-info/
--rw-rw-rw-   0        0        0     1418 2023-05-06 12:05:39.000000 frontengine_dev-0.0.6/frontengine_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2514 2023-05-06 12:05:39.000000 frontengine_dev-0.0.6/frontengine_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 12:05:39.000000 frontengine_dev-0.0.6/frontengine_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 12:05:39.000000 frontengine_dev-0.0.6/frontengine_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 12:05:39.000000 frontengine_dev-0.0.6/frontengine_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1142 2023-05-06 12:05:19.000000 frontengine_dev-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 12:05:39.473641 frontengine_dev-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.880188 frontengine_dev-0.0.7/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine_dev-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1418 2023-05-06 12:49:48.879188 frontengine_dev-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine_dev-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.647811 frontengine_dev-0.0.7/frontengine/
+-rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine_dev-0.0.7/frontengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.653790 frontengine_dev-0.0.7/frontengine/show/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.7/frontengine/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.658781 frontengine_dev-0.0.7/frontengine/show/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.7/frontengine/show/gif/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-05-06 11:59:16.000000 frontengine_dev-0.0.7/frontengine/show/gif/paint_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.662768 frontengine_dev-0.0.7/frontengine/show/image/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.7/frontengine/show/image/__init__.py
+-rw-rw-rw-   0        0        0     1549 2023-05-06 11:59:16.000000 frontengine_dev-0.0.7/frontengine/show/image/paint_image.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.668752 frontengine_dev-0.0.7/frontengine/show/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.7/frontengine/show/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-05-06 11:59:16.000000 frontengine_dev-0.0.7/frontengine/show/sound_player/sound_effect.py
+-rw-rw-rw-   0        0        0     1720 2023-05-06 11:59:16.000000 frontengine_dev-0.0.7/frontengine/show/sound_player/sound_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.672744 frontengine_dev-0.0.7/frontengine/show/text/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.7/frontengine/show/text/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-05-06 11:59:16.000000 frontengine_dev-0.0.7/frontengine/show/text/draw_text.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.678725 frontengine_dev-0.0.7/frontengine/show/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.7/frontengine/show/video/__init__.py
+-rw-rw-rw-   0        0        0     1962 2023-05-06 11:59:16.000000 frontengine_dev-0.0.7/frontengine/show/video/video_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.683711 frontengine_dev-0.0.7/frontengine/show/web/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.7/frontengine/show/web/__init__.py
+-rw-rw-rw-   0        0        0      897 2023-05-06 11:59:16.000000 frontengine_dev-0.0.7/frontengine/show/web/webview.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.686703 frontengine_dev-0.0.7/frontengine/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.7/frontengine/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.689696 frontengine_dev-0.0.7/frontengine/ui/main/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.7/frontengine/ui/main/__init__.py
+-rw-rw-rw-   0        0        0     2659 2023-05-06 12:49:14.000000 frontengine_dev-0.0.7/frontengine/ui/main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.691690 frontengine_dev-0.0.7/frontengine/ui/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/ui/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.695679 frontengine_dev-0.0.7/frontengine/ui/setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/ui/setting/gif/__init__.py
+-rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine_dev-0.0.7/frontengine/ui/setting/gif/gif_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.700665 frontengine_dev-0.0.7/frontengine/ui/setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/ui/setting/image/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine_dev-0.0.7/frontengine/ui/setting/image/image_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.708645 frontengine_dev-0.0.7/frontengine/ui/setting/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/ui/setting/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine_dev-0.0.7/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.715629 frontengine_dev-0.0.7/frontengine/ui/setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/ui/setting/text/__init__.py
+-rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine_dev-0.0.7/frontengine/ui/setting/text/text_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.721610 frontengine_dev-0.0.7/frontengine/ui/setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/ui/setting/video/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine_dev-0.0.7/frontengine/ui/setting/video/video_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.725599 frontengine_dev-0.0.7/frontengine/ui/setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/ui/setting/web/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine_dev-0.0.7/frontengine/ui/setting/web/web_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.727595 frontengine_dev-0.0.7/frontengine/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.7/frontengine/user_setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.731588 frontengine_dev-0.0.7/frontengine/user_setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.7/frontengine/user_setting/gif/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine_dev-0.0.7/frontengine/user_setting/gif/gif_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.737567 frontengine_dev-0.0.7/frontengine/user_setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.7/frontengine/user_setting/image/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine_dev-0.0.7/frontengine/user_setting/image/image_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.741557 frontengine_dev-0.0.7/frontengine/user_setting/sound/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.7/frontengine/user_setting/sound/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine_dev-0.0.7/frontengine/user_setting/sound/sound_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.744548 frontengine_dev-0.0.7/frontengine/user_setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.7/frontengine/user_setting/text/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine_dev-0.0.7/frontengine/user_setting/text/text_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.747540 frontengine_dev-0.0.7/frontengine/user_setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.7/frontengine/user_setting/video/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine_dev-0.0.7/frontengine/user_setting/video/video_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.752527 frontengine_dev-0.0.7/frontengine/user_setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.7/frontengine/user_setting/web/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine_dev-0.0.7/frontengine/user_setting/web/web_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.754522 frontengine_dev-0.0.7/frontengine/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.7/frontengine/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.760505 frontengine_dev-0.0.7/frontengine/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.762500 frontengine_dev-0.0.7/frontengine/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.766490 frontengine_dev-0.0.7/frontengine/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.773476 frontengine_dev-0.0.7/frontengine/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.777460 frontengine_dev-0.0.7/frontengine/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.782447 frontengine_dev-0.0.7/frontengine/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine_dev-0.0.7/frontengine/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:49:48.874202 frontengine_dev-0.0.7/frontengine_dev.egg-info/
+-rw-rw-rw-   0        0        0     1418 2023-05-06 12:49:48.000000 frontengine_dev-0.0.7/frontengine_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2514 2023-05-06 12:49:48.000000 frontengine_dev-0.0.7/frontengine_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 12:49:48.000000 frontengine_dev-0.0.7/frontengine_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 12:49:48.000000 frontengine_dev-0.0.7/frontengine_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 12:49:48.000000 frontengine_dev-0.0.7/frontengine_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1142 2023-05-06 12:49:28.000000 frontengine_dev-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 12:49:48.880188 frontengine_dev-0.0.7/setup.cfg
```

### Comparing `frontengine_dev-0.0.6/LICENSE` & `frontengine_dev-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/PKG-INFO` & `frontengine_dev-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine_dev
-Version: 0.0.6
+Version: 0.0.7
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine_dev-0.0.6/README.md` & `frontengine_dev-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/show/gif/paint_gif.py` & `frontengine_dev-0.0.7/frontengine/show/gif/paint_gif.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/show/image/paint_image.py` & `frontengine_dev-0.0.7/frontengine/show/image/paint_image.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/show/sound_player/sound_effect.py` & `frontengine_dev-0.0.7/frontengine/show/sound_player/sound_effect.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/show/sound_player/sound_player.py` & `frontengine_dev-0.0.7/frontengine/show/sound_player/sound_player.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/show/text/draw_text.py` & `frontengine_dev-0.0.7/frontengine/show/text/draw_text.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/show/video/video_player.py` & `frontengine_dev-0.0.7/frontengine/show/video/video_player.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/show/web/webview.py` & `frontengine_dev-0.0.7/frontengine/show/web/webview.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/ui/main/main_ui.py` & `frontengine_dev-0.0.7/frontengine/ui/main/main_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os
 import sys
+from pathlib import Path
 
-from PySide6.QtGui import QImage
-from PySide6.QtWidgets import QMainWindow, QApplication, QGridLayout, QTabWidget
+from PySide6.QtGui import QImage, QIcon
+from PySide6.QtWidgets import QMainWindow, QApplication, QGridLayout, QTabWidget, QSystemTrayIcon
 from qt_material import apply_stylesheet
 
 from frontengine.ui.setting.gif.gif_setting_ui import GIFSettingUI
 from frontengine.ui.setting.image.image_setting_ui import ImageSettingUI
 from frontengine.ui.setting.sound_player.sound_player_setting_ui import SoundPlayerSettingUI
 from frontengine.ui.setting.text.text_setting_ui import TextSettingUI
 from frontengine.ui.setting.video.video_setting_ui import VideoSettingUI
```

### Comparing `frontengine_dev-0.0.6/frontengine/ui/setting/gif/gif_setting_ui.py` & `frontengine_dev-0.0.7/frontengine/ui/setting/gif/gif_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/ui/setting/image/image_setting_ui.py` & `frontengine_dev-0.0.7/frontengine/ui/setting/image/image_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/ui/setting/sound_player/sound_player_setting_ui.py` & `frontengine_dev-0.0.7/frontengine/ui/setting/sound_player/sound_player_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/ui/setting/text/text_setting_ui.py` & `frontengine_dev-0.0.7/frontengine/ui/setting/text/text_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/ui/setting/video/video_setting_ui.py` & `frontengine_dev-0.0.7/frontengine/ui/setting/video/video_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/ui/setting/web/web_setting_ui.py` & `frontengine_dev-0.0.7/frontengine/ui/setting/web/web_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/utils/file/open/open_file.py` & `frontengine_dev-0.0.7/frontengine/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/utils/file/save/save_file.py` & `frontengine_dev-0.0.7/frontengine/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/utils/json/json_file.py` & `frontengine_dev-0.0.7/frontengine/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine/utils/json_format/json_process.py` & `frontengine_dev-0.0.7/frontengine/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/frontengine_dev.egg-info/PKG-INFO` & `frontengine_dev-0.0.7/frontengine_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine-dev
-Version: 0.0.6
+Version: 0.0.7
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine_dev-0.0.6/frontengine_dev.egg-info/SOURCES.txt` & `frontengine_dev-0.0.7/frontengine_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.6/pyproject.toml` & `frontengine_dev-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frontengine_dev"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 dependencies = [
     "PySide6",
     "qt-material",
 ]
```

