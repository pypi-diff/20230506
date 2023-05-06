# Comparing `tmp/ayugespidertools-2.0.2.tar.gz` & `tmp/ayugespidertools-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-2.0.2.tar", max compression
+gzip compressed data, was "ayugespidertools-2.0.3.tar", max compression
```

## Comparing `ayugespidertools-2.0.2.tar` & `ayugespidertools-2.0.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/LICENSE
--rw-r--r--   0        0        0    13798 2023-04-27 03:19:49.000000 ayugespidertools-2.0.2/README.md
--rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-2.0.2/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-2.0.2/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      158 2023-04-25 08:54:15.594268 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      536 2023-04-25 08:55:28.881319 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      685 2023-04-25 08:54:15.595268 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
--rw-r--r--   0        0        0     2871 2023-04-27 08:04:48.083361 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
--rw-r--r--   0        0        0     1086 2023-04-25 08:54:15.618268 ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-2.0.2/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     4050 2023-04-27 07:39:48.000000 ayugespidertools-2.0.2/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-2.0.2/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-2.0.2/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-2.0.2/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     6885 2023-05-05 06:09:23.000000 ayugespidertools-2.0.2/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    11765 2023-04-27 08:36:37.000000 ayugespidertools-2.0.2/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13474 2023-04-25 02:55:56.000000 ayugespidertools-2.0.2/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-2.0.2/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-2.0.2/ayugespidertools/common/spiderdbconf.py
--rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-2.0.2/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-2.0.2/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    11325 2023-04-26 08:38:41.000000 ayugespidertools-2.0.2/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-2.0.2/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-2.0.2/ayugespidertools/config.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-2.0.2/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-2.0.2/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-2.0.2/ayugespidertools/items.py
--rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-2.0.2/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-2.0.2/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-2.0.2/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-2.0.2/ayugespidertools/oss.py
--rw-r--r--   0        0        0      802 2023-05-04 09:14:56.000000 ayugespidertools-2.0.2/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/processmanager.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-2.0.2/ayugespidertools/request.py
--rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-2.0.2/ayugespidertools/rpa.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/runjs.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0      356 2023-04-26 08:48:02.859698 ayugespidertools-2.0.2/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-25 08:54:13.045266 ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1068 2023-04-27 08:45:17.819120 ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0      981 2023-04-25 08:58:10.179432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-04-25 08:58:10.180432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
--rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0      475 2023-04-25 08:58:10.180432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7677 2023-04-27 07:35:53.380544 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc
--rw-r--r--   0        0        0     2200 2023-04-25 08:58:10.182432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
--rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0      481 2023-04-25 08:58:10.183432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3911 2023-04-25 08:58:10.184432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
--rw-r--r--   0        0        0     3056 2023-04-26 08:48:05.030700 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
--rw-r--r--   0        0        0     7795 2023-04-25 08:58:10.186432 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
--rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      885 2023-04-25 08:58:19.202438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0      173 2023-04-25 08:58:19.202438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2624 2023-05-05 08:55:33.703084 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc
--rw-r--r--   0        0        0     2971 2023-05-05 08:55:33.673084 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1820 2023-04-25 08:58:19.205438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     2114 2023-05-05 07:48:47.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2872 2023-05-04 09:09:37.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1356 2023-04-25 03:00:42.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    13396 2023-04-25 03:01:05.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0    11209 2023-04-25 08:58:19.207438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4019 2023-05-05 08:55:33.680084 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
--rw-r--r--   0        0        0      717 2023-04-25 08:58:19.219438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
--rw-r--r--   0        0        0     1998 2023-05-04 07:33:52.883359 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-04-25 08:58:19.223438 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
--rw-r--r--   0        0        0     4379 2023-05-05 08:25:40.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3794 2023-04-25 03:02:20.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     6737 2023-04-25 03:02:38.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     4569 2023-04-25 08:54:13.141266 ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      760 2023-04-25 08:54:14.345267 ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-2.0.2/ayugespidertools/spiders.py
--rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      613 2023-04-25 05:46:03.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     4093 2023-04-25 04:01:51.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-2.0.2/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6409 2023-04-25 08:46:25.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1941 2023-04-25 08:47:57.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-2.0.2/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.2/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0      155 2023-04-25 08:55:31.774321 ayugespidertools-2.0.2/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5327 2023-04-27 08:04:47.882360 ayugespidertools-2.0.2/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
--rw-r--r--   0        0        0     5920 2023-04-27 07:40:39.000000 ayugespidertools-2.0.2/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-2.0.2/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3021 2023-05-05 09:31:16.000000 ayugespidertools-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    15498 1970-01-01 00:00:00.000000 ayugespidertools-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/LICENSE
+-rw-r--r--   0        0        0    13798 2023-04-27 03:19:49.000000 ayugespidertools-2.0.3/README.md
+-rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-2.0.3/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-2.0.3/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-25 08:54:15.594268 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      536 2023-04-25 08:55:28.881319 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      685 2023-04-25 08:54:15.595268 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
+-rw-r--r--   0        0        0     2860 2023-05-06 06:33:53.042068 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
+-rw-r--r--   0        0        0     1086 2023-04-25 08:54:15.618268 ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-2.0.3/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     4039 2023-05-06 06:32:50.000000 ayugespidertools-2.0.3/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-2.0.3/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-2.0.3/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-2.0.3/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     6885 2023-05-05 06:09:23.000000 ayugespidertools-2.0.3/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    11765 2023-04-27 08:36:37.000000 ayugespidertools-2.0.3/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13474 2023-04-25 02:55:56.000000 ayugespidertools-2.0.3/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-2.0.3/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-2.0.3/ayugespidertools/common/spiderdbconf.py
+-rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-2.0.3/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-2.0.3/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    11325 2023-04-26 08:38:41.000000 ayugespidertools-2.0.3/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-2.0.3/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-2.0.3/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-2.0.3/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-2.0.3/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-2.0.3/ayugespidertools/items.py
+-rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-2.0.3/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-2.0.3/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-2.0.3/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-2.0.3/ayugespidertools/oss.py
+-rw-r--r--   0        0        0      802 2023-05-04 09:14:56.000000 ayugespidertools-2.0.3/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/processmanager.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-2.0.3/ayugespidertools/request.py
+-rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-2.0.3/ayugespidertools/rpa.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/runjs.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0      356 2023-04-26 08:48:02.859698 ayugespidertools-2.0.3/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1442 2023-04-25 08:54:13.045266 ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1068 2023-04-27 08:45:17.819120 ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-25 08:58:10.179432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-04-25 08:58:10.180432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc
+-rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-25 08:58:10.180432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7677 2023-04-27 07:35:53.380544 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc
+-rw-r--r--   0        0        0     2200 2023-04-25 08:58:10.182432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc
+-rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0      481 2023-04-25 08:58:10.183432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3911 2023-04-25 08:58:10.184432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc
+-rw-r--r--   0        0        0     3056 2023-04-26 08:48:05.030700 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc
+-rw-r--r--   0        0        0     7795 2023-04-25 08:58:10.186432 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc
+-rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-25 08:58:19.202438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-25 08:58:19.202438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2624 2023-05-05 08:55:33.703084 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc
+-rw-r--r--   0        0        0     2971 2023-05-05 08:55:33.673084 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1820 2023-04-25 08:58:19.205438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     2114 2023-05-05 07:48:47.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2872 2023-05-04 09:09:37.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1356 2023-04-25 03:00:42.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0    13396 2023-04-25 03:01:05.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0    11209 2023-04-25 08:58:19.207438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4019 2023-05-05 08:55:33.680084 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc
+-rw-r--r--   0        0        0      717 2023-04-25 08:58:19.219438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc
+-rw-r--r--   0        0        0     1998 2023-05-04 07:33:52.883359 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-04-25 08:58:19.223438 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc
+-rw-r--r--   0        0        0     4379 2023-05-05 08:25:40.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3794 2023-04-25 03:02:20.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     6737 2023-04-25 03:02:38.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     4569 2023-04-25 08:54:13.141266 ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      760 2023-04-25 08:54:14.345267 ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-2.0.3/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/.gitignore
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      613 2023-04-25 05:46:03.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     4093 2023-04-25 04:01:51.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-2.0.3/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6409 2023-04-25 08:46:25.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1941 2023-04-25 08:47:57.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-2.0.3/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-2.0.3/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-25 08:55:31.774321 ayugespidertools-2.0.3/ayugespidertools/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5316 2023-05-06 06:33:52.862068 ayugespidertools-2.0.3/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc
+-rw-r--r--   0        0        0     5909 2023-05-06 06:33:34.000000 ayugespidertools-2.0.3/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-2.0.3/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3135 2023-05-06 07:47:20.000000 ayugespidertools-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    15541 1970-01-01 00:00:00.000000 ayugespidertools-2.0.3/PKG-INFO
```

### Comparing `ayugespidertools-2.0.2/LICENSE` & `ayugespidertools-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/README.md` & `ayugespidertools-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 27 07:39:48 2023 UTC, .py size: 4050 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c426 4a64 d20f 0000  U........&Jd....
+00000000: 550d 0d0a 0000 0000 92f4 5564 c70f 0000  U.........Ud....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6401 6c0d  m.Z.m.Z...d.d.l.
@@ -104,77 +104,76 @@
 00000670: 6563 746f 7279 2027 7a0e 272c 2063 7265  ectory 'z.', cre
 00000680: 6174 6564 2069 6e3a 7a04 2020 2020 da01  ated in:z.    ..
 00000690: 0a7a 2559 6f75 2063 616e 2073 7461 7274  .z%You can start
 000006a0: 2079 6f75 7220 6669 7273 7420 7370 6964   your first spid
 000006b0: 6572 2077 6974 683a 7a07 2020 2020 6364  er with:z.    cd
 000006c0: 207a 2820 2020 2073 6372 6170 7920 6765   z(    scrapy ge
 000006d0: 6e73 7069 6465 7220 6578 616d 706c 6520  nspider example 
-000006e0: 6578 616d 706c 652e 636f 6d7a 394f 7220  example.comz9Or 
+000006e0: 6578 616d 706c 652e 636f 6d7a 2e4f 7220  example.comz.Or 
 000006f0: 796f 7520 6361 6e20 7374 6172 7420 796f  you can start yo
 00000700: 7572 2066 6972 7374 2073 7069 6465 7220  ur first spider 
-00000710: 7769 7468 2061 7975 6765 7370 6964 6572  with ayugespider
-00000720: 746f 6f6c 733a 7a27 2020 2020 6179 7567  tools:z'    ayug
-00000730: 6520 6765 6e73 7069 6465 7220 6578 616d  e genspider exam
-00000740: 706c 6520 6578 616d 706c 652e 636f 6d29  ple example.com)
-00000750: 12da 036c 656e 7206 0000 0072 0200 0000  ...lenr....r....
-00000760: da06 6578 6973 7473 da08 6578 6974 636f  ..exists..exitco
-00000770: 6465 da05 7072 696e 74da 0772 6573 6f6c  de..print..resol
-00000780: 7665 5a0e 5f69 735f 7661 6c69 645f 6e61  veZ._is_valid_na
-00000790: 6d65 da09 5f63 6f70 7974 7265 65da 0d74  me.._copytree..t
-000007a0: 656d 706c 6174 6573 5f64 6972 7204 0000  emplates_dirr...
-000007b0: 00da 1354 454d 504c 4154 4553 5f54 4f5f  ...TEMPLATES_TO_
-000007c0: 5245 4e44 4552 7207 0000 0072 0800 0000  RENDERr....r....
-000007d0: 7209 0000 00da 0a49 535f 5749 4e44 4f57  r......IS_WINDOW
-000007e0: 53da 0675 6e6c 696e 6bda 0373 7472 290a  S..unlink..str).
-000007f0: da04 7365 6c66 da04 6172 6773 da04 6f70  ..self..args..op
-00000800: 7473 5a15 5f68 6173 5f70 726f 6a65 6374  tsZ._has_project
-00000810: 5f64 6972 5f61 7267 735a 0b70 726f 6a65  _dir_argsZ.proje
-00000820: 6374 5f64 6972 da05 7061 7468 735a 0774  ct_dir..pathsZ.t
-00000830: 706c 6669 6c65 5a0e 7275 6e5f 7368 656c  plfileZ.run_shel
-00000840: 6c5f 7061 7468 5a11 7275 6e5f 7368 656c  l_pathZ.run_shel
-00000850: 6c5f 6162 7370 6174 685a 0864 656c 5f66  l_abspathZ.del_f
-00000860: 696c 6572 1900 0000 7212 0000 0072 1a00  iler....r....r..
-00000870: 0000 da03 7275 6e20 0000 0073 7000 0000  ....run ...sp...
-00000880: 0001 0c01 0602 0802 0c01 0401 0e02 0401  ................
-00000890: 0c02 0c01 0601 1201 0402 0a01 0601 0402  ................
-000008a0: 1601 1201 0801 0201 02ff 0202 0a02 02fe  ................
-000008b0: 04fe 0607 0201 0201 0202 0201 06fb 0809  ................
-000008c0: 0401 1202 1001 0c02 0801 0801 0801 0c01  ................
-000008d0: 0a03 0201 0201 0201 0a01 0201 06fb 0608  ................
-000008e0: 0201 12ff 0404 1401 0801 0e01 0802 0801  ................
-000008f0: 7a0e 4179 7543 6f6d 6d61 6e64 2e72 756e  z.AyuCommand.run
-00000900: 2901 da06 7265 7475 726e 6301 0000 0000  )...returnc.....
-00000910: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
-00000920: 0000 0073 1a00 0000 7400 7401 7401 7402  ...s....t.t.t.t.
-00000930: 6a03 6401 1900 6402 8302 6403 8302 8301  j.d...d...d.....
-00000940: 5300 2904 4e72 0100 0000 da09 7465 6d70  S.).Nr......temp
-00000950: 6c61 7465 73da 0770 726f 6a65 6374 2904  lates..project).
-00000960: 722a 0000 0072 0200 0000 da10 6179 7567  r*...r......ayug
-00000970: 6573 7069 6465 7274 6f6f 6c73 da08 5f5f  espidertools..__
-00000980: 7061 7468 5f5f 2901 722b 0000 0072 1900  path__).r+...r..
-00000990: 0000 7219 0000 0072 1a00 0000 7226 0000  ..r....r....r&..
-000009a0: 006a 0000 0073 0c00 0000 0003 0201 0201  .j...s..........
-000009b0: 0e01 02fe 02ff 7a18 4179 7543 6f6d 6d61  ......z.AyuComma
-000009c0: 6e64 2e74 656d 706c 6174 6573 5f64 6972  nd.templates_dir
-000009d0: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-000009e0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000009f0: 6c6e 616d 655f 5f72 2f00 0000 da08 7072  lname__r/.....pr
-00000a00: 6f70 6572 7479 722a 0000 0072 2600 0000  opertyr*...r&...
-00000a10: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00000a20: 1a00 0000 720e 0000 001f 0000 0073 0600  ....r........s..
-00000a30: 0000 0801 084a 0201 720e 0000 0029 1372  .....J..r....).r
-00000a40: 1400 0000 da07 7061 7468 6c69 6272 0200  ......pathlibr..
-00000a50: 0000 da06 7368 7574 696c 7203 0000 0072  ....shutilr....r
-00000a60: 0400 0000 5a1c 7363 7261 7079 2e63 6f6d  ....Z.scrapy.com
-00000a70: 6d61 6e64 732e 7374 6172 7470 726f 6a65  mands.startproje
-00000a80: 6374 7205 0000 00da 1173 6372 6170 792e  ctr......scrapy.
-00000a90: 6578 6365 7074 696f 6e73 7206 0000 00da  exceptionsr.....
-00000aa0: 1573 6372 6170 792e 7574 696c 732e 7465  .scrapy.utils.te
-00000ab0: 6d70 6c61 7465 7207 0000 0072 0800 0000  mplater....r....
-00000ac0: 7233 0000 00da 1e61 7975 6765 7370 6964  r3.....ayugespid
-00000ad0: 6572 746f 6f6c 732e 636f 6d6d 6f6e 2e70  ertools.common.p
-00000ae0: 6172 616d 7372 0900 0000 7227 0000 005a  aramsr....r'...Z
-00000af0: 0649 474e 4f52 4572 0e00 0000 7219 0000  .IGNOREr....r...
-00000b00: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000b10: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
-00000b20: 0000 0008 010c 0110 020c 010c 0110 0208  ................
-00000b30: 010c 0304 0f0c 03                        .......
+00000710: 7769 7468 2061 7975 6765 3a7a 2720 2020  with ayuge:z'   
+00000720: 2061 7975 6765 2067 656e 7370 6964 6572   ayuge genspider
+00000730: 2065 7861 6d70 6c65 2065 7861 6d70 6c65   example example
+00000740: 2e63 6f6d 2912 da03 6c65 6e72 0600 0000  .com)...lenr....
+00000750: 7202 0000 00da 0665 7869 7374 73da 0865  r......exists..e
+00000760: 7869 7463 6f64 65da 0570 7269 6e74 da07  xitcode..print..
+00000770: 7265 736f 6c76 655a 0e5f 6973 5f76 616c  resolveZ._is_val
+00000780: 6964 5f6e 616d 65da 095f 636f 7079 7472  id_name.._copytr
+00000790: 6565 da0d 7465 6d70 6c61 7465 735f 6469  ee..templates_di
+000007a0: 7272 0400 0000 da13 5445 4d50 4c41 5445  rr......TEMPLATE
+000007b0: 535f 544f 5f52 454e 4445 5272 0700 0000  S_TO_RENDERr....
+000007c0: 7208 0000 0072 0900 0000 da0a 4953 5f57  r....r......IS_W
+000007d0: 494e 444f 5753 da06 756e 6c69 6e6b da03  INDOWS..unlink..
+000007e0: 7374 7229 0ada 0473 656c 66da 0461 7267  str)...self..arg
+000007f0: 73da 046f 7074 735a 155f 6861 735f 7072  s..optsZ._has_pr
+00000800: 6f6a 6563 745f 6469 725f 6172 6773 5a0b  oject_dir_argsZ.
+00000810: 7072 6f6a 6563 745f 6469 72da 0570 6174  project_dir..pat
+00000820: 6873 5a07 7470 6c66 696c 655a 0e72 756e  hsZ.tplfileZ.run
+00000830: 5f73 6865 6c6c 5f70 6174 685a 1172 756e  _shell_pathZ.run
+00000840: 5f73 6865 6c6c 5f61 6273 7061 7468 5a08  _shell_abspathZ.
+00000850: 6465 6c5f 6669 6c65 7219 0000 0072 1200  del_filer....r..
+00000860: 0000 721a 0000 00da 0372 756e 2000 0000  ..r......run ...
+00000870: 7370 0000 0000 010c 0106 0208 020c 0104  sp..............
+00000880: 010e 0204 010c 020c 0106 0112 0104 020a  ................
+00000890: 0106 0104 0216 0112 0108 0102 0102 ff02  ................
+000008a0: 020a 0202 fe04 fe06 0702 0102 0102 0202  ................
+000008b0: 0106 fb08 0904 0112 0210 010c 0208 0108  ................
+000008c0: 0108 010c 010a 0302 0102 0102 010a 0102  ................
+000008d0: 0106 fb06 0802 0112 ff04 0414 0108 010e  ................
+000008e0: 0108 0208 017a 0e41 7975 436f 6d6d 616e  .....z.AyuComman
+000008f0: 642e 7275 6e29 01da 0672 6574 7572 6e63  d.run)...returnc
+00000900: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000910: 0500 0000 4300 0000 731a 0000 0074 0074  ....C...s....t.t
+00000920: 0174 0174 026a 0364 0119 0064 0283 0264  .t.t.j.d...d...d
+00000930: 0383 0283 0153 0029 044e 7201 0000 00da  .....S.).Nr.....
+00000940: 0974 656d 706c 6174 6573 da07 7072 6f6a  .templates..proj
+00000950: 6563 7429 0472 2a00 0000 7202 0000 00da  ect).r*...r.....
+00000960: 1061 7975 6765 7370 6964 6572 746f 6f6c  .ayugespidertool
+00000970: 73da 085f 5f70 6174 685f 5f29 0172 2b00  s..__path__).r+.
+00000980: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00000990: 0072 2600 0000 6a00 0000 730c 0000 0000  .r&...j...s.....
+000009a0: 0302 0102 010e 0102 fe02 ff7a 1841 7975  ...........z.Ayu
+000009b0: 436f 6d6d 616e 642e 7465 6d70 6c61 7465  Command.template
+000009c0: 735f 6469 724e 2907 da08 5f5f 6e61 6d65  s_dirN)...__name
+000009d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000009e0: 5f5f 7175 616c 6e61 6d65 5f5f 722f 0000  __qualname__r/..
+000009f0: 00da 0870 726f 7065 7274 7972 2a00 0000  ...propertyr*...
+00000a00: 7226 0000 0072 1900 0000 7219 0000 0072  r&...r....r....r
+00000a10: 1900 0000 721a 0000 0072 0e00 0000 1f00  ....r....r......
+00000a20: 0000 7306 0000 0008 0108 4a02 0172 0e00  ..s.......J..r..
+00000a30: 0000 2913 7214 0000 00da 0770 6174 686c  ..).r......pathl
+00000a40: 6962 7202 0000 00da 0673 6875 7469 6c72  ibr......shutilr
+00000a50: 0300 0000 7204 0000 005a 1c73 6372 6170  ....r....Z.scrap
+00000a60: 792e 636f 6d6d 616e 6473 2e73 7461 7274  y.commands.start
+00000a70: 7072 6f6a 6563 7472 0500 0000 da11 7363  projectr......sc
+00000a80: 7261 7079 2e65 7863 6570 7469 6f6e 7372  rapy.exceptionsr
+00000a90: 0600 0000 da15 7363 7261 7079 2e75 7469  ......scrapy.uti
+00000aa0: 6c73 2e74 656d 706c 6174 6572 0700 0000  ls.templater....
+00000ab0: 7208 0000 0072 3300 0000 da1e 6179 7567  r....r3.....ayug
+00000ac0: 6573 7069 6465 7274 6f6f 6c73 2e63 6f6d  espidertools.com
+00000ad0: 6d6f 6e2e 7061 7261 6d73 7209 0000 0072  mon.paramsr....r
+00000ae0: 2700 0000 5a06 4947 4e4f 5245 720e 0000  '...Z.IGNOREr...
+00000af0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
+00000b00: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000b10: 0000 0073 1400 0000 0801 0c01 1002 0c01  ...s............
+00000b20: 0c01 1002 0801 0c03 040f 0c03            ............
```

### Comparing `ayugespidertools-2.0.2/ayugespidertools/commands/__pycache__/version.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/commands/__pycache__/version.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/commands/startproject.py` & `ayugespidertools-2.0.3/ayugespidertools/commands/startproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             f"'{self.templates_dir}', created in:"
         )
         print(f"    {project_dir.resolve()}\n")
         print("You can start your first spider with:")
         print(f"    cd {project_dir}")
         print("    scrapy genspider example example.com")
         # 添加本库的文字提示内容
