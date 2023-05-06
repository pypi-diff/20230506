# Comparing `tmp/sphere_snap-1.0.0-py3-none-any.whl.zip` & `tmp/sphere_snap-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,15 @@
-Zip file size: 17643 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3128 b- defN 23-May-03 21:07 sphere_snap/__init__.py
--rw-r--r--  2.0 unx     7092 b- defN 23-May-03 20:59 sphere_snap/snap_config.py
+Zip file size: 24420 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     3128 b- defN 23-May-06 11:48 sphere_snap/__init__.py
+-rw-r--r--  2.0 unx     4478 b- defN 23-May-06 10:59 sphere_snap/radial_distortion.py
+-rw-r--r--  2.0 unx     7119 b- defN 23-May-06 10:40 sphere_snap/reprojections.py
+-rw-r--r--  2.0 unx     7348 b- defN 23-May-06 06:04 sphere_snap/snap_config.py
 -rw-r--r--  2.0 unx    12774 b- defN 23-May-03 20:59 sphere_snap/sphere_coor_projections.py
--rw-r--r--  2.0 unx    19890 b- defN 23-May-03 20:59 sphere_snap/sphere_snap.py
--rw-r--r--  2.0 unx     6660 b- defN 23-May-03 20:59 sphere_snap/utils.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-03 21:07 sphere_snap-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5553 b- defN 23-May-03 21:07 sphere_snap-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 21:07 sphere_snap-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-03 21:07 sphere_snap-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      826 b- defN 23-May-03 21:07 sphere_snap-1.0.0.dist-info/RECORD
-10 files, 57100 bytes uncompressed, 16237 bytes compressed:  71.6%
+-rw-r--r--  2.0 unx    22219 b- defN 23-May-06 11:02 sphere_snap/sphere_snap.py
+-rw-r--r--  2.0 unx     7360 b- defN 23-May-05 13:43 sphere_snap/top_view.py
+-rw-r--r--  2.0 unx     7244 b- defN 23-May-06 10:04 sphere_snap/utils.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6311 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1080 b- defN 23-May-06 11:56 sphere_snap-1.0.1.dist-info/RECORD
+13 files, 80238 bytes uncompressed, 22620 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -1,31 +1,40 @@
 Filename: sphere_snap/__init__.py
 Comment: 
 
+Filename: sphere_snap/radial_distortion.py
+Comment: 
+
+Filename: sphere_snap/reprojections.py
+Comment: 
+
 Filename: sphere_snap/snap_config.py
 Comment: 
 
 Filename: sphere_snap/sphere_coor_projections.py
 Comment: 
 
 Filename: sphere_snap/sphere_snap.py
 Comment: 
 
+Filename: sphere_snap/top_view.py
+Comment: 
+
 Filename: sphere_snap/utils.py
 Comment: 
 
-Filename: sphere_snap-1.0.0.dist-info/LICENSE
+Filename: sphere_snap-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: sphere_snap-1.0.0.dist-info/METADATA
+Filename: sphere_snap-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: sphere_snap-1.0.0.dist-info/WHEEL
+Filename: sphere_snap-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: sphere_snap-1.0.0.dist-info/top_level.txt
+Filename: sphere_snap-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sphere_snap-1.0.0.dist-info/RECORD
+Filename: sphere_snap-1.0.1.dist-info/RECORD
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
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = 'Andrei Georgescu'
 __credits__ = ''
 
 
 is_cupy_available = None
 
 def __init_cupy():
```

## sphere_snap/snap_config.py

```diff
@@ -1,25 +1,33 @@
 import numpy as np
 from scipy.spatial.transform import Rotation as R
 import sphere_snap.utils as snap_utils
 import sphere_snap.sphere_coor_projections as sphere_proj
