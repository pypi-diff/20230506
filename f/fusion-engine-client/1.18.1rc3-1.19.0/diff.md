# Comparing `tmp/fusion-engine-client-1.18.1rc3.tar.gz` & `tmp/fusion-engine-client-1.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.18.1rc3.tar", last modified: Wed May  3 22:14:26 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.19.0.tar", last modified: Fri May  5 22:20:30 2023, max compression
```

## Comparing `fusion-engine-client-1.18.1rc3.tar` & `fusion-engine-client-1.19.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    13145 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   107613 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55470 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.386067 fusion-engine-client-1.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.378066 fusion-engine-client-1.19.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13349 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.378066 fusion-engine-client-1.19.0/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.378066 fusion-engine-client-1.19.0/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   107613 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55470 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.378066 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 22:20:30.000000 fusion-engine-client-1.19.0/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:20:30.386067 fusion-engine-client-1.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:20:30.382067 fusion-engine-client-1.19.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-05-05 22:19:53.000000 fusion-engine-client-1.19.0/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.18.1rc3/PKG-INFO` & `fusion-engine-client-1.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.18.1rc3
+Version: 1.19.0
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.18.1rc3/README.md` & `fusion-engine-client-1.19.0/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/bin/p1_extract` & `fusion-engine-client-1.19.0/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/bin/p1_print` & `fusion-engine-client-1.19.0/bin/p1_print`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from fusion_engine_client.messages import *
 from fusion_engine_client.parsers import MixedLogReader
 from fusion_engine_client.utils import trace as logging
 from fusion_engine_client.utils.argument_parser import ArgumentParser, ExtendedBooleanAction
 from fusion_engine_client.utils.log import locate_log, DEFAULT_LOG_BASE_DIR
 from fusion_engine_client.utils.time_range import TimeRange
-from fusion_engine_client.utils.trace import HighlightFormatter
+from fusion_engine_client.utils.trace import HighlightFormatter, BrokenPipeStreamHandler
 
 _logger = logging.getLogger('point_one.fusion_engine.applications.print_contents')
 
 
 def print_message(header, contents, offset_bytes, format='pretty'):
     if isinstance(contents, MessagePayload):
         if format in ('oneline', 'oneline-detailed'):
@@ -125,14 +125,15 @@
         else:
             logging.getLogger('point_one.fusion_engine.parsers').setLevel(
                 logging.getTraceLevel(depth=options.verbose - 1))
     else:
         logging.basicConfig(level=logging.INFO, format='%(message)s', stream=sys.stdout)
 
     HighlightFormatter.install(color=True, standoff_level=logging.WARNING)
+    BrokenPipeStreamHandler.install()
 
     # Locate the input file and set the output directory.
     input_path, log_id = locate_log(input_path=options.log, log_base_dir=options.log_base_dir, return_log_id=True,
                                     extract_fusion_engine_data=False)
     if input_path is None:
         # locate_log() will log an error.
         sys.exit(1)
@@ -210,56 +211,57 @@
     try:
         for header, message, data, offset_bytes in reader:
             bytes_decoded += len(data)
 
             # Update the data summary in summary mode, or print the message contents otherwise.
             total_messages += 1
             if options.summary:
-                p1_time = message.get_p1_time()
-                if p1_time is not None:
-                    if first_p1_time_sec is None:
-                        first_p1_time_sec = float(p1_time)
-                        last_p1_time_sec = float(p1_time)
-                        newest_p1_time = p1_time
-                    else:
-                        if p1_time < newest_p1_time:
-                            _logger.warning('P1 time restart detected after %s.' % str(newest_p1_time))
-                        last_p1_time_sec = max(last_p1_time_sec, float(p1_time))
-                        newest_p1_time = p1_time
-
-                system_time_sec = message.get_system_time_sec()
-                if system_time_sec is not None:
-                    if first_system_time_sec is None:
-                        first_system_time_sec = system_time_sec
-                        last_system_time_sec = system_time_sec
-                        newest_system_time_sec = system_time_sec
-                    else:
-                        if system_time_sec < newest_system_time_sec:
-                            _logger.warning('System time restart detected after %s.' %
-                                            system_time_to_str(newest_system_time_sec, is_seconds=True))
-                        last_system_time_sec = max(last_system_time_sec, system_time_sec)
-                        newest_system_time_sec = system_time_sec
-
                 entry = message_stats[header.message_type]
                 entry['count'] += 1
+
+                if message is not None:
+                    p1_time = message.get_p1_time()
+                    if p1_time is not None:
+                        if first_p1_time_sec is None:
+                            first_p1_time_sec = float(p1_time)
+                            last_p1_time_sec = float(p1_time)
+                            newest_p1_time = p1_time
+                        else:
+                            if p1_time < newest_p1_time:
+                                _logger.warning('P1 time restart detected after %s.' % str(newest_p1_time))
+                            last_p1_time_sec = max(last_p1_time_sec, float(p1_time))
+                            newest_p1_time = p1_time
+
+                    system_time_sec = message.get_system_time_sec()
+                    if system_time_sec is not None:
+                        if first_system_time_sec is None:
+                            first_system_time_sec = system_time_sec
+                            last_system_time_sec = system_time_sec
+                            newest_system_time_sec = system_time_sec
+                        else:
+                            if system_time_sec < newest_system_time_sec:
+                                _logger.warning('System time restart detected after %s.' %
+                                                system_time_to_str(newest_system_time_sec, is_seconds=True))
+                            last_system_time_sec = max(last_system_time_sec, system_time_sec)
+                            newest_system_time_sec = system_time_sec
             else:
                 print_message(header, message, offset_bytes, format=options.format)
-    except (BrokenPipeError, KeyboardInterrupt):
+    except (BrokenPipeError, KeyboardInterrupt) as e:
         sys.exit(1)
 
     # Print the data summary.
     if options.summary:
         _logger.info('Input file: %s' % input_path)
         _logger.info('Log ID: %s' % log_id)
         if first_p1_time_sec is not None:
-            _logger.info('Duration (P1): %d seconds' % (last_p1_time_sec - first_p1_time_sec))
+            _logger.info('Duration (P1): %.1f seconds' % (last_p1_time_sec - first_p1_time_sec))
         else:
             _logger.info('Duration (P1): unknown')
         if first_system_time_sec is not None:
-            _logger.info('Duration (system): %d seconds' % (last_system_time_sec - first_system_time_sec))
+            _logger.info('Duration (system): %.1f seconds' % (last_system_time_sec - first_system_time_sec))
         else:
             _logger.info('Duration (system): unknown')
         _logger.info('Total data read: %d B' % reader.get_bytes_read())
         _logger.info('Selected data size: %d B' % bytes_decoded)
         _logger.info('')
 
         format_string = '| {:<50} | {:>8} |'
```

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.19.0/fusion_engine_client/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.19.0/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.19.0/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/configuration.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.19.0/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.19.0/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.19.0/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.19.0/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.19.0/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.19.0/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.19.0/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.19.0/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.19.0/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.19.0/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/numpy_utils.py` & `fusion-engine-client-1.19.0/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.19.0/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.19.0/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.18.1rc3
+Version: 1.19.0
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.19.0/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/setup.py` & `fusion-engine-client-1.19.0/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_config.py` & `fusion-engine-client-1.19.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_construct_utils.py` & `fusion-engine-client-1.19.0/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_data_loader.py` & `fusion-engine-client-1.19.0/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_decoder.py` & `fusion-engine-client-1.19.0/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_encoder.py` & `fusion-engine-client-1.19.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_enum_utils.py` & `fusion-engine-client-1.19.0/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_file_index.py` & `fusion-engine-client-1.19.0/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_message_defs.py` & `fusion-engine-client-1.19.0/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.19.0/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc3/tests/test_time_range.py` & `fusion-engine-client-1.19.0/tests/test_time_range.py`

 * *Files identical despite different names*

