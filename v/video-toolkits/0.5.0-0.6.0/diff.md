# Comparing `tmp/video_toolkits-0.5.0.tar.gz` & `tmp/video_toolkits-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/celestechen/Documents/github/video_toolkits/dist/tmpnztmja4t/video_toolkits-0.5.0.tar", last modified: Fri Aug 12 06:01:27 2022, max compression
+gzip compressed data, was "dist/video_toolkits-0.6.0.tar", last modified: Sat May  6 08:24:00 2023, max compression
```

## Comparing `video_toolkits-0.5.0.tar` & `video_toolkits-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 celestechen   (501) staff       (20)        0 2022-08-12 06:01:27.893660 video_toolkits-0.5.0/
--rw-rw-r--   0 celestechen   (501) staff       (20)     1060 2021-07-12 09:04:03.000000 video_toolkits-0.5.0/LICENSE
--rw-r--r--   0 celestechen   (501) staff       (20)     2884 2022-08-12 06:01:27.893311 video_toolkits-0.5.0/PKG-INFO
--rw-r--r--   0 celestechen   (501) staff       (20)     2429 2022-08-11 05:21:42.000000 video_toolkits-0.5.0/README.md
--rw-r--r--   0 celestechen   (501) staff       (20)      104 2021-09-04 10:25:50.000000 video_toolkits-0.5.0/pyproject.toml
--rw-r--r--   0 celestechen   (501) staff       (20)       38 2022-08-12 06:01:27.893776 video_toolkits-0.5.0/setup.cfg
--rw-r--r--   0 celestechen   (501) staff       (20)     2201 2022-08-11 05:21:42.000000 video_toolkits-0.5.0/setup.py
-drwxr-xr-x   0 celestechen   (501) staff       (20)        0 2022-08-12 06:01:27.890192 video_toolkits-0.5.0/video_toolkits/
--rw-r--r--   0 celestechen   (501) staff       (20)       69 2022-03-31 11:34:15.000000 video_toolkits-0.5.0/video_toolkits/__init__.py
--rw-rw-r--   0 celestechen   (501) staff       (20)       64 2022-08-11 05:21:42.000000 video_toolkits-0.5.0/video_toolkits/__version__.py
--rw-rw-r--   0 celestechen   (501) staff       (20)     4205 2022-08-11 05:21:42.000000 video_toolkits-0.5.0/video_toolkits/core.py
--rw-r--r--   0 celestechen   (501) staff       (20)     6932 2022-07-07 12:25:42.000000 video_toolkits-0.5.0/video_toolkits/draw.py
--rw-r--r--   0 celestechen   (501) staff       (20)      271 2021-09-04 09:44:49.000000 video_toolkits-0.5.0/video_toolkits/json_toolkits.py
-drwxr-xr-x   0 celestechen   (501) staff       (20)        0 2022-08-12 06:01:27.892506 video_toolkits-0.5.0/video_toolkits.egg-info/
--rw-r--r--   0 celestechen   (501) staff       (20)     2884 2022-08-12 06:01:27.000000 video_toolkits-0.5.0/video_toolkits.egg-info/PKG-INFO
--rw-r--r--   0 celestechen   (501) staff       (20)      365 2022-08-12 06:01:27.000000 video_toolkits-0.5.0/video_toolkits.egg-info/SOURCES.txt
--rw-rw-r--   0 celestechen   (501) staff       (20)        1 2022-08-12 06:01:27.000000 video_toolkits-0.5.0/video_toolkits.egg-info/dependency_links.txt
--rw-rw-r--   0 celestechen   (501) staff       (20)       17 2022-08-12 06:01:27.000000 video_toolkits-0.5.0/video_toolkits.egg-info/requires.txt
--rw-rw-r--   0 celestechen   (501) staff       (20)       15 2022-08-12 06:01:27.000000 video_toolkits-0.5.0/video_toolkits.egg-info/top_level.txt
+drwxr-xr-x   0 celestechen   (501) staff       (20)        0 2023-05-06 08:24:00.044835 video_toolkits-0.6.0/
+-rw-rw-r--   0 celestechen   (501) staff       (20)     1060 2021-07-12 09:04:03.000000 video_toolkits-0.6.0/LICENSE
+-rw-r--r--   0 celestechen   (501) staff       (20)     3685 2023-05-06 08:24:00.044523 video_toolkits-0.6.0/PKG-INFO
+-rw-r--r--   0 celestechen   (501) staff       (20)     2429 2022-08-11 05:21:42.000000 video_toolkits-0.6.0/README.md
+-rw-r--r--   0 celestechen   (501) staff       (20)      104 2021-09-04 10:25:50.000000 video_toolkits-0.6.0/pyproject.toml
+-rw-r--r--   0 celestechen   (501) staff       (20)       38 2023-05-06 08:24:00.044919 video_toolkits-0.6.0/setup.cfg
+-rw-r--r--   0 celestechen   (501) staff       (20)     2201 2023-05-06 08:22:32.000000 video_toolkits-0.6.0/setup.py
+drwxr-xr-x   0 celestechen   (501) staff       (20)        0 2023-05-06 08:24:00.040883 video_toolkits-0.6.0/video_toolkits/
+-rw-r--r--   0 celestechen   (501) staff       (20)       69 2022-03-31 11:34:15.000000 video_toolkits-0.6.0/video_toolkits/__init__.py
+-rw-rw-r--   0 celestechen   (501) staff       (20)       64 2023-05-06 08:22:32.000000 video_toolkits-0.6.0/video_toolkits/__version__.py
+-rw-rw-r--   0 celestechen   (501) staff       (20)     4205 2022-08-11 05:21:42.000000 video_toolkits-0.6.0/video_toolkits/core.py
+-rw-r--r--   0 celestechen   (501) staff       (20)     6968 2023-05-06 08:12:38.000000 video_toolkits-0.6.0/video_toolkits/draw.py
+-rw-r--r--   0 celestechen   (501) staff       (20)      271 2021-09-04 09:44:49.000000 video_toolkits-0.6.0/video_toolkits/json_toolkits.py
+drwxr-xr-x   0 celestechen   (501) staff       (20)        0 2023-05-06 08:24:00.044098 video_toolkits-0.6.0/video_toolkits.egg-info/
+-rw-r--r--   0 celestechen   (501) staff       (20)     3685 2023-05-06 08:23:59.000000 video_toolkits-0.6.0/video_toolkits.egg-info/PKG-INFO
+-rw-r--r--   0 celestechen   (501) staff       (20)      365 2023-05-06 08:24:00.000000 video_toolkits-0.6.0/video_toolkits.egg-info/SOURCES.txt
+-rw-rw-r--   0 celestechen   (501) staff       (20)        1 2023-05-06 08:23:59.000000 video_toolkits-0.6.0/video_toolkits.egg-info/dependency_links.txt
+-rw-rw-r--   0 celestechen   (501) staff       (20)       17 2023-05-06 08:23:59.000000 video_toolkits-0.6.0/video_toolkits.egg-info/requires.txt
+-rw-rw-r--   0 celestechen   (501) staff       (20)       15 2023-05-06 08:23:59.000000 video_toolkits-0.6.0/video_toolkits.egg-info/top_level.txt
```

### Comparing `video_toolkits-0.5.0/LICENSE` & `video_toolkits-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `video_toolkits-0.5.0/PKG-INFO` & `video_toolkits-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: video_toolkits
-Version: 0.5.0
-Summary: Toolkits for read/write video
-Home-page: https://github.com/Celeste-cj/video_toolkits
-Author: Celeste-cj
-Author-email: jingc2015@pku.edu.cn
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 :movie_camera: video_toolkits
 =======================
 
 This repo provides functions to read/write a video and draw keypoints.
 
 ** Defult BGR **
```