-        print("Or you can start your first spider with ayugespidertools:")
+        print("Or you can start your first spider with ayuge:")
         print("    ayuge genspider example example.com")
 
     @property
     def templates_dir(self) -> str:
         # 修改 startproject 模板文件路径为 ayugespidertools 的自定义路径
         return str(
             Path(
```

### Comparing `ayugespidertools-2.0.2/ayugespidertools/commands/version.py` & `ayugespidertools-2.0.3/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/encryption.py` & `ayugespidertools-2.0.3/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/expend.py` & `ayugespidertools-2.0.3/ayugespidertools/common/expend.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-2.0.3/ayugespidertools/common/mongodbpipe.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/multiplexing.py` & `ayugespidertools-2.0.3/ayugespidertools/common/multiplexing.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-2.0.3/ayugespidertools/common/mysqlerrhandle.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/params.py` & `ayugespidertools-2.0.3/ayugespidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/spiderdbconf.py` & `ayugespidertools-2.0.3/ayugespidertools/common/spiderdbconf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/sqlformat.py` & `ayugespidertools-2.0.3/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/typevars.py` & `ayugespidertools-2.0.3/ayugespidertools/common/typevars.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/utils.py` & `ayugespidertools-2.0.3/ayugespidertools/common/utils.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/common/yidungap.py` & `ayugespidertools-2.0.3/ayugespidertools/common/yidungap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/formatdata.py` & `ayugespidertools-2.0.3/ayugespidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/imgoperation.py` & `ayugespidertools-2.0.3/ayugespidertools/imgoperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/items.py` & `ayugespidertools-2.0.3/ayugespidertools/items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/middlewares.py` & `ayugespidertools-2.0.3/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/mongoclient.py` & `ayugespidertools-2.0.3/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/mysqlclient.py` & `ayugespidertools-2.0.3/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/oss.py` & `ayugespidertools-2.0.3/ayugespidertools/oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/pipelines.py` & `ayugespidertools-2.0.3/ayugespidertools/pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/rpa.py` & `ayugespidertools-2.0.3/ayugespidertools/rpa.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/runjs.py` & `ayugespidertools-2.0.3/ayugespidertools/runjs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/headers/__pycache__/ua.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/aiohttplib.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/__pycache__/requestslib.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/dynamic.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/exclusive.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/__pycache__/private.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/asynced.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/fantasy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/__pycache__/twisted.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/asynced.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/fantasy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/turbo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/__pycache__/twisted.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/project/.gitignore` & `ayugespidertools-2.0.3/ayugespidertools/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-2.0.3/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-2.0.3/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-2.0.3/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-2.0.3/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-2.0.3/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc` & `ayugespidertools-2.0.3/ayugespidertools/utils/__pycache__/cmdline.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 27 07:40:39 2023 UTC, .py size: 5920 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 f726 4a64 2017 0000  U........&Jd ...
+00000000: 550d 0d0a 0000 0000 bef4 5564 1517 0000  U.........Ud....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 2401 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
@@ -235,99 +235,99 @@
 00000ea0: 098d 0201 007c 017c 065f 127c 06a0 137c  .....|.|._.|...|
 00000eb0: 07a1 0101 007c 076a 147c 0064 0a64 0085  .....|.j.|.d.d..
 00000ec0: 0219 0064 0b8d 015c 027d 087d 0974 157c  ...d...\.}.}.t.|
 00000ed0: 077c 066a 167c 097c 0883 0401 0074 177c  .|.j.|.|.....t.|
 00000ee0: 0183 017c 065f 1874 157c 0774 197c 067c  ...|._.t.|.t.|.|
 00000ef0: 097c 0883 0501 0074 00a0 0a7c 066a 1aa1  .|.....t...|.j..
 00000f00: 0101 0064 0053 0029 0c4e da06 4544 4954  ...d.S.).N..EDIT
