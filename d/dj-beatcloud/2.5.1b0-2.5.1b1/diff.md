# Comparing `tmp/dj_beatcloud-2.5.1b0.tar.gz` & `tmp/dj_beatcloud-2.5.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.5.1b0.tar", last modified: Sat May  6 19:50:41 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.5.1b1.tar", last modified: Sat May  6 20:08:51 2023, max compression
```

## Comparing `dj_beatcloud-2.5.1b0.tar` & `dj_beatcloud-2.5.1b1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.315897 dj_beatcloud-2.5.1b0/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b0/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-06 19:50:41.315988 dj_beatcloud-2.5.1b0/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.307611 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1834 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-06 19:50:41.000000 dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.308259 dj_beatcloud-2.5.1b0/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2462 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b0/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.310030 dj_beatcloud-2.5.1b0/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2815 2023-05-06 19:49:39.000000 dj_beatcloud-2.5.1b0/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1241 2023-05-06 19:49:01.000000 dj_beatcloud-2.5.1b0/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13540 2023-05-06 19:49:38.000000 dj_beatcloud-2.5.1b0/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4504 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.310227 dj_beatcloud-2.5.1b0/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.312301 dj_beatcloud-2.5.1b0/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/playlist_combiner.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5338 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.313394 dj_beatcloud-2.5.1b0/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2151 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.314426 dj_beatcloud-2.5.1b0/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b0/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      733 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 19:50:41.315765 dj_beatcloud-2.5.1b0/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10100 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b0/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b0/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-06 19:50:41.316388 dj_beatcloud-2.5.1b0/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2209 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b0/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.935846 dj_beatcloud-2.5.1b1/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b1/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-06 20:08:51.935941 dj_beatcloud-2.5.1b1/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.923934 dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-06 20:08:51.000000 dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1834 2023-05-06 20:08:51.000000 dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-06 20:08:51.000000 dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-06 20:08:51.000000 dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-06 20:08:51.000000 dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-06 20:08:51.000000 dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.924827 dj_beatcloud-2.5.1b1/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2462 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b1/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.927141 dj_beatcloud-2.5.1b1/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2815 2023-05-06 19:49:39.000000 dj_beatcloud-2.5.1b1/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1241 2023-05-06 19:49:01.000000 dj_beatcloud-2.5.1b1/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13540 2023-05-06 19:49:38.000000 dj_beatcloud-2.5.1b1/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4504 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.927437 dj_beatcloud-2.5.1b1/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.930310 dj_beatcloud-2.5.1b1/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/playlist_combiner.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5338 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/test_shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.931949 dj_beatcloud-2.5.1b1/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2151 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.933732 dj_beatcloud-2.5.1b1/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b1/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      733 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-06 20:08:51.935640 dj_beatcloud-2.5.1b1/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-05-06 20:05:15.000000 dj_beatcloud-2.5.1b1/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-05-06 19:43:14.000000 dj_beatcloud-2.5.1b1/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b1/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b1/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-06 20:08:51.936246 dj_beatcloud-2.5.1b1/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2209 2023-05-06 20:02:57.000000 dj_beatcloud-2.5.1b1/setup.py
```

### Comparing `dj_beatcloud-2.5.1b0/LICENSE` & `dj_beatcloud-2.5.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/PKG-INFO` & `dj_beatcloud-2.5.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.5.1b0
+Version: 2.5.1b1
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b0 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b1 Summary: DJ Tools is
 a library for managing a collection of music and Rekordbox XML files. Home-
 page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
 alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
 spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
```

### Comparing `dj_beatcloud-2.5.1b0/README.md` & `dj_beatcloud-2.5.1b1/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.5.1b0
+Version: 2.5.1b1
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b0 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b1 Summary: DJ Tools is
 a library for managing a collection of music and Rekordbox XML files. Home-
 page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
 alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
 spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
```

### Comparing `dj_beatcloud-2.5.1b0/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.5.1b1/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/__init__.py` & `dj_beatcloud-2.5.1b1/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/__main__.py` & `dj_beatcloud-2.5.1b1/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/configs/config.py` & `dj_beatcloud-2.5.1b1/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/configs/config.yaml` & `dj_beatcloud-2.5.1b1/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/configs/helpers.py` & `dj_beatcloud-2.5.1b1/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.5.1b1/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/configs/test_config.py` & `dj_beatcloud-2.5.1b1/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/configs/test_helpers.py` & `dj_beatcloud-2.5.1b1/djtools/configs/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/config.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/playlist_combiner.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/playlist_combiner.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/shuffle_playlists.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_shuffle_playlists.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/test_shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.5.1b1/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/spotify/__init__.py` & `dj_beatcloud-2.5.1b1/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/spotify/config.py` & `dj_beatcloud-2.5.1b1/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/spotify/helpers.py` & `dj_beatcloud-2.5.1b1/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.5.1b1/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/spotify/test_config.py` & `dj_beatcloud-2.5.1b1/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.5.1b1/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.5.1b1/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/sync/__init__.py` & `dj_beatcloud-2.5.1b1/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/sync/config.py` & `dj_beatcloud-2.5.1b1/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/sync/helpers.py` & `dj_beatcloud-2.5.1b1/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/sync/sync_operations.py` & `dj_beatcloud-2.5.1b1/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/sync/test_config.py` & `dj_beatcloud-2.5.1b1/djtools/sync/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/sync/test_helpers.py` & `dj_beatcloud-2.5.1b1/djtools/sync/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.5.1b1/djtools/sync/test_sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/test_main.py` & `dj_beatcloud-2.5.1b1/djtools/test_main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/utils/__init__.py` & `dj_beatcloud-2.5.1b1/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/utils/check_tracks.py` & `dj_beatcloud-2.5.1b1/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/utils/config.py` & `dj_beatcloud-2.5.1b1/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/utils/helpers.py` & `dj_beatcloud-2.5.1b1/djtools/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,11 +318,13 @@
         path_lookup: Mapping of filenames to file paths.
 
     Returns:
         Mapping with the title and artist in the filenames reversed.
     """
     new_path_lookup = {}
     for key, value in path_lookup.items():
-        title, artist = key.split(" - ")
+        split = key.split(" - ")
+        title = " - ".join(split[:-1])
+        artist = split[-1]
         new_path_lookup[f"{artist} - {title}"] = value
 
     return new_path_lookup
```

### Comparing `dj_beatcloud-2.5.1b0/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.5.1b1/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/utils/test_helpers.py` & `dj_beatcloud-2.5.1b1/djtools/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/utils/test_url_download.py` & `dj_beatcloud-2.5.1b1/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/djtools/utils/url_download.py` & `dj_beatcloud-2.5.1b1/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b0/setup.py` & `dj_beatcloud-2.5.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.5.1-b0',
+    version='2.5.1-b1',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
```

