# Comparing `tmp/masonite-ready_auth-0.0.1.tar.gz` & `tmp/masonite-ready_auth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masonite-ready_auth-0.0.1.tar", last modified: Sat May  6 09:36:24 2023, max compression
+gzip compressed data, was "masonite-ready_auth-0.0.2.tar", last modified: Sat May  6 09:51:23 2023, max compression
```

## Comparing `masonite-ready_auth-0.0.1.tar` & `masonite-ready_auth-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:36:24.247367 masonite-ready_auth-0.0.1/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.1/LICENSE
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.1/MANIFEST.in
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 09:36:24.247367 masonite-ready_auth-0.0.1/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4372 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.1/README.md
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.1/pyproject.toml
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-06 09:36:24.247367 masonite-ready_auth-0.0.1/setup.cfg
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3582 2023-05-06 09:36:20.000000 masonite-ready_auth-0.0.1/setup.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:36:24.243366 masonite-ready_auth-0.0.1/src/
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:36:24.243366 masonite-ready_auth-0.0.1/src/masonite_ready_auth.egg-info/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 09:36:24.000000 masonite-ready_auth-0.0.1/src/masonite_ready_auth.egg-info/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      443 2023-05-06 09:36:24.000000 masonite-ready_auth-0.0.1/src/masonite_ready_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-06 09:36:24.000000 masonite-ready_auth-0.0.1/src/masonite_ready_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-06 09:36:24.000000 masonite-ready_auth-0.0.1/src/masonite_ready_auth.egg-info/requires.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       11 2023-05-06 09:36:24.000000 masonite-ready_auth-0.0.1/src/masonite_ready_auth.egg-info/top_level.txt
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:36:24.243366 masonite-ready_auth-0.0.1/src/ready_auth/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       79 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.1/src/ready_auth/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:36:24.247367 masonite-ready_auth-0.0.1/src/ready_auth/config/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      273 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.1/src/ready_auth/config/ready_auth.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:36:24.247367 masonite-ready_auth-0.0.1/src/ready_auth/providers/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1581 2023-05-06 09:21:02.000000 masonite-ready_auth-0.0.1/src/ready_auth/providers/ReadyAuthProvider.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.1/src/ready_auth/providers/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:51:23.219249 masonite-ready_auth-0.0.2/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.2/LICENSE
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.2/MANIFEST.in
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 09:51:23.219249 masonite-ready_auth-0.0.2/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4372 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.2/README.md
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.2/pyproject.toml
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-06 09:51:23.219249 masonite-ready_auth-0.0.2/setup.cfg
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3582 2023-05-06 09:43:28.000000 masonite-ready_auth-0.0.2/setup.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:51:23.215249 masonite-ready_auth-0.0.2/src/
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:51:23.219249 masonite-ready_auth-0.0.2/src/masonite_ready_auth.egg-info/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 09:51:23.000000 masonite-ready_auth-0.0.2/src/masonite_ready_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      443 2023-05-06 09:51:23.000000 masonite-ready_auth-0.0.2/src/masonite_ready_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-06 09:51:23.000000 masonite-ready_auth-0.0.2/src/masonite_ready_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-06 09:51:23.000000 masonite-ready_auth-0.0.2/src/masonite_ready_auth.egg-info/requires.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       11 2023-05-06 09:51:23.000000 masonite-ready_auth-0.0.2/src/masonite_ready_auth.egg-info/top_level.txt
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:51:23.219249 masonite-ready_auth-0.0.2/src/ready_auth/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       79 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.2/src/ready_auth/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:51:23.219249 masonite-ready_auth-0.0.2/src/ready_auth/config/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      273 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.2/src/ready_auth/config/ready_auth.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:51:23.219249 masonite-ready_auth-0.0.2/src/ready_auth/providers/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1320 2023-05-06 09:41:47.000000 masonite-ready_auth-0.0.2/src/ready_auth/providers/ReadyAuthProvider.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.2/src/ready_auth/providers/__init__.py
```

### Comparing `masonite-ready_auth-0.0.1/LICENSE` & `masonite-ready_auth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `masonite-ready_auth-0.0.1/PKG-INFO` & `masonite-ready_auth-0.0.2/src/masonite_ready_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: masonite-ready_auth
-Version: 0.0.1
+Name: masonite-ready-auth
+Version: 0.0.2
 Summary: Custom authentication module for Masonite 4.
 Home-page: https://github.com/lvjhn/masonite-ready_auth
 Author: LJ S.A.
 Author-email: lvjhn.mx@gmail.com
 License: MIT license
 Keywords: Masonite,Python,Development
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masonite-ready_auth Version: 0.0.1 Summary: Custom
+Metadata-Version: 2.1 Name: masonite-ready-auth Version: 0.0.2 Summary: Custom
 authentication module for Masonite 4. Home-page: https://github.com/lvjhn/
 masonite-ready_auth Author: LJ S.A. Author-email: lvjhn.mx@gmail.com License:
 MIT license Keywords: Masonite,Python,Development Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Environment :: Web Environment Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

### Comparing `masonite-ready_auth-0.0.1/README.md` & `masonite-ready_auth-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `masonite-ready_auth-0.0.1/setup.py` & `masonite-ready_auth-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="masonite-ready_auth",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.1",
+    version="0.0.2",
     packages=[
         "ready_auth",
         "ready_auth.providers",
         "ready_auth.config",
     ],
     package_dir={"": "src"},
     description="Custom authentication module for Masonite 4.",
```

### Comparing `masonite-ready_auth-0.0.1/src/masonite_ready_auth.egg-info/PKG-INFO` & `masonite-ready_auth-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: masonite-ready-auth
-Version: 0.0.1
+Name: masonite-ready_auth
+Version: 0.0.2
 Summary: Custom authentication module for Masonite 4.
 Home-page: https://github.com/lvjhn/masonite-ready_auth
 Author: LJ S.A.
 Author-email: lvjhn.mx@gmail.com
 License: MIT license
 Keywords: Masonite,Python,Development
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masonite-ready-auth Version: 0.0.1 Summary: Custom
+Metadata-Version: 2.1 Name: masonite-ready_auth Version: 0.0.2 Summary: Custom
 authentication module for Masonite 4. Home-page: https://github.com/lvjhn/
 masonite-ready_auth Author: LJ S.A. Author-email: lvjhn.mx@gmail.com License:
 MIT license Keywords: Masonite,Python,Development Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Environment :: Web Environment Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

