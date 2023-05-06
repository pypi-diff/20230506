# Comparing `tmp/inverter-connect-0.5.0.tar.gz` & `tmp/inverter-connect-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.5.0.tar", last modified: Fri May  5 20:06:42 2023, max compression
+gzip compressed data, was "inverter-connect-0.6.0.tar", last modified: Sat May  6 11:20:24 2023, max compression
```

## Comparing `inverter-connect-0.5.0.tar` & `inverter-connect-0.6.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.5.0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.5.0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.827138 inverter-connect-0.5.0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.827138 inverter-connect-0.5.0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-03 17:50:50.000000 inverter-connect-0.5.0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.5.0/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)    15040 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)    14626 2023-05-05 19:51:29.000000 inverter-connect-0.5.0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.5.0/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.5.0/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.827138 inverter-connect-0.5.0/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-05 20:00:24.000000 inverter-connect-0.5.0/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.5.0/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4771 2023-05-05 20:00:11.000000 inverter-connect-0.5.0/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    13143 2023-05-05 19:50:36.000000 inverter-connect-0.5.0/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-05-03 17:42:33.000000 inverter-connect-0.5.0/inverter/cli/dev.py
--rw-rw-r--   0 jens      (1000) users      (100)      480 2023-05-05 17:29:20.000000 inverter-connect-0.5.0/inverter/config.py
--rw-rw-r--   0 jens      (1000) users      (100)    10438 2023-05-05 14:42:51.000000 inverter-connect-0.5.0/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      261 2023-04-27 15:55:08.000000 inverter-connect-0.5.0/inverter/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     1963 2023-05-05 19:06:27.000000 inverter-connect-0.5.0/inverter/daily_reset.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.5.0/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2784 2023-04-23 17:17:07.000000 inverter-connect-0.5.0/inverter/definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      429 2023-04-27 16:18:39.000000 inverter-connect-0.5.0/inverter/exceptions.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/test_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/test_doctests.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.5.0/inverter/mqtt4homeassistant/utilities/string_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     2943 2023-05-05 19:48:37.000000 inverter-connect-0.5.0/inverter/publish_loop.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.5.0/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3262 2023-04-24 15:18:26.000000 inverter-connect-0.5.0/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)      795 2023-04-27 15:42:06.000000 inverter-connect-0.5.0/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     5897 2023-05-05 19:10:09.000000 inverter-connect-0.5.0/inverter/tests/test_daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     1452 2023-04-23 17:17:07.000000 inverter-connect-0.5.0/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.5.0/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.5.0/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     3422 2023-05-05 19:51:25.000000 inverter-connect-0.5.0/inverter/tests/test_readme.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.5.0/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-04-28 07:13:12.000000 inverter-connect-0.5.0/inverter/utilities/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.5.0/inverter/utilities/credentials.py
--rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.5.0/inverter/utilities/log_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.5.0/inverter/utilities/modbus_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)    15040 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1634 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      269 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-05 20:06:42.000000 inverter-connect-0.5.0/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4830 2023-05-05 18:27:54.000000 inverter-connect-0.5.0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    50845 2023-05-05 18:28:31.000000 inverter-connect-0.5.0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     5305 2023-05-05 18:28:07.000000 inverter-connect-0.5.0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-05 20:06:42.831138 inverter-connect-0.5.0/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.6.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.6.0/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-03 17:50:50.000000 inverter-connect-0.6.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.6.0/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)    16300 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    15886 2023-05-06 10:27:49.000000 inverter-connect-0.6.0/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.6.0/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.6.0/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-06 10:44:15.000000 inverter-connect-0.6.0/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.6.0/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4788 2023-05-06 10:38:46.000000 inverter-connect-0.6.0/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    13773 2023-05-06 10:27:47.000000 inverter-connect-0.6.0/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-05-03 17:42:33.000000 inverter-connect-0.6.0/inverter/cli/dev.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10044 2023-05-06 10:26:14.000000 inverter-connect-0.6.0/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      312 2023-05-06 10:27:41.000000 inverter-connect-0.6.0/inverter/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.6.0/inverter/daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3686 2023-05-06 11:17:52.000000 inverter-connect-0.6.0/inverter/data_types.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.6.0/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)      213 2023-05-06 09:30:48.000000 inverter-connect-0.6.0/inverter/definitions/deye_2mppt_validations.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.6.0/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.6.0/inverter/exceptions.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/test_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/test_doctests.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/utilities/string_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3047 2023-05-06 10:27:47.000000 inverter-connect-0.6.0/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.6.0/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.6.0/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.6.0/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5880 2023-05-06 10:42:16.000000 inverter-connect-0.6.0/inverter/tests/test_daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1589 2023-05-06 10:41:55.000000 inverter-connect-0.6.0/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.6.0/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3422 2023-05-05 19:51:25.000000 inverter-connect-0.6.0/inverter/tests/test_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-06 11:19:29.000000 inverter-connect-0.6.0/inverter/tests/test_validators.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.6.0/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-05-06 10:25:25.000000 inverter-connect-0.6.0/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.6.0/inverter/utilities/credentials.py
+-rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.6.0/inverter/utilities/log_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.6.0/inverter/utilities/modbus_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.6.0/inverter/validators.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    16300 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1744 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      277 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4882 2023-05-06 09:28:26.000000 inverter-connect-0.6.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53370 2023-05-06 09:28:51.000000 inverter-connect-0.6.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     7830 2023-05-06 09:28:32.000000 inverter-connect-0.6.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/setup.cfg
```

### Comparing `inverter-connect-0.5.0/.github/workflows/tests.yml` & `inverter-connect-0.6.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/PKG-INFO` & `inverter-connect-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: inverter-connect
-Version: 0.5.0
-Summary: Get information from Deye Microinverter
-Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
-License: GPL-3.0-or-later
-Project-URL: Documentation, https://github.com/jedie/inverter-connect
-Project-URL: Source, https://github.com/jedie/inverter-connect
-Requires-Python: <4,>=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
@@ -72,20 +60,25 @@
 Usage: ./cli.py publish-loop [OPTIONS] IP
 
  Publish current data via MQTT for Home Assistant (endless loop)
  The "Daily Production" count will be cleared in the night, by set the current date time via
  AT-command.
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --log/--no-log                                            [default: log]                         │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
+│                                                              [default: 48899; 1000<=x<=65535]    │
+│                                                              [required]                          │
+│ *  --inverter                TEXT                            Prefix of yaml config files in      │
+│                                                              inverter/definitions/               │
+│                                                              [default: deye_2mppt]               │
+│                                                              [required]                          │
+│    --log/--no-log                                            [default: log]                      │
+│    --verbose/--no-verbose                                    [default: verbose]                  │
+│    --debug/--no-debug                                        [default: no-debug]                 │
+│    --help                                                    Show this message and exit.         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
 
 
 ----
 
