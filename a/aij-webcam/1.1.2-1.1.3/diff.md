# Comparing `tmp/aij-webcam-1.1.2.tar.gz` & `tmp/aij-webcam-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.1.2.tar", last modified: Fri May  5 13:14:29 2023, max compression
+gzip compressed data, was "aij-webcam-1.1.3.tar", last modified: Sat May  6 19:27:30 2023, max compression
```

## Comparing `aij-webcam-1.1.2.tar` & `aij-webcam-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/
--rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.2/README.md
--rw-rw-rw-   0        0        0     6368 2023-05-05 13:14:18.000000 aij-webcam-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      175 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/news/
--rw-rw-rw-   0        0        0      567 2023-05-05 12:40:48.000000 aij-webcam-1.1.2/src/news/__init__.py
--rw-rw-rw-   0        0        0     4490 2023-05-05 12:35:58.000000 aij-webcam-1.1.2/src/news/core.py
--rw-rw-rw-   0        0        0     3663 2023-05-05 12:51:30.000000 aij-webcam-1.1.2/src/news/publisher.py
--rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-webcam-1.1.2/src/news/subscriber.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/webcam/
--rw-rw-rw-   0        0        0    17500 2023-05-05 13:14:12.000000 aij-webcam-1.1.2/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/
+-rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.3/README.md
+-rw-rw-rw-   0        0        0     6368 2023-05-06 19:27:10.000000 aij-webcam-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      175 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/news/
+-rw-rw-rw-   0        0        0      567 2023-05-05 12:40:48.000000 aij-webcam-1.1.3/src/news/__init__.py
+-rw-rw-rw-   0        0        0     4490 2023-05-05 12:35:58.000000 aij-webcam-1.1.3/src/news/core.py
+-rw-rw-rw-   0        0        0     3663 2023-05-05 12:51:30.000000 aij-webcam-1.1.3/src/news/publisher.py
+-rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-webcam-1.1.3/src/news/subscriber.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/webcam/
+-rw-rw-rw-   0        0        0    17500 2023-05-05 13:14:12.000000 aij-webcam-1.1.3/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.1.2/LICENSE.txt` & `aij-webcam-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.2/PKG-INFO` & `aij-webcam-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.1.2
+Version: 1.1.3
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.1.2/README.md` & `aij-webcam-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.2/pyproject.toml` & `aij-webcam-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.2"
+version = "1.1.3"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-webcam-1.1.2/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.1.3/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.1.2
+Version: 1.1.3
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.1.2/src/news/__init__.py` & `aij-webcam-1.1.3/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.2/src/news/core.py` & `aij-webcam-1.1.3/src/news/core.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.2/src/news/publisher.py` & `aij-webcam-1.1.3/src/news/publisher.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.2/src/news/subscriber.py` & `aij-webcam-1.1.3/src/news/subscriber.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.2/src/webcam/__init__.py` & `aij-webcam-1.1.3/src/webcam/__init__.py`

 * *Files identical despite different names*

