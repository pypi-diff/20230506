# Comparing `tmp/cyber-record-util-8.tar.gz` & `tmp/cyber-record-util-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyber-record-util-8.tar", last modified: Thu Nov 10 03:14:35 2022, max compression
+gzip compressed data, was "cyber-record-util-9.tar", last modified: Wed Mar 15 13:29:06 2023, max compression
```

## Comparing `cyber-record-util-8.tar` & `cyber-record-util-9.tar`

### file list

```diff
@@ -1,102 +1,105 @@
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.216888 cyber-record-util-8/
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1681 2022-11-10 03:13:06.000000 cyber-record-util-8/CMakeLists.txt
--rw-r--r--   0 whistler  (1000) whistler  (1000)    11425 2022-11-10 03:13:06.000000 cyber-record-util-8/LICENSE
--rw-r--r--   0 whistler  (1000) whistler  (1000)      162 2022-11-10 03:13:06.000000 cyber-record-util-8/MANIFEST.in
--rw-r--r--   0 whistler  (1000) whistler  (1000)      242 2022-11-10 03:14:35.216888 cyber-record-util-8/PKG-INFO
--rw-r--r--   0 whistler  (1000) whistler  (1000)      198 2022-11-10 03:13:06.000000 cyber-record-util-8/README.md
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.206888 cyber-record-util-8/cyber/
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.208888 cyber-record-util-8/cyber/base/
--rw-r--r--   0 whistler  (1000) whistler  (1000)     9017 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/atomic_hash_map.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3806 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/atomic_rw_lock.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     6736 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/bounded_queue.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4544 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/concurrent_object_pool.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1660 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/for_each.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2554 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/macros.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3948 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/object_pool.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4525 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/reentrant_rw_lock.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1866 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/rw_lock_guard.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4486 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/signal.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2960 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/thread_pool.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2435 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/thread_safe_queue.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2812 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/unbounded_queue.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3105 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/base/wait_strategy.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1231 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/binary.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1056 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/binary.h
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.209888 cyber-record-util-8/cyber/common/
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1618 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/environment.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)    11705 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/file.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     6978 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/file.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     7233 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/global_data.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3261 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/global_data.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4563 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/log.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3282 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/macros.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4917 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/time_conversion.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1464 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/types.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1302 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/common/util.h
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.210888 cyber-record-util-8/cyber/message/
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4408 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/message_header.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     9921 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/message_traits.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     7110 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/protobuf_factory.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4470 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/protobuf_factory.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2648 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/protobuf_traits.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4255 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/py_message.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1546 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/py_message_traits.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3013 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/raw_message.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1512 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/message/raw_message_traits.h
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.212888 cyber-record-util-8/cyber/proto/
--rw-r--r--   0 whistler  (1000) whistler  (1000)      693 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/choreography_conf.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      538 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/classic_conf.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      715 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/component_conf.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      359 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/cyber_conf.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      513 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/dag_conf.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      240 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/perf_conf.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      137 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/proto_desc.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      801 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/qos_profile.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2111 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/record.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      307 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/run_mode_conf.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)      571 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/scheduler_conf.proto
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1137 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/proto/transport_conf.proto
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.205888 cyber-record-util-8/cyber/python/
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.212888 cyber-record-util-8/cyber/python/internal/
--rw-r--r--   0 whistler  (1000) whistler  (1000)    20159 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/python/internal/py_record.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4445 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/python/internal/py_record.h
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.213888 cyber-record-util-8/cyber/record/
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.214887 cyber-record-util-8/cyber/record/file/
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1644 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/file/record_file_base.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1678 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/file/record_file_base.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4540 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/file/record_file_reader.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3224 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/file/record_file_reader.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     8634 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/file/record_file_writer.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     5662 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/file/record_file_writer.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1079 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/file/section.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3071 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/header_builder.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2518 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/header_builder.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2497 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/record_base.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1835 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/record_message.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     6038 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/record_reader.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3387 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/record_reader.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     6306 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/record_viewer.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4963 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/record_viewer.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     7043 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/record_writer.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     7137 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/record/record_writer.h
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.215888 cyber-record-util-8/cyber/time/
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2668 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/time/clock.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2757 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/time/clock.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     3507 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/time/duration.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2107 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/time/duration.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4287 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/time/rate.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1362 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/time/rate.h
--rw-r--r--   0 whistler  (1000) whistler  (1000)     4793 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/time/time.cc
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2873 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber/time/time.h
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.215888 cyber-record-util-8/cyber_record/
--rw-r--r--   0 whistler  (1000) whistler  (1000)     1003 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber_record/__init__.py
--rw-r--r--   0 whistler  (1000) whistler  (1000)     7756 2022-11-10 03:13:06.000000 cyber-record-util-8/cyber_record/record.py
-drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2022-11-10 03:14:35.216888 cyber-record-util-8/cyber_record_util.egg-info/
--rw-r--r--   0 whistler  (1000) whistler  (1000)      242 2022-11-10 03:14:34.000000 cyber-record-util-8/cyber_record_util.egg-info/PKG-INFO
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2400 2022-11-10 03:14:35.000000 cyber-record-util-8/cyber_record_util.egg-info/SOURCES.txt
--rw-r--r--   0 whistler  (1000) whistler  (1000)        1 2022-11-10 03:14:34.000000 cyber-record-util-8/cyber_record_util.egg-info/dependency_links.txt
--rw-r--r--   0 whistler  (1000) whistler  (1000)        1 2022-11-10 03:14:34.000000 cyber-record-util-8/cyber_record_util.egg-info/not-zip-safe
--rw-r--r--   0 whistler  (1000) whistler  (1000)       34 2022-11-10 03:14:35.000000 cyber-record-util-8/cyber_record_util.egg-info/top_level.txt
--rw-r--r--   0 whistler  (1000) whistler  (1000)       15 2022-11-10 03:13:06.000000 cyber-record-util-8/requirements.txt
--rw-r--r--   0 whistler  (1000) whistler  (1000)       38 2022-11-10 03:14:35.216888 cyber-record-util-8/setup.cfg
--rw-r--r--   0 whistler  (1000) whistler  (1000)     2823 2022-11-10 03:13:16.000000 cyber-record-util-8/setup.py
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.627778 cyber-record-util-9/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2107 2023-02-03 08:24:16.000000 cyber-record-util-9/CMakeLists.txt
+-rw-r--r--   0 whistler  (1000) whistler  (1000)    11425 2023-01-30 03:34:37.000000 cyber-record-util-9/LICENSE
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      162 2023-01-30 03:34:37.000000 cyber-record-util-9/MANIFEST.in
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      242 2023-03-15 13:29:06.627778 cyber-record-util-9/PKG-INFO
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      443 2023-02-01 08:01:18.000000 cyber-record-util-9/README.md
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.595778 cyber-record-util-9/cyber/
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.600778 cyber-record-util-9/cyber/base/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     9017 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/atomic_hash_map.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3806 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/atomic_rw_lock.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     6736 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/bounded_queue.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4544 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/concurrent_object_pool.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1660 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/for_each.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2554 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/macros.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3948 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/object_pool.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4525 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/reentrant_rw_lock.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1866 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/rw_lock_guard.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4486 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/signal.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2960 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/thread_pool.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2435 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/thread_safe_queue.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2812 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/unbounded_queue.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3105 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/base/wait_strategy.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1231 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/binary.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1056 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/binary.h
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.604778 cyber-record-util-9/cyber/common/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1618 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/environment.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)    11705 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/file.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     6978 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/file.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     7233 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/global_data.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3261 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/global_data.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4563 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/log.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3282 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/macros.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4917 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/time_conversion.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1464 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/types.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1302 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/common/util.h
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.592778 cyber-record-util-9/cyber/jni/
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.604778 cyber-record-util-9/cyber/jni/internal/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     5136 2023-01-30 09:07:10.000000 cyber-record-util-9/cyber/jni/internal/jni_record.cc
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.610778 cyber-record-util-9/cyber/message/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4408 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/message_header.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     9921 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/message_traits.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     7110 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/protobuf_factory.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4470 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/protobuf_factory.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2648 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/protobuf_traits.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4255 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/py_message.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1546 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/py_message_traits.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3013 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/raw_message.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1512 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/message/raw_message_traits.h
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.612778 cyber-record-util-9/cyber/proto/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      693 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/choreography_conf.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      538 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/classic_conf.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      715 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/component_conf.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      359 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/cyber_conf.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      513 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/dag_conf.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      240 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/perf_conf.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      137 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/proto_desc.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      801 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/qos_profile.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2111 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/record.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      307 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/run_mode_conf.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      571 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/scheduler_conf.proto
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1137 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/proto/transport_conf.proto
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.593778 cyber-record-util-9/cyber/python/
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.613778 cyber-record-util-9/cyber/python/internal/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)    20186 2023-01-30 08:43:26.000000 cyber-record-util-9/cyber/python/internal/py_record.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4445 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/python/internal/py_record.h
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.619778 cyber-record-util-9/cyber/record/
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.623778 cyber-record-util-9/cyber/record/file/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1644 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/file/record_file_base.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1678 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/file/record_file_base.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4540 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/file/record_file_reader.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3270 2023-03-15 13:26:20.000000 cyber-record-util-9/cyber/record/file/record_file_reader.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     8634 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/file/record_file_writer.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     5662 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/file/record_file_writer.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1079 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/file/section.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3071 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/header_builder.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2518 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/header_builder.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2497 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/record_base.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1835 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/record_message.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     6038 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/record_reader.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3387 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/record_reader.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     6306 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/record_viewer.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4963 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/record_viewer.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     7043 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/record_writer.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     7137 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/record/record_writer.h
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.626778 cyber-record-util-9/cyber/time/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2668 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/time/clock.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2757 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/time/clock.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     3507 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/time/duration.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2107 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/time/duration.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4287 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/time/rate.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1362 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/time/rate.h
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     4803 2023-02-03 08:21:07.000000 cyber-record-util-9/cyber/time/time.cc
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2873 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber/time/time.h
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.626778 cyber-record-util-9/cyber_record/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     1003 2023-01-30 03:34:37.000000 cyber-record-util-9/cyber_record/__init__.py
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     7756 2023-01-30 08:44:52.000000 cyber-record-util-9/cyber_record/record.py
+drwxr-xr-x   0 whistler  (1000) whistler  (1000)        0 2023-03-15 13:29:06.627778 cyber-record-util-9/cyber_record_util.egg-info/
+-rw-r--r--   0 whistler  (1000) whistler  (1000)      242 2023-03-15 13:29:06.000000 cyber-record-util-9/cyber_record_util.egg-info/PKG-INFO
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2433 2023-03-15 13:29:06.000000 cyber-record-util-9/cyber_record_util.egg-info/SOURCES.txt
+-rw-r--r--   0 whistler  (1000) whistler  (1000)        1 2023-03-15 13:29:06.000000 cyber-record-util-9/cyber_record_util.egg-info/dependency_links.txt
+-rw-r--r--   0 whistler  (1000) whistler  (1000)        1 2023-03-15 13:29:06.000000 cyber-record-util-9/cyber_record_util.egg-info/not-zip-safe
+-rw-r--r--   0 whistler  (1000) whistler  (1000)       34 2023-03-15 13:29:06.000000 cyber-record-util-9/cyber_record_util.egg-info/top_level.txt
+-rw-r--r--   0 whistler  (1000) whistler  (1000)       15 2023-01-30 03:34:37.000000 cyber-record-util-9/requirements.txt
+-rw-r--r--   0 whistler  (1000) whistler  (1000)       38 2023-03-15 13:29:06.627778 cyber-record-util-9/setup.cfg
+-rw-r--r--   0 whistler  (1000) whistler  (1000)     2823 2023-03-15 13:27:48.000000 cyber-record-util-9/setup.py
```

### Comparing `cyber-record-util-8/CMakeLists.txt` & `cyber-record-util-9/CMakeLists.txt`

 * *Files 24% similar despite different names*

```diff
@@ -18,43 +18,57 @@
     cyber/proto/component_conf.proto
     cyber/proto/dag_conf.proto
     cyber/proto/transport_conf.proto
     cyber/proto/run_mode_conf.proto
     cyber/proto/perf_conf.proto
 )
 
