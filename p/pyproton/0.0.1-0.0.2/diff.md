# Comparing `tmp/pyproton-0.0.1.tar.gz` & `tmp/pyproton-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproton-0.0.1.tar", last modified: Sat May  6 00:08:38 2023, max compression
+gzip compressed data, was "pyproton-0.0.2.tar", last modified: Sat May  6 00:30:46 2023, max compression
```

## Comparing `pyproton-0.0.1.tar` & `pyproton-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:08:38.827245 pyproton-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 00:08:18.000000 pyproton-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-06 00:08:38.827245 pyproton-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-06 00:08:18.000000 pyproton-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 00:08:18.000000 pyproton-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:08:38.823245 pyproton-0.0.1/pyproton/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 00:08:18.000000 pyproton-0.0.1/pyproton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-06 00:08:18.000000 pyproton-0.0.1/pyproton/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:08:38.827245 pyproton-0.0.1/pyproton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-06 00:08:38.000000 pyproton-0.0.1/pyproton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-06 00:08:38.000000 pyproton-0.0.1/pyproton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:08:38.000000 pyproton-0.0.1/pyproton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 00:08:38.000000 pyproton-0.0.1/pyproton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:08:38.827245 pyproton-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 00:08:18.000000 pyproton-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:30:46.348348 pyproton-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 00:30:23.000000 pyproton-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-06 00:30:46.348348 pyproton-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-06 00:30:23.000000 pyproton-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 00:30:23.000000 pyproton-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:30:46.344347 pyproton-0.0.2/pyproton/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 00:30:23.000000 pyproton-0.0.2/pyproton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-06 00:30:23.000000 pyproton-0.0.2/pyproton/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:30:46.344347 pyproton-0.0.2/pyproton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-06 00:30:46.000000 pyproton-0.0.2/pyproton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-06 00:30:46.000000 pyproton-0.0.2/pyproton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:30:46.000000 pyproton-0.0.2/pyproton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 00:30:46.000000 pyproton-0.0.2/pyproton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:30:46.348348 pyproton-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 00:30:23.000000 pyproton-0.0.2/setup.py
```

### Comparing `pyproton-0.0.1/LICENSE` & `pyproton-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproton-0.0.1/PKG-INFO` & `pyproton-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,11 @@
-Metadata-Version: 2.1
-Name: pyproton
-Version: 0.0.1
-Summary: Minimal wrapper implementation of the linux protonvpn-cli
-Home-page: https://github.com/aastopher/pyproton
-Author: Aaron Stopher
-Project-URL: Bug Tracker, https://github.com/aastopher/pyproton/issues
-Keywords: vpn,proton vpn,proton,wrapper,cli
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyProton
 
+[![PyPI version](https://badge.fury.io/py/pyproton.svg)](https://badge.fury.io/py/pyproton)
+
 This package is a lightweight minimal wrapper implementation of the linux protonvpn-cli; designed to be an intuitive and simple to use interface for the Proton VPN in python.
 
 ## Getting Started
 
 ### **Install the CLI:**
 
 [Proton VPN Docs](https://protonvpn.com/support/linux-vpn-tool/)
@@ -65,8 +52,8 @@
 ```
 
 ### **TO-DO**
 
 * PyTest & Tox testing
 * Sphynx docs
 * Coverage
-* Deepsource scanning
+* Deepsource scanning
```

### Comparing `pyproton-0.0.1/pyproton/vpn.py` & `pyproton-0.0.2/pyproton/vpn.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,33 +32,33 @@
             child = pexpect.spawn(f'protonvpn-cli login {self.user}')
             index = child.expect(['Enter your Proton VPN password:', 'You are already logged in.'], timeout=5)
             if index == 0:
                 child.sendline(self.pw)
                 index = child.expect(['Successful login', 'Incorrect login credentials', 'error occured'], timeout=20)
                 if index == 0:
                     child.expect(pexpect.EOF)
+                    if self.verbose:
+                        sys.stdout.write('successfully logged in\n')
+                    self.logged_in = True
+                    return
                 elif index == 1:
                     raise VPNException("invalid credentials", 401)
                 else:
                     raise VPNException("error logging in", 401)
             elif index == 1:
                 try:
                     raise VPNException("already logged in", 409)
                 except VPNException as e:
                     if self.verbose:
                         sys.stderr.write('already logged in skipping step...\n')
                     self.logged_in = True
                     return
-
-            
+                
         except pexpect.ExceptionPexpect as e:
             raise VPNException(str(e), 500)
-        if self.verbose:
-            sys.stdout.write('successfully logged in\n')
-        self.logged_in = True
 
     def logout(self):
         '''logs the user out of proton vpn'''
         try:
             child = pexpect.spawn('protonvpn-cli logout')
             index = child.expect(['successfully logged out', 'login first', 'Logging out will disconnect the active VPN'], timeout=5)
             if index == 0:
@@ -72,14 +72,15 @@
                 child.sendline('y')
                 index_c = child.expect(['successfully logged out'], timeout=10)
                 if index_c == 0:
                     child.expect(pexpect.EOF)
                     if self.verbose:
                         sys.stdout.write('successfully logged out\n')
                     self.logged_in = False
+                    return
                 else:
                     raise VPNException("error logging out", 500)
             else:
                 raise VPNException("error logging out", 500)
         
         except pexpect.ExceptionPexpect as e:
             raise VPNException(str(e), 500)
@@ -107,14 +108,15 @@
             if index == 0:
                 output = child.before.decode().strip().splitlines()[-1]
                 child.expect(pexpect.EOF)
                 if self.verbose:
                     sys.stdout.write(output)
                     sys.stdout.write('\nsuccessfully connected\n')
                 self.active = True
+                return
             else:
                 raise VPNException('error connecting to vpn', 500)
 
         except pexpect.ExceptionPexpect as e:
             raise VPNException(str(e), 500)
 
     def disconnect(self):
```

### Comparing `pyproton-0.0.1/pyproton.egg-info/PKG-INFO` & `pyproton-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pyproton
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimal wrapper implementation of the linux protonvpn-cli
 Home-page: https://github.com/aastopher/pyproton
 Author: Aaron Stopher
 Project-URL: Bug Tracker, https://github.com/aastopher/pyproton/issues
 Keywords: vpn,proton vpn,proton,wrapper,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyProton
 
+[![PyPI version](https://badge.fury.io/py/pyproton.svg)](https://badge.fury.io/py/pyproton)
+
 This package is a lightweight minimal wrapper implementation of the linux protonvpn-cli; designed to be an intuitive and simple to use interface for the Proton VPN in python.
 
 ## Getting Started
 
 ### **Install the CLI:**
 
 [Proton VPN Docs](https://protonvpn.com/support/linux-vpn-tool/)
```

### Comparing `pyproton-0.0.1/setup.py` & `pyproton-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyproton",
-    version="0.0.1",
+    version="0.0.2",
     author="Aaron Stopher",
     packages=setuptools.find_packages(include=["pyproton"]),
     description="Minimal wrapper implementation of the linux protonvpn-cli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aastopher/pyproton",
     project_urls={
```

