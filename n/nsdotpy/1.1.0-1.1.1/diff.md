# Comparing `tmp/nsdotpy-1.1.0.tar.gz` & `tmp/nsdotpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.1.0.tar", max compression
+gzip compressed data, was "nsdotpy-1.1.1.tar", max compression
```

## Comparing `nsdotpy-1.1.0.tar` & `nsdotpy-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35005 2023-04-26 23:31:32.556941 nsdotpy-1.1.0/LICENSE.md
--rw-r--r--   0        0        0      697 2023-05-06 06:25:57.998233 nsdotpy-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      662 2023-05-06 06:38:30.363856 nsdotpy-1.1.0/README.md
--rw-r--r--   0        0        0      805 2023-05-06 06:05:20.689321 nsdotpy-1.1.0/src/__init__.py
--rw-r--r--   0        0        0    32154 2023-05-06 06:41:51.956145 nsdotpy-1.1.0/src/session.py
--rw-r--r--   0        0        0     2400 2023-05-06 06:05:24.536374 nsdotpy-1.1.0/src/valid_tags.py
--rw-r--r--   0        0        0     1519 1970-01-01 00:00:00.000000 nsdotpy-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35005 2023-04-26 23:31:32.556941 nsdotpy-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0      805 2023-05-06 06:05:20.689321 nsdotpy-1.1.1/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    32154 2023-05-06 07:46:35.968122 nsdotpy-1.1.1/nsdotpy/session.py
+-rw-r--r--   0        0        0     2400 2023-05-06 06:05:24.536374 nsdotpy-1.1.1/nsdotpy/valid_tags.py
+-rw-r--r--   0        0        0      665 2023-05-06 07:45:43.726513 nsdotpy-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      738 2023-05-06 07:51:44.902801 nsdotpy-1.1.1/README.md
+-rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 nsdotpy-1.1.1/PKG-INFO
```

### Comparing `nsdotpy-1.1.0/LICENSE.md` & `nsdotpy-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.0/README.md` & `nsdotpy-1.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 A Python wrapper around requests for legally interacting with the HTML NationStates site, as well as a barebones API client. Built for legality first and foremost, as well as ease of use.
 
 ## Installation
 ``pip install nsdotpy``
 
 ## Simple Example
 ```python
-from nsdotpy import NSClient
+from nsdotpy.session import NSClient
 session = NSClient("NSDotPy Example," "1.0.0", "User Nation", "Dev Nation")
 if session.login("User Nation", "Password"):  # logs in and checks if login was successful
     session.move_to_region("Lily")  # only moves if you successfully logged in
 ```
 ## TODO:
 - ~~Region Admin Controls~~
 - Dossier and reports handling
 - More fleshed out API Client
+## Docs
+https://sw33ze.github.io/NSDotPy/src/session.html#NSSession
```

### Comparing `nsdotpy-1.1.0/src/__init__.py` & `nsdotpy-1.1.1/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.0/src/session.py` & `nsdotpy-1.1.1/nsdotpy/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.1.0"
+        self.VERSION = "1.1.1"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
```

### Comparing `nsdotpy-1.1.0/src/valid_tags.py` & `nsdotpy-1.1.1/nsdotpy/valid_tags.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.0/PKG-INFO` & `nsdotpy-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A wrapper around requests that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -22,17 +22,18 @@
 A Python wrapper around requests for legally interacting with the HTML NationStates site, as well as a barebones API client. Built for legality first and foremost, as well as ease of use.
 
 ## Installation
 ``pip install nsdotpy``
 
 ## Simple Example
 ```python
-from nsdotpy import NSClient
+from nsdotpy.session import NSClient
 session = NSClient("NSDotPy Example," "1.0.0", "User Nation", "Dev Nation")
 if session.login("User Nation", "Password"):  # logs in and checks if login was successful
     session.move_to_region("Lily")  # only moves if you successfully logged in
 ```
 ## TODO:
 - ~~Region Admin Controls~~
 - Dossier and reports handling
 - More fleshed out API Client
-
+## Docs
+https://sw33ze.github.io/NSDotPy/src/session.html#NSSession
```