-add_library(_cyber_record_wrapper SHARED
+add_library(CyberRecordWrapper SHARED
     cyber/binary.cc
     cyber/message/protobuf_factory.cc
     cyber/common/global_data.cc
     cyber/common/file.cc
     cyber/record/record_viewer.cc
     cyber/record/record_reader.cc
     cyber/record/header_builder.cc
     cyber/record/record_writer.cc
     cyber/record/file/record_file_base.cc
     cyber/record/file/record_file_reader.cc
     cyber/record/file/record_file_writer.cc
     cyber/python/internal/py_record.cc
+    cyber/jni/internal/jni_record.cc
     cyber/time/clock.cc
     cyber/time/duration.cc
     cyber/time/rate.cc
     cyber/time/time.cc
     ${PROTO_SRCS}
 )
 
-target_include_directories(_cyber_record_wrapper PRIVATE .
+if (JAVA)
+    include_directories("$ENV{JAVA_HOME}/include")
+    include_directories("$ENV{JAVA_HOME}/include/linux")
+    include_directories("$ENV{JAVA_HOME}/include/darwin")
+    add_definitions(-DWITH_JAVA)
+    set_target_properties(
+        CyberRecordWrapper
+        PROPERTIES
+        OUTPUT_NAME "CyberRecordWrapper"
+        LINKER_LANGUAGE CXX
+    )
+else ()
+    set_target_properties(
+        CyberRecordWrapper
+        PROPERTIES
+        PREFIX ""
+        OUTPUT_NAME "_cyber_record_wrapper"
+        LINKER_LANGUAGE CXX
+    )
+endif()
+
+target_include_directories(CyberRecordWrapper PRIVATE .
     ${Protobuf_INCLUDE_DIRS}
     ${CMAKE_CURRENT_BINARY_DIR}
     ${PYTHON3_INCLUDE_DIRS}
     ${GLOG_INCLUDE_DIRS}
 )
 
-set_target_properties(
-    _cyber_record_wrapper
-    PROPERTIES
-    PREFIX ""
-    OUTPUT_NAME "_cyber_record_wrapper"
-    LINKER_LANGUAGE CXX
-)
-
-target_link_libraries(_cyber_record_wrapper ${PROTOBUF_LIBRARY} ${PYTHON3_LIBRARIES} ${GLOG_LIBRARIES})
+target_link_libraries(CyberRecordWrapper ${PROTOBUF_LIBRARY} ${PYTHON3_LIBRARIES} ${GLOG_LIBRARIES})
```

### Comparing `cyber-record-util-8/LICENSE` & `cyber-record-util-9/LICENSE`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/atomic_hash_map.h` & `cyber-record-util-9/cyber/base/atomic_hash_map.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/atomic_rw_lock.h` & `cyber-record-util-9/cyber/base/atomic_rw_lock.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/bounded_queue.h` & `cyber-record-util-9/cyber/base/bounded_queue.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/concurrent_object_pool.h` & `cyber-record-util-9/cyber/base/concurrent_object_pool.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/for_each.h` & `cyber-record-util-9/cyber/base/for_each.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/macros.h` & `cyber-record-util-9/cyber/base/macros.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/object_pool.h` & `cyber-record-util-9/cyber/base/object_pool.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/reentrant_rw_lock.h` & `cyber-record-util-9/cyber/base/reentrant_rw_lock.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/rw_lock_guard.h` & `cyber-record-util-9/cyber/base/rw_lock_guard.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/signal.h` & `cyber-record-util-9/cyber/base/signal.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/thread_pool.h` & `cyber-record-util-9/cyber/base/thread_pool.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/thread_safe_queue.h` & `cyber-record-util-9/cyber/base/thread_safe_queue.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/unbounded_queue.h` & `cyber-record-util-9/cyber/base/unbounded_queue.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/base/wait_strategy.h` & `cyber-record-util-9/cyber/base/wait_strategy.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/binary.cc` & `cyber-record-util-9/cyber/binary.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/binary.h` & `cyber-record-util-9/cyber/binary.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/environment.h` & `cyber-record-util-9/cyber/common/environment.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/file.cc` & `cyber-record-util-9/cyber/common/file.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/file.h` & `cyber-record-util-9/cyber/common/file.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/global_data.cc` & `cyber-record-util-9/cyber/common/global_data.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/global_data.h` & `cyber-record-util-9/cyber/common/global_data.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/log.h` & `cyber-record-util-9/cyber/common/log.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/macros.h` & `cyber-record-util-9/cyber/common/macros.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/time_conversion.h` & `cyber-record-util-9/cyber/common/time_conversion.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/types.h` & `cyber-record-util-9/cyber/common/types.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/common/util.h` & `cyber-record-util-9/cyber/common/util.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/message_header.h` & `cyber-record-util-9/cyber/message/message_header.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/message_traits.h` & `cyber-record-util-9/cyber/message/message_traits.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/protobuf_factory.cc` & `cyber-record-util-9/cyber/message/protobuf_factory.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/protobuf_factory.h` & `cyber-record-util-9/cyber/message/protobuf_factory.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/protobuf_traits.h` & `cyber-record-util-9/cyber/message/protobuf_traits.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/py_message.h` & `cyber-record-util-9/cyber/message/py_message.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/py_message_traits.h` & `cyber-record-util-9/cyber/message/py_message_traits.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/raw_message.h` & `cyber-record-util-9/cyber/message/raw_message.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/message/raw_message_traits.h` & `cyber-record-util-9/cyber/message/raw_message_traits.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/proto/choreography_conf.proto` & `cyber-record-util-9/cyber/proto/choreography_conf.proto`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/proto/classic_conf.proto` & `cyber-record-util-9/cyber/proto/classic_conf.proto`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/proto/component_conf.proto` & `cyber-record-util-9/cyber/proto/component_conf.proto`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/proto/dag_conf.proto` & `cyber-record-util-9/cyber/proto/dag_conf.proto`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/proto/qos_profile.proto` & `cyber-record-util-9/cyber/proto/qos_profile.proto`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/proto/record.proto` & `cyber-record-util-9/cyber/proto/record.proto`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/proto/scheduler_conf.proto` & `cyber-record-util-9/cyber/proto/scheduler_conf.proto`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/proto/transport_conf.proto` & `cyber-record-util-9/cyber/proto/transport_conf.proto`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/python/internal/py_record.cc` & `cyber-record-util-9/cyber/python/internal/py_record.cc`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *****************************************************************************/
 
+#ifndef WITH_JAVA
+
 #include "cyber/python/internal/py_record.h"
 #include <limits>
 #include <set>
 #include <string>
 
 #include <Python.h>
 
@@ -570,7 +572,9 @@
       nullptr,
       nullptr,
   };
 
   AINFO << "init _cyber_record_wrapper";
   return PyModule_Create(&module_def);
 }
