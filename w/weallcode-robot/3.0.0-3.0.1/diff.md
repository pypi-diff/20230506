# Comparing `tmp/weallcode_robot-3.0.0.tar.gz` & `tmp/weallcode_robot-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weallcode_robot-3.0.0.tar", last modified: Sat Apr  8 14:27:17 2023, max compression
+gzip compressed data, was "weallcode_robot-3.0.1.tar", max compression
```

## Comparing `weallcode_robot-3.0.0.tar` & `weallcode_robot-3.0.1.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxr-xr-x   0 danielmconrad   (501) staff       (20)        0 2023-04-08 14:27:17.513181 weallcode_robot-3.0.0/
--rw-r--r--   0 danielmconrad   (501) staff       (20)     2932 2023-04-08 14:27:17.512833 weallcode_robot-3.0.0/PKG-INFO
--rw-r--r--   0 danielmconrad   (501) staff       (20)     2245 2023-04-08 14:21:45.000000 weallcode_robot-3.0.0/README.md
--rw-r--r--   0 danielmconrad   (501) staff       (20)      489 2023-04-08 14:21:45.000000 weallcode_robot-3.0.0/pyproject.toml
--rw-r--r--   0 danielmconrad   (501) staff       (20)       38 2023-04-08 14:27:17.513308 weallcode_robot-3.0.0/setup.cfg
--rw-r--r--   0 danielmconrad   (501) staff       (20)     1166 2023-04-08 14:23:11.000000 weallcode_robot-3.0.0/setup.py
-drwxr-xr-x   0 danielmconrad   (501) staff       (20)        0 2023-04-08 14:27:17.509286 weallcode_robot-3.0.0/weallcode_robot/
--rw-r--r--   0 danielmconrad   (501) staff       (20)      217 2023-04-08 14:27:10.000000 weallcode_robot-3.0.0/weallcode_robot/__init__.py
--rw-r--r--   0 danielmconrad   (501) staff       (20)     4724 2023-04-08 14:23:11.000000 weallcode_robot-3.0.0/weallcode_robot/commands.py
--rw-r--r--   0 danielmconrad   (501) staff       (20)     3649 2023-04-08 14:27:10.000000 weallcode_robot-3.0.0/weallcode_robot/robot.py
-drwxr-xr-x   0 danielmconrad   (501) staff       (20)        0 2023-04-08 14:27:17.512149 weallcode_robot-3.0.0/weallcode_robot.egg-info/
--rw-r--r--   0 danielmconrad   (501) staff       (20)     2932 2023-04-08 14:27:17.000000 weallcode_robot-3.0.0/weallcode_robot.egg-info/PKG-INFO
--rw-r--r--   0 danielmconrad   (501) staff       (20)      308 2023-04-08 14:27:17.000000 weallcode_robot-3.0.0/weallcode_robot.egg-info/SOURCES.txt
--rw-r--r--   0 danielmconrad   (501) staff       (20)        1 2023-04-08 14:27:17.000000 weallcode_robot-3.0.0/weallcode_robot.egg-info/dependency_links.txt
--rw-r--r--   0 danielmconrad   (501) staff       (20)        6 2023-04-08 14:27:17.000000 weallcode_robot-3.0.0/weallcode_robot.egg-info/requires.txt
--rw-r--r--   0 danielmconrad   (501) staff       (20)       16 2023-04-08 14:27:17.000000 weallcode_robot-3.0.0/weallcode_robot.egg-info/top_level.txt
+-rw-r--r--   0        0        0     2245 2023-05-06 02:15:11.930793 weallcode_robot-3.0.1/README.md
+-rw-r--r--   0        0        0     1706 2023-05-06 02:15:11.930793 weallcode_robot-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-06 02:15:11.934793 weallcode_robot-3.0.1/weallcode_robot/__init__.py
+-rw-r--r--   0        0        0     4724 2023-05-06 02:15:11.934793 weallcode_robot-3.0.1/weallcode_robot/commands.py
+-rw-r--r--   0        0        0     3735 2023-05-06 02:15:11.934793 weallcode_robot-3.0.1/weallcode_robot/robot.py
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 weallcode_robot-3.0.1/PKG-INFO
```

### Comparing `weallcode_robot-3.0.0/PKG-INFO` & `weallcode_robot-3.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
-Name: weallcode_robot
-Version: 3.0.0
-Summary: We All Code Robot Client
-Home-page: https://github.com/weallcode/robot
-Author: We All Code
-Author-email: hello@weallcode.org
+Name: weallcode-robot
+Version: 3.0.1
+Summary: 
 License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
