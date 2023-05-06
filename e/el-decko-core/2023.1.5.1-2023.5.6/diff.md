# Comparing `tmp/el_decko_core-2023.1.5.1.tar.gz` & `tmp/el_decko_core-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "el_decko_core-2023.1.5.1.tar", last modified: Thu Jan  5 16:29:08 2023, max compression
+gzip compressed data, was "el_decko_core-2023.5.6.tar", last modified: Sat May  6 20:01:23 2023, max compression
```

## Comparing `el_decko_core-2023.1.5.1.tar` & `el_decko_core-2023.5.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-01-05 16:29:08.542959 el_decko_core-2023.1.5.1/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2022-12-26 12:12:56.000000 el_decko_core-2023.1.5.1/LICENSE
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2660 2023-01-05 16:29:08.542959 el_decko_core-2023.1.5.1/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2455 2022-12-30 15:31:58.000000 el_decko_core-2023.1.5.1/README.md
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-01-05 16:29:08.542959 el_decko_core-2023.1.5.1/ed_core/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      739 2023-01-05 16:28:58.000000 el_decko_core-2023.1.5.1/ed_core/__init__.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1660 2023-01-05 15:28:53.000000 el_decko_core-2023.1.5.1/ed_core/dyn_data.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1656 2022-12-28 17:01:33.000000 el_decko_core-2023.1.5.1/ed_core/streamdeck.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2694 2023-01-05 16:21:11.000000 el_decko_core-2023.1.5.1/ed_core/streamdeck_config.py
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-01-05 16:29:08.542959 el_decko_core-2023.1.5.1/el_decko_core.egg-info/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2660 2023-01-05 16:29:08.000000 el_decko_core-2023.1.5.1/el_decko_core.egg-info/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      347 2023-01-05 16:29:08.000000 el_decko_core-2023.1.5.1/el_decko_core.egg-info/SOURCES.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-01-05 16:29:08.000000 el_decko_core-2023.1.5.1/el_decko_core.egg-info/dependency_links.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      104 2023-01-05 16:29:08.000000 el_decko_core-2023.1.5.1/el_decko_core.egg-info/entry_points.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       96 2023-01-05 16:29:08.000000 el_decko_core-2023.1.5.1/el_decko_core.egg-info/requires.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        8 2023-01-05 16:29:08.000000 el_decko_core-2023.1.5.1/el_decko_core.egg-info/top_level.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      650 2023-01-05 16:26:39.000000 el_decko_core-2023.1.5.1/pyproject.toml
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-01-05 16:29:08.542959 el_decko_core-2023.1.5.1/setup.cfg
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 20:01:23.057290 el_decko_core-2023.5.6/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-03-22 10:21:15.000000 el_decko_core-2023.5.6/LICENSE
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4677 2023-05-06 20:01:23.057290 el_decko_core-2023.5.6/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4475 2023-05-06 19:53:35.000000 el_decko_core-2023.5.6/README.md
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 20:01:23.057290 el_decko_core-2023.5.6/ed_core/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      994 2023-05-06 19:57:55.000000 el_decko_core-2023.5.6/ed_core/__init__.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1660 2023-03-22 10:21:16.000000 el_decko_core-2023.5.6/ed_core/dyn_data.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1818 2023-05-06 19:47:12.000000 el_decko_core-2023.5.6/ed_core/streamdeck.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2694 2023-03-22 10:21:16.000000 el_decko_core-2023.5.6/ed_core/streamdeck_config.py
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 20:01:23.057290 el_decko_core-2023.5.6/el_decko_core.egg-info/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     4677 2023-05-06 20:01:23.000000 el_decko_core-2023.5.6/el_decko_core.egg-info/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      347 2023-05-06 20:01:23.000000 el_decko_core-2023.5.6/el_decko_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-06 20:01:23.000000 el_decko_core-2023.5.6/el_decko_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      104 2023-05-06 20:01:23.000000 el_decko_core-2023.5.6/el_decko_core.egg-info/entry_points.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      112 2023-05-06 20:01:23.000000 el_decko_core-2023.5.6/el_decko_core.egg-info/requires.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        8 2023-05-06 20:01:23.000000 el_decko_core-2023.5.6/el_decko_core.egg-info/top_level.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      669 2023-05-06 19:45:46.000000 el_decko_core-2023.5.6/pyproject.toml
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-06 20:01:23.057290 el_decko_core-2023.5.6/setup.cfg
```

### Comparing `el_decko_core-2023.1.5.1/LICENSE` & `el_decko_core-2023.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.1.5.1/ed_core/__init__.py` & `el_decko_core-2023.5.6/ed_core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from importlib.metadata import entry_points
 
 from ed_core import streamdeck
 from ed_core.streamdeck_config import load_config, apply_config
 
