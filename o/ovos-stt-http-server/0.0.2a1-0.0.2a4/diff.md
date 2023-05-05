# Comparing `tmp/ovos-stt-http-server-0.0.2a1.tar.gz` & `tmp/ovos-stt-http-server-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-http-server-0.0.2a1.tar", last modified: Fri Apr 22 15:58:24 2022, max compression
+gzip compressed data, was "ovos-stt-http-server-0.0.2a4.tar", last modified: Fri May  5 22:02:37 2023, max compression
```

## Comparing `ovos-stt-http-server-0.0.2a1.tar` & `ovos-stt-http-server-0.0.2a4.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-04-22 15:58:24.430892 ovos-stt-http-server-0.0.2a1/
--rw-r--r--   0 user      (1000) user      (1000)    11347 2022-04-12 13:24:23.000000 ovos-stt-http-server-0.0.2a1/LICENSE.md
--rw-r--r--   0 user      (1000) user      (1000)     1068 2022-04-22 15:58:24.427559 ovos-stt-http-server-0.0.2a1/PKG-INFO
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-04-22 15:58:24.427559 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server/
--rw-r--r--   0 user      (1000) user      (1000)     1647 2022-04-22 15:58:06.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1008 2022-04-14 20:35:12.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server/__main__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-04-22 15:58:24.427559 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1068 2022-04-22 15:58:24.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      390 2022-04-22 15:58:24.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-04-22 15:58:24.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       72 2022-04-22 15:58:24.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       26 2022-04-22 15:58:24.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       21 2022-04-22 15:58:24.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-04-14 19:53:33.000000 ovos-stt-http-server-0.0.2a1/ovos_stt_http_server.egg-info/zip-safe
--rw-r--r--   0 user      (1000) user      (1000)       38 2022-04-22 15:58:24.430892 ovos-stt-http-server-0.0.2a1/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)     1355 2022-04-22 15:57:07.000000 ovos-stt-http-server-0.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:02:37.584654 ovos-stt-http-server-0.0.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-05 22:02:37.584654 ovos-stt-http-server-0.0.2a4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:02:37.576654 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:02:37.584654 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)    58605 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/ca.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    54765 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/de.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    50925 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/en.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    55341 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/es.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    57453 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/fr.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/it.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    68781 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/nl.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/pt.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    67821 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/audio/uk.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:02:37.580654 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:02:37.000000 ovos-stt-http-server-0.0.2a4/ovos_stt_http_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:02:37.584654 ovos-stt-http-server-0.0.2a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3049 2023-05-05 22:02:36.000000 ovos-stt-http-server-0.0.2a4/setup.py
```

### Comparing `ovos-stt-http-server-0.0.2a1/LICENSE.md` & `ovos-stt-http-server-0.0.2a4/LICENSE.md`

 * *Files identical despite different names*