@@ -98,18 +91,23 @@
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
 
  Print all known register values from Inverter, e.g.:
  .../inverter-connect$ ./cli.py print-values 192.168.123.456
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: no-debug]                        │
-│ --help                                                Show this message and exit.                │
+│    --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
+│                                                              [default: 48899; 1000<=x<=65535]    │
+│ *  --inverter                TEXT                            Prefix of yaml config files in      │
+│                                                              inverter/definitions/               │
+│                                                              [default: deye_2mppt]               │
+│                                                              [required]                          │
+│    --verbose/--no-verbose                                    [default: verbose]                  │
+│    --debug/--no-debug                                        [default: no-debug]                 │
+│    --help                                                    Show this message and exit.         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
 Example output of `print-values` call:
 
 ![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
@@ -135,18 +133,19 @@
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
  NTPSER NTPEN
  wait a while and request the current date time:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: no-debug]                        │
-│ --help                                                Show this message and exit.                │
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
 Example output of `print-at-commands` call:
 
 ![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
@@ -166,18 +165,19 @@
  e.g.: read 3 registers starting from 0x16:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
  e.g.: read the first 32 registers:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: debug]                           │
-│ --help                                                Show this message and exit.                │
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
 
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
```

### Comparing `inverter-connect-0.5.0/README.md` & `inverter-connect-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: inverter-connect
+Version: 0.6.0
+Summary: Get information from Deye Microinverter
+Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://github.com/jedie/inverter-connect
+Project-URL: Source, https://github.com/jedie/inverter-connect
+Requires-Python: <4,>=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # inverter
 
 [![tests](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/jedie/inverter-connect/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/github/jedie/inverter-connect/branch/main/graph/badge.svg)](https://app.codecov.io/github/jedie/inverter-connect)
 [![inverter-connect @ PyPi](https://img.shields.io/pypi/v/inverter-connect?label=inverter-connect%20%40%20PyPi)](https://pypi.org/project/inverter-connect/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/pyproject.toml)
 [![License GPL-3.0-or-later](https://img.shields.io/pypi/l/inverter-connect)](https://github.com/jedie/inverter-connect/blob/main/LICENSE)
@@ -60,20 +72,25 @@
 Usage: ./cli.py publish-loop [OPTIONS] IP
 
  Publish current data via MQTT for Home Assistant (endless loop)
  The "Daily Production" count will be cleared in the night, by set the current date time via
  AT-command.
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --log/--no-log                                            [default: log]                         │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
+│                                                              [default: 48899; 1000<=x<=65535]    │
+│                                                              [required]                          │
+│ *  --inverter                TEXT                            Prefix of yaml config files in      │
+│                                                              inverter/definitions/               │
+│                                                              [default: deye_2mppt]               │
+│                                                              [required]                          │
+│    --log/--no-log                                            [default: log]                      │
+│    --verbose/--no-verbose                                    [default: verbose]                  │
+│    --debug/--no-debug                                        [default: no-debug]                 │
+│    --help                                                    Show this message and exit.         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
 
 
 ----
 
@@ -86,18 +103,23 @@
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
 
  Print all known register values from Inverter, e.g.:
  .../inverter-connect$ ./cli.py print-values 192.168.123.456
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: no-debug]                        │
-│ --help                                                Show this message and exit.                │
+│    --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
+│                                                              [default: 48899; 1000<=x<=65535]    │
+│ *  --inverter                TEXT                            Prefix of yaml config files in      │
+│                                                              inverter/definitions/               │
+│                                                              [default: deye_2mppt]               │
+│                                                              [required]                          │
+│    --verbose/--no-verbose                                    [default: verbose]                  │
+│    --debug/--no-debug                                        [default: no-debug]                 │
+│    --help                                                    Show this message and exit.         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
 Example output of `print-values` call:
 
 ![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
@@ -123,18 +145,19 @@
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
  NTPSER NTPEN
  wait a while and request the current date time:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: no-debug]                        │
-│ --help                                                Show this message and exit.                │
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
 Example output of `print-at-commands` call:
 
 ![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
@@ -154,18 +177,19 @@
  e.g.: read 3 registers starting from 0x16:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
  e.g.: read the first 32 registers:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: debug]                           │
-│ --help                                                Show this message and exit.                │
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
 
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
```

### Comparing `inverter-connect-0.5.0/cli.py` & `inverter-connect-0.6.0/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/dev-cli.py` & `inverter-connect-0.6.0/dev-cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/.github/workflows/tests.yml` & `inverter-connect-0.6.0/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/api.py` & `inverter-connect-0.6.0/inverter/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,26 @@
 from __future__ import annotations
 
-import dataclasses
 import logging
 from collections.abc import Iterable
 from datetime import datetime
-from enum import Enum
 
 from rich import print  # noqa
+from rich.pretty import pprint
 
-from inverter.config import Config
-from inverter.connection import InverterSock, ModbusReadResult
+from inverter.connection import InverterSock
+from inverter.data_types import Config, InverterValue, ModbusReadResult, ValueType
 from inverter.definitions import get_parameter
+from inverter.exceptions import ValidationError
+from inverter.validators import InverterValueValidator
 
 
 logger = logging.getLogger(__name__)
 
 
-class ValueType(Enum):
-    READ_OUT = 'read out'
-    COMPUTED = 'computed'
-
-
-@dataclasses.dataclass
-class InverterValue:
-    type: ValueType
-    name: str
-    value: float | str
-    device_class: str  # e.g.: "voltage" / "current" / "energy" etc.
-    state_class: str | None  # e.g.: "measurement" / "total" / "total_increasing" etc.
-    unit: str  # e.g.: "V" / "A" / "kWh" etc.
-    result: ModbusReadResult | None
-
-
 def compute_values(values: dict) -> Iterable[InverterValue]:
     total_power = None
     for no in range(1, 10):
         section = f'PV{no}'
 
         voltage_name = f'{section} Voltage'
         current_name = f'{section} Current'
@@ -83,15 +68,16 @@
             result=None,
         )
 
 
 class Inverter:
     def __init__(self, config: Config):
         self.config = config
-        self.parameters = get_parameter(yaml_filename=config.yaml_filename, debug=config.debug)
+        self.parameters = get_parameter(config=config)
+        self.value_validator = InverterValueValidator(config=config)
         self.inv_sock = InverterSock(config)
 
     def __enter__(self):
         self.inv_sock.__enter__()
         return self
 
     def __iter__(self) -> Iterable[InverterValue]:
@@ -115,14 +101,23 @@
                 name=name,
                 value=result.parsed_value,
                 device_class=parameter.device_class,
                 state_class=parameter.state_class,
                 unit=parameter.unit,
                 result=result,
             )
+            if self.config.debug:
+                pprint(value, indent_guides=False)
+
+            try:
+                self.value_validator(inverter_value=value)
+            except ValidationError as err:
+                logger.info(f'Validation error: {err}')
+                raise
+
             assert name not in values, f'Double {name=}: {value=} - {values=}'
             values[name] = value
             yield value
 
         if values := compute_values(values):
             yield from values
```

### Comparing `inverter-connect-0.5.0/inverter/cli/cli_app.py` & `inverter-connect-0.6.0/inverter/cli/cli_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 from bx_py_utils.path import assert_is_file
 from rich import print  # noqa
 from rich.pretty import pprint
 from rich_click import RichGroup
 
 import inverter
 from inverter import constants
-from inverter.api import Inverter, ValueType, set_current_time
-from inverter.config import Config
-from inverter.connection import InverterInfo, InverterSock
+from inverter.api import Inverter, set_current_time
+from inverter.connection import InverterSock
 from inverter.constants import ERROR_STR_NO_DATA
-from inverter.definitions import Parameter
+from inverter.data_types import Config, InverterInfo, Parameter, ValueType
 from inverter.mqtt4homeassistant.data_classes import MqttSettings
 from inverter.mqtt4homeassistant.mqtt import get_connected_client
 from inverter.publish_loop import publish_forever
 from inverter.utilities.cli import convert_address_option, print_register
 from inverter.utilities.credentials import get_mqtt_settings, store_mqtt_settings
 from inverter.utilities.log_setup import basic_log_setup
 
@@ -49,14 +48,22 @@
         path_type=Path,
     )
 )
 ARGUMENT_EXISTING_FILE = dict(
     type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True, path_type=Path)
 )
 