-VERSION = "2023.1.5.1"
+VERSION = "2023.5.6"
 BACKENDS = {}
 
 
 def run():
-    print("El Decko Core running.")
-    load_config()
-    discovered_backends = entry_points(group='eldecko.backend')
-    for edb in discovered_backends:
-        edb_id = edb.value.split(":")[0]
-        edb_function = edb.load()
-        edb_name: str = edb.name
-        if edb_name.lower() == "init":
-            edb_function()
-        else:
-            if edb_id not in BACKENDS:
-                BACKENDS[edb_id] = {}
-            BACKENDS[edb_id][edb_name] = edb_function
-
-    streamdeck.initialize(BACKENDS)
+    try:
+        print("El Decko Core running.")
+        load_config()
+        discovered_backends = entry_points(group='eldecko.backend')
+        for edb in discovered_backends:
+            edb_id = edb.value.split(":")[0]
+            edb_function = edb.load()
+            edb_name: str = edb.name
+            if edb_name.lower() == "init":
+                edb_function()
+            else:
+                if edb_id not in BACKENDS:
+                    BACKENDS[edb_id] = {}
+                BACKENDS[edb_id][edb_name] = edb_function
+
+        streamdeck.initialize(BACKENDS)
+    except KeyboardInterrupt:
+        streamdeck.shutdown()
+        for backend in BACKENDS:
+            print(backend)
+            shutdown = BACKENDS[backend]["stop"]
+            shutdown()
 
 
 def backends():
     return BACKENDS
```

### Comparing `el_decko_core-2023.1.5.1/ed_core/dyn_data.py` & `el_decko_core-2023.5.6/ed_core/dyn_data.py`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.1.5.1/ed_core/streamdeck.py` & `el_decko_core-2023.5.6/ed_core/streamdeck.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,22 @@
         for t in threading.enumerate():
             try:
                 t.join()
             except RuntimeError:
                 pass
 
 
+def shutdown():
+    for index, deck in enumerate(stream_decks):
+        if not deck.is_visual():
+            continue
+        deck.reset()
+        deck.close()
+
+
 # Returns a list of all available Stream Decks
 def get_stream_decks():
     return stream_decks
 
 
 def get_supported_image_formats(deck: StreamDeck):
     deck.key_image_format()
```

### Comparing `el_decko_core-2023.1.5.1/ed_core/streamdeck_config.py` & `el_decko_core-2023.5.6/ed_core/streamdeck_config.py`

 * *Files identical despite different names*

### Comparing `el_decko_core-2023.1.5.1/pyproject.toml` & `el_decko_core-2023.5.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 dependencies = [
     "streamdeck",
     "Pillow",
     "xdg; platform_system=='Linux'"
 ]
 
 [project.optional-dependencies]
-backends = ["el_decko_backend_obs_ws>=0.0.1"]
+backends = ["el_decko_backend_obs_ws", "el_decko_backend_mpris"]
 
 [project.scripts]
 ed-core = "ed_core:run"
 
 [project.entry-points."eldecko.core"]
 start = "ed_core:run"
 backends = "ed_core:backends"
```

