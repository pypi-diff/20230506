# Comparing `tmp/hilly-0.1.1.tar.gz` & `tmp/hilly-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilly-0.1.1.tar", max compression
+gzip compressed data, was "hilly-0.1.2a0.tar", max compression
```

## Comparing `hilly-0.1.1.tar` & `hilly-0.1.2a0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1979 2023-05-06 18:30:35.386359 hilly-0.1.1/README.md
--rw-r--r--   0        0        0      491 2023-05-06 17:51:43.415570 hilly-0.1.1/hilly/__init__.py
--rw-r--r--   0        0        0      126 2023-05-06 17:29:56.362666 hilly-0.1.1/hilly/constants.py
--rw-r--r--   0        0        0     3015 2023-05-05 04:28:25.917707 hilly-0.1.1/hilly/io.py
--rw-r--r--   0        0        0     4202 2023-05-05 04:11:43.516707 hilly-0.1.1/hilly/ski.py
--rw-r--r--   0        0        0     5360 2023-05-05 04:28:25.921707 hilly-0.1.1/hilly/utils.py
--rw-r--r--   0        0        0      637 2023-05-06 17:51:34.227417 hilly-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 hilly-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-06 21:10:21.625217 hilly-0.1.2a0/LICENSE
+-rw-r--r--   0        0        0     1979 2023-05-06 18:30:35.386359 hilly-0.1.2a0/README.md
+-rw-r--r--   0        0        0      491 2023-05-06 17:51:43.415570 hilly-0.1.2a0/hilly/__init__.py
+-rw-r--r--   0        0        0      126 2023-05-06 17:29:56.362666 hilly-0.1.2a0/hilly/constants.py
+-rw-r--r--   0        0        0     3015 2023-05-05 04:28:25.917707 hilly-0.1.2a0/hilly/io.py
+-rw-r--r--   0        0        0     4202 2023-05-05 04:11:43.516707 hilly-0.1.2a0/hilly/ski.py
+-rw-r--r--   0        0        0     5360 2023-05-05 04:28:25.921707 hilly-0.1.2a0/hilly/utils.py
+-rw-r--r--   0        0        0      729 2023-05-06 21:18:11.722575 hilly-0.1.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2934 1970-01-01 00:00:00.000000 hilly-0.1.2a0/PKG-INFO
```

### Comparing `hilly-0.1.1/README.md` & `hilly-0.1.2a0/README.md`

 * *Files identical despite different names*

### Comparing `hilly-0.1.1/hilly/io.py` & `hilly-0.1.2a0/hilly/io.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.1/hilly/ski.py` & `hilly-0.1.2a0/hilly/ski.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.1/hilly/utils.py` & `hilly-0.1.2a0/hilly/utils.py`

 * *Files identical despite different names*

### Comparing `hilly-0.1.1/pyproject.toml` & `hilly-0.1.2a0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
 name = "hilly"
-version = "0.1.1"
+version = "0.1.2a"
 description = "Tools for summarizing and viewing sporty GPX traces"
 authors = ["Ryan <code+git@mcginger.net>"]
 readme = "README.md"
+keywords = ["gpx", "maps", "outdoors"]
+repository = "https://gitlab.com/ryanmcginger/hilly"
 
 [tool.poetry.dependencies]
 python = "~3.10"
 geopandas = "^0.12.2"
 gpxpy = "^1.5.0"
 lxml = "^4.9.2"
 gpxcsv = "^0.2.15"
@@ -16,15 +18,14 @@
 mapclassify = "^2.5.0"
 matplotlib = "^3.7.1"
 pyqt5 = "^5.15.9"
 tqdm = "^4.65.0"
 rasterio = "^1.3.6"
 loguru = "^0.7.0"
 
-
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.11.0"
 pytest = "^7.2.2"
 pre-commit = "^3.1.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `hilly-0.1.1/PKG-INFO` & `hilly-0.1.2a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: hilly
-Version: 0.1.1
+Version: 0.1.2a0
 Summary: Tools for summarizing and viewing sporty GPX traces
+Home-page: https://gitlab.com/ryanmcginger/hilly
+Keywords: gpx,maps,outdoors
 Author: Ryan
 Author-email: code+git@mcginger.net
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: folium (>=0.14.0,<0.15.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
@@ -15,14 +17,15 @@
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: mapclassify (>=2.5.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: rasterio (>=1.3.6,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Repository, https://gitlab.com/ryanmcginger/hilly
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <img src="docs/img/hilly-icon_sm.png" />
 </p>
```

