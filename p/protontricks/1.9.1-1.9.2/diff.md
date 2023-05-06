# Comparing `tmp/protontricks-1.9.1.tar.gz` & `tmp/protontricks-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protontricks-1.9.1.tar", last modified: Sun Aug 28 09:15:56 2022, max compression
+gzip compressed data, was "protontricks-1.9.2.tar", last modified: Fri Sep 16 14:31:37 2022, max compression
```

## Comparing `protontricks-1.9.1.tar` & `protontricks-1.9.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.748281 protontricks-1.9.1/.github/
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.748281 protontricks-1.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1080 2022-02-26 07:51:17.000000 protontricks-1.9.1/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.748281 protontricks-1.9.1/.github/workflows/
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1526 2022-08-18 15:09:31.000000 protontricks-1.9.1/.github/workflows/tests.yml
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1534 2022-02-26 07:51:17.000000 protontricks-1.9.1/.gitignore
--rw-r--r--   0 matoking  (1000) matoking  (1000)    12068 2022-08-28 09:14:54.000000 protontricks-1.9.1/CHANGELOG.md
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1094 2020-01-26 13:49:51.000000 protontricks-1.9.1/CONTRIBUTING.md
--rw-r--r--   0 matoking  (1000) matoking  (1000)    35147 2020-01-26 13:49:51.000000 protontricks-1.9.1/LICENSE
--rw-r--r--   0 matoking  (1000) matoking  (1000)      136 2021-07-24 15:10:40.000000 protontricks-1.9.1/MANIFEST.in
--rw-r--r--   0 matoking  (1000) matoking  (1000)      319 2021-07-31 13:06:23.000000 protontricks-1.9.1/Makefile
--rw-r--r--   0 matoking  (1000) matoking  (1000)     9642 2022-08-28 09:15:56.751614 protontricks-1.9.1/PKG-INFO
--rw-r--r--   0 matoking  (1000) matoking  (1000)     8813 2022-08-04 16:10:34.000000 protontricks-1.9.1/README.md
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1823 2021-04-12 16:48:34.000000 protontricks-1.9.1/TROUBLESHOOTING.md
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/data/
--rw-r--r--   0 matoking  (1000) matoking  (1000)     2411 2022-08-28 09:15:17.000000 protontricks-1.9.1/data/com.github.Matoking.protontricks.metainfo.xml
--rw-r--r--   0 matoking  (1000) matoking  (1000)    73771 2021-08-26 14:49:55.000000 protontricks-1.9.1/data/screenshot.png
--rw-r--r--   0 matoking  (1000) matoking  (1000)      264 2022-08-22 16:45:23.000000 protontricks-1.9.1/pyproject.toml
--rw-r--r--   0 matoking  (1000) matoking  (1000)        9 2022-04-30 09:22:33.000000 protontricks-1.9.1/requirements.txt
--rw-r--r--   0 matoking  (1000) matoking  (1000)       44 2020-09-18 10:10:17.000000 protontricks-1.9.1/requirements_dev.txt
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1379 2022-08-28 09:15:56.751614 protontricks-1.9.1/setup.cfg
--rw-r--r--   0 matoking  (1000) matoking  (1000)      502 2022-08-22 16:45:23.000000 protontricks-1.9.1/setup.py
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.748281 protontricks-1.9.1/src/
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/src/protontricks/
--rw-r--r--   0 matoking  (1000) matoking  (1000)      217 2020-01-26 13:49:51.000000 protontricks-1.9.1/src/protontricks/__init__.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)      176 2022-08-28 09:15:56.000000 protontricks-1.9.1/src/protontricks/_version.py
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/src/protontricks/cli/
--rw-r--r--   0 matoking  (1000) matoking  (1000)        0 2021-07-24 15:10:40.000000 protontricks-1.9.1/src/protontricks/cli/__init__.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1675 2022-02-26 07:51:17.000000 protontricks-1.9.1/src/protontricks/cli/desktop_install.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     5897 2022-04-30 09:22:33.000000 protontricks-1.9.1/src/protontricks/cli/launch.py
--rwxr-xr-x   0 matoking  (1000) matoking  (1000)    13215 2022-06-19 09:25:28.000000 protontricks-1.9.1/src/protontricks/cli/main.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     4976 2022-04-30 09:22:33.000000 protontricks-1.9.1/src/protontricks/cli/util.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1291 2022-04-30 09:22:33.000000 protontricks-1.9.1/src/protontricks/config.py
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.748281 protontricks-1.9.1/src/protontricks/data/
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/src/protontricks/data/data/
--rw-r--r--   0 matoking  (1000) matoking  (1000)     4758 2022-02-26 07:51:17.000000 protontricks-1.9.1/src/protontricks/data/data/icon_placeholder.png
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/src/protontricks/data/scripts/
--rw-r--r--   0 matoking  (1000) matoking  (1000)     2161 2022-08-16 16:46:12.000000 protontricks-1.9.1/src/protontricks/data/scripts/bwrap_launcher.sh
--rw-r--r--   0 matoking  (1000) matoking  (1000)     7497 2022-08-16 16:46:12.000000 protontricks-1.9.1/src/protontricks/data/scripts/wine_launch.sh
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1312 2022-08-16 16:37:35.000000 protontricks-1.9.1/src/protontricks/data/scripts/wineserver_keepalive.bat
--rw-r--r--   0 matoking  (1000) matoking  (1000)     2429 2022-04-30 09:22:33.000000 protontricks-1.9.1/src/protontricks/data/scripts/wineserver_keepalive.sh
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.748281 protontricks-1.9.1/src/protontricks/data/share/
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/src/protontricks/data/share/applications/
--rw-r--r--   0 matoking  (1000) matoking  (1000)      243 2022-02-26 07:51:17.000000 protontricks-1.9.1/src/protontricks/data/share/applications/protontricks-launch.desktop
--rw-r--r--   0 matoking  (1000) matoking  (1000)      247 2022-02-26 07:51:17.000000 protontricks-1.9.1/src/protontricks/data/share/applications/protontricks.desktop
--rw-r--r--   0 matoking  (1000) matoking  (1000)     3766 2022-04-30 09:22:33.000000 protontricks-1.9.1/src/protontricks/flatpak.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)    11027 2022-04-30 09:22:33.000000 protontricks-1.9.1/src/protontricks/gui.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)    40293 2022-08-25 16:32:50.000000 protontricks-1.9.1/src/protontricks/steam.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)    15041 2022-08-16 16:46:12.000000 protontricks-1.9.1/src/protontricks/util.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1007 2021-05-03 16:31:01.000000 protontricks-1.9.1/src/protontricks/winetricks.py
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/src/protontricks.egg-info/
--rw-r--r--   0 matoking  (1000) matoking  (1000)     9642 2022-08-28 09:15:56.000000 protontricks-1.9.1/src/protontricks.egg-info/PKG-INFO
--rw-r--r--   0 matoking  (1000) matoking  (1000)     1579 2022-08-28 09:15:56.000000 protontricks-1.9.1/src/protontricks.egg-info/SOURCES.txt
--rw-r--r--   0 matoking  (1000) matoking  (1000)        1 2022-08-28 09:15:56.000000 protontricks-1.9.1/src/protontricks.egg-info/dependency_links.txt
--rw-r--r--   0 matoking  (1000) matoking  (1000)      177 2022-08-28 09:15:56.000000 protontricks-1.9.1/src/protontricks.egg-info/entry_points.txt
--rw-r--r--   0 matoking  (1000) matoking  (1000)       20 2022-08-28 09:15:56.000000 protontricks-1.9.1/src/protontricks.egg-info/requires.txt
--rw-r--r--   0 matoking  (1000) matoking  (1000)       13 2022-08-28 09:15:56.000000 protontricks-1.9.1/src/protontricks.egg-info/top_level.txt
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/tests/
-drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-08-28 09:15:56.751614 protontricks-1.9.1/tests/cli/
--rw-r--r--   0 matoking  (1000) matoking  (1000)        0 2021-08-07 08:09:57.000000 protontricks-1.9.1/tests/cli/__init__.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)      534 2022-04-30 09:22:33.000000 protontricks-1.9.1/tests/cli/test_desktop_install.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     6718 2022-04-30 09:22:33.000000 protontricks-1.9.1/tests/cli/test_launch.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)    32054 2022-06-19 09:25:28.000000 protontricks-1.9.1/tests/cli/test_main.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     3587 2022-04-30 09:22:33.000000 protontricks-1.9.1/tests/cli/test_util.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)    25904 2022-05-10 17:39:38.000000 protontricks-1.9.1/tests/conftest.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)      901 2022-04-30 09:22:33.000000 protontricks-1.9.1/tests/test_config.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     6082 2022-04-30 09:22:33.000000 protontricks-1.9.1/tests/test_flatpak.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)    11173 2022-04-30 09:22:33.000000 protontricks-1.9.1/tests/test_gui.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)    33842 2022-08-25 16:32:50.000000 protontricks-1.9.1/tests/test_steam.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)     5628 2022-04-30 09:22:33.000000 protontricks-1.9.1/tests/test_util.py
--rw-r--r--   0 matoking  (1000) matoking  (1000)      704 2020-12-07 17:21:58.000000 protontricks-1.9.1/tests/test_winetricks.py
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.569876 protontricks-1.9.2/
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.563209 protontricks-1.9.2/.github/
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.563209 protontricks-1.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1080 2022-02-26 07:51:17.000000 protontricks-1.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.563209 protontricks-1.9.2/.github/workflows/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1526 2022-08-18 15:09:31.000000 protontricks-1.9.2/.github/workflows/tests.yml
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1534 2022-02-26 07:51:17.000000 protontricks-1.9.2/.gitignore
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    12270 2022-09-16 14:29:37.000000 protontricks-1.9.2/CHANGELOG.md
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1094 2020-01-26 13:49:51.000000 protontricks-1.9.2/CONTRIBUTING.md
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    35147 2020-01-26 13:49:51.000000 protontricks-1.9.2/LICENSE
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      136 2021-07-24 15:10:40.000000 protontricks-1.9.2/MANIFEST.in
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      319 2021-07-31 13:06:23.000000 protontricks-1.9.2/Makefile
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     9640 2022-09-16 14:31:37.569876 protontricks-1.9.2/PKG-INFO
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     8813 2022-09-15 16:44:25.000000 protontricks-1.9.2/README.md
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1823 2021-04-12 16:48:34.000000 protontricks-1.9.2/TROUBLESHOOTING.md
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.563209 protontricks-1.9.2/data/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     2462 2022-09-16 14:28:43.000000 protontricks-1.9.2/data/com.github.Matoking.protontricks.metainfo.xml
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    73771 2021-08-26 14:49:55.000000 protontricks-1.9.2/data/screenshot.png
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      264 2022-09-03 19:32:23.000000 protontricks-1.9.2/pyproject.toml
+-rw-r--r--   0 matoking  (1000) matoking  (1000)        9 2022-04-30 09:22:33.000000 protontricks-1.9.2/requirements.txt
+-rw-r--r--   0 matoking  (1000) matoking  (1000)       44 2020-09-18 10:10:17.000000 protontricks-1.9.2/requirements_dev.txt
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1379 2022-09-16 14:31:37.569876 protontricks-1.9.2/setup.cfg
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      502 2022-09-03 19:32:23.000000 protontricks-1.9.2/setup.py
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.563209 protontricks-1.9.2/src/
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.566543 protontricks-1.9.2/src/protontricks/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      217 2020-01-26 13:49:51.000000 protontricks-1.9.2/src/protontricks/__init__.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      176 2022-09-16 14:31:36.000000 protontricks-1.9.2/src/protontricks/_version.py
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.566543 protontricks-1.9.2/src/protontricks/cli/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)        0 2021-07-24 15:10:40.000000 protontricks-1.9.2/src/protontricks/cli/__init__.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1675 2022-02-26 07:51:17.000000 protontricks-1.9.2/src/protontricks/cli/desktop_install.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     5897 2022-04-30 09:22:33.000000 protontricks-1.9.2/src/protontricks/cli/launch.py
+-rwxr-xr-x   0 matoking  (1000) matoking  (1000)    13215 2022-06-19 09:25:28.000000 protontricks-1.9.2/src/protontricks/cli/main.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     4976 2022-04-30 09:22:33.000000 protontricks-1.9.2/src/protontricks/cli/util.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1291 2022-04-30 09:22:33.000000 protontricks-1.9.2/src/protontricks/config.py
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.563209 protontricks-1.9.2/src/protontricks/data/
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.566543 protontricks-1.9.2/src/protontricks/data/data/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     4758 2022-02-26 07:51:17.000000 protontricks-1.9.2/src/protontricks/data/data/icon_placeholder.png
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.569876 protontricks-1.9.2/src/protontricks/data/scripts/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     2165 2022-09-05 17:28:22.000000 protontricks-1.9.2/src/protontricks/data/scripts/bwrap_launcher.sh
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     7731 2022-09-05 17:28:22.000000 protontricks-1.9.2/src/protontricks/data/scripts/wine_launch.sh
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1312 2022-08-16 16:37:35.000000 protontricks-1.9.2/src/protontricks/data/scripts/wineserver_keepalive.bat
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     2429 2022-09-06 18:00:39.000000 protontricks-1.9.2/src/protontricks/data/scripts/wineserver_keepalive.sh
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.563209 protontricks-1.9.2/src/protontricks/data/share/
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.569876 protontricks-1.9.2/src/protontricks/data/share/applications/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      243 2022-09-15 15:54:59.000000 protontricks-1.9.2/src/protontricks/data/share/applications/protontricks-launch.desktop
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      247 2022-09-15 15:54:59.000000 protontricks-1.9.2/src/protontricks/data/share/applications/protontricks.desktop
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     3766 2022-04-30 09:22:33.000000 protontricks-1.9.2/src/protontricks/flatpak.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    11027 2022-09-15 15:54:59.000000 protontricks-1.9.2/src/protontricks/gui.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    40293 2022-09-03 19:32:23.000000 protontricks-1.9.2/src/protontricks/steam.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    15041 2022-09-03 19:32:23.000000 protontricks-1.9.2/src/protontricks/util.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1007 2021-05-03 16:31:01.000000 protontricks-1.9.2/src/protontricks/winetricks.py
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.566543 protontricks-1.9.2/src/protontricks.egg-info/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     9640 2022-09-16 14:31:37.000000 protontricks-1.9.2/src/protontricks.egg-info/PKG-INFO
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     1579 2022-09-16 14:31:37.000000 protontricks-1.9.2/src/protontricks.egg-info/SOURCES.txt
+-rw-r--r--   0 matoking  (1000) matoking  (1000)        1 2022-09-16 14:31:37.000000 protontricks-1.9.2/src/protontricks.egg-info/dependency_links.txt
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      177 2022-09-16 14:31:37.000000 protontricks-1.9.2/src/protontricks.egg-info/entry_points.txt
+-rw-r--r--   0 matoking  (1000) matoking  (1000)       20 2022-09-16 14:31:37.000000 protontricks-1.9.2/src/protontricks.egg-info/requires.txt
+-rw-r--r--   0 matoking  (1000) matoking  (1000)       13 2022-09-16 14:31:37.000000 protontricks-1.9.2/src/protontricks.egg-info/top_level.txt
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.569876 protontricks-1.9.2/tests/
+drwxr-xr-x   0 matoking  (1000) matoking  (1000)        0 2022-09-16 14:31:37.569876 protontricks-1.9.2/tests/cli/
+-rw-r--r--   0 matoking  (1000) matoking  (1000)        0 2021-08-07 08:09:57.000000 protontricks-1.9.2/tests/cli/__init__.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      534 2022-04-30 09:22:33.000000 protontricks-1.9.2/tests/cli/test_desktop_install.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     6718 2022-04-30 09:22:33.000000 protontricks-1.9.2/tests/cli/test_launch.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    32054 2022-06-19 09:25:28.000000 protontricks-1.9.2/tests/cli/test_main.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     3587 2022-04-30 09:22:33.000000 protontricks-1.9.2/tests/cli/test_util.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    25904 2022-05-10 17:39:38.000000 protontricks-1.9.2/tests/conftest.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      901 2022-04-30 09:22:33.000000 protontricks-1.9.2/tests/test_config.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     6082 2022-04-30 09:22:33.000000 protontricks-1.9.2/tests/test_flatpak.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    11173 2022-04-30 09:22:33.000000 protontricks-1.9.2/tests/test_gui.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)    33842 2022-09-03 19:32:23.000000 protontricks-1.9.2/tests/test_steam.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)     5628 2022-04-30 09:22:33.000000 protontricks-1.9.2/tests/test_util.py
+-rw-r--r--   0 matoking  (1000) matoking  (1000)      704 2020-12-07 17:21:58.000000 protontricks-1.9.2/tests/test_winetricks.py
```

### Comparing `protontricks-1.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `protontricks-1.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/.github/workflows/tests.yml` & `protontricks-1.9.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/.gitignore` & `protontricks-1.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/CHANGELOG.md` & `protontricks-1.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 
+## [1.9.2] - 2022-09-16
+### Fixed
+ - Fix random crashes when running Wine commands due to race condition in Wine launcher script
+
 ## [1.9.1] - 2022-08-28
 ### Added
  - Print a warning when multiple Steam directories are detected and `STEAM_DIR` is not used to specify the directory
  
 ### Changed
  - Launch Steam Runtime sandbox with `--bus-name` parameter instead of the now deprecated `--socket`
 
@@ -222,15 +226,16 @@
  - Corrupted appmanifest files are now skipped. See [Sirmentio/protontricks#36](https://github.com/Sirmentio/protontricks/pull/36).
  - Display a proper error message when $STEAM_DIR doesn't point to a valid Steam installation. See [Sirmentio/protontricks#46](https://github.com/Sirmentio/protontricks/issues/46).
 
 ## 1.0 - 2019-01-16
 ### Added
  - The last release of Protontricks maintained by [@Sirmentio](https://github.com/Sirmentio).
 
-[Unreleased]: https://github.com/Matoking/protontricks/compare/1.9.1...HEAD
+[Unreleased]: https://github.com/Matoking/protontricks/compare/1.9.2...HEAD
+[1.9.2]: https://github.com/Matoking/protontricks/compare/1.9.1...1.9.2
 [1.9.1]: https://github.com/Matoking/protontricks/compare/1.9.0...1.9.1
 [1.9.0]: https://github.com/Matoking/protontricks/compare/1.8.2...1.9.0
 [1.8.2]: https://github.com/Matoking/protontricks/compare/1.8.1...1.8.2
 [1.8.1]: https://github.com/Matoking/protontricks/compare/1.8.0...1.8.1
 [1.8.0]: https://github.com/Matoking/protontricks/compare/1.7.0...1.8.0
 [1.7.0]: https://github.com/Matoking/protontricks/compare/1.6.2...1.7.0
 [1.6.2]: https://github.com/Matoking/protontricks/compare/1.6.1...1.6.2
```

