# Comparing `tmp/yz-core2-1.0.45.tar.gz` & `tmp/yz-core2-1.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yz-core2-1.0.45.tar", last modified: Wed Apr 26 02:47:07 2023, max compression
+gzip compressed data, was "yz-core2-1.0.47.tar", last modified: Sat May  6 03:13:16 2023, max compression
```

## Comparing `yz-core2-1.0.45.tar` & `yz-core2-1.0.47.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.319373 yz-core2-1.0.45/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.45/LICENSE
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-04-26 02:47:07.319242 yz-core2-1.0.45/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.45/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-04-26 02:47:07.319409 yz-core2-1.0.45/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-04-26 02:34:51.000000 yz-core2-1.0.45/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.304702 yz-core2-1.0.45/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.45/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.45/tests/test_setting_reload.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.45/tests/test_uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.305370 yz-core2-1.0.45/yz_core2.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-04-26 02:47:07.000000 yz-core2-1.0.45/yz_core2.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     3386 2023-04-26 02:47:07.000000 yz-core2-1.0.45/yz_core2.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-04-26 02:47:07.000000 yz-core2-1.0.45/yz_core2.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-04-26 02:47:07.000000 yz-core2-1.0.45/yz_core2.egg-info/entry_points.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-04-26 02:47:07.000000 yz-core2-1.0.45/yz_core2.egg-info/requires.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-04-26 02:47:07.000000 yz-core2-1.0.45/yz_core2.egg-info/top_level.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.306136 yz-core2-1.0.45/yzcore/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/__main__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.307151 yz-core2-1.0.45/yzcore/core/
--rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/data_hash.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/datastructures.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/encoders.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.307645 yz-core2-1.0.45/yzcore/core/management/
--rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/management/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/management/base.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.308045 yz-core2-1.0.45/yzcore/core/management/commands/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/management/commands/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/management/commands/startapp.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/management/commands/startproject.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/core/management/templates.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     6459 2023-04-26 02:45:49.000000 yz-core2-1.0.45/yzcore/core/storage.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.308576 yz-core2-1.0.45/yzcore/db/
--rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/db/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/db/db_session.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/db/pymongo_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/db/sqlalchemy_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/decorators.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/default_settings.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.45/yzcore/exceptions.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.308839 yz-core2-1.0.45/yzcore/extensions/
--rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/extensions/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.310181 yz-core2-1.0.45/yzcore/extensions/storage/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.45/yzcore/extensions/storage/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.310488 yz-core2-1.0.45/yzcore/extensions/storage/azure/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6726 2023-04-24 09:03:30.000000 yz-core2-1.0.45/yzcore/extensions/storage/azure/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10503 2023-04-21 07:30:35.000000 yz-core2-1.0.45/yzcore/extensions/storage/base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.45/yzcore/extensions/storage/const.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.310714 yz-core2-1.0.45/yzcore/extensions/storage/minio/
--rw-r--r--   0 zhouwei    (501) staff       (20)     7522 2023-04-21 07:30:35.000000 yz-core2-1.0.45/yzcore/extensions/storage/minio/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.311485 yz-core2-1.0.45/yzcore/extensions/storage/obs/
--rw-r--r--   0 zhouwei    (501) staff       (20)     8370 2023-04-25 06:05:51.000000 yz-core2-1.0.45/yzcore/extensions/storage/obs/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.45/yzcore/extensions/storage/obs/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2948 2023-04-21 02:05:49.000000 yz-core2-1.0.45/yzcore/extensions/storage/obs/obs_inherit.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.45/yzcore/extensions/storage/obs/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.311968 yz-core2-1.0.45/yzcore/extensions/storage/oss/
--rw-r--r--   0 zhouwei    (501) staff       (20)    12066 2023-04-24 10:39:38.000000 yz-core2-1.0.45/yzcore/extensions/storage/oss/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.45/yzcore/extensions/storage/oss/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1203 2023-04-24 09:03:30.000000 yz-core2-1.0.45/yzcore/extensions/storage/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.45/yzcore/extensions/storage/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/extensions/uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.312604 yz-core2-1.0.45/yzcore/logger/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/logger/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/logger/config.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/logger/filters.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/logger/handlers.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.312910 yz-core2-1.0.45/yzcore/request/
--rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/request/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/request/aio_http.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.313295 yz-core2-1.0.45/yzcore/response/
--rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/response/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/response/response.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/response/response_code.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.313477 yz-core2-1.0.45/yzcore/templates/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.314268 yz-core2-1.0.45/yzcore/templates/app_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/app_template/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/app_template/controllers.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/app_template/models.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/app_template/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/app_template/tests.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/app_template/views.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.314670 yz-core2-1.0.45/yzcore/templates/project_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/.gitignore
--rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/README.md
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.314895 yz-core2-1.0.45/yzcore/templates/project_template/docs/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/docs/install_explain.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/docs/supervisor.ini
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.315081 yz-core2-1.0.45/yzcore/templates/project_template/migrations/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/migrations/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/requirements.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.315478 yz-core2-1.0.45/yzcore/templates/project_template/src/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.315690 yz-core2-1.0.45/yzcore/templates/project_template/src/apps/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/apps/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.316538 yz-core2-1.0.45/yzcore/templates/project_template/src/conf/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/conf/config_dev.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/conf/config_dev.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/conf/config_production.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/conf/config_production.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/conf/config_testing.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/conf/config_testing.yaml
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.317054 yz-core2-1.0.45/yzcore/templates/project_template/src/const/
--rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/const/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/const/_job.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/const/_task.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/main.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/settings.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.317430 yz-core2-1.0.45/yzcore/templates/project_template/src/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/tests/test_xxx.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.317629 yz-core2-1.0.45/yzcore/templates/project_template/src/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/templates/project_template/src/utils/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-26 02:47:07.319025 yz-core2-1.0.45/yzcore/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/utils/check_path.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/utils/check_sys.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/utils/crypto.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-04-26 02:34:51.000000 yz-core2-1.0.45/yzcore/utils/decorator.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/utils/encoding.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.45/yzcore/utils/nacos.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1834 2023-04-21 07:30:35.000000 yz-core2-1.0.45/yzcore/utils/time_utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.476584 yz-core2-1.0.47/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.47/LICENSE
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-06 03:13:16.476447 yz-core2-1.0.47/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.47/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-05-06 03:13:16.476623 yz-core2-1.0.47/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-05-06 03:13:09.000000 yz-core2-1.0.47/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.459320 yz-core2-1.0.47/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.47/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.47/tests/test_setting_reload.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.47/tests/test_uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.460296 yz-core2-1.0.47/yz_core2.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3386 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/entry_points.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/requires.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-05-06 03:13:16.000000 yz-core2-1.0.47/yz_core2.egg-info/top_level.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.461205 yz-core2-1.0.47/yzcore/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/__main__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.462309 yz-core2-1.0.47/yzcore/core/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/data_hash.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/datastructures.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/encoders.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.463123 yz-core2-1.0.47/yzcore/core/management/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/base.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.463731 yz-core2-1.0.47/yzcore/core/management/commands/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/commands/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/commands/startapp.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/commands/startproject.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/core/management/templates.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6459 2023-05-05 06:04:45.000000 yz-core2-1.0.47/yzcore/core/storage.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.464397 yz-core2-1.0.47/yzcore/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/db/db_session.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/db/pymongo_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/db/sqlalchemy_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/decorators.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/default_settings.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.47/yzcore/exceptions.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.464722 yz-core2-1.0.47/yzcore/extensions/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/extensions/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.465910 yz-core2-1.0.47/yzcore/extensions/storage/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.47/yzcore/extensions/storage/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.466231 yz-core2-1.0.47/yzcore/extensions/storage/azure/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7286 2023-05-06 03:12:37.000000 yz-core2-1.0.47/yzcore/extensions/storage/azure/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10660 2023-05-06 03:12:38.000000 yz-core2-1.0.47/yzcore/extensions/storage/base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.47/yzcore/extensions/storage/const.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.466441 yz-core2-1.0.47/yzcore/extensions/storage/minio/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8091 2023-05-06 03:12:37.000000 yz-core2-1.0.47/yzcore/extensions/storage/minio/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.467440 yz-core2-1.0.47/yzcore/extensions/storage/obs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8886 2023-05-06 03:12:37.000000 yz-core2-1.0.47/yzcore/extensions/storage/obs/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.47/yzcore/extensions/storage/obs/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.47/yzcore/extensions/storage/obs/obs_inherit.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.47/yzcore/extensions/storage/obs/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.468064 yz-core2-1.0.47/yzcore/extensions/storage/oss/
+-rw-r--r--   0 zhouwei    (501) staff       (20)    12259 2023-05-06 03:12:38.000000 yz-core2-1.0.47/yzcore/extensions/storage/oss/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.47/yzcore/extensions/storage/oss/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1203 2023-04-24 09:03:30.000000 yz-core2-1.0.47/yzcore/extensions/storage/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.47/yzcore/extensions/storage/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/extensions/uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.468681 yz-core2-1.0.47/yzcore/logger/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/logger/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/logger/config.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/logger/filters.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/logger/handlers.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.469084 yz-core2-1.0.47/yzcore/request/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/request/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/request/aio_http.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.469699 yz-core2-1.0.47/yzcore/response/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/response/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/response/response.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/response/response_code.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.469909 yz-core2-1.0.47/yzcore/templates/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.470704 yz-core2-1.0.47/yzcore/templates/app_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/controllers.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/models.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/tests.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/app_template/views.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.471142 yz-core2-1.0.47/yzcore/templates/project_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/.gitignore
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/README.md
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.471440 yz-core2-1.0.47/yzcore/templates/project_template/docs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/docs/install_explain.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/docs/supervisor.ini
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.471622 yz-core2-1.0.47/yzcore/templates/project_template/migrations/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/migrations/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/requirements.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.472003 yz-core2-1.0.47/yzcore/templates/project_template/src/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.472140 yz-core2-1.0.47/yzcore/templates/project_template/src/apps/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/apps/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.472908 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_dev.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_dev.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_production.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_production.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_testing.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/conf/config_testing.yaml
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.473639 yz-core2-1.0.47/yzcore/templates/project_template/src/const/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/const/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/const/_job.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/const/_task.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/main.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/settings.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.474038 yz-core2-1.0.47/yzcore/templates/project_template/src/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/tests/test_xxx.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.474203 yz-core2-1.0.47/yzcore/templates/project_template/src/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/templates/project_template/src/utils/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-06 03:13:16.476128 yz-core2-1.0.47/yzcore/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/check_path.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/check_sys.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/crypto.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-04-26 02:34:51.000000 yz-core2-1.0.47/yzcore/utils/decorator.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/encoding.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.47/yzcore/utils/nacos.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1834 2023-04-21 07:30:35.000000 yz-core2-1.0.47/yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.45/LICENSE` & `yz-core2-1.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/PKG-INFO` & `yz-core2-1.0.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.45
+Version: 1.0.47
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.45/README.md` & `yz-core2-1.0.47/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/setup.py` & `yz-core2-1.0.47/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yz-core2",  # Replace with your own username
-    version="1.0.45",
+    version="1.0.47",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     description="An ID generator for distributed microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhouwe1/yz-core.git",
     packages=setuptools.find_packages(),
