# Comparing `tmp/pyproton-0.0.2.tar.gz` & `tmp/pyproton-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproton-0.0.2.tar", last modified: Sat May  6 00:30:46 2023, max compression
+gzip compressed data, was "pyproton-0.0.3.tar", last modified: Sat May  6 02:20:26 2023, max compression
```

## Comparing `pyproton-0.0.2.tar` & `pyproton-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:30:46.348348 pyproton-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 00:30:23.000000 pyproton-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-06 00:30:46.348348 pyproton-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-06 00:30:23.000000 pyproton-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 00:30:23.000000 pyproton-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:30:46.344347 pyproton-0.0.2/pyproton/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 00:30:23.000000 pyproton-0.0.2/pyproton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-06 00:30:23.000000 pyproton-0.0.2/pyproton/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:30:46.344347 pyproton-0.0.2/pyproton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-06 00:30:46.000000 pyproton-0.0.2/pyproton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-06 00:30:46.000000 pyproton-0.0.2/pyproton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:30:46.000000 pyproton-0.0.2/pyproton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 00:30:46.000000 pyproton-0.0.2/pyproton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:30:46.348348 pyproton-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 00:30:23.000000 pyproton-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 02:20:26.010092 pyproton-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 02:20:04.000000 pyproton-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-06 02:20:26.010092 pyproton-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-06 02:20:04.000000 pyproton-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 02:20:04.000000 pyproton-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 02:20:26.006092 pyproton-0.0.3/pyproton/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 02:20:04.000000 pyproton-0.0.3/pyproton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-06 02:20:04.000000 pyproton-0.0.3/pyproton/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 02:20:26.010092 pyproton-0.0.3/pyproton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-06 02:20:25.000000 pyproton-0.0.3/pyproton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-06 02:20:26.000000 pyproton-0.0.3/pyproton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 02:20:25.000000 pyproton-0.0.3/pyproton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 02:20:25.000000 pyproton-0.0.3/pyproton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 02:20:26.010092 pyproton-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 02:20:04.000000 pyproton-0.0.3/setup.py
```

### Comparing `pyproton-0.0.2/LICENSE` & `pyproton-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproton-0.0.2/PKG-INFO` & `pyproton-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproton
-Version: 0.0.2
+Version: 0.0.3
 Summary: Minimal wrapper implementation of the linux protonvpn-cli
 Home-page: https://github.com/aastopher/pyproton
 Author: Aaron Stopher
 Project-URL: Bug Tracker, https://github.com/aastopher/pyproton/issues
 Keywords: vpn,proton vpn,proton,wrapper,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,32 +39,40 @@
 
 ### **Install pyproton:**
 
 `pip install pyproton`
 
 ### **Import and use pyproton VPN:**
 
-* `verbose=True` (optional: `default=False`) turns on/off the stdin output for each step.
-* `vpn.login()` log the user into proton VPN
-* `vpn.logout()` log the user out of proton VPN
+#### Args
+
+* `user` **required:** user name string
+* `pw` **required:** password string
+* `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
+* `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
+* `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+
+#### Methods
+
+* `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
+* `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
+* `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
+* `vpn.disconnect()` disconnect from proton VPN endpoint - (context manager): `__exit__`
 * `vpn.shuffle()` disconnects from the current VPN and connected to another
-* `vpn.connect()` connect to proton VPN endpoint
-* `vpn.disconnect()` disconnect from proton VPN endpoint
-* Using the context manager will automatically (login / connect) and (disconnect / logout) when entering and exiting the VPN context.
 
 **NOTE:** It is generally recommended to use `dotenv` or some secrets library to load in credentials.
 
 ```python
 import os
 from pyproton import VPN
 
 user = 'user'
 pw = 'pw'
 
-with VPN(user, pw, verbose=True) as vpn:
+with VPN(user, pw) as vpn:
     print('do some stuff')
     vpn.shuffle()
     print('do more stuff')
 ```
 
 ### **TO-DO**
