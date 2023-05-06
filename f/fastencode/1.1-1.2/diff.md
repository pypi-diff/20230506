# Comparing `tmp/fastencode-1.1.tar.gz` & `tmp/fastencode-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastencode-1.1.tar", last modified: Sun Apr  9 14:12:57 2023, max compression
+gzip compressed data, was "fastencode-1.2.tar", last modified: Sat May  6 19:52:22 2023, max compression
```

## Comparing `fastencode-1.1.tar` & `fastencode-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 14:12:57.974356 fastencode-1.1/
--rw-rw-rw-   0        0        0     1077 2023-04-09 08:15:47.000000 fastencode-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3772 2023-04-09 14:12:57.974356 fastencode-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2601 2023-04-09 14:10:43.000000 fastencode-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 14:12:57.966729 fastencode-1.1/fastencode/
--rw-rw-rw-   0        0        0       36 2023-04-09 09:11:20.000000 fastencode-1.1/fastencode/__init__.py
--rw-rw-rw-   0        0        0     3058 2023-04-09 09:23:06.000000 fastencode-1.1/fastencode/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 14:12:57.973355 fastencode-1.1/fastencode.egg-info/
--rw-rw-rw-   0        0        0     3772 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-09 14:12:57.975757 fastencode-1.1/setup.cfg
--rw-rw-rw-   0        0        0     2147 2023-04-09 14:12:34.000000 fastencode-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:52:22.005345 fastencode-1.2/
+-rw-rw-rw-   0        0        0     1077 2023-04-09 08:15:47.000000 fastencode-1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3787 2023-05-06 19:52:22.005345 fastencode-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2601 2023-04-09 14:15:14.000000 fastencode-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 19:52:22.005345 fastencode-1.2/fastencode/
+-rw-rw-rw-   0        0        0       36 2023-04-09 14:15:14.000000 fastencode-1.2/fastencode/__init__.py
+-rw-rw-rw-   0        0        0     3456 2023-04-14 08:35:40.000000 fastencode-1.2/fastencode/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:52:22.005345 fastencode-1.2/fastencode.egg-info/
+-rw-rw-rw-   0        0        0     3787 2023-05-06 19:52:21.000000 fastencode-1.2/fastencode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-06 19:52:21.000000 fastencode-1.2/fastencode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:52:21.000000 fastencode-1.2/fastencode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-06 19:52:21.000000 fastencode-1.2/fastencode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 19:52:21.000000 fastencode-1.2/fastencode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-06 19:52:22.018358 fastencode-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2177 2023-05-06 19:52:19.000000 fastencode-1.2/setup.py
```

### Comparing `fastencode-1.1/LICENSE.txt` & `fastencode-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastencode-1.1/PKG-INFO` & `fastencode-1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fastencode
-Version: 1.1
-Summary: An easy way to use different encoding: bytes, hex, ascii array, binary, long
+Version: 1.2
+Summary: An easy way to use different encoding: bytes, hex, ascii array, binary, long, base64
 Home-page: https://github.com/user/reponame
 Author: ES3
 Author-email: ourteamscare@gmail.com
 License: MIT
 Download-URL: https://github.com/elyassaf/Easy-Encoding/archive/refs/tags/v_1.0.tar.gz
-Keywords: encoding,hex,bytes,binary representation,decoding,ascii
+Keywords: encoding,hex,bytes,binary representation,decoding,ascii,base64
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `fastencode-1.1/README.md` & `fastencode-1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastencode-1.1/fastencode.egg-info/PKG-INFO` & `fastencode-1.2/fastencode.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fastencode
-Version: 1.1
-Summary: An easy way to use different encoding: bytes, hex, ascii array, binary, long
+Version: 1.2
+Summary: An easy way to use different encoding: bytes, hex, ascii array, binary, long, base64
 Home-page: https://github.com/user/reponame
 Author: ES3
 Author-email: ourteamscare@gmail.com
 License: MIT
 Download-URL: https://github.com/elyassaf/Easy-Encoding/archive/refs/tags/v_1.0.tar.gz
-Keywords: encoding,hex,bytes,binary representation,decoding,ascii
+Keywords: encoding,hex,bytes,binary representation,decoding,ascii,base64
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `fastencode-1.1/setup.py` & `fastencode-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 long_description = (this_directory / "README.md").read_text()
 
 
 
 setup(
   name = 'fastencode',         # How you named your package folder (MyLib)
   packages = ['fastencode'],   # Chose the same as "name"
-  version = '1.1',      # Start with a small number and increase it with every change you make
+  version = '1.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'An easy way to use different encoding: bytes, hex, ascii array, binary, long',   # Give a short description about your library
+  description = 'An easy way to use different encoding: bytes, hex, ascii array, binary, long, base64',   # Give a short description about your library
   long_description = long_description,
   long_description_content_type='text/markdown',
   author = 'ES3',                   # Type in your name
   author_email = 'ourteamscare@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/elyassaf/Easy-Encoding/archive/refs/tags/v_1.0.tar.gz',    # I explain this later on
-  keywords = ['encoding', 'hex', 'bytes', 'binary representation', 'decoding', 'ascii'],   # Keywords that define your package best
-  install_requires=['typing'],
+  keywords = ['encoding', 'hex', 'bytes', 'binary representation', 'decoding', 'ascii', 'base64'],   # Keywords that define your package best
+  install_requires=['typing', 'base64'],
   classifiers=[
     'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
@@ -31,8 +31,8 @@
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
   ],
-)
+)
```

