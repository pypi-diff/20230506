# Comparing `tmp/gbopyrator-0.2.tar.gz` & `tmp/gbopyrator-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbopyrator-0.2.tar", last modified: Mon Apr  3 21:03:10 2023, max compression
+gzip compressed data, was "gbopyrator-0.3.tar", last modified: Sat May  6 11:36:24 2023, max compression
```

## Comparing `gbopyrator-0.2.tar` & `gbopyrator-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-03 21:03:10.634481 gbopyrator-0.2/
--rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-04-03 21:03:10.634481 gbopyrator-0.2/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      709 2023-04-03 20:48:18.000000 gbopyrator-0.2/README.md
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-03 21:03:10.634481 gbopyrator-0.2/gbopyrator/
--rw-rw-r--   0 robin     (1000) robin     (1000)       20 2023-04-03 21:02:39.000000 gbopyrator-0.2/gbopyrator/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)       67 2023-04-03 20:03:50.000000 gbopyrator-0.2/gbopyrator/__main__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     6155 2023-04-03 20:33:15.000000 gbopyrator-0.2/gbopyrator/cartrige_utils.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    11293 2023-04-03 20:27:51.000000 gbopyrator-0.2/gbopyrator/coms_utils.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1651 2023-04-03 19:42:57.000000 gbopyrator-0.2/gbopyrator/constants.py
--rw-rw-r--   0 robin     (1000) robin     (1000)  2708184 2023-04-03 19:47:49.000000 gbopyrator-0.2/gbopyrator/gb_gbc_roms_info.json
--rw-rw-r--   0 robin     (1000) robin     (1000)     2869 2023-04-03 20:34:54.000000 gbopyrator-0.2/gbopyrator/gbopyrator.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1546 2023-03-12 10:28:40.000000 gbopyrator-0.2/gbopyrator/printer.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-04-03 21:03:10.634481 gbopyrator-0.2/gbopyrator.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-04-03 21:03:10.000000 gbopyrator-0.2/gbopyrator.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      428 2023-04-03 21:03:10.000000 gbopyrator-0.2/gbopyrator.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-04-03 21:03:10.000000 gbopyrator-0.2/gbopyrator.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       58 2023-04-03 21:03:10.000000 gbopyrator-0.2/gbopyrator.egg-info/entry_points.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       53 2023-04-03 21:03:10.000000 gbopyrator-0.2/gbopyrator.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       11 2023-04-03 21:03:10.000000 gbopyrator-0.2/gbopyrator.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-04-03 21:03:10.634481 gbopyrator-0.2/setup.cfg
--rw-rw-r--   0 robin     (1000) robin     (1000)      850 2023-04-03 21:02:37.000000 gbopyrator-0.2/setup.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:36:24.437320 gbopyrator-0.3/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-05-06 11:36:24.437320 gbopyrator-0.3/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)      956 2023-05-06 11:32:49.000000 gbopyrator-0.3/README.md
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:36:24.433320 gbopyrator-0.3/gbopyrator/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      295 2023-05-06 11:34:25.000000 gbopyrator-0.3/gbopyrator/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)       67 2023-04-03 20:03:50.000000 gbopyrator-0.3/gbopyrator/__main__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5694 2023-05-06 10:32:25.000000 gbopyrator-0.3/gbopyrator/cartridge_utils.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    11293 2023-04-05 08:50:47.000000 gbopyrator-0.3/gbopyrator/coms_utils.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1651 2023-04-03 19:42:57.000000 gbopyrator-0.3/gbopyrator/constants.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)  2708184 2023-04-03 19:47:49.000000 gbopyrator-0.3/gbopyrator/gb_gbc_roms_info.json
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2674 2023-05-06 10:35:54.000000 gbopyrator-0.3/gbopyrator/gbopyrator.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1546 2023-03-12 10:28:40.000000 gbopyrator-0.3/gbopyrator/printer.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:36:24.433320 gbopyrator-0.3/gbopyrator.egg-info/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)      429 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/SOURCES.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/dependency_links.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       58 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/entry_points.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       53 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/requires.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       11 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/top_level.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-05-06 11:36:24.437320 gbopyrator-0.3/setup.cfg
+-rw-rw-r--   0 robin     (1000) robin     (1000)      850 2023-05-06 11:36:08.000000 gbopyrator-0.3/setup.py
```

### Comparing `gbopyrator-0.2/README.md` & `gbopyrator-0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-# gbopyrator: a Python module to control the GB Operator
+# gbopyrator: a command line tool and library for the GB Operator
 
-⚠️ Under development
+![](imgs/gbopyrator_demo.gif)
 
-## Information
+## ℹ️ Information
 
