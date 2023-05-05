# Comparing `tmp/FlipperNested-2.3.0.tar.gz` & `tmp/FlipperNested-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-2.3.0.tar", last modified: Tue May  2 16:58:46 2023, max compression
+gzip compressed data, was "FlipperNested-2.3.1.tar", last modified: Fri May  5 23:22:53 2023, max compression
```

## Comparing `FlipperNested-2.3.0.tar` & `FlipperNested-2.3.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.235860 FlipperNested-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.219860 FlipperNested-2.3.0/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.219860 FlipperNested-2.3.0/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.219860 FlipperNested-2.3.0/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 16:58:46.000000 FlipperNested-2.3.0/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-02 16:58:46.000000 FlipperNested-2.3.0/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:58:46.000000 FlipperNested-2.3.0/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 16:58:46.000000 FlipperNested-2.3.0/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 16:58:46.000000 FlipperNested-2.3.0/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 16:58:46.000000 FlipperNested-2.3.0/FlipperNested.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.219860 FlipperNested-2.3.0/HardNestedSolver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/bucketsort.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/bucketsort.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    85428 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/cmdhfmfhard.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/cmdhfmfhard.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    18805 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/crapto1.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2951 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/crapto1.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6561 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/crypto1.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.231860 FlipperNested-2.3.0/HardNestedSolver/hardnested/
--rwxr-xr-x   0 runner    (1001) docker     (123)   494104 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_benchmark_data.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    33334 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bf_core.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4073 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bf_core.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    31568 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bitarray_core.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3347 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bitarray_core.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    19427 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bruteforce.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2249 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bruteforce.h
--rwxr-xr-x   0 runner    (1001) docker     (123)  5060431 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/tables.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/hardnested/tables.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/library.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/library.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3340 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/parity.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.235860 FlipperNested-2.3.0/HardNestedSolver/pm3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1608 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/ansi.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3405 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/common.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/commonutil.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/commonutil.h
--rwxr-xr-x   0 runner    (1001) docker     (123)   110555 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/emojis.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/emojis_alt.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    13770 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/ui.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/ui.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/util.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/util.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/util_posix.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/pm3/util_posix.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/HardNestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.235860 FlipperNested-2.3.0/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 16:58:46.235860 FlipperNested-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:58:46.235860 FlipperNested-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:58:46.235860 FlipperNested-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 16:58:34.000000 FlipperNested-2.3.0/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.400812 FlipperNested-2.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.380811 FlipperNested-2.3.1/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.384811 FlipperNested-2.3.1/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.380811 FlipperNested-2.3.1/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-05 23:22:53.000000 FlipperNested-2.3.1/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-05 23:22:53.000000 FlipperNested-2.3.1/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:22:53.000000 FlipperNested-2.3.1/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 23:22:53.000000 FlipperNested-2.3.1/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 23:22:53.000000 FlipperNested-2.3.1/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 23:22:53.000000 FlipperNested-2.3.1/FlipperNested.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.384811 FlipperNested-2.3.1/HardNestedSolver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/bucketsort.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/bucketsort.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    85428 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/cmdhfmfhard.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/cmdhfmfhard.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18805 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/crapto1.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2951 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/crapto1.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6561 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/crypto1.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.396811 FlipperNested-2.3.1/HardNestedSolver/hardnested/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   494104 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_benchmark_data.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33334 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bf_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4073 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bf_core.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31568 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bitarray_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3347 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bitarray_core.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19427 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bruteforce.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2249 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bruteforce.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5060431 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/tables.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/hardnested/tables.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/library.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/library.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3340 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/parity.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.396811 FlipperNested-2.3.1/HardNestedSolver/pm3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1608 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/ansi.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3405 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/common.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/commonutil.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/commonutil.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110555 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/emojis.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/emojis_alt.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13770 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/ui.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/ui.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/util.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/util.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/util_posix.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/pm3/util_posix.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/HardNestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.400812 FlipperNested-2.3.1/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-05 23:22:53.400812 FlipperNested-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 23:22:53.400812 FlipperNested-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:22:53.400812 FlipperNested-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-05 23:22:42.000000 FlipperNested-2.3.1/tests/test_parse.py
```

### Comparing `FlipperNested-2.3.0/FlipperNested/bridge.py` & `FlipperNested-2.3.1/FlipperNested/bridge.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/FlipperNested/cli.py` & `FlipperNested-2.3.1/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/FlipperNested/main.py` & `FlipperNested-2.3.1/FlipperNested/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,17 +164,18 @@
                 contents = self.connection.file_read(self.FLIPPER_PATH + file["name"]).decode()
                 if not self.parse_file(contents):
                     print("[!] Failed to parse", file["name"])
                     continue
                 if self.save:
                     open(file["name"], "w+").write(contents)
                     print("[?] Saved nonces to", file["name"])