+INVERTER_NAME = dict(
+    required=True,
+    type=str,
+    default='deye_2mppt',
+    help='Prefix of yaml config files in inverter/definitions/',
+    show_default=True,
+)
+
 
 class ClickGroup(RichGroup):  # FIXME: How to set the "info_name" easier?
     def make_context(self, info_name, *args, **kwargs):
         info_name = './cli.py'
         return super().make_context(info_name, *args, **kwargs)
 
 
@@ -79,24 +86,26 @@
 
 
 @click.command()
 @click.argument('ip')
 @click.option(
     '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
 )
+@click.option('--inverter', **INVERTER_NAME)
+@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
 @click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def print_values(ip, port, debug):
+def print_values(ip, port, inverter, verbose, debug):
     """
     Print all known register values from Inverter, e.g.:
 
     .../inverter-connect$ ./cli.py print-values 192.168.123.456
     """
     basic_log_setup(debug=debug)
 
-    config = Config(yaml_filename='deye_2mppt.yaml', host=ip, port=port, debug=debug)
+    config = Config(inverter_name=inverter, host=ip, port=port, verbose=verbose, debug=debug)
     with Inverter(config=config) as inverter:
         inverter_info: InverterInfo = inverter.inv_sock.inverter_info
         print(inverter_info)
         print()
 
         for value in inverter:
             print(f'\t* [yellow]{value.name:<31}[/yellow]:', end=' ')
@@ -126,16 +135,17 @@
 
 @click.command()
 @click.argument('ip')
 @click.argument('commands', nargs=-1)
 @click.option(
     '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
 )
+@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
 @click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def print_at_commands(ip, port, commands, debug):
+def print_at_commands(ip, port, commands, verbose, debug):
     """
     Print one or more AT command values from Inverter.
 
     Use all known AT commands, if no one is given, e.g.:
 
     .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456
 
@@ -197,15 +207,15 @@
             'NTPRF',  # NTP request interval in min (?)
             'NTPEN',  # Enable/Disable NTP Server
             'WSDNS',  # Set/Get the DNS Server address
             'DEVICENUM',  # Set/Get Device Link Num
             'DEVSELCTL',  # Set/Get Web Device List Info
         )
 
-    config = Config(yaml_filename=None, host=ip, port=port, debug=debug)
+    config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
     if debug:
         print(config)
 
     with InverterSock(config) as inv_sock:
         inverter_info: InverterInfo = inv_sock.inverter_info
         print(inverter_info)
         print()
@@ -221,27 +231,28 @@
 
 @click.command()
 @click.argument('ip')
 @click.option(
     '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
 )
 @click.option('--register', default="0x16", help='Start address', show_default=True)
+@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
 @click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
-def set_time(ip, port, register, debug):
+def set_time(ip, port, register, verbose, debug):
     """
     Set current date time in the inverter device.
 
     Default start address is 0x16, so that this will be filled:
         0x16 - year + month
         0x17 - day + hour
         0x18 - minute + second
     """
     address = convert_address_option(raw_address=register, debug=debug)
 
-    config = Config(yaml_filename=None, host=ip, port=port, debug=debug)
+    config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
     if debug:
         print(config)
 
     with InverterSock(config) as inv_sock:
         inverter_info: InverterInfo = inv_sock.inverter_info
         print(inverter_info)
         print()
@@ -262,18 +273,19 @@
 
 
 @click.command()
 @click.argument('ip')
 @click.option(
     '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
 )
-@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_TRUE)
 @click.argument('register')
 @click.argument('length', type=click.IntRange(1, 100))
-def read_register(ip, port, register, length, debug):
+@click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
+@click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
+def read_register(ip, port, register, length, verbose, debug):
     """
     Read register(s) from the inverter
 
     e.g.: read 3 registers starting from 0x16:
 
         .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
 
