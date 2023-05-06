# Comparing `tmp/mutil-0.3.2.tar.gz` & `tmp/mutil-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutil-0.3.2.tar", last modified: Fri Mar 24 21:39:09 2023, max compression
+gzip compressed data, was "mutil-0.4.0.tar", last modified: Sat May  6 05:36:41 2023, max compression
```

## Comparing `mutil-0.3.2.tar` & `mutil-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,20 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-03-24 21:39:09.266748 mutil-0.3.2/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1059 2023-02-23 18:49:29.000000 mutil-0.3.2/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      557 2023-03-24 21:39:09.266393 mutil-0.3.2/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       61 2023-02-23 19:03:06.000000 mutil-0.3.2/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-03-24 21:39:09.127615 mutil-0.3.2/mutil.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      557 2023-03-24 21:39:09.000000 mutil-0.3.2/mutil.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      535 2023-03-24 21:39:09.000000 mutil-0.3.2/mutil.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-03-24 21:39:09.000000 mutil-0.3.2/mutil.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       43 2023-03-24 21:39:09.000000 mutil-0.3.2/mutil.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-03-24 21:39:09.000000 mutil-0.3.2/mutil.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        6 2023-03-24 21:39:09.000000 mutil-0.3.2/mutil.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      689 2023-03-24 21:38:47.000000 mutil-0.3.2/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-03-24 21:39:09.266897 mutil-0.3.2/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2023-03-24 21:15:46.000000 mutil-0.3.2/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-03-24 21:39:09.112842 mutil-0.3.2/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-03-24 21:39:09.265652 mutil-0.3.2/src/mutil/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      638 2023-02-23 20:56:19.000000 mutil-0.3.2/src/mutil/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1570 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/mdraft.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1206 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/menact.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2392 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/mfree.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1473 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/minduct.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      859 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/mprevious.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      859 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/mproposed.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1177 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/mrepeal.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4023 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/mreserve.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1588 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/mretire.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6384 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/musage.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    13751 2023-03-24 21:38:13.000000 mutil-0.3.2/src/mutil/mutil.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/setup.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2239 2023-03-24 17:08:11.000000 mutil-0.3.2/src/mutil/update_shared.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-03-24 21:38:41.000000 mutil-0.3.2/src/mutil/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-05-06 05:36:41.125846 mutil-0.4.0/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1059 2023-02-23 18:49:29.000000 mutil-0.4.0/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1813 2023-05-06 05:36:41.125347 mutil-0.4.0/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1317 2023-05-06 05:35:30.000000 mutil-0.4.0/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-05-06 05:36:41.105531 mutil-0.4.0/mutil.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1813 2023-05-06 05:36:41.000000 mutil-0.4.0/mutil.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      300 2023-05-06 05:36:41.000000 mutil-0.4.0/mutil.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-05-06 05:36:41.000000 mutil-0.4.0/mutil.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       43 2023-05-06 05:36:41.000000 mutil-0.4.0/mutil.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-05-06 05:36:41.000000 mutil-0.4.0/mutil.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        6 2023-05-06 05:36:41.000000 mutil-0.4.0/mutil.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      689 2023-05-01 15:00:35.000000 mutil-0.4.0/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-05-06 05:36:41.126303 mutil-0.4.0/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       69 2023-03-24 21:15:46.000000 mutil-0.4.0/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-05-06 05:36:41.093267 mutil-0.4.0/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-05-06 05:36:41.123917 mutil-0.4.0/src/mutil/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      638 2023-02-23 20:56:19.000000 mutil-0.4.0/src/mutil/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1473 2023-03-24 17:08:11.000000 mutil-0.4.0/src/mutil/minduct.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    29189 2023-04-20 05:03:42.000000 mutil-0.4.0/src/mutil/mutil.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-05-01 15:00:43.000000 mutil-0.4.0/src/mutil/version.py
```

### Comparing `mutil-0.3.2/LICENSE` & `mutil-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutil-0.3.2/pyproject.toml` & `mutil-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mutil"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   { name="Anthony Aylward", email="aaylward@salk.edu" },
 ]
 description = "Utility for managing memory with cgroup"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mutil-0.3.2/src/mutil/__init__.py` & `mutil-0.4.0/src/mutil/__init__.py`

 * *Files identical despite different names*

### Comparing `mutil-0.3.2/src/mutil/menact.py` & `mutil-0.4.0/src/mutil/minduct.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 #!/usr/bin/env python3
 #===============================================================================
-# menact.py
+# minduct.py
 #===============================================================================
 
-"""Enact the proposed memory policy"""
+"""Induct a user into the memory policy"""
 
 
 
 
 # Imports ----------------------------------------------------------------------
 
 import argparse
-import shutil
+import getpass
 
 import mutil
 
 
 
 
-# Functions --------------------------------------------------------------------
+# Function ---------------------------------------------------------------------
 
 def main(args):
-    mutil.require_super_user()
-    shutil.move(mutil.CURRENT_POLICY_PATH, mutil.PREVIOUS_POLICY_PATH)
-    shutil.copy(mutil.PROPOSED_POLICY_PATH, mutil.CURRENT_POLICY_PATH)
-    policy = mutil.load_policy(mutil.CURRENT_POLICY_PATH)
-    mutil.enact_policy(policy, no_daemon=args.no_daemon)
+    new_users = set(user for user in args.users.split(','))
+    policy = mutil.load_policy(mutil.PROPOSED_POLICY_PATH)
+    existing_users = mutil.get_user_set(policy)
+    for user in new_users.intersection(existing_users):
+        print('{} is already in the memory policy.'.format(user))
+    policy['free']['users'].extend(list(new_users - existing_users))
+    mutil.dump_policy(policy, mutil.PROPOSED_POLICY_PATH)
+    for user in new_users - existing_users:
+        print('{} has been inducted into the memory policy.'.format(user))
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(
-        description=('Enact the proposed memory policy'))
+        description=(
+            'Induct a new user into the memory policy'))
     parser.add_argument(
-        '--no-daemon', action='store_true',
-        help='Don\'t restart the daemon. (This is for use in setup).')
+        '-u', '--users', default=getpass.getuser(),
+        help='comma-separated list of users to induct')
     return parser.parse_args()
 
 
 
 
 # Execute ----------------------------------------------------------------------
```