+Author: Blaine Rothrock
+Author-email: blaine.p.rothrock@gmail.com
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bleak (>=0.20.1,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Micro:bit TinyBit BLE Python Library
 
 A Python package to control a custom Robot V2 via Bluetooth Low Energy (BLE) communication. The package provides an API for controlling the robot's movements and LED colors.
 
 ## Installation
@@ -102,7 +97,8 @@
 pre-commit run --all-files
 ```
 
 ## Authors
 
 - Blaine Rothrock
 - Ali Karbassi
+
```

### Comparing `weallcode_robot-3.0.0/README.md` & `weallcode_robot-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `weallcode_robot-3.0.0/setup.py` & `weallcode_robot-3.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,64 @@
-import io, os, re
-from setuptools import setup
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
-def read(filename):
-    filename = os.path.join(os.path.dirname(__file__), filename)
-    text_type = type(u"")
-    with io.open(filename, mode="r", encoding='utf-8') as fd:
-        return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
-
-setup(
-   name="weallcode_robot",
-    version="3.0.0",
-    url="https://github.com/weallcode/robot",
-    license='MIT',
-
-    author="We All Code",
-    author_email="hello@weallcode.org",
-    
-    description="We All Code Robot Client",
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-
-    packages=["weallcode_robot"],
-    install_requires=["bleak"],
-    
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-    ],
-)
+# [project]
+# name = "weallcode_robot"
+# description = "We All Code Robot Client"
+# readme = "README.md"
+# requires-python = ">=3.7"
+# license = "MIT"
+# authors = [
+#     { name="Ali Karbassi", email="ali@karbassi.com" },
+#     { name="Blaine Rothrock", email="blaine.p.rothrock@gmail.com" },
+# ]
+# classifiers = [
+#     "Development Status :: 4 - Beta",
+#     "License :: OSI Approved :: MIT License",
+#     "Programming Language :: Python",
+#     "Programming Language :: Python :: 3 :: Only",
+#     "Programming Language :: Python :: 3",
+#     "Programming Language :: Python :: 3.4",
+#     "Programming Language :: Python :: 3.5",
+#     "Programming Language :: Python :: 3.6",
+#     "Programming Language :: Python :: 3.7",
+#     "Programming Language :: Python :: 3.8",
+#     "Programming Language :: Python :: 3.9",
+#     "Programming Language :: Python :: 3.10",
+#     "Programming Language :: Python :: 3.11",
+# ]
+# dependencies = [
+#     'bleak>=0.20.1,<0.21.0'
+# ]
+# dynamic = ["version"]
+
+# [project.urls]
+# Homepage = "https://github.com/WeAllCode/tinybit-python"
+# Documentation = "https://github.com/WeAllCode/tinybit-python"
+
+[tool.poetry]
+name = "weallcode_robot"
+version = "3.0.1"
+description = ""
+authors = [
+    "Blaine Rothrock <blaine.p.rothrock@gmail.com>",
+    "Ali Karbassi <ali@weallcode.org>",
+]
+readme = "README.md"
+license = "MIT"
+packages = [
+    { include = "weallcode_robot" },
+]
+
+[tool.isort]
+profile = "black"
+
+[tool.poetry.dependencies]
+python = "^3.11"
+bleak = "^0.20.1"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pre-commit = "^3.2.1"
+isort = "^5.12.0"
+ruff = "^0.0.260"
```

### Comparing `weallcode_robot-3.0.0/weallcode_robot/commands.py` & `weallcode_robot-3.0.1/weallcode_robot/commands.py`

 * *Files identical despite different names*

### Comparing `weallcode_robot-3.0.0/weallcode_robot/robot.py` & `weallcode_robot-3.0.1/weallcode_robot/robot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 import asyncio
-import json
 import logging
 
 from bleak import BleakClient, BleakScanner
 
 from .commands import (
     BuzzerCommand,
     DisplayDotMatrixCommand,
     DisplayTextCommand,
     LEDCommand,
     MoveCommand,
     WaitCommand,
 )
 
 device_name_map = {
-  "beep": "WAC-2463",
-  "boop": "WAC-7F36",
-  "buzz": "WAC-98CE",
-  "bzzt": "WAC-D329",
-  "chirp": "WAC-1A74",
-  "click": "WAC-27B7",
-  "clonk": "WAC-9776",
-  "clunk": "WAC-7740",
-  "crash": "WAC-22F2",
-  "dink": "WAC-6BC7",
-  "doot": "WAC-47F1",
-  "fizz": "WAC-121A",
-  "honk": "WAC-5613",
-  "hoot": "WAC-9717",
-  "jolt": "WAC-A466",
-  "noot": "WAC-EC1C",
-  "oink": "",
-  "pew": "",
-  "ping": "",
-  "pong": "",
-  "pop": "",
-  "pow": "",
-  "purr": "",
-  "quark": "",
-  "ring": "",
-  "roar": "",
-  "sigh": "",
-  "snip": "",
-  "sput": "",
-  "swsh": "",
-  "tape": "",
-  "thud": "",
-  "thum": "",
-  "tik": "",
-  "tok": "",
-  "tong": "",
-  "vroom": "",
-  "whim": "",
-  "whir": "",
-  "whiz": "",
-  "whoop": "",
-  "whum": "",
-  "wizz": "",
-  "wow": "",
-  "yip": "",
-  "zap": "",
-  "zip": "",
-  "zot": ""
+    "beep": "WAC-2463",
+    "boop": "WAC-7F36",
+    "buzz": "WAC-98CE",
+    "bzzt": "WAC-D329",
+    "chirp": "WAC-1A74",
+    "click": "WAC-27B7",
+    "clonk": "WAC-9776",
+    "clunk": "WAC-7740",
+    "crash": "WAC-22F2",
+    "dink": "WAC-6BC7",
+    "doot": "WAC-47F1",
+    "fizz": "WAC-121A",
+    "honk": "WAC-5613",
+    "hoot": "WAC-9717",
+    "jolt": "WAC-A466",
+    "noot": "WAC-EC1C",
+    "oink": "",
+    "pew": "",
+    "ping": "",
+    "pong": "",
+    "pop": "",
+    "pow": "",
+    "purr": "",
+    "quark": "",
+    "ring": "",
+    "roar": "",
+    "sigh": "",
+    "snip": "",
+    "sput": "",
+    "swsh": "",
+    "tape": "",
+    "thud": "",
+    "thum": "",
+    "tik": "",
+    "tok": "",
+    "tong": "",
+    "vroom": "",
+    "whim": "",
+    "whir": "",
+    "whiz": "",
+    "whoop": "",
+    "whum": "",
+    "wizz": "",
+    "wow": "",
+    "yip": "",
+    "zap": "",
+    "zip": "",
+    "zot": "",
 }
 
+
 class Robot:
     def __init__(self, name, debug=False, scan_timeout=2.0):
         self.name = name.lower()
         self.commands = []
         self.scan_timeout = scan_timeout
 
         self.device_map = device_name_map
```

