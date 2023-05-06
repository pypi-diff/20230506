# Comparing `tmp/docker-sand-0.0.5.tar.gz` & `tmp/docker-sand-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-sand-0.0.5.tar", last modified: Sat May  6 16:51:06 2023, max compression
+gzip compressed data, was "docker-sand-0.0.6.tar", last modified: Sat May  6 17:14:19 2023, max compression
```

## Comparing `docker-sand-0.0.5.tar` & `docker-sand-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.674926 docker-sand-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-06 16:51:05.000000 docker-sand-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-06 16:51:06.674926 docker-sand-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-06 16:51:05.000000 docker-sand-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.670926 docker-sand-0.0.5/docker_sand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.674926 docker-sand-0.0.5/sand/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.674926 docker-sand-0.0.5/sand/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.674926 docker-sand-0.0.5/sand/internal/sandfile_executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/sandfile_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/sandfile_executor/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/sandfile_executor/sandfile_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/sandfile_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/sand.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:51:06.674926 docker-sand-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-06 16:51:05.000000 docker-sand-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:14:19.174820 docker-sand-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-06 17:14:16.000000 docker-sand-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-06 17:14:19.174820 docker-sand-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-06 17:14:16.000000 docker-sand-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:14:19.170820 docker-sand-0.0.6/docker_sand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-06 17:14:18.000000 docker-sand-0.0.6/docker_sand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-06 17:14:19.000000 docker-sand-0.0.6/docker_sand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 17:14:18.000000 docker-sand-0.0.6/docker_sand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 17:14:18.000000 docker-sand-0.0.6/docker_sand.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 17:14:18.000000 docker-sand-0.0.6/docker_sand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 17:14:18.000000 docker-sand-0.0.6/docker_sand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:14:19.170820 docker-sand-0.0.6/sand/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:14:19.170820 docker-sand-0.0.6/sand/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/internal/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/internal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:14:19.174820 docker-sand-0.0.6/sand/internal/sandfile_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/internal/sandfile_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/internal/sandfile_executor/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/internal/sandfile_executor/sandfile_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/internal/sandfile_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-06 17:14:16.000000 docker-sand-0.0.6/sand/sand.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 17:14:19.174820 docker-sand-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-06 17:14:16.000000 docker-sand-0.0.6/setup.py
```

### Comparing `docker-sand-0.0.5/LICENSE` & `docker-sand-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.5/PKG-INFO` & `docker-sand-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: docker-sand
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sand is a Dockerfile generator based on python that allows you to write your Dockerfile in a more convenient way.
 Home-page: https://github.com/gkpln3/Sand
 Author: Guy Kaplan
 License: MIT
 Description: # Sand 🏝
         [![.github/workflows/ci.yml](https://github.com/gkpln3/Sand/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gkpln3/Sand/actions/workflows/ci.yml)
         
         Sand is a Dockerfile generator.
         
         It allows you to write cleaner, shorter and more configurable Dockerfiles.
         
         ## Developers ❤️ Sand
         Sand is built by developers, for developers. It's built to be as simple as possible, while still being super useful.
         
+        ## Installation
+        You can install Sand using pip.
+        ```bash
+        pip3 install docker-sand
+        ```
+        
         ## Features
         ✅ Simple, easy to learn syntax based on Python.
         
         ✅ Configurable Dockerfiles. 
         
         ✅ Share code between Dockerfiles.
         
@@ -108,21 +114,16 @@
         from sand import *
         
         MyService("home-timeline") # Defined in ../Sandfile
         ```
         
         This allows you to share code between your Dockerfiles, and keep them [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
         
-        This works similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
+        This is similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
         
-        ## Installation
-        You can install Sand using pip.
-        ```bash
-        pip3 install docker-sand
-        ```
         
         ## Usage
         Running Sand is as simple as running `sand` in your terminal.
         This will generate Dockerfiles for all Sandfiles in the current directory.
         ```
         $ sand config
         Saving Dockerfile to backend/service1/Dockerfile
```

### Comparing `docker-sand-0.0.5/README.md` & `docker-sand-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 Sand is a Dockerfile generator.
 
 It allows you to write cleaner, shorter and more configurable Dockerfiles.
 
 ## Developers ❤️ Sand
 Sand is built by developers, for developers. It's built to be as simple as possible, while still being super useful.
 
+## Installation
+You can install Sand using pip.
+```bash
+pip3 install docker-sand
+```
+
 ## Features
 ✅ Simple, easy to learn syntax based on Python.
 
 ✅ Configurable Dockerfiles. 
 
 ✅ Share code between Dockerfiles.
 
@@ -101,21 +107,16 @@
 from sand import *
 
 MyService("home-timeline") # Defined in ../Sandfile
 ```
 
 This allows you to share code between your Dockerfiles, and keep them [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
 
-This works similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
+This is similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
 
-## Installation
-You can install Sand using pip.
-```bash
-pip3 install docker-sand
-```
 
 ## Usage
 Running Sand is as simple as running `sand` in your terminal.
 This will generate Dockerfiles for all Sandfiles in the current directory.
 ```
 $ sand config
 Saving Dockerfile to backend/service1/Dockerfile
```

### Comparing `docker-sand-0.0.5/docker_sand.egg-info/PKG-INFO` & `docker-sand-0.0.6/docker_sand.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: docker-sand
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sand is a Dockerfile generator based on python that allows you to write your Dockerfile in a more convenient way.
 Home-page: https://github.com/gkpln3/Sand
 Author: Guy Kaplan
 License: MIT
 Description: # Sand 🏝
         [![.github/workflows/ci.yml](https://github.com/gkpln3/Sand/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gkpln3/Sand/actions/workflows/ci.yml)
         
         Sand is a Dockerfile generator.
         
         It allows you to write cleaner, shorter and more configurable Dockerfiles.
         
         ## Developers ❤️ Sand
         Sand is built by developers, for developers. It's built to be as simple as possible, while still being super useful.
         
+        ## Installation
+        You can install Sand using pip.
+        ```bash
+        pip3 install docker-sand
+        ```
+        
         ## Features
         ✅ Simple, easy to learn syntax based on Python.
         
         ✅ Configurable Dockerfiles. 
         
         ✅ Share code between Dockerfiles.
         
@@ -108,21 +114,16 @@
         from sand import *
         
         MyService("home-timeline") # Defined in ../Sandfile
         ```
         
         This allows you to share code between your Dockerfiles, and keep them [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
         
-        This works similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
+        This is similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
         
-        ## Installation
-        You can install Sand using pip.
-        ```bash
-        pip3 install docker-sand
-        ```
         
         ## Usage
         Running Sand is as simple as running `sand` in your terminal.
         This will generate Dockerfiles for all Sandfiles in the current directory.
         ```
         $ sand config
         Saving Dockerfile to backend/service1/Dockerfile
```

### Comparing `docker-sand-0.0.5/docker_sand.egg-info/SOURCES.txt` & `docker-sand-0.0.6/docker_sand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.5/sand/internal/docker_image.py` & `docker-sand-0.0.6/sand/internal/docker_image.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.5/sand/internal/main.py` & `docker-sand-0.0.6/sand/internal/main.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.5/sand/internal/sandfile_executor/commands.py` & `docker-sand-0.0.6/sand/internal/sandfile_executor/commands.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.5/sand/internal/sandfile_executor/sandfile_executor.py` & `docker-sand-0.0.6/sand/internal/sandfile_executor/sandfile_executor.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.5/sand/internal/sandfile_watcher.py` & `docker-sand-0.0.6/sand/internal/sandfile_watcher.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.5/sand/sand.py` & `docker-sand-0.0.6/sand/sand.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.5/setup.py` & `docker-sand-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,37 @@
+import os
 from setuptools import setup, find_packages
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 def get_git_tag():
     import subprocess
     tag = subprocess.check_output(["git", "describe", "--tags"]).decode("utf-8").strip()
     return tag
 
+def get_version():
+    try:
+        version = get_git_tag()
+        with open("VERSION", "w") as f:
+            f.write(version)
+        return version
+    except:
+        # Not a git repo
+        pass
+
+    with open("VERSION", "r") as f:
+        version = f.read()
+    return version
+
 setup(
     name='docker-sand',
-    version=get_git_tag(),
+    version=get_version(),
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'sand = sand.internal.main:main'
         ]
     },
     install_requires=[
```