### Comparing `protontricks-1.9.1/CONTRIBUTING.md` & `protontricks-1.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/LICENSE` & `protontricks-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/PKG-INFO` & `protontricks-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protontricks
-Version: 1.9.1
+Version: 1.9.2
 Summary: A simple wrapper for running Winetricks commands for Proton-enabled games.
 Home-page: https://github.com/Matoking/protontricks
 Author: Janne Pulkkinen
 Author-email: janne.pulkkinen@protonmail.com
 License: GPL3
 Platform: linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -35,15 +35,15 @@
 
 # What is it?
 
 This is a wrapper script that allows you to easily run Winetricks commands for Steam Play/Proton games among other common Wine features, such as launching external Windows executables. This is often useful when a game requires closed-source runtime libraries or applications that are not included with Proton.
 
 # Requirements
 
-* Python 3.5 or newer
+* Python 3.6 or newer
 * Winetricks
 * Steam
 * YAD (recommended) **or** Zenity. Required for GUI.
 
 # Usage
 
 **Protontricks can be launched from desktop or using the `protontricks` command.**
@@ -212,9 +212,7 @@
 python3 -m pip install --user protontricks
 ```
 
 To install the latest development version (requires `git`):
 ```sh
 sudo python3 -m pip install git+https://github.com/Matoking/protontricks.git
 ```
-
-
```