-00000f10: 4f52 7201 0000 0072 0c00 0000 7a11 6179  ORr....r....z.ay
-00000f20: 7567 6573 7069 6465 7274 6f6f 6c73 2072  ugespidertools r
-00000f30: 4700 0000 da07 7265 736f 6c76 6529 04da  G.....resolve)..
-00000f40: 0f66 6f72 6d61 7474 6572 5f63 6c61 7373  .formatter_class
-00000f50: da05 7573 6167 65da 1063 6f6e 666c 6963  ..usage..conflic
-00000f60: 745f 6861 6e64 6c65 72da 0b64 6573 6372  t_handler..descr
-00000f70: 6970 7469 6f6e da07 636f 6d6d 616e 6429  iption..command)
-00000f80: 01da 0870 7269 6f72 6974 7972 3800 0000  ...priorityr8...
-00000f90: 2901 723f 0000 0029 1b72 4f00 0000 723b  ).r?...).rO...r;
-00000fa0: 0000 0072 0700 0000 da02 6f73 da07 656e  ...r......os..en
-00000fb0: 7669 726f 6eda 084b 6579 4572 726f 7272  viron..KeyErrorr
-00000fc0: 0800 0000 7237 0000 0072 3e00 0000 724a  ....r7...r>...rJ
-00000fd0: 0000 0072 5000 0000 724b 0000 0072 0b00  ...rP...rK...r..
-00000fe0: 0000 7203 0000 005a 0673 796e 7461 785a  ..r....Z.syntaxZ
-00000ff0: 096c 6f6e 675f 6465 7363 da07 7365 7464  .long_desc..setd
-00001000: 6963 74da 1064 6566 6175 6c74 5f73 6574  ict..default_set
-00001010: 7469 6e67 7372 3600 0000 5a0b 6164 645f  tingsr6...Z.add_
-00001020: 6f70 7469 6f6e 73da 1070 6172 7365 5f6b  options..parse_k
-00001030: 6e6f 776e 5f61 7267 7372 5600 0000 5a0f  nown_argsrV...Z.
-00001040: 7072 6f63 6573 735f 6f70 7469 6f6e 7372  process_optionsr
-00001050: 0400 0000 5a0f 6372 6177 6c65 725f 7072  ....Z.crawler_pr
-00001060: 6f63 6573 73da 0c5f 7275 6e5f 636f 6d6d  ocess.._run_comm
-00001070: 616e 64da 0865 7869 7463 6f64 6529 0a72  and..exitcode).r
-00001080: 3b00 0000 7236 0000 005a 0665 6469 746f  ;...r6...Z.edito
-00001090: 7272 2600 0000 7231 0000 0072 2900 0000  rr&...r1...r)...
-000010a0: 7228 0000 0072 5100 0000 7240 0000 0072  r(...rQ...r@...r
-000010b0: 3f00 0000 7213 0000 0072 1300 0000 7214  ?...r....r....r.
-000010c0: 0000 00da 0765 7865 6375 7465 7700 0000  .....executew...
-000010d0: 7342 0000 0000 0108 0106 0208 0106 0202  sB..............
-000010e0: 010e 010e 0106 0208 0206 010a 0108 0104  ................
-000010f0: 010a 010c 0108 010c 010a 0208 0102 0102  ................
-00001100: 0112 0102 0106 fc06 0610 0106 010a 0118  ................
-00001110: 0110 020a 0110 0172 6700 0000 6303 0000  .......rg...c...
-00001120: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00001130: 0043 0000 0073 2400 0000 7c02 6a00 7214  .C...s$...|.j.r.
-00001140: 7401 7c00 7c01 7c02 8303 0100 6e0c 7c00  t.|.|.|.....n.|.
-00001150: a002 7c01 7c02 a102 0100 6400 5300 7219  ..|.|.....d.S.r.
-00001160: 0000 0029 03da 0770 726f 6669 6c65 da15  ...)...profile..
-00001170: 5f72 756e 5f63 6f6d 6d61 6e64 5f70 726f  _run_command_pro
-00001180: 6669 6c65 6472 4300 0000 2903 7228 0000  filedrC...).r(..
-00001190: 0072 3f00 0000 7240 0000 0072 1300 0000  .r?...r@...r....
-000011a0: 7213 0000 0072 1400 0000 7265 0000 00a1  r....r....re....
-000011b0: 0000 0073 0600 0000 0001 0601 0e02 7265  ...s..........re
-000011c0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-000011d0: 0500 0000 0500 0000 4300 0000 7350 0000  ........C...sP..
-000011e0: 007c 026a 0072 1c74 016a 02a0 0364 017c  .|.j.r.t.j...d.|
-000011f0: 026a 009b 0264 029d 03a1 0101 0074 0483  .j...d.......t..
-00001200: 007d 0374 05a0 06a1 007d 047c 04a0 0764  .}.t.....}.|...d
-00001210: 0374 0883 007c 03a1 0301 007c 026a 0072  .t...|.....|.j.r
-00001220: 4c7c 04a0 097c 026a 00a1 0101 0064 0053  L|...|.j.....d.S
-00001230: 0029 044e 7a2c 6179 7567 6573 7069 6465  .).Nz,ayugespide
-00001240: 7274 6f6f 6c73 3a20 7772 6974 696e 6720  rtools: writing 
-00001250: 6350 726f 6669 6c65 2073 7461 7473 2074  cProfile stats t
-00001260: 6f20 7242 0000 007a 1363 6d64 2e72 756e  o rB...z.cmd.run
-00001270: 2861 7267 732c 206f 7074 7329 290a 7268  (args, opts)).rh
-00001280: 0000 0072 4f00 0000 da06 7374 6465 7272  ...rO.....stderr
-00001290: da05 7772 6974 65da 066c 6f63 616c 73da  ..write..locals.
-000012a0: 0863 5072 6f66 696c 655a 0750 726f 6669  .cProfileZ.Profi
-000012b0: 6c65 5a06 7275 6e63 7478 da07 676c 6f62  leZ.runctx..glob
-000012c0: 616c 735a 0a64 756d 705f 7374 6174 7329  alsZ.dump_stats)
-000012d0: 0572 2800 0000 723f 0000 0072 4000 0000  .r(...r?...r@...
-000012e0: da03 6c6f 63da 0170 7213 0000 0072 1300  ..loc..pr....r..
-000012f0: 0000 7214 0000 0072 6900 0000 a800 0000  ..r....ri.......
-00001300: 7312 0000 0000 0106 0106 010c ff04 0306  s...............
-00001310: 0108 0110 0106 0172 6900 0000 da08 5f5f  .......ri.....__
-00001320: 6d61 696e 5f5f 2901 722b 0000 0029 024e  main__).r+...).N
-00001330: 4e29 25da 0861 7267 7061 7273 6572 6d00  N)%..argparserm.
-00001340: 0000 721c 0000 0072 5f00 0000 724f 0000  ..r....r_...rO..
-00001350: 0072 2c00 0000 5a0f 7363 7261 7079 2e63  .r,...Z.scrapy.c
-00001360: 6f6d 6d61 6e64 7372 0200 0000 7203 0000  ommandsr....r...
-00001370: 005a 0e73 6372 6170 792e 6372 6177 6c65  .Z.scrapy.crawle
-00001380: 7272 0400 0000 da11 7363 7261 7079 2e65  rr......scrapy.e
-00001390: 7863 6570 7469 6f6e 7372 0500 0000 da11  xceptionsr......
-000013a0: 7363 7261 7079 2e75 7469 6c73 2e6d 6973  scrapy.utils.mis
-000013b0: 6372 0600 0000 5a14 7363 7261 7079 2e75  cr....Z.scrapy.u
-000013c0: 7469 6c73 2e70 726f 6a65 6374 7207 0000  tils.projectr...
-000013d0: 0072 0800 0000 da13 7363 7261 7079 2e75  .r......scrapy.u
-000013e0: 7469 6c73 2e70 7974 686f 6e72 0900 0000  tils.pythonr....
-000013f0: 5a21 6179 7567 6573 7069 6465 7274 6f6f  Z!ayugespidertoo
-00001400: 6c73 2e63 6f6d 6d61 6e64 732e 7665 7273  ls.commands.vers
-00001410: 696f 6e72 0a00 0000 da0e 4172 6775 6d65  ionr......Argume
-00001420: 6e74 5061 7273 6572 720b 0000 0072 2200  ntParserr....r".
-00001430: 0000 722a 0000 0072 3300 0000 7237 0000  ..r*...r3...r7..
-00001440: 0072 3e00 0000 7246 0000 0072 4a00 0000  .r>...rF...rJ...
-00001450: 724b 0000 0072 5600 0000 7267 0000 0072  rK...rV...rg...r
-00001460: 6500 0000 7269 0000 0072 1500 0000 7213  e...ri...r....r.
-00001470: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00001480: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001490: 733a 0000 0008 0108 0108 0108 0108 0208  s:..............
-000014a0: 0110 010c 010c 010c 0110 010c 020c 0312  ................
-000014b0: 0908 0e08 090a 0b08 0908 0908 0808 0f08  ................
-000014c0: 0608 0b0a 2a08 0708 0c0a 0102 010a 05    ....*..........
+00000f10: 4f52 7201 0000 0072 0c00 0000 7a06 6179  ORr....r....z.ay
+00000f20: 7567 6520 7247 0000 00da 0772 6573 6f6c  uge rG.....resol
+00000f30: 7665 2904 da0f 666f 726d 6174 7465 725f  ve)...formatter_
+00000f40: 636c 6173 73da 0575 7361 6765 da10 636f  class..usage..co
+00000f50: 6e66 6c69 6374 5f68 616e 646c 6572 da0b  nflict_handler..
+00000f60: 6465 7363 7269 7074 696f 6eda 0763 6f6d  description..com
+00000f70: 6d61 6e64 2901 da08 7072 696f 7269 7479  mand)...priority
+00000f80: 7238 0000 0029 0172 3f00 0000 291b 724f  r8...).r?...).rO
+00000f90: 0000 0072 3b00 0000 7207 0000 00da 026f  ...r;...r......o
+00000fa0: 73da 0765 6e76 6972 6f6e da08 4b65 7945  s..environ..KeyE
+00000fb0: 7272 6f72 7208 0000 0072 3700 0000 723e  rrorr....r7...r>
+00000fc0: 0000 0072 4a00 0000 7250 0000 0072 4b00  ...rJ...rP...rK.
+00000fd0: 0000 720b 0000 0072 0300 0000 5a06 7379  ..r....r....Z.sy
+00000fe0: 6e74 6178 5a09 6c6f 6e67 5f64 6573 63da  ntaxZ.long_desc.
+00000ff0: 0773 6574 6469 6374 da10 6465 6661 756c  .setdict..defaul
+00001000: 745f 7365 7474 696e 6773 7236 0000 005a  t_settingsr6...Z
+00001010: 0b61 6464 5f6f 7074 696f 6e73 da10 7061  .add_options..pa
+00001020: 7273 655f 6b6e 6f77 6e5f 6172 6773 7256  rse_known_argsrV
+00001030: 0000 005a 0f70 726f 6365 7373 5f6f 7074  ...Z.process_opt
+00001040: 696f 6e73 7204 0000 005a 0f63 7261 776c  ionsr....Z.crawl
+00001050: 6572 5f70 726f 6365 7373 da0c 5f72 756e  er_process.._run
+00001060: 5f63 6f6d 6d61 6e64 da08 6578 6974 636f  _command..exitco
+00001070: 6465 290a 723b 0000 0072 3600 0000 5a06  de).r;...r6...Z.
+00001080: 6564 6974 6f72 7226 0000 0072 3100 0000  editorr&...r1...
+00001090: 7229 0000 0072 2800 0000 7251 0000 0072  r)...r(...rQ...r
+000010a0: 4000 0000 723f 0000 0072 1300 0000 7213  @...r?...r....r.
+000010b0: 0000 0072 1400 0000 da07 6578 6563 7574  ...r......execut
+000010c0: 6577 0000 0073 4200 0000 0001 0801 0602  ew...sB.........
+000010d0: 0801 0602 0201 0e01 0e01 0602 0802 0601  ................
+000010e0: 0a01 0801 0401 0a01 0c01 0801 0c01 0a02  ................
+000010f0: 0801 0201 0201 1201 0201 06fc 0606 1001  ................
+00001100: 0601 0a01 1801 1002 0a01 1001 7267 0000  ............rg..
+00001110: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
+00001120: 0000 0400 0000 4300 0000 7324 0000 007c  ......C...s$...|
+00001130: 026a 0072 1474 017c 007c 017c 0283 0301  .j.r.t.|.|.|....
+00001140: 006e 0c7c 00a0 027c 017c 02a1 0201 0064  .n.|...|.|.....d
+00001150: 0053 0072 1900 0000 2903 da07 7072 6f66  .S.r....)...prof
+00001160: 696c 65da 155f 7275 6e5f 636f 6d6d 616e  ile.._run_comman
+00001170: 645f 7072 6f66 696c 6564 7243 0000 0029  d_profiledrC...)
+00001180: 0372 2800 0000 723f 0000 0072 4000 0000  .r(...r?...r@...
+00001190: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+000011a0: 6500 0000 a100 0000 7306 0000 0000 0106  e.......s.......
+000011b0: 010e 0272 6500 0000 6303 0000 0000 0000  ...re...c.......
+000011c0: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
+000011d0: 0073 5000 0000 7c02 6a00 721c 7401 6a02  .sP...|.j.r.t.j.
+000011e0: a003 6401 7c02 6a00 9b02 6402 9d03 a101  ..d.|.j...d.....
+000011f0: 0100 7404 8300 7d03 7405 a006 a100 7d04  ..t...}.t.....}.
+00001200: 7c04 a007 6403 7408 8300 7c03 a103 0100  |...d.t...|.....
+00001210: 7c02 6a00 724c 7c04 a009 7c02 6a00 a101  |.j.rL|...|.j...
+00001220: 0100 6400 5300 2904 4e7a 2c61 7975 6765  ..d.S.).Nz,ayuge
+00001230: 7370 6964 6572 746f 6f6c 733a 2077 7269  spidertools: wri
+00001240: 7469 6e67 2063 5072 6f66 696c 6520 7374  ting cProfile st
+00001250: 6174 7320 746f 2072 4200 0000 7a13 636d  ats to rB...z.cm
+00001260: 642e 7275 6e28 6172 6773 2c20 6f70 7473  d.run(args, opts
+00001270: 2929 0a72 6800 0000 724f 0000 00da 0673  )).rh...rO.....s
+00001280: 7464 6572 72da 0577 7269 7465 da06 6c6f  tderr..write..lo
+00001290: 6361 6c73 da08 6350 726f 6669 6c65 5a07  cals..cProfileZ.
+000012a0: 5072 6f66 696c 655a 0672 756e 6374 78da  ProfileZ.runctx.
+000012b0: 0767 6c6f 6261 6c73 5a0a 6475 6d70 5f73  .globalsZ.dump_s
+000012c0: 7461 7473 2905 7228 0000 0072 3f00 0000  tats).r(...r?...
+000012d0: 7240 0000 00da 036c 6f63 da01 7072 1300  r@.....loc..pr..
+000012e0: 0000 7213 0000 0072 1400 0000 7269 0000  ..r....r....ri..
+000012f0: 00a8 0000 0073 1200 0000 0001 0601 0601  .....s..........
+00001300: 0cff 0403 0601 0801 1001 0601 7269 0000  ............ri..
+00001310: 00da 085f 5f6d 6169 6e5f 5f29 0172 2b00  ...__main__).r+.
+00001320: 0000 2902 4e4e 2925 da08 6172 6770 6172  ..).NN)%..argpar
+00001330: 7365 726d 0000 0072 1c00 0000 725f 0000  serm...r....r_..
+00001340: 0072 4f00 0000 722c 0000 005a 0f73 6372  .rO...r,...Z.scr
+00001350: 6170 792e 636f 6d6d 616e 6473 7202 0000  apy.commandsr...
+00001360: 0072 0300 0000 5a0e 7363 7261 7079 2e63  .r....Z.scrapy.c
+00001370: 7261 776c 6572 7204 0000 00da 1173 6372  rawlerr......scr
+00001380: 6170 792e 6578 6365 7074 696f 6e73 7205  apy.exceptionsr.
+00001390: 0000 00da 1173 6372 6170 792e 7574 696c  .....scrapy.util
+000013a0: 732e 6d69 7363 7206 0000 005a 1473 6372  s.miscr....Z.scr
+000013b0: 6170 792e 7574 696c 732e 7072 6f6a 6563  apy.utils.projec
+000013c0: 7472 0700 0000 7208 0000 00da 1373 6372  tr....r......scr
+000013d0: 6170 792e 7574 696c 732e 7079 7468 6f6e  apy.utils.python
+000013e0: 7209 0000 005a 2161 7975 6765 7370 6964  r....Z!ayugespid
+000013f0: 6572 746f 6f6c 732e 636f 6d6d 616e 6473  ertools.commands
+00001400: 2e76 6572 7369 6f6e 720a 0000 00da 0e41  .versionr......A
+00001410: 7267 756d 656e 7450 6172 7365 7272 0b00  rgumentParserr..
+00001420: 0000 7222 0000 0072 2a00 0000 7233 0000  ..r"...r*...r3..
+00001430: 0072 3700 0000 723e 0000 0072 4600 0000  .r7...r>...rF...
+00001440: 724a 0000 0072 4b00 0000 7256 0000 0072  rJ...rK...rV...r
+00001450: 6700 0000 7265 0000 0072 6900 0000 7215  g...re...ri...r.
+00001460: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
+00001470: 0000 7214 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00001480: 3e01 0000 0073 3a00 0000 0801 0801 0801  >....s:.........
+00001490: 0801 0802 0801 1001 0c01 0c01 0c01 1001  ................
+000014a0: 0c02 0c03 1209 080e 0809 0a0b 0809 0809  ................
+000014b0: 0808 080f 0806 080b 0a2a 0807 080c 0a01  .........*......
+000014c0: 0201 0a05                                ....
```

### Comparing `ayugespidertools-2.0.2/ayugespidertools/utils/cmdline.py` & `ayugespidertools-2.0.3/ayugespidertools/utils/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     elif cmdname not in cmds:
         _print_unknown_command(settings, cmdname, inproject)
         sys.exit(2)
 
     cmd = cmds[cmdname]
     parser = ScrapyArgumentParser(
         formatter_class=ScrapyHelpFormatter,
-        usage=f"ayugespidertools {cmdname} {cmd.syntax()}",
+        usage=f"ayuge {cmdname} {cmd.syntax()}",
         conflict_handler="resolve",
         description=cmd.long_desc(),
     )
     settings.setdict(cmd.default_settings, priority="command")
     cmd.settings = settings
     cmd.add_options(parser)
     opts, args = parser.parse_known_args(args=argv[1:])
