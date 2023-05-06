# Comparing `tmp/txdtaiac-1.0.tar.gz` & `tmp/txdtaiac-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txdtaiac-1.0.tar", last modified: Sat May  6 03:46:42 2023, max compression
+gzip compressed data, was "txdtaiac-2.0.tar", last modified: Sat May  6 04:07:46 2023, max compression
```

## Comparing `txdtaiac-1.0.tar` & `txdtaiac-2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:46:42.664958 txdtaiac-1.0/
--rw-rw-rw-   0        0        0      192 2023-05-06 03:46:42.664958 txdtaiac-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-06 03:41:59.068551 txdtaiac-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:46:42.664958 txdtaiac-1.0/txdtaiac/
--rw-rw-rw-   0        0        0       46 2023-05-06 03:45:54.422536 txdtaiac-1.0/txdtaiac/__init__.py
--rw-rw-rw-   0        0        0     1338 2023-05-06 03:35:32.136393 txdtaiac-1.0/txdtaiac/taiac.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:07:46.704856 txdtaiac-2.0/
+-rw-rw-rw-   0        0        0      192 2023-05-06 04:07:46.704856 txdtaiac-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-06 04:05:32.038316 txdtaiac-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:07:46.704856 txdtaiac-2.0/txdtaiac/
+-rw-rw-rw-   0        0        0       47 2023-05-06 04:01:54.078074 txdtaiac-2.0/txdtaiac/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-05-06 03:35:32.136393 txdtaiac-2.0/txdtaiac/taiac.py
```

### Comparing `txdtaiac-1.0/txdtaiac/taiac.py` & `txdtaiac-2.0/txdtaiac/taiac.py`

 * *Files identical despite different names*