@@ -282,17 +294,15 @@
     .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
 
     The start address can be pass as decimal number or as hex string, e.g.: 0x123
     """
     print(f'Read {length} register(s) from {register=!r} ({ip}:{port})')
     address = convert_address_option(raw_address=register, debug=debug)
 
-    config = Config(yaml_filename=None, host=ip, port=port, debug=debug)
-    if debug:
-        print(config)
+    config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
 
     with InverterSock(config) as inv_sock:
         inverter_info: InverterInfo = inv_sock.inverter_info
         print(inverter_info)
         print()
         print_register(inv_sock, start_register=address, length=length)
 
@@ -376,30 +386,36 @@
 
 cli.add_command(test_mqtt_connection)
 
 
 @click.command()
 @click.argument('ip')
 @click.option(
-    '--port', type=click.IntRange(1000, 65535), default=48899, help='Port of the inverter', show_default=True
+    '--port',
+    type=click.IntRange(1000, 65535),
+    default=48899,
+    help='Port of the inverter',
+    show_default=True,
+    required=True,
 )
+@click.option('--inverter', **INVERTER_NAME)
 @click.option('--log/--no-log', **OPTION_ARGS_DEFAULT_TRUE)
 @click.option('--verbose/--no-verbose', **OPTION_ARGS_DEFAULT_TRUE)
 @click.option('--debug/--no-debug', **OPTION_ARGS_DEFAULT_FALSE)
-def publish_loop(ip, port, log, verbose, debug):
+def publish_loop(ip, port, inverter, log, verbose, debug):
     """
     Publish current data via MQTT for Home Assistant (endless loop)
 
     The "Daily Production" count will be cleared in the night,
     by set the current date time via AT-command.
     """
     if log:
         basic_log_setup(debug=debug)
 
-    config = Config(yaml_filename='deye_2mppt.yaml', host=ip, port=port, debug=debug)
+    config = Config(inverter_name=inverter, host=ip, port=port, verbose=verbose, debug=debug)
 
     mqtt_settings: MqttSettings = get_mqtt_settings()
     pprint(mqtt_settings.anonymized())
     try:
         publish_forever(mqtt_settings=mqtt_settings, config=config, verbose=verbose)
     except KeyboardInterrupt:
         print('Bye, bye')
```

### Comparing `inverter-connect-0.5.0/inverter/cli/dev.py` & `inverter-connect-0.6.0/inverter/cli/dev.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/connection.py` & `inverter-connect-0.6.0/inverter/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,23 @@
 from __future__ import annotations
 
-import dataclasses
 import logging
 import socket
 import time
 
 from rich import print  # noqa
 
-from inverter.config import Config
 from inverter.constants import AT_READ_FUNC_NUMBER, AT_WRITE_FUNC_NUMBER, ERROR_STR_NO_DATA
-from inverter.definitions import Parameter
+from inverter.data_types import Config, InverterInfo, ModbusReadResult, ModbusResponse, Parameter, RawModBusResponse
 from inverter.exceptions import CrcError, ModbusNoData, ModbusNoHexData, ParseModbusValueError, ReadTimeout
 
 
 logger = logging.getLogger(__name__)
 
 
-@dataclasses.dataclass
-class InverterInfo:
-    ip: str
-    mac: str
-    serial: int
-
-
-@dataclasses.dataclass
-class RawModBusResponse:
-    prefix: str
-    data: str
-
-
-@dataclasses.dataclass
-class ModbusResponse:
-    slave_id: int
-    modbus_function: int
-    data_hex: str
-
-
-@dataclasses.dataclass
-class ModbusReadResult:
-    parameter: Parameter
-    parsed_value: float | str
-    response: ModbusResponse = None
-
-
 def make_modbus_result(*, response: ModbusResponse, parameter: Parameter) -> ModbusReadResult:
     parser_func = parameter.parser
     data_hex = response.data_hex
     logger.debug('Call %s with %r', parser_func.__class__.__name__, data_hex)
     try:
         parsed_value = parser_func(
             data_hex=data_hex,
```

### Comparing `inverter-connect-0.5.0/inverter/daily_reset.py` & `inverter-connect-0.6.0/inverter/daily_reset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,16 @@
-import dataclasses
 import logging
 from datetime import datetime
 
-from inverter.api import Inverter, InverterValue, set_current_time
-from inverter.config import Config
-
+from inverter.api import Inverter, set_current_time
+from inverter.data_types import Config, InverterValue, ResetState
 
 logger = logging.getLogger(__name__)
 
 
-@dataclasses.dataclass
-class ResetState:
-    started: datetime
-    set_time_count: int = 0
-    successful_count: int = 0
-    last_success_dt: datetime = None
-    reset_needed: bool = False
-
-
 class DailyProductionReset:
     """
     Deye SUN600 will not automatically reset the "Daily Production" counter.
     Ro reset this counter it's needed to set the current time
     """
 
     def __init__(self, reset_state: ResetState, inverter: Inverter, config: Config):
```

### Comparing `inverter-connect-0.5.0/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.6.0/inverter/definitions/deye_2mppt.yaml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/definitions.py` & `inverter-connect-0.6.0/inverter/definitions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,44 @@
 from __future__ import annotations
 
-import dataclasses
 from collections.abc import Iterable
-from typing import Callable
 
 import yaml
 from bx_py_utils.dict_utils import pluck
 from bx_py_utils.path import assert_is_file
 
-from inverter.constants import BASE_PATH
+from inverter.data_types import Config, Parameter
 from inverter.utilities.modbus_converter import debug_converter, parse_number, parse_string, parse_swapped_number
 
 
-@dataclasses.dataclass
-class Parameter:
-    start_register: int
-    length: int
-    group: str
-    name: str  # e.g.: "PV1 Voltage" / "PV1 Current" / "Daily Production" etc.
-    device_class: str  # e.g.: "voltage" / "current" / "energy" etc.
-    state_class: str | None  # e.g.: "measurement" / "total" / "total_increasing" etc.
-    unit: str  # e.g.: "V" / "A" / "kWh" etc.
-    scale: float | int  # e.g.: 1 / 0.1
-    parser: Callable
-    offset: int | None = None
-    lookup: dict | None = None
-
-
 rule2converter = {
     1: parse_number,
     3: parse_swapped_number,
     5: parse_string,
 }
 
 
-def get_definition(yaml_filename):
-    yaml_path = BASE_PATH / 'definitions' / yaml_filename
-    assert_is_file(yaml_path)
-    content = yaml_path.read_text(encoding='UTF-8')
+def get_definition(*, config: Config):
+    definition_file_path = config.definition_file_path
+    assert_is_file(definition_file_path)
+    content = definition_file_path.read_text(encoding='UTF-8')
     data = yaml.safe_load(content)
     return data['parameters']
 
 
 def convert_lookup(raw_lookup: list):
     """
     >>> convert_lookup([{'key': 2, 'value': 'Normal'},{'key': 3, 'value': 'Warning'}])
     {2: 'Normal', 3: 'Warning'}
     """
     return {entry['key']: entry['value'] for entry in raw_lookup}
 
 
-def get_parameter(yaml_filename, debug=False) -> Iterable[Parameter]:
-    data = get_definition(yaml_filename)
+def get_parameter(*, config: Config) -> Iterable[Parameter]:
+    data = get_definition(config=config)
     parameters = []
     for group_data in data:
         group_name = group_data['group']
         for item in group_data['items']:
             # example = {
             #     'name': 'PV1 Voltage',
             #     'class': 'voltage',
```

### Comparing `inverter-connect-0.5.0/inverter/mqtt4homeassistant/converter.py` & `inverter-connect-0.6.0/inverter/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/mqtt4homeassistant/data_classes.py` & `inverter-connect-0.6.0/inverter/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/mqtt4homeassistant/mqtt.py` & `inverter-connect-0.6.0/inverter/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/mqtt4homeassistant/tests/test_converter.py` & `inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/publish_loop.py` & `inverter-connect-0.6.0/inverter/publish_loop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 import time
 from datetime import datetime
 
 from rich import print  # noqa
 
-from inverter.api import Inverter, InverterValue
-from inverter.config import Config
-from inverter.connection import InverterInfo
+from inverter.api import Inverter
 from inverter.constants import ERROR_STR_NO_DATA
-from inverter.daily_reset import DailyProductionReset, ResetState
-from inverter.exceptions import ReadInverterError, ReadTimeout
+from inverter.daily_reset import DailyProductionReset
+from inverter.data_types import Config, InverterInfo, InverterValue, ResetState
+from inverter.exceptions import ReadInverterError, ReadTimeout, ValidationError
 from inverter.mqtt4homeassistant.converter import values2mqtt_payload
 from inverter.mqtt4homeassistant.data_classes import HaValue, HaValues, MqttSettings
 from inverter.mqtt4homeassistant.mqtt import HaMqttPublisher
 
 
 logger = logging.getLogger(__name__)
 
@@ -46,14 +45,16 @@
                                     name=value.name,
                                     value=value.value,
                                     device_class=value.device_class,
                                     state_class=value.state_class,
                                     unit=value.unit,
                                 )
                             )
+                    except ValidationError as err:
+                        print(f'[red]Skip send values: {err}')
                     except ReadInverterError as err:
                         print(f'[red]{err}')
                     else:
                         values = HaValues(
                             device_name=str(inverter_info.serial),
                             values=values,
                             prefix='homeassistant',
```

### Comparing `inverter-connect-0.5.0/inverter/tests/test_api.py` & `inverter-connect-0.6.0/inverter/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest import TestCase
 
-from inverter.api import InverterValue, ValueType, compute_values
+from inverter.api import compute_values
+from inverter.data_types import InverterValue, ValueType
 
 
 class ApiTestCase(TestCase):
     def test_compute_values(self):
         results = list(compute_values(values={}))
         self.assertEqual(results, [])
```

### Comparing `inverter-connect-0.5.0/inverter/tests/test_connect.py` & `inverter-connect-0.6.0/inverter/tests/test_connect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest import TestCase
 
-from inverter.connection import ModbusResponse, Parameter, parse_modbus_response
+from inverter.connection import parse_modbus_response
+from inverter.data_types import ModbusResponse, Parameter
 
 
 def get_parameter(**kwargs) -> Parameter:
     used_kwargs = dict(
         start_register=0,
         length=0,
         name='',
```

### Comparing `inverter-connect-0.5.0/inverter/tests/test_daily_reset.py` & `inverter-connect-0.6.0/inverter/tests/test_daily_reset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 from datetime import datetime, timedelta
 from unittest import TestCase
 
 from freezegun import freeze_time
 
-from inverter.api import InverterValue, ValueType
-from inverter.config import Config
-from inverter.daily_reset import DailyProductionReset, ResetState
+from inverter.daily_reset import DailyProductionReset
+from inverter.data_types import Config, InverterValue, ResetState, ValueType
 
 
 class DailyProductionResetTestCase(TestCase):
     @freeze_time('2020-01-01T00:00:00+0000', as_kwarg='frozen_time')
     def test_happy_path(self, frozen_time):
         start_dt = datetime.now()
 
@@ -23,15 +22,15 @@
             def __init__(self):
                 self.inv_sock = self
 
             def write(self, *, address, values):
                 self.writes.append((address, values))
 
         inverter = InverterMock()
-        config = Config(yaml_filename=None, host='foo')
+        config = Config(inverter_name=None, verbose=False)
 
         with DailyProductionReset(reset_state, inverter, config) as daily_production_reset:
             self.assertEqual(
                 daily_production_reset.reset_state,
                 ResetState(started=start_dt, set_time_count=0, successful_count=0, reset_needed=False),
             )
```

### Comparing `inverter-connect-0.5.0/inverter/tests/test_definitions.py` & `inverter-connect-0.6.0/inverter/tests/test_definitions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from unittest import TestCase
 
-from inverter.definitions import Parameter, get_definition, get_parameter
+from inverter.data_types import Config, Parameter
+from inverter.definitions import get_definition, get_parameter
 from inverter.utilities.modbus_converter import parse_number
 
 
 class DefinitionsTestCase(TestCase):
     def test_get_definition(self):
-        result = get_definition(yaml_filename='deye_2mppt.yaml')
+        config = Config(inverter_name='deye_2mppt', verbose=False)
+        result = get_definition(config=config)
         self.assertIsInstance(result, list)
         example = result[0]['items'][0]
         self.assertEqual(
             example,
             {
                 'class': 'voltage',
                 'icon': 'mdi:solar-power',
@@ -20,15 +22,16 @@
                 'scale': 0.1,
                 'state_class': 'measurement',
                 'uom': 'V',
             },
         )
 
     def test_get_parameter(self):
-        parameters = get_parameter(yaml_filename='deye_2mppt.yaml')
+        config = Config(inverter_name='deye_2mppt', verbose=False)
+        parameters = get_parameter(config=config)
         self.assertIsInstance(parameters, list)
         example = parameters[0]
         self.assertEqual(
             example,
             Parameter(
                 start_register=109,
                 length=1,
```

### Comparing `inverter-connect-0.5.0/inverter/tests/test_project_setup.py` & `inverter-connect-0.6.0/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/tests/test_readme.py` & `inverter-connect-0.6.0/inverter/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/utilities/cli.py` & `inverter-connect-0.6.0/inverter/utilities/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bx_py_utils.iteration import chunk_iterable
 from rich import print  # noqa
 from rich.console import Console
 from rich.table import Table
 
-from inverter.connection import ModbusResponse
+from inverter.data_types import ModbusResponse
 from inverter.exceptions import ModbusNoData, ModbusNoHexData
 
 
 def convert_address_option(raw_address: str, debug: bool = True) -> int:
     """
     >>> convert_address_option(raw_address='0x123', debug=True)
     Address: 0x123
