# Comparing `tmp/aiontutil-0.0.1.tar.gz` & `tmp/aiontutil-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiontutil-0.0.1.tar", max compression
+gzip compressed data, was "aiontutil-0.1.1.tar", max compression
```

## Comparing `aiontutil-0.0.1.tar` & `aiontutil-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-06 08:20:41.951559 aiontutil-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-06 08:20:41.951559 aiontutil-0.0.1/aiontutil/__init__.py
--rw-r--r--   0        0        0      698 2023-05-06 08:26:24.711560 aiontutil-0.0.1/aiontutil/signal.py
--rw-r--r--   0        0        0      316 2023-05-06 09:06:15.411559 aiontutil-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 aiontutil-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 08:20:41.951559 aiontutil-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 08:20:41.951559 aiontutil-0.1.1/aiontutil/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-06 08:26:24.711560 aiontutil-0.1.1/aiontutil/signal.py
+-rw-r--r--   0        0        0      333 2023-05-06 08:52:02.431559 aiontutil-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 aiontutil-0.1.1/PKG-INFO
```

### Comparing `aiontutil-0.0.1/aiontutil/signal.py` & `aiontutil-0.1.1/aiontutil/signal.py`

 * *Files identical despite different names*

