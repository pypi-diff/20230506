# Comparing `tmp/palp-0.0.98.tar.gz` & `tmp/palp-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palp-0.0.98.tar", last modified: Wed Dec 14 02:04:12 2022, max compression
+gzip compressed data, was "palp-0.0.99.tar", last modified: Wed Dec 14 02:23:30 2022, max compression
```

## Comparing `palp-0.0.98.tar` & `palp-0.0.99.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.102290 palp-0.0.98/
--rw-rw-rw-   0        0        0      334 2022-12-01 01:17:01.000000 palp-0.0.98/MANIFEST.in
--rw-rw-rw-   0        0        0    17380 2022-12-14 02:04:12.101291 palp-0.0.98/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:11.949906 palp-0.0.98/palp/
--rw-rw-rw-   0        0        0        7 2022-11-06 06:46:26.000000 palp-0.0.98/palp/.gitignore
--rw-rw-rw-   0        0        0    17082 2022-12-13 12:43:44.000000 palp-0.0.98/palp/README.md
--rw-rw-rw-   0        0        0        6 2022-12-14 02:03:22.000000 palp-0.0.98/palp/VERSION
--rw-rw-rw-   0        0        0      657 2022-12-12 07:53:03.000000 palp-0.0.98/palp/__init__.py
--rw-rw-rw-   0        0        0     2690 2022-12-08 00:42:25.000000 palp-0.0.98/palp/conn.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:11.968577 palp-0.0.98/palp/controller/
--rw-rw-rw-   0        0        0      124 2022-12-08 08:48:12.000000 palp-0.0.98/palp/controller/__init__.py
--rw-rw-rw-   0        0        0     4411 2022-12-13 08:25:00.000000 palp-0.0.98/palp/controller/controller_item.py
--rw-rw-rw-   0        0        0     7136 2022-12-12 07:44:06.000000 palp-0.0.98/palp/controller/controller_spider.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:11.974328 palp-0.0.98/palp/decorator/
--rw-rw-rw-   0        0        0       69 2022-12-13 12:25:17.000000 palp-0.0.98/palp/decorator/__init__.py
--rw-rw-rw-   0        0        0      983 2022-12-14 01:57:22.000000 palp-0.0.98/palp/decorator/decorator_run_func_by_thread.py
--rw-rw-rw-   0        0        0      895 2022-12-12 03:29:41.000000 palp-0.0.98/palp/decorator/decorator_spider_middleware.py
--rw-rw-rw-   0        0        0      768 2022-12-07 06:51:25.000000 palp-0.0.98/palp/exception.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:11.986278 palp-0.0.98/palp/filter/
--rw-rw-rw-   0        0        0      214 2022-12-08 08:52:48.000000 palp-0.0.98/palp/filter/__init__.py
--rw-rw-rw-   0        0        0     1995 2022-12-08 08:49:30.000000 palp-0.0.98/palp/filter/filter.py
--rw-rw-rw-   0        0        0     1399 2022-12-08 01:07:28.000000 palp-0.0.98/palp/filter/filter_bloom.py
--rw-rw-rw-   0        0        0     2646 2022-12-08 01:19:07.000000 palp-0.0.98/palp/filter/filter_redis_bloom.py
--rw-rw-rw-   0        0        0     1519 2022-12-08 01:19:31.000000 palp-0.0.98/palp/filter/filter_redis_set.py
--rw-rw-rw-   0        0        0     1388 2022-12-08 01:19:07.000000 palp-0.0.98/palp/filter/filter_set.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:11.992278 palp-0.0.98/palp/item/
--rw-rw-rw-   0        0        0       86 2022-12-08 05:36:21.000000 palp-0.0.98/palp/item/__init__.py
--rw-rw-rw-   0        0        0     2933 2022-12-07 09:00:21.000000 palp-0.0.98/palp/item/item.py
--rw-rw-rw-   0        0        0     1253 2022-12-08 05:37:38.000000 palp-0.0.98/palp/item/item_strict.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.010279 palp-0.0.98/palp/middleware/
--rw-rw-rw-   0        0        0      279 2022-12-08 01:49:00.000000 palp-0.0.98/palp/middleware/__init__.py
--rw-rw-rw-   0        0        0     2574 2022-12-12 08:04:31.000000 palp-0.0.98/palp/middleware/middleware_request.py
--rw-rw-rw-   0        0        0      966 2022-12-08 06:41:39.000000 palp-0.0.98/palp/middleware/middleware_request_check.py
--rw-rw-rw-   0        0        0     2453 2022-12-08 06:41:39.000000 palp-0.0.98/palp/middleware/middleware_request_filter.py
--rw-rw-rw-   0        0        0     2072 2022-12-13 02:29:03.000000 palp-0.0.98/palp/middleware/middleware_request_recycle.py
--rw-rw-rw-   0        0        0     1305 2022-12-12 08:02:30.000000 palp-0.0.98/palp/middleware/middleware_spider.py
--rw-rw-rw-   0        0        0     1157 2022-12-08 06:26:23.000000 palp-0.0.98/palp/middleware/middleware_spider_recycle.py
--rw-rw-rw-   0        0        0      483 2022-12-12 05:13:30.000000 palp-0.0.98/palp/middleware/middleware_spider_wait.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.028280 palp-0.0.98/palp/network/
--rw-rw-rw-   0        0        0      532 2022-12-12 08:06:15.000000 palp-0.0.98/palp/network/__init__.py
--rw-rw-rw-   0        0        0     2532 2022-12-12 06:47:45.000000 palp-0.0.98/palp/network/downloader.py
--rw-rw-rw-   0        0        0     2068 2022-12-13 02:15:57.000000 palp-0.0.98/palp/network/downloader_httpx.py
--rw-rw-rw-   0        0        0     1392 2022-12-13 02:15:57.000000 palp-0.0.98/palp/network/downloader_requests.py
--rw-rw-rw-   0        0        0     9027 2022-12-13 02:15:57.000000 palp-0.0.98/palp/network/request.py
--rw-rw-rw-   0        0        0     1036 2022-12-12 08:42:58.000000 palp-0.0.98/palp/network/request_method.py
--rw-rw-rw-   0        0        0     4086 2022-12-13 07:42:05.000000 palp-0.0.98/palp/network/response.py
--rw-rw-rw-   0        0        0     1172 2022-12-12 06:39:40.000000 palp-0.0.98/palp/network/response_httpx.py
--rw-rw-rw-   0        0        0     1173 2022-12-12 06:39:23.000000 palp-0.0.98/palp/network/response_requests.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.037278 palp-0.0.98/palp/pipeline/
--rw-rw-rw-   0        0        0      249 2022-12-08 01:48:59.000000 palp-0.0.98/palp/pipeline/__init__.py
--rw-rw-rw-   0        0        0     2520 2022-12-12 08:02:30.000000 palp-0.0.98/palp/pipeline/pipeline.py
--rw-rw-rw-   0        0        0     2185 2022-12-08 06:41:39.000000 palp-0.0.98/palp/pipeline/pipeline_filter.py
--rw-rw-rw-   0        0        0      803 2022-12-08 08:43:43.000000 palp-0.0.98/palp/pipeline/pipeline_recycle.py
--rw-rw-rw-   0        0        0      816 2022-11-04 06:30:55.000000 palp-0.0.98/palp/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.046643 palp-0.0.98/palp/sequence/
--rw-rw-rw-   0        0        0      336 2022-12-08 08:52:48.000000 palp-0.0.98/palp/sequence/__init__.py
--rw-rw-rw-   0        0        0     1669 2022-12-08 02:25:39.000000 palp-0.0.98/palp/sequence/sequence.py
--rw-rw-rw-   0        0        0     1984 2022-12-12 07:09:25.000000 palp-0.0.98/palp/sequence/sequence_memory.py
--rw-rw-rw-   0        0        0      610 2022-12-08 05:38:05.000000 palp-0.0.98/palp/sequence/sequence_redis_item.py
--rw-rw-rw-   0        0        0     2775 2022-12-12 07:09:45.000000 palp-0.0.98/palp/sequence/sequence_redis_request.py
--rw-rw-rw-   0        0        0     9121 2022-12-12 07:57:50.000000 palp-0.0.98/palp/settings.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.054016 palp-0.0.98/palp/spider/
--rw-rw-rw-   0        0        0      114 2022-12-08 08:53:55.000000 palp-0.0.98/palp/spider/__init__.py
--rw-rw-rw-   0        0        0     9923 2022-12-14 02:02:13.000000 palp-0.0.98/palp/spider/spider.py
--rw-rw-rw-   0        0        0     8618 2022-12-14 02:02:41.000000 palp-0.0.98/palp/spider/spider_distributive.py
--rw-rw-rw-   0        0        0     1146 2022-12-14 02:02:13.000000 palp-0.0.98/palp/spider/spider_local.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:11.928817 palp-0.0.98/palp/template/
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.056016 palp-0.0.98/palp/template/item/
--rw-rw-rw-   0        0        0      321 2022-12-08 09:02:54.000000 palp-0.0.98/palp/template/item/item.tmpl
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.060020 palp-0.0.98/palp/template/project/
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.063033 palp-0.0.98/palp/template/project/items/
--rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.98/palp/template/project/items/__init__.py
--rw-rw-rw-   0        0        0      291 2022-12-13 08:56:31.000000 palp-0.0.98/palp/template/project/items/item.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.067027 palp-0.0.98/palp/template/project/middlewares/
--rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.98/palp/template/project/middlewares/__init__.py
--rw-rw-rw-   0        0        0     2359 2022-12-12 09:03:09.000000 palp-0.0.98/palp/template/project/middlewares/middleware.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.070031 palp-0.0.98/palp/template/project/pipelines/
--rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.98/palp/template/project/pipelines/__init__.py
--rw-rw-rw-   0        0        0     1319 2022-12-12 08:00:43.000000 palp-0.0.98/palp/template/project/pipelines/pipeline.py
--rw-rw-rw-   0        0        0     4890 2022-12-12 09:13:16.000000 palp-0.0.98/palp/template/project/settings.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.073020 palp-0.0.98/palp/template/project/spiders/
--rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.98/palp/template/project/spiders/__init__.py
--rw-rw-rw-   0        0        0      197 2022-12-01 01:17:34.000000 palp-0.0.98/palp/template/project/start.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.076042 palp-0.0.98/palp/template/spider/
--rw-rw-rw-   0        0        0      828 2022-12-01 01:17:34.000000 palp-0.0.98/palp/template/spider/distributive_spider.tmpl
--rw-rw-rw-   0        0        0      797 2022-12-12 08:09:38.000000 palp-0.0.98/palp/template/spider/spider.tmpl
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.093925 palp-0.0.98/palp/tool/
--rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.98/palp/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:12.099293 palp-0.0.98/palp/tool/alarm/
--rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.98/palp/tool/alarm/__init__.py
--rw-rw-rw-   0        0        0     1665 2022-12-01 01:17:34.000000 palp-0.0.98/palp/tool/alarm/ding_talk.py
--rw-rw-rw-   0        0        0      476 2022-12-01 01:17:34.000000 palp-0.0.98/palp/tool/alarm/email.py
--rw-rw-rw-   0        0        0     6408 2022-12-14 02:02:13.000000 palp-0.0.98/palp/tool/client_heart.py
--rw-rw-rw-   0        0        0     1325 2022-12-01 01:17:34.000000 palp-0.0.98/palp/tool/create_project.py
--rw-rw-rw-   0        0        0     2889 2022-12-08 08:46:10.000000 palp-0.0.98/palp/tool/create_spider.py
--rw-rw-rw-   0        0        0     2359 2022-12-01 01:17:34.000000 palp-0.0.98/palp/tool/shell.py
--rw-rw-rw-   0        0        0     4029 2022-12-09 03:28:48.000000 palp-0.0.98/palp/tool/short_module.py
--rw-rw-rw-   0        0        0     3018 2022-12-08 08:46:10.000000 palp-0.0.98/palp/tool/start_spider.py
--rw-rw-rw-   0        0        0    45163 2022-12-01 01:17:34.000000 palp-0.0.98/palp/tool/user_agent.py
-drwxrwxrwx   0        0        0        0 2022-12-14 02:04:11.962573 palp-0.0.98/palp.egg-info/
--rw-rw-rw-   0        0        0    17380 2022-12-14 02:04:11.000000 palp-0.0.98/palp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2506 2022-12-14 02:04:11.000000 palp-0.0.98/palp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 02:04:11.000000 palp-0.0.98/palp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2022-12-14 02:04:11.000000 palp-0.0.98/palp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2022-12-14 02:04:11.000000 palp-0.0.98/palp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-12-14 02:04:11.000000 palp-0.0.98/palp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-14 02:04:12.103291 palp-0.0.98/setup.cfg
--rw-rw-rw-   0        0        0     1067 2022-12-14 02:03:22.000000 palp-0.0.98/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.125814 palp-0.0.99/
+-rw-rw-rw-   0        0        0      334 2022-12-01 01:17:01.000000 palp-0.0.99/MANIFEST.in
+-rw-rw-rw-   0        0        0    18035 2022-12-14 02:23:30.124827 palp-0.0.99/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:29.993059 palp-0.0.99/palp/
+-rw-rw-rw-   0        0        0        7 2022-11-06 06:46:26.000000 palp-0.0.99/palp/.gitignore
+-rw-rw-rw-   0        0        0    17737 2022-12-14 02:23:26.000000 palp-0.0.99/palp/README.md
+-rw-rw-rw-   0        0        0        6 2022-12-14 02:23:26.000000 palp-0.0.99/palp/VERSION
+-rw-rw-rw-   0        0        0      657 2022-12-12 07:53:03.000000 palp-0.0.99/palp/__init__.py
+-rw-rw-rw-   0        0        0     2690 2022-12-08 00:42:25.000000 palp-0.0.99/palp/conn.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.009058 palp-0.0.99/palp/controller/
+-rw-rw-rw-   0        0        0      124 2022-12-08 08:48:12.000000 palp-0.0.99/palp/controller/__init__.py
+-rw-rw-rw-   0        0        0     4411 2022-12-13 08:25:00.000000 palp-0.0.99/palp/controller/controller_item.py
+-rw-rw-rw-   0        0        0     7136 2022-12-12 07:44:06.000000 palp-0.0.99/palp/controller/controller_spider.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.014059 palp-0.0.99/palp/decorator/
+-rw-rw-rw-   0        0        0       69 2022-12-13 12:25:17.000000 palp-0.0.99/palp/decorator/__init__.py
+-rw-rw-rw-   0        0        0      983 2022-12-14 01:57:22.000000 palp-0.0.99/palp/decorator/decorator_run_func_by_thread.py
+-rw-rw-rw-   0        0        0      895 2022-12-12 03:29:41.000000 palp-0.0.99/palp/decorator/decorator_spider_middleware.py
+-rw-rw-rw-   0        0        0      768 2022-12-07 06:51:25.000000 palp-0.0.99/palp/exception.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.026064 palp-0.0.99/palp/filter/
+-rw-rw-rw-   0        0        0      214 2022-12-08 08:52:48.000000 palp-0.0.99/palp/filter/__init__.py
+-rw-rw-rw-   0        0        0     1995 2022-12-08 08:49:30.000000 palp-0.0.99/palp/filter/filter.py
+-rw-rw-rw-   0        0        0     1399 2022-12-08 01:07:28.000000 palp-0.0.99/palp/filter/filter_bloom.py
+-rw-rw-rw-   0        0        0     2646 2022-12-08 01:19:07.000000 palp-0.0.99/palp/filter/filter_redis_bloom.py
+-rw-rw-rw-   0        0        0     1519 2022-12-08 01:19:31.000000 palp-0.0.99/palp/filter/filter_redis_set.py
+-rw-rw-rw-   0        0        0     1388 2022-12-08 01:19:07.000000 palp-0.0.99/palp/filter/filter_set.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.030059 palp-0.0.99/palp/item/
+-rw-rw-rw-   0        0        0       86 2022-12-08 05:36:21.000000 palp-0.0.99/palp/item/__init__.py
+-rw-rw-rw-   0        0        0     2933 2022-12-07 09:00:21.000000 palp-0.0.99/palp/item/item.py
+-rw-rw-rw-   0        0        0     1253 2022-12-08 05:37:38.000000 palp-0.0.99/palp/item/item_strict.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.045055 palp-0.0.99/palp/middleware/
+-rw-rw-rw-   0        0        0      279 2022-12-08 01:49:00.000000 palp-0.0.99/palp/middleware/__init__.py
+-rw-rw-rw-   0        0        0     2574 2022-12-12 08:04:31.000000 palp-0.0.99/palp/middleware/middleware_request.py
+-rw-rw-rw-   0        0        0      966 2022-12-08 06:41:39.000000 palp-0.0.99/palp/middleware/middleware_request_check.py
+-rw-rw-rw-   0        0        0     2453 2022-12-08 06:41:39.000000 palp-0.0.99/palp/middleware/middleware_request_filter.py
+-rw-rw-rw-   0        0        0     2072 2022-12-13 02:29:03.000000 palp-0.0.99/palp/middleware/middleware_request_recycle.py
+-rw-rw-rw-   0        0        0     1305 2022-12-12 08:02:30.000000 palp-0.0.99/palp/middleware/middleware_spider.py
+-rw-rw-rw-   0        0        0     1157 2022-12-08 06:26:23.000000 palp-0.0.99/palp/middleware/middleware_spider_recycle.py
+-rw-rw-rw-   0        0        0      483 2022-12-12 05:13:30.000000 palp-0.0.99/palp/middleware/middleware_spider_wait.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.060827 palp-0.0.99/palp/network/
+-rw-rw-rw-   0        0        0      532 2022-12-12 08:06:15.000000 palp-0.0.99/palp/network/__init__.py
+-rw-rw-rw-   0        0        0     2532 2022-12-12 06:47:45.000000 palp-0.0.99/palp/network/downloader.py
+-rw-rw-rw-   0        0        0     2068 2022-12-13 02:15:57.000000 palp-0.0.99/palp/network/downloader_httpx.py
+-rw-rw-rw-   0        0        0     1392 2022-12-13 02:15:57.000000 palp-0.0.99/palp/network/downloader_requests.py
+-rw-rw-rw-   0        0        0     9027 2022-12-13 02:15:57.000000 palp-0.0.99/palp/network/request.py
+-rw-rw-rw-   0        0        0     1036 2022-12-12 08:42:58.000000 palp-0.0.99/palp/network/request_method.py
+-rw-rw-rw-   0        0        0     4086 2022-12-13 07:42:05.000000 palp-0.0.99/palp/network/response.py
+-rw-rw-rw-   0        0        0     1172 2022-12-12 06:39:40.000000 palp-0.0.99/palp/network/response_httpx.py
+-rw-rw-rw-   0        0        0     1173 2022-12-12 06:39:23.000000 palp-0.0.99/palp/network/response_requests.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.067813 palp-0.0.99/palp/pipeline/
+-rw-rw-rw-   0        0        0      249 2022-12-08 01:48:59.000000 palp-0.0.99/palp/pipeline/__init__.py
+-rw-rw-rw-   0        0        0     2520 2022-12-12 08:02:30.000000 palp-0.0.99/palp/pipeline/pipeline.py
+-rw-rw-rw-   0        0        0     2185 2022-12-08 06:41:39.000000 palp-0.0.99/palp/pipeline/pipeline_filter.py
+-rw-rw-rw-   0        0        0      803 2022-12-08 08:43:43.000000 palp-0.0.99/palp/pipeline/pipeline_recycle.py
+-rw-rw-rw-   0        0        0      816 2022-11-04 06:30:55.000000 palp-0.0.99/palp/requirements.txt
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.076814 palp-0.0.99/palp/sequence/
+-rw-rw-rw-   0        0        0      336 2022-12-08 08:52:48.000000 palp-0.0.99/palp/sequence/__init__.py
+-rw-rw-rw-   0        0        0     1669 2022-12-08 02:25:39.000000 palp-0.0.99/palp/sequence/sequence.py
+-rw-rw-rw-   0        0        0     1984 2022-12-12 07:09:25.000000 palp-0.0.99/palp/sequence/sequence_memory.py
+-rw-rw-rw-   0        0        0      610 2022-12-08 05:38:05.000000 palp-0.0.99/palp/sequence/sequence_redis_item.py
+-rw-rw-rw-   0        0        0     2775 2022-12-12 07:09:45.000000 palp-0.0.99/palp/sequence/sequence_redis_request.py
+-rw-rw-rw-   0        0        0     9121 2022-12-12 07:57:50.000000 palp-0.0.99/palp/settings.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.085814 palp-0.0.99/palp/spider/
+-rw-rw-rw-   0        0        0      114 2022-12-08 08:53:55.000000 palp-0.0.99/palp/spider/__init__.py
+-rw-rw-rw-   0        0        0     9922 2022-12-14 02:23:26.000000 palp-0.0.99/palp/spider/spider.py
+-rw-rw-rw-   0        0        0     8618 2022-12-14 02:02:41.000000 palp-0.0.99/palp/spider/spider_distributive.py
+-rw-rw-rw-   0        0        0     1146 2022-12-14 02:02:13.000000 palp-0.0.99/palp/spider/spider_local.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:29.975554 palp-0.0.99/palp/template/
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.086814 palp-0.0.99/palp/template/item/
+-rw-rw-rw-   0        0        0      321 2022-12-08 09:02:54.000000 palp-0.0.99/palp/template/item/item.tmpl
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.090809 palp-0.0.99/palp/template/project/
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.092814 palp-0.0.99/palp/template/project/items/
+-rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.99/palp/template/project/items/__init__.py
+-rw-rw-rw-   0        0        0      291 2022-12-13 08:56:31.000000 palp-0.0.99/palp/template/project/items/item.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.095814 palp-0.0.99/palp/template/project/middlewares/
+-rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.99/palp/template/project/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     2505 2022-12-14 02:23:26.000000 palp-0.0.99/palp/template/project/middlewares/middleware.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.099813 palp-0.0.99/palp/template/project/pipelines/
+-rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.99/palp/template/project/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     1456 2022-12-14 02:23:26.000000 palp-0.0.99/palp/template/project/pipelines/pipeline.py
+-rw-rw-rw-   0        0        0     4890 2022-12-12 09:13:16.000000 palp-0.0.99/palp/template/project/settings.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.101814 palp-0.0.99/palp/template/project/spiders/
+-rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.99/palp/template/project/spiders/__init__.py
+-rw-rw-rw-   0        0        0      197 2022-12-01 01:17:34.000000 palp-0.0.99/palp/template/project/start.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.104815 palp-0.0.99/palp/template/spider/
+-rw-rw-rw-   0        0        0      828 2022-12-01 01:17:34.000000 palp-0.0.99/palp/template/spider/distributive_spider.tmpl
+-rw-rw-rw-   0        0        0      797 2022-12-12 08:09:38.000000 palp-0.0.99/palp/template/spider/spider.tmpl
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.118815 palp-0.0.99/palp/tool/
+-rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.99/palp/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.123827 palp-0.0.99/palp/tool/alarm/
+-rw-rw-rw-   0        0        0        0 2022-12-01 01:17:34.000000 palp-0.0.99/palp/tool/alarm/__init__.py
+-rw-rw-rw-   0        0        0     1665 2022-12-01 01:17:34.000000 palp-0.0.99/palp/tool/alarm/ding_talk.py
+-rw-rw-rw-   0        0        0      476 2022-12-01 01:17:34.000000 palp-0.0.99/palp/tool/alarm/email.py
+-rw-rw-rw-   0        0        0     6408 2022-12-14 02:02:13.000000 palp-0.0.99/palp/tool/client_heart.py
+-rw-rw-rw-   0        0        0     1325 2022-12-01 01:17:34.000000 palp-0.0.99/palp/tool/create_project.py
+-rw-rw-rw-   0        0        0     2889 2022-12-08 08:46:10.000000 palp-0.0.99/palp/tool/create_spider.py
+-rw-rw-rw-   0        0        0     2359 2022-12-01 01:17:34.000000 palp-0.0.99/palp/tool/shell.py
+-rw-rw-rw-   0        0        0     4029 2022-12-09 03:28:48.000000 palp-0.0.99/palp/tool/short_module.py
+-rw-rw-rw-   0        0        0     3018 2022-12-08 08:46:10.000000 palp-0.0.99/palp/tool/start_spider.py
+-rw-rw-rw-   0        0        0    45163 2022-12-01 01:17:34.000000 palp-0.0.99/palp/tool/user_agent.py
+drwxrwxrwx   0        0        0        0 2022-12-14 02:23:30.004043 palp-0.0.99/palp.egg-info/
+-rw-rw-rw-   0        0        0    18035 2022-12-14 02:23:29.000000 palp-0.0.99/palp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2506 2022-12-14 02:23:29.000000 palp-0.0.99/palp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-14 02:23:29.000000 palp-0.0.99/palp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2022-12-14 02:23:29.000000 palp-0.0.99/palp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2022-12-14 02:23:29.000000 palp-0.0.99/palp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-12-14 02:23:29.000000 palp-0.0.99/palp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-12-14 02:23:30.125814 palp-0.0.99/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2022-12-14 02:23:26.000000 palp-0.0.99/setup.py
```

### Comparing `palp-0.0.98/PKG-INFO` & `palp-0.0.99/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palp
-Version: 0.0.98
+Version: 0.0.99
 Summary: 一个 爬虫框架
 Home-page: https://github.com/Leviathangk/palp
 Author: 郭一会儿
 Author-email: 1015295213@qq.com
 License: MIT Licence
 Keywords: palp,scrapy,feapder
 Platform: any