```

### Comparing `inverter-connect-0.5.0/inverter/utilities/credentials.py` & `inverter-connect-0.6.0/inverter/utilities/credentials.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter/utilities/modbus_converter.py` & `inverter-connect-0.6.0/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.5.0/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.6.0/inverter_connect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.5.0
+Version: 0.6.0
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -72,20 +72,25 @@
 Usage: ./cli.py publish-loop [OPTIONS] IP
 
  Publish current data via MQTT for Home Assistant (endless loop)
  The "Daily Production" count will be cleared in the night, by set the current date time via
  AT-command.
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
-│                                                           [default: 48899; 1000<=x<=65535]       │
-│ --log/--no-log                                            [default: log]                         │
-│ --verbose/--no-verbose                                    [default: verbose]                     │
-│ --debug/--no-debug                                        [default: no-debug]                    │
-│ --help                                                    Show this message and exit.            │
+│ *  --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
+│                                                              [default: 48899; 1000<=x<=65535]    │
+│                                                              [required]                          │
+│ *  --inverter                TEXT                            Prefix of yaml config files in      │
+│                                                              inverter/definitions/               │
+│                                                              [default: deye_2mppt]               │
+│                                                              [required]                          │
+│    --log/--no-log                                            [default: log]                      │
+│    --verbose/--no-verbose                                    [default: verbose]                  │
+│    --debug/--no-debug                                        [default: no-debug]                 │
+│    --help                                                    Show this message and exit.         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated publish-loop help end ✂✂✂)
 
 
 ----
 
