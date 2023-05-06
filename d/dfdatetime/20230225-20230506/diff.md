# Comparing `tmp/dfdatetime-20230225.tar.gz` & `tmp/dfdatetime-20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfdatetime-20230225.tar", last modified: Sat Feb 25 09:11:23 2023, max compression
+gzip compressed data, was "dfdatetime-20230506.tar", last modified: Sat May  6 15:13:12 2023, max compression
```

## Comparing `dfdatetime-20230225.tar` & `dfdatetime-20230506.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.312722 dfdatetime-20230225/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:22.812721 dfdatetime-20230225/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:22.889721 dfdatetime-20230225/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2022-12-20 19:33:04.000000 dfdatetime-20230225/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1352 2022-12-20 19:33:04.000000 dfdatetime-20230225/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2022-12-20 19:33:04.000000 dfdatetime-20230225/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21911 2022-12-20 17:56:12.000000 dfdatetime-20230225/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       94 2017-04-22 10:13:23.000000 dfdatetime-20230225/.style.yapf
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      661 2016-03-12 13:43:08.000000 dfdatetime-20230225/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      368 2016-03-12 13:43:08.000000 dfdatetime-20230225/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-03-10 06:45:13.000000 dfdatetime-20230225/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      497 2021-11-01 04:57:04.000000 dfdatetime-20230225/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      644 2023-02-25 09:11:23.312722 dfdatetime-20230225/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      213 2020-12-31 07:59:59.000000 dfdatetime-20230225/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2022-12-20 17:56:12.000000 dfdatetime-20230225/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:22.813721 dfdatetime-20230225/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:22.911721 dfdatetime-20230225/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2022-12-20 17:56:12.000000 dfdatetime-20230225/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2022-12-20 17:56:12.000000 dfdatetime-20230225/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2022-12-20 17:56:12.000000 dfdatetime-20230225/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:22.931721 dfdatetime-20230225/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      173 2023-02-25 08:13:21.000000 dfdatetime-20230225/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       23 2018-02-18 11:30:40.000000 dfdatetime-20230225/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2022-12-20 17:56:12.000000 dfdatetime-20230225/config/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      554 2022-12-20 17:56:12.000000 dfdatetime-20230225/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      968 2018-02-18 11:30:40.000000 dfdatetime-20230225/config/dpkg/copyright
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2022-12-20 17:56:12.000000 dfdatetime-20230225/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:22.931721 dfdatetime-20230225/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2018-02-18 11:30:40.000000 dfdatetime-20230225/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:22.943721 dfdatetime-20230225/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      229 2019-05-12 09:21:52.000000 dfdatetime-20230225/config/pylint/spelling-private-dict
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        0 2018-02-18 11:30:40.000000 dfdatetime-20230225/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.130722 dfdatetime-20230225/dfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      870 2023-02-25 08:12:55.000000 dfdatetime-20230225/dfdatetime/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2592 2022-11-06 04:31:45.000000 dfdatetime-20230225/dfdatetime/apfs_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4560 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/cocoa_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 08:21:27.000000 dfdatetime-20230225/dfdatetime/decorators.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2331 2022-10-22 13:44:47.000000 dfdatetime-20230225/dfdatetime/definitions.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5432 2023-02-25 09:10:44.000000 dfdatetime-20230225/dfdatetime/delphi_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4820 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/dotnet_datetime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2022-10-23 05:47:17.000000 dfdatetime-20230225/dfdatetime/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4147 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/fake_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10574 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/fat_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4871 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/filetime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7733 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/golang_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4373 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/hfs_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31660 2023-02-25 08:12:51.000000 dfdatetime-20230225/dfdatetime/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1977 2022-11-06 04:31:45.000000 dfdatetime-20230225/dfdatetime/java_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5083 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/ole_automation_date.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16385 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/posix_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7906 2022-09-18 08:21:27.000000 dfdatetime-20230225/dfdatetime/precisions.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8171 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/rfc2579_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9079 2022-11-06 04:31:45.000000 dfdatetime-20230225/dfdatetime/semantic_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7249 2022-11-13 04:33:05.000000 dfdatetime-20230225/dfdatetime/serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7311 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/systemtime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43963 2022-11-06 15:15:00.000000 dfdatetime-20230225/dfdatetime/time_elements.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5068 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/uuid_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4623 2022-11-07 04:49:22.000000 dfdatetime-20230225/dfdatetime/webkit_time.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.132722 dfdatetime-20230225/dfdatetime.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      644 2023-02-25 09:11:20.000000 dfdatetime-20230225/dfdatetime.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2198 2023-02-25 09:11:22.000000 dfdatetime-20230225/dfdatetime.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-02-25 09:11:20.000000 dfdatetime-20230225/dfdatetime.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       11 2023-02-25 09:11:21.000000 dfdatetime-20230225/dfdatetime.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       11 2023-02-25 09:11:21.000000 dfdatetime-20230225/dfdatetime.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      760 2022-01-09 19:31:27.000000 dfdatetime-20230225/dfdatetime.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.133721 dfdatetime-20230225/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5077 2022-12-20 17:56:12.000000 dfdatetime-20230225/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      593 2021-11-01 05:28:24.000000 dfdatetime-20230225/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2022-12-20 17:56:23.000000 dfdatetime-20230225/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.147722 dfdatetime-20230225/docs/sources/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16860 2022-08-05 06:29:06.000000 dfdatetime-20230225/docs/sources/Date-and-time-values.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.177722 dfdatetime-20230225/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3945 2022-08-06 09:48:11.000000 dfdatetime-20230225/docs/sources/api/dfdatetime.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       67 2020-06-21 04:22:12.000000 dfdatetime-20230225/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.203722 dfdatetime-20230225/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1652 2021-12-28 06:44:43.000000 dfdatetime-20230225/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2020-06-21 04:22:12.000000 dfdatetime-20230225/docs/sources/user/index.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       13 2022-12-20 17:56:12.000000 dfdatetime-20230225/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-09-18 08:21:27.000000 dfdatetime-20230225/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      299 2023-02-25 09:11:23.313722 dfdatetime-20230225/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6238 2022-12-20 17:56:12.000000 dfdatetime-20230225/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:21.000000 dfdatetime-20230225/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-20 17:56:12.000000 dfdatetime-20230225/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.295722 dfdatetime-20230225/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-02-19 20:11:27.000000 dfdatetime-20230225/tests/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/apfs_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6041 2023-02-25 08:12:51.000000 dfdatetime-20230225/tests/cocoa_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8304 2023-02-25 09:10:44.000000 dfdatetime-20230225/tests/delphi_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3582 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/dotnet_datetime.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2020-12-31 07:59:59.000000 dfdatetime-20230225/tests/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6019 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/fake_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12218 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/fat_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5538 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/filetime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8416 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/golang_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5513 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/hfs_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22233 2022-10-22 13:44:47.000000 dfdatetime-20230225/tests/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5002 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/java_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6494 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/ole_automation_date.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24634 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/posix_time.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4703 2020-12-31 08:00:00.000000 dfdatetime-20230225/tests/precisions.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12027 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/rfc2579_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7935 2022-08-10 15:55:53.000000 dfdatetime-20230225/tests/semantic_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10367 2022-11-13 04:33:05.000000 dfdatetime-20230225/tests/serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9408 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/systemtime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65798 2022-11-06 04:31:45.000000 dfdatetime-20230225/tests/time_elements.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7119 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/uuid_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5674 2022-11-05 17:43:33.000000 dfdatetime-20230225/tests/webkit_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1385 2022-12-20 17:56:12.000000 dfdatetime-20230225/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-25 09:11:23.312722 dfdatetime-20230225/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2016-03-12 13:43:08.000000 dfdatetime-20230225/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2022-12-20 17:56:12.000000 dfdatetime-20230225/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2022-12-20 17:56:12.000000 dfdatetime-20230225/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      825 2021-11-01 04:57:04.000000 dfdatetime-20230225/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.838971 dfdatetime-20230506/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:11.823969 dfdatetime-20230506/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.179970 dfdatetime-20230506/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2023-04-30 04:46:32.000000 dfdatetime-20230506/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1352 2023-04-30 04:32:35.000000 dfdatetime-20230506/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4029 2023-04-30 04:32:35.000000 dfdatetime-20230506/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21911 2023-04-30 04:32:35.000000 dfdatetime-20230506/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       94 2017-04-22 10:13:23.000000 dfdatetime-20230506/.style.yapf
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      661 2016-03-12 13:43:08.000000 dfdatetime-20230506/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      368 2016-03-12 13:43:08.000000 dfdatetime-20230506/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-03-10 06:45:13.000000 dfdatetime-20230506/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      497 2021-11-01 04:57:04.000000 dfdatetime-20230506/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      644 2023-05-06 15:13:12.838971 dfdatetime-20230506/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      213 2020-12-31 07:59:59.000000 dfdatetime-20230506/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2023-04-30 04:32:35.000000 dfdatetime-20230506/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:11.823969 dfdatetime-20230506/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.203970 dfdatetime-20230506/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      828 2023-04-30 04:32:35.000000 dfdatetime-20230506/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-04-30 04:32:35.000000 dfdatetime-20230506/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-04-30 04:32:35.000000 dfdatetime-20230506/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.300970 dfdatetime-20230506/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      173 2023-05-06 15:12:30.000000 dfdatetime-20230506/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       23 2018-02-18 11:30:40.000000 dfdatetime-20230506/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-04-30 04:32:35.000000 dfdatetime-20230506/config/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      554 2023-04-30 04:32:35.000000 dfdatetime-20230506/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      968 2018-02-18 11:30:40.000000 dfdatetime-20230506/config/dpkg/copyright
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-30 04:32:35.000000 dfdatetime-20230506/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.300970 dfdatetime-20230506/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2018-02-18 11:30:40.000000 dfdatetime-20230506/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.312970 dfdatetime-20230506/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      229 2019-05-12 09:21:52.000000 dfdatetime-20230506/config/pylint/spelling-private-dict
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        0 2018-02-18 11:30:40.000000 dfdatetime-20230506/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.395970 dfdatetime-20230506/dfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      870 2023-05-06 15:12:30.000000 dfdatetime-20230506/dfdatetime/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2592 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/apfs_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4560 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/cocoa_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/decorators.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2331 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/definitions.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5432 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/delphi_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4820 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/dotnet_datetime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2023-03-24 05:49:26.000000 dfdatetime-20230506/dfdatetime/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4147 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/fake_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10574 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/fat_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4871 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/filetime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7733 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/golang_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4373 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/hfs_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31660 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1977 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/java_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5083 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/ole_automation_date.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16385 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/posix_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7906 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/precisions.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8171 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/rfc2579_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9079 2023-03-24 05:49:26.000000 dfdatetime-20230506/dfdatetime/semantic_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7583 2023-05-06 15:12:30.000000 dfdatetime-20230506/dfdatetime/serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7311 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/systemtime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43963 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/time_elements.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5068 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/uuid_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4623 2023-03-24 05:54:49.000000 dfdatetime-20230506/dfdatetime/webkit_time.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.397970 dfdatetime-20230506/dfdatetime.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      644 2023-05-06 15:13:06.000000 dfdatetime-20230506/dfdatetime.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2198 2023-05-06 15:13:11.000000 dfdatetime-20230506/dfdatetime.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-06 15:13:06.000000 dfdatetime-20230506/dfdatetime.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       11 2023-05-06 15:13:06.000000 dfdatetime-20230506/dfdatetime.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       11 2023-05-06 15:13:06.000000 dfdatetime-20230506/dfdatetime.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      760 2022-01-09 19:31:27.000000 dfdatetime-20230506/dfdatetime.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.422970 dfdatetime-20230506/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5077 2023-04-30 04:32:35.000000 dfdatetime-20230506/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      593 2021-11-01 05:28:24.000000 dfdatetime-20230506/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-04-30 04:32:42.000000 dfdatetime-20230506/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.442970 dfdatetime-20230506/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16860 2022-08-05 06:29:06.000000 dfdatetime-20230506/docs/sources/Date-and-time-values.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.468970 dfdatetime-20230506/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3945 2022-08-06 09:48:11.000000 dfdatetime-20230506/docs/sources/api/dfdatetime.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       67 2020-06-21 04:22:12.000000 dfdatetime-20230506/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.494970 dfdatetime-20230506/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1652 2021-12-28 06:44:43.000000 dfdatetime-20230506/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2020-06-21 04:22:12.000000 dfdatetime-20230506/docs/sources/user/index.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       13 2023-04-30 04:32:35.000000 dfdatetime-20230506/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-09-18 08:21:27.000000 dfdatetime-20230506/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      299 2023-05-06 15:13:12.839970 dfdatetime-20230506/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6238 2023-04-30 04:32:35.000000 dfdatetime-20230506/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:21.000000 dfdatetime-20230506/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-30 04:32:35.000000 dfdatetime-20230506/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.796970 dfdatetime-20230506/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-02-19 20:11:27.000000 dfdatetime-20230506/tests/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/apfs_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6041 2023-02-25 08:12:51.000000 dfdatetime-20230506/tests/cocoa_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8304 2023-02-25 09:10:44.000000 dfdatetime-20230506/tests/delphi_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3582 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/dotnet_datetime.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2020-12-31 07:59:59.000000 dfdatetime-20230506/tests/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6019 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/fake_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12218 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/fat_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5538 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/filetime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8416 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/golang_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5513 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/hfs_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22233 2022-10-22 13:44:47.000000 dfdatetime-20230506/tests/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5002 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/java_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6494 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/ole_automation_date.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24634 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/posix_time.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4703 2020-12-31 08:00:00.000000 dfdatetime-20230506/tests/precisions.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12027 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/rfc2579_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7935 2022-08-10 15:55:53.000000 dfdatetime-20230506/tests/semantic_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11261 2023-05-06 15:12:30.000000 dfdatetime-20230506/tests/serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9408 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/systemtime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65798 2022-11-06 04:31:45.000000 dfdatetime-20230506/tests/time_elements.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7119 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/uuid_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5674 2022-11-05 17:43:33.000000 dfdatetime-20230506/tests/webkit_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2023-04-30 04:32:35.000000 dfdatetime-20230506/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 15:13:12.825971 dfdatetime-20230506/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2016-03-12 13:43:08.000000 dfdatetime-20230506/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-04-30 04:32:35.000000 dfdatetime-20230506/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-04-30 04:32:35.000000 dfdatetime-20230506/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      825 2021-11-01 04:57:04.000000 dfdatetime-20230506/utils/update_release.sh
```

### Comparing `dfdatetime-20230225/.github/workflows/test_docker.yml` & `dfdatetime-20230506/.github/workflows/test_docker.yml`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 on: [push]
 permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['36']
+        version: ['38']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
         dnf install -y @development-tools python3 python3-devel python3-setuptools
@@ -41,15 +41,15 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         version: ['22.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
```

