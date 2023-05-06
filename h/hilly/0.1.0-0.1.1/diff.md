# Comparing `tmp/hilly-0.1.0.tar.gz` & `tmp/hilly-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilly-0.1.0.tar", max compression
+gzip compressed data, was "hilly-0.1.1.tar", max compression
```

## Comparing `hilly-0.1.0.tar` & `hilly-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1722 2023-05-06 17:29:34.602328 hilly-0.1.0/README.md
--rw-r--r--   0        0        0      491 2023-05-06 17:36:57.613221 hilly-0.1.0/hilly/__init__.py
--rw-r--r--   0        0        0      126 2023-05-06 17:29:56.362666 hilly-0.1.0/hilly/constants.py
--rw-r--r--   0        0        0     3015 2023-05-05 04:28:25.917707 hilly-0.1.0/hilly/io.py
--rw-r--r--   0        0        0     4202 2023-05-05 04:11:43.516707 hilly-0.1.0/hilly/ski.py
--rw-r--r--   0        0        0     5360 2023-05-05 04:28:25.921707 hilly-0.1.0/hilly/utils.py
--rw-r--r--   0        0        0      637 2023-05-06 17:31:01.467680 hilly-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2535 1970-01-01 00:00:00.000000 hilly-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1979 2023-05-06 18:30:35.386359 hilly-0.1.1/README.md
+-rw-r--r--   0        0        0      491 2023-05-06 17:51:43.415570 hilly-0.1.1/hilly/__init__.py
+-rw-r--r--   0        0        0      126 2023-05-06 17:29:56.362666 hilly-0.1.1/hilly/constants.py
+-rw-r--r--   0        0        0     3015 2023-05-05 04:28:25.917707 hilly-0.1.1/hilly/io.py
+-rw-r--r--   0        0        0     4202 2023-05-05 04:11:43.516707 hilly-0.1.1/hilly/ski.py
+-rw-r--r--   0        0        0     5360 2023-05-05 04:28:25.921707 hilly-0.1.1/hilly/utils.py
+-rw-r--r--   0        0        0      637 2023-05-06 17:51:34.227417 hilly-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 hilly-0.1.1/PKG-INFO
```

### Comparing `hilly-0.1.0/hilly/io.py` & `hilly-0.1.1/hilly/io.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.0/hilly/ski.py` & `hilly-0.1.1/hilly/ski.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.0/hilly/utils.py` & `hilly-0.1.1/hilly/utils.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.0/pyproject.toml` & `hilly-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hilly"
-version = "0.1.0"
+version = "0.1.1"
 description = "Tools for summarizing and viewing sporty GPX traces"
 authors = ["Ryan <code+git@mcginger.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.10"
 geopandas = "^0.12.2"
```

### Comparing `hilly-0.1.0/PKG-INFO` & `hilly-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilly
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for summarizing and viewing sporty GPX traces
 Author: Ryan
 Author-email: code+git@mcginger.net
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: folium (>=0.14.0,<0.15.0)
@@ -17,14 +17,20 @@
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: rasterio (>=1.3.6,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
+
+<p align="center">
+  <img src="docs/img/hilly-icon_sm.png" />
+</p>
+
+
 # Hilly
 
 Tools for summarizing and viewing sporty GPX traces
 
 ## Install
 
 ```bash
@@ -78,23 +84,25 @@
 #    Total lift time: 0 days 00:36:55.990000
 #    Time Ratio: 0.4747313841668961
 ```
 
 Or, you can view the trace:
 
 ```python
-# open leaflet map showing points
-m = ski_df.explore("labels")
+# open leaflet map showing points, dropping datetime column for proper JSON
+m = ski_df.drop(columns=["time"]).explore("labels", cmap="coolwarm_r")
 m.show_in_browser()
 ```
+![ski-point-map](docs/img/ski-point-map.png)
 
 or rasterize the trace to get a density map:
 ```python
-arr, bounds = hilly.utils.rasterize(df, runs_only=True)
+arr, bounds = hilly.utils.rasterize(ski_df, runs_only=True, res=1)
 m = hilly.io.map_raster(arr, bounds)
 m.show_in_browser()
 ```
+![ski-raster-map](docs/img/ski-raster-map.png)
 
 # Collecting Traces
 
 There are many apps available for collecting traces. I use [OpenTracks](https://opentracksapp.com/) and follow the Export instructions from the settings menu.
```

