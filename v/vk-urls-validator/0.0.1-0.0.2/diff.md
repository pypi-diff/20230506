# Comparing `tmp/vk_urls_validator-0.0.1.tar.gz` & `tmp/vk_urls_validator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vk_urls_validator-0.0.1.tar", last modified: Fri May  5 15:36:50 2023, max compression
+gzip compressed data, was "vk_urls_validator-0.0.2.tar", last modified: Sat May  6 12:51:37 2023, max compression
```

## Comparing `vk_urls_validator-0.0.1.tar` & `vk_urls_validator-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 wipedout   (502) staff       (20)        0 2023-05-05 15:36:50.115690 vk_urls_validator-0.0.1/
--rw-r--r--   0 wipedout   (502) staff       (20)    11357 2023-05-05 09:50:05.000000 vk_urls_validator-0.0.1/LICENSE
--rw-r--r--   0 wipedout   (502) staff       (20)     1152 2023-05-05 15:36:50.115573 vk_urls_validator-0.0.1/PKG-INFO
--rw-r--r--   0 wipedout   (502) staff       (20)      490 2023-05-05 15:34:54.000000 vk_urls_validator-0.0.1/README.md
--rw-r--r--   0 wipedout   (502) staff       (20)       38 2023-05-05 15:36:50.115728 vk_urls_validator-0.0.1/setup.cfg
--rw-r--r--   0 wipedout   (502) staff       (20)     1021 2023-05-05 15:36:23.000000 vk_urls_validator-0.0.1/setup.py
-drwxr-xr-x   0 wipedout   (502) staff       (20)        0 2023-05-05 15:36:50.114249 vk_urls_validator-0.0.1/vk_urls_validator/
--rw-r--r--   0 wipedout   (502) staff       (20)       69 2023-05-04 23:04:29.000000 vk_urls_validator-0.0.1/vk_urls_validator/__init__.py
-drwxr-xr-x   0 wipedout   (502) staff       (20)        0 2023-05-05 15:36:50.115301 vk_urls_validator-0.0.1/vk_urls_validator/utils/
--rw-r--r--   0 wipedout   (502) staff       (20)        0 2023-05-04 21:03:33.000000 vk_urls_validator-0.0.1/vk_urls_validator/utils/__init__.py
--rw-r--r--   0 wipedout   (502) staff       (20)      956 2023-05-05 14:45:42.000000 vk_urls_validator-0.0.1/vk_urls_validator/utils/exceptions.py
--rw-r--r--   0 wipedout   (502) staff       (20)     1828 2023-05-05 15:17:24.000000 vk_urls_validator-0.0.1/vk_urls_validator/utils/utils.py
--rw-r--r--   0 wipedout   (502) staff       (20)     1178 2023-05-05 15:34:54.000000 vk_urls_validator-0.0.1/vk_urls_validator/validator.py
-drwxr-xr-x   0 wipedout   (502) staff       (20)        0 2023-05-05 15:36:50.114809 vk_urls_validator-0.0.1/vk_urls_validator.egg-info/
--rw-r--r--   0 wipedout   (502) staff       (20)     1152 2023-05-05 15:36:50.000000 vk_urls_validator-0.0.1/vk_urls_validator.egg-info/PKG-INFO
--rw-r--r--   0 wipedout   (502) staff       (20)      358 2023-05-05 15:36:50.000000 vk_urls_validator-0.0.1/vk_urls_validator.egg-info/SOURCES.txt
--rw-r--r--   0 wipedout   (502) staff       (20)        1 2023-05-05 15:36:50.000000 vk_urls_validator-0.0.1/vk_urls_validator.egg-info/dependency_links.txt
--rw-r--r--   0 wipedout   (502) staff       (20)       18 2023-05-05 15:36:50.000000 vk_urls_validator-0.0.1/vk_urls_validator.egg-info/top_level.txt
+drwxr-xr-x   0 wipedout   (502) staff       (20)        0 2023-05-06 12:51:37.012032 vk_urls_validator-0.0.2/
+-rw-r--r--   0 wipedout   (502) staff       (20)    11357 2023-05-06 12:47:45.000000 vk_urls_validator-0.0.2/LICENSE
+-rw-r--r--   0 wipedout   (502) staff       (20)     1152 2023-05-06 12:51:37.011920 vk_urls_validator-0.0.2/PKG-INFO
+-rw-r--r--   0 wipedout   (502) staff       (20)      490 2023-05-06 12:47:45.000000 vk_urls_validator-0.0.2/README.md
+-rw-r--r--   0 wipedout   (502) staff       (20)       38 2023-05-06 12:51:37.012076 vk_urls_validator-0.0.2/setup.cfg
+-rw-r--r--   0 wipedout   (502) staff       (20)     1021 2023-05-06 12:49:58.000000 vk_urls_validator-0.0.2/setup.py
+drwxr-xr-x   0 wipedout   (502) staff       (20)        0 2023-05-06 12:51:37.010745 vk_urls_validator-0.0.2/vk_urls_validator/
+-rw-r--r--   0 wipedout   (502) staff       (20)       69 2023-05-06 12:47:45.000000 vk_urls_validator-0.0.2/vk_urls_validator/__init__.py
+-rw-r--r--   0 wipedout   (502) staff       (20)       81 2023-05-06 12:49:04.000000 vk_urls_validator-0.0.2/vk_urls_validator/a.py
+drwxr-xr-x   0 wipedout   (502) staff       (20)        0 2023-05-06 12:51:37.011647 vk_urls_validator-0.0.2/vk_urls_validator/utils/
+-rw-r--r--   0 wipedout   (502) staff       (20)        0 2023-05-06 12:47:45.000000 vk_urls_validator-0.0.2/vk_urls_validator/utils/__init__.py
+-rw-r--r--   0 wipedout   (502) staff       (20)      956 2023-05-06 12:47:45.000000 vk_urls_validator-0.0.2/vk_urls_validator/utils/exceptions.py
+-rw-r--r--   0 wipedout   (502) staff       (20)     1829 2023-05-06 12:49:45.000000 vk_urls_validator-0.0.2/vk_urls_validator/utils/utils.py
+-rw-r--r--   0 wipedout   (502) staff       (20)     1178 2023-05-06 12:47:45.000000 vk_urls_validator-0.0.2/vk_urls_validator/validator.py
+drwxr-xr-x   0 wipedout   (502) staff       (20)        0 2023-05-06 12:51:37.011252 vk_urls_validator-0.0.2/vk_urls_validator.egg-info/
+-rw-r--r--   0 wipedout   (502) staff       (20)     1152 2023-05-06 12:51:36.000000 vk_urls_validator-0.0.2/vk_urls_validator.egg-info/PKG-INFO
+-rw-r--r--   0 wipedout   (502) staff       (20)      381 2023-05-06 12:51:36.000000 vk_urls_validator-0.0.2/vk_urls_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 wipedout   (502) staff       (20)        1 2023-05-06 12:51:36.000000 vk_urls_validator-0.0.2/vk_urls_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 wipedout   (502) staff       (20)       18 2023-05-06 12:51:36.000000 vk_urls_validator-0.0.2/vk_urls_validator.egg-info/top_level.txt
```

### Comparing `vk_urls_validator-0.0.1/LICENSE` & `vk_urls_validator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vk_urls_validator-0.0.1/PKG-INFO` & `vk_urls_validator-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vk_urls_validator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Validator for VK URLs.
 Home-page: https://github.com/Wiped-Out/vk_urls_validator
 Download-URL: https://github.com/Wiped-Out/vk_urls_validator/releases/latest
 Author: Emir Takhaviev
 Author-email: tah116emir@outlook.com
 Keywords: python,vk urls,validation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vk_urls_validator-0.0.1/setup.py` & `vk_urls_validator-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Validator for VK URLs.'
 
 # Setting up
 setup(
     name="vk_urls_validator",
     version=VERSION,
     author="Emir Takhaviev",
```

### Comparing `vk_urls_validator-0.0.1/vk_urls_validator/utils/exceptions.py` & `vk_urls_validator-0.0.2/vk_urls_validator/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vk_urls_validator-0.0.1/vk_urls_validator/utils/utils.py` & `vk_urls_validator-0.0.2/vk_urls_validator/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional
 
 from vk_urls_validator.utils import exceptions
 import string
 
-ALLOWED_CHARACTERS = string.digits + string.ascii_uppercase + string.ascii_lowercase + '.'
+ALLOWED_CHARACTERS = string.digits + string.ascii_uppercase + string.ascii_lowercase + '._'
 
 
 def get_hostname(hostname: str, hostnames: List[str]) -> Optional[str]:
     for prefix in hostnames:
         if hostname.startswith(prefix):
             return prefix
     return None
```

### Comparing `vk_urls_validator-0.0.1/vk_urls_validator/validator.py` & `vk_urls_validator-0.0.2/vk_urls_validator/validator.py`

 * *Files identical despite different names*

### Comparing `vk_urls_validator-0.0.1/vk_urls_validator.egg-info/PKG-INFO` & `vk_urls_validator-0.0.2/vk_urls_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vk-urls-validator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Validator for VK URLs.
 Home-page: https://github.com/Wiped-Out/vk_urls_validator
 Download-URL: https://github.com/Wiped-Out/vk_urls_validator/releases/latest
 Author: Emir Takhaviev
 Author-email: tah116emir@outlook.com
 Keywords: python,vk urls,validation
 Classifier: Development Status :: 3 - Alpha
```