@@ -154,14 +154,46 @@
         print(response)
 
 
 if __name__ == '__main__':
     BaiduSpider(thread_count=1).start()
 ```
 
+# 启动爬虫
+
+## 爬虫内启动
+
+```
+BaiduSpider(thread_count=1).start() # 启动可选参数看源码，就几个
+```
+
+## 启动文件启动
+
+注意：是进程形式启动，推荐直接使用 start.py 即可，可同时启动多个爬虫
+
+参数介绍
+
+- spider_name：爬虫名（spider 内一致）
+- count：启动多少个实例（可实现单机分布式，就是进程启动多少个）
+- **kwargs：爬虫启动参数，同 spider 的启动参数
+
+【示例】
+
+```
+from palp import start_spider
+
+
+def main():
+    start_spider.execute(spider_name='xxx', count=1)
+ 
+ 
+if __name__ == '__main__':
+    main()
+```
+
 # 数据库连接
 
 通过 quickdb 模块，内置了 redis、mongo、mysql、kafka、postgresql 的连接，引用方式如下：
 
 ```
 from palp import conn
 conn.redis_conn # 接原始命令
```

### Comparing `palp-0.0.98/palp/README.md` & `palp-0.0.99/palp/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -142,14 +142,46 @@
         print(response)
 
 
 if __name__ == '__main__':
     BaiduSpider(thread_count=1).start()
 ```
 
+# 启动爬虫
+
+## 爬虫内启动
+
+```
+BaiduSpider(thread_count=1).start() # 启动可选参数看源码，就几个
+```
+
+## 启动文件启动
+
+注意：是进程形式启动，推荐直接使用 start.py 即可，可同时启动多个爬虫
+
+参数介绍
+
+- spider_name：爬虫名（spider 内一致）
+- count：启动多少个实例（可实现单机分布式，就是进程启动多少个）
+- **kwargs：爬虫启动参数，同 spider 的启动参数
+
+【示例】
+
+```
+from palp import start_spider
+
+
+def main():
+    start_spider.execute(spider_name='xxx', count=1)
+ 
+ 
+if __name__ == '__main__':
+    main()
+```
+
 # 数据库连接
 
 通过 quickdb 模块，内置了 redis、mongo、mysql、kafka、postgresql 的连接，引用方式如下：
 
 ```
 from palp import conn
 conn.redis_conn # 接原始命令