### Comparing `protontricks-1.9.1/README.md` & `protontricks-1.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # What is it?
 
 This is a wrapper script that allows you to easily run Winetricks commands for Steam Play/Proton games among other common Wine features, such as launching external Windows executables. This is often useful when a game requires closed-source runtime libraries or applications that are not included with Proton.
 
 # Requirements
 
-* Python 3.5 or newer
+* Python 3.6 or newer
 * Winetricks
 * Steam
 * YAD (recommended) **or** Zenity. Required for GUI.
 
 # Usage
 
 **Protontricks can be launched from desktop or using the `protontricks` command.**
```

### Comparing `protontricks-1.9.1/TROUBLESHOOTING.md` & `protontricks-1.9.2/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/data/com.github.Matoking.protontricks.metainfo.xml` & `protontricks-1.9.2/data/com.github.Matoking.protontricks.metainfo.xml`

 * *Files 11% similar despite different names*

#### Comparing `protontricks-1.9.1/data/com.github.Matoking.protontricks.metainfo.xml` & `protontricks-1.9.2/data/com.github.Matoking.protontricks.metainfo.xml`

```diff
@@ -32,14 +32,15 @@
   <url type="homepage">https://github.com/Matoking/protontricks</url>
   <url type="help">https://github.com/Matoking/protontricks#readme</url>
   <url type="bugtracker">https://github.com/Matoking/protontricks/issues</url>
   <project_license>GPL-3.0</project_license>
   <metadata_license>CC0-1.0</metadata_license>
   <update_contact>janne.pulkkinen@protonmail.com</update_contact>
   <releases>