+from enum import Enum
+
+class ImageProjectionType(Enum):
+    EQUI = 'equirectangular'
+    PINHOLE = 'pinhole'
+    FISHEYE_180 = 'fisheye180'
+    RADIAL_DISTORTED = 'distorted_pinhole'
+
 
 
 class SnapConfig:
     """
     Contains all properties needed to construct an image snap
     """
 
     def __init__(self, orientation_quat,
                  out_hw,
                  out_fov_deg,
                  source_img_hw,
                  source_img_fov_deg=None,
                  source_dist_coeff=None,
-                 source_img_type="equi"
+                 source_img_type=ImageProjectionType.EQUI
                 ):
 
         """
         Given the input parameters, creates an ImageViewProperties object
 
         The camera coordinate system is (xy in the screen plane, z+ going in the screen):
              ^
@@ -36,15 +44,15 @@
         :param fov_deg: a tuple containing (hfov, vfov)
         :param orientation_quat: array_like (4,1) of an orientation
         :param out_hw: a tuple containing output image size(height, width)
         :param source_dist_coeff: array containing distortion parameters, center offset should be normalised
                                 {lambda, center_offset_x, center_offset_y} (Default: None)
         :param source_img_hw: a tuple containing source image size(height, width)
         :param source_img_fov_deg: a tuple containing (hfov, vfov) of the perspective source image, if this is None the image is equirectangular
-        :param source_img_type: type of the source image eg. (plane, equi, fisheye180), default is equi.
+        :param source_img_type: ImageProjectionType of the source image eg. (PINHOLE, EQUI, FISHEYE_180, RADIAL_DISTORTED), default is EQUI.
         """
 
         rot_matrix = R.from_quat(orientation_quat).as_matrix()
 
         self.out_fov_deg = out_fov_deg
         self.out_hw = out_hw
         self.source_img_hw = source_img_hw
@@ -70,15 +78,15 @@
     @classmethod
     def createFromPoint(cls, center_point_xyz,
                         out_hw,
                         out_fov_deg,
                         source_img_hw,
                         source_img_fov_deg=None,
                         source_dist_coeff=None,
-                        source_img_type="equi",
+                        source_img_type=ImageProjectionType.EQUI,
                         quaternion = None,
                         ):
         """
         Given the input parameters, creates an ImageViewProperties object
         :param center_point_xyz: a point on the sphere where we want the view to be centered;
                 for a point to be on the sphere, its corresponding position vector should have
                 magnitude of 1 (= radius of sphere) and x, y, z in [-1, 1]
```

## sphere_snap/sphere_snap.py

```diff
@@ -1,31 +1,32 @@
 import logging
 import cv2
 import numpy as npy
 
 from scipy.spatial.transform import Rotation as R
 from math import isclose
+import copy
 
 import sphere_snap.utils as snap_utils
 import sphere_snap.sphere_coor_projections as sphere_proj
-from sphere_snap.snap_config import SnapConfig
+from sphere_snap.snap_config import SnapConfig, ImageProjectionType
 from sphere_snap import cupy_available, to_cp, to_np
 from sphere_snap import custom_cupy_wrap, convert_to_cupy, convert_to_numpy
-
+from sphere_snap.radial_distortion import RadialDistorter
 
 class SphereSnap:
     """
     Reproject various image types by projecting them first on a sphere surface
     """
 
     def __init__(self, snap_config):
         """
         Given the input parameters, creates an SphereSnap object
         """
-        self.snap_config = snap_config
+        self.snap_config = copy.deepcopy(snap_config) 
         self.snap_config.to_numpy()
         self.sphere_polygon_xyz = self.__create_snap_sphere_polygon()
         self.full_img_sphere_polygon_xyz = self.__create_source_img_sphere_polygon()
 
 
     def get_xyz_from_pixel(self, uv):
         """
@@ -182,19 +183,19 @@
         src_coor = to_np(src_coor)
         coors = src_coor.reshape((*self.snap_config.out_hw, 2))
         return coors
 
 
     def snap_to_perspective(self, source_img):
         # sanity checks
-        if self.snap_config.source_img_type == "equi":
+        if self.snap_config.source_img_type == ImageProjectionType.EQUI:
             h, w = self.snap_config.source_img_hw
             ar = w/h
             assert isclose(ar, 2, abs_tol=1e-2), f"Aspect ratio for equirectangular image is not 2:1. Resolution: [{w, h}]"
-        elif self.snap_config.source_img_type == "fisheye180":
+        elif self.snap_config.source_img_type == ImageProjectionType.FISHEYE_180:
             h, w = self.snap_config.source_img_hw
             ar = w/h
             assert isclose(ar, 1, abs_tol=1e-2), f"Aspect ratio for fisheye180 image is not 1:1. Resolution: [{w, h}]"
 
 
         # get coordinates from source image
         src_coor = self.get_source_image_coors()
@@ -202,34 +203,48 @@
         # resize image if description does not match reality
         if (source_img.shape[:2] != self.snap_config.source_img_hw[:2]).any():
             logging.warning("Source image dim " + str(source_img.shape) + " was different than expected: " +
                             str(self.snap_config.source_img_hw))
             source_img = cv2.resize(source_img, tuple(self.snap_config.source_img_hw[::-1]))
 
         # sample coordinates and create image