```

### Comparing `palp-0.0.98/palp/__init__.py` & `palp-0.0.99/palp/__init__.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/conn.py` & `palp-0.0.99/palp/conn.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/controller/controller_item.py` & `palp-0.0.99/palp/controller/controller_item.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/controller/controller_spider.py` & `palp-0.0.99/palp/controller/controller_spider.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/decorator/decorator_run_func_by_thread.py` & `palp-0.0.99/palp/decorator/decorator_run_func_by_thread.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/decorator/decorator_spider_middleware.py` & `palp-0.0.99/palp/decorator/decorator_spider_middleware.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/exception.py` & `palp-0.0.99/palp/exception.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/filter/filter.py` & `palp-0.0.99/palp/filter/filter.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/filter/filter_bloom.py` & `palp-0.0.99/palp/filter/filter_bloom.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/filter/filter_redis_bloom.py` & `palp-0.0.99/palp/filter/filter_redis_bloom.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/filter/filter_redis_set.py` & `palp-0.0.99/palp/filter/filter_redis_set.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/filter/filter_set.py` & `palp-0.0.99/palp/filter/filter_set.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/item/item.py` & `palp-0.0.99/palp/item/item.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/item/item_strict.py` & `palp-0.0.99/palp/item/item_strict.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/middleware/middleware_request.py` & `palp-0.0.99/palp/middleware/middleware_request.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/middleware/middleware_request_check.py` & `palp-0.0.99/palp/middleware/middleware_request_check.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/middleware/middleware_request_filter.py` & `palp-0.0.99/palp/middleware/middleware_request_filter.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/middleware/middleware_request_recycle.py` & `palp-0.0.99/palp/middleware/middleware_request_recycle.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/middleware/middleware_spider.py` & `palp-0.0.99/palp/middleware/middleware_spider.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/middleware/middleware_spider_recycle.py` & `palp-0.0.99/palp/middleware/middleware_spider_recycle.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/__init__.py` & `palp-0.0.99/palp/network/__init__.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/downloader.py` & `palp-0.0.99/palp/network/downloader.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/downloader_httpx.py` & `palp-0.0.99/palp/network/downloader_httpx.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/downloader_requests.py` & `palp-0.0.99/palp/network/downloader_requests.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/request.py` & `palp-0.0.99/palp/network/request.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/request_method.py` & `palp-0.0.99/palp/network/request_method.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/response.py` & `palp-0.0.99/palp/network/response.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/response_httpx.py` & `palp-0.0.99/palp/network/response_httpx.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/network/response_requests.py` & `palp-0.0.99/palp/network/response_requests.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/pipeline/pipeline.py` & `palp-0.0.99/palp/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/pipeline/pipeline_filter.py` & `palp-0.0.99/palp/pipeline/pipeline_filter.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/pipeline/pipeline_recycle.py` & `palp-0.0.99/palp/pipeline/pipeline_recycle.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/requirements.txt` & `palp-0.0.99/palp/requirements.txt`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/sequence/sequence.py` & `palp-0.0.99/palp/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/sequence/sequence_memory.py` & `palp-0.0.99/palp/sequence/sequence_memory.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/sequence/sequence_redis_item.py` & `palp-0.0.99/palp/sequence/sequence_redis_item.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/sequence/sequence_redis_request.py` & `palp-0.0.99/palp/sequence/sequence_redis_request.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/settings.py` & `palp-0.0.99/palp/settings.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/spider/spider.py` & `palp-0.0.99/palp/spider/spider.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         是否分发任务已经完成
 
         :return:
         """
         done_status = True
 
         for p in self.distribute_thread_list:
-            if not p.waiting:
+            if p.is_alive():
                 done_status = False
                 break
 
         return done_status
 
     def all_spider_controller_is_waiting(self) -> bool:
         """
```

