# Comparing `tmp/pyproton-0.0.3.tar.gz` & `tmp/pyproton-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproton-0.0.3.tar", last modified: Sat May  6 02:20:26 2023, max compression
+gzip compressed data, was "pyproton-0.0.4.tar", last modified: Sat May  6 08:22:52 2023, max compression
```

## Comparing `pyproton-0.0.3.tar` & `pyproton-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 02:20:26.010092 pyproton-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 02:20:04.000000 pyproton-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-06 02:20:26.010092 pyproton-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-06 02:20:04.000000 pyproton-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 02:20:04.000000 pyproton-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 02:20:26.006092 pyproton-0.0.3/pyproton/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 02:20:04.000000 pyproton-0.0.3/pyproton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-06 02:20:04.000000 pyproton-0.0.3/pyproton/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 02:20:26.010092 pyproton-0.0.3/pyproton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-06 02:20:25.000000 pyproton-0.0.3/pyproton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-06 02:20:26.000000 pyproton-0.0.3/pyproton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 02:20:25.000000 pyproton-0.0.3/pyproton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 02:20:25.000000 pyproton-0.0.3/pyproton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 02:20:26.010092 pyproton-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 02:20:04.000000 pyproton-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:52.533567 pyproton-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 08:22:35.000000 pyproton-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-06 08:22:52.533567 pyproton-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-06 08:22:35.000000 pyproton-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 08:22:35.000000 pyproton-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:52.529567 pyproton-0.0.4/pyproton/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 08:22:35.000000 pyproton-0.0.4/pyproton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-05-06 08:22:35.000000 pyproton-0.0.4/pyproton/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:52.533567 pyproton-0.0.4/pyproton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-06 08:22:52.000000 pyproton-0.0.4/pyproton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-06 08:22:52.000000 pyproton-0.0.4/pyproton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:22:52.000000 pyproton-0.0.4/pyproton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 08:22:52.000000 pyproton-0.0.4/pyproton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:22:52.533567 pyproton-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 08:22:35.000000 pyproton-0.0.4/setup.py
```

### Comparing `pyproton-0.0.3/LICENSE` & `pyproton-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproton-0.0.3/PKG-INFO` & `pyproton-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproton
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimal wrapper implementation of the linux protonvpn-cli
 Home-page: https://github.com/aastopher/pyproton
 Author: Aaron Stopher
 Project-URL: Bug Tracker, https://github.com/aastopher/pyproton/issues
 Keywords: vpn,proton vpn,proton,wrapper,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,24 +46,27 @@
 #### Args
 
 * `user` **required:** user name string
 * `pw` **required:** password string
 * `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
 * `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
 * `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+* `location` **optional:** (`default='U'`) location of servers to connect to (free servers only): `{'J':'Japan','N':'Netherlands','U':'United States'}`.
 
 #### Methods
 
 * `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
 * `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
 * `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
 * `vpn.disconnect()` disconnect from proton VPN endpoint - (context manager): `__exit__`
 * `vpn.shuffle()` disconnects from the current VPN and connected to another
 
-**NOTE:** It is generally recommended to use `dotenv` or some secrets library to load in credentials.
+#### Basic Usage
+
+**NOTE:** It is generally recommended to use `dotenv` or another method for loading in secrets. Please do NOT hardcode account credentials in a production environment, this is a critical security risk!
 
 ```python
 import os
 from pyproton import VPN
 
 user = 'user'
 pw = 'pw'
```

### Comparing `pyproton-0.0.3/README.md` & `pyproton-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,24 +31,27 @@
 #### Args
 
 * `user` **required:** user name string
 * `pw` **required:** password string
 * `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
 * `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
 * `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+* `location` **optional:** (`default='U'`) location of servers to connect to (free servers only): `{'J':'Japan','N':'Netherlands','U':'United States'}`.
 
 #### Methods
 
 * `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
 * `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
 * `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
 * `vpn.disconnect()` disconnect from proton VPN endpoint - (context manager): `__exit__`
 * `vpn.shuffle()` disconnects from the current VPN and connected to another
 
