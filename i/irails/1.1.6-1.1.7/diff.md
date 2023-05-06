# Comparing `tmp/irails-1.1.6.tar.gz` & `tmp/irails-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.1.6.tar", last modified: Fri May  5 14:48:27 2023, max compression
+gzip compressed data, was "irails-1.1.7.tar", last modified: Sat May  6 13:42:28 2023, max compression
```

## Comparing `irails-1.1.6.tar` & `irails-1.1.7.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.564814 irails-1.1.6/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     7120 2023-05-05 14:48:27.564814 irails-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     6339 2023-05-05 14:48:27.000000 irails-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.505604 irails-1.1.6/irails/
--rw-rw-rw-   0        0        0      318 2023-05-05 14:48:24.000000 irails-1.1.6/irails/__init__.py
--rw-rw-rw-   0        0        0     1921 2023-05-05 06:08:39.000000 irails-1.1.6/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.6/irails/_utils.py
--rw-rw-rw-   0        0        0    11702 2023-05-04 04:55:19.000000 irails-1.1.6/irails/auth.py
--rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.6/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.515577 irails-1.1.6/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.516575 irails-1.1.6/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.6/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.6/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.6/irails/cbv.py
--rw-rw-rw-   0        0        0     6656 2023-05-05 08:24:35.000000 irails-1.1.6/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.6/irails/controller.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.6/irails/controller_utils.py
--rw-rw-rw-   0        0        0    14397 2023-05-05 11:09:47.000000 irails-1.1.6/irails/core.py
--rw-rw-rw-   0        0        0     6338 2023-05-05 11:07:47.000000 irails-1.1.6/irails/database.py
--rw-rw-rw-   0        0        0     8134 2023-05-05 14:29:33.000000 irails-1.1.6/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.6/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.6/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.522347 irails-1.1.6/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.6/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7785 2023-05-05 10:17:36.000000 irails-1.1.6/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     8189 2023-05-05 06:14:02.000000 irails-1.1.6/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.6/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.6/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.6/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.476691 irails-1.1.6/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.533316 irails-1.1.6/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.6/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.6/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.6/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.1.6/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.6/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.6/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.6/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.6/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.535311 irails-1.1.6/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.6/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.537306 irails-1.1.6/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.6/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.547287 irails-1.1.6/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.6/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.6/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.6/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.6/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.6/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.6/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.6/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.6/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.550379 irails-1.1.6/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.6/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.6/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.552376 irails-1.1.6/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.483663 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.555382 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.559357 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.485657 irails-1.1.6/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.562350 irails-1.1.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.1.6/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.513583 irails-1.1.6/irails.egg-info/
--rw-rw-rw-   0        0        0     7120 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      753 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 14:48:27.565813 irails-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.615230 irails-1.1.7/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     7120 2023-05-06 13:42:28.613235 irails-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6339 2023-05-06 13:42:28.000000 irails-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.553960 irails-1.1.7/irails/
+-rw-rw-rw-   0        0        0      325 2023-05-06 13:42:16.000000 irails-1.1.7/irails/__init__.py
+-rw-rw-rw-   0        0        0     4239 2023-05-06 13:29:30.000000 irails-1.1.7/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.1.7/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.7/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.1.7/irails/auth.py
+-rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.7/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.562371 irails-1.1.7/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.563370 irails-1.1.7/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.7/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.7/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.7/irails/cbv.py
+-rw-rw-rw-   0        0        0     7252 2023-05-06 13:39:48.000000 irails-1.1.7/irails/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.7/irails/controller.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.7/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    14707 2023-05-06 10:10:49.000000 irails-1.1.7/irails/core.py
+-rw-rw-rw-   0        0        0     6338 2023-05-05 11:07:47.000000 irails-1.1.7/irails/database.py
+-rw-rw-rw-   0        0        0     8134 2023-05-05 14:29:33.000000 irails-1.1.7/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.7/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.7/irails/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.571348 irails-1.1.7/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.7/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7813 2023-05-06 13:37:52.000000 irails-1.1.7/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7603 2023-05-06 13:40:20.000000 irails-1.1.7/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     1416 2023-05-06 13:40:43.000000 irails-1.1.7/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.7/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.7/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.7/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.521452 irails-1.1.7/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.580325 irails-1.1.7/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.7/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.7/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.7/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.1.7/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.7/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.7/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.7/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.7/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.585318 irails-1.1.7/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.7/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.586309 irails-1.1.7/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.7/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.594287 irails-1.1.7/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.7/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.7/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.7/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.7/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.7/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.7/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.7/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.7/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.596281 irails-1.1.7/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.7/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.7/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.601277 irails-1.1.7/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.527423 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.604259 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.609246 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.527423 irails-1.1.7/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.610243 irails-1.1.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.1.7/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.560377 irails-1.1.7/irails.egg-info/
+-rw-rw-rw-   0        0        0     7120 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      753 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 13:42:28.615230 irails-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.7/setup.py
```

### Comparing `irails-1.1.6/PKG-INFO` & `irails-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.6
+Version: 1.1.7
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.6/README.md` & `irails-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/_loader.py` & `irails-1.1.7/irails/_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import importlib
 import sys,os
 from .config import config,ROOT_PATH,_log