@@ -98,18 +103,23 @@
 ```
 Usage: ./cli.py print-values [OPTIONS] IP
 
  Print all known register values from Inverter, e.g.:
  .../inverter-connect$ ./cli.py print-values 192.168.123.456
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: no-debug]                        │
-│ --help                                                Show this message and exit.                │
+│    --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                │
+│                                                              [default: 48899; 1000<=x<=65535]    │
+│ *  --inverter                TEXT                            Prefix of yaml config files in      │
+│                                                              inverter/definitions/               │
+│                                                              [default: deye_2mppt]               │
+│                                                              [required]                          │
+│    --verbose/--no-verbose                                    [default: verbose]                  │
+│    --debug/--no-debug                                        [default: no-debug]                 │
+│    --help                                                    Show this message and exit.         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-values help end ✂✂✂)
 
 Example output of `print-values` call:
 
 ![print-values](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-55.png "2023-04-28_08-55.png")
@@ -135,18 +145,19 @@
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPSER=192.168.1.1 NTPEN=on
  NTPSER NTPEN
  wait a while and request the current date time:
  .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
  (Note: The prefix "AT+" will be added to every command)
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: no-debug]                        │
-│ --help                                                Show this message and exit.                │
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated print-at-commands help end ✂✂✂)
 
 Example output of `print-at-commands` call:
 
 ![print-at-commands](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-57.png "2023-04-28_08-57.png")
@@ -166,18 +177,19 @@
  e.g.: read 3 registers starting from 0x16:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
  e.g.: read the first 32 registers:
  .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --port                INTEGER RANGE [1000<=x<=65535]  Port of the inverter                       │
-│                                                       [default: 48899; 1000<=x<=65535]           │
-│ --debug/--no-debug                                    [default: debug]                           │
-│ --help                                                Show this message and exit.                │
+│ --port                    INTEGER RANGE [1000<=x<=65535]  Port of the inverter                   │
+│                                                           [default: 48899; 1000<=x<=65535]       │
+│ --verbose/--no-verbose                                    [default: verbose]                     │
+│ --debug/--no-debug                                        [default: no-debug]                    │
+│ --help                                                    Show this message and exit.            │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated read-register help end ✂✂✂)
 
 Example output of `read-register` call:
 
 ![read-register](https://raw.githubusercontent.com/jedie/jedie.github.io/master/screenshots/inverter-connect/2023-04-28_08-53.png "2023-04-28_08-53.png")
```

