# Comparing `tmp/weallcode_robot-3.0.1.tar.gz` & `tmp/weallcode_robot-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weallcode_robot-3.0.1.tar", max compression
+gzip compressed data, was "weallcode_robot-3.0.2.tar", max compression
```

## Comparing `weallcode_robot-3.0.1.tar` & `weallcode_robot-3.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2245 2023-05-06 02:15:11.930793 weallcode_robot-3.0.1/README.md
--rw-r--r--   0        0        0     1706 2023-05-06 02:15:11.930793 weallcode_robot-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-06 02:15:11.934793 weallcode_robot-3.0.1/weallcode_robot/__init__.py
--rw-r--r--   0        0        0     4724 2023-05-06 02:15:11.934793 weallcode_robot-3.0.1/weallcode_robot/commands.py
--rw-r--r--   0        0        0     3735 2023-05-06 02:15:11.934793 weallcode_robot-3.0.1/weallcode_robot/robot.py
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 weallcode_robot-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2246 2023-05-06 02:25:31.669977 weallcode_robot-3.0.2/README.md
+-rw-r--r--   0        0        0     1312 2023-05-06 02:25:31.669977 weallcode_robot-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-06 02:25:31.669977 weallcode_robot-3.0.2/weallcode_robot/__init__.py
+-rw-r--r--   0        0        0     4724 2023-05-06 02:25:31.669977 weallcode_robot-3.0.2/weallcode_robot/commands.py
+-rw-r--r--   0        0        0     3735 2023-05-06 02:25:31.669977 weallcode_robot-3.0.2/weallcode_robot/robot.py
+-rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 weallcode_robot-3.0.2/PKG-INFO
```

### Comparing `weallcode_robot-3.0.1/README.md` & `weallcode_robot-3.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ```
 
 ## Usage
 
 The `example.py` script demonstrates how to use the package to control the robot.
 
 ```python
-from robot_v2.robot import Robot
+from weallcode_robot import Robot
 
 robot = Robot("WAC")
 
 robot.led(255, 0, 0)        # Set the LED color to red
 robot.move(100, 100)        # Move forward
 robot.wait(2)               # Wait for 2 seconds
 robot.move(0, 0)            # Stop the robot
```

### Comparing `weallcode_robot-3.0.1/pyproject.toml` & `weallcode_robot-3.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,38 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-# [project]
-# name = "weallcode_robot"
-# description = "We All Code Robot Client"
-# readme = "README.md"
-# requires-python = ">=3.7"
-# license = "MIT"
-# authors = [
-#     { name="Ali Karbassi", email="ali@karbassi.com" },
-#     { name="Blaine Rothrock", email="blaine.p.rothrock@gmail.com" },
-# ]
-# classifiers = [
-#     "Development Status :: 4 - Beta",
-#     "License :: OSI Approved :: MIT License",
-#     "Programming Language :: Python",
-#     "Programming Language :: Python :: 3 :: Only",
-#     "Programming Language :: Python :: 3",
-#     "Programming Language :: Python :: 3.4",
-#     "Programming Language :: Python :: 3.5",
-#     "Programming Language :: Python :: 3.6",
-#     "Programming Language :: Python :: 3.7",
-#     "Programming Language :: Python :: 3.8",
-#     "Programming Language :: Python :: 3.9",
-#     "Programming Language :: Python :: 3.10",
-#     "Programming Language :: Python :: 3.11",
-# ]
-# dependencies = [
-#     'bleak>=0.20.1,<0.21.0'
-# ]
-# dynamic = ["version"]
-
-# [project.urls]
-# Homepage = "https://github.com/WeAllCode/tinybit-python"
-# Documentation = "https://github.com/WeAllCode/tinybit-python"
-
 [tool.poetry]
 name = "weallcode_robot"
-version = "3.0.1"
-description = ""
+version = "3.0.2"
+description = "Micro:bit TinyBit BLE Python Library"
+license = "MIT"
 authors = [
     "Blaine Rothrock <blaine.p.rothrock@gmail.com>",
     "Ali Karbassi <ali@weallcode.org>",
 ]
 readme = "README.md"
-license = "MIT"
+homepage = "https://github.com/WeAllCode/tinybit-python"
+repository = "https://github.com/WeAllCode/tinybit-python"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.4",
+    "Programming Language :: Python :: 3.5",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
 packages = [
     { include = "weallcode_robot" },
 ]
 
 [tool.isort]
 profile = "black"
```

### Comparing `weallcode_robot-3.0.1/weallcode_robot/commands.py` & `weallcode_robot-3.0.2/weallcode_robot/commands.py`

 * *Files identical despite different names*

### Comparing `weallcode_robot-3.0.1/weallcode_robot/robot.py` & `weallcode_robot-3.0.2/weallcode_robot/robot.py`

 * *Files identical despite different names*