```

### Comparing `yz-core2-1.0.45/tests/test_setting_reload.py` & `yz-core2-1.0.47/tests/test_setting_reload.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/tests/test_uid.py` & `yz-core2-1.0.47/tests/test_uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yz_core2.egg-info/PKG-INFO` & `yz-core2-1.0.47/yz_core2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.45
+Version: 1.0.47
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.45/yz_core2.egg-info/SOURCES.txt` & `yz-core2-1.0.47/yz_core2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/core/datastructures.py` & `yz-core2-1.0.47/yzcore/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/core/encoders.py` & `yz-core2-1.0.47/yzcore/core/encoders.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/core/management/__init__.py` & `yz-core2-1.0.47/yzcore/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/core/management/commands/startapp.py` & `yz-core2-1.0.47/yzcore/core/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/core/management/commands/startproject.py` & `yz-core2-1.0.47/yzcore/core/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/core/management/templates.py` & `yz-core2-1.0.47/yzcore/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/core/storage.py` & `yz-core2-1.0.47/yzcore/core/storage.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/db/db_session.py` & `yz-core2-1.0.47/yzcore/db/db_session.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/db/pymongo_crud_base.py` & `yz-core2-1.0.47/yzcore/db/pymongo_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/db/sqlalchemy_crud_base.py` & `yz-core2-1.0.47/yzcore/db/sqlalchemy_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/decorators.py` & `yz-core2-1.0.47/yzcore/decorators.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/default_settings.py` & `yz-core2-1.0.47/yzcore/default_settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/exceptions.py` & `yz-core2-1.0.47/yzcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/__init__.py` & `yz-core2-1.0.47/yzcore/extensions/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/azure/__init__.py` & `yz-core2-1.0.47/yzcore/extensions/storage/azure/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -171,10 +171,27 @@
                     blob_client.upload_blob(f)
             else:
                 blob_client.upload_blob(filepath)
             return self.get_file_url(key)
         except Exception as e:
             raise StorageRequestError(f'azure blob upload error: {e}')
 
