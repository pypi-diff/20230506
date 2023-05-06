# Comparing `tmp/py-Ayra-8.7.3.tar.gz` & `tmp/py-Ayra-8.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayra-8.7.3.tar", last modified: Sat May  6 08:10:51 2023, max compression
+gzip compressed data, was "py-Ayra-8.7.4.tar", last modified: Sat May  6 19:01:17 2023, max compression
```

## Comparing `py-Ayra-8.7.3.tar` & `py-Ayra-8.7.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 08:10:51.459558 py-Ayra-8.7.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 08:10:51.451557 py-Ayra-8.7.3/Ayra/
--rw-r--r--   0 root         (0) root         (0)     2984 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 08:10:51.455558 py-Ayra-8.7.3/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12369 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-05-06 06:05:13.000000 py-Ayra-8.7.3/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 08:10:51.459558 py-Ayra-8.7.3/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     2038 2023-05-06 08:10:27.000000 py-Ayra-8.7.3/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 08:10:51.459558 py-Ayra-8.7.3/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    19939 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17343 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28822 2023-05-03 20:26:34.000000 py-Ayra-8.7.3/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 08:10:51.459558 py-Ayra-8.7.3/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18377 2023-05-03 17:10:02.000000 py-Ayra-8.7.3/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-06 08:10:27.000000 py-Ayra-8.7.3/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3387 2023-05-06 08:10:51.459558 py-Ayra-8.7.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 08:10:51.459558 py-Ayra-8.7.3/py_Ayra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3387 2023-05-06 08:10:51.000000 py-Ayra-8.7.3/py_Ayra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1466 2023-05-06 08:10:51.000000 py-Ayra-8.7.3/py_Ayra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 08:10:51.000000 py-Ayra-8.7.3/py_Ayra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 08:10:51.000000 py-Ayra-8.7.3/py_Ayra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-06 08:10:51.000000 py-Ayra-8.7.3/py_Ayra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 08:10:51.463559 py-Ayra-8.7.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-03 16:58:28.000000 py-Ayra-8.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:01:17.150447 py-Ayra-8.7.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:01:17.142446 py-Ayra-8.7.4/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:01:17.142446 py-Ayra-8.7.4/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12369 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-05-06 06:05:13.000000 py-Ayra-8.7.4/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:01:17.146446 py-Ayra-8.7.4/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     1962 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:01:17.146446 py-Ayra-8.7.4/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    19988 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17343 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28822 2023-05-03 20:26:34.000000 py-Ayra-8.7.4/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:01:17.150447 py-Ayra-8.7.4/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18378 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-06 19:00:55.000000 py-Ayra-8.7.4/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-05-06 19:01:17.150447 py-Ayra-8.7.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:01:17.150447 py-Ayra-8.7.4/py_Ayra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-05-06 19:01:17.000000 py-Ayra-8.7.4/py_Ayra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-05-06 19:01:17.000000 py-Ayra-8.7.4/py_Ayra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 19:01:17.000000 py-Ayra-8.7.4/py_Ayra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 19:01:17.000000 py-Ayra-8.7.4/py_Ayra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-06 19:01:17.000000 py-Ayra-8.7.4/py_Ayra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 19:01:17.150447 py-Ayra-8.7.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-03 16:58:28.000000 py-Ayra-8.7.4/setup.py
```

### Comparing `py-Ayra-8.7.3/Ayra/__init__.py` & `py-Ayra-8.7.4/Ayra/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
             sys.exit()
     else:
         ayra_bot = AyraClient(
             validate_session(Var.SESSION, LOGS),
             udB=udB,
             app_version=ayra_version,
-            device_model="Ayra",
+            device_model="Naya-Userbot",
         )
         ayra_bot.run_in_loop(autobot())
 
     asst = AyraClient(None, bot_token=udB.get_key("BOT_TOKEN"), udB=udB)
 
     if BOT_MODE:
         ayra_bot = asst
