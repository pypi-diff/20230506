# Comparing `tmp/dj_beatcloud-2.5.0b0.tar.gz` & `tmp/dj_beatcloud-2.5.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.5.0b0.tar", last modified: Wed May  3 03:53:24 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.5.1b0.tar", last modified: Sat May  6 19:50:41 2023, max compression
```

## Comparing `dj_beatcloud-2.5.0b0.tar` & `dj_beatcloud-2.5.1b0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.217272 dj_beatcloud-2.5.0b0/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.0b0/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2002 2023-05-03 03:53:24.217364 dj_beatcloud-2.5.0b0/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)      717 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.202279 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2002 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1872 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.203371 dj_beatcloud-2.5.0b0/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2462 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.206815 dj_beatcloud-2.5.0b0/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2815 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1213 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13431 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-03 01:35:47.000000 dj_beatcloud-2.5.0b0/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5020 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.207070 dj_beatcloud-2.5.0b0/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.210947 dj_beatcloud-2.5.0b0/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_combiner.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5334 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.212896 dj_beatcloud-2.5.0b0/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16576 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5977 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2151 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.214475 dj_beatcloud-2.5.0b0/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4710 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8276 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4324 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8707 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5000 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      880 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.216990 dj_beatcloud-2.5.0b0/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      879 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3478 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9526 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8363 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-25 19:26:48.000000 dj_beatcloud-2.5.0b0/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-03 03:53:24.217669 dj_beatcloud-2.5.0b0/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2223 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.315897 dj_beatcloud-2.5.1b0/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b0/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-06 19:50:41.315988 dj_beatcloud-2.5.1b0/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.307611 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1834 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.308259 dj_beatcloud-2.5.1b0/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2462 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b0/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.310030 dj_beatcloud-2.5.1b0/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2815 2023-05-06 19:49:39.000000 dj_beatcloud-2.5.1b0/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1241 2023-05-06 19:49:01.000000 dj_beatcloud-2.5.1b0/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13540 2023-05-06 19:49:38.000000 dj_beatcloud-2.5.1b0/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4504 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.310227 dj_beatcloud-2.5.1b0/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.312301 dj_beatcloud-2.5.1b0/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/playlist_combiner.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5338 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.313394 dj_beatcloud-2.5.1b0/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2151 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.314426 dj_beatcloud-2.5.1b0/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b0/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      733 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.315765 dj_beatcloud-2.5.1b0/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10100 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b0/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-06 19:50:41.316388 dj_beatcloud-2.5.1b0/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2209 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/setup.py
```

### Comparing `dj_beatcloud-2.5.0b0/LICENSE` & `dj_beatcloud-2.5.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/PKG-INFO` & `dj_beatcloud-2.5.1b0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 5f62  : 2.1.Name: dj_b
 00000020: 6561 7463 6c6f 7564 0a56 6572 7369 6f6e  eatcloud.Version
-00000030: 3a20 322e 352e 3062 300a 5375 6d6d 6172  : 2.5.0b0.Summar
+00000030: 3a20 322e 352e 3162 300a 5375 6d6d 6172  : 2.5.1b0.Summar
 00000040: 793a 2044 4a20 546f 6f6c 7320 6973 2061  y: DJ Tools is a
 00000050: 206c 6962 7261 7279 2066 6f72 206d 616e   library for man
 00000060: 6167 696e 6720 6120 636f 6c6c 6563 7469  aging a collecti
 00000070: 6f6e 206f 6620 6d75 7369 6320 616e 6420  on of music and 
 00000080: 5265 6b6f 7264 626f 7820 584d 4c20 6669  Rekordbox XML fi
 00000090: 6c65 732e 0a48 6f6d 652d 7061 6765 3a20  les..Home-page: 
 000000a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
@@ -82,45 +82,82 @@
 00000510: 5b21 5b69 6d61 6765 5d28 6874 7470 733a  [![image](https:
 00000520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
 00000530: 2f70 7970 692f 762f 646a 2d62 6561 7463  /pypi/v/dj-beatc
 00000540: 6c6f 7564 2e73 7667 295d 2868 7474 7073  loud.svg)](https
 00000550: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
 00000560: 6563 742f 646a 2d62 6561 7463 6c6f 7564  ect/dj-beatcloud
 00000570: 2f29 0a0a 506c 6561 7365 2073 6565 2074  /)..Please see t
