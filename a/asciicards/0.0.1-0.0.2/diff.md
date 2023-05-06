# Comparing `tmp/asciicards-0.0.1.tar.gz` & `tmp/asciicards-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciicards-0.0.1.tar", last modified: Sat May  6 18:31:54 2023, max compression
+gzip compressed data, was "asciicards-0.0.2.tar", last modified: Sat May  6 21:02:47 2023, max compression
```

## Comparing `asciicards-0.0.1.tar` & `asciicards-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:31:54.060391 asciicards-0.0.1/
--rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      495 2023-05-06 18:31:54.059390 asciicards-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 18:31:54.058390 asciicards-0.0.1/asciicards.egg-info/
--rw-rw-rw-   0        0        0      495 2023-05-06 18:31:54.000000 asciicards-0.0.1/asciicards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-06 18:31:54.000000 asciicards-0.0.1/asciicards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:31:54.000000 asciicards-0.0.1/asciicards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:31:54.000000 asciicards-0.0.1/asciicards.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-05-06 18:24:32.000000 asciicards-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 18:31:54.060391 asciicards-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      489 2023-05-06 18:31:41.000000 asciicards-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:02:47.876139 asciicards-0.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      495 2023-05-06 21:02:47.876139 asciicards-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 21:02:47.874137 asciicards-0.0.2/asciicards.egg-info/
+-rw-rw-rw-   0        0        0      495 2023-05-06 21:02:47.000000 asciicards-0.0.2/asciicards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-06 21:02:47.000000 asciicards-0.0.2/asciicards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 21:02:47.000000 asciicards-0.0.2/asciicards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 21:02:47.000000 asciicards-0.0.2/asciicards.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-05-06 18:24:32.000000 asciicards-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 21:02:47.876139 asciicards-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      489 2023-05-06 21:02:27.000000 asciicards-0.0.2/setup.py
```

### Comparing `asciicards-0.0.1/LICENSE` & `asciicards-0.0.2/LICENSE`

 * *Files identical despite different names*

