# Comparing `tmp/smartjs-0.0.4.tar.gz` & `tmp/smartjs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.0.4.tar", max compression
+gzip compressed data, was "smartjs-0.0.5.tar", max compression
```

## Comparing `smartjs-0.0.4.tar` & `smartjs-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      302 2023-05-06 00:35:38.338532 smartjs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.0.4/smartjs/__init__.py
--rw-r--r--   0        0        0    13325 2023-05-06 00:12:29.975202 smartjs-0.0.4/smartjs/base.py
--rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.0.4/smartjs/constants.py
--rw-r--r--   0        0        0     4479 2023-05-04 15:42:17.533986 smartjs-0.0.4/smartjs/elements.py
--rw-r--r--   0        0        0     5801 2023-05-04 01:36:29.647942 smartjs-0.0.4/smartjs/functions.py
--rw-r--r--   0        0        0    13961 2023-05-06 00:12:29.971024 smartjs-0.0.4/smartjs/javascript.py
--rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.0.4/smartjs/page.py
--rw-r--r--   0        0        0      807 2023-05-05 22:30:55.828371 smartjs-0.0.4/smartjs/path.py
--rw-r--r--   0        0        0     1598 2023-05-05 03:48:44.383638 smartjs-0.0.4/smartjs/style.py
--rw-r--r--   0        0        0      584 2023-05-06 00:35:42.461233 smartjs-0.0.4/setup.py
--rw-r--r--   0        0        0      333 2023-05-06 00:35:42.461458 smartjs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      302 2023-05-06 00:22:13.174930 smartjs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.0.5/smartjs/__init__.py
+-rw-r--r--   0        0        0    13325 2023-05-06 00:12:29.975202 smartjs-0.0.5/smartjs/base.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.0.5/smartjs/constants.py
+-rw-r--r--   0        0        0     4479 2023-05-04 15:42:17.533986 smartjs-0.0.5/smartjs/elements.py
+-rw-r--r--   0        0        0     5801 2023-05-04 01:36:29.647942 smartjs-0.0.5/smartjs/functions.py
+-rw-r--r--   0        0        0    13961 2023-05-06 00:12:29.971024 smartjs-0.0.5/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.0.5/smartjs/page.py
+-rw-r--r--   0        0        0      807 2023-05-05 22:30:55.828371 smartjs-0.0.5/smartjs/path.py
+-rw-r--r--   0        0        0     1598 2023-05-05 03:48:44.383638 smartjs-0.0.5/smartjs/style.py
+-rw-r--r--   0        0        0      584 2023-05-06 00:22:19.733975 smartjs-0.0.5/setup.py
+-rw-r--r--   0        0        0      333 2023-05-06 00:22:19.734213 smartjs-0.0.5/PKG-INFO
```

### Comparing `smartjs-0.0.4/smartjs/base.py` & `smartjs-0.0.5/smartjs/base.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.4/smartjs/constants.py` & `smartjs-0.0.5/smartjs/constants.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.4/smartjs/elements.py` & `smartjs-0.0.5/smartjs/elements.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.4/smartjs/functions.py` & `smartjs-0.0.5/smartjs/functions.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.4/smartjs/javascript.py` & `smartjs-0.0.5/smartjs/javascript.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.4/smartjs/page.py` & `smartjs-0.0.5/smartjs/page.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.4/smartjs/path.py` & `smartjs-0.0.5/smartjs/path.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.4/smartjs/style.py` & `smartjs-0.0.5/smartjs/style.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.4/setup.py` & `smartjs-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': '',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