+
+#endif
```

### Comparing `cyber-record-util-8/cyber/python/internal/py_record.h` & `cyber-record-util-9/cyber/python/internal/py_record.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/file/record_file_base.cc` & `cyber-record-util-9/cyber/record/file/record_file_base.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/file/record_file_base.h` & `cyber-record-util-9/cyber/record/file/record_file_base.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/file/record_file_reader.cc` & `cyber-record-util-9/cyber/record/file/record_file_reader.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/file/record_file_reader.h` & `cyber-record-util-9/cyber/record/file/record_file_reader.h`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
   if (size < std::numeric_limits<int>::min() ||
       size > std::numeric_limits<int>::max()) {
     AERROR << "Size value greater than the range of int value.";
     return false;
   }
   FileInputStream raw_input(fd_, static_cast<int>(size));
   CodedInputStream coded_input(&raw_input);
+  coded_input.SetTotalBytesLimit(size, size);
   CodedInputStream::Limit limit = coded_input.PushLimit(static_cast<int>(size));
   if (!message->ParseFromCodedStream(&coded_input)) {
     AERROR << "Parse section message failed.";
     end_of_file_ = coded_input.ExpectAtEnd();
     return false;
   }
   if (!coded_input.ConsumedEntireMessage()) {
```

### Comparing `cyber-record-util-8/cyber/record/file/record_file_writer.cc` & `cyber-record-util-9/cyber/record/file/record_file_writer.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/file/record_file_writer.h` & `cyber-record-util-9/cyber/record/file/record_file_writer.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/file/section.h` & `cyber-record-util-9/cyber/record/file/section.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/header_builder.cc` & `cyber-record-util-9/cyber/record/header_builder.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/header_builder.h` & `cyber-record-util-9/cyber/record/header_builder.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/record_base.h` & `cyber-record-util-9/cyber/record/record_base.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/record_message.h` & `cyber-record-util-9/cyber/record/record_message.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/record_reader.cc` & `cyber-record-util-9/cyber/record/record_reader.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/record_reader.h` & `cyber-record-util-9/cyber/record/record_reader.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/record_viewer.cc` & `cyber-record-util-9/cyber/record/record_viewer.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/record_viewer.h` & `cyber-record-util-9/cyber/record/record_viewer.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/record_writer.cc` & `cyber-record-util-9/cyber/record/record_writer.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/record/record_writer.h` & `cyber-record-util-9/cyber/record/record_writer.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/time/clock.cc` & `cyber-record-util-9/cyber/time/clock.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/time/clock.h` & `cyber-record-util-9/cyber/time/clock.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/time/duration.cc` & `cyber-record-util-9/cyber/time/duration.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/time/duration.h` & `cyber-record-util-9/cyber/time/duration.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/time/rate.cc` & `cyber-record-util-9/cyber/time/rate.cc`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/time/rate.h` & `cyber-record-util-9/cyber/time/rate.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber/time/time.cc` & `cyber-record-util-9/cyber/time/time.cc`

 * *Files 24% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 uint64_t Time::ToNanosecond() const { return nanoseconds_; }
 
 uint64_t Time::ToMicrosecond() const {
   return static_cast<uint64_t>(nanoseconds_ / 1000.0);
 }
 
 std::string Time::ToString() const {
-  auto nano = std::chrono::nanoseconds(nanoseconds_);
-  system_clock::time_point tp(nano);
+  auto micro = std::chrono::microseconds(ToMicrosecond());
+  system_clock::time_point tp(micro);
   auto time = system_clock::to_time_t(tp);
   struct tm stm;
   auto ret = localtime_r(&time, &stm);
   if (ret == nullptr) {
     return std::to_string(static_cast<double>(nanoseconds_) / 1000000000.0);
   }
 
@@ -106,16 +106,16 @@
   ss << std::string(date_time) << "." << std::setw(9) << std::setfill('0')
      << nanoseconds_ % 1000000000UL;
 #endif
   return ss.str();
 }
 
 void Time::SleepUntil(const Time& time) {
-  auto nano = std::chrono::nanoseconds(time.ToNanosecond());
-  system_clock::time_point tp(nano);
+  auto micro = std::chrono::microseconds(time.ToMicrosecond());
+  system_clock::time_point tp(micro);
   std::this_thread::sleep_until(tp);
 }
 
 Duration Time::operator-(const Time& rhs) const {
   return Duration(static_cast<int64_t>(nanoseconds_ - rhs.nanoseconds_));
 }