-00000580: 6865 205b 646f 6373 5d28 646f 6373 2f69  he [docs](docs/i
-00000590: 6e64 6578 2e6d 6429 2066 6f72 2074 7574  ndex.md) for tut
-000005a0: 6f72 6961 6c73 2c20 686f 772d 746f 2067  orials, how-to g
-000005b0: 7569 6465 732c 2063 6f6e 6365 7074 7561  uides, conceptua
-000005c0: 6c20 6775 6964 6573 2c20 616e 6420 7265  l guides, and re
-000005d0: 6665 7265 6e63 6573 210a 0a23 2052 656c  ferences!..# Rel
-000005e0: 6561 7365 2050 6c61 6e0a 2a20 322e 342e  ease Plan.* 2.4.
-000005f0: 310a 2020 2020 2d20 5b20 5d20 4d61 6b65  1.    - [ ] Make
-00000600: 2053 706f 7469 6679 2041 5049 2063 616c   Spotify API cal
-00000610: 6c73 2061 7379 6e63 6872 6f6e 6f75 730a  ls asynchronous.
-00000620: 2020 2020 2d20 5b20 5d20 496d 7072 6f76      - [ ] Improv
-00000630: 6564 2053 706f 7469 6679 2041 5049 2072  ed Spotify API r
-00000640: 6571 7565 7374 2073 7461 6269 6c69 7479  equest stability
-00000650: 200a 2020 2020 2d20 5b20 5d20 496d 7072   .    - [ ] Impr
-00000660: 6f76 6564 2052 6564 6469 7420 706f 7374  oved Reddit post
-00000670: 2070 6172 7369 6e67 2061 6e64 2053 706f   parsing and Spo
-00000680: 7469 6679 2073 6561 7263 6869 6e67 0a20  tify searching. 
-00000690: 2020 202d 205b 205d 204f 7074 696d 697a     - [ ] Optimiz
-000006a0: 6520 7079 7465 7374 2d63 6f76 2077 6f72  e pytest-cov wor
-000006b0: 6b66 6c6f 7720 616e 6420 6164 6420 5769  kflow and add Wi
-000006c0: 6e64 6f77 7320 7275 6e6e 6572 0a2a 2032  ndows runner.* 2
-000006d0: 2e35 2e30 0a20 2020 202d 205b 205d 2043  .5.0.    - [ ] C
-000006e0: 7265 6174 6520 7365 7269 616c 697a 6572  reate serializer
-000006f0: 7320 7061 636b 6167 6520 666f 7220 636f  s package for co
-00000700: 6e76 6572 7469 6e67 2064 6174 6162 6173  nverting databas
-00000710: 6520 6669 6c65 7320 6672 6f6d 206f 7468  e files from oth
-00000720: 6572 2044 4a20 736f 6674 7761 7265 2028  er DJ software (
-00000730: 652e 672e 2053 6572 6174 6f2c 2054 7261  e.g. Serato, Tra
-00000740: 6b74 6f72 2c20 4465 6e6f 6e2c 2065 7463  ktor, Denon, etc
-00000750: 2e29 2073 6f20 7468 6174 206f 7065 7261  .) so that opera
-00000760: 7469 6f6e 7320 696e 2074 6865 2072 656b  tions in the rek
-00000770: 6f72 6462 6f78 2070 6163 6b61 6765 2063  ordbox package c
-00000780: 616e 2062 6520 7573 6564 206f 6e20 7468  an be used on th
-00000790: 656d 0a0a 2320 436f 6e74 7269 6275 7469  em..# Contributi
-000007a0: 6f6e 0a50 6c65 6173 6520 7365 6520 7468  on.Please see th
-000007b0: 6520 5b43 4f4e 5452 4942 5554 494e 475d  e [CONTRIBUTING]
-000007c0: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
-000007d0: 290a                                     ).
+00000580: 6865 205b 646f 6373 5d28 6874 7470 733a  he [docs](https:
+00000590: 2f2f 612d 7269 6368 2e67 6974 6875 622e  //a-rich.github.
+000005a0: 696f 2f44 4a2d 546f 6f6c 732f 2920 666f  io/DJ-Tools/) fo
+000005b0: 7220 7475 746f 7269 616c 732c 2068 6f77  r tutorials, how
+000005c0: 2d74 6f20 6775 6964 6573 2c20 636f 6e63  -to guides, conc
+000005d0: 6570 7475 616c 2067 7569 6465 732c 2061  eptual guides, a
+000005e0: 6e64 2072 6566 6572 656e 6365 7321 0a0a  nd references!..
+000005f0: 2320 5265 6c65 6173 6520 506c 616e 0a2a  # Release Plan.*
+00000600: 2032 2e35 2e31 0a20 2020 202d 205b 205d   2.5.1.    - [ ]
+00000610: 205b 5374 6162 696c 6974 7920 6973 7375   [Stability issu
+00000620: 6573 2077 6974 6820 7265 7175 6573 7473  es with requests
+00000630: 2074 6f20 7468 6520 7365 6172 6368 2065   to the search e
+00000640: 6e64 706f 696e 7420 6f66 2074 6865 2053  ndpoint of the S
+00000650: 706f 7469 6679 2041 5049 5d28 6874 7470  potify API](http
+00000660: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00000670: 2d72 6963 682f 444a 2d54 6f6f 6c73 2f69  -rich/DJ-Tools/i
+00000680: 7373 7565 732f 3538 290a 2020 2020 2d20  ssues/58).    - 
+00000690: 5b20 5d20 5b4d 616b 6520 5370 6f74 6966  [ ] [Make Spotif
+000006a0: 7920 4150 4920 6361 6c6c 7320 6173 796e  y API calls asyn
+000006b0: 6368 726f 6e6f 7573 5d28 6874 7470 733a  chronous](https:
+000006c0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 2d72  //github.com/a-r
+000006d0: 6963 682f 444a 2d54 6f6f 6c73 2f69 7373  ich/DJ-Tools/iss
+000006e0: 7565 732f 3338 290a 2020 2020 2d20 5b20  ues/38).    - [ 
+000006f0: 5d20 5b50 7269 6e74 2041 5343 4949 2068  ] [Print ASCII h
+00000700: 6973 746f 6772 616d 206f 6620 7461 6720  istogram of tag 
+00000710: 7374 6174 6973 7469 6373 2066 6f72 2043  statistics for C
+00000720: 6f6d 6269 6e65 7220 706c 6179 6c69 7374  ombiner playlist
+00000730: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000740: 622e 636f 6d2f 612d 7269 6368 2f44 4a2d  b.com/a-rich/DJ-
+00000750: 546f 6f6c 732f 6973 7375 6573 2f38 3729  Tools/issues/87)
+00000760: 0a20 2020 202d 205b 785d 205b 4465 7072  .    - [x] [Depr
+00000770: 6563 6174 6520 7265 6769 7374 6572 6564  ecate registered
+00000780: 5f75 7365 7273 2e79 616d 6c5d 2868 7474  _users.yaml](htt
+00000790: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000007a0: 612d 7269 6368 2f44 4a2d 546f 6f6c 732f  a-rich/DJ-Tools/
+000007b0: 6973 7375 6573 2f39 3929 0a20 2020 202d  issues/99).    -
+000007c0: 205b 785d 205b 5061 7261 6d65 7465 7269   [x] [Parameteri
+000007d0: 7a65 2077 6865 7468 6572 2042 6561 7463  ze whether Beatc
+000007e0: 6c6f 7564 2074 7261 636b 7320 7368 6f75  loud tracks shou
+000007f0: 6c64 2062 6520 7265 6164 2061 7320 3c74  ld be read as <t
+00000800: 6974 6c65 3e20 2d20 3c61 7274 6973 743e  itle> - <artist>
+00000810: 206f 7220 7669 6365 2076 6572 7361 5d28   or vice versa](
+00000820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000830: 6f6d 2f61 2d72 6963 682f 444a 2d54 6f6f  om/a-rich/DJ-Too
+00000840: 6c73 2f69 7373 7565 732f 3935 290a 2a20  ls/issues/95).* 
+00000850: 322e 362e 300a 2020 2020 2d20 5b20 5d20  2.6.0.    - [ ] 
+00000860: 5b43 7265 6174 6520 7365 7269 616c 697a  [Create serializ
+00000870: 6572 7320 7061 636b 6167 6520 666f 7220  ers package for 
+00000880: 636f 6e76 6572 7469 6e67 2064 6174 6162  converting datab
+00000890: 6173 6520 6669 6c65 7320 6672 6f6d 206f  ase files from o
+000008a0: 7468 6572 2044 4a20 736f 6674 7761 7265  ther DJ software
+000008b0: 2028 652e 672e 2053 6572 6174 6f2c 2054   (e.g. Serato, T
+000008c0: 7261 6b74 6f72 2c20 4465 6e6f 6e2c 2065  raktor, Denon, e
+000008d0: 7463 2e29 2073 6f20 7468 6174 206f 7065  tc.) so that ope
+000008e0: 7261 7469 6f6e 7320 696e 2074 6865 2072  rations in the r
+000008f0: 656b 6f72 6462 6f78 2070 6163 6b61 6765  ekordbox package
+00000900: 2063 616e 2062 6520 7573 6564 206f 6e20   can be used on 
+00000910: 7468 656d 5d28 6874 7470 733a 2f2f 6769  them](https://gi
+00000920: 7468 7562 2e63 6f6d 2f61 2d72 6963 682f  thub.com/a-rich/
+00000930: 444a 2d54 6f6f 6c73 2f69 7373 7565 732f  DJ-Tools/issues/
+00000940: 3638 290a 2020 2020 2d20 5b20 5d20 5b49  68).    - [ ] [I
+00000950: 6d70 726f 7665 2052 6564 6469 7420 7375  mprove Reddit su
+00000960: 626d 6973 7369 6f6e 2074 6974 6c65 2070  bmission title p
+00000970: 6172 7369 6e67 2069 6e20 6f72 6465 7220  arsing in order 
+00000980: 746f 2069 6d70 726f 7665 2070 7265 6369  to improve preci
+00000990: 7369 6f6e 2061 6e64 2072 6563 616c 6c20  sion and recall 
+000009a0: 6f66 2053 706f 7469 6679 2041 5049 2073  of Spotify API s
+000009b0: 6561 7263 6820 7265 7375 6c74 735d 2868  earch results](h
+000009c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000009d0: 6d2f 612d 7269 6368 2f44 4a2d 546f 6f6c  m/a-rich/DJ-Tool
+000009e0: 732f 6973 7375 6573 2f35 3929 0a0a 2320  s/issues/59)..# 
+000009f0: 436f 6e74 7269 6275 7469 6f6e 0a50 6c65  Contribution.Ple
+00000a00: 6173 6520 7365 6520 7468 6520 5b43 4f4e  ase see the [CON
+00000a10: 5452 4942 5554 494e 475d 2843 4f4e 5452  TRIBUTING](CONTR
+00000a20: 4942 5554 494e 472e 6d64 290a            IBUTING.md).
```

### Comparing `dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 2d62  : 2.1.Name: dj-b
 00000020: 6561 7463 6c6f 7564 0a56 6572 7369 6f6e  eatcloud.Version