-    def get_policy(self, filepath: str, callback_url: str, callback_data: dict = None,
-                   callback_content_type: str = "application/json"):
+    def get_policy(
+            self,
+            filepath: str,
+            callback_url: str,
+            callback_data: dict = None,
+            callback_content_type: str = "application/json",
+            callback_directly: bool = True,
+    ):
+        """
+        授权给第三方上传
+        :param filepath:
+        :param callback_url: 对象存储的回调地址
+        :param callback_data: 需要回传的参数
+        :param callback_content_type: 回调时的Content-Type
+               "application/json"
+               "application/x-www-form-urlencoded"
+        :param callback_directly: True 由对象存储自动发起回调 / False 需要前端主动发起回调
+        :return:
+        """
         pass
```

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/base.py` & `yz-core2-1.0.47/yzcore/extensions/storage/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,24 +141,26 @@
 
     @abstractmethod
     def get_policy(
             self,
             filepath: str,
             callback_url: str,
             callback_data: dict = None,
-            callback_content_type: str = "application/json"
+            callback_content_type: str = "application/json",
+            callback_directly: bool = True,
     ):
         """
         授权给第三方上传
         :param filepath:
         :param callback_url: 对象存储的回调地址
         :param callback_data: 需要回传的参数
         :param callback_content_type: 回调时的Content-Type
                "application/json"
                "application/x-www-form-urlencoded"
+        :param callback_directly: True 由对象存储自动发起回调 / False 需要前端主动发起回调
         :return:
         """
 
     @property
     def host(self):
         return u'//{}.{}'.format(self.bucket_name, self.endpoint)
```

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/const.py` & `yz-core2-1.0.47/yzcore/extensions/storage/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/minio/__init__.py` & `yz-core2-1.0.47/yzcore/extensions/storage/minio/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -163,16 +163,33 @@
                 self.minioClient.fput_object(self.bucket_name, key, filepath, content_type=content_type)
             else:
                 self.minioClient.put_object(self.bucket_name, key, filepath, length=-1, content_type=content_type, part_size=1024*1024*5)
             return self.get_file_url(key)
         except Exception as e:
             raise StorageRequestError(f'minio upload error: {e}')
 
