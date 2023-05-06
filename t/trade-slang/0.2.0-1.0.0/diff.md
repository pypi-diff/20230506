# Comparing `tmp/trade_slang-0.2.0.tar.gz` & `tmp/trade_slang-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trade_slang-0.2.0.tar", max compression
+gzip compressed data, was "trade_slang-1.0.0.tar", max compression
```

## Comparing `trade_slang-0.2.0.tar` & `trade_slang-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34523 2023-05-05 23:46:04.000000 trade_slang-0.2.0/LICENSE
--rw-r--r--   0        0        0       22 2023-05-06 06:58:52.937649 trade_slang-0.2.0/README.md
--rw-r--r--   0        0        0      388 2023-05-06 07:02:49.842132 trade_slang-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 06:52:07.902358 trade_slang-0.2.0/slang/__init__.py
--rw-r--r--   0        0        0       64 2023-05-06 06:58:10.506490 trade_slang-0.2.0/slang/__main__.py
--rw-r--r--   0        0        0     1232 2023-05-06 07:02:49.838562 trade_slang-0.2.0/slang/cli.py
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 trade_slang-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-05 23:46:04.000000 trade_slang-1.0.0/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-06 06:58:52.937649 trade_slang-1.0.0/README.md
+-rw-r--r--   0        0        0      388 2023-05-06 07:05:58.254423 trade_slang-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-06 06:52:07.902358 trade_slang-1.0.0/slang/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-06 06:58:10.506490 trade_slang-1.0.0/slang/__main__.py
+-rw-r--r--   0        0        0     1232 2023-05-06 07:02:49.838562 trade_slang-1.0.0/slang/cli.py
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 trade_slang-1.0.0/PKG-INFO
```

### Comparing `trade_slang-0.2.0/LICENSE` & `trade_slang-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trade_slang-0.2.0/slang/cli.py` & `trade_slang-1.0.0/slang/cli.py`

 * *Files identical despite different names*