### Comparing `video_toolkits-0.5.0/setup.py` & `video_toolkits-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Package meta-data.
 NAME = 'video_toolkits'
 DESCRIPTION = 'Toolkits for read/write video'
 URL = 'https://github.com/Celeste-cj/video_toolkits'
 EMAIL = 'jingc2015@pku.edu.cn'
 AUTHOR = 'Celeste-cj'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.0'
+VERSION = '0.6.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'opencv-python', 'av'
 ]
 
 # What packages are optional?
```

### Comparing `video_toolkits-0.5.0/video_toolkits/core.py` & `video_toolkits-0.6.0/video_toolkits/core.py`

 * *Files identical despite different names*

### Comparing `video_toolkits-0.5.0/video_toolkits/draw.py` & `video_toolkits-0.6.0/video_toolkits/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,29 @@
     color_r,
     color_g,
     color_g,
 
     color_r,
     color_r,
     color_g,
-    color_g
+    color_g,
+
+    color_b
 ])
 
 sklts_simbase_foot = [
     [0, 1], [1, 2], [3, 4], [4, 5], [2, 6], [3, 6],
     [6, 22], [22, 7], [7, 8], [8, 9],
     [12, 22], [13, 22], [2, 22], [3, 22],
     [10, 11], [11, 12], [13, 14], [14, 15], [8, 12], [8, 13],
     [0, 19], [0, 21],
     [5, 16], [5, 18],
     [10, 23], [10, 24],
-    [15, 25], [15, 26]
+    [15, 25], [15, 26],
+    [8, 27], [9, 27]
 ]
 
 
 def is_visible(confs, idx):
     return confs is None or confs[idx] == 1
```

