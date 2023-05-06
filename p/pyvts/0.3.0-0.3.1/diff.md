# Comparing `tmp/pyvts-0.3.0.tar.gz` & `tmp/pyvts-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvts-0.3.0.tar", last modified: Fri Apr 14 16:34:24 2023, max compression
+gzip compressed data, was "pyvts-0.3.1.tar", last modified: Sat May  6 21:28:54 2023, max compression
```

## Comparing `pyvts-0.3.0.tar` & `pyvts-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 16:34:24.933472 pyvts-0.3.0/
--rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.3.0/LICENSE
--rw-r--r--   0 genteki    (501) staff       (20)     2855 2023-04-14 16:34:24.933301 pyvts-0.3.0/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)     2010 2023-04-14 16:32:53.000000 pyvts-0.3.0/README.md
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 16:34:24.930720 pyvts-0.3.0/pyvts/
--rw-r--r--   0 genteki    (501) staff       (20)      216 2023-04-14 16:32:53.000000 pyvts-0.3.0/pyvts/__init__.py
--rw-r--r--   0 genteki    (501) staff       (20)      264 2023-04-14 16:32:53.000000 pyvts-0.3.0/pyvts/config.py
--rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.3.0/pyvts/error.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 16:34:24.932625 pyvts-0.3.0/pyvts/tests/
--rw-r--r--   0 genteki    (501) staff       (20)        0 2023-02-28 10:07:07.000000 pyvts-0.3.0/pyvts/tests/__init__.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 16:34:24.933061 pyvts-0.3.0/pyvts/tests/integration/
--rw-r--r--   0 genteki    (501) staff       (20)        0 2023-03-02 07:55:23.000000 pyvts-0.3.0/pyvts/tests/integration/__init__.py
--rw-r--r--   0 genteki    (501) staff       (20)      864 2023-03-02 20:34:19.000000 pyvts-0.3.0/pyvts/tests/integration/test_integration.py
--rw-r--r--   0 genteki    (501) staff       (20)     4448 2023-03-26 06:13:29.000000 pyvts-0.3.0/pyvts/tests/test_utils.py
--rw-r--r--   0 genteki    (501) staff       (20)     4207 2023-04-10 05:03:27.000000 pyvts-0.3.0/pyvts/tests/test_vts.py
--rw-r--r--   0 genteki    (501) staff       (20)      477 2023-03-25 05:41:19.000000 pyvts-0.3.0/pyvts/tests/test_vts_request.py
--rw-r--r--   0 genteki    (501) staff       (20)     6349 2023-04-11 05:55:48.000000 pyvts-0.3.0/pyvts/vts.py
--rw-r--r--   0 genteki    (501) staff       (20)    10126 2023-04-14 16:32:53.000000 pyvts-0.3.0/pyvts/vts_request.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 16:34:24.931861 pyvts-0.3.0/pyvts.egg-info/
--rw-r--r--   0 genteki    (501) staff       (20)     2855 2023-04-14 16:34:24.000000 pyvts-0.3.0/pyvts.egg-info/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)      439 2023-04-14 16:34:24.000000 pyvts-0.3.0/pyvts.egg-info/SOURCES.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-14 16:34:24.000000 pyvts-0.3.0/pyvts.egg-info/dependency_links.txt
--rw-r--r--   0 genteki    (501) staff       (20)       20 2023-04-14 16:34:24.000000 pyvts-0.3.0/pyvts.egg-info/requires.txt
--rw-r--r--   0 genteki    (501) staff       (20)        6 2023-04-14 16:34:24.000000 pyvts-0.3.0/pyvts.egg-info/top_level.txt
--rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-14 16:34:24.933524 pyvts-0.3.0/setup.cfg
--rw-r--r--   0 genteki    (501) staff       (20)     1208 2023-04-14 16:32:53.000000 pyvts-0.3.0/setup.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-05-06 21:28:54.060842 pyvts-0.3.1/
+-rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.3.1/LICENSE
+-rw-r--r--   0 genteki    (501) staff       (20)     2650 2023-05-06 21:28:54.060714 pyvts-0.3.1/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)     1792 2023-05-06 21:24:20.000000 pyvts-0.3.1/README.md
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-05-06 21:28:54.059262 pyvts-0.3.1/pyvts/
+-rw-r--r--   0 genteki    (501) staff       (20)      216 2023-05-06 21:28:46.000000 pyvts-0.3.1/pyvts/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      264 2023-04-14 16:32:53.000000 pyvts-0.3.1/pyvts/config.py
+-rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.3.1/pyvts/error.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-05-06 21:28:54.060323 pyvts-0.3.1/pyvts/tests/
+-rw-r--r--   0 genteki    (501) staff       (20)        0 2023-02-28 10:07:07.000000 pyvts-0.3.1/pyvts/tests/__init__.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-05-06 21:28:54.060524 pyvts-0.3.1/pyvts/tests/integration/
+-rw-r--r--   0 genteki    (501) staff       (20)        0 2023-03-02 07:55:23.000000 pyvts-0.3.1/pyvts/tests/integration/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      864 2023-03-02 20:34:19.000000 pyvts-0.3.1/pyvts/tests/integration/test_integration.py
+-rw-r--r--   0 genteki    (501) staff       (20)     4448 2023-03-26 06:13:29.000000 pyvts-0.3.1/pyvts/tests/test_utils.py
+-rw-r--r--   0 genteki    (501) staff       (20)     4207 2023-04-10 05:03:27.000000 pyvts-0.3.1/pyvts/tests/test_vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)      477 2023-03-25 05:41:19.000000 pyvts-0.3.1/pyvts/tests/test_vts_request.py
+-rw-r--r--   0 genteki    (501) staff       (20)     6349 2023-04-11 05:55:48.000000 pyvts-0.3.1/pyvts/vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)    10126 2023-04-14 16:32:53.000000 pyvts-0.3.1/pyvts/vts_request.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-05-06 21:28:54.059848 pyvts-0.3.1/pyvts.egg-info/
+-rw-r--r--   0 genteki    (501) staff       (20)     2650 2023-05-06 21:28:54.000000 pyvts-0.3.1/pyvts.egg-info/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)      439 2023-05-06 21:28:54.000000 pyvts-0.3.1/pyvts.egg-info/SOURCES.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-05-06 21:28:54.000000 pyvts-0.3.1/pyvts.egg-info/dependency_links.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       20 2023-05-06 21:28:54.000000 pyvts-0.3.1/pyvts.egg-info/requires.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        6 2023-05-06 21:28:54.000000 pyvts-0.3.1/pyvts.egg-info/top_level.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       38 2023-05-06 21:28:54.060881 pyvts-0.3.1/setup.cfg
+-rw-r--r--   0 genteki    (501) staff       (20)     1221 2023-05-06 21:28:46.000000 pyvts-0.3.1/setup.py
```

### Comparing `pyvts-0.3.0/LICENSE` & `pyvts-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvts-0.3.0/PKG-INFO` & `pyvts-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,73 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyvts
+
 [![License: MIT](https://img.shields.io/github/license/Genteki/pyvts?style=flat-square)](https://opensource.org/licenses/MIT) [![issue](https://img.shields.io/github/issues/genteki/pyvts?style=flat-square)](https://github.com/Genteki/pyvts/issues) [![build](https://img.shields.io/circleci/build/github/Genteki/pyvts?style=flat-square)](https://circleci.com/gh/Genteki/pyvts)
 [![codecov](https://img.shields.io/codecov/c/github/genteki/pyvts?color=informational&style=flat-square)](https://codecov.io/gh/Genteki/pyvts)
 [![PyPI](https://img.shields.io/pypi/v/pyvts?style=flat-square)](https://pypi.org/project/pyvts/)
 [![docs](https://img.shields.io/badge/docs-passing-success?style=flat-square)](https://genteki.github.io/pyvts)
 
 A python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
 ## Overview
+
 `pyvts` is a python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
 You can easily use the library to develop VTubeStudio Plugin to achieve your goals. For example, adding new tracking parameters to enable more actions on live2d avatars.
 
 ## Quick Start
 
 ### Installation
 
-```
+```shell
 pip3 install pyvts 
 ```
 
 ### Get Started
 
 First import library you need,
-```
+
+```python
 import pyvts
 import asyncio
 ```
 
 Create an instance with default values, and do whateveer you want!
-```
+
+```python
 async def main():
     vts = pyvts.vts()
     await vts.connect()
     # Implement what you want to do
     await vts.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
-### Demo
+To see more examples, you could visit [tutorial](https://genteki.github.io/pyvts/toctree2_tutorial.html) in documentation.
 
-Demo [examples/start.py](./examples/start.py) is a good startpoint to make plugin for VTubeStudio. 
-
-Before you get started, make sure you've clone the library and installed all the dependcies
-
-```
-pip3 install -r requirements.txt 
-```
-
-Then, launch `VTubeStudio`, and run
-
-``` 
-python3 examples/start.py 
-```
+### Contributing
 
-in command line. You will see a new tracking parameter "start_parameter" added to VTubeStudio and some information about it in command line ouput.
+Contribution is welcome. Please follow the guide of [CONTRIBUING.md](CONTRIBUTING.md).
```

### Comparing `pyvts-0.3.0/README.md` & `pyvts-0.3.1/pyvts.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,73 @@
+Metadata-Version: 2.1
+Name: pyvts
+Version: 0.3.1
+Summary: A python library for interacting with the VTube Studio API
+Home-page: https://github.com/Genteki/pyvts
+Author: Genteki Zhang
+Author-email: zhangkaiyuan.null@gmail.com
+License: MIT
+Keywords: vtubestudio
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyvts
+
 [![License: MIT](https://img.shields.io/github/license/Genteki/pyvts?style=flat-square)](https://opensource.org/licenses/MIT) [![issue](https://img.shields.io/github/issues/genteki/pyvts?style=flat-square)](https://github.com/Genteki/pyvts/issues) [![build](https://img.shields.io/circleci/build/github/Genteki/pyvts?style=flat-square)](https://circleci.com/gh/Genteki/pyvts)
 [![codecov](https://img.shields.io/codecov/c/github/genteki/pyvts?color=informational&style=flat-square)](https://codecov.io/gh/Genteki/pyvts)
 [![PyPI](https://img.shields.io/pypi/v/pyvts?style=flat-square)](https://pypi.org/project/pyvts/)
 [![docs](https://img.shields.io/badge/docs-passing-success?style=flat-square)](https://genteki.github.io/pyvts)
 
 A python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
 ## Overview
+
 `pyvts` is a python library for interacting with the [VTube Studio API](https://github.com/DenchiSoft/VTubeStudio).
 
 You can easily use the library to develop VTubeStudio Plugin to achieve your goals. For example, adding new tracking parameters to enable more actions on live2d avatars.
 
 ## Quick Start
 
 ### Installation
 
-```
+```shell
 pip3 install pyvts 
 ```
 
 ### Get Started
 
 First import library you need,
-```
+
+```python
 import pyvts
 import asyncio
 ```
 
 Create an instance with default values, and do whateveer you want!
-```
+
+```python
 async def main():
     vts = pyvts.vts()
     await vts.connect()
     # Implement what you want to do
     await vts.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
-### Demo
+To see more examples, you could visit [tutorial](https://genteki.github.io/pyvts/toctree2_tutorial.html) in documentation.
 
-Demo [examples/start.py](./examples/start.py) is a good startpoint to make plugin for VTubeStudio. 
-
-Before you get started, make sure you've clone the library and installed all the dependcies
-
-```
-pip3 install -r requirements.txt 
-```
-
-Then, launch `VTubeStudio`, and run
-
-``` 
-python3 examples/start.py 
-```
+### Contributing
 
-in command line. You will see a new tracking parameter "start_parameter" added to VTubeStudio and some information about it in command line ouput.
+Contribution is welcome. Please follow the guide of [CONTRIBUING.md](CONTRIBUTING.md).
```

### Comparing `pyvts-0.3.0/pyvts/tests/integration/test_integration.py` & `pyvts-0.3.1/pyvts/tests/integration/test_integration.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.3.0/pyvts/tests/test_utils.py` & `pyvts-0.3.1/pyvts/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.3.0/pyvts/tests/test_vts.py` & `pyvts-0.3.1/pyvts/tests/test_vts.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.3.0/pyvts/vts.py` & `pyvts-0.3.1/pyvts/vts.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.3.0/pyvts/vts_request.py` & `pyvts-0.3.1/pyvts/vts_request.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.3.0/setup.py` & `pyvts-0.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """A python library for interacting with the VTube Studio API"""
 
 from setuptools import setup, find_packages
 
 DESCRIPTION = "A python library for interacting with the VTube Studio API"
-VERSION = "v0.3.0"
+VERSION = "v0.3.1"
 
 setup(
     name="pyvts",
     version=VERSION,
     description=DESCRIPTION,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="vtubestudio",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