+    <release version="1.9.2" date="2022-09-16"/>
     <release version="1.9.1" date="2022-08-28"/>
     <release version="1.9.0" date="2022-07-02"/>
     <release version="1.8.2" date="2022-05-16"/>
     <release version="1.8.1" date="2022-03-20"/>
     <release version="1.8.0" date="2022-02-26"/>
     <release version="1.7.0" date="2022-01-08"/>
     <release version="1.6.2" date="2021-11-28"/>
```

### Comparing `protontricks-1.9.1/data/screenshot.png` & `protontricks-1.9.2/data/screenshot.png`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/setup.cfg` & `protontricks-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/cli/desktop_install.py` & `protontricks-1.9.2/src/protontricks/cli/desktop_install.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/cli/launch.py` & `protontricks-1.9.2/src/protontricks/cli/launch.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/cli/main.py` & `protontricks-1.9.2/src/protontricks/cli/main.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/cli/util.py` & `protontricks-1.9.2/src/protontricks/cli/util.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/config.py` & `protontricks-1.9.2/src/protontricks/config.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/data/data/icon_placeholder.png` & `protontricks-1.9.2/src/protontricks/data/data/icon_placeholder.png`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/data/scripts/bwrap_launcher.sh` & `protontricks-1.9.2/src/protontricks/data/scripts/bwrap_launcher.sh`

 * *Files 4% similar despite different names*

```diff
@@ -78,8 +78,8 @@
 done
 
 log_info "Following directories will be mounted inside container: ${mount_dirs[*]}"
 log_info "Using temporary directory: $PROTONTRICKS_TEMP_PATH"
 
 exec "$STEAM_RUNTIME_PATH"/run --share-pid --launcher \
 "${mount_params[@]}" -- \