-        warp_mode = True if self.snap_config.source_img_type=="equi" else False
+        warp_mode = True if self.snap_config.source_img_type==ImageProjectionType.EQUI else False
         pers_img = npy.stack([snap_utils.sample_from_img(source_img[..., i], src_coor, clamp=warp_mode)
                                 for i in range(source_img.shape[2])], axis=-1)
         return pers_img.astype(npy.uint8)
 
+    @staticmethod
+    def __undistort_coors(u_coor, hw, dist_coeff):
+        """
+        Extracts the raw coordinates from a list of coordinates in the undistorted image
+        """
+        distortion_map = RadialDistorter.get().coor_mapping(hw, dist_coeff)
+        u_coor = u_coor.astype(int)
+        # clip values
+        in_bounds_indices = snap_utils.check_uv_in_bounds(u_coor, distortion_map.shape[:2])
+        # extract real coordinates from distortion map
+        coor = distortion_map[u_coor[in_bounds_indices, 1], u_coor[in_bounds_indices, 0]]
+        # swap from vu, to uv
+        coor[..., [0, 1]] = coor[..., [1, 0]]
+        return coor, in_bounds_indices
 
     @custom_cupy_wrap(convert_to_cupy, convert_to_numpy)
     def image2spherical(coors, snap_config, np=npy):
         """
         Transforms from image coordinates to sphere coordinates
         return the image sphere
         """
         s_hw = to_cp(snap_config.source_img_hw)
 
-        if snap_config.source_img_type == "equi":
+        if snap_config.source_img_type == ImageProjectionType.EQUI:
             return sphere_proj.equi_coor2spherical._original(coors, s_hw, np=np)
-        elif snap_config.source_img_type == "fisheye180":
+        elif snap_config.source_img_type == ImageProjectionType.FISHEYE_180:
             return sphere_proj.fisheye180_coor2spherical._original(coors, s_hw, np=np)
-
-        if snap_config.source_dist_coeff is not None:
+        elif snap_config.source_img_type == ImageProjectionType.RADIAL_DISTORTED:
+            assert snap_config.source_dist_coeff is not None, "Missing distortion coefficients !"
             dist_coeff = snap_config.source_dist_coeff
             # change from xy to yx
             coors = coors[...,[1,0]]
             # get undistorted coordinates, this is needed to correctly obtain spherical coordinates
             coors = sphere_proj.undistort(coors, np.array(dist_coeff), np.array(s_hw), normalize_values=True, np=np)
             coors = coors * np.array(s_hw)
             coors[...,[0,1]] = coors[...,[1,0]]
@@ -244,42 +259,52 @@
     def spherical2image(spherical, snap_config, np=npy) :
         """
         Transforms from sphere coordinates to image coordinates
         return the image coordinates
         :param spherical: spherical coordinates for the sphere surface points that we want to project
         :param snap_config: a snap_config object containing metadata of the snap
         """
-        if snap_config.source_img_type == "plane":
-            if snap_config.source_dist_coeff is not None:
-                assert False, "Not implemented yet !"
-            else:
-                coor = sphere_proj.pinhole_spherical2coor._original(spherical,
-                                                                    snap_config.source_img_fov_deg,
-                                                                    snap_config.source_img_hw, 
-                                                                    (0,0), 0, np=np)
+        if snap_config.source_img_type == ImageProjectionType.PINHOLE:
+            coor = sphere_proj.pinhole_spherical2coor._original(spherical,
+                                                                snap_config.source_img_fov_deg,
+                                                                snap_config.source_img_hw, 
+                                                                (0,0), 0, np=np)
+            return coor
+        elif snap_config.source_img_type == ImageProjectionType.RADIAL_DISTORTED:
+            assert snap_config.source_dist_coeff is not None, "Missing distortion coefficients !"
+            distortion_map = RadialDistorter.get().coor_mapping(snap_config.source_img_hw, snap_config.source_dist_coeff)
+            coor = sphere_proj.pinhole_spherical2coor._original(spherical,
+                                                                snap_config.source_img_fov_deg,
+                                                                np.array(distortion_map.shape[:2]), 
+                                                                (0,0), 0, np=np)
+            coor = to_np(coor)
+            distorted_coor, in_bounds_indices = SphereSnap.__undistort_coors(coor,
+                                                                            to_np(snap_config.source_img_hw),
+                                                                            to_np(snap_config.source_dist_coeff))
+            coor[in_bounds_indices] = distorted_coor
             return coor
 