-00000030: 3a20 322e 352e 3062 300a 5375 6d6d 6172  : 2.5.0b0.Summar
+00000030: 3a20 322e 352e 3162 300a 5375 6d6d 6172  : 2.5.1b0.Summar
 00000040: 793a 2044 4a20 546f 6f6c 7320 6973 2061  y: DJ Tools is a
 00000050: 206c 6962 7261 7279 2066 6f72 206d 616e   library for man
 00000060: 6167 696e 6720 6120 636f 6c6c 6563 7469  aging a collecti
 00000070: 6f6e 206f 6620 6d75 7369 6320 616e 6420  on of music and 
 00000080: 5265 6b6f 7264 626f 7820 584d 4c20 6669  Rekordbox XML fi
 00000090: 6c65 732e 0a48 6f6d 652d 7061 6765 3a20  les..Home-page: 
 000000a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
@@ -82,45 +82,82 @@
 00000510: 5b21 5b69 6d61 6765 5d28 6874 7470 733a  [![image](https:
 00000520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
 00000530: 2f70 7970 692f 762f 646a 2d62 6561 7463  /pypi/v/dj-beatc
 00000540: 6c6f 7564 2e73 7667 295d 2868 7474 7073  loud.svg)](https
 00000550: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
 00000560: 6563 742f 646a 2d62 6561 7463 6c6f 7564  ect/dj-beatcloud
 00000570: 2f29 0a0a 506c 6561 7365 2073 6565 2074  /)..Please see t
-00000580: 6865 205b 646f 6373 5d28 646f 6373 2f69  he [docs](docs/i
-00000590: 6e64 6578 2e6d 6429 2066 6f72 2074 7574  ndex.md) for tut
-000005a0: 6f72 6961 6c73 2c20 686f 772d 746f 2067  orials, how-to g
-000005b0: 7569 6465 732c 2063 6f6e 6365 7074 7561  uides, conceptua
-000005c0: 6c20 6775 6964 6573 2c20 616e 6420 7265  l guides, and re
-000005d0: 6665 7265 6e63 6573 210a 0a23 2052 656c  ferences!..# Rel
-000005e0: 6561 7365 2050 6c61 6e0a 2a20 322e 342e  ease Plan.* 2.4.
-000005f0: 310a 2020 2020 2d20 5b20 5d20 4d61 6b65  1.    - [ ] Make
-00000600: 2053 706f 7469 6679 2041 5049 2063 616c   Spotify API cal
-00000610: 6c73 2061 7379 6e63 6872 6f6e 6f75 730a  ls asynchronous.
-00000620: 2020 2020 2d20 5b20 5d20 496d 7072 6f76      - [ ] Improv
-00000630: 6564 2053 706f 7469 6679 2041 5049 2072  ed Spotify API r
-00000640: 6571 7565 7374 2073 7461 6269 6c69 7479  equest stability
-00000650: 200a 2020 2020 2d20 5b20 5d20 496d 7072   .    - [ ] Impr
-00000660: 6f76 6564 2052 6564 6469 7420 706f 7374  oved Reddit post
-00000670: 2070 6172 7369 6e67 2061 6e64 2053 706f   parsing and Spo
-00000680: 7469 6679 2073 6561 7263 6869 6e67 0a20  tify searching. 
-00000690: 2020 202d 205b 205d 204f 7074 696d 697a     - [ ] Optimiz
-000006a0: 6520 7079 7465 7374 2d63 6f76 2077 6f72  e pytest-cov wor
-000006b0: 6b66 6c6f 7720 616e 6420 6164 6420 5769  kflow and add Wi
-000006c0: 6e64 6f77 7320 7275 6e6e 6572 0a2a 2032  ndows runner.* 2
-000006d0: 2e35 2e30 0a20 2020 202d 205b 205d 2043  .5.0.    - [ ] C
-000006e0: 7265 6174 6520 7365 7269 616c 697a 6572  reate serializer
-000006f0: 7320 7061 636b 6167 6520 666f 7220 636f  s package for co
-00000700: 6e76 6572 7469 6e67 2064 6174 6162 6173  nverting databas
-00000710: 6520 6669 6c65 7320 6672 6f6d 206f 7468  e files from oth
-00000720: 6572 2044 4a20 736f 6674 7761 7265 2028  er DJ software (
-00000730: 652e 672e 2053 6572 6174 6f2c 2054 7261  e.g. Serato, Tra
-00000740: 6b74 6f72 2c20 4465 6e6f 6e2c 2065 7463  ktor, Denon, etc
-00000750: 2e29 2073 6f20 7468 6174 206f 7065 7261  .) so that opera
-00000760: 7469 6f6e 7320 696e 2074 6865 2072 656b  tions in the rek
-00000770: 6f72 6462 6f78 2070 6163 6b61 6765 2063  ordbox package c
-00000780: 616e 2062 6520 7573 6564 206f 6e20 7468  an be used on th
-00000790: 656d 0a0a 2320 436f 6e74 7269 6275 7469  em..# Contributi
-000007a0: 6f6e 0a50 6c65 6173 6520 7365 6520 7468  on.Please see th
-000007b0: 6520 5b43 4f4e 5452 4942 5554 494e 475d  e [CONTRIBUTING]
-000007c0: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
-000007d0: 290a                                     ).
+00000580: 6865 205b 646f 6373 5d28 6874 7470 733a  he [docs](https:
+00000590: 2f2f 612d 7269 6368 2e67 6974 6875 622e  //a-rich.github.
+000005a0: 696f 2f44 4a2d 546f 6f6c 732f 2920 666f  io/DJ-Tools/) fo
+000005b0: 7220 7475 746f 7269 616c 732c 2068 6f77  r tutorials, how
+000005c0: 2d74 6f20 6775 6964 6573 2c20 636f 6e63  -to guides, conc
+000005d0: 6570 7475 616c 2067 7569 6465 732c 2061  eptual guides, a
+000005e0: 6e64 2072 6566 6572 656e 6365 7321 0a0a  nd references!..
+000005f0: 2320 5265 6c65 6173 6520 506c 616e 0a2a  # Release Plan.*
+00000600: 2032 2e35 2e31 0a20 2020 202d 205b 205d   2.5.1.    - [ ]
+00000610: 205b 5374 6162 696c 6974 7920 6973 7375   [Stability issu
+00000620: 6573 2077 6974 6820 7265 7175 6573 7473  es with requests
+00000630: 2074 6f20 7468 6520 7365 6172 6368 2065   to the search e
+00000640: 6e64 706f 696e 7420 6f66 2074 6865 2053  ndpoint of the S
+00000650: 706f 7469 6679 2041 5049 5d28 6874 7470  potify API](http
+00000660: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00000670: 2d72 6963 682f 444a 2d54 6f6f 6c73 2f69  -rich/DJ-Tools/i
+00000680: 7373 7565 732f 3538 290a 2020 2020 2d20  ssues/58).    - 
+00000690: 5b20 5d20 5b4d 616b 6520 5370 6f74 6966  [ ] [Make Spotif
+000006a0: 7920 4150 4920 6361 6c6c 7320 6173 796e  y API calls asyn
+000006b0: 6368 726f 6e6f 7573 5d28 6874 7470 733a  chronous](https:
+000006c0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 2d72  //github.com/a-r
+000006d0: 6963 682f 444a 2d54 6f6f 6c73 2f69 7373  ich/DJ-Tools/iss
+000006e0: 7565 732f 3338 290a 2020 2020 2d20 5b20  ues/38).    - [ 
+000006f0: 5d20 5b50 7269 6e74 2041 5343 4949 2068  ] [Print ASCII h
+00000700: 6973 746f 6772 616d 206f 6620 7461 6720  istogram of tag 
+00000710: 7374 6174 6973 7469 6373 2066 6f72 2043  statistics for C
+00000720: 6f6d 6269 6e65 7220 706c 6179 6c69 7374  ombiner playlist
+00000730: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000740: 622e 636f 6d2f 612d 7269 6368 2f44 4a2d  b.com/a-rich/DJ-
+00000750: 546f 6f6c 732f 6973 7375 6573 2f38 3729  Tools/issues/87)
+00000760: 0a20 2020 202d 205b 785d 205b 4465 7072  .    - [x] [Depr
+00000770: 6563 6174 6520 7265 6769 7374 6572 6564  ecate registered
+00000780: 5f75 7365 7273 2e79 616d 6c5d 2868 7474  _users.yaml](htt
+00000790: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000007a0: 612d 7269 6368 2f44 4a2d 546f 6f6c 732f  a-rich/DJ-Tools/
+000007b0: 6973 7375 6573 2f39 3929 0a20 2020 202d  issues/99).    -
+000007c0: 205b 785d 205b 5061 7261 6d65 7465 7269   [x] [Parameteri
+000007d0: 7a65 2077 6865 7468 6572 2042 6561 7463  ze whether Beatc
+000007e0: 6c6f 7564 2074 7261 636b 7320 7368 6f75  loud tracks shou
+000007f0: 6c64 2062 6520 7265 6164 2061 7320 3c74  ld be read as <t
+00000800: 6974 6c65 3e20 2d20 3c61 7274 6973 743e  itle> - <artist>
+00000810: 206f 7220 7669 6365 2076 6572 7361 5d28   or vice versa](
+00000820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000830: 6f6d 2f61 2d72 6963 682f 444a 2d54 6f6f  om/a-rich/DJ-Too
+00000840: 6c73 2f69 7373 7565 732f 3935 290a 2a20  ls/issues/95).* 
+00000850: 322e 362e 300a 2020 2020 2d20 5b20 5d20  2.6.0.    - [ ] 
+00000860: 5b43 7265 6174 6520 7365 7269 616c 697a  [Create serializ
+00000870: 6572 7320 7061 636b 6167 6520 666f 7220  ers package for 
+00000880: 636f 6e76 6572 7469 6e67 2064 6174 6162  converting datab
+00000890: 6173 6520 6669 6c65 7320 6672 6f6d 206f  ase files from o
+000008a0: 7468 6572 2044 4a20 736f 6674 7761 7265  ther DJ software
+000008b0: 2028 652e 672e 2053 6572 6174 6f2c 2054   (e.g. Serato, T
+000008c0: 7261 6b74 6f72 2c20 4465 6e6f 6e2c 2065  raktor, Denon, e
+000008d0: 7463 2e29 2073 6f20 7468 6174 206f 7065  tc.) so that ope
+000008e0: 7261 7469 6f6e 7320 696e 2074 6865 2072  rations in the r
+000008f0: 656b 6f72 6462 6f78 2070 6163 6b61 6765  ekordbox package
+00000900: 2063 616e 2062 6520 7573 6564 206f 6e20   can be used on 
+00000910: 7468 656d 5d28 6874 7470 733a 2f2f 6769  them](https://gi
+00000920: 7468 7562 2e63 6f6d 2f61 2d72 6963 682f  thub.com/a-rich/
+00000930: 444a 2d54 6f6f 6c73 2f69 7373 7565 732f  DJ-Tools/issues/
+00000940: 3638 290a 2020 2020 2d20 5b20 5d20 5b49  68).    - [ ] [I
+00000950: 6d70 726f 7665 2052 6564 6469 7420 7375  mprove Reddit su
+00000960: 626d 6973 7369 6f6e 2074 6974 6c65 2070  bmission title p
+00000970: 6172 7369 6e67 2069 6e20 6f72 6465 7220  arsing in order 
+00000980: 746f 2069 6d70 726f 7665 2070 7265 6369  to improve preci
+00000990: 7369 6f6e 2061 6e64 2072 6563 616c 6c20  sion and recall 
+000009a0: 6f66 2053 706f 7469 6679 2041 5049 2073  of Spotify API s
+000009b0: 6561 7263 6820 7265 7375 6c74 735d 2868  earch results](h
+000009c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000009d0: 6d2f 612d 7269 6368 2f44 4a2d 546f 6f6c  m/a-rich/DJ-Tool
+000009e0: 732f 6973 7375 6573 2f35 3929 0a0a 2320  s/issues/59)..# 
+000009f0: 436f 6e74 7269 6275 7469 6f6e 0a50 6c65  Contribution.Ple
+00000a00: 6173 6520 7365 6520 7468 6520 5b43 4f4e  ase see the [CON
+00000a10: 5452 4942 5554 494e 475d 2843 4f4e 5452  TRIBUTING](CONTR
+00000a20: 4942 5554 494e 472e 6d64 290a            IBUTING.md).
```

### Comparing `dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 djtools/__main__.py
 djtools/test_main.py
 djtools/configs/__init__.py
 djtools/configs/config.py
 djtools/configs/config.yaml
 djtools/configs/helpers.py
 djtools/configs/logging.conf
