# Comparing `tmp/docker-sand-0.0.3.tar.gz` & `tmp/docker-sand-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-sand-0.0.3.tar", last modified: Tue May  2 16:02:17 2023, max compression
+gzip compressed data, was "docker-sand-0.0.5.tar", last modified: Sat May  6 16:51:06 2023, max compression
```

## Comparing `docker-sand-0.0.3.tar` & `docker-sand-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-02 16:02:17.551635 docker-sand-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-02 16:02:14.000000 docker-sand-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/docker_sand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/sand/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/sand/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/sand/internal/sandfile_executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/sandfile_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/sandfile_executor/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/sandfile_executor/sandfile_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/sandfile_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/sand.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:02:17.551635 docker-sand-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-02 16:02:14.000000 docker-sand-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.674926 docker-sand-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-06 16:51:05.000000 docker-sand-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-06 16:51:06.674926 docker-sand-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-06 16:51:05.000000 docker-sand-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.670926 docker-sand-0.0.5/docker_sand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 16:51:06.000000 docker-sand-0.0.5/docker_sand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.674926 docker-sand-0.0.5/sand/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.674926 docker-sand-0.0.5/sand/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:06.674926 docker-sand-0.0.5/sand/internal/sandfile_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/sandfile_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/sandfile_executor/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/sandfile_executor/sandfile_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/internal/sandfile_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-06 16:51:05.000000 docker-sand-0.0.5/sand/sand.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:51:06.674926 docker-sand-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-06 16:51:05.000000 docker-sand-0.0.5/setup.py
```

### Comparing `docker-sand-0.0.3/PKG-INFO` & `docker-sand-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: docker-sand
-Version: 0.0.3
+Version: 0.0.5
 Summary: Sand is a Dockerfile generator based on python that allows you to write your Dockerfile in a more convenient way.
 Home-page: https://github.com/gkpln3/Sand
 Author: Guy Kaplan
 License: MIT
 Description: # Sand 🏝
