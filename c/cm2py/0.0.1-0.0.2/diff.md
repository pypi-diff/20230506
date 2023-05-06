# Comparing `tmp/cm2py-0.0.1.tar.gz` & `tmp/cm2py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.0.1.tar", last modified: Sat May  6 11:05:27 2023, max compression
+gzip compressed data, was "cm2py-0.0.2.tar", last modified: Sat May  6 11:52:18 2023, max compression
```

## Comparing `cm2py-0.0.1.tar` & `cm2py-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:05:27.749041 cm2py-0.0.1/
--rw-rw-rw-   0        0        0    35921 2023-05-06 09:53:00.000000 cm2py-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    43012 2023-05-06 11:05:27.747537 cm2py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1087 2023-05-06 10:42:35.000000 cm2py-0.0.1/README.md
--rw-rw-rw-   0        0        0      709 2023-05-06 09:53:00.000000 cm2py-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 11:05:27.749041 cm2py-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 11:05:27.707789 cm2py-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 11:05:27.721289 cm2py-0.0.1/src/cm2py/
--rw-rw-rw-   0        0        0        0 2023-05-06 09:53:00.000000 cm2py-0.0.1/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     4345 2023-05-06 10:45:34.000000 cm2py-0.0.1/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:05:27.744541 cm2py-0.0.1/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0    43012 2023-05-06 11:05:27.000000 cm2py-0.0.1/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-06 11:05:27.000000 cm2py-0.0.1/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:05:27.000000 cm2py-0.0.1/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-06 11:05:27.000000 cm2py-0.0.1/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 11:05:27.000000 cm2py-0.0.1/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:52:18.351434 cm2py-0.0.2/
+-rw-rw-rw-   0        0        0    35921 2023-05-06 09:53:00.000000 cm2py-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    43012 2023-05-06 11:52:18.349934 cm2py-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1087 2023-05-06 10:42:35.000000 cm2py-0.0.2/README.md
+-rw-rw-rw-   0        0        0      709 2023-05-06 11:51:09.000000 cm2py-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 11:52:18.352184 cm2py-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 11:52:18.242674 cm2py-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:52:18.254675 cm2py-0.0.2/src/cm2py/
+-rw-rw-rw-   0        0        0      128 2023-05-06 11:45:23.000000 cm2py-0.0.2/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     4209 2023-05-06 11:51:04.000000 cm2py-0.0.2/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:52:18.346185 cm2py-0.0.2/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0    43012 2023-05-06 11:52:18.000000 cm2py-0.0.2/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-06 11:52:18.000000 cm2py-0.0.2/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:52:18.000000 cm2py-0.0.2/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-06 11:52:18.000000 cm2py-0.0.2/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 11:52:18.000000 cm2py-0.0.2/src/cm2py.egg-info/top_level.txt
```

### Comparing `cm2py-0.0.1/LICENSE` & `cm2py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.0.1/PKG-INFO` & `cm2py-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEK <qestudios17@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cm2py-0.0.1/README.md` & `cm2py-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cm2py-0.0.1/pyproject.toml` & `cm2py-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="SKM GEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `cm2py-0.0.1/src/cm2py/cm2py.py` & `cm2py-0.0.2/src/cm2py/cm2py.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,32 +22,19 @@
 __copyright__ = "Copyright 2023, SKM GEEK"
 __date__ = "2023/04/29"
 __deprecated__ = False
 __email__ =  "qestudios17@example.com"
 __license__ = "GPLv3"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 
 from uuid import UUID, uuid4
 
-
-
-# Pre-defined blockId definitions"""
-NOR = 0
-AND = 1
-OR = 2
-XOR = 3
-BUTTON = 4
-FLIPFLOP = 5
-LED = 6
-MUSIC = 7
-CLOCK = 8
-
 class save:
     
     def __init__(self):
         self.blocks = []
         self.connections = {}
 
     def addBlock(self, blockId, pos, state=False, snapToGrid=True):
```

### Comparing `cm2py-0.0.1/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.0.2/src/cm2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEK <qestudios17@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