```

### Comparing `ayugespidertools-2.0.2/ayugespidertools/verificationcode.py` & `ayugespidertools-2.0.3/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-2.0.2/pyproject.toml` & `ayugespidertools-2.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "2.0.2"
+version = "2.0.3"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -36,29 +36,33 @@
 pycryptodome = "^3.15.0"
 oss2 = "^2.16.0"
 aiomysql = "^0.1.1"
 attrs = "^22.2.0"
 toml = "^0.10.2"
 python-hcl2 = "^4.3.0"
 motor = "2.5.1"
+urllib3 = "~1.26.15"
 
 [tool.poetry.scripts]
 ayuge = "ayugespidertools.utils.cmdline:execute"
 ayugespidertools = "ayugespidertools.utils.cmdline:execute"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^23.1.0"
 isort = "^5.12.0"
-sphinx-rtd-theme = "^1.2.0"
-recommonmark = "^0.7.1"
+sphinx-rtd-theme = "1.2.0"
 coverage = "^7.2.2"
 tox = "^4.4.8"
 flake8 = "^6.0.0"
 testfixtures = "^7.1.0"
+myst-parser = "1.0.0"
+sphinx-markdown-tables = "0.0.17"
+sphinx-hoverxref = "1.3.0"
+sphinx-notfound-page = "0.8.3"
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple"
 
 [tool.pytest.ini_options]
 xfail_strict = true
```

### Comparing `ayugespidertools-2.0.2/PKG-INFO` & `ayugespidertools-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 2.0.2
+Version: 2.0.3
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -35,14 +35,15 @@
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
 Requires-Dist: pymongo (>=3.12.3,<4.0.0)
 Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: urllib3 (>=1.26.15,<1.27.0)
 Project-URL: Documentation, https://ayugespidertools.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/shengchenyang/AyugeSpiderTools
 Description-Content-Type: text/markdown
 
 ![ayugespidertools-logo](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/artwork/ayugespidertools-logo.png)
 
 [![OSCS Status](https://www.oscs1024.com/platform/badge/AyugeSpiderTools.svg?size=small)](https://www.murphysec.com/accept?code=0ec375759aebea7fd260248910b98806&type=1&from=2)
```