---bus-name="com.github.Matoking.protontricks.App$STEAM_APPID-$PROTONTRICKS_SESSION_ID"
+--bus-name="com.github.Matoking.protontricks.App${STEAM_APPID}_${PROTONTRICKS_SESSION_ID}"
```

### Comparing `protontricks-1.9.1/src/protontricks/data/scripts/wine_launch.sh` & `protontricks-1.9.2/src/protontricks/data/scripts/wine_launch.sh`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,19 @@
             wineserver_pid="$pid"
 
             log_info "Found running wineserver instance with PID ${wineserver_pid}"
         fi
     done < <(pgrep "wineserver$")
 
     if [[ "$wineserver_found" = true ]]; then
-        # wineserver found, retrieve its environment variables
-        wineserver_env_vars=$(xargs -0 -L1 -a "/proc/${wineserver_pid}/environ")
+        # wineserver found, retrieve its environment variables.
+        # wineserver might disappear from under our foot especially if we're
+        # in the middle of running a lot of Wine commands in succession,
+        # so don't assume the wineserver still exists.
+        wineserver_env_vars=$(xargs -0 -L1 -a "/proc/${wineserver_pid}/environ" 2> /dev/null || echo "")
 
         # Copy the required environment variables found in the
         # existing wineserver process
         for env_name in "${WINESERVER_ENV_VARS_TO_COPY[@]}"; do
             env_declr=$(echo "$wineserver_env_vars" | grep "^${env_name}=" || :)
             if [[ -n "$env_declr" ]]; then
                 log_info "Copying env var from running wineserver: ${env_declr}"
@@ -164,15 +167,15 @@
     # Use "pressure-vessel-launch" to launch it in the existing container.
 
     log_info "Starting Wine process using 'pressure-vessel-launch'"
 
     # It would be nicer to use the PID here, but that would break multiple
     # simultaneous Protontricks sessions inside Flatpak, which doesn't seem to
     # expose the unique host PID.
-    bus_name="com.github.Matoking.protontricks.App$STEAM_APPID-$PROTONTRICKS_SESSION_ID"
+    bus_name="com.github.Matoking.protontricks.App${STEAM_APPID}_${PROTONTRICKS_SESSION_ID}"
 
     # Wait until socket is created
     if ! dbus-send --print-reply --dest=org.freedesktop.DBus  /org/freedesktop/DBus org.freedesktop.DBus.ListNames | grep -q "$bus_name"; then
         log_info "bwrap-launcher D-Bus object not yet available, waiting..."
         while ! dbus-send --print-reply --dest=org.freedesktop.DBus  /org/freedesktop/DBus org.freedesktop.DBus.ListNames | grep -q "$bus_name"; do
             sleep 0.25
         done
```

