# Comparing `tmp/aixlab.cn-0.1.tar.gz` & `tmp/aixlab.cn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixlab.cn-0.1.tar", last modified: Sat Apr 29 02:37:50 2023, max compression
+gzip compressed data, was "aixlab.cn-0.1.1.tar", last modified: Sat May  6 03:25:20 2023, max compression
```

## Comparing `aixlab.cn-0.1.tar` & `aixlab.cn-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 02:37:50.933606 aixlab.cn-0.1/
--rw-rw-rw-   0        0        0      199 2023-04-29 02:37:50.932605 aixlab.cn-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 02:37:50.931609 aixlab.cn-0.1/aixlab.cn.egg-info/
--rw-rw-rw-   0        0        0      199 2023-04-29 02:37:50.000000 aixlab.cn-0.1/aixlab.cn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-29 02:37:50.000000 aixlab.cn-0.1/aixlab.cn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 02:37:50.000000 aixlab.cn-0.1/aixlab.cn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-29 02:37:50.000000 aixlab.cn-0.1/aixlab.cn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 02:37:50.000000 aixlab.cn-0.1/aixlab.cn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 02:37:50.933606 aixlab.cn-0.1/setup.cfg
--rw-rw-rw-   0        0        0      395 2023-04-29 02:37:04.000000 aixlab.cn-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:25:20.320842 aixlab.cn-0.1.1/
+-rw-rw-rw-   0        0        0      201 2023-05-06 03:25:20.319849 aixlab.cn-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 03:25:20.319849 aixlab.cn-0.1.1/aixlab.cn.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 03:25:20.320842 aixlab.cn-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      529 2023-05-06 03:25:08.000000 aixlab.cn-0.1.1/setup.py
```

