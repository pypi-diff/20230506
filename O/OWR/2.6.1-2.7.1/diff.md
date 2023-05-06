# Comparing `tmp/OWR-2.6.1.tar.gz` & `tmp/OWR-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.6.1.tar", last modified: Thu May  4 14:18:29 2023, max compression
+gzip compressed data, was "OWR-2.7.1.tar", last modified: Sat May  6 07:22:37 2023, max compression
```

## Comparing `OWR-2.6.1.tar` & `OWR-2.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:18:29.320929 OWR-2.6.1/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.6.1/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:18:29.316929 OWR-2.6.1/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     8319 2023-05-04 14:14:15.000000 OWR-2.6.1/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:18:29.316929 OWR-2.6.1/OWR/data/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     5788 2023-05-04 14:14:15.000000 OWR-2.6.1/OWR/data/obscenity_words.json
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:18:29.316929 OWR-2.6.1/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 14:18:29.316929 OWR-2.6.1/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-04 14:14:15.000000 OWR-2.6.1/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-04 14:18:29.320929 OWR-2.6.1/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      747 2023-05-04 14:18:13.000000 OWR-2.6.1/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 07:22:37.335755 OWR-2.7.1/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.7.1/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 07:22:37.335755 OWR-2.7.1/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    15092 2023-05-06 07:20:26.000000 OWR-2.7.1/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 07:22:37.335755 OWR-2.7.1/OWR/data/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     5788 2023-05-06 07:20:17.000000 OWR-2.7.1/OWR/data/obscenity_words.json
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-06 07:22:37.335755 OWR-2.7.1/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-06 07:22:37.000000 OWR-2.7.1/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-06 07:22:37.335755 OWR-2.7.1/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-06 07:20:17.000000 OWR-2.7.1/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-06 07:22:37.335755 OWR-2.7.1/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      747 2023-05-06 07:22:26.000000 OWR-2.7.1/setup.py
```

### Comparing `OWR-2.6.1/LICENSE` & `OWR-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.6.1/OWR/data/obscenity_words.json` & `OWR-2.7.1/OWR/data/obscenity_words.json`

 * *Files identical despite different names*

### Comparing `OWR-2.6.1/setup.py` & `OWR-2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='2.6.1',
+    version='2.7.1',
     description='Obscene word recognition package',
     url='https://github.com/RuslanGaliullin/FFixTelegramBot/tree/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
     package_data={'': ['data/obscenity_words.json']},
```

