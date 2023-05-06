# Comparing `tmp/segment-geospatial-0.3.0.tar.gz` & `tmp/segment-geospatial-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.3.0.tar", last modified: Wed Apr 26 15:21:47 2023, max compression
+gzip compressed data, was "segment-geospatial-0.4.0.tar", last modified: Sat May  6 04:53:40 2023, max compression
```

## Comparing `segment-geospatial-0.3.0.tar` & `segment-geospatial-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39601 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/samgeo/samgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/setup.py
```

### Comparing `segment-geospatial-0.3.0/LICENSE` & `segment-geospatial-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.3.0/PKG-INFO` & `segment-geospatial-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.3.0
+Version: 0.4.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -28,25 +28,33 @@
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
--   Documentation: https://samgeo.gishub.org
+-   Documentation: <https://samgeo.gishub.org>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+-   Visualize segmentation results on interactive maps
 
 ## Examples
 
-- [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
+
+## Demos
+
+-   Automatic mask generator
+
+![](https://i.imgur.com/I1IhDgz.gif)
 
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
```

### Comparing `segment-geospatial-0.3.0/README.md` & `segment-geospatial-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,25 +7,33 @@
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
--   Documentation: https://samgeo.gishub.org
+-   Documentation: <https://samgeo.gishub.org>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+-   Visualize segmentation results on interactive maps
 
 ## Examples
 
-- [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
+
+## Demos
+
+-   Automatic mask generator
+
+![](https://i.imgur.com/I1IhDgz.gif)
 
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
```

### Comparing `segment-geospatial-0.3.0/samgeo/common.py` & `segment-geospatial-0.4.0/samgeo/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import cv2
 import numpy as np
 import rasterio
 from tqdm import tqdm
 
 import shapely
 import geopandas as gpd
+from pyproj import Transformer, transform
 import rasterio
 from rasterio import features
 
 
 def check_file_path(file_path, make_dirs=True):
     """Gets the absolute file path.
 
@@ -176,24 +177,24 @@
         output (str, optional): The output file path. Defaults to None.
         overwrite (bool, optional): Overwrite the file if it already exists. Defaults to False.
 
     Returns:
         str: The output file path.
     """
     checkpoints = {
-        'sam_vit_h_4b8939.pth': "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
-        'sam_vit_l_0b3195.pth': "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
-        'sam_vit_b_01ec64.pth': "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
+        "sam_vit_h_4b8939.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
+        "sam_vit_l_0b3195.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
+        "sam_vit_b_01ec64.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
     }
 
     if isinstance(url, str) and url in checkpoints:
         url = checkpoints[url]
 
     if url is None:
-        url = checkpoints['sam_vit_h_4b8939.pth']
+        url = checkpoints["sam_vit_h_4b8939.pth"]
 
     if output is None:
         output = os.path.basename(url)
 
     return download_file(url, output, overwrite=overwrite, **kwargs)
 
 
@@ -576,14 +577,70 @@
             reproject(output, output, crs, to_cog=to_cog)
         elif to_cog:
             image_to_cog(output, output)
     except Exception as e:
         raise Exception(e)
 
 
+def get_profile(src_fp):
+    with rasterio.open(src_fp) as src:
+        return src.profile
+
+
+def get_crs(src_fp):
+    with rasterio.open(src_fp) as src:
+        return src.crs
+
+
+def get_features(src_fp, bidx=1):
+    with rasterio.open(src_fp) as src:
+        features = rasterio.features.dataset_features(
+            src,
+            bidx=bidx,
+            sampling=1,
+            band=True,
+            as_mask=False,
+            with_nodata=False,
+            geographic=True,
+            precision=-1,
+        )
+        gdf = gpd.GeoDataFrame.from_features(features)
+        gdf.set_crs(src.crs)
+        return gdf
+
+
+def set_transform(geo_box, width, height):
+    return rasterio.transform.from_bounds(*geo_box, width, height)
+
+
+def transform_coords(x, y, src_crs, dst_crs):
+    transformer = Transformer.from_crs(src_crs, dst_crs, always_xy=True)
+    return transformer.transform(x, y)
+
+
+def get_pixel_coords(src_fp, xs, ys):
+    with rasterio.open(src_fp) as src:
+        rows, cols = rasterio.transform.rowcol(src.transform, xs, ys)
+        box = np.array([min(cols), min(rows), max(cols), max(rows)])
+    return box
+
+
+def write_features(gdf, dst_fp):
+    gdf.to_file(dst_fp)
+
+
+def write_raster(dst_fp, dst_arr, profile, width, height, transform, crs):
+    profile.update({"driver": "GTiff", "nodata": "0"})
+    with rasterio.open(dst_fp, "w", **profile) as dst:
+        if len(dst_arr.shape) == 2:
+            dst_arr = dst_arr[np.newaxis, ...]
+        for i in range(dst_arr.shape[0]):
+            dst.write(dst_arr[i], i + 1)
+
+
 def chw_to_hwc(block):
     # Grab first 3 channels
     block = block[:3, ...]
     # CHW to HWC
     block = np.transpose(block, (1, 2, 0))
     return block
 
@@ -603,19 +660,19 @@
     for y in range(-bound, raster_h, h):
         for x in range(-bound, raster_w, w):
             rigth_x_bound = max(bound, x + width - raster_w)
             bottom_y_bound = max(bound, y + height - raster_h)
 
             blocks.append(
                 {
-                    'x': x,
-                    'y': y,
-                    'height': height,
-                    'width': width,
-                    'bounds': [[bound, bottom_y_bound], [bound, rigth_x_bound]],
+                    "x": x,
+                    "y": y,
+                    "height": height,
+                    "width": width,
+                    "bounds": [[bound, bottom_y_bound], [bound, rigth_x_bound]],
                 }
             )
     return blocks
 
 
 def read_block(src, x, y, height, width, nodata=0, **kwargs):
     return src.read(
@@ -645,52 +702,54 @@
     sample_resize=None,
     bound=128,
 ):
     with rasterio.open(src_fp) as src:
         profile = src.profile
 
         # Computer blocks
-        rh, rw = profile['height'], profile['width']
+        rh, rw = profile["height"], profile["width"]
         sh, sw = sample_size
         bound = bound
 
         resize_hw = sample_resize
 
+        # Subdivide image into tiles
         sample_grid = calculate_sample_grid(
             raster_h=rh, raster_w=rw, sample_h=sh, sample_w=sw, bound=bound
         )
         # set 1 channel uint8 output
-        profile['count'] = 1
-        profile['dtype'] = 'uint8'
+        profile["count"] = 1
+        profile["dtype"] = "uint8"
 
-        with rasterio.open(dst_fp, 'w', **profile) as dst:
+        with rasterio.open(dst_fp, "w", **profile) as dst:
             for b in tqdm(sample_grid):
+                # Read each tile from the source
                 r = read_block(src, **b)
-
+                # Extract the first 3 channels as RGB
                 uint8_rgb_in = data_to_rgb(r)
                 orig_size = uint8_rgb_in.shape[:2]
                 if resize_hw is not None:
                     uint8_rgb_in = cv2.resize(
                         uint8_rgb_in, resize_hw, interpolation=cv2.INTER_LINEAR
                     )
 
-                # Do something
+                # Run the model, call the __call__ method of SamGeo class
                 uin8_out = func(uint8_rgb_in)
 
                 if resize_hw is not None:
                     uin8_out = cv2.resize(
                         uin8_out, orig_size, interpolation=cv2.INTER_NEAREST
                     )
-                # Zero channel, because
+                # Write the output to the destination
                 write_block(dst, uin8_out, **b)
 
 
 def image_to_image(image, func, sample_size=(384, 384), sample_resize=None, bound=128):
     with tempfile.NamedTemporaryFile() as src_tmpfile:
-        s, b = cv2.imencode('.tif', image)
+        s, b = cv2.imencode(".tif", image)
         src_tmpfile.write(b.tobytes())
         src_fp = src_tmpfile.name
         with tempfile.NamedTemporaryFile() as dst_tmpfile:
             dst_fp = dst_tmpfile.name
             tiff_to_tiff(
                 src_fp,
                 dst_fp,
@@ -896,7 +955,293 @@
     xyz_dict = get_xyz_dict(free_only=free_only)
     for item in xyz_dict:
         name = xyz_dict[item].name
         url = xyz_dict[item].build_url()
         basemaps[name] = url
 
     return basemaps
+
+
+def array_to_image(
+    array, output, source=None, dtype=None, compress="deflate", **kwargs
+):
+    """Save a NumPy array as a GeoTIFF using the projection information from an existing GeoTIFF file.
+
+    Args:
+        array (np.ndarray): The NumPy array to be saved as a GeoTIFF.
+        output (str): The path to the output image.
+        source (str, optional): The path to an existing GeoTIFF file with map projection information. Defaults to None.
+        dtype (np.dtype, optional): The data type of the output array. Defaults to None.
+        compress (str, optional): The compression method. Can be one of the following: "deflate", "lzw", "packbits", "jpeg". Defaults to "deflate".
+    """
+
+    from PIL import Image
+
+    if isinstance(array, str) and os.path.exists(array):
+        array = cv2.imread(array)
+        array = cv2.cvtColor(array, cv2.COLOR_BGR2RGB)
+
+    if output.endswith(".tif") and source is not None:
+        with rasterio.open(source) as src:
+            crs = src.crs
+            transform = src.transform
+            if compress is None:
+                compress = src.compression
+
+        # Determine the minimum and maximum values in the array
+        min_value = np.min(array)
+        max_value = np.max(array)
+
+        if dtype is None:
+            # Determine the best dtype for the array
+            if min_value >= 0 and max_value <= 1:
+                dtype = np.float32
+            elif min_value >= 0 and max_value <= 255:
+                dtype = np.uint8
+            elif min_value >= -128 and max_value <= 127:
+                dtype = np.int8
+            elif min_value >= 0 and max_value <= 65535:
+                dtype = np.uint16
+            elif min_value >= -32768 and max_value <= 32767:
+                dtype = np.int16
+            else:
+                dtype = np.float64
+
+        # Convert the array to the best dtype
+        array = array.astype(dtype)
+
+        # Define the GeoTIFF metadata
+        if array.ndim == 2:
+            metadata = {
+                "driver": "GTiff",
+                "height": array.shape[0],
+                "width": array.shape[1],
+                "count": 1,
+                "dtype": array.dtype,
+                "crs": crs,
+                "transform": transform,
+            }
+        elif array.ndim == 3:
+            metadata = {
+                "driver": "GTiff",
+                "height": array.shape[0],
+                "width": array.shape[1],
+                "count": array.shape[2],
+                "dtype": array.dtype,
+                "crs": crs,
+                "transform": transform,
+            }
+
+        if compress is not None:
+            metadata["compress"] = compress
+        else:
+            raise ValueError("Array must be 2D or 3D.")
+
+        # Create a new GeoTIFF file and write the array to it
+        with rasterio.open(output, "w", **metadata) as dst:
+            if array.ndim == 2:
+                dst.write(array, 1)
+            elif array.ndim == 3:
+                for i in range(array.shape[2]):
+                    dst.write(array[:, :, i], i + 1)
+
+    else:
+        img = Image.fromarray(array)
+        img.save(output, **kwargs)
+
+
+def show_image(
+    source, figsize=(20, 20), cmap=None, axis="off", fig_args={}, show_args={}, **kwargs
+):
+    import matplotlib.pyplot as plt
+
+    if isinstance(source, str):
+        if source.startswith("http"):
+            source = download_file(source)
+
+        if not os.path.exists(source):
+            raise ValueError(f"Input path {source} does not exist.")
+
+        source = cv2.imread(source)
+        source = cv2.cvtColor(source, cv2.COLOR_BGR2RGB)
+
+    plt.figure(figsize=figsize, **fig_args)
+    plt.imshow(source, cmap=cmap, **show_args)
+    plt.axis(axis)
+    plt.show(**kwargs)
+
+
+def overlay_images(
+    image1,
+    image2,
+    opacity=0.5,
+    backend="TkAgg",
+    height_ratios=[10, 1],
+    show_args1={},
+    show_args2={},
+):
+    import sys
+    import matplotlib
+    import matplotlib.widgets as mpwidgets
+    import matplotlib.pyplot as plt
+
+    if "google.colab" in sys.modules:
+        backend = "inline"
+        print(
+            "The TkAgg backend is not supported in Google Colab. The overlay_images function will not work on Colab."
+        )
+        return
+
+    matplotlib.use(backend)
+
+    if isinstance(image1, str):
+        if image1.startswith("http"):
+            image1 = download_file(image1)
+
+        if not os.path.exists(image1):
+            raise ValueError(f"Input path {image1} does not exist.")
+
+    if isinstance(image2, str):
+        if image2.startswith("http"):
+            image2 = download_file(image2)
+
+        if not os.path.exists(image2):
+            raise ValueError(f"Input path {image2} does not exist.")
+
+    # Load the two images
+    x = plt.imread(image1)
+    y = plt.imread(image2)
+
+    # Create the plot
+    fig, (ax0, ax1) = plt.subplots(2, 1, gridspec_kw={"height_ratios": height_ratios})
+    img0 = ax0.imshow(x, **show_args1)
+    img1 = ax0.imshow(y, alpha=opacity, **show_args2)
+
+    # Define the update function
+    def update(value):
+        img1.set_alpha(value)
+        fig.canvas.draw_idle()
+
+    # Create the slider
+    slider0 = mpwidgets.Slider(
+        ax=ax1, label="opacity", valmin=0, valmax=1, valinit=opacity
+    )
+    slider0.on_changed(update)
+
+    # Display the plot
+    plt.show()
+
+
+def blend_images(
+    img1,
+    img2,
+    alpha=0.5,
+    output=False,
+    show=True,
+    figsize=(12, 10),
+    axis="off",
+    **kwargs,
+):
+    """
+    Blends two images together using the addWeighted function from the OpenCV library.
+
+    Args:
+        img1 (numpy.ndarray): The first input image on top represented as a NumPy array.
+        img2 (numpy.ndarray): The second input image at the bottom represented as a NumPy array.
+        alpha (float): The weighting factor for the first image in the blend. By default, this is set to 0.5.
+        output (str, optional): The path to the output image. Defaults to False.
+        show (bool, optional): Whether to display the blended image. Defaults to True.
+        figsize (tuple, optional): The size of the figure. Defaults to (12, 10).
+        axis (str, optional): The axis of the figure. Defaults to "off".
+        **kwargs: Additional keyword arguments to pass to the cv2.addWeighted() function.
+
+    Returns:
+        numpy.ndarray: The blended image as a NumPy array.
+    """
+    # Resize the images to have the same dimensions
+    import matplotlib.pyplot as plt
+
+    if isinstance(img1, str):
+        if img1.startswith("http"):
+            img1 = download_file(img1)
+
+        if not os.path.exists(img1):
+            raise ValueError(f"Input path {img1} does not exist.")
+
+        img1 = cv2.imread(img1)
+
+    if isinstance(img2, str):
+        if img2.startswith("http"):
+            img2 = download_file(img2)
+
+        if not os.path.exists(img2):
+            raise ValueError(f"Input path {img2} does not exist.")
+
+        img2 = cv2.imread(img2)
+
+    if img1.dtype == np.float32:
+        img1 = (img1 * 255).astype(np.uint8)
+
+    if img2.dtype == np.float32:
+        img2 = (img2 * 255).astype(np.uint8)
+
+    if img1.dtype != img2.dtype:
+        img2 = img2.astype(img1.dtype)
+
+    img1 = cv2.resize(img1, (img2.shape[1], img2.shape[0]))
+
+    # Blend the images using the addWeighted function
+    beta = 1 - alpha
+    blend_img = cv2.addWeighted(img1, alpha, img2, beta, 0, **kwargs)
+
+    if output:
+        array_to_image(blend_img, output, img2)
+
+    if show:
+        plt.figure(figsize=figsize)
+        plt.imshow(blend_img)
+        plt.axis(axis)
+        plt.show()
+    else:
+        return blend_img
+
+
+def update_package(out_dir=None, keep=False, **kwargs):
+    """Updates the package from the GitHub repository without the need to use pip or conda.
+
+    Args:
+        out_dir (str, optional): The output directory. Defaults to None.
+        keep (bool, optional): Whether to keep the downloaded package. Defaults to False.
+        **kwargs: Additional keyword arguments to pass to the download_file() function.
+    """
+
+    import shutil
+
+    try:
+        if out_dir is None:
+            out_dir = os.getcwd()
+        url = (
+            "https://github.com/opengeos/segment-geospatial/archive/refs/heads/main.zip"
+        )
+        filename = "segment-geospatial-main.zip"
+        download_file(url, filename, **kwargs)
+
+        pkg_dir = os.path.join(out_dir, "segment-geospatial-main")
+        work_dir = os.getcwd()
+        os.chdir(pkg_dir)
+
+        if shutil.which("pip") is None:
+            cmd = "pip3 install ."
+        else:
+            cmd = "pip install ."
+
+        os.system(cmd)
+        os.chdir(work_dir)
+
+        if not keep:
+            shutil.rmtree(pkg_dir)
+            os.remove(filename)
+
+        print("Package updated successfully.")
+
+    except Exception as e:
+        raise Exception(e)
```

### Comparing `segment-geospatial-0.3.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.4.0/segment_geospatial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.3.0
+Version: 0.4.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -28,25 +28,33 @@
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 
 **A Python package for segmenting geospatial data with the Segment Anything Model (SAM)**
 
 The **segment-geospatial** package draws its inspiration from [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository authored by [Aliaksandr Hancharenka](https://github.com/aliaksandr960). To facilitate the use of the Segment Anything Model (SAM) for geospatial data, I have developed the [segment-anything-py](https://github.com/opengeos/segment-anything) and [segment-geospatial](https://github.com/opengeos/segment-geospatial) Python packages, which are now available on PyPI and conda-forge. My primary objective is to simplify the process of leveraging SAM for geospatial data analysis by enabling users to achieve this with minimal coding effort. I have adapted the source code of segment-geospatial from the [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo) repository, and credit for its original version goes to Aliaksandr Hancharenka.
 
 -   Free software: MIT license
--   Documentation: https://samgeo.gishub.org
+-   Documentation: <https://samgeo.gishub.org>
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+-   Visualize segmentation results on interactive maps
 
 ## Examples
 
-- [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
+
+## Demos
+
+-   Automatic mask generator
+
+![](https://i.imgur.com/I1IhDgz.gif)
 
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
```

### Comparing `segment-geospatial-0.3.0/setup.py` & `segment-geospatial-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='samgeo',
     name='segment-geospatial',
     packages=find_packages(include=['samgeo', 'samgeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/segment-geospatial',
-    version='0.3.0',
+    version='0.4.0',
     zip_safe=False,
 )
```