@@ -92,14 +92,14 @@
     SUDOS = udB.get_key("SUDOS") or "1054295664"
     VC_SUDOS = udB.get_key("VC_SUDOS") or "1054295664"
     DUAL_HNDLR = udB.get_key("DUAL_HNDLR") or "/"
     SUDO_HNDLR = udB.get_key("SUDO_HNDLR") or "$"
     INLINE_PM = udB.set_key("INLINE_PM", "True")
     PMLOG = udB.set_key("PMLOG", "True")
 else:
-    print("Ayra 2022 © senpai80")
+    print("Naya-Userbot © @Rizzvbss")
 
     from logging import getLogger
 
-    LOGS = getLogger("Ayra")
+    LOGS = getLogger("Naya-Userbot")
 
     ayra_bot = asst = udB = vcClient = None
```

### Comparing `py-Ayra-8.7.3/Ayra/__main__.py` & `py-Ayra-8.7.4/Ayra/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,17 +60,17 @@
     ) is None:
         _plugins = "autocorrect autopic audiotools compressor forcesubscribe fedutils gdrive glitch instagram nsfwfilter nightmode pdftools profanityfilter writer youtube"
         udB.set_key("EXCLUDE_OFFICIAL", _plugins)
 
     load_other_plugins(addons=addons, pmbot=pmbot, manager=manager, vcbot=vcbot)
 
     suc_msg = """
-            ----------------------------------------------------------------------
-                                      ◈ ᴀʏʀᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ​ ◈
-            ----------------------------------------------------------------------
+  -------------------------------------------------------
+                      иᴀʏᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ
+  -------------------------------------------------------
     """
 
     # for channel plugins
     plugin_channels = udB.get_key("PLUGIN_CHANNEL")
 
     # Customize ayra Assistant...
     ayra_bot.run_in_loop(customize())
@@ -88,15 +88,15 @@
 
     try:
         cleanup_cache()
     except BaseException:
         pass
 
     LOGS.info(
-        f"Took {time_formatter((time.time() - start_time)*1000)} to start ◈ ᴀʏʀᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ​ ◈"
+        f"Took {time_formatter((time.time() - start_time)*1000)} to start иᴀʏᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ"
     )
     LOGS.info(suc_msg)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `py-Ayra-8.7.3/Ayra/_misc/__init__.py` & `py-Ayra-8.7.4/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/_misc/_assistant.py` & `py-Ayra-8.7.4/Ayra/_misc/_assistant.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 from .. import LOGS, asst, udB, ayra_bot
 from ..fns.admins import admin_check
 from . import append_or_update, owner_and_sudos
 
 OWNER = ayra_bot.full_name
 
 MSG = f"""
-**ᴀʏʀᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ​**
+**иᴀʏᴀ ꭙ ᴜꜱᴇʀʙᴏᴛ**
 ╼┅━━━━━━━━━━╍━━━━━━━━━━┅╾
 **Owner**: [{OWNER}](tg://user?id={ayra_bot.uid})
 **Support**: @KynanSupport
 ╼┅━━━━━━━━━━╍━━━━━━━━━━┅╾
 """
 
 IN_BTTS = [
     [
         Button.url(
             "Repository",
-            url="https://github.com/naya1503/ayra",
+            url="https://github.com/naya1503/Naya-Userbot",
         ),
         Button.url("Support", url="https://t.me/kynansupport"),
     ]
 ]
 
 
 # decorator for assistant
```

### Comparing `py-Ayra-8.7.3/Ayra/_misc/_decorators.py` & `py-Ayra-8.7.4/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/_misc/_supporter.py` & `py-Ayra-8.7.4/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/_misc/_wrappers.py` & `py-Ayra-8.7.4/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/configs.py` & `py-Ayra-8.7.4/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/__init__.py` & `py-Ayra-8.7.4/Ayra/dB/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,15 @@
     993270486, #rama2
     1488093812, #vicky2
     1936017380,  #otan
 ]
 
 DEFAULT = list(map(int, b64decode("MTA1NDI5NTY2NA==").split()))
 