```

### Comparing `cyber-record-util-8/cyber/time/time.h` & `cyber-record-util-9/cyber/time/time.h`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber_record/__init__.py` & `cyber-record-util-9/cyber_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber_record/record.py` & `cyber-record-util-9/cyber_record/record.py`

 * *Files identical despite different names*

### Comparing `cyber-record-util-8/cyber_record_util.egg-info/SOURCES.txt` & `cyber-record-util-9/cyber_record_util.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 cyber/common/global_data.cc
 cyber/common/global_data.h
 cyber/common/log.h
 cyber/common/macros.h
 cyber/common/time_conversion.h
 cyber/common/types.h
 cyber/common/util.h
+cyber/jni/internal/jni_record.cc
 cyber/message/message_header.h
 cyber/message/message_traits.h
 cyber/message/protobuf_factory.cc
 cyber/message/protobuf_factory.h
 cyber/message/protobuf_traits.h
 cyber/message/py_message.h
 cyber/message/py_message_traits.h
```

### Comparing `cyber-record-util-8/setup.py` & `cyber-record-util-9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if not os.path.exists(self.build_temp):
             os.makedirs(self.build_temp)
         subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call(['cmake', '--build', '.'] + build_args, cwd=self.build_temp)
 
 setup(
     name = 'cyber-record-util',
-    version = '8',
+    version = '9',
     description = 'standalone apollo cyber record reader/writer',
     author = 'Wei Mingzhi',
     author_email = 'whistler@member.fsf.org',
     url = 'https://github.com/weimzh/cyber-record/',
     packages = ['cyber_record'],
     ext_modules = [CMakeExtension('cyber_record_wrapper', '.')],
     cmdclass = dict(build_ext=CMakeBuild),
```