-djtools/configs/registered_users.yaml
 djtools/configs/rekordbox_playlists.yaml
 djtools/configs/spotify_playlists.yaml
 djtools/configs/test_config.py
 djtools/configs/test_helpers.py
 djtools/logs/empty.txt
 djtools/rekordbox/__init__.py
 djtools/rekordbox/config.py
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/__init__.py` & `dj_beatcloud-2.5.1b0/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/__main__.py` & `dj_beatcloud-2.5.1b0/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/configs/config.py` & `dj_beatcloud-2.5.1b0/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/configs/config.yaml` & `dj_beatcloud-2.5.1b0/djtools/configs/config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 configs:
-  AWS_PROFILE: 'default'
+  AWS_PROFILE: default
   LOG_LEVEL: INFO
   VERBOSITY: 0
-  XML_PATH: ''
+  XML_PATH: null
 rekordbox:
   BUILD_PLAYLISTS: false
   BUILD_PLAYLISTS_REMAINDER: folder
   COPY_PLAYLISTS: []
-  COPY_PLAYLISTS_DESTINATION: ''
+  COPY_PLAYLISTS_DESTINATION: null
   PURE_GENRE_PLAYLISTS: []
   SHUFFLE_PLAYLISTS: []
 spotify:
   AUTO_PLAYLIST_DEFAULT_LIMIT: 50
   AUTO_PLAYLIST_DEFAULT_PERIOD: week
   AUTO_PLAYLIST_DEFAULT_TYPE: hot
   AUTO_PLAYLIST_FUZZ_RATIO: 70
@@ -23,29 +23,30 @@
   REDDIT_CLIENT_SECRET: ''
   REDDIT_USER_AGENT: ''
   SPOTIFY_CLIENT_ID: ''
   SPOTIFY_CLIENT_SECRET: ''
   SPOTIFY_REDIRECT_URI: ''
   SPOTIFY_USERNAME: ''
 sync:
+  ARTIST_FIRST: false
   AWS_USE_DATE_MODIFIED: false
   DISCORD_URL: ''
   DOWNLOAD_EXCLUDE_DIRS: []
   DOWNLOAD_INCLUDE_DIRS: []
   DOWNLOAD_MUSIC: false
   DOWNLOAD_SPOTIFY: ''
   DOWNLOAD_XML: false
   DRYRUN: false
   IMPORT_USER: ''
   UPLOAD_EXCLUDE_DIRS: []
   UPLOAD_INCLUDE_DIRS: []
   UPLOAD_MUSIC: false
   UPLOAD_XML: false
-  USB_PATH: ''
+  USB_PATH: null
   USER: ''
 utils:
   CHECK_TRACKS: false
   CHECK_TRACKS_FUZZ_RATIO: 80
   CHECK_TRACKS_LOCAL_DIRS: []
   CHECK_TRACKS_SPOTIFY_PLAYLISTS: []
   URL_DOWNLOAD: ''