### Comparing `palp-0.0.98/palp/spider/spider_distributive.py` & `palp-0.0.99/palp/spider/spider_distributive.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/spider/spider_local.py` & `palp-0.0.99/palp/spider/spider_local.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/template/project/middlewares/middleware.py` & `palp-0.0.99/palp/template/project/middlewares/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
-    中间件
-    SpiderMiddleware：爬虫中间件
-    RequestMiddleware：请求中间件
+    Middleware
 
-    参数全部可直接原地修改
+    注意：默认报错是 logger.error 输出，需要详细信息请使用 logger.exception（输出会很多，但很细）
 """
 import palp
 from typing import Union
 from palp import settings
 from loguru import logger
 from palp.network.request import Request
 
 
 class SpiderMiddleware(palp.SpiderMiddleware):
+    """
+        Spider 中间件：处理 spider 开启关闭任务
+    """
+
     def spider_start(self, spider) -> None:
         """
         spider 开始时的操作
 
         :param spider:
         :return:
         """
@@ -25,26 +27,30 @@
         """
         spider 出错时的操作
 
         :param spider:
         :param exception: 错误的详细信息
         :return:
         """
-        logger.exception(exception)
+        logger.error(exception)
 
     def spider_close(self, spider) -> None:
         """
         spider 结束的操作
 
         :param spider:
         :return:
         """
 
 
 class RequestMiddleware(palp.RequestMiddleware):
+    """
+        Request 中间件：处理请求
+    """
+
     def request_in(self, spider, request) -> None:
         """
         请求进入时的操作
 
         :param spider:
         :param request:
         :return:
@@ -60,15 +66,15 @@
         请求出错时的操作
 
         :param spider:
         :param request: 该参数可返回（用于放弃当前请求，并发起新请求）
         :param exception: 错误的详细信息
         :return: [Request, None]
         """
-        logger.exception(exception)
+        logger.error(exception)
 
         return
 
     def request_failed(self, spider, request) -> None:
         """
         超过最大重试次数时的操作
```

### Comparing `palp-0.0.98/palp/template/project/settings.py` & `palp-0.0.99/palp/template/project/settings.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/template/spider/distributive_spider.tmpl` & `palp-0.0.99/palp/template/spider/distributive_spider.tmpl`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/template/spider/spider.tmpl` & `palp-0.0.99/palp/template/spider/spider.tmpl`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/tool/alarm/ding_talk.py` & `palp-0.0.99/palp/tool/alarm/ding_talk.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/tool/client_heart.py` & `palp-0.0.99/palp/tool/client_heart.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/tool/create_project.py` & `palp-0.0.99/palp/tool/create_project.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/tool/create_spider.py` & `palp-0.0.99/palp/tool/create_spider.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/tool/shell.py` & `palp-0.0.99/palp/tool/shell.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/tool/short_module.py` & `palp-0.0.99/palp/tool/short_module.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/tool/start_spider.py` & `palp-0.0.99/palp/tool/start_spider.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp/tool/user_agent.py` & `palp-0.0.99/palp/tool/user_agent.py`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/palp.egg-info/PKG-INFO` & `palp-0.0.99/palp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palp
-Version: 0.0.98
+Version: 0.0.99
 Summary: 一个 爬虫框架
 Home-page: https://github.com/Leviathangk/palp
 Author: 郭一会儿
 Author-email: 1015295213@qq.com
 License: MIT Licence
 Keywords: palp,scrapy,feapder
 Platform: any
@@ -154,14 +154,46 @@
         print(response)
 
 
 if __name__ == '__main__':
     BaiduSpider(thread_count=1).start()
 ```
 