-    def get_policy(self, filepath: str, callback_url: str, callback_data: dict = None,
-                   callback_content_type: str = "application/json"):
+    def get_policy(
+            self,
+            filepath: str,
+            callback_url: str,
+            callback_data: dict = None,
+            callback_content_type: str = "application/json",
+            callback_directly: bool = False,
+    ):
+        """
+        授权给第三方上传
+        :param filepath:
+        :param callback_url: 对象存储的回调地址
+        :param callback_data: 需要回传的参数
+        :param callback_content_type: 回调时的Content-Type
+               "application/json"
+               "application/x-www-form-urlencoded"
+        :param callback_directly:  False 需要前端主动发起回调 minio没有回调功能，只能由前端发起
+        :return:
+        """
         form_data = self.post_sign_url(filepath)
         data = {
             'mode': 'minio',
             'host': f'{self.scheme}:{self.host}',
             'dir': filepath,
             'success_action_status': 200,
             'callback': {'url': callback_url, 'data': callback_data},
```

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/obs/__init__.py` & `yz-core2-1.0.47/yzcore/extensions/storage/obs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,50 +148,60 @@
         return self.get_file_url(key)
 
     def get_policy(
             self,
             filepath: str,
             callback_url: str,
             callback_data: dict = None,
-            callback_content_type: str = "application/json"):
+            callback_content_type: str = "application/json",
+            callback_directly: bool = True,
+    ):
         """
         授权给第三方上传
 
         :param filepath:
         :param callback_url:
         :param callback_data: 需要回传的参数
         :param callback_content_type: 回调时的Content-Type
                "application/json"
                "application/x-www-form-urlencoded"
                 华为云目前只能用application/json格式，用x-www-form-urlencoded时回调数据会在url中
+        :param callback_directly: True OBS直接发起回调 / False 由前端发起回调
+                由于华为云只有单az模式支持回调，多az不支持，可以根据不同情况选择obs回调或者前端发起回调
         :return:
         """
-        callback_body = '{"filepath":"$(key)","etag":"$(etag)","size":$(fsize),"mime_type":"$(ext)",' \
-                        '"data":' \
-                        + json.dumps(callback_data) + '}'
-
-        callback_body_plain = json.dumps(callback_body).strip().encode()
-        base64_callback_body = base64.b64encode(callback_body_plain)
-
-        form_param = {
-            'body': base64_callback_body.decode(),
-            'url': callback_url,
-            'body-type': callback_content_type,
-            # 'success_action_status': '200',
-        }
-        res = self.post_sign_url(key=None, form_param=form_param)
+        if callback_directly:
+            callback_body = '{"filepath":"$(key)","etag":"$(etag)","size":$(fsize),"mime_type":"$(ext)",' \
+                            '"data":' \
+                            + json.dumps(callback_data) + '}'
+
+            callback_body_plain = json.dumps(callback_body).strip().encode()
+            base64_callback_body = base64.b64encode(callback_body_plain)
+
+            form_param = {
+                'body': base64_callback_body.decode(),
+                'url': callback_url,
+                'body-type': callback_content_type,
+                # 'success_action_status': '200',
+            }
+        else:
+            form_param = {}
+
+        res = self.post_sign_url(key=filepath, form_param=form_param)
 
         data = dict(
             mode='obs',
             AccessKeyId=self.access_key_id,
             host=f'{self.scheme}:{self.host}',
             policy=res.policy,
             signature=res.signature,
             dir=filepath
         )
+        if not callback_directly:
+            data['callback'] = {'url': callback_url, 'data': callback_data}
         return data
 
     def update_file_headers(self, key, headers: dict):
         # 兼容 oss.update_file_headers
         obs_headers = SetObjectMetadataHeader()
         obs_headers.contentType = headers.get('Content-Type')  # oss 和 obs的参数名称不相同
         self.obsClient.setObjectMetadata(self.bucket_name, key, obs_headers)
```

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/obs/const.py` & `yz-core2-1.0.47/yzcore/extensions/storage/obs/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/obs/obs_inherit.py` & `yz-core2-1.0.47/yzcore/extensions/storage/obs/obs_inherit.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,38 +21,41 @@
         expires = 300 if expires is None else util.to_int(expires)
         expires = date + timedelta(seconds=expires)
 
         expires = expires.strftime(const.EXPIRATION_DATE_FORMAT)
 
         formParams = self._parse_post_params(formParams, securityProvider, is_v4,
                                              bucketName, objectKey, longDate, shortDate)
-
-        policy = ['{"expiration":"']
-        policy.append(expires)
-        policy.append('", "callback":[')
+        policy = [f'{{"expiration":"{expires}",']
 
         # 添加callback数据
-        policy.append('{"url":"' + formParams.get('url', '') + '"},')
-        policy.append('{"body":"' + formParams.get('body', '') + '"},')
-        policy.append('{"body-type":"' + formParams.get('body-type', '') + '"},')
-        policy.append('], "conditions":[')
+        if formParams.get('url'):
+            policy.append('"callback":[')
+            policy.append(f'{{"url":"{formParams.get("url", "")}"}},')
+            policy.append(f'{{"body":"{formParams.get("body", "")}"}},')
+            policy.append(f'{{"body-type":"{formParams.get("body-type", "")}"}},')
+            policy.append('], ')
+
+        policy.append('"conditions":[')
 
         matchAnyBucket = True
         matchAnyKey = True
 
         conditionAllowKeys = ['acl', 'bucket', 'key', 'success_action_redirect', 'redirect', 'success_action_status']
 
         for key, value in formParams.items():
             if key:
                 key = util.to_string(key).lower()
 
                 if key == 'bucket':
                     matchAnyBucket = False
                 elif key == 'key':
                     matchAnyKey = False
+                    policy.append(f'["starts-with", "$key", "{value}"],')
+                    continue
 
                 if key not in const.ALLOWED_REQUEST_HTTP_HEADER_METADATA_NAMES \
                         and not key.startswith(self.ha._get_header_prefix()) \
                         and not key.startswith(const.OBS_HEADER_PREFIX) and key not in conditionAllowKeys:
                     continue
 
                 policy.append('{"')
```

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/obs/utils.py` & `yz-core2-1.0.47/yzcore/extensions/storage/obs/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/oss/__init__.py` & `yz-core2-1.0.47/yzcore/extensions/storage/oss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,25 +229,27 @@
         return self.get_file_url(key)
 
     def get_policy(
             self,
             filepath: str,
             callback_url: str,
             callback_data: dict = None,
-            callback_content_type: str = "application/json"):
+            callback_content_type: str = "application/json",
+            callback_directly: bool = True,
+    ):
         """
         授权给第三方上传
 
         :param filepath:
         :param callback_url:
         :param callback_data: 需要回传的参数
         :param callback_content_type: 回调时的Content-Type
                "application/json"
                "application/x-www-form-urlencoded"
-
+        :param callback_directly: True 由对象存储自动发起回调 / False 需要前端主动发起回调  oss不需要前端发起回调
         :return:
         """
         params = parse.urlencode(
             dict(data=json.dumps(callback_data)))
         policy_encode = self._get_policy_encode(filepath)
         sign = self.get_signature(policy_encode)
```

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/oss/const.py` & `yz-core2-1.0.47/yzcore/extensions/storage/oss/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/extensions/storage/schemas.py` & `yz-core2-1.0.47/yzcore/extensions/storage/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/extensions/uid.py` & `yz-core2-1.0.47/yzcore/extensions/uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/logger/__init__.py` & `yz-core2-1.0.47/yzcore/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/logger/config.py` & `yz-core2-1.0.47/yzcore/logger/config.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/logger/filters.py` & `yz-core2-1.0.47/yzcore/logger/filters.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/logger/handlers.py` & `yz-core2-1.0.47/yzcore/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/request/aio_http.py` & `yz-core2-1.0.47/yzcore/request/aio_http.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/response/response.py` & `yz-core2-1.0.47/yzcore/response/response.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/response/response_code.py` & `yz-core2-1.0.47/yzcore/response/response_code.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/app_template/controllers.py` & `yz-core2-1.0.47/yzcore/templates/app_template/controllers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/app_template/schemas.py` & `yz-core2-1.0.47/yzcore/templates/app_template/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/app_template/views.py` & `yz-core2-1.0.47/yzcore/templates/app_template/views.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/project_template/.gitignore` & `yz-core2-1.0.47/yzcore/templates/project_template/.gitignore`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/project_template/README.md` & `yz-core2-1.0.47/yzcore/templates/project_template/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/project_template/docs/supervisor.ini` & `yz-core2-1.0.47/yzcore/templates/project_template/docs/supervisor.ini`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/project_template/src/main.py` & `yz-core2-1.0.47/yzcore/templates/project_template/src/main.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/project_template/src/settings.py` & `yz-core2-1.0.47/yzcore/templates/project_template/src/settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/templates/project_template/src/tests/test_xxx.py` & `yz-core2-1.0.47/yzcore/templates/project_template/src/tests/test_xxx.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/utils/check_sys.py` & `yz-core2-1.0.47/yzcore/utils/check_sys.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/utils/crypto.py` & `yz-core2-1.0.47/yzcore/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/utils/decorator.py` & `yz-core2-1.0.47/yzcore/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/utils/encoding.py` & `yz-core2-1.0.47/yzcore/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/utils/nacos.py` & `yz-core2-1.0.47/yzcore/utils/nacos.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.45/yzcore/utils/time_utils.py` & `yz-core2-1.0.47/yzcore/utils/time_utils.py`

 * *Files identical despite different names*