-  URL_DOWNLOAD_DESTINATION: ''
+  URL_DOWNLOAD_DESTINATION: null
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/configs/helpers.py` & `dj_beatcloud-2.5.1b0/djtools/configs/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,22 @@
     library's configs folder via the --link-configs argument.
 
     Returns:
         argparse.NameSpace: Command-line arguments.
     """
     parser = ArgumentParser()
     parser.add_argument(
+        "--artist-first",
+        action="store_true",
+        help=(
+            "Indicate that Beatcloud tracks are in the format "
+            "`Artist - Track Title` instead of `Track Title - Artist`",
+        ),
+    )
+    parser.add_argument(
         "--auto-playlist-default-limit",
         type=int,
         help="Default number of tracks for a Spotify auto-playlist",
     )
     parser.add_argument(
         "--auto-playlist-default-period",
         type=str,
@@ -179,16 +187,15 @@
         "--dryrun",
         action="store_true",
         help='Show result of "aws s3 sync" command without running it',
     )
     parser.add_argument(
         "--import-user",
         type=str,
-        metavar="Entry of registered_user.yaml",
-        help="Registered USER whose XML_PATH you're downloading",
+        help="USER whose XML_PATH you're downloading",
     )
     parser.add_argument(
         "--link-configs",
         type=convert_to_paths,
         help="Location to symlink library configuration files to",
     )
     parser.add_argument(
@@ -287,16 +294,15 @@
         "--usb-path",
         type=convert_to_paths,
         help="Path to a drive with audio files",
     )
     parser.add_argument(
         "--user",
         type=str,
-        metavar="Entry of registered_user.yaml",
-        help="Entry in registered_users.yaml which maps to your USB_PATH",
+        help="Username of the current user",
     )
     parser.add_argument(
         "--verbosity",
         "-v",
         action="count",
         default=0,
         help="Logging verbosity",
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.5.1b0/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/configs/test_config.py` & `dj_beatcloud-2.5.1b0/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/configs/test_helpers.py` & `dj_beatcloud-2.5.1b0/djtools/configs/test_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,22 +57,14 @@
             f'{link_path} must be a directory that does not already exist'
         ),
     ):
         arg_parse()
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
-@mock.patch(
-    "builtins.open",
-    MockOpen(
-        files=["registered_users.yaml"],
-        user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
-        user_b=("other_user", "/other/USB/"),
-    ).open,
-)
 def test_build_config():
     """Test for the build_config function."""
     with mock.patch(
         "argparse.ArgumentParser.parse_args",
     ) as mock_parse_args:
         mock_parse_args.return_value = Namespace(
             link_configs="", log_level="INFO"
@@ -90,22 +82,14 @@
     caplog.set_level("CRITICAL")
     with pytest.raises(RuntimeError):
         build_config()
     assert 'Error reading "config.yaml"' in caplog.records[0].message
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
-@mock.patch(
-    "builtins.open",
-    MockOpen(
-        files=["registered_users.yaml", "config.yaml"],
-        user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
-        user_b=("test_user", "/test/USB/"),
-    ).open
-)
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_build_config_no_config_yaml(mock_parse_args):
     """Test for the build_config function."""
     mock_parse_args.return_value = Namespace(
         link_configs="", log_level="INFO"
     )
     config_dir = Path(__file__).parent.parent / "configs"
@@ -125,18 +109,14 @@
             assert isinstance(path, Path)
     else:
         assert isinstance(paths, Path)
 
 
 @pytest.mark.parametrize("config", pkg_cfg.values())
 @mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
-@mock.patch(
-    "builtins.open",
-    MockOpen(files=["registered_users.yaml"], write_only=True).open
-)
 def test_filter_dict(config):
     """Test for the filter_dict function."""
     super_config = BaseConfig()
     sub_config = config(**dict(super_config))
     result = filter_dict(sub_config)
     super_keys = set(super_config.dict())
     sub_keys = set(sub_config.dict())
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/config.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_combiner.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/playlist_combiner.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/shuffle_playlists.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_playlist_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Testing for the playlist_builder module."""
-import os
 from pathlib import Path
 
 from bs4 import BeautifulSoup
 import pytest
 import yaml
 
 from djtools.rekordbox.playlist_builder import (
@@ -30,14 +29,15 @@
     )()
 
 
 def test_playlistbuilder_combiner_playlist_contains_new_playlist_selector_tracks(
     test_playlist_config, test_xml, xml
 ):
     """Test for the PlaylistBuilder class."""
+    test_xml = Path(test_xml)
     # Insert test track and Combiner playlist to target it.
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     new_track = xml.new_tag("TRACK")
     new_track_id = "-1"
     new_track.attrs = {
         "TrackID": new_track_id,
@@ -77,18 +77,17 @@
     # Run the PlaylistBuilder (GenreTagParser and Combiner).
     PlaylistBuilder(
         rekordbox_database=Path(test_xml),
         playlist_config=Path(test_playlist_config),
     )()
 
     # Load XML generated by the PlaylistBuilder.
-    path, file_name = os.path.split(test_xml)
-    with open(
-        os.path.join(path, f"auto_{file_name}"), mode="r", encoding="utf-8"
-    ) as _file:
+    path = test_xml.parent
+    file_name = test_xml.name
+    with open(path / f"auto_{file_name}", mode="r", encoding="utf-8") as _file:
         database = BeautifulSoup(_file.read(), "xml")
 
     # Test that the test track was inserted into the "Dubstep" playlist.
     test_track = None
     playlist = database.find_all("NODE", {"Name": "Dubstep", "Type": "1"})[0]
     for track_key in playlist.find_all("TRACK"):
         if track_key["Key"] == new_track_id:
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_shuffle_playlists.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/spotify/__init__.py` & `dj_beatcloud-2.5.1b0/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/spotify/config.py` & `dj_beatcloud-2.5.1b0/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/spotify/helpers.py` & `dj_beatcloud-2.5.1b0/djtools/spotify/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,21 +345,21 @@
     playlist_name: str,
     playlist_ids: Dict[str, str],
     spotify_username: str,
     spotify: spotipy.Spotify,
     tracks: List[Tuple[str]],
     playlist_limit: Optional[int] = sys.maxsize,
     verbosity: Optional[int] = 0,
-):
+) -> Dict[str, str]:
     """Inserts tracks into either a new playlist or an existing one.
 
     Args:
         playlist_name: Name of the playlist.
         playlist_ids: Lookup of playlist IDs.
-        spotify_username: Spotify users's username.
+        spotify_username: Spotify user's username.
         spotify: Spotify client.
         tracks: List of tracks.
         playlist_limit: Maximum number of tracks allowed in a playlist.
         verbosity: Logging verbosity level.
 
     Returns:
         Updated playlist IDs.
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.5.1b0/djtools/spotify/playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,16 @@
             continue
         file_ = Path(line).stem
         try:
             track, artist = file_.strip().split(" - ")
         except ValueError:
             logger.warning(f'{line} is not a valid file')
             continue
+        if config.ARTIST_FIRST:
+            track, artist = artist, track
         files.append((track, artist))
     files = list(filter(lambda x: len(x) == 2, files))
 
     # Query Spotify for files in upload output.
     threshold = config.AUTO_PLAYLIST_FUZZ_RATIO
     tracks = []
     for title, artist in files:
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/spotify/test_config.py` & `dj_beatcloud-2.5.1b0/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.5.1b0/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.5.1b0/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/sync/__init__.py` & `dj_beatcloud-2.5.1b0/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/sync/helpers.py` & `dj_beatcloud-2.5.1b0/djtools/sync/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 """
 from datetime import datetime, timedelta
 from itertools import groupby
 import logging
 from pathlib import Path
 from subprocess import Popen, PIPE, CalledProcessError
 from typing import Optional
+from urllib.parse import quote, unquote
 
 from bs4 import BeautifulSoup
 import requests
-import yaml
 
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -78,41 +78,39 @@
     if config.DRYRUN:
         _cmd.append("--dryrun")
     logger.info(" ".join(_cmd))
 
     return _cmd
 
 
-def rewrite_xml(config: BaseConfig):
+def rewrite_xml(config: BaseConfig, loc_prefix: str = "file://localhost"):
     """This function modifies the "Location" field of track tags in a
         downloaded Rekordbox XML replacing the "USB_PATH" written by
         "IMPORT_USER" with the "USB_PATH" in "config.yaml".
 
     Args:
         config: Configuration object.
+        loc_prefix: Prefix of the `Location` field.
     """
