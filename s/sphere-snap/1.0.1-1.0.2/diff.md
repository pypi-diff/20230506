# Comparing `tmp/sphere_snap-1.0.1-py3-none-any.whl.zip` & `tmp/sphere_snap-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 24420 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3128 b- defN 23-May-06 11:48 sphere_snap/__init__.py
+Zip file size: 24419 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     3128 b- defN 23-May-06 12:01 sphere_snap/__init__.py
 -rw-r--r--  2.0 unx     4478 b- defN 23-May-06 10:59 sphere_snap/radial_distortion.py
 -rw-r--r--  2.0 unx     7119 b- defN 23-May-06 10:40 sphere_snap/reprojections.py
 -rw-r--r--  2.0 unx     7348 b- defN 23-May-06 06:04 sphere_snap/snap_config.py
 -rw-r--r--  2.0 unx    12774 b- defN 23-May-03 20:59 sphere_snap/sphere_coor_projections.py
 -rw-r--r--  2.0 unx    22219 b- defN 23-May-06 11:02 sphere_snap/sphere_snap.py
 -rw-r--r--  2.0 unx     7360 b- defN 23-May-05 13:43 sphere_snap/top_view.py
 -rw-r--r--  2.0 unx     7244 b- defN 23-May-06 10:04 sphere_snap/utils.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6311 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1080 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/RECORD
-13 files, 80238 bytes uncompressed, 22620 bytes compressed:  71.8%
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6312 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1080 b- defN 23-May-06 12:01 sphere_snap-1.0.2.dist-info/RECORD
+13 files, 80239 bytes uncompressed, 22619 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: sphere_snap/top_view.py
 Comment: 
 
 Filename: sphere_snap/utils.py
 Comment: 
 
-Filename: sphere_snap-1.0.1.dist-info/LICENSE
+Filename: sphere_snap-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: sphere_snap-1.0.1.dist-info/METADATA
+Filename: sphere_snap-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: sphere_snap-1.0.1.dist-info/WHEEL
+Filename: sphere_snap-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: sphere_snap-1.0.1.dist-info/top_level.txt
+Filename: sphere_snap-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sphere_snap-1.0.1.dist-info/RECORD
+Filename: sphere_snap-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphere_snap/__init__.py

```diff
@@ -4,15 +4,15 @@
 A quick and easy to use library for reprojecting various image types.
 """
 from __future__ import absolute_import
 import logging
 import numpy as np
 
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __author__ = 'Andrei Georgescu'
 __credits__ = ''
 
 
 is_cupy_available = None
 
 def __init_cupy():
```

## Comparing `sphere_snap-1.0.1.dist-info/LICENSE` & `sphere_snap-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sphere_snap-1.0.1.dist-info/METADATA` & `sphere_snap-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphere-snap
-Version: 1.0.1
+Version: 1.0.2
 Summary: A quick and easy to use library for reprojecting various image types
 Home-page: https://androclassic.github.io/SphereSnap/sphere_snap.html
 Author: Andrei Georgescu
 Author-email: andrei.georgescu@yahoo.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -31,14 +31,15 @@
 <img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621440-5f2fa7f1-b072-4aff-8596-48b236c1d60f.jpg">
 
 ### Create equirectangular image using cubemap faces
 <img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/236621503-b5cf5e22-6a89-41c1-8765-3c5d23c1df1d.png">
 
 ### Create fisheye images from equirectangular or cubemap images
 <img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621560-cf9f5344-d041-4769-8b86-c52efa2958f6.png">
+
 ### Create top view images from equirectangular/fisheye/planar images
 <img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621633-4c6b30b5-0141-4a43-95fd-e93409d56d3e.png">
 
 ### Correct radially distorted images
 <img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621823-a32b57f9-ec4c-4d8c-b45d-f5cda1dbaecc.png">
```

