# Comparing `tmp/tsp_wrapper-0.1.0.tar.gz` & `tmp/tsp_wrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsp_wrapper-0.1.0.tar", max compression
+gzip compressed data, was "tsp_wrapper-1.0.1.tar", last modified: Sat May  6 20:27:56 2023, max compression
```

## Comparing `tsp_wrapper-0.1.0.tar` & `tsp_wrapper-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,52 @@
--rw-r--r--   0        0        0     1078 2023-04-19 16:27:50.282688 tsp_wrapper-0.1.0/LICENSE
--rw-r--r--   0        0        0       50 2023-04-19 16:27:50.282688 tsp_wrapper-0.1.0/README.md
--rw-r--r--   0        0        0      533 2023-04-24 20:45:04.832091 tsp_wrapper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 10:51:22.896813 tsp_wrapper-0.1.0/tsp_wrapper/brokers/__init__.py
--rw-r--r--   0        0        0     1925 2023-04-24 19:26:25.504752 tsp_wrapper-0.1.0/tsp_wrapper/brokers/broker.py
--rw-r--r--   0        0        0     1858 2023-04-24 15:25:05.305610 tsp_wrapper-0.1.0/tsp_wrapper/brokers/builder.py
--rw-r--r--   0        0        0     1644 2023-04-24 19:26:25.504752 tsp_wrapper-0.1.0/tsp_wrapper/brokers/consumer.py
--rw-r--r--   0        0        0      939 2023-04-24 19:26:25.504752 tsp_wrapper-0.1.0/tsp_wrapper/brokers/producer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:26:25.504752 tsp_wrapper-0.1.0/tsp_wrapper/config/__init__.py
--rw-r--r--   0        0        0      552 2023-04-24 19:26:25.504752 tsp_wrapper-0.1.0/tsp_wrapper/config/logging.conf
--rw-r--r--   0        0        0      854 2023-04-24 19:26:25.504752 tsp_wrapper-0.1.0/tsp_wrapper/config/settings.py
--rw-r--r--   0        0        0        0 2023-04-24 10:51:22.956815 tsp_wrapper-0.1.0/tsp_wrapper/middleware/__init__.py
--rw-r--r--   0        0        0      148 2023-04-24 10:51:22.956815 tsp_wrapper-0.1.0/tsp_wrapper/middleware/schema.py
--rw-r--r--   0        0        0     4143 2023-04-24 19:26:25.504752 tsp_wrapper-0.1.0/tsp_wrapper/services.py
--rw-r--r--   0        0        0     4217 2023-04-24 19:26:25.504752 tsp_wrapper-0.1.0/tsp_wrapper/tsp.py
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 tsp_wrapper-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 20:27:56.188828 tsp_wrapper-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-06 20:27:56.188828 tsp_wrapper-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.176827 tsp_wrapper-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.180827 tsp_wrapper-1.0.1/src/tsp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.180827 tsp_wrapper-1.0.1/src/tsp_wrapper/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.180827 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/core/management/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/dict_to_city.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/euclidean_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/tsp_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.180827 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 20:27:56.000000 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-06 20:27:56.000000 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:27:56.000000 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 20:27:56.000000 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/top_level.txt
```