### Comparing `protontricks-1.9.1/src/protontricks/data/scripts/wineserver_keepalive.bat` & `protontricks-1.9.2/src/protontricks/data/scripts/wineserver_keepalive.bat`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/data/scripts/wineserver_keepalive.sh` & `protontricks-1.9.2/src/protontricks/data/scripts/wineserver_keepalive.sh`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/flatpak.py` & `protontricks-1.9.2/src/protontricks/flatpak.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/gui.py` & `protontricks-1.9.2/src/protontricks/gui.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/steam.py` & `protontricks-1.9.2/src/protontricks/steam.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/util.py` & `protontricks-1.9.2/src/protontricks/util.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks/winetricks.py` & `protontricks-1.9.2/src/protontricks/winetricks.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/src/protontricks.egg-info/PKG-INFO` & `protontricks-1.9.2/src/protontricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protontricks
-Version: 1.9.1
+Version: 1.9.2
 Summary: A simple wrapper for running Winetricks commands for Proton-enabled games.
 Home-page: https://github.com/Matoking/protontricks
 Author: Janne Pulkkinen
 Author-email: janne.pulkkinen@protonmail.com
 License: GPL3
 Platform: linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -35,15 +35,15 @@
 
 # What is it?
 
 This is a wrapper script that allows you to easily run Winetricks commands for Steam Play/Proton games among other common Wine features, such as launching external Windows executables. This is often useful when a game requires closed-source runtime libraries or applications that are not included with Proton.
 
 # Requirements
 
