# Comparing `tmp/masonite-ready_auth-0.0.6.tar.gz` & `tmp/masonite-ready_auth-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masonite-ready_auth-0.0.6.tar", last modified: Sat May  6 10:42:46 2023, max compression
+gzip compressed data, was "masonite-ready_auth-0.0.7.tar", last modified: Sat May  6 10:46:13 2023, max compression
```

## Comparing `masonite-ready_auth-0.0.6.tar` & `masonite-ready_auth-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:42:45.999053 masonite-ready_auth-0.0.6/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.6/LICENSE
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.6/MANIFEST.in
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 10:42:45.999053 masonite-ready_auth-0.0.6/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4372 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.6/README.md
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.6/pyproject.toml
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-06 10:42:46.003053 masonite-ready_auth-0.0.6/setup.cfg
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3655 2023-05-06 10:42:44.000000 masonite-ready_auth-0.0.6/setup.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:42:45.995053 masonite-ready_auth-0.0.6/src/
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:42:45.999053 masonite-ready_auth-0.0.6/src/masonite_ready_auth.egg-info/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 10:42:45.000000 masonite-ready_auth-0.0.6/src/masonite_ready_auth.egg-info/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1184 2023-05-06 10:42:45.000000 masonite-ready_auth-0.0.6/src/masonite_ready_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-06 10:42:45.000000 masonite-ready_auth-0.0.6/src/masonite_ready_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-06 10:42:45.000000 masonite-ready_auth-0.0.6/src/masonite_ready_auth.egg-info/requires.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       11 2023-05-06 10:42:45.000000 masonite-ready_auth-0.0.6/src/masonite_ready_auth.egg-info/top_level.txt
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:42:45.999053 masonite-ready_auth-0.0.6/src/ready_auth/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       79 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.6/src/ready_auth/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:42:45.999053 masonite-ready_auth-0.0.6/src/ready_auth/config/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      273 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.6/src/ready_auth/config/ready_auth.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:42:45.995053 masonite-ready_auth-0.0.6/src/ready_auth/database/
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:42:45.999053 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      434 2023-05-06 09:21:10.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171516_drop_conflicting_tables.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      441 2023-05-06 09:17:13.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171713_create_ip_addresses_table.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      437 2023-05-06 09:17:21.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171721_create_user_agents_table.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      437 2023-05-06 09:17:26.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171726_create_auth_tokens_table.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      437 2023-05-06 09:17:31.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171731_create_user_tokens_table.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      415 2023-05-06 09:17:37.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171737_create_users_table.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      445 2023-05-06 09:18:04.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171804_create_user_sessions_table.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      457 2023-05-06 09:18:21.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171821_create_access_locations_table.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      479 2023-05-06 09:18:59.000000 masonite-ready_auth-0.0.6/src/ready_auth/database/migrations/2023_05_06_171859_create_personal_access_tokens_table.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:42:45.999053 masonite-ready_auth-0.0.6/src/ready_auth/providers/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1401 2023-05-06 10:05:31.000000 masonite-ready_auth-0.0.6/src/ready_auth/providers/ReadyAuthProvider.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.6/src/ready_auth/providers/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:46:13.141634 masonite-ready_auth-0.0.7/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.7/LICENSE
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.7/MANIFEST.in
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 10:46:13.141634 masonite-ready_auth-0.0.7/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4372 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.7/README.md
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.7/pyproject.toml
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-06 10:46:13.141634 masonite-ready_auth-0.0.7/setup.cfg
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3655 2023-05-06 10:46:08.000000 masonite-ready_auth-0.0.7/setup.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:46:13.133634 masonite-ready_auth-0.0.7/src/
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:46:13.137634 masonite-ready_auth-0.0.7/src/masonite_ready_auth.egg-info/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5583 2023-05-06 10:46:13.000000 masonite-ready_auth-0.0.7/src/masonite_ready_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1184 2023-05-06 10:46:13.000000 masonite-ready_auth-0.0.7/src/masonite_ready_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-06 10:46:13.000000 masonite-ready_auth-0.0.7/src/masonite_ready_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-06 10:46:13.000000 masonite-ready_auth-0.0.7/src/masonite_ready_auth.egg-info/requires.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       11 2023-05-06 10:46:13.000000 masonite-ready_auth-0.0.7/src/masonite_ready_auth.egg-info/top_level.txt
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:46:13.137634 masonite-ready_auth-0.0.7/src/ready_auth/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       79 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.7/src/ready_auth/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:46:13.137634 masonite-ready_auth-0.0.7/src/ready_auth/config/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      273 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.7/src/ready_auth/config/ready_auth.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:46:13.133634 masonite-ready_auth-0.0.7/src/ready_auth/database/
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:46:13.137634 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      434 2023-05-06 09:21:10.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171516_drop_conflicting_tables.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      441 2023-05-06 09:17:13.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171713_create_ip_addresses_table.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      437 2023-05-06 09:17:21.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171721_create_user_agents_table.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      437 2023-05-06 09:17:26.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171726_create_auth_tokens_table.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      437 2023-05-06 09:17:31.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171731_create_user_tokens_table.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      415 2023-05-06 09:17:37.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171737_create_users_table.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      445 2023-05-06 09:18:04.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171804_create_user_sessions_table.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      457 2023-05-06 09:18:21.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171821_create_access_locations_table.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      479 2023-05-06 09:18:59.000000 masonite-ready_auth-0.0.7/src/ready_auth/database/migrations/2023_05_06_171859_create_personal_access_tokens_table.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-06 10:46:13.141634 masonite-ready_auth-0.0.7/src/ready_auth/providers/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1239 2023-05-06 10:45:28.000000 masonite-ready_auth-0.0.7/src/ready_auth/providers/ReadyAuthProvider.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-06 09:06:53.000000 masonite-ready_auth-0.0.7/src/ready_auth/providers/__init__.py
```

### Comparing `masonite-ready_auth-0.0.6/LICENSE` & `masonite-ready_auth-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `masonite-ready_auth-0.0.6/PKG-INFO` & `masonite-ready_auth-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-ready_auth
-Version: 0.0.6
+Version: 0.0.7
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
-Metadata-Version: 2.1 Name: masonite-ready_auth Version: 0.0.6 Summary: Custom
+Metadata-Version: 2.1 Name: masonite-ready_auth Version: 0.0.7 Summary: Custom
 authentication module for Masonite 4. Home-page: https://github.com/lvjhn/
 masonite-ready_auth Author: LJ S.A. Author-email: lvjhn.mx@gmail.com License:
 MIT license Keywords: Masonite,Python,Development Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Environment :: Web Environment Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

### Comparing `masonite-ready_auth-0.0.6/README.md` & `masonite-ready_auth-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `masonite-ready_auth-0.0.6/setup.py` & `masonite-ready_auth-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="masonite-ready_auth",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.6",
+    version="0.0.7",
     packages=[
         "ready_auth",
         "ready_auth.providers",
         "ready_auth.config",
         "ready_auth.database", 
         "ready_auth.database.migrations"
     ],
```

### Comparing `masonite-ready_auth-0.0.6/src/masonite_ready_auth.egg-info/PKG-INFO` & `masonite-ready_auth-0.0.7/src/masonite_ready_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-ready-auth
-Version: 0.0.6
+Version: 0.0.7
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
-Metadata-Version: 2.1 Name: masonite-ready-auth Version: 0.0.6 Summary: Custom
+Metadata-Version: 2.1 Name: masonite-ready-auth Version: 0.0.7 Summary: Custom
 authentication module for Masonite 4. Home-page: https://github.com/lvjhn/
 masonite-ready_auth Author: LJ S.A. Author-email: lvjhn.mx@gmail.com License:
 MIT license Keywords: Masonite,Python,Development Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Environment :: Web Environment Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

### Comparing `masonite-ready_auth-0.0.6/src/masonite_ready_auth.egg-info/SOURCES.txt` & `masonite-ready_auth-0.0.7/src/masonite_ready_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