```

### Comparing `pyproton-0.0.2/README.md` & `pyproton-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,32 +24,40 @@
 
 ### **Install pyproton:**
 
 `pip install pyproton`
 
 ### **Import and use pyproton VPN:**
 
-* `verbose=True` (optional: `default=False`) turns on/off the stdin output for each step.
-* `vpn.login()` log the user into proton VPN
-* `vpn.logout()` log the user out of proton VPN
+#### Args
+
+* `user` **required:** user name string
+* `pw` **required:** password string
+* `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
+* `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
+* `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+
+#### Methods
+
+* `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
+* `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
+* `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
+* `vpn.disconnect()` disconnect from proton VPN endpoint - (context manager): `__exit__`
 * `vpn.shuffle()` disconnects from the current VPN and connected to another
-* `vpn.connect()` connect to proton VPN endpoint
-* `vpn.disconnect()` disconnect from proton VPN endpoint
-* Using the context manager will automatically (login / connect) and (disconnect / logout) when entering and exiting the VPN context.
 
 **NOTE:** It is generally recommended to use `dotenv` or some secrets library to load in credentials.
 
 ```python
 import os
 from pyproton import VPN
 
 user = 'user'
 pw = 'pw'
 
-with VPN(user, pw, verbose=True) as vpn:
+with VPN(user, pw) as vpn:
     print('do some stuff')
     vpn.shuffle()
     print('do more stuff')
 ```
 
 ### **TO-DO**
```

### Comparing `pyproton-0.0.2/pyproton/vpn.py` & `pyproton-0.0.3/pyproton/vpn.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,31 @@
     '''
     Wrapper for the linux protonvpn-cli
     
     Proton version compatibility:
     Proton VPN CLI v3.13.0 (protonvpn-nm-lib v3.14.0; proton-client v0.7.1)
     '''
 
-    def __init__(self, user, pw, verbose=False):
+    def __init__(self, user, pw, verbose=False, retries=3, timeout=20):
         self.user = user
         self.pw = pw
         self.logged_in = False
         self.active = False
         self.verbose = verbose
+        self.retries = retries
+        self.timeout = timeout
 
     def login(self):
         '''logs the user into proton vpn'''
         try:
             child = pexpect.spawn(f'protonvpn-cli login {self.user}')
             index = child.expect(['Enter your Proton VPN password:', 'You are already logged in.'], timeout=5)
             if index == 0:
                 child.sendline(self.pw)
-                index = child.expect(['Successful login', 'Incorrect login credentials', 'error occured'], timeout=20)
+                index = child.expect(['Successful login', 'Incorrect login credentials', 'error occured'], timeout=self.timeout)
                 if index == 0:
                     child.expect(pexpect.EOF)
                     if self.verbose:
                         sys.stdout.write('successfully logged in\n')
                     self.logged_in = True
                     return
                 elif index == 1:
@@ -80,48 +82,55 @@
                 else:
                     raise VPNException("error logging out", 500)
             else:
                 raise VPNException("error logging out", 500)
         
         except pexpect.ExceptionPexpect as e:
             raise VPNException(str(e), 500)
-        
 
     def connect(self):
         '''
         connects to a random US Proton VPN
 
         NOTE: less than 1 second sleep intervals resulted in frequent incomplete connections
         '''
