# Comparing `tmp/CreateAI-0.8.tar.gz` & `tmp/CreateAI-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CreateAI-0.8.tar", last modified: Fri May  5 14:58:40 2023, max compression
+gzip compressed data, was "CreateAI-0.8.1.tar", last modified: Sat May  6 04:23:14 2023, max compression
```

## Comparing `CreateAI-0.8.tar` & `CreateAI-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:40.931055 CreateAI-0.8/
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:40.918056 CreateAI-0.8/CreateAI/
--rw-rw-rw-   0        0        0     4394 2023-05-05 14:46:47.000000 CreateAI-0.8/CreateAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:58:40.930056 CreateAI-0.8/CreateAI.egg-info/
--rw-rw-rw-   0        0        0     1730 2023-05-05 14:58:40.000000 CreateAI-0.8/CreateAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-05 14:58:40.000000 CreateAI-0.8/CreateAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:58:40.000000 CreateAI-0.8/CreateAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 14:58:40.000000 CreateAI-0.8/CreateAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1097 2023-05-05 14:50:25.000000 CreateAI-0.8/LICENCE
--rw-rw-rw-   0        0        0       18 2023-05-05 14:58:40.000000 CreateAI-0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1730 2023-05-05 14:58:40.932054 CreateAI-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2023-05-05 14:36:12.000000 CreateAI-0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 14:58:40.933056 CreateAI-0.8/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-05-05 14:58:40.000000 CreateAI-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:23:14.216918 CreateAI-0.8.1/
+drwxrwxrwx   0        0        0        0 2023-05-06 04:23:14.198917 CreateAI-0.8.1/CreateAI/
+-rw-rw-rw-   0        0        0     4394 2023-05-05 15:01:45.000000 CreateAI-0.8.1/CreateAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:23:14.214914 CreateAI-0.8.1/CreateAI.egg-info/
+-rw-rw-rw-   0        0        0     1816 2023-05-06 04:23:14.000000 CreateAI-0.8.1/CreateAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-06 04:23:14.000000 CreateAI-0.8.1/CreateAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 04:23:14.000000 CreateAI-0.8.1/CreateAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 04:23:14.000000 CreateAI-0.8.1/CreateAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1097 2023-05-05 14:50:25.000000 CreateAI-0.8.1/LICENCE
+-rw-rw-rw-   0        0        0       18 2023-05-06 04:23:13.000000 CreateAI-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1816 2023-05-06 04:23:14.217916 CreateAI-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1371 2023-05-05 16:57:35.000000 CreateAI-0.8.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 04:23:14.219918 CreateAI-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-05-06 04:23:13.000000 CreateAI-0.8.1/setup.py
```

### Comparing `CreateAI-0.8/CreateAI/__init__.py` & `CreateAI-0.8.1/CreateAI/__init__.py`

 * *Files identical despite different names*

### Comparing `CreateAI-0.8/CreateAI.egg-info/PKG-INFO` & `CreateAI-0.8.1/CreateAI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: CreateAI
-Version: 0.8
-Summary: Easy tool for creating ai in python
+Version: 0.8.1
+Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
-# Create AI
+# CreateAI
 It's easy tool to create ai in python easy and fast.
+You can edit code of CreateAI on my [github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
@@ -34,25 +35,25 @@
 
 ## Installation
 
 Install my-project with pip
 
 Windows:
 ```bash
-pip install createai
+pip install СreateAI
 ```
 
 MacOS:
 ```bash
-pip3 install createai
+pip3 install СreateAI
 ```
 
 Linux:
 ```bash
-sudo pip install createai
+sudo pip install СreateAI
 ```
 
 ## Example
 ```python
 from CreateAI import *
 """
 inputs - create inputs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CreateAI-0.8/LICENCE` & `CreateAI-0.8.1/LICENCE`

 * *Files identical despite different names*

### Comparing `CreateAI-0.8/PKG-INFO` & `CreateAI-0.8.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: CreateAI
-Version: 0.8
-Summary: Easy tool for creating ai in python
+Version: 0.8.1
+Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
-# Create AI
+# CreateAI
 It's easy tool to create ai in python easy and fast.
+You can edit code of CreateAI on my [github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
@@ -34,25 +35,25 @@
 
 ## Installation
 
 Install my-project with pip
 
 Windows:
 ```bash
-pip install createai
+pip install СreateAI
 ```
 
 MacOS:
 ```bash
-pip3 install createai
+pip3 install СreateAI
 ```
 
 Linux:
 ```bash
-sudo pip install createai
+sudo pip install СreateAI
 ```
 
 ## Example
 ```python
 from CreateAI import *
 """
 inputs - create inputs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CreateAI-0.8/README.md` & `CreateAI-0.8.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
-# Create AI
+# CreateAI
 It's easy tool to create ai in python easy and fast.
+You can edit code of CreateAI on my [github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
@@ -20,25 +21,25 @@
 
 ## Installation
 
 Install my-project with pip
 
 Windows:
 ```bash
-pip install createai
+pip install СreateAI
 ```
 
 MacOS:
 ```bash
-pip3 install createai
+pip3 install СreateAI
 ```
 
 Linux:
 ```bash
-sudo pip install createai
+sudo pip install СreateAI
 ```
 
 ## Example
 ```python
 from CreateAI import *
 """
 inputs - create inputs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CreateAI-0.8/setup.py` & `CreateAI-0.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 with open(r'C:\MyUse\code\python\EasyPack\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='CreateAI',
-	version='0.8',
+	version='0.8.1',
 	author='R0fael',
 	author_email='roslobodchikov@gmail.com',
-	description='Easy tool for creating ai in python',
+	description='Easy tool for creating AI in python',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/R0fael/CreateAI',
 	packages=['CreateAI'],
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
```