-AYRA_IMAGES = [
-    f"https://graph.org/file/{_}.jpg"
-    for _ in [
-        "a51b51ca8a7cc5327fd42",
-        "02f9ca4617cec58377b9d",
-    ]
-]
+AYRA_IMAGES = ["https://graph.org/file/60408fea8439e6702674d.jpg"]
 
 stickers = [
     "CAADAQADeAIAAm_BZBQh8owdViocCAI",
     "CAADAQADegIAAm_BZBQ6j8GpKtnrSgI",
     "CAADAQADfAIAAm_BZBQpqC84n9JNXgI",
     "CAADAQADfgIAAm_BZBSxLmTyuHvlzgI",
     "CAADAQADgAIAAm_BZBQ3TZaueMkS-gI",
```

### Comparing `py-Ayra-8.7.3/Ayra/dB/afk_db.py` & `py-Ayra-8.7.4/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/antiflood_db.py` & `py-Ayra-8.7.4/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/asst_fns.py` & `py-Ayra-8.7.4/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/asstcmd_db.py` & `py-Ayra-8.7.4/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/autoban_db.py` & `py-Ayra-8.7.4/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/blacklist_db.py` & `py-Ayra-8.7.4/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/botchat_db.py` & `py-Ayra-8.7.4/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/broadcast_db.py` & `py-Ayra-8.7.4/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/ch_db.py` & `py-Ayra-8.7.4/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/dnd_db.py` & `py-Ayra-8.7.4/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/echo_db.py` & `py-Ayra-8.7.4/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/filestore_db.py` & `py-Ayra-8.7.4/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/filter_db.py` & `py-Ayra-8.7.4/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/forcesub_db.py` & `py-Ayra-8.7.4/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/gban_mute_db.py` & `py-Ayra-8.7.4/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/gcast_blacklist_db.py` & `py-Ayra-8.7.4/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/greetings_db.py` & `py-Ayra-8.7.4/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/logusers_db.py` & `py-Ayra-8.7.4/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/mute_db.py` & `py-Ayra-8.7.4/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/night_db.py` & `py-Ayra-8.7.4/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/notes_db.py` & `py-Ayra-8.7.4/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/nsfw_db.py` & `py-Ayra-8.7.4/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/pmpermit_db.py` & `py-Ayra-8.7.4/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/snips_db.py` & `py-Ayra-8.7.4/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/vc_sudos.py` & `py-Ayra-8.7.4/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/dB/warn_db.py` & `py-Ayra-8.7.4/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/FastTelethon.py` & `py-Ayra-8.7.4/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/__init__.py` & `py-Ayra-8.7.4/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/admins.py` & `py-Ayra-8.7.4/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/executor.py` & `py-Ayra-8.7.4/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/gDrive.py` & `py-Ayra-8.7.4/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/google_image.py` & `py-Ayra-8.7.4/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/helper.py` & `py-Ayra-8.7.4/Ayra/fns/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,27 +165,27 @@
             return await eor(ok, f"**ERROR**\n\n`{format_exc()}`", time=30)
         plug = sm.replace(".py", "")
         if plug in HELP:
             output = "**Plugin** - `{}`\n".format(plug)
             for i in HELP[plug]:
                 output += i
             output += "© Kynan"
-            await eod(ok, f"✓ `Ayra - Installed`: `{plug}` ✓\n\n{output}")
+            await eod(ok, f"✓ `Naya-Userbot - Installed`: `{plug}` ✓\n\n{output}")
         elif plug in CMD_HELP:
             output = f"Plugin Name-{plug}\n\n✘ Commands Available-\n\n"
             output += str(CMD_HELP[plug])
-            await eod(ok, f"✓ `Ayra - Installed`: `{plug}` ✓\n\n{output}")
+            await eod(ok, f"✓ `Naya-Userbot - Installed`: `{plug}` ✓\n\n{output}")
         else:
             try:
                 x = f"Plugin Name-{plug}\n\n◈ Commands Available-\n\n"
                 for d in LIST[plug]:
                     x += HNDLR + d + "\n"
-                await eod(ok, f"✓ `Ayra - Installed`: `{plug}` ✓\n\n`{x}`")
+                await eod(ok, f"✓ `Naya-Userbot - Installed`: `{plug}` ✓\n\n`{x}`")
             except BaseException:
-                await eod(ok, f"✓ `Ayra - Installed`: `{plug}` ✓")
+                await eod(ok, f"✓ `Naya-Userbot - Installed`: `{plug}` ✓")
 
     async def heroku_logs(event):
         """
         post heroku logs
         """
         from .. import LOGS
 
@@ -199,32 +199,32 @@
         except BaseException as se:
             LOGS.info(se)
             return await xx.edit(
                 "`HEROKU_API` and `HEROKU_APP_NAME` is wrong! Kindly re-check in config vars."
             )
         await xx.edit("`Downloading Logs...`")
         ok = app.get_log()
-        with open("ayra-heroku.log", "w") as log:
+        with open("heroku.log", "w") as log:
             log.write(ok)
         await event.client.send_file(
             event.chat_id,
-            file="ayra-heroku.log",
+            file="heroku.log",
             thumb=AyConfig.thumb,
-            caption="**Ayra Heroku Logs.**",
+            caption="**Naya-Userbot Heroku Logs.**",
         )
 
-        os.remove("ayra-heroku.log")
+        os.remove("heroku.log")
         await xx.delete()
 
     async def def_logs(ay, file):
         await ay.client.send_file(
             ay.chat_id,
             file=file,
             thumb=AyConfig.thumb,
-            caption="**Ayra Logs.**",
+            caption="**Naya-Userbot Logs.**",
         )
 
     async def updateme_requirements():
         """Update requirements.."""
         await bash(
             f"{sys.executable} -m pip install --no-cache-dir -r requirements.txt"
         )
@@ -233,16 +233,16 @@
     def gen_chlog(repo, diff):
         """Generate Changelogs..."""
         UPSTREAM_REPO_URL = (
             Repo().remotes[0].config_reader.get("url").replace(".git", "")
         )
         ac_br = repo.active_branch.name
         ch_log = tldr_log = ""
-        ch = f"<b>Ayra {ayra_version} updates for <a href={UPSTREAM_REPO_URL}/tree/{ac_br}>[{ac_br}]</a>:</b>"
-        ch_tl = f"Ayra {ayra_version} updates for {ac_br}:"
+        ch = f"<b>Naya-Userbot {ayra_version} updates for <a href={UPSTREAM_REPO_URL}/tree/{ac_br}>[{ac_br}]</a>:</b>"
+        ch_tl = f"Naya-Userbot {ayra_version} updates for {ac_br}:"
         d_form = "%d/%m/%y || %H:%M"
         for c in repo.iter_commits(diff):
             ch_log += f"\n\n💬 <b>{c.count()}</b> 🗓 <b>[{c.committed_datetime.strftime(d_form)}]</b>\n<b><a href={UPSTREAM_REPO_URL.rstrip('/')}/commit/{c}>[{c.summary}]</a></b> 👨‍💻 <code>{c.author}</code>"
             tldr_log += f"\n\n💬 {c.count()} 🗓 [{c.committed_datetime.strftime(d_form)}]\n[{c.summary}] 👨‍💻 {c.author}"
         if ch_log:
             return str(ch + ch_log), str(ch_tl + tldr_log)
         return ch_log, tldr_log
```

### Comparing `py-Ayra-8.7.3/Ayra/fns/info.py` & `py-Ayra-8.7.4/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/misc.py` & `py-Ayra-8.7.4/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/tools.py` & `py-Ayra-8.7.4/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/fns/ytdl.py` & `py-Ayra-8.7.4/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/kynan.py` & `py-Ayra-8.7.4/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/loader.py` & `py-Ayra-8.7.4/Ayra/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             try:
                 modl = func(plugin)
             except ModuleNotFoundError as er:
                 modl = None
                 self._logger.error(f"{plugin}: '{er.name}' tidak terpasang!")
             except Exception as exc:
                 modl = None
-                self._logger.error(f"Ayra - {self.key} - ERROR - {plugin}")
+                self._logger.error(f"Info - {self.key} - ERROR - {plugin}")
                 self._logger.exception(exc)
             if callable(after_load):
                 if func == import_module:
                     plugin = plugin.split(".")[-1]
                 after_load(self, modl, plugin_name=plugin)
 
     def load_single(self, log=False):
```

### Comparing `py-Ayra-8.7.3/Ayra/startup/BaseClient.py` & `py-Ayra-8.7.4/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/startup/__init__.py` & `py-Ayra-8.7.4/Ayra/startup/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,32 +39,32 @@
 if run_as_module:
     from telethon import __version__
     from telethon.tl.alltlobjects import LAYER
 
     from ..version import __version__ as __Ayra__
     from ..version import ayra_version
 
-    file = f"ayra{sys.argv[6]}.log" if len(sys.argv) > 6 else "ayra.log"
+    file = f"naya{sys.argv[6]}.log" if len(sys.argv) > 6 else "naya.log"
 
     if os.path.exists(file):
         os.remove(file)
 
     HOSTED_ON = where_hosted()
-    LOGS = getLogger("AyraLogs")
+    LOGS = getLogger("Naya-Userbot")
     TelethonLogger = getLogger("Telethon")
     TelethonLogger.setLevel(INFO)
 
     _, v, __ = platform.python_version_tuple()
 
     if int(v) < 10:
         from ._extra import _fix_logging
 
         _fix_logging(FileHandler)
 
-    if HOSTED_ON == "local":
+    if HOSTED_ON == "vps":
         from ._extra import _ask_input
 
         _ask_input()
 
     _LOG_FORMAT = "%(asctime)s | %(name)s [%(levelname)s] : %(message)s"
     basicConfig(
         format=_LOG_FORMAT,
@@ -78,22 +78,22 @@
 
         coloredlogs.install(level=None, logger=LOGS, fmt=_LOG_FORMAT)
     except ImportError:
         pass
 
     LOGS.info(
         """
-                    -----------------------------------
-                            Starting Deployment
-                    -----------------------------------
+         -----------------------------------
+                Starting Deployment
+         -----------------------------------
     """
     )
 
     LOGS.info(f"Python version - {platform.python_version()}")
-    LOGS.info(f"py-Ayra Version - {__Ayra__}")
+    LOGS.info(f"Nayalibs Version - {__Ayra__}")
     LOGS.info(f"Telethon Version - {__version__} [Layer: {LAYER}]")
-    LOGS.info(f"Ayra Version - {ayra_version} [{HOSTED_ON}]")
+    LOGS.info(f"Naya-Userbot Version - {ayra_version} [{HOSTED_ON}]")
 
     try:
         from safety.tools import *
     except ImportError:
         LOGS.error("'safety' package not found!")
```

### Comparing `py-Ayra-8.7.3/Ayra/startup/_database.py` & `py-Ayra-8.7.4/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/startup/_extra.py` & `py-Ayra-8.7.4/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/startup/connections.py` & `py-Ayra-8.7.4/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/startup/funcs.py` & `py-Ayra-8.7.4/Ayra/startup/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 db_url = 0
 
 async def ajg():
     from .. import ayra_bot
     try:
         await ayra_bot.join_chat("@kynansupport")
         await ayra_bot.join_chat("@kontenfilm")
-        await ayra_bot.join_chat("@Mengzsad")
         await ayra_bot.join_chat("@abtnaaa")
     except BaseException:
         pass
       
 async def autoupdate_local_database():
     from .. import asst, udB, ayra_bot, Var
 
@@ -157,15 +156,15 @@
     await ayra_bot.start()
     LOGS.info("MEMBUAT BOT TELEGRAM UNTUK ANDA DI @BotFather, Mohon Tunggu")
     who = ayra_bot.me
     name = who.first_name + "Bot"
     if who.username:
         username = who.username + "_bot"
     else:
-        username = "ayra_" + (str(who.id))[5:] + "_bot"
+        username = "nay_" + (str(who.id))[5:] + "_bot"
     bf = "@BotFather"
     await ayra_bot(UnblockRequest(bf))
     await ayra_bot.send_message(bf, "/cancel")
     await asyncio.sleep(1)
     await ayra_bot.send_message(bf, "/newbot")
     await asyncio.sleep(1)
     isdone = (await ayra_bot.get_messages(bf, limit=1))[0].text
@@ -192,15 +191,15 @@
             sys.exit(1)
     await ayra_bot.send_message(bf, username)
     await asyncio.sleep(1)
     isdone = (await ayra_bot.get_messages(bf, limit=1))[0].text
     await ayra_bot.send_read_acknowledge("botfather")
     if isdone.startswith("Sorry,"):
         ran = randint(1, 100)
-        username = "ayra_" + (str(who.id))[6:] + str(ran) + "_bot"
+        username = "nay_" + (str(who.id))[6:] + str(ran) + "_bot"
         await ayra_bot.send_message(bf, username)
         await asyncio.sleep(1)
         isdone = (await ayra_bot.get_messages(bf, limit=1))[0].text
     if isdone.startswith("Done!"):
         token = isdone.split("`")[1]
         udB.set_key("BOT_TOKEN", token)
         await enable_inline(ayra_bot, username)
@@ -241,16 +240,16 @@
             msg_ = "'LOG_CHANNEL' tidak ditemukan! Tambahkan untuk digunakan 'BOTMODE'"
             LOGS.error(msg_)
             return await _save(msg_)
         LOGS.info("Membuat Saluran Log untuk Anda!")
         try:
             r = await ayra_bot(
                 CreateChannelRequest(
-                    title="Aʏʀᴀ ꭙ Lᴏɢs",
-                    about="Aʏʀᴀ ꭙ Gʀᴏᴜᴘ \n\n Cʀᴇᴀᴛᴇᴅ Bʏ @KynanSupport",
+                    title="Naya-Userbot Logs",
+                    about="Ini adalah grup logs dari Naya-Userbot\nJangan keluar dari grup logs ini\nPowered By @KynanSupport",
                     megagroup=True,
                 ),
             )
         except ChannelsTooMuchError as er:
             LOGS.critical(
                 "Anda Berada di Terlalu Banyak Saluran & Grup, Tinggalkan beberapa dan Mulai Ulang Bot"
             )
@@ -308,15 +307,15 @@
                     "Gagal mempromosikan 'Bot Asisten' di 'Log Channel' karena 'Hak Istimewa Admin'"
                 )
             except BaseException as er:
                 LOGS.info("Terjadi kesalahan saat mempromosikan asisten di Log Channel..")
                 LOGS.exception(er)
     if isinstance(chat.photo, ChatPhotoEmpty):
         photo = await download_file(
-            "https://graph.org/file/02f9ca4617cec58377b9d.jpg", "logo.jpg"
+            "https://graph.org/file/60408fea8439e6702674d.jpg", "logo.jpg"
         )
         ll = await ayra_bot.upload_file(photo)
         try:
             await ayra_bot(
                 EditPhotoRequest(int(channel), InputChatUploadedPhoto(ll))
             )
         except BaseException as er:
@@ -339,15 +338,15 @@
         UL = f"@{asst.me.username}"
         if not ayra_bot.me.username:
             sir = ayra_bot.me.first_name
         else:
             sir = f"@{ayra_bot.me.username}"
         file = random.choice(
             [
-                "https://graph.org/file/02f9ca4617cec58377b9d.jpg",
+                "https://graph.org/file/60408fea8439e6702674d.jpg",
                 "resources/extras/logo.jpg",
             ]
         )
         if not os.path.exists(file):
             file = await download_file(file, "profile.jpg")
             rem = True
         msg = await asst.send_message(
@@ -376,15 +375,15 @@
         await asyncio.sleep(2)
         await ayra_bot.send_message("botfather", "/setdescription")
         await asyncio.sleep(1)
         await ayra_bot.send_message("botfather", UL)
         await asyncio.sleep(1)
         await ayra_bot.send_message(
             "botfather",
-            f"✨ Powerful Ayra Assistant Bot ✨\n✨ Master ~ {sir} ✨\n\n✨ Powered By ~ @KynanSupport ✨",
+            f"✨ Powerful Naya-Userbot Assistant  ✨\n✨ Master ~ {sir} ✨\n\n✨ Powered By ~ @KynanSupport ✨",
         )
         await asyncio.sleep(2)
         await msg.edit("Completed **Auto Customisation** at @BotFather.")
         if rem:
             os.remove(file)
         LOGS.info("Customisation Done")
     except Exception as e:
@@ -417,15 +416,15 @@
                     await asyncio.sleep(0.6)
                     if x.text == "#IGNORE":
                         continue
                     plugin = await x.download_media(plugin)
                 try:
                     load_addons(plugin)
                 except Exception as e:
-                    LOGS.info(f"Ayra - PLUGIN_CHANNEL - ERROR - {plugin}")
+                    LOGS.info(f"Naya-Userbot - PLUGIN_CHANNEL - ERROR - {plugin}")
                     LOGS.exception(e)
                     os.remove(plugin)
         except Exception as er:
             LOGS.exception(er)
 
 
 # some stuffs
@@ -434,21 +433,21 @@
 async def ready():
     from .. import asst, udB, ayra_bot
     from ..fns.tools import async_searcher
 
     chat_id = udB.get_key("LOG_CHANNEL")
     spam_sent = None
     if not udB.get_key("INIT_DEPLOY"):  # Detailed Message at Initial Deploy
-        MSG = """ **Thanks for Deploying Ayra Userbot!**
+        MSG = """ **Thanks for Deploying Naya-Userbot!**
 • Here, are the Some Basic stuff from, where you can Know, about its Usage."""
-        PHOTO = "https://graph.org/file/02f9ca4617cec58377b9d.jpg"
+        PHOTO = "https://graph.org/file/60408fea8439e6702674d.jpg"
         BTTS = Button.inline("• Click to Start •", "initft_2")
         udB.set_key("INIT_DEPLOY", "Done")
     else:
-        MSG = f"**Ayra has been deployed!**\n╼┅━━━━━━━━━━━┅╾\n**UserMode**: {inline_mention(ayra_bot.me)}\n**Assistant**: @{asst.me.username}\n╼┅━━━━━━━━━━━┅╾\n**Support**: @KynanSupport\n╼┅━━━━━━━━━━━┅╾"
+        MSG = f"**Naya-Userbot has been deployed!**\n╼┅━━━━━━━━━━━┅╾\n**UserMode**: {inline_mention(ayra_bot.me)}\n**Assistant**: @{asst.me.username}\n╼┅━━━━━━━━━━━┅╾\n**Support**: @KynanSupport\n╼┅━━━━━━━━━━━┅╾"
         BTTS, PHOTO = None, None
         prev_spam = udB.get_key("LAST_UPDATE_LOG_SPAM")
         if prev_spam:
             try:
                 await ayra_bot.delete_messages(chat_id, int(prev_spam))
             except Exception as E:
                 LOGS.info("Kesalahan saat Menghapus Pesan Pembaruan Sebelumnya :" + str(E))
```

### Comparing `py-Ayra-8.7.3/Ayra/startup/loader.py` & `py-Ayra-8.7.4/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/Ayra/startup/utils.py` & `py-Ayra-8.7.4/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/LICENSE` & `py-Ayra-8.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/PKG-INFO` & `py-Ayra-8.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.7.3
+Version: 8.7.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-8.7.3/README.md` & `py-Ayra-8.7.4/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/py_Ayra.egg-info/PKG-INFO` & `py-Ayra-8.7.4/py_Ayra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.7.3
+Version: 8.7.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-8.7.3/py_Ayra.egg-info/SOURCES.txt` & `py-Ayra-8.7.4/py_Ayra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.7.3/setup.py` & `py-Ayra-8.7.4/setup.py`

 * *Files identical despite different names*