### Comparing `dfdatetime-20230225/.github/workflows/test_docs.yml` & `dfdatetime-20230506/.github/workflows/test_docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       matrix:
         include:
         - python-version: '3.8'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
```

### Comparing `dfdatetime-20230225/.pylintrc` & `dfdatetime-20230506/.pylintrc`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/ACKNOWLEDGEMENTS` & `dfdatetime-20230506/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/LICENSE` & `dfdatetime-20230506/LICENSE`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/PKG-INFO` & `dfdatetime-20230506/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfdatetime
-Version: 20230225
+Version: 20230506
 Summary: Digital Forensics date and time (dfDateTime).
 Home-page: https://github.com/log2timeline/dfdatetime
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfdatetime-20230225/appveyor.yml` & `dfdatetime-20230506/appveyor.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 environment:
   PYPI_TOKEN:
     secure: /FwQrmudDyj+Mu3DaxLEo23Y6/OEgdHJqyWyZTjkJKje8pxCOrUorN8ZlXRGXbd3UA60emClt0M+SI+xqyA/qkpqZTgd5CKohpVAGH2EfzRc/zwJSGJ4tmZmMVAG8ayk6N9zFxCeC+y0BgZPQnj/Eq/RfuS4YIuaKutIUa5gTMmhWpODFKGV/2Wx1w67xWxAoONfEC5j0Gu3R274SS7FfBb4qWyIiBIJMwHGjlgp1Onk8KlpCLauZv8/hGfQDmWEdZ+mjcsTYyQYr1xfr1/FjQ==
   matrix:
-  - DESCRIPTION: "Windows with 32-bit Python 3.10"
+  - DESCRIPTION: "Windows with 32-bit Python 3.11"
     MACHINE_TYPE: "x86"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
-  - DESCRIPTION: "Windows with 64-bit Python 3.10"
+  - DESCRIPTION: "Windows with 64-bit Python 3.11"
     MACHINE_TYPE: "amd64"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310-x64"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311-x64"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
   - DESCRIPTION: "Mac OS with Python 3.11"
     APPVEYOR_BUILD_WORKER_IMAGE: macos-monterey
     HOMEBREW_NO_INSTALL_CLEANUP: 1
 
 install:
 - cmd: "%PYTHON%\\python.exe -m pip install -U pip setuptools twine wheel"
```

### Comparing `dfdatetime-20230225/config/appveyor/install.ps1` & `dfdatetime-20230506/config/appveyor/install.ps1`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Script to set up tests on AppVeyor Windows.
 
 $Dependencies = ""
-$Dependencies = ${Dependencies} -split " "
 
-$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1"
-Write-Host (${Output} | Out-String)
-
-If ($env:APPVEYOR_REPO_BRANCH -eq "main")
-{
-	$Track = "stable"
-}
-Else
+If ($Dependencies.Length -gt 0)
 {
-	$Track = $env:APPVEYOR_REPO_BRANCH
-}
-New-Item -ItemType "directory" -Name "dependencies"
+	$Dependencies = ${Dependencies} -split " "
 
-$env:PYTHONPATH = "..\l2tdevtools"
+	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
 
-$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1"
-Write-Host (${Output} | Out-String)
+	If ($env:APPVEYOR_REPO_BRANCH -eq "main")
+	{
+		$Track = "stable"
+	}
+	Else
+	{
+		$Track = $env:APPVEYOR_REPO_BRANCH
+	}
+	New-Item -ItemType "directory" -Name "dependencies"
+
+	$env:PYTHONPATH = "..\l2tdevtools"
+
+	$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
+}
```

