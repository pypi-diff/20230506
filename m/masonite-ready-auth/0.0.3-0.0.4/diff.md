# Comparing `tmp/masonite-ready_auth-0.0.3.tar.gz` & `tmp/masonite-ready_auth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masonite-ready_auth-0.0.3.tar", last modified: Sat May  6 09:56:38 2023, max compression
+gzip compressed data, was "masonite-ready_auth-0.0.4.tar", last modified: Sat May  6 10:14:00 2023, max compression
```

## Comparing `masonite-ready_auth-0.0.3.tar` & `masonite-ready_auth-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:56:38.841710 masonite-ready_auth-0.0.3/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.3/LICENSE
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.3/MANIFEST.in
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 09:56:38.841710 masonite-ready_auth-0.0.3/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4372 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.3/README.md
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.3/pyproject.toml
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-06 09:56:38.845710 masonite-ready_auth-0.0.3/setup.cfg
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3582 2023-05-06 09:56:17.000000 masonite-ready_auth-0.0.3/setup.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:56:38.837710 masonite-ready_auth-0.0.3/src/
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:56:38.841710 masonite-ready_auth-0.0.3/src/masonite_ready_auth.egg-info/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 09:56:38.000000 masonite-ready_auth-0.0.3/src/masonite_ready_auth.egg-info/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      443 2023-05-06 09:56:38.000000 masonite-ready_auth-0.0.3/src/masonite_ready_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-06 09:56:38.000000 masonite-ready_auth-0.0.3/src/masonite_ready_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-06 09:56:38.000000 masonite-ready_auth-0.0.3/src/masonite_ready_auth.egg-info/requires.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       11 2023-05-06 09:56:38.000000 masonite-ready_auth-0.0.3/src/masonite_ready_auth.egg-info/top_level.txt
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:56:38.841710 masonite-ready_auth-0.0.3/src/ready_auth/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       79 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.3/src/ready_auth/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:56:38.841710 masonite-ready_auth-0.0.3/src/ready_auth/config/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      273 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.3/src/ready_auth/config/ready_auth.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:56:38.841710 masonite-ready_auth-0.0.3/src/ready_auth/providers/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1401 2023-05-06 09:56:11.000000 masonite-ready_auth-0.0.3/src/ready_auth/providers/ReadyAuthProvider.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.3/src/ready_auth/providers/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:14:00.521766 masonite-ready_auth-0.0.4/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.4/LICENSE
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.4/MANIFEST.in
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 10:14:00.521766 masonite-ready_auth-0.0.4/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4372 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.4/README.md
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.4/pyproject.toml
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-06 10:14:00.521766 masonite-ready_auth-0.0.4/setup.cfg
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3582 2023-05-06 10:13:45.000000 masonite-ready_auth-0.0.4/setup.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:14:00.517766 masonite-ready_auth-0.0.4/src/
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:14:00.517766 masonite-ready_auth-0.0.4/src/masonite_ready_auth.egg-info/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 10:14:00.000000 masonite-ready_auth-0.0.4/src/masonite_ready_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      443 2023-05-06 10:14:00.000000 masonite-ready_auth-0.0.4/src/masonite_ready_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-06 10:14:00.000000 masonite-ready_auth-0.0.4/src/masonite_ready_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-06 10:14:00.000000 masonite-ready_auth-0.0.4/src/masonite_ready_auth.egg-info/requires.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       11 2023-05-06 10:14:00.000000 masonite-ready_auth-0.0.4/src/masonite_ready_auth.egg-info/top_level.txt
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:14:00.517766 masonite-ready_auth-0.0.4/src/ready_auth/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       79 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.4/src/ready_auth/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:14:00.517766 masonite-ready_auth-0.0.4/src/ready_auth/config/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      273 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.4/src/ready_auth/config/ready_auth.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:14:00.517766 masonite-ready_auth-0.0.4/src/ready_auth/providers/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1401 2023-05-06 10:05:31.000000 masonite-ready_auth-0.0.4/src/ready_auth/providers/ReadyAuthProvider.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.4/src/ready_auth/providers/__init__.py
```

### Comparing `masonite-ready_auth-0.0.3/LICENSE` & `masonite-ready_auth-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `masonite-ready_auth-0.0.3/PKG-INFO` & `masonite-ready_auth-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-ready_auth
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: masonite-ready_auth Version: 0.0.3 Summary: Custom
+Metadata-Version: 2.1 Name: masonite-ready_auth Version: 0.0.4 Summary: Custom
 authentication module for Masonite 4. Home-page: https://github.com/lvjhn/
 masonite-ready_auth Author: LJ S.A. Author-email: lvjhn.mx@gmail.com License:
 MIT license Keywords: Masonite,Python,Development Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Environment :: Web Environment Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

### Comparing `masonite-ready_auth-0.0.3/README.md` & `masonite-ready_auth-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `masonite-ready_auth-0.0.3/setup.py` & `masonite-ready_auth-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="masonite-ready_auth",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.3",
+    version="0.0.4",
     packages=[
         "ready_auth",
         "ready_auth.providers",
         "ready_auth.config",
     ],
     package_dir={"": "src"},
     description="Custom authentication module for Masonite 4.",
```

### Comparing `masonite-ready_auth-0.0.3/src/masonite_ready_auth.egg-info/PKG-INFO` & `masonite-ready_auth-0.0.4/src/masonite_ready_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-ready-auth
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: masonite-ready-auth Version: 0.0.3 Summary: Custom
+Metadata-Version: 2.1 Name: masonite-ready-auth Version: 0.0.4 Summary: Custom
 authentication module for Masonite 4. Home-page: https://github.com/lvjhn/
 masonite-ready_auth Author: LJ S.A. Author-email: lvjhn.mx@gmail.com License:
 MIT license Keywords: Masonite,Python,Development Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Environment :: Web Environment Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

### Comparing `masonite-ready_auth-0.0.3/src/ready_auth/providers/ReadyAuthProvider.py` & `masonite-ready_auth-0.0.4/src/ready_auth/providers/ReadyAuthProvider.py`

 * *Files identical despite different names*

