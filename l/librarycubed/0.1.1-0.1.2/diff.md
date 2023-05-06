# Comparing `tmp/librarycubed-0.1.1.tar.gz` & `tmp/librarycubed-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librarycubed-0.1.1.tar", max compression
+gzip compressed data, was "librarycubed-0.1.2.tar", max compression
```

## Comparing `librarycubed-0.1.1.tar` & `librarycubed-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       48 2023-05-06 16:02:00.962200 librarycubed-0.1.1/librarycubed/__init__.py
--rw-r--r--   0        0        0     1093 2023-05-06 00:35:20.056921 librarycubed-0.1.1/LICENSE
--rw-r--r--   0        0        0      290 2023-05-06 14:41:10.751487 librarycubed-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 00:25:33.411930 librarycubed-0.1.1/README.md
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 librarycubed-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      426 2023-05-06 21:17:17.103650 librarycubed-0.1.2/librarycubed/__init__.py
+-rw-r--r--   0        0        0     8192 2023-05-06 21:09:55.967259 librarycubed-0.1.2/librarycubed/blockchain.db
+-rw-r--r--   0        0        0     1093 2023-05-06 00:35:20.056921 librarycubed-0.1.2/LICENSE
+-rw-r--r--   0        0        0      291 2023-05-06 21:34:08.813315 librarycubed-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-06 21:29:17.237050 librarycubed-0.1.2/README.rst
+-rw-r--r--   0        0        0      313 1970-01-01 00:00:00.000000 librarycubed-0.1.2/PKG-INFO
```

### Comparing `librarycubed-0.1.1/LICENSE` & `librarycubed-0.1.2/LICENSE`

 * *Files identical despite different names*