### Comparing `dfdatetime-20230225/config/appveyor/runtests.sh` & `dfdatetime-20230506/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/config/dpkg/control` & `dfdatetime-20230506/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/config/dpkg/copyright` & `dfdatetime-20230506/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/__init__.py` & `dfdatetime-20230506/dfdatetime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 from dfdatetime import semantic_time
 from dfdatetime import systemtime
 from dfdatetime import time_elements
 from dfdatetime import uuid_time
 from dfdatetime import webkit_time
 
 
-__version__ = '20230225'
+__version__ = '20230506'
```

### Comparing `dfdatetime-20230225/dfdatetime/apfs_time.py` & `dfdatetime-20230506/dfdatetime/apfs_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/cocoa_time.py` & `dfdatetime-20230506/dfdatetime/cocoa_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/decorators.py` & `dfdatetime-20230506/dfdatetime/decorators.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/definitions.py` & `dfdatetime-20230506/dfdatetime/definitions.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/delphi_date_time.py` & `dfdatetime-20230506/dfdatetime/delphi_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/dotnet_datetime.py` & `dfdatetime-20230506/dfdatetime/dotnet_datetime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/factory.py` & `dfdatetime-20230506/dfdatetime/factory.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/fake_time.py` & `dfdatetime-20230506/dfdatetime/fake_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/fat_date_time.py` & `dfdatetime-20230506/dfdatetime/fat_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/filetime.py` & `dfdatetime-20230506/dfdatetime/filetime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/golang_time.py` & `dfdatetime-20230506/dfdatetime/golang_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/hfs_time.py` & `dfdatetime-20230506/dfdatetime/hfs_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/interface.py` & `dfdatetime-20230506/dfdatetime/interface.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/java_time.py` & `dfdatetime-20230506/dfdatetime/java_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/ole_automation_date.py` & `dfdatetime-20230506/dfdatetime/ole_automation_date.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/posix_time.py` & `dfdatetime-20230506/dfdatetime/posix_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/precisions.py` & `dfdatetime-20230506/dfdatetime/precisions.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/rfc2579_date_time.py` & `dfdatetime-20230506/dfdatetime/rfc2579_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/semantic_time.py` & `dfdatetime-20230506/dfdatetime/semantic_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/serializer.py` & `dfdatetime-20230506/dfdatetime/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,14 +116,21 @@
       json_dict['rfc2579_date_time_tuple'] = (
           date_time_values.year, date_time_values.month,
           date_time_values.day_of_month, date_time_values.hours,
           date_time_values.minutes, date_time_values.seconds,
           date_time_values.deciseconds, time_zone_sign, time_zone_hours,
           time_zone_minutes)
 