-    registered_users_path = (
-        Path(__file__).parent.parent / "configs" / "registered_users.yaml"
-    )
-
-    with open(registered_users_path, mode="r", encoding="utf-8") as _file:
-        registered_users = yaml.load(_file, Loader=yaml.FullLoader)
-        src = registered_users[config.IMPORT_USER].strip("/")
-        dst = registered_users[config.USER].strip("/")
-
     xml_path = (
         Path(config.XML_PATH).parent / f"{config.IMPORT_USER}_rekordbox.xml"
     )
+    music_path = "DJ Music"
+    usb_path = config.USB_PATH.as_posix().strip("/")
 
     with open(xml_path, mode="r", encoding="utf-8") as _file:
         soup = BeautifulSoup(_file.read(), "xml")
         for track in soup.find_all("TRACK"):
             if not track.get("Location"):
                 continue
-            track["Location"] = track["Location"].replace(src, dst)
+            loc = unquote(track["Location"])
+            common_path = f"{music_path}/{loc.split(music_path + '/')[-1]}"
+            loc = f"{loc_prefix}/{usb_path}/{common_path}"
+            track["Location"] = quote(loc)
+
 
     with open(xml_path, mode="wb", encoding=soup.orignal_encoding) as _file:
         _file.write(soup.prettify("utf-8"))
 
 
 def run_sync(_cmd: str) -> str:
     """Runs subprocess for "aws s3 sync" command. Output is collected and
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/sync/sync_operations.py` & `dj_beatcloud-2.5.1b0/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/sync/test_config.py` & `dj_beatcloud-2.5.1b0/djtools/sync/test_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,38 +2,16 @@
 from unittest import mock
 
 import getpass
 import pytest
 
 
 from djtools.sync.config import SyncConfig
-from djtools.utils.helpers import mock_exists, MockOpen
 
 
-@mock.patch(
-    "builtins.open",
-    MockOpen(
-        files=["registered_users.yaml"],
-        content="bad:\tfile",
-    ).open,
-)
-def test_syncconfig_bad_registered_users():
-    """Test for the SyncConfig class."""
-    with pytest.raises(
-        RuntimeError,
-        match="Error reading registered_users.yaml",
-    ):
-        SyncConfig()
-
-
-@mock.patch(
-    "builtins.open",
-    MockOpen(files=["registered_users.yaml"],
-    write_only=True).open,
-)
 @pytest.mark.parametrize("operations", [(True, False), (False, True)])
 @pytest.mark.parametrize("usb_path", ["", "nonexistent/path"])
 def test_syncconfig_download_or_upload_without_usb_path(operations, usb_path):
     """Test for the SyncConfig class."""
     download, upload = operations
     cfg = {
         "AWS_PROFILE": "myprofile",
@@ -52,21 +30,20 @@
 
 
 def test_syncconfig_download_without_import_user():
     """Test for the SyncConfig class."""
     cfg = {
         "DOWNLOAD_XML": True,
         "AWS_PROFILE": "myprofile",
-        "IMPORT_USER": "not a valid user",
+        "IMPORT_USER": "",
     }
     with pytest.raises(
         RuntimeError,
         match=(
-            "Unable to import from XML of unregistered IMPORT_USER "
-            f'"{cfg["IMPORT_USER"]}"'
+            f'Unable to import from XML of IMPORT_USER "{cfg["IMPORT_USER"]}"'
         ),
     ):
         SyncConfig(**cfg)
 
 
 def test_syncconfig_mutually_exclusive_dirs():
     """Test for the SyncConfig class."""
@@ -88,56 +65,22 @@
     with pytest.raises(
         RuntimeError,
         match="Config must include AWS_PROFILE for sync operations"
     ):
         SyncConfig(**cfg)
 
 
-@mock.patch(
-    "djtools.sync.config.Path.exists",
-    lambda path: mock_exists([("registered_users.yaml", False)], path)
-)
-@mock.patch(
-    "builtins.open",
-    MockOpen(files=["registered_users.yaml"],
-    write_only=True).open,
-)
-@mock.patch("djtools.spotify.helpers.get_spotify_client", mock.MagicMock())
-def test_syncconfig_no_registered_users(test_xml, caplog):
-    """Test for the SyncConfig class."""
-    cfg = {
-        "XML_PATH": test_xml,
-        "SPOTIFY_CLIENT_ID": "id",
-        "SPOTIFY_CLIENT_SECRET": "secret",
-        "SPOTIFY_REDIRECT_URI": "uri",
-        "SPOTIFY_USERNAME": "name",
-    }
-    caplog.set_level("WARNING")
-    SyncConfig(**cfg)
-    assert caplog.records[0].message == "No registered users!"
-
-
-@mock.patch(
-    "builtins.open",
-    MockOpen(files=["registered_users.yaml"],
-    write_only=True).open,
-)
 def test_syncconfig_set_user():
     """Test for the SyncConfig class."""
     cfg = {"USER": ""}
     assert not SyncConfig.__fields__["USER"].default
     sync_config = SyncConfig(**cfg)
     assert sync_config.USER == getpass.getuser()
 
 
-@mock.patch(
-    "builtins.open",
-    MockOpen(files=["registered_users.yaml"],
-    write_only=True).open,
-)
 @mock.patch("djtools.spotify.helpers.get_spotify_client", mock.MagicMock())
 def test_syncconfig_upload_without_discord_url(test_xml, caplog):
     """Test for the SyncConfig class."""
     caplog.set_level("WARNING")
     cfg = {
         "USB_PATH": ".",
         "UPLOAD_MUSIC": True,
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/sync/test_helpers.py` & `dj_beatcloud-2.5.1b0/djtools/sync/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Testing for the helpers module."""
 from datetime import datetime, timedelta
 import os
 from pathlib import Path
 import tempfile
 from unittest import mock
+from urllib.parse import unquote
 
 from bs4 import BeautifulSoup
 import pytest
 
 from djtools.sync.helpers import (
     parse_sync_command, rewrite_xml, run_sync, upload_log, webhook
 )
