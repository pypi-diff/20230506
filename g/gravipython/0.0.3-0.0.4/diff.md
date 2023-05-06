# Comparing `tmp/gravipython-0.0.3.tar.gz` & `tmp/gravipython-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravipython-0.0.3.tar", last modified: Fri May  5 14:15:43 2023, max compression
+gzip compressed data, was "gravipython-0.0.4.tar", last modified: Sat May  6 08:41:49 2023, max compression
```

## Comparing `gravipython-0.0.3.tar` & `gravipython-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:15:44.000000 gravipython-0.0.3/
--rw-rw-rw-   0        0        0     1721 2023-05-05 14:15:44.000000 gravipython-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1440 2023-05-05 13:55:16.000000 gravipython-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/
--rw-rw-rw-   0        0        0     1721 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/dependency_links.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/
--rw-rw-rw-   0        0        0     1680 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 14:05:34.000000 gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:15:44.000000 gravipython-0.0.3/gravipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1060 2023-05-02 13:51:28.000000 gravipython-0.0.3/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 14:15:44.000000 gravipython-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-05 14:15:32.000000 gravipython-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:41:50.000000 gravipython-0.0.4/
+-rw-rw-rw-   0        0        0     1721 2023-05-06 08:41:50.000000 gravipython-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2023-05-05 13:55:16.000000 gravipython-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 08:41:50.000000 gravipython-0.0.4/gravipython.egg-info/
+-rw-rw-rw-   0        0        0     1721 2023-05-06 08:41:50.000000 gravipython-0.0.4/gravipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-05-06 08:41:50.000000 gravipython-0.0.4/gravipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 08:41:50.000000 gravipython-0.0.4/gravipython.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 08:41:50.000000 gravipython-0.0.4/gravipython.egg-info/gravipython.egg-info/
+-rw-rw-rw-   0        0        0     1680 2023-05-05 14:05:34.000000 gravipython-0.0.4/gravipython.egg-info/gravipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-05 14:05:34.000000 gravipython-0.0.4/gravipython.egg-info/gravipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:05:34.000000 gravipython-0.0.4/gravipython.egg-info/gravipython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 14:05:34.000000 gravipython-0.0.4/gravipython.egg-info/gravipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 14:05:34.000000 gravipython-0.0.4/gravipython.egg-info/gravipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 08:41:50.000000 gravipython-0.0.4/gravipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 08:41:50.000000 gravipython-0.0.4/gravipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1060 2023-05-02 13:51:28.000000 gravipython-0.0.4/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 08:41:50.000000 gravipython-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      735 2023-05-06 08:41:42.000000 gravipython-0.0.4/setup.py
```

### Comparing `gravipython-0.0.3/PKG-INFO` & `gravipython-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravipython
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python module for simulating planets trajectories in 2D.
 Author: Tom Brandt
 Author-email: latomateultime@gmail.com
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `gravipython-0.0.3/README.md` & `gravipython-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gravipython-0.0.3/gravipython.egg-info/PKG-INFO` & `gravipython-0.0.4/gravipython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravipython
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python module for simulating planets trajectories in 2D.
 Author: Tom Brandt
 Author-email: latomateultime@gmail.com
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `gravipython-0.0.3/gravipython.egg-info/gravipython.egg-info/PKG-INFO` & `gravipython-0.0.4/gravipython.egg-info/gravipython.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `gravipython-0.0.3/license.txt` & `gravipython-0.0.4/license.txt`

 * *Files identical despite different names*

### Comparing `gravipython-0.0.3/setup.py` & `gravipython-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as descfile:
     longdesc = descfile.read()
 
 setuptools.setup(name="gravipython",
-                 version="0.0.3",
+                 version="0.0.4",
                  author="Tom Brandt",
                  author_email="latomateultime@gmail.com",
                  description="A python module for simulating planets trajectories in 2D.",
                  long_description_content_type="text/markdown",
                  long_description=longdesc,
                  license="MIT license",
-                 packages=setuptools.find_packages("gravitypython"),
+                 packages=setuptools.find_packages("gravipython"),
 #                  package_dir={'': "gravitypython"},
                  install_requires=["pygame", "numpy"],
                  include_package_data = True)
```