+    elif class_name == 'Systemtime':
+      json_dict['system_time_tuple'] = (
+          date_time_values.year, date_time_values.month,
+          date_time_values.day_of_week, date_time_values.day_of_month,
+          date_time_values.hours, date_time_values.minutes,
+          date_time_values.seconds, date_time_values.milliseconds)
+
     elif class_name == 'TimeElements':
       json_dict['time_elements_tuple'] = (
           date_time_values.year, date_time_values.month,
           date_time_values.day_of_month, date_time_values.hours,
           date_time_values.minutes, date_time_values.seconds)
 
     elif class_name == 'TimeElementsInMilliseconds':
```

### Comparing `dfdatetime-20230225/dfdatetime/systemtime.py` & `dfdatetime-20230506/dfdatetime/systemtime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/time_elements.py` & `dfdatetime-20230506/dfdatetime/time_elements.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/uuid_time.py` & `dfdatetime-20230506/dfdatetime/uuid_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime/webkit_time.py` & `dfdatetime-20230506/dfdatetime/webkit_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime.egg-info/PKG-INFO` & `dfdatetime-20230506/dfdatetime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfdatetime
-Version: 20230225
+Version: 20230506
 Summary: Digital Forensics date and time (dfDateTime).
 Home-page: https://github.com/log2timeline/dfdatetime
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfdatetime-20230225/dfdatetime.egg-info/SOURCES.txt` & `dfdatetime-20230506/dfdatetime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/dfdatetime.ini` & `dfdatetime-20230506/dfdatetime.ini`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/docs/conf.py` & `dfdatetime-20230506/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/docs/index.rst` & `dfdatetime-20230506/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/docs/sources/Date-and-time-values.md` & `dfdatetime-20230506/docs/sources/Date-and-time-values.md`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/docs/sources/api/dfdatetime.rst` & `dfdatetime-20230506/docs/sources/api/dfdatetime.rst`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/docs/sources/user/Installation-instructions.md` & `dfdatetime-20230506/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/run_tests.py` & `dfdatetime-20230506/run_tests.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/setup.py` & `dfdatetime-20230506/setup.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/apfs_time.py` & `dfdatetime-20230506/tests/apfs_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/cocoa_time.py` & `dfdatetime-20230506/tests/cocoa_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/delphi_date_time.py` & `dfdatetime-20230506/tests/delphi_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/dotnet_datetime.py` & `dfdatetime-20230506/tests/dotnet_datetime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/factory.py` & `dfdatetime-20230506/tests/factory.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/fake_time.py` & `dfdatetime-20230506/tests/fake_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/fat_date_time.py` & `dfdatetime-20230506/tests/fat_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/filetime.py` & `dfdatetime-20230506/tests/filetime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/golang_time.py` & `dfdatetime-20230506/tests/golang_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/hfs_time.py` & `dfdatetime-20230506/tests/hfs_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/interface.py` & `dfdatetime-20230506/tests/interface.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/java_time.py` & `dfdatetime-20230506/tests/java_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/ole_automation_date.py` & `dfdatetime-20230506/tests/ole_automation_date.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/posix_time.py` & `dfdatetime-20230506/tests/posix_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/precisions.py` & `dfdatetime-20230506/tests/precisions.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/rfc2579_date_time.py` & `dfdatetime-20230506/tests/rfc2579_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/semantic_time.py` & `dfdatetime-20230506/tests/semantic_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/serializer.py` & `dfdatetime-20230506/tests/serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dfdatetime import dotnet_datetime
 from dfdatetime import fat_date_time
 from dfdatetime import golang_time
 from dfdatetime import posix_time
 from dfdatetime import rfc2579_date_time
 from dfdatetime import semantic_time
 from dfdatetime import serializer
+from dfdatetime import systemtime
 from dfdatetime import time_elements
 
 
 class SerializerTest(unittest.TestCase):
   """Tests for the date and time values serializer."""
 
   def testConvertDateTimeValuesToJSON(self):
@@ -113,14 +114,26 @@
         '__type__': 'DateTimeValues',
         'rfc2579_date_time_tuple': (2010, 8, 12, 20, 6, 31, 6, '+', 2, 0)}
 
     json_dict = serializer.Serializer.ConvertDateTimeValuesToJSON(
         rfc2579_date_time_object)
     self.assertEqual(json_dict, expected_json_dict)
 
+    systemtime_object = systemtime.Systemtime(
+        system_time_tuple=(2010, 8, 4, 12, 20, 6, 31, 142))
+
+    expected_json_dict = {
+        '__class_name__': 'Systemtime',
+        '__type__': 'DateTimeValues',
+        'system_time_tuple': (2010, 8, 4, 12, 20, 6, 31, 142)}
+
+    json_dict = serializer.Serializer.ConvertDateTimeValuesToJSON(
+        systemtime_object)
+    self.assertEqual(json_dict, expected_json_dict)
+
     time_elements_object = time_elements.TimeElements(
         is_delta=True, time_elements_tuple=(2010, 8, 12, 20, 6, 31))
 
     expected_json_dict = {
         '__class_name__': 'TimeElements',
         '__type__': 'DateTimeValues',
         'is_delta': True,
@@ -252,14 +265,26 @@
         rfc2579_date_time_tuple=(2010, 8, 12, 20, 6, 31, 6, '+', 2, 0))
 
     date_time_object = serializer.Serializer.ConvertJSONToDateTimeValues(
         json_dict)
     self.assertEqual(date_time_object, expected_date_time_object)
 
     json_dict = {
+        '__class_name__': 'Systemtime',
+        '__type__': 'DateTimeValues',
+        'system_time_tuple': (2010, 8, 4, 12, 20, 6, 31, 142)}
+
+    expected_date_time_object = systemtime.Systemtime(
+        system_time_tuple=(2010, 8, 4, 12, 20, 6, 31, 142))
+
+    date_time_object = serializer.Serializer.ConvertJSONToDateTimeValues(
+        json_dict)
+    self.assertEqual(date_time_object, expected_date_time_object)
+
+    json_dict = {
         '__class_name__': 'TimeElements',
         '__type__': 'DateTimeValues',
         'is_delta': True,
         'time_elements_tuple': (2010, 8, 12, 20, 6, 31)}
 
     expected_date_time_object = time_elements.TimeElements(
         is_delta=True, time_elements_tuple=(2010, 8, 12, 20, 6, 31))
```

### Comparing `dfdatetime-20230225/tests/systemtime.py` & `dfdatetime-20230506/tests/systemtime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/time_elements.py` & `dfdatetime-20230506/tests/time_elements.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/uuid_time.py` & `dfdatetime-20230506/tests/uuid_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/tests/webkit_time.py` & `dfdatetime-20230506/tests/webkit_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/utils/dependencies.py` & `dfdatetime-20230506/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20230225/utils/update_release.sh` & `dfdatetime-20230506/utils/update_release.sh`

 * *Files identical despite different names*