+        [![.github/workflows/ci.yml](https://github.com/gkpln3/Sand/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gkpln3/Sand/actions/workflows/ci.yml)
+        
         Sand is a Dockerfile generator.
         
         It allows you to write cleaner, shorter and more configurable Dockerfiles.
         
         ## Developers ❤️ Sand
         Sand is built by developers, for developers. It's built to be as simple as possible, while still being super useful.
         
@@ -18,23 +20,35 @@
         
         ✅ Configurable Dockerfiles. 
         
         ✅ Share code between Dockerfiles.
         
         ✅ Perfect for monorepos composed of multiple microservices.
         
+        ✅ Supports multi-stage builds.
+        
+        
+        #### Planned Features:
+            
+        🔘 Optimize builds by finding common layers between Dockerfiles, and merging them into a base image.
+        
+        🔘 Minimizing the number of layers by combining multiple RUN commands into one.    
+        
+        
         # Example
         Write your Dockerfile in a Python-like syntax.
         ```python
         # Sandfile
         from sand import *
         
         From("ubuntu", Tag="20.04")
-        Run("apt-get update")
-        Run("apt-get install ffmpeg python3")
+        Run([
+            "apt-get update",
+            "apt-get install ffmpeg python3"
+        ])
         
         # Install python debugger on debug images.
         if config.DEBUG:
             Run("pip3 install pdb")
         
         Copy("app", "/app")
         Entrypoint("python3 /app/app.py")
@@ -53,30 +67,34 @@
         Because `Sandfile`s are just Python files, and are being evaluated in an hierarchical manner by using the `Sand` directive, so you can easily share code between them.
         
         Given the following directory structure:
         ```
         my-monorepo/
         │
         ├── tweet-service/
+        |   ├── src/
+        |   ├── ...
         │   └── Sandfile
         │
         ├── home-timeline/
+        |   ├── src/
+        |   ├── ...
         │   └── Sandfile
         │
         └── Sandfile
         ```
         You can write your `Sandfile`s like this:
         ```python
         # ./my-monorepo/Sandfile
         from sand import *
         
         def MyService(name):
             From("ubuntu", "20.04")
-            Run(f"apt-get install python3")
-            Copy(Src="app", Dst="/app")
+            Run("apt-get install python3")
+            Copy(Src="src", Dst="/app")
             Entrypoint(f"python3 /app/{name}.py")
         
         Sand("tweet-service")
         Sand("home-timeline")
         ```
         ```python
         # ./my-monorepo/tweet-service/Sandfile
@@ -90,14 +108,21 @@
         from sand import *
         
         MyService("home-timeline") # Defined in ../Sandfile
         ```
         
         This allows you to share code between your Dockerfiles, and keep them [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
         
+        This works similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
+        
+        ## Installation
+        You can install Sand using pip.
+        ```bash
+        pip3 install docker-sand
+        ```
         
         ## Usage
         Running Sand is as simple as running `sand` in your terminal.
         This will generate Dockerfiles for all Sandfiles in the current directory.
         ```
         $ sand config
         Saving Dockerfile to backend/service1/Dockerfile
@@ -111,15 +136,15 @@
         ```
         
         ### Configuration
         You can pass configuration values to Sand using the `-D` or `--set` flag.
         ```
         $ sand config -DDEBUG=True
         ```
-        Or use a YAML file. (not implemented yet)
+        Or use a YAML file.
         ```yaml
         # sand.yaml
         DEBUG: True
         ```
         ```
         $ sand config --values sand.yaml
         ```
```

### Comparing `docker-sand-0.0.3/README.md` & `docker-sand-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Sand 🏝
+[![.github/workflows/ci.yml](https://github.com/gkpln3/Sand/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gkpln3/Sand/actions/workflows/ci.yml)
+
 Sand is a Dockerfile generator.
 
 It allows you to write cleaner, shorter and more configurable Dockerfiles.
 
 ## Developers ❤️ Sand
 Sand is built by developers, for developers. It's built to be as simple as possible, while still being super useful.
 
@@ -11,23 +13,35 @@
 
 ✅ Configurable Dockerfiles. 
 
 ✅ Share code between Dockerfiles.
 
 ✅ Perfect for monorepos composed of multiple microservices.
 
+✅ Supports multi-stage builds.
+
+
+#### Planned Features:
+    
+🔘 Optimize builds by finding common layers between Dockerfiles, and merging them into a base image.
+
+🔘 Minimizing the number of layers by combining multiple RUN commands into one.    
+
+
 # Example
 Write your Dockerfile in a Python-like syntax.
 ```python
 # Sandfile
 from sand import *
 
 From("ubuntu", Tag="20.04")
-Run("apt-get update")
-Run("apt-get install ffmpeg python3")
+Run([
+    "apt-get update",
+    "apt-get install ffmpeg python3"
+])
 
 # Install python debugger on debug images.
 if config.DEBUG:
     Run("pip3 install pdb")
 
 Copy("app", "/app")
 Entrypoint("python3 /app/app.py")
@@ -46,30 +60,34 @@
 Because `Sandfile`s are just Python files, and are being evaluated in an hierarchical manner by using the `Sand` directive, so you can easily share code between them.
 
 Given the following directory structure:
 ```
 my-monorepo/
 │
 ├── tweet-service/
+|   ├── src/
+|   ├── ...
 │   └── Sandfile
 │
 ├── home-timeline/
+|   ├── src/
+|   ├── ...
 │   └── Sandfile
 │
 └── Sandfile
 ```
 You can write your `Sandfile`s like this:
 ```python
 # ./my-monorepo/Sandfile
 from sand import *
 
 def MyService(name):
     From("ubuntu", "20.04")
-    Run(f"apt-get install python3")
-    Copy(Src="app", Dst="/app")
+    Run("apt-get install python3")
+    Copy(Src="src", Dst="/app")
     Entrypoint(f"python3 /app/{name}.py")
 
 Sand("tweet-service")
 Sand("home-timeline")
 ```
 ```python
 # ./my-monorepo/tweet-service/Sandfile
@@ -83,14 +101,21 @@
 from sand import *
 
 MyService("home-timeline") # Defined in ../Sandfile
 ```
 
 This allows you to share code between your Dockerfiles, and keep them [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
 
+This works similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
+
+## Installation
+You can install Sand using pip.
+```bash
+pip3 install docker-sand
+```
 
 ## Usage
 Running Sand is as simple as running `sand` in your terminal.
 This will generate Dockerfiles for all Sandfiles in the current directory.
 ```
 $ sand config
 Saving Dockerfile to backend/service1/Dockerfile
@@ -104,15 +129,15 @@
 ```
 
 ### Configuration
 You can pass configuration values to Sand using the `-D` or `--set` flag.
 ```
 $ sand config -DDEBUG=True
 ```
-Or use a YAML file. (not implemented yet)
+Or use a YAML file.
 ```yaml
 # sand.yaml
 DEBUG: True
 ```
 ```
 $ sand config --values sand.yaml
 ```
```

### Comparing `docker-sand-0.0.3/docker_sand.egg-info/PKG-INFO` & `docker-sand-0.0.5/docker_sand.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: docker-sand
-Version: 0.0.3
+Version: 0.0.5
 Summary: Sand is a Dockerfile generator based on python that allows you to write your Dockerfile in a more convenient way.
 Home-page: https://github.com/gkpln3/Sand
 Author: Guy Kaplan
 License: MIT
 Description: # Sand 🏝
+        [![.github/workflows/ci.yml](https://github.com/gkpln3/Sand/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gkpln3/Sand/actions/workflows/ci.yml)
+        
         Sand is a Dockerfile generator.
         
         It allows you to write cleaner, shorter and more configurable Dockerfiles.
         
         ## Developers ❤️ Sand
         Sand is built by developers, for developers. It's built to be as simple as possible, while still being super useful.
         
@@ -18,23 +20,35 @@
         
         ✅ Configurable Dockerfiles. 
         
         ✅ Share code between Dockerfiles.
         
         ✅ Perfect for monorepos composed of multiple microservices.
         
+        ✅ Supports multi-stage builds.
+        
+        
+        #### Planned Features:
+            
+        🔘 Optimize builds by finding common layers between Dockerfiles, and merging them into a base image.
+        
+        🔘 Minimizing the number of layers by combining multiple RUN commands into one.    
+        
+        
         # Example
         Write your Dockerfile in a Python-like syntax.
         ```python
         # Sandfile
         from sand import *
         
         From("ubuntu", Tag="20.04")
-        Run("apt-get update")
-        Run("apt-get install ffmpeg python3")
+        Run([
+            "apt-get update",
+            "apt-get install ffmpeg python3"
+        ])
         
         # Install python debugger on debug images.
         if config.DEBUG:
             Run("pip3 install pdb")
         
         Copy("app", "/app")
         Entrypoint("python3 /app/app.py")
@@ -53,30 +67,34 @@
         Because `Sandfile`s are just Python files, and are being evaluated in an hierarchical manner by using the `Sand` directive, so you can easily share code between them.
         
         Given the following directory structure:
         ```
         my-monorepo/
         │
         ├── tweet-service/
+        |   ├── src/
+        |   ├── ...
         │   └── Sandfile
         │
         ├── home-timeline/
+        |   ├── src/
+        |   ├── ...
         │   └── Sandfile
         │
         └── Sandfile
         ```
         You can write your `Sandfile`s like this:
         ```python
         # ./my-monorepo/Sandfile
         from sand import *
         
         def MyService(name):
             From("ubuntu", "20.04")
-            Run(f"apt-get install python3")
-            Copy(Src="app", Dst="/app")
+            Run("apt-get install python3")
+            Copy(Src="src", Dst="/app")
             Entrypoint(f"python3 /app/{name}.py")
         
         Sand("tweet-service")
         Sand("home-timeline")
         ```
         ```python
         # ./my-monorepo/tweet-service/Sandfile
@@ -90,14 +108,21 @@
         from sand import *
         
         MyService("home-timeline") # Defined in ../Sandfile
         ```
         
         This allows you to share code between your Dockerfiles, and keep them [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
         
+        This works similar to the way `add_subdirectory` works in [CMake](https://cmake.org/)
+        
+        ## Installation
+        You can install Sand using pip.
+        ```bash
+        pip3 install docker-sand
+        ```
         
         ## Usage
         Running Sand is as simple as running `sand` in your terminal.
         This will generate Dockerfiles for all Sandfiles in the current directory.
         ```
         $ sand config
         Saving Dockerfile to backend/service1/Dockerfile
@@ -111,15 +136,15 @@
         ```
         
         ### Configuration
         You can pass configuration values to Sand using the `-D` or `--set` flag.
         ```
         $ sand config -DDEBUG=True
         ```
-        Or use a YAML file. (not implemented yet)
+        Or use a YAML file.
         ```yaml
         # sand.yaml
         DEBUG: True
         ```
         ```
         $ sand config --values sand.yaml
         ```
```

### Comparing `docker-sand-0.0.3/docker_sand.egg-info/SOURCES.txt` & `docker-sand-0.0.5/docker_sand.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 docker_sand.egg-info/PKG-INFO
 docker_sand.egg-info/SOURCES.txt
 docker_sand.egg-info/dependency_links.txt
 docker_sand.egg-info/entry_points.txt
 docker_sand.egg-info/requires.txt
```

### Comparing `docker-sand-0.0.3/sand/internal/docker_image.py` & `docker-sand-0.0.5/sand/internal/docker_image.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.3/sand/internal/main.py` & `docker-sand-0.0.5/sand/internal/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import argparse
 import glob
 import os
 import re
 from typing import List
+import yaml
 
 from ..sand import AttributeDict
 from .sandfile_watcher import watch_for_sandfile_changes
 
 from .docker_image import DockerImage
 from .sandfile_executor.sandfile_executor import SandfileExecutor
 
 
 def _add_config_command(subparsers):
     parser = subparsers.add_parser("config", help="config the image")
     parser.add_argument("dir", type=str, nargs='?', help="Directory to config from", default=".")
     parser.add_argument("-D", "--set", dest="config", type=str, action="append", help="Set config variable, these variables will be accessible by using the `config` variable in the Sandfile")
     parser.add_argument("-w", "--watch", action="store_true", help="Watch for changes in the Sandfile and rebuild the Dockerfile")
+    parser.add_argument("--values", type=str, nargs='?', help="Path to values file")
     return parser
 
 def _add_ignore_command(subparsers):
     parser = subparsers.add_parser("ignore", help="Add all generated Dockerfiles to .gitignore")
     parser.add_argument("dir", type=str, nargs='?', help="Root directory of Sandfile", default=".")
     return parser
 
@@ -116,18 +118,24 @@
                     f.write("Dockerfile\n")
         else:
             print(f"Creating {gitignore_path}")
             with open(gitignore_path, "w") as f:
                 f.write("Dockerfile\n")
 
 def _parse_config(args) -> dict:
+    config = {}
+
+    if args.values is not None:
+        with open(args.values, "r") as f:
+            config = yaml.load(f, Loader=yaml.SafeLoader)
+        return config
+    
     if args.config is None:
-        return {}
+        return config
     
-    config = {}
     for arg in args.config:
         if "=" not in arg:
             config[arg] = True
         else:
             key, value = arg.split("=")
             config[key] = value
     return config
```

### Comparing `docker-sand-0.0.3/sand/internal/sandfile_executor/commands.py` & `docker-sand-0.0.5/sand/internal/sandfile_executor/commands.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.3/sand/internal/sandfile_executor/sandfile_executor.py` & `docker-sand-0.0.5/sand/internal/sandfile_executor/sandfile_executor.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.3/sand/internal/sandfile_watcher.py` & `docker-sand-0.0.5/sand/internal/sandfile_watcher.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.3/sand/sand.py` & `docker-sand-0.0.5/sand/sand.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.3/setup.py` & `docker-sand-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from setuptools import setup, find_packages
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
+def get_git_tag():
+    import subprocess
+    tag = subprocess.check_output(["git", "describe", "--tags"]).decode("utf-8").strip()
+    return tag
+
 setup(
     name='docker-sand',
-    version='0.0.3',
+    version=get_git_tag(),
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'sand = sand.internal.main:main'
         ]
     },
     install_requires=[
```