### Comparing `inverter-connect-0.5.0/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.6.0/inverter_connect.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 .github/workflows/tests.yml
 inverter/.editorconfig
 inverter/.flake8
 inverter/.gitignore
 inverter/__init__.py
 inverter/__main__.py
 inverter/api.py
-inverter/config.py
 inverter/connection.py
 inverter/constants.py
 inverter/daily_reset.py
+inverter/data_types.py
 inverter/definitions.py
 inverter/exceptions.py
 inverter/publish_loop.py
+inverter/validators.py
 inverter/.github/workflows/tests.yml
 inverter/cli/__init__.py
 inverter/cli/cli_app.py
 inverter/cli/dev.py
 inverter/definitions/deye_2mppt.yaml
+inverter/definitions/deye_2mppt_validations.yaml
 inverter/mqtt4homeassistant/__init__.py
 inverter/mqtt4homeassistant/converter.py
 inverter/mqtt4homeassistant/data_classes.py
 inverter/mqtt4homeassistant/mqtt.py
 inverter/mqtt4homeassistant/tests/__init__.py
 inverter/mqtt4homeassistant/tests/test_converter.py
 inverter/mqtt4homeassistant/tests/test_doctests.py
@@ -39,14 +41,15 @@
 inverter/tests/test_api.py
 inverter/tests/test_connect.py
 inverter/tests/test_daily_reset.py
 inverter/tests/test_definitions.py
 inverter/tests/test_doctests.py
 inverter/tests/test_project_setup.py
 inverter/tests/test_readme.py
+inverter/tests/test_validators.py
 inverter/utilities/__init__.py
 inverter/utilities/cli.py
 inverter/utilities/credentials.py
 inverter/utilities/log_setup.py
 inverter/utilities/modbus_converter.py
 inverter_connect.egg-info/PKG-INFO
 inverter_connect.egg-info/SOURCES.txt
```

### Comparing `inverter-connect-0.5.0/pyproject.toml` & `inverter-connect-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 readme = "README.md"
 authors = [
     {name = 'Jens Diemer', email = 'inverter-connect@jensdiemer.de'}
 ]
 requires-python = ">=3.9,<4"
 dependencies = [
     "paho-mqtt",  # https://pypi.org/project/paho-mqtt/
+    "msgspec",  # https://github.com/jcrist/msgspec
     "pyyaml",  # https://github.com/yaml/pyyaml
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
 ]
 [project.optional-dependencies]
```

### Comparing `inverter-connect-0.5.0/requirements.dev.txt` & `inverter-connect-0.6.0/requirements.dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -459,14 +459,45 @@
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
 more-itertools==9.1.0 \
     --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
     --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
     # via jaraco-classes
+msgspec==0.14.2 \
+    --hash=sha256:03ddc8c518afbea4fb89afb587d77f11d00909f003966d437f31fb8fffdfac28 \
+    --hash=sha256:1c8f7e631fad9d5a33fcfb0f2a27eb86dc0390e91d6b51c95a604b7ccbc264f1 \
+    --hash=sha256:1fc99f0929fa91cc53fa35f59be366d67f116c2b7f0f3b29dc60e3179f6fb205 \
+    --hash=sha256:2039451b22813af2fd5cbe99eaecfc318d64fcee5af0ce5b3d5cce12427d24cd \
+    --hash=sha256:26bcb3a69b348be2757ab19e86038e586920522a99d49d358c12890fbcfb6aa8 \
+    --hash=sha256:3288b65ee7c78d08f32003a8b5ca72fff12c6a7400bd35f9d65630c9d58efce2 \
+    --hash=sha256:4f13e47803aedbb32c9375317fedbd20af3397dc024d311eebdc635c07f6f908 \
+    --hash=sha256:57a79cfa306fda2c66f4fc7eb72836c0f78fd9a6d748d028960b387797f0381b \
+    --hash=sha256:580464c7ca5c47a1422973c853301bbfd3d1a4184bdb6bddb73b5df094d8fc55 \
+    --hash=sha256:587371a65798a0f0182d0a7a4b7c4b87a5f46e25e8821c6474b3f717dcfcad14 \
+    --hash=sha256:59491de3566c7789bdb0a152f305e150a6ba3e825af471680b05a029a664a89a \
+    --hash=sha256:78361dadef4b993b8c4a887d3d267b89b0ea0846259eadf2fe993659e4dbf9c8 \
+    --hash=sha256:7e50885274e2041e49ec5d7cce8e59768f599c27dfb4c046edaf9ab25b1fddc2 \
+    --hash=sha256:87c4cd1bb197be11f89ad779038c8989d6ffcb8b360705107f034e4d2783c0a6 \
+    --hash=sha256:8927efaf506e5a8f9ffe76602e08d30a80c19b38d50a7e783887c317573ecd80 \
+    --hash=sha256:8b8a766b9f3e7f87946965a8ffc6e72f7a3ec8d031b3168df16762bfd3d03205 \
+    --hash=sha256:8ed61cad6b20f0218a8d239294c4b30b4e82854871ba0434cf0d54497043bffe \
+    --hash=sha256:907ed4305a97b50248e6b86e79ddc8edcf9b718eab0c93a6b46d673c5edbe3a4 \
+    --hash=sha256:94fc3d9a8835f18c18b48fdf49f7d445184061bfbc457a6623a4eb1f74ebe806 \
+    --hash=sha256:a0a3908309581e4e632457fac1938fec7fd84121396ddab6ddca37784e6db068 \
+    --hash=sha256:a12e704786256431d559c2027d6135a64f2339f009118d97906709cd8409e7ac \
+    --hash=sha256:b965c14851f146537f1b732cd2ed16c38e0c59662f23b72d396aee21e81aed4f \
+    --hash=sha256:d03861f0d271b696faefb1a885ea0c7dc7db70baaa05c7f18086f2b9085d1cb8 \
+    --hash=sha256:d469aede5d986223d6ec9a8d0713156f96fd6b427b12e14f81d26627a47687b9 \
+    --hash=sha256:d85e9bfd1441216010c084626d968e96a3d88d762959c5eb430de62076cd7fe9 \
+    --hash=sha256:decd1d2015d340ebfd58f29ed2916e118ca255b6a94fc1787a236a2654dfd8ff \
+    --hash=sha256:eee59e73982ca0d730f8d4e8fb5f01da9fa466490dea43ea1bcfa23b8a8bbc0d \
+    --hash=sha256:f97006b9c9e24e9677fb84f43586fb4d03a72eb426199656a1c24775c62b9fe4 \
+    --hash=sha256:ff7c987330e2be62eb8811bc2da33507e8edeb761f4fd343f2fa5fdafce4f989
+    # via inverter-connect (pyproject.toml)
 mypy==1.2.0 \
     --hash=sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521 \
     --hash=sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140 \
     --hash=sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48 \
     --hash=sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128 \
     --hash=sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336 \
     --hash=sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a \