+from ._i18n import load_app_translations
+from gettext import gettext as _
 app_cfg=config.get('app')
 app_dirs = app_cfg.get("appdir")
 app_enabled = app_cfg.get("enabled")
 
 def __list_directories(dir):
     """
     return all subdirectory under :dir
@@ -30,32 +32,36 @@
         return module
     return None
 def _load_app(app_dir):
     try:
         _path = os.path.join(ROOT_PATH,app_dir.split(".")[0])
         if _path not in sys.path:
             sys.path.insert(-1,_path)
-        _log.info(f'Loading app: {app_dir}')
-        __import__(app_dir)
-        return True
+        _log.info(_('Loading app:%s')%app_dir)
+        return importlib.import_module(app_dir)
+          
     except ImportError as e:
-        _log.error(f"load app{app_dir} failed")
+        _log.error(_("load app %s failed")%app_dir)
         _log.error(e.args)
         raise e
     
 def _load_apps(debug=False):
     if ROOT_PATH not in sys.path:
         sys.path.insert(-1,ROOT_PATH)
     unloaded = 0
     loaded = 0
     for app_dir in app_dirs:
         app_list =  __list_directories(app_dir)
         for app in app_list:
             if __check_if_enabled(app):  
-                if _load_app(f'{app_dir}.{app}'):
+                _dir = os.path.join(app_dir,app)
+                module = _load_app(f'{app_dir}.{app}')
+                if module:
+                    t =  load_app_translations(_dir)
+                    setattr(module,"_translation",t)
                     loaded = loaded + 1
                 else:
                     unloaded = unloaded + 1
             else:
                 unloaded = unloaded + 1
```

### Comparing `irails-1.1.6/irails/_utils.py` & `irails-1.1.7/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/auth.py` & `irails-1.1.7/irails/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # from .midware_casbin import CasbinMiddleware
  
 from .config import config,_log
 import jwt
 from datetime import datetime, timedelta
 from typing import Optional, Tuple, Type, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
+
 AUTH_EXPIRED='[EXPIRED]!'
 
 _session_name:str = ""
 
 class CasbinAuth:
     def __init__(self,enforcer:Enforcer,session_name="user") -> None:
         global _session_name
```

### Comparing `irails-1.1.6/irails/base_controller.py` & `irails-1.1.7/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.1.7/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.1.7/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/cbv.py` & `irails-1.1.7/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/config.py` & `irails-1.1.7/irails/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,32 @@
 import os,sys
 import yaml
 import logging
 from hashlib import md5
 from typing import Dict
 import os.path
 import re
-
+def is_in_app(directory):
+    """
+    check exists controllers , views dir in :directory
+    """
+    
+    controller_dir = os.path.join(directory, 'controllers')
+    views_dir = os.path.join(directory, 'views')  
+    if not os.path.exists(controller_dir):
+        print(f"can't location `controller` dir")
+        return False  
+    if  not os.path.exists(views_dir) :
+        print(f"can't location `views` dir")
+        return False
+    # initfile = os.path.join(controller_dir, '__init__.py') 
+    # if not os.path.exists(initfile):
+    #     return False
+    
+    return True
 def is_in_irails(directory):
     """
     check exists configs dir,   main.py and configs/general.yaml 
     """
     
     configs_dir = os.path.join(directory, 'configs')
     main_file = os.path.join(directory, 'main.py')
```

### Comparing `irails-1.1.6/irails/controller.py` & `irails-1.1.7/irails/controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/controller_utils.py` & `irails-1.1.7/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/core.py` & `irails-1.1.7/irails/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,24 @@
 from .config import config,ROOT_PATH,_log
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 from . import database
 from ._utils import get_controller_name,get_snaked_name
-
+from ._i18n import load_app_translations
+_=None
 __is_debug=config.get('debug',False)
 
+def __load_core_i18n():
+    _dir = os.path.dirname(__file__)
+    t = load_app_translations(_dir,True)
+    global _
+    _ = t.gettext
+__load_core_i18n()
 
 class MvcApp(FastAPI):
     def __init__(self,  **kwargs):
         self.__authObj:auth.AuthenticationBackend_ = None 
         self._data_engine:database.Engine = None
         self.__user_auth_url=""
         self.__public_auth_url=""
@@ -31,25 +38,25 @@
     @property
     def public_auth_url(self):
         """public user auth url"""
         return self.__public_auth_url
     @public_auth_url.setter
     def public_auth_url(self,url):
         if self.__public_auth_url:
-            raise RuntimeError(f"public_auth_url only can be setting once time,current is:{self.__public_auth_url}")
+            raise RuntimeError(_("public_auth_url only can be setting once time,current is:%s") % self.__public_auth_url)
         self.__public_auth_url = url
         
     @property
     def user_auth_url(self):
         """internal user auth url"""
         return self.__user_auth_url
     @user_auth_url.setter
     def user_auth_url(self,url):
         if self.__user_auth_url:
-            raise RuntimeError(f"user_auth_url only can be setting once time,current is:{self.__user_auth_url}")
+            raise RuntimeError(_("user_auth_url only can be setting once time,current is:%s") % self.__user_auth_url)
         self.__user_auth_url = url
     @property
     def modify_authorization(self):
         return self.__authObj.casbin_auth.modify_authorization
     @property
     def authObj(self)->auth.AuthenticationBackend_:
         return self.__authObj
@@ -77,23 +84,23 @@
 def check_init_database(): 
     db_cfg = config.get("database")
     db_uri:str = db_cfg.get("uri")
     alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
     if db_uri: 
         application.data_engine=database.init_database(db_uri,__is_debug, alembic_ini,cfg=db_cfg)
     else:
-        _log.warn(f"Warning: database.uri is empty in config")
+        _log.warn(_("Warning: database.uri is empty in config"))
     return db_cfg
 
 def __init_auth(app,auth_type:str,casbin_adapter_class,__adapter_uri):
     
     
     auth_class = auth.get_auth_backend(auth_type)
     if not auth_class:
-        raise f"{auth_type} auth type not support"
+        raise RuntimeError(_("%s auth type not support") % auth_type)
     
     
     secret_key = config.get("auth").get(f"{auth_type}_key","")
     kwargs = {'secret_key':secret_key,'adapter_uri':__adapter_uri} 
     return auth.init(app=app, backend = auth_class,adapter_class=casbin_adapter_class, **kwargs)
 
 
@@ -112,15 +119,15 @@
         app_dir = os.sep.join(relative_path.split(os.sep)[:-2]) # os.path.dirname(os.path.dirname(relative_path)).replace(os.sep,"")
     else:
         app_dir = "app"
     app_dir = os.path.join(ROOT_PATH,app_dir.lstrip(os.sep))
 
     def format_path(p,v):
         if p and not p.startswith("/"):
-            raise RuntimeError(f"route path must start with '/',{p} is not alowed!")
+            raise RuntimeError(_("route path must start with '/',%s is not alowed!") % p)
         if p and  '{controller}' not in p :
             p += '/{controller}' 
             p += '/{version}' if v else ''
         if v and not path:
             p = "/{controller}/{version}"
         return p
     path = format_path(path,version) 
@@ -133,25 +140,25 @@
     def _wapper(targetController):  
         
         class puppetController( targetController ,_controllerBase ): 
             '''puppet class inherited by the User defined controller class '''
             def __init__(self,**kwags) -> None: 
                 
                 super().__init__()
-            def _user_logout(self,msg='your are successed logout!',redirect:str="/"):
+            def _user_logout(self,msg=_('your are successed logout!'),redirect:str="/"):
                 """see .core.py"""
                 self.flash  = msg
                 if  hasattr(application,'authObj'):
                     application.authObj.clear_userinfo(request=self.request)
                 accept_header = self.request.headers.get("Accept")    
                 if accept_header == "application/json":
                     return {'status':'success','msg':msg}
                 else:
                     return self.redirect(redirect)
-            def _verity_successed(self,user, msg="User authentication successed!",redirect_url='/'):
+            def _verity_successed(self,user, msg=_("User authentication successed!"),redirect_url='/'):
                 '''call by targetController''' 
                  
                 self.flash  = msg
                 accept_header = self._request.headers.get("Accept")
                 if  hasattr(application,'authObj'):
                     access_token = application.authObj.create_access_token(user,request=self.request)
                 
@@ -159,15 +166,15 @@
                         return {'status':'success','msg':msg,'token':str(access_token)}
                      
                 else:  
                     if accept_header == "application/json":
                         return {'status':'success','msg':msg }
                  
                 return RedirectResponse(redirect_url,status_code=StateCodes.HTTP_303_SEE_OTHER)
-            def _verity_error(self,msg="User authentication failed!"):
+            def _verity_error(self,msg=_("User authentication failed!")):
                 '''call by targetController'''
                  
                 self.flash  = msg 
                 
                 accept_header = self.request.headers.get("Accept")
                 if accept_header == "application/json":
                     return JSONResponse(content={'status':StateCodes.HTTP_200_OK,'msg':msg})
@@ -181,46 +188,46 @@
                 
                 if not hasattr(application,'authObj') or application.authObj is None:
                     return True,None
                 
                 kwargs['session'] = request.session  
                 ret,user = await application.authObj.authenticate(request,**kwargs)
                 if user==auth.AUTH_EXPIRED:
-                    request.session['flash']  = "your authencation has been expired!"  
+                    request.session['flash']  = _("your authencation has been expired!"  )
                     user = False
                 if auth_type=='none':
                     return True,user
                 def add_redirect_param(url: str, redirect_url: str) -> str:
                     if "?" in url:
                         return url + "&redirect=" + redirect_url
                     else:
                         return url + "?redirect=" + redirect_url
                 accept_header = request.headers.get("Accept")
                 if user: #continue singture 
                     if config.get("session").get('auto_refresh_token',True):
                         application.authObj.create_access_token(user=user, expires_delta=None,request=request)
                 #
                 if not ret and not user: 
-                    _log.debug(f'Failed Auth[type:{auth_type}] url:'+str(request.url))
+                    _log.debug(_('Failed Auth on type:%s at url:%s') % (auth_type,str(request.url)))
                     if accept_header == "application/json":
                         return  ORJSONResponse(content={"message": "401 UNAUTHORIZED!"},
                                                    status_code=StateCodes.HTTP_401_UNAUTHORIZED),None
                     _auth_url = getattr(application,f"{auth_type}_auth_url") 
 
                     if _auth_url: 
                         if 'flash' not in request.session:
                             request.session['flash']=''
                         if request.session['flash']=="":
-                            request.session['flash']  = "you are not authenticated,please login!"  
+                            request.session['flash']  = _("you are not authenticated,please login!")
                         _auth_url = add_redirect_param(_auth_url,str(request.url))
                         return RedirectResponse(_auth_url,status_code=StateCodes.HTTP_303_SEE_OTHER),None
                     else:  
                         return RedirectResponse('/',status_code=StateCodes.HTTP_303_SEE_OTHER),None
                 else:
-                    _log.debug(f'Successed Auth[type:{auth_type}] Url:'+str(request.url)+',User:'+str(user))
+                    _log.debug(_('Successed Auth on %s at url:%s [User:%s]') % (auth_type,str(request.url),str(user)) )
                     return ret,user
 
         setattr(puppetController,AUTH_KEY,allargs['auth'])         
         setattr(puppetController,"__name__",targetController.__name__)  
         controller_name = get_controller_name(targetController.__name__)
         setattr(puppetController,"__controller_name__",controller_name)  
         
@@ -279,56 +286,56 @@
             all_routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type}
     application.routers_map = all_routers_map  
 def generate_mvc_app( ):
     global __is_debug
     _log.disabled = False
     from ._loader import _load_apps
     
-    _log.info("\n\init mvc app...")
+    _log.info(_("\n\init mvc app..."))
     loaded,unloaded=_load_apps(debug=__is_debug) 
-    _log.info(f'Load Apps Completed,{loaded} loaded,{unloaded} unloaded')  
+    _log.info(_('Load Apps Completed,%s loaded,%s unloaded') %(loaded,unloaded))  
     if not len(__all_controller__)>0:
-        raise RuntimeError("must use @api_route to define a controller class")
+        raise RuntimeError(_("not found any controller class"))
     
     _register_controllers()
 
-    _log.info("static files mouting...")
+    _log.info(_("static files mouting..."))
     midware.init(app=application,debug=__is_debug)
 
     if __is_debug:
-        _log.info("checking database configure...")
+        _log.info(_("checking database configure..."))
     db_cfg = check_init_database()
     auth_type = config.get("auth",None)
     _casbin_adapter_class=None
     _adapter_uri:str=None
     if auth_type:
         auth_type=auth_type.get("type" )
         if auth_type:
             __type_casbin_adapter = config.get("auth").get("casbin_adapter","file")
             _casbin_adapter_class =  auth.get_adapter_module(__type_casbin_adapter)
             _adapter_uri = config.get("auth").get("adapter_uri") 
             if not _casbin_adapter_class:
-                raise f"Not support {__type_casbin_adapter} ,Adapter config error in auth.casbin_adapter"
+                raise RuntimeError(_( "Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
             
     
     if __is_debug and db_cfg:
-        _log.info("checking database migrations....")
+        _log.info(_("checking database migrations...."))
         try:
              
             alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
             uri = db_cfg.get("uri")
             if uri:
                 database.check_migration(application.data_engine,uri,alembic_ini)
         except Exception as e:
             _log.disabled = False
             _log.error(e.args)
     if _casbin_adapter_class and _adapter_uri:
-        _log.info("init casbin auth system...")
+        _log.info(_("init casbin auth system..."))
         application.authObj = __init_auth(application,auth_type,_casbin_adapter_class,_adapter_uri)
-    _log.info("init mvc app end.")
+    _log.info(_("init mvc app end."))
     return application
 
 def run(app,*args,**kwargs): 
     import uvicorn
     global __is_debug 
     if  "debug" in kwargs:
         __is_debug = kwargs["debug"]
```

### Comparing `irails-1.1.6/irails/database.py` & `irails-1.1.7/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/midware.py` & `irails-1.1.7/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/midware_casbin.py` & `irails-1.1.7/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/midware_session.py` & `irails-1.1.7/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/_app.py` & `irails-1.1.7/irails/scripts/_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
             
             
             dirs_items =  [
                 'controllers',
                 'models',
                 'services',
                 'views',
+                'locales',
                 'tests'
             ]
             context = {'app':app_name}
             for dir in dirs_items:
                 _current_dir = os.path.join(store_dir,dir)
                 os.makedirs(_current_dir,exist_ok=True)
```

### Comparing `irails-1.1.6/irails/scripts/_controller.py` & `irails-1.1.7/irails/scripts/_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys,os,re
 from typing import Any
 from jinja2 import Template
 from irails._utils import is_valid_filename,get_controller_name,get_snaked_name
-from  irails.config import is_in_irails
+from  irails.config import is_in_irails,is_in_app
 
 class Generator():
     def __init__(self,args,dir) -> None:
         self.args = args
         self.dir = dir
         pass
     def gen_common(self):
@@ -148,32 +148,15 @@
             actions = "\n".join(acts)
             context['actions'] = actions    
             self.gen_tpl(tpl_file=dirs_items['controllers']['tpl'],dest=controller_file,context=context,use_micro=True,dir_only=False) 
 
         print("Done!")
     pass
 
-def is_in_app(directory):
-    """
-    check exists controllers , views dir in :directory
-    """
-    
-    controller_dir = os.path.join(directory, 'controllers')
-    views_dir = os.path.join(directory, 'views')  
-    if not os.path.exists(controller_dir):
-        print(f"can't location `controller` dir")
-        return False  
-    if  not os.path.exists(views_dir) :
-        print(f"can't location `views` dir")
-        return False
-    # initfile = os.path.join(controller_dir, '__init__.py') 
-    # if not os.path.exists(initfile):
-    #     return False
-    
-    return True
+
 def main():
      
     cur_dir = os.path.abspath(os.curdir)
     root_path = os.path.abspath(os.path.join(cur_dir,"../.."))
     if os.path.exists(root_path) and  os.path.isdir(root_path): 
         if not is_in_irails(root_path) or not is_in_app(cur_dir):
             print(f"Please exec in irails project's app dir ,like `apps/app`")
```

### Comparing `irails-1.1.6/irails/scripts/_project.py` & `irails-1.1.7/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/_run.py` & `irails-1.1.7/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/main.py` & `irails-1.1.7/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/app/home.css.tpl` & `irails-1.1.7/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/app/home.tpl` & `irails-1.1.7/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.1.7/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.1.7/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.1.7/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/public/error_404.html` & `irails-1.1.7/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/public/error_500.html` & `irails-1.1.7/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.1.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.1.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.1.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails/view.py` & `irails-1.1.7/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/irails.egg-info/PKG-INFO` & `irails-1.1.7/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.6
+Version: 1.1.7
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.6/irails.egg-info/SOURCES.txt` & `irails-1.1.7/irails.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 setup.py
 irails/__init__.py
+irails/_i18n.py
 irails/_loader.py
 irails/_utils.py
 irails/auth.py
 irails/base_controller.py
 irails/cbv.py
 irails/config.py
 irails/controller.py
@@ -24,14 +25,15 @@
 irails.egg-info/top_level.txt
 irails/scripts/main.py
 irails/casbin_adapters/sqlalchemy_adapter.py
 irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
 irails/scripts/__init__.py
 irails/scripts/_app.py
 irails/scripts/_controller.py
+irails/scripts/_i18n.py
 irails/scripts/_project.py
 irails/scripts/_run.py
 irails/scripts/main.py
 irails/scripts/tpls/app/controller.tpl
 irails/scripts/tpls/app/css.tpl
 irails/scripts/tpls/app/home.css.tpl
 irails/scripts/tpls/app/home.tpl
```

### Comparing `irails-1.1.6/irails.egg-info/requires.txt` & `irails-1.1.7/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.6/setup.py` & `irails-1.1.7/setup.py`

 * *Files identical despite different names*