-from djtools.utils.helpers import MockOpen
 
 
 @pytest.mark.parametrize("upload", [True, False])
 @pytest.mark.parametrize(
     "include_dirs", [[], ["path/to/stuff", "path/to/things.mp3"]]
 )
 @pytest.mark.parametrize(
@@ -59,61 +59,54 @@
         assert "--include *" in cmd
     if use_date_modified:
         assert "--size-only" in cmd
     if dryrun:
         assert "--dryrun" in cmd
 
 
-@mock.patch(
-    "builtins.open",
-    MockOpen(
-        files=["registered_users.yaml"],
-        user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
-        user_b=("other_user", "/Volumes/my_beat_stick/"),
-    ).open
-)
 def test_rewrite_xml(test_config, test_xml, xml):
     """Test for the rewrite_xml function."""
     user_a_path= "/Volumes/AWEEEEZY/"
     user_b_path= "/Volumes/my_beat_stick/"
     test_user = "aweeeezy"
     other_user = "other_user"
     test_config.USER = test_user
     test_config.IMPORT_USER = other_user
     test_config.XML_PATH = test_xml
+    test_config.USB_PATH = Path("/Volumes/AWEEEEZY/")
     other_users_xml = Path(test_xml).parent / f"{other_user}_rekordbox.xml"
     other_users_xml.write_text(
         Path(test_xml).read_text(encoding="utf-8"), encoding="utf-8"
     )
 
     for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
         # NOTE(a-rich): `Location` attributes in the XML's `TRACK` tags always
         # have unix-style paths so paths created in Windows must be
         # interpreted `.as_posix()`.
         track["Location"] = (
             Path(track["Location"]).parent / user_b_path.strip("/") /
-            Path(track["Location"]).name
+            "DJ Music" / Path(track["Location"]).name
         ).as_posix()
 
     with open(
-        other_users_xml, mode="wb", encoding=xml.orignal_encoding
+        other_users_xml, mode="wb", encoding=xml.original_encoding
     ) as _file:
         _file.write(xml.prettify("utf-8"))
 
     rewrite_xml(test_config)
 
     with open(other_users_xml, mode="r", encoding="utf-8") as _file:
         soup = BeautifulSoup(_file.read(), "xml")
         for track in soup.find_all("TRACK"):
             if not track.get("Location"):
                 continue
-            assert user_a_path in track["Location"]
-            assert user_b_path not in track["Location"]
+            assert user_a_path in unquote(track["Location"])
+            assert user_b_path not in unquote(track["Location"])
 
 
 @mock.patch("djtools.sync.helpers.Popen")
 def test_run_sync(mock_popen, tmpdir):
     """Test for the run_sync function."""
     with open(Path(tmpdir) / "track.mp3", mode="w", encoding="utf-8") as _file:
         _file.write("")
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.5.1b0/djtools/sync/test_sync_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from unittest import mock
 
 import pytest
 
 from djtools.sync.sync_operations import (
     download_music, download_xml, upload_music, upload_xml
 )
-from djtools.utils.helpers import MockOpen
 
 
 @pytest.mark.parametrize("playlist_name", ["", "playlist Uploads"])
 @mock.patch(
     "djtools.sync.sync_operations.compare_tracks",
     mock.Mock(
         return_value=(
@@ -50,22 +49,14 @@
     assert caplog.records[0].message == "Found 0 files"
     assert caplog.records[1].message == "Syncing remote track collection..."
     assert caplog.records[2].message == " ".join(cmd)
     assert caplog.records[3].message == "Found 1 new files"
     assert Path(caplog.records[4].message).name == "file.mp3"
 
 
-@mock.patch(
-    "builtins.open", 
-    MockOpen(
-        files=["registered_users.yaml"],
-        user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
-        user_b=("test_user", "/test/USB/"),
-    ).open,
-)
 @mock.patch("djtools.sync.sync_operations.rewrite_xml")
 @mock.patch("subprocess.Popen.wait", mock.Mock())
 def test_download_xml(mock_rewrite_xml, test_config, test_xml, caplog):
     """Test for the download_xml function."""
     caplog.set_level("INFO")
     test_user = "test_user"
     other_user = "aweeeezy"
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/test_main.py` & `dj_beatcloud-2.5.1b0/djtools/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 """Testing the main entrypoint for the djtools library."""
 from argparse import Namespace
 from unittest import mock
 
 from djtools import main
-from djtools.utils.helpers import MockOpen
 
 
-@mock.patch(
-    "builtins.open",
-    MockOpen(files=["registered_users.yaml"], write_only=True).open
-)
 @mock.patch("djtools.upload_log", mock.Mock())
 @mock.patch("djtools.UTILS_OPERATIONS")
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_main(mock_parse_args, mock_utils_operations):
     """Test for the main function."""
     mock_ops = {
         "CHECK_TRACKS": lambda x, beatcloud_tracks=[]: None,
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/utils/__init__.py` & `dj_beatcloud-2.5.1b0/djtools/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,25 +4,23 @@
     * `config`: the configuration object for the `utils` package
     * `helpers`: helper functions for the `utils` package and the `djtools`
         library in general
     * `url_download`: download tracks from a URL (e.g. Soundcloud playlist).
 """
 from djtools.utils.config import UtilsConfig
 from djtools.utils.check_tracks import compare_tracks
-from djtools.utils.helpers import initialize_logger, mock_exists, MockOpen
+from djtools.utils.helpers import initialize_logger
 from djtools.utils.url_download import url_download
 
 
 UTILS_OPERATIONS = {
     "CHECK_TRACKS": compare_tracks,
     "URL_DOWNLOAD": url_download,
 }
 
 __all__ = (
     "compare_tracks",
     "initialize_logger",
-    "mock_exists",
-    "MockOpen",
     "url_download",
     "UtilsConfig",
     "UTILS_OPERATIONS",
 )
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/utils/check_tracks.py` & `dj_beatcloud-2.5.1b0/djtools/utils/check_tracks.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from itertools import groupby
 import logging
 from operator import itemgetter
 from typing import List, Optional, Tuple
 
 from djtools.configs.config import BaseConfig
 from djtools.utils.helpers import (
-    find_matches, get_spotify_tracks, get_beatcloud_tracks, get_local_tracks
+    find_matches,
+    get_spotify_tracks,
+    get_beatcloud_tracks,
+    get_local_tracks,
+    reverse_title_and_artist,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 def compare_tracks(
@@ -69,14 +73,16 @@
 
     if not beatcloud_tracks:
         beatcloud_tracks = get_beatcloud_tracks()
 
     path_lookup = {x.stem: x for x in beatcloud_tracks}
 
     for tracks, track_type in track_sets:
+        if config.ARTIST_FIRST and track_type == "Local Directory Tracks":
+            path_lookup = reverse_title_and_artist(path_lookup)
         matches = find_matches(
             tracks,
             path_lookup.keys(),
             config,
         )
         logger.info(f"\n{track_type} / Beatcloud Matches: {len(matches)}")
         for loc, matches in groupby(
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/utils/config.py` & `dj_beatcloud-2.5.1b0/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/utils/helpers.py` & `dj_beatcloud-2.5.1b0/djtools/utils/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from itertools import product
 import logging
 import logging.config
 import os
 from pathlib import Path
 from subprocess import check_output
 import tempfile
-from typing import Any, Dict, List, Optional, Set, Tuple
+from typing import Any, Dict, IO, List, Optional, Set, Tuple
 from unittest import mock
 
 from fuzzywuzzy import fuzz
 import spotipy
 from tqdm import tqdm
 
 from djtools.configs.config import BaseConfig
@@ -38,64 +38,59 @@
     ):
         self._user_a = user_a
         self._user_b = user_b
         self._files = files
         self._content = content
         self._write_only = write_only
 
-    def open(self, *args, **kwargs):
+    def open(self, *args, **kwargs) -> IO:
         """Function to replace the builtin open function.
 
         Returns:
             File handler.
         """
-        file_name = os.path.basename(args[0])
+        file_name = Path(args[0]).name
         if file_name in self._files:
             if "w" in kwargs.get("mode"):
                 return tempfile.TemporaryFile(mode=kwargs["mode"])
             if not self._write_only:
                 return self._file_strategy(file_name, *args, **kwargs)
         return self.builtin_open(*args, **kwargs)
 
-    def _file_strategy(self, file_name, *args, **kwargs):
+    def _file_strategy(self, *args, **kwargs):
         """Apply logic for file contents based on file name.
 
-        Args:
-            file_name: Name of the file to open.
-
         Returns:
             Mock file handler object.
         """
         data = "{}"
         if self._content:
             data = self._content
-        elif file_name == "registered_users.yaml":
-            data = (
-                f'{{"{self._user_a[0]}": "{self._user_a[1]}", '
-                f'"{self._user_b[0]}": "{self._user_b[1]}"}}'
-            )
 
         return mock.mock_open(read_data=data)(*args, **kwargs)
 
 
-def add_tracks(result: Dict[str, Any]) -> List[str]:
+def add_tracks(result: Dict[str, Any], artist_first: bool) -> List[str]:
     """Parses a page of Spotify API result tracks and returns a list of the
         track titles and artist names.
 
     Args:
         result: Paged result of Spotify tracks.
+        artist_first: Whether or not artist should come before track title.
 
     Returns:
         Spotify track titles and artist names.
     """
     tracks = []
     for track in result["items"]:
         title = track["track"]["name"]
         artists = ", ".join([y["name"] for y in track["track"]["artists"]])
-        tracks.append(f"{title} - {artists}")
+        tracks.append(
+            f"{artists} - {title}" if artist_first else f"{title} - {artists}"
+        )
 
     return tracks
 
 
 def compute_distance(
     spotify_playlist: str,
     spotify_track: str,
@@ -208,21 +203,22 @@
     local_tracks_count = sum(len(x) for x in local_dir_tracks.values())
     logger.info(f"Got {local_tracks_count} files under local directories")
 
     return local_dir_tracks
 
 
 def get_playlist_tracks(
-    spotify: spotipy.Spotify, playlist_id: str
+    spotify: spotipy.Spotify, playlist_id: str, artist_first: bool
 ) -> Set[str]:
     """Queries Spotify API for a playlist and pulls tracks from it.
 
     Args:
         spotify: Spotify client.
         playlist_id: Playlist ID of Spotify playlist to pull tracks from.
+        artist_first: Whether or not artist should come before track title.
 
     Raises:
         RuntimeError: Playlist_id must correspond with a valid Spotify playlist.
 
     Returns:
         Spotify track titles and artist names from a given playlist.
     """
@@ -230,19 +226,19 @@
         playlist = spotify.playlist(playlist_id)
     except Exception:
         raise RuntimeError(
             f"Failed to get playlist with ID {playlist_id}"
         ) from Exception
 
     result = playlist["tracks"]
-    tracks = add_tracks(result)
+    tracks = add_tracks(result, artist_first)
 
     while result["next"]:
         result = spotify.next(result)
-        tracks.extend(add_tracks(result))
+        tracks.extend(add_tracks(result, artist_first))
 
     return set(tracks)
 
 
 def get_spotify_tracks(config: BaseConfig) -> Dict[str, Set[str]]:
     """Aggregates the tracks from one or more Spotify playlists into a
         dictionary mapped with playlist names.
@@ -260,26 +256,30 @@
     _sum = 0
     for playlist in config.CHECK_TRACKS_SPOTIFY_PLAYLISTS:
         playlist_id = playlist_ids.get(playlist)
         if not playlist_id:
             logger.error(f"{playlist} not in spotify_playlists.yaml")
             continue
 
-        playlist_tracks[playlist] = get_playlist_tracks(spotify, playlist_id)
+        playlist_tracks[playlist] = get_playlist_tracks(
+            spotify, playlist_id, config.ARTIST_FIRST
+        )
         length = len(playlist_tracks[playlist])
         logger.info(
             f'Got {length} track{"" if length == 1 else "s"} from Spotify '
             f'playlist "{playlist}"'
         )
         _sum += length
 
         if config.VERBOSITY > 0:
             for track in playlist_tracks[playlist]:
                 logger.info(f"\t{track}")
-    logger.info(f"Got {_sum} tracks from Spotify in total")
+    logger.info(
+        f'Got {_sum} track{"" if _sum == 1 else "s"} from Spotify in total'
+    )
 
     return playlist_tracks
 
 
 def initialize_logger() -> Tuple[logging.Logger, str]:
     """Initializes logger from configuration.
 
@@ -305,7 +305,24 @@
     """Function for mocking the existence of pathlib.Path object."""
     ret = True
     for file_name, exists in files:
         if file_name == path.name:
             ret = exists
             break
     return ret
+
+
+def reverse_title_and_artist(path_lookup: Dict[str, str]) -> Dict[str, str]:
+    """Reverses the title and artist parts of the filename.
+
+    Args:
+        path_lookup: Mapping of filenames to file paths.
+
+    Returns:
+        Mapping with the title and artist in the filenames reversed.
+    """
+    new_path_lookup = {}
+    for key, value in path_lookup.items():
+        title, artist = key.split(" - ")
+        new_path_lookup[f"{artist} - {title}"] = value
+
+    return new_path_lookup
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/utils/test_helpers.py` & `dj_beatcloud-2.5.1b0/djtools/utils/test_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     find_matches,
     get_beatcloud_tracks,
     get_local_tracks,
     get_playlist_tracks,
     get_spotify_tracks,
     initialize_logger,
     MockOpen,
+    reverse_title_and_artist,
 )
 
 
 def test_add_tracks():
     """Test for the add_tracks function."""
     test_input = {
         "items": [
@@ -42,18 +43,31 @@
             },
         ],
     }
     expected = [
         "track title - artist name",
         "another track title - another artist name, a second artist name"
     ]
-    output = add_tracks(test_input)
+    output = add_tracks(test_input, False)
     assert output == expected
 
 
+def test_add_tracks_with_reverse_title_and_artist():
+    """Test for the add_tracks function."""
+    test_input = {
+        "items": [
+            {"track": {"name": "title", "artists": [{"name": "artist"}]}},
+        ],
+    }
+    expected = ["artist - title"]
+    output = add_tracks(test_input, True)
+    assert output == expected
+
+
+
 @pytest.mark.parametrize("track_a", ["some track", "another track"])
 @pytest.mark.parametrize("track_b", ["some track", "another track"])
 def test_compute_distance(track_a, track_b):
     """Test for the compute_distance function."""
     ret = compute_distance(
         "playlist",
         track_a,
@@ -203,15 +217,15 @@
     mock_spotipy.playlist.return_value = mock_spotipy_playlist.return_value
     mock_spotipy.next.return_value = mock_spotipy_next.return_value
     expected = sorted(set([
         "track title - artist name",
         "another track title - another artist name, a second artist name",
         "last track title - final artist name"
     ]))
-    tracks = sorted(get_playlist_tracks(mock_spotipy, "some ID"))
+    tracks = sorted(get_playlist_tracks(mock_spotipy, "some ID", False))
     assert tracks == expected
 
 
 @mock.patch("djtools.spotify.helpers.spotipy.Spotify")
 @mock.patch(
     "djtools.spotify.helpers.spotipy.Spotify.playlist",
     side_effect=Exception()
@@ -221,15 +235,15 @@
 ):
     """Test for the get_playlist_tracks function."""
     test_playlist_id = "some ID"
     mock_spotipy.playlist.side_effect = mock_spotipy_playlist.side_effect
     with pytest.raises(
         Exception, match=f"Failed to get playlist with ID {test_playlist_id}"
     ):
-        get_playlist_tracks(mock_spotipy, test_playlist_id)
+        get_playlist_tracks(mock_spotipy, test_playlist_id, False)
 
 
 @pytest.mark.parametrize("verbosity", [0, 1])
 @mock.patch("builtins.open", MockOpen(
     files=["spotify_playlists.yaml"],
     content='{"r/techno | Top weekly Posts": "5gex4eBgWH9nieoVuV8hDC"}',
 ).open)
@@ -264,7 +278,15 @@
 
 def test_initialize_logger():
     """Test for the intitialize_logger function."""
     today = f'{datetime.now().strftime("%Y-%m-%d")}.log'
     logger, log_file = initialize_logger()
     assert isinstance(logger, logging.Logger)
     assert log_file.name == today
+
+
+def test_reverse_title_and_artist():
+    """Test for the reverse_title_and_artist function."""
+    path_lookup = {"title - artist": "path/to/title - artist.mp3"}
+    expected = {"artist - title": "path/to/title - artist.mp3"}
+    new_path_lookup = reverse_title_and_artist(path_lookup)
+    assert new_path_lookup == expected
```

### Comparing `dj_beatcloud-2.5.0b0/djtools/utils/test_url_download.py` & `dj_beatcloud-2.5.1b0/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/djtools/utils/url_download.py` & `dj_beatcloud-2.5.1b0/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.0b0/setup.py` & `dj_beatcloud-2.5.1b0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Setup 'djtools' package.
 """
-from setuptools import find_packages, setup
+from setuptools import setup
 
 
 with open('README.md', encoding='utf-8') as _file:
     LONG_DESCRIPTION = _file.read()
 
 REQUIREMENTS = [
     "asyncpraw==7.6.1",
@@ -44,15 +44,15 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.5.0b0',
+    version='2.5.1-b0',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
```