-* Python 3.5 or newer
+* Python 3.6 or newer
 * Winetricks
 * Steam
 * YAD (recommended) **or** Zenity. Required for GUI.
 
 # Usage
 
 **Protontricks can be launched from desktop or using the `protontricks` command.**
@@ -212,9 +212,7 @@
 python3 -m pip install --user protontricks
 ```
 
 To install the latest development version (requires `git`):
 ```sh
 sudo python3 -m pip install git+https://github.com/Matoking/protontricks.git
 ```
-
-
```

### Comparing `protontricks-1.9.1/src/protontricks.egg-info/SOURCES.txt` & `protontricks-1.9.2/src/protontricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/cli/test_desktop_install.py` & `protontricks-1.9.2/tests/cli/test_desktop_install.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/cli/test_launch.py` & `protontricks-1.9.2/tests/cli/test_launch.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/cli/test_main.py` & `protontricks-1.9.2/tests/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/cli/test_util.py` & `protontricks-1.9.2/tests/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/conftest.py` & `protontricks-1.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/test_config.py` & `protontricks-1.9.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/test_flatpak.py` & `protontricks-1.9.2/tests/test_flatpak.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/test_gui.py` & `protontricks-1.9.2/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/test_steam.py` & `protontricks-1.9.2/tests/test_steam.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/test_util.py` & `protontricks-1.9.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `protontricks-1.9.1/tests/test_winetricks.py` & `protontricks-1.9.2/tests/test_winetricks.py`

 * *Files identical despite different names*

