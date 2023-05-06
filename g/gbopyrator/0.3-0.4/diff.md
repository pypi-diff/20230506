# Comparing `tmp/gbopyrator-0.3.tar.gz` & `tmp/gbopyrator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbopyrator-0.3.tar", last modified: Sat May  6 11:36:24 2023, max compression
+gzip compressed data, was "gbopyrator-0.4.tar", last modified: Sat May  6 11:39:41 2023, max compression
```

## Comparing `gbopyrator-0.3.tar` & `gbopyrator-0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:36:24.437320 gbopyrator-0.3/
--rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-05-06 11:36:24.437320 gbopyrator-0.3/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      956 2023-05-06 11:32:49.000000 gbopyrator-0.3/README.md
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:36:24.433320 gbopyrator-0.3/gbopyrator/
--rw-rw-r--   0 robin     (1000) robin     (1000)      295 2023-05-06 11:34:25.000000 gbopyrator-0.3/gbopyrator/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)       67 2023-04-03 20:03:50.000000 gbopyrator-0.3/gbopyrator/__main__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     5694 2023-05-06 10:32:25.000000 gbopyrator-0.3/gbopyrator/cartridge_utils.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    11293 2023-04-05 08:50:47.000000 gbopyrator-0.3/gbopyrator/coms_utils.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1651 2023-04-03 19:42:57.000000 gbopyrator-0.3/gbopyrator/constants.py
--rw-rw-r--   0 robin     (1000) robin     (1000)  2708184 2023-04-03 19:47:49.000000 gbopyrator-0.3/gbopyrator/gb_gbc_roms_info.json
--rw-rw-r--   0 robin     (1000) robin     (1000)     2674 2023-05-06 10:35:54.000000 gbopyrator-0.3/gbopyrator/gbopyrator.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1546 2023-03-12 10:28:40.000000 gbopyrator-0.3/gbopyrator/printer.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:36:24.433320 gbopyrator-0.3/gbopyrator.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      429 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       58 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/entry_points.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       53 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       11 2023-05-06 11:36:24.000000 gbopyrator-0.3/gbopyrator.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-05-06 11:36:24.437320 gbopyrator-0.3/setup.cfg
--rw-rw-r--   0 robin     (1000) robin     (1000)      850 2023-05-06 11:36:08.000000 gbopyrator-0.3/setup.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:39:41.778063 gbopyrator-0.4/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-05-06 11:39:41.778063 gbopyrator-0.4/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)      956 2023-05-06 11:32:49.000000 gbopyrator-0.4/README.md
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:39:41.774063 gbopyrator-0.4/gbopyrator/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      295 2023-05-06 11:38:55.000000 gbopyrator-0.4/gbopyrator/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)       67 2023-04-03 20:03:50.000000 gbopyrator-0.4/gbopyrator/__main__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5694 2023-05-06 10:32:25.000000 gbopyrator-0.4/gbopyrator/cartridge_utils.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    11293 2023-04-05 08:50:47.000000 gbopyrator-0.4/gbopyrator/coms_utils.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1651 2023-04-03 19:42:57.000000 gbopyrator-0.4/gbopyrator/constants.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)  2708184 2023-04-03 19:47:49.000000 gbopyrator-0.4/gbopyrator/gb_gbc_roms_info.json
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2689 2023-05-06 11:38:30.000000 gbopyrator-0.4/gbopyrator/gbopyrator.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1546 2023-03-12 10:28:40.000000 gbopyrator-0.4/gbopyrator/printer.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-06 11:39:41.778063 gbopyrator-0.4/gbopyrator.egg-info/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-05-06 11:39:41.000000 gbopyrator-0.4/gbopyrator.egg-info/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)      429 2023-05-06 11:39:41.000000 gbopyrator-0.4/gbopyrator.egg-info/SOURCES.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-05-06 11:39:41.000000 gbopyrator-0.4/gbopyrator.egg-info/dependency_links.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       58 2023-05-06 11:39:41.000000 gbopyrator-0.4/gbopyrator.egg-info/entry_points.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       53 2023-05-06 11:39:41.000000 gbopyrator-0.4/gbopyrator.egg-info/requires.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       11 2023-05-06 11:39:41.000000 gbopyrator-0.4/gbopyrator.egg-info/top_level.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-05-06 11:39:41.778063 gbopyrator-0.4/setup.cfg
+-rw-rw-r--   0 robin     (1000) robin     (1000)      850 2023-05-06 11:39:07.000000 gbopyrator-0.4/setup.py
```

### Comparing `gbopyrator-0.3/README.md` & `gbopyrator-0.4/README.md`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.3/gbopyrator/cartridge_utils.py` & `gbopyrator-0.4/gbopyrator/cartridge_utils.py`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.3/gbopyrator/coms_utils.py` & `gbopyrator-0.4/gbopyrator/coms_utils.py`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.3/gbopyrator/constants.py` & `gbopyrator-0.4/gbopyrator/constants.py`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.3/gbopyrator/gb_gbc_roms_info.json` & `gbopyrator-0.4/gbopyrator/gb_gbc_roms_info.json`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.3/gbopyrator/gbopyrator.py` & `gbopyrator-0.4/gbopyrator/gbopyrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     cr.printer.greetings()
 
     if (args.dump_save is not None) and (args.write_save is not None):
         cr.printer.warning(
             "`dump-save` and `write-save` are both set. GBOpyrator will dump the save first and write it after."
         )
-    cr.initialize_reader_blocking()
+    cr.initialize_reader(blocking=True,timeout=10)
 
     rom_epilogue_id = cr.get_epilogue_id()
     roms_db = load_roms_db()
 
     # Print cartridge info
     if rom_epilogue_id in roms_db:
         rom_info = roms_db[rom_epilogue_id]
```

### Comparing `gbopyrator-0.3/gbopyrator/printer.py` & `gbopyrator-0.4/gbopyrator/printer.py`

 * *Files identical despite different names*

### Comparing `gbopyrator-0.3/setup.py` & `gbopyrator-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_requirements(file):
     with open(file, "r") as f:
         return f.read().splitlines()
 
 
 setup(
     name="gbopyrator",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "gbopyrator = gbopyrator.gbopyrator:main",
         ],
     },
     package_data={"gbopyrator": ["gb_gbc_roms_info.json"]},
```