-                if self.recover_keys():
-                    break
+                stop = self.recover_keys()
                 self.save_keys_to_flipper()
+                if stop:
+                    break
 
     def extract_nonces_from_file(self, file):
         self.filename = file.name
         if not self.parse_file(file.read()):
             print("[!] Failed to parse", self.filename)
             return
         self.recover_keys()
```

### Comparing `FlipperNested-2.3.0/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-2.3.1/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/FlipperNested/proto/storage_pb2.py` & `FlipperNested-2.3.1/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-2.3.1/FlipperNested.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 2.3.0
+Version: 2.3.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-2.3.0/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-2.3.1/FlipperNested.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/bucketsort.c` & `FlipperNested-2.3.1/HardNestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/bucketsort.h` & `FlipperNested-2.3.1/HardNestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/cmdhfmfhard.c` & `FlipperNested-2.3.1/HardNestedSolver/cmdhfmfhard.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/cmdhfmfhard.h` & `FlipperNested-2.3.1/HardNestedSolver/cmdhfmfhard.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/crapto1.c` & `FlipperNested-2.3.1/HardNestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/crapto1.h` & `FlipperNested-2.3.1/HardNestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/crypto1.c` & `FlipperNested-2.3.1/HardNestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_benchmark_data.h` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_benchmark_data.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bf_core.c` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bf_core.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bf_core.h` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bf_core.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bitarray_core.c` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bitarray_core.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bitarray_core.h` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bitarray_core.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bruteforce.c` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bruteforce.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/hardnested_bruteforce.h` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/hardnested_bruteforce.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/tables.c` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/tables.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/hardnested/tables.h` & `FlipperNested-2.3.1/HardNestedSolver/hardnested/tables.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/parity.h` & `FlipperNested-2.3.1/HardNestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/ansi.h` & `FlipperNested-2.3.1/HardNestedSolver/pm3/ansi.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/common.h` & `FlipperNested-2.3.1/HardNestedSolver/pm3/common.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/commonutil.c` & `FlipperNested-2.3.1/HardNestedSolver/pm3/commonutil.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/commonutil.h` & `FlipperNested-2.3.1/HardNestedSolver/pm3/commonutil.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/emojis.h` & `FlipperNested-2.3.1/HardNestedSolver/pm3/emojis.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/emojis_alt.h` & `FlipperNested-2.3.1/HardNestedSolver/pm3/emojis_alt.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/ui.c` & `FlipperNested-2.3.1/HardNestedSolver/pm3/ui.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/ui.h` & `FlipperNested-2.3.1/HardNestedSolver/pm3/ui.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/util.c` & `FlipperNested-2.3.1/HardNestedSolver/pm3/util.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/util.h` & `FlipperNested-2.3.1/HardNestedSolver/pm3/util.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/util_posix.c` & `FlipperNested-2.3.1/HardNestedSolver/pm3/util_posix.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/pm3/util_posix.h` & `FlipperNested-2.3.1/HardNestedSolver/pm3/util_posix.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/HardNestedSolver/python.c` & `FlipperNested-2.3.1/HardNestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/LICENSE.md` & `FlipperNested-2.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/bucketsort.c` & `FlipperNested-2.3.1/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/bucketsort.h` & `FlipperNested-2.3.1/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/crapto1.c` & `FlipperNested-2.3.1/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/crapto1.h` & `FlipperNested-2.3.1/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/crypto1.c` & `FlipperNested-2.3.1/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/library.c` & `FlipperNested-2.3.1/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/library.h` & `FlipperNested-2.3.1/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/parity.h` & `FlipperNested-2.3.1/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/progress.c` & `FlipperNested-2.3.1/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/NestedSolver/python.c` & `FlipperNested-2.3.1/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/PKG-INFO` & `FlipperNested-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 2.3.0
+Version: 2.3.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-2.3.0/README.md` & `FlipperNested-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.0/setup.py` & `FlipperNested-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                                                      "HardNestedSolver/pm3/util_posix.c",
                                                      "HardNestedSolver/python.c"], include_dirs=include_dirs,
                               library_dirs=include_dirs, extra_compile_args=extra_compile_args, libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-setuptools.setup(name="FlipperNested", version="2.3.0", author="AloneLiberty",
+setuptools.setup(name="FlipperNested", version="2.3.1", author="AloneLiberty",
                  description="Recover keys from collected nonces", long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AloneLiberty/FlipperNestedRecovery",
                  entry_points={"console_scripts": ["FlipperNested = FlipperNested.cli:main"]},
                  install_requires=["protobuf>4", "pyserial"], ext_modules=[nested_solver, hardnested_solver],
                  packages=["FlipperNested", "FlipperNested.proto"], python_requires=">=3.8",
                  classifiers=["Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9",
```

### Comparing `FlipperNested-2.3.0/tests/test_calculate.py` & `FlipperNested-2.3.1/tests/test_calculate.py`

 * *Files identical despite different names*

