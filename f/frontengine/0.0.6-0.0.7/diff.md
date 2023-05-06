# Comparing `tmp/frontengine-0.0.6.tar.gz` & `tmp/frontengine-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontengine-0.0.6.tar", last modified: Sat May  6 11:59:38 2023, max compression
+gzip compressed data, was "frontengine-0.0.7.tar", last modified: Sat May  6 12:50:53 2023, max compression
```

## Comparing `frontengine-0.0.6.tar` & `frontengine-0.0.7.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.350331 frontengine-0.0.6/
--rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1414 2023-05-06 11:59:38.349333 frontengine-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.153645 frontengine-0.0.6/frontengine/
--rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine-0.0.6/frontengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.195533 frontengine-0.0.6/frontengine/show/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.6/frontengine/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.198526 frontengine-0.0.6/frontengine/show/gif/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.6/frontengine/show/gif/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-05-06 11:59:16.000000 frontengine-0.0.6/frontengine/show/gif/paint_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.202516 frontengine-0.0.6/frontengine/show/image/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.6/frontengine/show/image/__init__.py
--rw-rw-rw-   0        0        0     1549 2023-05-06 11:59:16.000000 frontengine-0.0.6/frontengine/show/image/paint_image.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.209496 frontengine-0.0.6/frontengine/show/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.6/frontengine/show/sound_player/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-05-06 11:59:16.000000 frontengine-0.0.6/frontengine/show/sound_player/sound_effect.py
--rw-rw-rw-   0        0        0     1720 2023-05-06 11:59:16.000000 frontengine-0.0.6/frontengine/show/sound_player/sound_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.213489 frontengine-0.0.6/frontengine/show/text/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.6/frontengine/show/text/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-05-06 11:59:16.000000 frontengine-0.0.6/frontengine/show/text/draw_text.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.218472 frontengine-0.0.6/frontengine/show/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.6/frontengine/show/video/__init__.py
--rw-rw-rw-   0        0        0     1962 2023-05-06 11:59:16.000000 frontengine-0.0.6/frontengine/show/video/video_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.221464 frontengine-0.0.6/frontengine/show/web/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.6/frontengine/show/web/__init__.py
--rw-rw-rw-   0        0        0      897 2023-05-06 11:59:16.000000 frontengine-0.0.6/frontengine/show/web/webview.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.224457 frontengine-0.0.6/frontengine/ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.6/frontengine/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.228445 frontengine-0.0.6/frontengine/ui/main/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.6/frontengine/ui/main/__init__.py
--rw-rw-rw-   0        0        0     2598 2023-05-06 11:59:16.000000 frontengine-0.0.6/frontengine/ui/main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.229443 frontengine-0.0.6/frontengine/ui/setting/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/ui/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.232435 frontengine-0.0.6/frontengine/ui/setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/ui/setting/gif/__init__.py
--rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine-0.0.6/frontengine/ui/setting/gif/gif_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.236424 frontengine-0.0.6/frontengine/ui/setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/ui/setting/image/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine-0.0.6/frontengine/ui/setting/image/image_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.239417 frontengine-0.0.6/frontengine/ui/setting/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/ui/setting/sound_player/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine-0.0.6/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.242407 frontengine-0.0.6/frontengine/ui/setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/ui/setting/text/__init__.py
--rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine-0.0.6/frontengine/ui/setting/text/text_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.245400 frontengine-0.0.6/frontengine/ui/setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/ui/setting/video/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine-0.0.6/frontengine/ui/setting/video/video_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.248392 frontengine-0.0.6/frontengine/ui/setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/ui/setting/web/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine-0.0.6/frontengine/ui/setting/web/web_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.250387 frontengine-0.0.6/frontengine/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.6/frontengine/user_setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.252380 frontengine-0.0.6/frontengine/user_setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.6/frontengine/user_setting/gif/__init__.py
--rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine-0.0.6/frontengine/user_setting/gif/gif_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.259362 frontengine-0.0.6/frontengine/user_setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.6/frontengine/user_setting/image/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine-0.0.6/frontengine/user_setting/image/image_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.267341 frontengine-0.0.6/frontengine/user_setting/sound/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.6/frontengine/user_setting/sound/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine-0.0.6/frontengine/user_setting/sound/sound_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.276321 frontengine-0.0.6/frontengine/user_setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.6/frontengine/user_setting/text/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine-0.0.6/frontengine/user_setting/text/text_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.284295 frontengine-0.0.6/frontengine/user_setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.6/frontengine/user_setting/video/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine-0.0.6/frontengine/user_setting/video/video_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.291277 frontengine-0.0.6/frontengine/user_setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.6/frontengine/user_setting/web/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine-0.0.6/frontengine/user_setting/web/web_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.293271 frontengine-0.0.6/frontengine/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.6/frontengine/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.309231 frontengine-0.0.6/frontengine/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.311224 frontengine-0.0.6/frontengine/utils/file/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.319409 frontengine-0.0.6/frontengine/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.328388 frontengine-0.0.6/frontengine/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.337364 frontengine-0.0.6/frontengine/utils/json/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.347338 frontengine-0.0.6/frontengine/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine-0.0.6/frontengine/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:59:38.191545 frontengine-0.0.6/frontengine.egg-info/
--rw-rw-rw-   0        0        0     1414 2023-05-06 11:59:38.000000 frontengine-0.0.6/frontengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2494 2023-05-06 11:59:38.000000 frontengine-0.0.6/frontengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:59:38.000000 frontengine-0.0.6/frontengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 11:59:38.000000 frontengine-0.0.6/frontengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 11:59:38.000000 frontengine-0.0.6/frontengine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1138 2023-05-06 11:59:16.000000 frontengine-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 11:59:38.350331 frontengine-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.121584 frontengine-0.0.7/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1414 2023-05-06 12:50:53.120586 frontengine-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.422460 frontengine-0.0.7/frontengine/
+-rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine-0.0.7/frontengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.633889 frontengine-0.0.7/frontengine/show/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.7/frontengine/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.638877 frontengine-0.0.7/frontengine/show/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.7/frontengine/show/gif/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-05-06 11:59:16.000000 frontengine-0.0.7/frontengine/show/gif/paint_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.646854 frontengine-0.0.7/frontengine/show/image/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.7/frontengine/show/image/__init__.py
+-rw-rw-rw-   0        0        0     1549 2023-05-06 11:59:16.000000 frontengine-0.0.7/frontengine/show/image/paint_image.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.729633 frontengine-0.0.7/frontengine/show/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.7/frontengine/show/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-05-06 11:59:16.000000 frontengine-0.0.7/frontengine/show/sound_player/sound_effect.py
+-rw-rw-rw-   0        0        0     1720 2023-05-06 11:59:16.000000 frontengine-0.0.7/frontengine/show/sound_player/sound_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.755565 frontengine-0.0.7/frontengine/show/text/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.7/frontengine/show/text/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-05-06 11:59:16.000000 frontengine-0.0.7/frontengine/show/text/draw_text.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.802438 frontengine-0.0.7/frontengine/show/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.7/frontengine/show/video/__init__.py
+-rw-rw-rw-   0        0        0     1962 2023-05-06 11:59:16.000000 frontengine-0.0.7/frontengine/show/video/video_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.833355 frontengine-0.0.7/frontengine/show/web/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.7/frontengine/show/web/__init__.py
+-rw-rw-rw-   0        0        0      897 2023-05-06 11:59:16.000000 frontengine-0.0.7/frontengine/show/web/webview.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.933088 frontengine-0.0.7/frontengine/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.7/frontengine/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.952038 frontengine-0.0.7/frontengine/ui/main/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.7/frontengine/ui/main/__init__.py
+-rw-rw-rw-   0        0        0     2659 2023-05-06 12:49:14.000000 frontengine-0.0.7/frontengine/ui/main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.960016 frontengine-0.0.7/frontengine/ui/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/ui/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.971985 frontengine-0.0.7/frontengine/ui/setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/ui/setting/gif/__init__.py
+-rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine-0.0.7/frontengine/ui/setting/gif/gif_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.976972 frontengine-0.0.7/frontengine/ui/setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/ui/setting/image/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine-0.0.7/frontengine/ui/setting/image/image_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.008885 frontengine-0.0.7/frontengine/ui/setting/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/ui/setting/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine-0.0.7/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.013872 frontengine-0.0.7/frontengine/ui/setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/ui/setting/text/__init__.py
+-rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine-0.0.7/frontengine/ui/setting/text/text_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.026838 frontengine-0.0.7/frontengine/ui/setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/ui/setting/video/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine-0.0.7/frontengine/ui/setting/video/video_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.035813 frontengine-0.0.7/frontengine/ui/setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/ui/setting/web/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine-0.0.7/frontengine/ui/setting/web/web_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.039804 frontengine-0.0.7/frontengine/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.7/frontengine/user_setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.044790 frontengine-0.0.7/frontengine/user_setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.7/frontengine/user_setting/gif/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine-0.0.7/frontengine/user_setting/gif/gif_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.050773 frontengine-0.0.7/frontengine/user_setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.7/frontengine/user_setting/image/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine-0.0.7/frontengine/user_setting/image/image_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.055760 frontengine-0.0.7/frontengine/user_setting/sound/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.7/frontengine/user_setting/sound/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine-0.0.7/frontengine/user_setting/sound/sound_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.062742 frontengine-0.0.7/frontengine/user_setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.7/frontengine/user_setting/text/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine-0.0.7/frontengine/user_setting/text/text_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.069723 frontengine-0.0.7/frontengine/user_setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.7/frontengine/user_setting/video/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine-0.0.7/frontengine/user_setting/video/video_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.073715 frontengine-0.0.7/frontengine/user_setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.7/frontengine/user_setting/web/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine-0.0.7/frontengine/user_setting/web/web_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.078699 frontengine-0.0.7/frontengine/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.7/frontengine/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.090667 frontengine-0.0.7/frontengine/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.092662 frontengine-0.0.7/frontengine/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.095653 frontengine-0.0.7/frontengine/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.104630 frontengine-0.0.7/frontengine/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.113605 frontengine-0.0.7/frontengine/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:53.118592 frontengine-0.0.7/frontengine/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine-0.0.7/frontengine/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:50:52.564075 frontengine-0.0.7/frontengine.egg-info/
+-rw-rw-rw-   0        0        0     1414 2023-05-06 12:50:52.000000 frontengine-0.0.7/frontengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2494 2023-05-06 12:50:52.000000 frontengine-0.0.7/frontengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 12:50:52.000000 frontengine-0.0.7/frontengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 12:50:52.000000 frontengine-0.0.7/frontengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 12:50:52.000000 frontengine-0.0.7/frontengine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1138 2023-05-06 12:50:29.000000 frontengine-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 12:50:53.122582 frontengine-0.0.7/setup.cfg
```

### Comparing `frontengine-0.0.6/LICENSE` & `frontengine-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/PKG-INFO` & `frontengine-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine
-Version: 0.0.6
+Version: 0.0.7
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine-0.0.6/README.md` & `frontengine-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/show/gif/paint_gif.py` & `frontengine-0.0.7/frontengine/show/gif/paint_gif.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/show/image/paint_image.py` & `frontengine-0.0.7/frontengine/show/image/paint_image.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/show/sound_player/sound_effect.py` & `frontengine-0.0.7/frontengine/show/sound_player/sound_effect.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/show/sound_player/sound_player.py` & `frontengine-0.0.7/frontengine/show/sound_player/sound_player.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/show/text/draw_text.py` & `frontengine-0.0.7/frontengine/show/text/draw_text.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/show/video/video_player.py` & `frontengine-0.0.7/frontengine/show/video/video_player.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/show/web/webview.py` & `frontengine-0.0.7/frontengine/show/web/webview.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/ui/main/main_ui.py` & `frontengine-0.0.7/frontengine/ui/main/main_ui.py`

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

### Comparing `frontengine-0.0.6/frontengine/ui/setting/gif/gif_setting_ui.py` & `frontengine-0.0.7/frontengine/ui/setting/gif/gif_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/ui/setting/image/image_setting_ui.py` & `frontengine-0.0.7/frontengine/ui/setting/image/image_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/ui/setting/sound_player/sound_player_setting_ui.py` & `frontengine-0.0.7/frontengine/ui/setting/sound_player/sound_player_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/ui/setting/text/text_setting_ui.py` & `frontengine-0.0.7/frontengine/ui/setting/text/text_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/ui/setting/video/video_setting_ui.py` & `frontengine-0.0.7/frontengine/ui/setting/video/video_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/ui/setting/web/web_setting_ui.py` & `frontengine-0.0.7/frontengine/ui/setting/web/web_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/utils/file/open/open_file.py` & `frontengine-0.0.7/frontengine/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/utils/file/save/save_file.py` & `frontengine-0.0.7/frontengine/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/utils/json/json_file.py` & `frontengine-0.0.7/frontengine/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine/utils/json_format/json_process.py` & `frontengine-0.0.7/frontengine/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/frontengine.egg-info/PKG-INFO` & `frontengine-0.0.7/frontengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine
-Version: 0.0.6
+Version: 0.0.7
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine-0.0.6/frontengine.egg-info/SOURCES.txt` & `frontengine-0.0.7/frontengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.6/pyproject.toml` & `frontengine-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frontengine"
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