-`gbopyrator` is a Python package that enables you to control the GB Operator from [Epilogue](https://www.epilogue.co/) via the command line.
-Currently, `gbopyrator` is only compatible with **GameBoy** and **GameBoy Color** games. Support for GameBoy Advance is in development!
-## Installation
+GBOpyrator is a versatile Python package that allows you to manage and control the GB Operator from [Epilogue](https://www.epilogue.co/) via the command line. It currently supports **GameBoy** and **GameBoy Color** games, with GameBoy Advance compatibility in the works! 
+
+GBOpyrator can also be integrated into your own projects as a library.
+
+## ⬇️ Installation
 ```bash
 pip install gbopyrator
 ```
-## Usage
+## 🕹️ Usage
+### As a CLI tool
 ```bash
 gbopyrator \
     --dump-rom rom.gb               # dump the ROM to rom.gb file \
     --dump-save save.sav            # dump the RAM (save) to file \
     --write-save save_backup.sav    # read the file save_backup.sav and upload it to the cartridge RAM (save) \
-```
+```
+### As a library
+For detailed information on utilizing PyGBOperator as a library, please refer to the [DOC.md](DOC.md) file.
```

### Comparing `gbopyrator-0.2/gbopyrator/cartrige_utils.py` & `gbopyrator-0.3/gbopyrator/cartridge_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import binascii
 import time
 import re
 from rich.console import Console
 from . import coms_utils as cu
 from .printer import Printer
-
+import sys
 
 def check_initialized(func):
     def wrapper(*args, **kwargs):
         if args[0].initialized:
             return func(*args, **kwargs)
         else:
             raise Exception(
@@ -43,46 +43,37 @@
 class CartridgeReader(object):
     def __init__(self, quiet=False):
         self.initialized = False
         self.console = Console()
         self.quiet = quiet
         self.printer = Printer(quiet=quiet)
 
-    def initialize_reader(self):
+    def initialize_reader(self, blocking=False, timeout=0):
+        if not blocking and timeout != 0:
+            print("[WARNING] timeout is ignored when blocking is set to Fale",file=sys.stderr)
+
         with self.printer.status("Initializing reader..."):
-            dev = cu.find_gb_operator()
+            if blocking:
+                dev = cu.find_gb_operator_blocking(timeout=timeout)
+            else:
+                dev = cu.find_gb_operator()
 
         if dev is None:
             raise ValueError(
                 """
                 GB Operator not found, check it is plugged in or that the appropriate udev rules are set up if you are on linux. See : https://support.epilogue.co/hc/en-us/articles/4403827118738-How-can-I-connect-my-Operator-device-on-Linux-under-a-non-root-user-
                 """
             )
         else:
             self.gbop_device = cu.init_gb_operator(dev)
             self.initialized = True
             self.printer.success("[bold green]Reader initialized[/bold green]")
 
         return
 
-    def initialize_reader_blocking(self, timeout=0):
-        with self.printer.status("Initializing reader..."):
-            dev = cu.find_gb_operator_blocking(timeout=timeout)
-        if dev is None:
-            raise ValueError(
-                """
-                GB Operator not found, check it is plugged in or that the appropriate udev rules are set up if you are on linux. See : https://support.epilogue.co/hc/en-us/articles/4403827118738-How-can-I-connect-my-Operator-device-on-Linux-under-a-non-root-user-
-                """
-            )
-        else:
-            self.gbop_device = cu.init_gb_operator(dev)
-            self.initialized = True
-            self.printer.success("[bold green]Reader initialized[/bold green]")
-        return
-
     @check_initialized
     @release_device
     def read_cartridge_info(self):
         # with self.printer.status("Reading cartridge info..."):
         _cartridge_info = cu.read_cartridge_info(self.gbop_device)
         return _cartridge_info
```

### Comparing `gbopyrator-0.2/gbopyrator/coms_utils.py` & `gbopyrator-0.3/gbopyrator/coms_utils.py`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.2/gbopyrator/constants.py` & `gbopyrator-0.3/gbopyrator/constants.py`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.2/gbopyrator/gb_gbc_roms_info.json` & `gbopyrator-0.3/gbopyrator/gb_gbc_roms_info.json`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.2/gbopyrator/gbopyrator.py` & `gbopyrator-0.3/gbopyrator/gbopyrator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,11 @@
 # %%
 import argparse
-from .cartrige_utils import CartridgeReader
-import json
-
-from pkg_resources import resource_filename
-
-
-def load_roms_db(filename=resource_filename(__name__, "gb_gbc_roms_info.json")):
-    with open(filename, "r") as file:
-        roms_db = json.load(file)
-    return roms_db
-
+from .cartridge_utils import CartridgeReader
+from gbopyrator import load_roms_db
 
 # %%
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--dump-rom", type=str, default=None, help="Dump ROM to file")
     parser.add_argument("--dump-save", type=str, default=None, help="Dump save to file")
     parser.add_argument(
```

### Comparing `gbopyrator-0.2/gbopyrator/printer.py` & `gbopyrator-0.3/gbopyrator/printer.py`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.2/setup.py` & `gbopyrator-0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_requirements(file):
     with open(file, "r") as f:
         return f.read().splitlines()
 
 
 setup(
     name="gbopyrator",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "gbopyrator = gbopyrator.gbopyrator:main",
         ],
     },
     package_data={"gbopyrator": ["gb_gbc_roms_info.json"]},
```