```

### Comparing `inverter-connect-0.5.0/requirements.txt` & `inverter-connect-0.6.0/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -18,14 +18,45 @@
     --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
     --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
     # via rich
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
+msgspec==0.14.2 \
+    --hash=sha256:03ddc8c518afbea4fb89afb587d77f11d00909f003966d437f31fb8fffdfac28 \
+    --hash=sha256:1c8f7e631fad9d5a33fcfb0f2a27eb86dc0390e91d6b51c95a604b7ccbc264f1 \
+    --hash=sha256:1fc99f0929fa91cc53fa35f59be366d67f116c2b7f0f3b29dc60e3179f6fb205 \
+    --hash=sha256:2039451b22813af2fd5cbe99eaecfc318d64fcee5af0ce5b3d5cce12427d24cd \
+    --hash=sha256:26bcb3a69b348be2757ab19e86038e586920522a99d49d358c12890fbcfb6aa8 \
+    --hash=sha256:3288b65ee7c78d08f32003a8b5ca72fff12c6a7400bd35f9d65630c9d58efce2 \
+    --hash=sha256:4f13e47803aedbb32c9375317fedbd20af3397dc024d311eebdc635c07f6f908 \
+    --hash=sha256:57a79cfa306fda2c66f4fc7eb72836c0f78fd9a6d748d028960b387797f0381b \
+    --hash=sha256:580464c7ca5c47a1422973c853301bbfd3d1a4184bdb6bddb73b5df094d8fc55 \
+    --hash=sha256:587371a65798a0f0182d0a7a4b7c4b87a5f46e25e8821c6474b3f717dcfcad14 \
+    --hash=sha256:59491de3566c7789bdb0a152f305e150a6ba3e825af471680b05a029a664a89a \
+    --hash=sha256:78361dadef4b993b8c4a887d3d267b89b0ea0846259eadf2fe993659e4dbf9c8 \
+    --hash=sha256:7e50885274e2041e49ec5d7cce8e59768f599c27dfb4c046edaf9ab25b1fddc2 \
+    --hash=sha256:87c4cd1bb197be11f89ad779038c8989d6ffcb8b360705107f034e4d2783c0a6 \
+    --hash=sha256:8927efaf506e5a8f9ffe76602e08d30a80c19b38d50a7e783887c317573ecd80 \
+    --hash=sha256:8b8a766b9f3e7f87946965a8ffc6e72f7a3ec8d031b3168df16762bfd3d03205 \
+    --hash=sha256:8ed61cad6b20f0218a8d239294c4b30b4e82854871ba0434cf0d54497043bffe \
+    --hash=sha256:907ed4305a97b50248e6b86e79ddc8edcf9b718eab0c93a6b46d673c5edbe3a4 \
+    --hash=sha256:94fc3d9a8835f18c18b48fdf49f7d445184061bfbc457a6623a4eb1f74ebe806 \
+    --hash=sha256:a0a3908309581e4e632457fac1938fec7fd84121396ddab6ddca37784e6db068 \
+    --hash=sha256:a12e704786256431d559c2027d6135a64f2339f009118d97906709cd8409e7ac \
+    --hash=sha256:b965c14851f146537f1b732cd2ed16c38e0c59662f23b72d396aee21e81aed4f \
+    --hash=sha256:d03861f0d271b696faefb1a885ea0c7dc7db70baaa05c7f18086f2b9085d1cb8 \
+    --hash=sha256:d469aede5d986223d6ec9a8d0713156f96fd6b427b12e14f81d26627a47687b9 \
+    --hash=sha256:d85e9bfd1441216010c084626d968e96a3d88d762959c5eb430de62076cd7fe9 \
+    --hash=sha256:decd1d2015d340ebfd58f29ed2916e118ca255b6a94fc1787a236a2654dfd8ff \
+    --hash=sha256:eee59e73982ca0d730f8d4e8fb5f01da9fa466490dea43ea1bcfa23b8a8bbc0d \
+    --hash=sha256:f97006b9c9e24e9677fb84f43586fb4d03a72eb426199656a1c24775c62b9fe4 \
+    --hash=sha256:ff7c987330e2be62eb8811bc2da33507e8edeb761f4fd343f2fa5fdafce4f989
+    # via inverter-connect (pyproject.toml)
 paho-mqtt==1.6.1 \
     --hash=sha256:2a8291c81623aec00372b5a85558a372c747cbca8e9934dfe218638b8eefc26f
     # via inverter-connect (pyproject.toml)
 pygments==2.15.1 \
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
     # via rich
```

