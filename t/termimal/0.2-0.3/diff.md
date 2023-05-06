# Comparing `tmp/termimal-0.2.tar.gz` & `tmp/termimal-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termimal-0.2.tar", last modified: Sat May  6 19:32:47 2023, max compression
+gzip compressed data, was "termimal-0.3.tar", last modified: Sat May  6 19:48:45 2023, max compression
```

## Comparing `termimal-0.2.tar` & `termimal-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:32:47.244912 termimal-0.2/
--rw-rw-rw-   0        0        0      613 2023-05-06 19:32:47.236731 termimal-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-05-06 17:46:56.000000 termimal-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 19:32:47.244912 termimal-0.2/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-05-06 19:32:30.000000 termimal-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:32:47.236731 termimal-0.2/termimal.egg-info/
--rw-rw-rw-   0        0        0      613 2023-05-06 19:32:46.000000 termimal-0.2/termimal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-06 19:32:47.000000 termimal-0.2/termimal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:32:46.000000 termimal-0.2/termimal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 19:32:47.000000 termimal-0.2/termimal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:32:47.000000 termimal-0.2/termimal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 19:48:45.905989 termimal-0.3/
+-rw-rw-rw-   0        0        0      634 2023-05-06 19:48:45.905989 termimal-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-05-06 17:46:56.000000 termimal-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 19:48:45.905989 termimal-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      872 2023-05-06 19:48:21.000000 termimal-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:48:45.897783 termimal-0.3/termimal.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-05-06 19:48:45.000000 termimal-0.3/termimal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-06 19:48:45.000000 termimal-0.3/termimal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:48:45.000000 termimal-0.3/termimal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 19:48:45.000000 termimal-0.3/termimal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:48:45.000000 termimal-0.3/termimal.egg-info/top_level.txt
```

### Comparing `termimal-0.2/PKG-INFO` & `termimal-0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: termimal
-Version: 0.2
+Version: 0.3
 Summary: termimal simple
 Home-page: https://github.com/julianurielar/terminal.git
 Author: julian uriel weitzman
 Author-email: weijulian3@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+
+<h1>terminal</h1>
```

### Comparing `termimal-0.2/termimal.egg-info/PKG-INFO` & `termimal-0.3/termimal.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: termimal
-Version: 0.2
+Version: 0.3
 Summary: termimal simple
 Home-page: https://github.com/julianurielar/terminal.git
 Author: julian uriel weitzman
 Author-email: weijulian3@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+
+<h1>terminal</h1>
```

