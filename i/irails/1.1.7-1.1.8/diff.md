# Comparing `tmp/irails-1.1.7.tar.gz` & `tmp/irails-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.1.7.tar", last modified: Sat May  6 13:42:28 2023, max compression
+gzip compressed data, was "irails-1.1.8.tar", last modified: Sat May  6 14:50:20 2023, max compression
```

## Comparing `irails-1.1.7.tar` & `irails-1.1.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.615230 irails-1.1.7/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7120 2023-05-06 13:42:28.613235 irails-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6339 2023-05-06 13:42:28.000000 irails-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.553960 irails-1.1.7/irails/
--rw-rw-rw-   0        0        0      325 2023-05-06 13:42:16.000000 irails-1.1.7/irails/__init__.py
--rw-rw-rw-   0        0        0     4239 2023-05-06 13:29:30.000000 irails-1.1.7/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.1.7/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.7/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.1.7/irails/auth.py
--rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.7/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.562371 irails-1.1.7/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.563370 irails-1.1.7/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.7/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.7/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.7/irails/cbv.py
--rw-rw-rw-   0        0        0     7252 2023-05-06 13:39:48.000000 irails-1.1.7/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.7/irails/controller.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.7/irails/controller_utils.py
--rw-rw-rw-   0        0        0    14707 2023-05-06 10:10:49.000000 irails-1.1.7/irails/core.py
--rw-rw-rw-   0        0        0     6338 2023-05-05 11:07:47.000000 irails-1.1.7/irails/database.py
--rw-rw-rw-   0        0        0     8134 2023-05-05 14:29:33.000000 irails-1.1.7/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.7/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.7/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.571348 irails-1.1.7/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.7/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7813 2023-05-06 13:37:52.000000 irails-1.1.7/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7603 2023-05-06 13:40:20.000000 irails-1.1.7/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     1416 2023-05-06 13:40:43.000000 irails-1.1.7/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.7/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.7/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.7/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.521452 irails-1.1.7/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.580325 irails-1.1.7/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.7/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.7/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.7/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.1.7/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.7/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.7/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.7/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.7/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.585318 irails-1.1.7/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.7/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.586309 irails-1.1.7/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.7/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.594287 irails-1.1.7/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.7/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.7/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.7/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.7/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.7/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.7/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.7/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.7/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.596281 irails-1.1.7/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.7/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.7/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.601277 irails-1.1.7/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.527423 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.604259 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.609246 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.527423 irails-1.1.7/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.610243 irails-1.1.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.1.7/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:42:28.560377 irails-1.1.7/irails.egg-info/
--rw-rw-rw-   0        0        0     7120 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      753 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 13:42:28.000000 irails-1.1.7/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 13:42:28.615230 irails-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.358504 irails-1.1.8/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     7120 2023-05-06 14:50:20.357503 irails-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6339 2023-05-06 14:50:20.000000 irails-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.300391 irails-1.1.8/irails/
+-rw-rw-rw-   0        0        0      325 2023-05-06 14:49:50.000000 irails-1.1.8/irails/__init__.py
+-rw-rw-rw-   0        0        0     4474 2023-05-06 14:45:44.000000 irails-1.1.8/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.1.8/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.8/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.1.8/irails/auth.py
+-rw-rw-rw-   0        0        0    10888 2023-05-06 14:48:07.000000 irails-1.1.8/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.311236 irails-1.1.8/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.312233 irails-1.1.8/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.8/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.8/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.8/irails/cbv.py
+-rw-rw-rw-   0        0        0     7252 2023-05-06 13:39:48.000000 irails-1.1.8/irails/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.8/irails/controller.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.8/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    14863 2023-05-06 14:23:18.000000 irails-1.1.8/irails/core.py
+-rw-rw-rw-   0        0        0     6338 2023-05-05 11:07:47.000000 irails-1.1.8/irails/database.py
+-rw-rw-rw-   0        0        0     8134 2023-05-05 14:29:33.000000 irails-1.1.8/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.8/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.8/irails/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.318216 irails-1.1.8/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.8/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7813 2023-05-06 13:37:52.000000 irails-1.1.8/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7603 2023-05-06 13:40:20.000000 irails-1.1.8/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     1881 2023-05-06 14:04:56.000000 irails-1.1.8/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.8/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.8/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.8/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.270688 irails-1.1.8/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.328190 irails-1.1.8/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.8/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.8/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.8/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.1.8/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.8/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.8/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.8/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.8/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.330185 irails-1.1.8/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.8/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.331182 irails-1.1.8/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.8/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.340157 irails-1.1.8/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.8/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.8/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.8/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.8/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.8/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.8/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.8/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.8/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.343150 irails-1.1.8/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.8/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.8/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.345532 irails-1.1.8/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.275656 irails-1.1.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.348526 irails-1.1.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.353541 irails-1.1.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.276885 irails-1.1.8/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.355509 irails-1.1.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.1.8/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:50:20.309241 irails-1.1.8/irails.egg-info/
+-rw-rw-rw-   0        0        0     7120 2023-05-06 14:50:20.000000 irails-1.1.8/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2023-05-06 14:50:20.000000 irails-1.1.8/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 14:50:20.000000 irails-1.1.8/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-06 14:50:20.000000 irails-1.1.8/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      753 2023-05-06 14:50:20.000000 irails-1.1.8/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 14:50:20.000000 irails-1.1.8/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 14:50:20.358504 irails-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.8/setup.py
```

### Comparing `irails-1.1.7/PKG-INFO` & `irails-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.7
+Version: 1.1.8
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.7/README.md` & `irails-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/_i18n.py` & `irails-1.1.8/irails/_i18n.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
-import gettext  
+import gettext
+import importlib  
 
 import os,sys
 import gettext
 from typing import Union
 _default_localedir = os.path.join(sys.base_prefix, 'share', 'locale')
 _old_find = gettext.find
 def _expand_lang(loc):