-        try:
-            child = pexpect.spawn('protonvpn-cli c')
-            time.sleep(1)
-            child.sendline('U') # select United States
-            time.sleep(1)
-            # randomly select VPN connection
-            for _ in range(random.randint(0, 30)):
-                child.send('+')
-            child.sendline('+') # + 1 and enter VPN selection
-            time.sleep(1)
-            child.sendline('u') # select updb - better speed
-            time.sleep(1)
-            index = child.expect(['Successfully connected'], timeout=30)
-            if index == 0:
-                output = child.before.decode().strip().splitlines()[-1]
-                child.expect(pexpect.EOF)
-                if self.verbose:
-                    sys.stdout.write(output)
-                    sys.stdout.write('\nsuccessfully connected\n')
-                self.active = True
-                return
-            else:
-                raise VPNException('error connecting to vpn', 500)
+        for retry in range(self.retries):
+            try:
+                time.sleep(0.1)
+                child = pexpect.spawn('protonvpn-cli c')
+                time.sleep(1)
+                child.sendline('U') # select United States
+                time.sleep(1)
+                # randomly select VPN connection
+                for _ in range(random.randint(0, 30)):
+                    child.send('+')
+                child.sendline('+') # + 1 and enter VPN selection
+                time.sleep(1)
+                child.sendline('u') # select updb - better speed
+                time.sleep(1)
+                index = child.expect(['Successfully connected'], timeout=10)
+                if index == 0:
+                    output = child.before.decode().strip().splitlines()[-1]
+                    child.expect(pexpect.EOF)
+                    if self.verbose:
+                        sys.stdout.write(output)
+                        sys.stdout.write('\nsuccessfully connected\n')
+                    self.active = True
+                    return
+                else:
+                    raise VPNException('error connecting to vpn', 500)
 
-        except pexpect.ExceptionPexpect as e:
-            raise VPNException(str(e), 500)
+            except pexpect.ExceptionPexpect as e:
+                if retry == self.retries-1:
+                    raise VPNException('maximum retries reached while connecting to VPN', 500)
+                else:
+                    time.sleep(3)
+                    if self.verbose:
+                        sys.stderr.write(f'error while connecting to VPN; retrying connection... {retry}\n')
+                    continue
 
     def disconnect(self):
         '''disconnects from VPN connection'''
         try:
             child = pexpect.spawn('protonvpn-cli d')
             index = child.expect(['Successfully disconnected','No Proton VPN connection was found'], timeout=5)
             if index == 0:
```

### Comparing `pyproton-0.0.2/pyproton.egg-info/PKG-INFO` & `pyproton-0.0.3/pyproton.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproton
-Version: 0.0.2
+Version: 0.0.3
 Summary: Minimal wrapper implementation of the linux protonvpn-cli
 Home-page: https://github.com/aastopher/pyproton
 Author: Aaron Stopher
 Project-URL: Bug Tracker, https://github.com/aastopher/pyproton/issues
 Keywords: vpn,proton vpn,proton,wrapper,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,32 +39,40 @@
 
 ### **Install pyproton:**
 
 `pip install pyproton`
 
 ### **Import and use pyproton VPN:**
 
-* `verbose=True` (optional: `default=False`) turns on/off the stdin output for each step.
-* `vpn.login()` log the user into proton VPN
-* `vpn.logout()` log the user out of proton VPN
+#### Args
+
+* `user` **required:** user name string
+* `pw` **required:** password string
+* `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
+* `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
+* `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+
+#### Methods
+
+* `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
+* `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
+* `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
+* `vpn.disconnect()` disconnect from proton VPN endpoint - (context manager): `__exit__`
 * `vpn.shuffle()` disconnects from the current VPN and connected to another
-* `vpn.connect()` connect to proton VPN endpoint
-* `vpn.disconnect()` disconnect from proton VPN endpoint
-* Using the context manager will automatically (login / connect) and (disconnect / logout) when entering and exiting the VPN context.
 
 **NOTE:** It is generally recommended to use `dotenv` or some secrets library to load in credentials.
 
 ```python
 import os
 from pyproton import VPN
 
 user = 'user'
 pw = 'pw'
 
-with VPN(user, pw, verbose=True) as vpn:
+with VPN(user, pw) as vpn:
     print('do some stuff')
     vpn.shuffle()
     print('do more stuff')
 ```
 
 ### **TO-DO**
```

### Comparing `pyproton-0.0.2/setup.py` & `pyproton-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyproton",
-    version="0.0.2",
+    version="0.0.3",
     author="Aaron Stopher",
     packages=setuptools.find_packages(include=["pyproton"]),
     description="Minimal wrapper implementation of the linux protonvpn-cli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aastopher/pyproton",
     project_urls={
```