-        elif snap_config.source_img_type == "fisheye180":
+        elif snap_config.source_img_type == ImageProjectionType.FISHEYE_180:
             return sphere_proj.fisheye180_spherical2coor._original(spherical, snap_config.source_img_hw, np=np)
-        elif snap_config.source_img_type == "equi":
+        elif snap_config.source_img_type == ImageProjectionType.EQUI:
             return sphere_proj.equi_spherical2coor._original(spherical, snap_config.source_img_hw, np=np)
         else:
             assert False, "Not implemented yet !"
 
 
     @staticmethod
-    def merge_multiple_snaps(output_hw, sphere_snaps, imgs, merge_method='average', target_type="equi"):
+    def merge_multiple_snaps(output_hw, sphere_snaps, imgs, merge_method='average', target_type=ImageProjectionType.EQUI):
         """
         Given a list of images extracted from a source image, re-create an image 
         return the full image obtained from the source views
         :param output_hw: a tuple containing source image size(height, width)
         :param views: a list of views we want to merge back in the full image
         :param imgs: a list of imgs coresponding to the views 
         :param merge_method: average, sum, max, last
-        :param target_type: image projection type (equi, fisheye180)
+        :param target_type: image projection type (ImageProjectionType.EQUI, ImageProjectionType.FISHEYE_180..)
         """
 
         imgs = [to_cp(img) for img in imgs]
 
         np = npy
         if cupy_available():
             import cupy as cp
@@ -300,15 +325,15 @@
         target = np.zeros((output_hw[0], output_hw[1], nb_channels), np.float)
         cnt = np.zeros((output_hw[0], output_hw[1], 1), np.uint8)
         
         # construct image uv coordinates
         img_all_coors = sphere_proj.get_2D_coor_grid._pipe(output_hw)
 
         # exclude region outside the circle
-        if cp_snap.source_img_type == "fisheye180":
+        if cp_snap.source_img_type == ImageProjectionType.FISHEYE_180:
             xy = img_all_coors-(np.array(output_hw)/2)
             r = np.linalg.norm(xy, axis=-1)
             img_all_coors = img_all_coors[r<(output_hw[0]/2)]
 
         img_all_sphere = SphereSnap.image2spherical._pipe(img_all_coors, cp_snap)
         for sphere_snap, snap_img in zip(sphere_snaps, imgs):
             # extract the coordinates in the view from each pixel in the source image
@@ -352,15 +377,18 @@
         :param hw: resolution of the source image you want to sample from
         :param source_img_fov_deg: a tuple containing (hfov, vfov) of the perspective source image, if this is None the image is equirectangular
         :param source_dist_coeff: None if does not exist, array containing radial distortion parameters,
                         offset center should be normalised {lambda, center_offset_x, center_offest_y}
         :param return_polar: If true, it will return also the sphere projection of the points in polar coordinates
         """
         if source_dist_coeff is not None:
-            assert False , "Not implemented yet!"
+            distortion_map = RadialDistorter.get().coor_mapping(hw, source_dist_coeff)
+            coor, polar = sphere_proj.sample_polygon(points, distortion_map.shape[:2], _)
+            coor, in_bounds_indices = SphereSnap.__undistort_coors(coor, hw, source_dist_coeff)
+            polar = polar[in_bounds_indices]        
         else:
             coor, polar = snap_utils.sample_polygon(points, hw, source_img_fov_deg)
 
         if return_polar is True:
             return coor, polar
         return coor
     
@@ -417,14 +445,15 @@
                             
         xyz = npy.ones((uv.shape[0], 3), npy.float64)
         fov_halftan = npy.tan(npy.radians(npy.array(self.snap_config.source_img_fov_deg) / 2))
         xyz[:, :2] = ((2*uv)-1) * fov_halftan
         xyz = self.__normalize_xyz(xyz)
         return xyz
 
+
     def __normalize_xyz(self, xyz):
         """
         Normalizes the xyz vectors
         """
         prev_shape = xyz.shape
         # keepdims=True for broadcasting when dividing below by the norm
         norm = npy.linalg.norm(xyz.reshape(-1, 3), axis=-1, keepdims=True)
```

## sphere_snap/utils.py

```diff
@@ -1,12 +1,14 @@
 import numpy as npy
 from scipy.ndimage import map_coordinates
-
+from scipy.spatial.transform import Rotation as R
+from scipy import ndimage
 from . import cupy_available, custom_cupy_wrap, convert_to_cupy, convert_to_numpy, to_np
 
+
 __CONSISTENCY_THRESHOLD = 0.12
 
 @custom_cupy_wrap(convert_to_cupy, convert_to_numpy)
 def construct_map(distorted_coor, undistorted_coor, res_hw, np=npy):
     """ 
     Given to sets of coordinates creates a map between them
     returns map from undistorted to distorted coordinates, 