@@ -104,32 +105,41 @@
         if os.path.exists(mo_file):
             mod_time =  (os.stat(mo_file).st_mtime)
         else:
             mod_time = 0
         pod_time =  (os.stat(po_file).st_mtime) 
         if pod_time>mod_time: 
             do_command()
-             
+# 获取当前模块的 ModuleSpec 实例
+module_spec = importlib.util.find_spec(__name__)
+
+__all_trans = {}           
 def load_app_translations(module_dir,is_core:bool=False,lan=None) -> gettext.GNUTranslations: 
+    global __all_trans
+    if module_dir in __all_trans:
+        return __all_trans[module_dir]
     if not is_core:
         from .config import config
         cfg = config.get('i18n')
         if not cfg:
             lan = ['en','zh']
         else:
             lan = cfg.get('lang')
         if not isinstance(lan,list):
             lan=[lan]
     else:
         if not lan:
             lan = ['en','zh']
     # 加载翻译文件
     locales_dir = os.path.join(module_dir, "locales")
+    ret = None
     try:
-        zh_translations = gettext.translation("messages", locales_dir, languages=lan) 
-        return zh_translations # 返回翻译器对象
+        ret = gettext.translation("messages", locales_dir, languages=lan) 
+         
     except FileNotFoundError as e:
         pass
     
-    return gettext
+    ret = gettext
+    __all_trans[module_dir] = ret
+    return ret
```

### Comparing `irails-1.1.7/irails/_loader.py` & `irails-1.1.8/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/_utils.py` & `irails-1.1.8/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/auth.py` & `irails-1.1.8/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/base_controller.py` & `irails-1.1.8/irails/base_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .config import config,ROOT_PATH,_log
 import os,uuid
 from hashlib import md5
 from typing import Dict
 from logging import Logger
 import inspect
 import datetime
-
+from irails._i18n import load_app_translations
  
 __session_config = config.get('session') 
 _session_key = "session_id"
 alow_extensions = []
 MAX_UPLOAD_LEN = -1
 MAX_FILES = 1
 if __session_config:
@@ -26,15 +26,21 @@
     updir = __upload_cfg['dir'] or "uploads"
     MAX_UPLOAD_LEN = int(eval(__max_upload)) if __max_upload else -1
     MAX_FILES = int(eval(__max_files)) if __max_files else -1
 
     alow_extensions = __upload_cfg['extensions'] or []
 
 class BaseController:
-     
+    @property
+    def _(self):
+        m = getattr(self,'__appdir__').split(os.sep)
+        if len(m)>2:
+            m = os.sep.join(m[-2:])
+        t = load_app_translations(module_dir=m)
+        return t.gettext
     @property
     def log(self)->Logger:
         return _log
     @property 
     def cookies(self)->Dict[str,str]: 
         """
         cookies object
@@ -161,14 +167,15 @@
         view_path,context = get_path(caller_frame)
         
         if not 'flash' in context:
             context['flash'] = self._request.session['flash']
         template_path = os.path.join(self.__appdir__,"views")
         viewobj = _View(self._request,self._response, tmpl_path=template_path) 
         viewobj._templates.env.globals["url_for"] = url_for 
+        viewobj._templates.env.globals["_"] = self._ 
         return viewobj(view_path,context,**kwargs)
     
     async def _save_upload_file(self,file:File):  
         """return the file to saved path and http URL"""
         file.file.seek(0, 2)  # 将指针移动到文件末尾
 
         if MAX_UPLOAD_LEN>=0 and file.file.tell() > MAX_UPLOAD_LEN:
```

### Comparing `irails-1.1.7/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.1.8/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.1.8/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/cbv.py` & `irails-1.1.8/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/config.py` & `irails-1.1.8/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/controller.py` & `irails-1.1.8/irails/controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/controller_utils.py` & `irails-1.1.8/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/core.py` & `irails-1.1.8/irails/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,17 @@
     kwargs = {'secret_key':secret_key,'adapter_uri':__adapter_uri} 
     return auth.init(app=app, backend = auth_class,adapter_class=casbin_adapter_class, **kwargs)
 
 
 def api_router(path:str="", version:str="",**allargs):  
     '''
     :param path :special path format ,ex. '/{controller}/{version}'
+           if given any value,it's will be ensure {controller} flag in here auto
     :param version :str like 'v1.0' ,'2.0'..
+           if given any value,the :path will have {controller} flag auto
     '''
     if not 'auth' in allargs:
         allargs['auth'] = 'none'
 
     caller_frame = inspect.currentframe().f_back
     caller_file = caller_frame.f_code.co_filename
     relative_path = caller_file.replace(ROOT_PATH,"")
```

### Comparing `irails-1.1.7/irails/database.py` & `irails-1.1.8/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/midware.py` & `irails-1.1.8/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/midware_casbin.py` & `irails-1.1.8/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/midware_session.py` & `irails-1.1.8/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/_app.py` & `irails-1.1.8/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/_controller.py` & `irails-1.1.8/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/_i18n.py` & `irails-1.1.8/irails/scripts/_i18n.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,30 +6,44 @@
         spec = importlib.util.spec_from_file_location(module_name, module_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         return module
     return None
 def do_command(i18n_tool_file:str):
     if i18n_tool_file.lower()=='gettext':
-        i18n_tool_file='pygettext.py'
+        i18n_tool_file='pygettext'
+    if i18n_tool_file=='pygettext':
+        locales_path = os.path.abspath('locales') 
+        if not os.path.exists(locales_path):
+            os.makedirs(locales_path,exist_ok=True)
+        if not '-o' in sys.argv:
+            sys.argv.insert(1,'-o') 
+            sys.argv.insert(2,f'{locales_path}{os.sep}messages.pot') 
+         
+            
     _tools_file = os.path.join(sys.prefix,'Tools','i18n',f"{i18n_tool_file}.py")
     module = load_module(i18n_tool_file,_tools_file)
     if module:
-        module.main()
+        try:
+            module.main()
+            print(f"Done!")
+        except Exception as e:
+            print(e)
     else:
         print(f"not found tools file:{i18n_tool_file}")
 def main(): 
     #irails pygettext  -a -o messages.pot /path/to/your/dir/*.py
     cur_dir = os.path.abspath(os.curdir)
     root_path = os.path.abspath(os.path.join(cur_dir,"../.."))
     if os.path.exists(root_path) and  os.path.isdir(root_path): 
         if not is_in_irails(root_path) or not is_in_app(cur_dir):
             print(f"Please exec in irails project's app dir ,like `apps/app`")
             exit()
-    if len(sys.argv)>1:
+    if len(sys.argv)>2:
+         
         cmd = sys.argv.pop(1)
         do_command(cmd)
     else:
         self_file = os.path.basename(__file__).lstrip("_").replace(".py",'')
         print(f"Usage: irails {self_file} [args...]")
         sys.exit(0)
```

### Comparing `irails-1.1.7/irails/scripts/_project.py` & `irails-1.1.8/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/_run.py` & `irails-1.1.8/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/main.py` & `irails-1.1.8/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/app/home.css.tpl` & `irails-1.1.8/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/app/home.tpl` & `irails-1.1.8/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.1.8/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.1.8/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.1.8/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/public/error_404.html` & `irails-1.1.8/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/public/error_500.html` & `irails-1.1.8/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.1.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.1.8/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.1.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.1.8/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.1.8/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails/view.py` & `irails-1.1.8/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails.egg-info/PKG-INFO` & `irails-1.1.8/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.7
+Version: 1.1.8
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.7/irails.egg-info/SOURCES.txt` & `irails-1.1.8/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/irails.egg-info/requires.txt` & `irails-1.1.8/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.7/setup.py` & `irails-1.1.8/setup.py`

 * *Files identical despite different names*

