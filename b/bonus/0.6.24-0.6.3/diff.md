# Comparing `tmp/bonus-0.6.24.tar.gz` & `tmp/bonus-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Serega\Downloads\bonus-0.6.21\bonus-0.6.21\dist\.tmp-moe915gm\bonus-0.6.24.tar", last modified: Sat May  6 09:03:43 2023, max compression
+gzip compressed data, was "bonus-0.6.3.tar", last modified: Sat Dec 17 20:14:41 2022, max compression
```

## Comparing `bonus-0.6.24.tar` & `bonus-0.6.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 09:03:43.000000 bonus-0.6.24/
--rw-rw-rw-   0        0        0      123 2023-05-06 09:03:43.000000 bonus-0.6.24/PKG-INFO
--rw-rw-rw-   0        0        0      196 2020-07-15 06:42:11.000000 bonus-0.6.24/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 09:03:43.000000 bonus-0.6.24/bonus/
--rw-rw-rw-   0        0        0     8887 2023-05-06 09:02:56.000000 bonus-0.6.24/bonus/bonus.py
-drwxrwxrwx   0        0        0        0 2023-05-06 09:03:43.000000 bonus-0.6.24/bonus.egg-info/
--rw-rw-rw-   0        0        0      123 2023-05-06 09:03:43.000000 bonus-0.6.24/bonus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-05-06 09:03:43.000000 bonus-0.6.24/bonus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 09:03:43.000000 bonus-0.6.24/bonus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 09:03:43.000000 bonus-0.6.24/bonus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 09:03:43.000000 bonus-0.6.24/setup.cfg
--rw-rw-rw-   0        0        0      212 2023-05-06 09:02:24.000000 bonus-0.6.24/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-17 20:14:41.417698 bonus-0.6.3/
+-rw-rw-rw-   0        0        0      122 2022-12-17 20:14:41.418698 bonus-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2020-07-15 06:42:11.000000 bonus-0.6.3/README.rst
+drwxrwxrwx   0        0        0        0 2022-12-17 20:14:41.374696 bonus-0.6.3/bonus/
+-rw-rw-rw-   0        0        0     2943 2022-12-17 20:13:32.000000 bonus-0.6.3/bonus/bonus.py
+drwxrwxrwx   0        0        0        0 2022-12-17 20:14:41.412697 bonus-0.6.3/bonus.egg-info/
+-rw-rw-rw-   0        0        0      122 2022-12-17 20:14:41.000000 bonus-0.6.3/bonus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2022-12-17 20:14:41.000000 bonus-0.6.3/bonus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-17 20:14:41.000000 bonus-0.6.3/bonus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2022-12-17 20:14:41.000000 bonus-0.6.3/bonus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-12-17 20:14:41.419697 bonus-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      211 2022-12-17 20:14:02.000000 bonus-0.6.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