-**NOTE:** It is generally recommended to use `dotenv` or some secrets library to load in credentials.
+#### Basic Usage
+
+**NOTE:** It is generally recommended to use `dotenv` or another method for loading in secrets. Please do NOT hardcode account credentials in a production environment, this is a critical security risk!
 
 ```python
 import os
 from pyproton import VPN
 
 user = 'user'
 pw = 'pw'
```

### Comparing `pyproton-0.0.3/pyproton/vpn.py` & `pyproton-0.0.4/pyproton/vpn.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,26 @@
     '''
     Wrapper for the linux protonvpn-cli
     
     Proton version compatibility:
     Proton VPN CLI v3.13.0 (protonvpn-nm-lib v3.14.0; proton-client v0.7.1)
     '''
 
-    def __init__(self, user, pw, verbose=False, retries=3, timeout=20):
+    def __init__(self, user, pw, verbose=False, retries=3, timeout=20, location='U'):
         self.user = user
         self.pw = pw
         self.logged_in = False
         self.active = False
         self.verbose = verbose
         self.retries = retries
         self.timeout = timeout
+        if location in ['J','N','U']:
+            self.location = location
+        else:
+            raise VPNException(f'invalid location {location}', 400)
 
     def login(self):
         '''logs the user into proton vpn'''
         try:
             child = pexpect.spawn(f'protonvpn-cli login {self.user}')
             index = child.expect(['Enter your Proton VPN password:', 'You are already logged in.'], timeout=5)
             if index == 0:
@@ -94,15 +98,15 @@
         NOTE: less than 1 second sleep intervals resulted in frequent incomplete connections
         '''
         for retry in range(self.retries):
             try:
                 time.sleep(0.1)
                 child = pexpect.spawn('protonvpn-cli c')
                 time.sleep(1)
-                child.sendline('U') # select United States
+                child.sendline(self.location) # select location
                 time.sleep(1)
                 # randomly select VPN connection
                 for _ in range(random.randint(0, 30)):
                     child.send('+')
                 child.sendline('+') # + 1 and enter VPN selection
                 time.sleep(1)
                 child.sendline('u') # select updb - better speed
```

### Comparing `pyproton-0.0.3/pyproton.egg-info/PKG-INFO` & `pyproton-0.0.4/pyproton.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproton
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimal wrapper implementation of the linux protonvpn-cli
 Home-page: https://github.com/aastopher/pyproton
 Author: Aaron Stopher
 Project-URL: Bug Tracker, https://github.com/aastopher/pyproton/issues
 Keywords: vpn,proton vpn,proton,wrapper,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,24 +46,27 @@
 #### Args
 
 * `user` **required:** user name string
 * `pw` **required:** password string
 * `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
 * `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
 * `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+* `location` **optional:** (`default='U'`) location of servers to connect to (free servers only): `{'J':'Japan','N':'Netherlands','U':'United States'}`.
 
 #### Methods
 
 * `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
 * `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
 * `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
 * `vpn.disconnect()` disconnect from proton VPN endpoint - (context manager): `__exit__`
 * `vpn.shuffle()` disconnects from the current VPN and connected to another
 
-**NOTE:** It is generally recommended to use `dotenv` or some secrets library to load in credentials.
+#### Basic Usage
+
+**NOTE:** It is generally recommended to use `dotenv` or another method for loading in secrets. Please do NOT hardcode account credentials in a production environment, this is a critical security risk!
 
 ```python
 import os
 from pyproton import VPN
 
 user = 'user'
 pw = 'pw'
```

### Comparing `pyproton-0.0.3/setup.py` & `pyproton-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyproton",
-    version="0.0.3",
+    version="0.0.4",
     author="Aaron Stopher",
     packages=setuptools.find_packages(include=["pyproton"]),
     description="Minimal wrapper implementation of the linux protonvpn-cli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aastopher/pyproton",
     project_urls={
```

