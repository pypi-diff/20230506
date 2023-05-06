# Comparing `tmp/propelauth-py-3.1.1.tar.gz` & `tmp/propelauth-py-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-py-3.1.1.tar", last modified: Wed May  3 19:34:02 2023, max compression
+gzip compressed data, was "propelauth-py-3.1.2.tar", last modified: Sat May  6 18:54:49 2023, max compression
```

## Comparing `propelauth-py-3.1.1.tar` & `propelauth-py-3.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:02.270700 propelauth-py-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-03 19:34:02.270700 propelauth-py-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:02.266700 propelauth-py-3.1.1/propelauth_py/
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/auth_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:02.270700 propelauth-py-3.1.1/propelauth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:34:02.270700 propelauth-py-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/propelauth_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/auth_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/propelauth_py/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/propelauth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 18:54:49.000000 propelauth-py-3.1.2/propelauth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 18:54:49.040270 propelauth-py-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-06 18:54:39.000000 propelauth-py-3.1.2/setup.py
```

### Comparing `propelauth-py-3.1.1/LICENSE` & `propelauth-py-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.1/PKG-INFO` & `propelauth-py-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.1
+Version: 3.1.2
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.1 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.2 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.1/README.md` & `propelauth-py-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.1/propelauth_py/__init__.py` & `propelauth-py-3.1.2/propelauth_py/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.1/propelauth_py/api.py` & `propelauth-py-3.1.2/propelauth_py/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,14 +335,16 @@
     elif response.status_code == 403:
         raise UserNotFoundException()
     elif response.status_code == 404:
         raise RuntimeError("Access token creation is not enabled")
     elif not response.ok:
         raise RuntimeError("Unknown error when creating access token")
 
+    return response.json()
+
 
 def _migrate_user_from_external_source(auth_url, api_key, email, email_confirmed,
                                        existing_user_id=None, existing_password_hash=None,
                                        existing_mfa_base32_encoded_secret=None,
                                        ask_user_to_update_password_on_login=False,
                                        enabled=None, first_name=None, last_name=None, username=None):
     url = auth_url + "/api/backend/v1/migrate_user/"
```

### Comparing `propelauth-py-3.1.1/propelauth_py/auth_fns.py` & `propelauth-py-3.1.2/propelauth_py/auth_fns.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.1/propelauth_py/errors.py` & `propelauth-py-3.1.2/propelauth_py/errors.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.1/propelauth_py/jwt.py` & `propelauth-py-3.1.2/propelauth_py/jwt.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.1/propelauth_py/user.py` & `propelauth-py-3.1.2/propelauth_py/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.1/propelauth_py.egg-info/PKG-INFO` & `propelauth-py-3.1.2/propelauth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.1
+Version: 3.1.2
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.1 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.2 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.1/setup.py` & `propelauth-py-3.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-py",
-    version="3.1.1",
+    version="3.1.2",
     description="A python authentication library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-py",
     packages=find_packages(include=["propelauth_py"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
```