+# 启动爬虫
+
+## 爬虫内启动
+
+```
+BaiduSpider(thread_count=1).start() # 启动可选参数看源码，就几个
+```
+
+## 启动文件启动
+
+注意：是进程形式启动，推荐直接使用 start.py 即可，可同时启动多个爬虫
+
+参数介绍
+
+- spider_name：爬虫名（spider 内一致）
+- count：启动多少个实例（可实现单机分布式，就是进程启动多少个）
+- **kwargs：爬虫启动参数，同 spider 的启动参数
+
+【示例】
+
+```
+from palp import start_spider
+
+
+def main():
+    start_spider.execute(spider_name='xxx', count=1)
+ 
+ 
+if __name__ == '__main__':
+    main()
+```
+
 # 数据库连接
 
 通过 quickdb 模块，内置了 redis、mongo、mysql、kafka、postgresql 的连接，引用方式如下：
 
 ```
 from palp import conn
 conn.redis_conn # 接原始命令
```

### Comparing `palp-0.0.98/palp.egg-info/SOURCES.txt` & `palp-0.0.99/palp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palp-0.0.98/setup.py` & `palp-0.0.99/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 file_path = './palp/README.md'
 
 setup(
     name="palp",  # 这里是pip项目发布的名称
-    version="0.0.98",  # 版本号，数值大的会优先被pip
+    version="0.0.99",  # 版本号，数值大的会优先被pip
     keywords=["palp", "scrapy", "feapder"],  # 关键字
     description="一个 爬虫框架",  # 描述
     long_description=open(file_path, 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license="MIT Licence",  # 许可证
 
     url="https://github.com/Leviathangk/palp",  # 项目相关文件地址，一般是github项目地址即可
```