@@ -169,7 +171,24 @@
     res_ar = hw[0] / hw[1]
     # adjust the FOV depending on the AR of the image. If portrait, take hfov as reference, if landscape, vfov
     focal_length = fyx[1] if res_ar < 1 else fyx[0]
     if npy.abs(1 - px_ar) > threshold:
         fov = compute_fovs([focal_length, focal_length], hw)
     return fov
 
+def rotation(yaw, pitch, roll):
+    return R.from_euler("yxz",[yaw,pitch,roll], degrees=True)
+
+
+def interpolate_nans(A):
+    # all large empty space in the image are set to zero
+    k_size = 9
+    k = npy.ones((k_size,k_size))
+    B = ndimage.convolve(A, k, mode='constant', cval=-1)
+    A[B<0] = -1e-1
+    # holes smaller than kernel size are interpolated
+    ok = A > 0
+    xp = ok.ravel().nonzero()[0]
+    fp = A[ok]
+    x  = (A==-1).ravel().nonzero()[0]
+    A[A==-1] = npy.interp(x, xp, fp)
+    return A
```

## Comparing `sphere_snap-1.0.0.dist-info/LICENSE` & `sphere_snap-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sphere_snap-1.0.0.dist-info/METADATA` & `sphere_snap-1.0.1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphere-snap
-Version: 1.0.0
+Version: 1.0.1
 Summary: A quick and easy to use library for reprojecting various image types
 Home-page: https://androclassic.github.io/SphereSnap/sphere_snap.html
 Author: Andrei Georgescu
 Author-email: andrei.georgescu@yahoo.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,90 +23,111 @@
 Requires-Dist: logging
 
 # SphereSnap
 A quick and easy to use library for reprojecting various image types. (inspired by http://paulbourke.net/panorama/sphere2persp/ ) 
 
 ## Examples and usecases
 ### Reprojecting equirectangular image into pinhole-camera images with customizable FoV and resolution
-<img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/227978179-f0c820d0-7a1e-470b-af85-ff5800addc8b.png">
-<img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/227983634-d915aa5c-ca84-4124-8d1d-086568e4c9bd.png">
+<img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/236621219-457eae8c-ad88-452d-8e89-8b16e4750dd1.jpg">
+<img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621440-5f2fa7f1-b072-4aff-8596-48b236c1d60f.jpg">
 
 ### Create equirectangular image using cubemap faces
-<img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/227979707-1c30f125-6677-4c84-93e5-bb71e290a602.png">
-<img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/227978179-f0c820d0-7a1e-470b-af85-ff5800addc8b.png">
+<img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/236621503-b5cf5e22-6a89-41c1-8765-3c5d23c1df1d.png">
 
 ### Create fisheye images from equirectangular or cubemap images
-<img width="727" alt="image" src="https://user-images.githubusercontent.com/1941529/227982333-aa13a305-556a-40dd-83cf-aedbd6019b7b.png">
+<img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621560-cf9f5344-d041-4769-8b86-c52efa2958f6.png">
+### Create top view images from equirectangular/fisheye/planar images
+<img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621633-4c6b30b5-0141-4a43-95fd-e93409d56d3e.png">
+
+### Correct radially distorted images
+<img width="320" alt="image" src="https://user-images.githubusercontent.com/1941529/236621823-a32b57f9-ec4c-4d8c-b45d-f5cda1dbaecc.png">
 
 
 ## How to use it
+
+Module sphere_snap.reprojections contains easy to use functions for simple situations: 
+- equi2cubemap
+- cubemap2equi
+- cubemap2fisheye
+- equi2fisheye
+- fisheye2equi
+- equi2tv
+
+For more complex situtation SphereSnaper can be used which is more flexible
+
 ```python
 import sphere_snap.utils as snap_utils
 import sphere_snap.sphere_coor_projections as sphere_proj
-from sphere_snap.snap_config import SnapConfig
+from sphere_snap.snap_config import SnapConfig, ImageProjectionType
 from sphere_snap.sphere_snap import SphereSnap
+import sphere_snap.reprojections as rpr
+
 ```
 
 ## Snap to perspective from equirectangular
 ```python
-snap_config = SnapConfig( [0,0,0,1], (1400,1400),(120,120), equi_img.shape[:2], source_img_type="equi")
+snap_config = SnapConfig( [0,0,0,1], (1400,1400),(120,120), equi_photo.shape[:2], source_img_type=ImageProjectionType.EQUI)
 snap_test = SphereSnap(snap_config)
-persp_img = snap_test.snap_to_perspective(equi_img)
+persp_img = snap_test.snap_to_perspective(equi_photo)
 ```
 ## Reproject equirectangular into 6 planar images of 90 degrees FoV (Cubemap)
 ```python
-def get_cube_map_faces(face_size=1440, source_img_hw=(2000,4000), source_img_type="equi"):
+def get_cube_map_faces(face_size=1440, source_img_hw=(2000,4000), source_img_type=ImageProjectionType.EQUI):
 
     snap_configs = [SnapConfig( rot(90*i,0), (face_size,face_size),(90,90), source_img_hw, source_img_type=source_img_type)
                         for i in range(4)]
     # top
     snap_configs.append(SnapConfig( rot(0,90), (face_size,face_size),(90,90), source_img_hw, source_img_type=source_img_type))
     # bottom
     snap_configs.append(SnapConfig( rot(0,-90), (face_size,face_size),(90,90), source_img_hw, source_img_type=source_img_type))
     return snap_configs
 
 cube_configs = get_cube_map_faces(face_size=1440, source_img_hw=equi_img.shape[:2])
 cube_faces_snaps = [SphereSnap(c) for c in cube_configs]
 cumbe_faces_imgs = [snap.snap_to_perspective(equi_img) for snap in cube_faces_snaps]
 
 ```
+or
+```python
+cube_faces_imgs = rpr.equi2cubemap(equi_img)
+```
 
 ## Reproject a planar image into equirectangular
 ```python
 reconstructed_equi = SphereSnap.merge_multiple_snaps((1000,2000), 
                                                      cube_faces_snaps, # snap object specifies destination position
                                                      cumbe_faces_imgs[::-1], # snap image contains planar image pixels
-                                                     target_type="equi", # destination image type
+                                                     target_type=ImageProjectionType.EQUI, # destination image type
                                                      merge_method="max")
 ```
 ## Reproject a planar image into fisheye 180
 ```python
 reconstructed_fisheye = SphereSnap.merge_multiple_snaps((1000,1000), 
                                                     cube_faces_snaps, # snap object specifies destination position
                                                     cumbe_faces_imgs, # snap image contains planar image pixels
-                                                    target_type="fisheye180", # destination image type
+                                                    target_type=ImageProjectionType.FISHEYE_180, # destination image type
                                                     merge_method="max")                                                    
 ```
 
 ## Snap to perspective from fisheye 180
 ```python
-snap_config = SnapConfig( rot(45,1), (1400,1400),(100,100), reconstructed_fisheye.shape[:2], source_img_type="fisheye180")
+snap_config = SnapConfig( rot(45,1), (1400,1400),(100,100), reconstructed_fisheye.shape[:2], source_img_type=ImageProjectionType.FISHEYE_180)
 snap_test = SphereSnap(snap_config)
 persp_img = snap_test.snap_to_perspective(reconstructed_fisheye)
 ```
 
 ## Reproject fisheye 180 to equirectangular
 ```python
-snap_configs = [SnapConfig( rot(yaw,pitch), (800,800),(90,90), fisheye180_img.shape[:2], source_img_type="fisheye180") 
+snap_configs = [SnapConfig( rot(yaw,pitch), (800,800),(90,90), fisheye180_img.shape[:2], source_img_type=ImageProjectionType.FISHEYE_180) 
                     for yaw,pitch in [[-45,-45],[45,-45],[-45,45],[45,45],[0,0]]]
 snaps = [SphereSnap(c) for c in snap_configs]
 snap_imgs = [snap.snap_to_perspective(fisheye180_img) for snap in snaps]
 
 reconstructed_equi = SphereSnap.merge_multiple_snaps((1000,2000), 
                                                      snaps, # snap object specifies destination position
                                                      snap_imgs, # snap image contains planar image pixels
-                                                     target_type="equi", # destination image type
+                                                     target_type=ImageProjectionType.EQUI, # destination image type
                                                      merge_method="max")
 
 ```
```

