# Comparing `tmp/odc-geo-0.3.3.tar.gz` & `tmp/odc-geo-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odc-geo-0.3.3.tar", last modified: Tue Dec 27 23:46:45 2022, max compression
+gzip compressed data, was "odc-geo-0.4.0a1.tar", last modified: Mon May  1 01:17:20 2023, max compression
```

## Comparing `odc-geo-0.3.3.tar` & `odc-geo-0.4.0a1.tar`

### file list

```diff
@@ -1,44 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 23:46:45.158183 odc-geo-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-27 23:46:33.000000 odc-geo-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-27 23:46:33.000000 odc-geo-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2022-12-27 23:46:45.158183 odc-geo-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2022-12-27 23:46:33.000000 odc-geo-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 23:46:45.154183 odc-geo-0.3.3/odc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 23:46:45.158183 odc-geo-0.3.3/odc/geo/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/_cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/_rgba.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    24643 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/_xr_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14454 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/crs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 23:46:45.158183 odc-geo-0.3.3/odc/geo/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/data/gbox.css
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/data/ocean.geojson.xz
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    40027 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/geobox.py
--rw-r--r--   0 runner    (1001) docker     (123)    41911 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/gridspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    18441 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/overlap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13709 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-27 23:46:33.000000 odc-geo-0.3.3/odc/geo/xr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 23:46:45.158183 odc-geo-0.3.3/odc_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2022-12-27 23:46:45.000000 odc-geo-0.3.3/odc_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-27 23:46:45.000000 odc-geo-0.3.3/odc_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 23:46:45.000000 odc-geo-0.3.3/odc_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 23:46:44.000000 odc-geo-0.3.3/odc_geo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-27 23:46:45.000000 odc-geo-0.3.3/odc_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-27 23:46:45.000000 odc-geo-0.3.3/odc_geo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-27 23:46:33.000000 odc-geo-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-27 23:46:45.162183 odc-geo-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 23:46:33.000000 odc-geo-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:17:19.996806 odc-geo-0.4.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-01 01:17:19.996806 odc-geo-0.4.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:17:19.988805 odc-geo-0.4.0a1/odc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:17:19.992805 odc-geo-0.4.0a1/odc/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26932 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/_xr_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/crs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:17:19.992805 odc-geo-0.4.0a1/odc/geo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/data/gbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/data/ocean.geojson.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42911 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/geobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42282 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18443 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/odc/geo/xr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:17:19.992805 odc-geo-0.4.0a1/odc_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-01 01:17:19.000000 odc-geo-0.4.0a1/odc_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-01 01:17:19.000000 odc-geo-0.4.0a1/odc_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 01:17:19.000000 odc-geo-0.4.0a1/odc_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 01:17:19.000000 odc-geo-0.4.0a1/odc_geo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 01:17:19.000000 odc-geo-0.4.0a1/odc_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-01 01:17:19.000000 odc-geo-0.4.0a1/odc_geo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-01 01:17:19.996806 odc-geo-0.4.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 01:17:19.996806 odc-geo-0.4.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_dask_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_gbox_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_geobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_geoboxtiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31468 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_rioxarray_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-05-01 01:16:56.000000 odc-geo-0.4.0a1/tests/test_xr_interop.py
```

### Comparing `odc-geo-0.3.3/LICENSE` & `odc-geo-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/PKG-INFO` & `odc-geo-0.4.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.3.3
+Version: 0.4.0a1
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-geo-0.3.3/README.rst` & `odc-geo-0.4.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/__init__.py` & `odc-geo-0.4.0a1/odc/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/_cog.py` & `odc-geo-0.4.0a1/odc/geo/_cog.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
         return align_up(dim, 16)
     return align_up(block, 16)
 
 
 def _default_cog_opts(
     *, blocksize: int = 512, shape: SomeShape = (0, 0), is_float: bool = False, **other
 ) -> Dict[str, Any]:
-
     nx, ny = shape_(shape).xy
     return dict(
         tiled=True,
         blockxsize=_adjust_blocksize(blocksize, nx),
         blockysize=_adjust_blocksize(blocksize, ny),
         zlevel=6,
         predictor=3 if is_float else 2,
@@ -77,15 +76,14 @@
 
 
 def _norm_compression_opts(
     compression: Union[bool, str, Dict[str, Any]],
     default_compress: str = "deflate",
     default_zlevel: int = 2,
 ) -> Dict[str, Any]:
-
     if isinstance(compression, bool):
         if compression:
             return {"compress": default_compress, "zlevel": default_zlevel}
         return {"compress": None}
     if isinstance(compression, str):
         compression = {"compress": compression}
     return compression
```

### Comparing `odc-geo-0.3.3/odc/geo/_compress.py` & `odc-geo-0.4.0a1/odc/geo/_compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "png": ("PNG", "zlevel", "image/png"),
     "jpeg": ("JPEG", "quality", "image/jpeg"),
     "webp": ("WEBP", "quality", "image/webp"),
 }
 
 
 def _compress_image(im: np.ndarray, driver="PNG", **opts) -> bytes:
-
     if im.ndim > 2:
         im = np.squeeze(im)
 
     if im.ndim == 3:
         h, w, nc = im.shape
         bands = np.transpose(im, axes=(2, 0, 1))  # Y,X,B -> B,Y,X
     elif im.ndim == 2:
```

### Comparing `odc-geo-0.3.3/odc/geo/_interop.py` & `odc-geo-0.4.0a1/odc/geo/_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/_map.py` & `odc-geo-0.4.0a1/odc/geo/_map.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/_rgba.py` & `odc-geo-0.4.0a1/odc/geo/_rgba.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/_xr_interop.py` & `odc-geo-0.4.0a1/odc/geo/_xr_interop.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
 from ._interop import have, is_dask_collection
 from ._rgba import colorize, to_rgba
 from .crs import CRS, CRSError, SomeCRS, norm_crs_or_error
 from .gcp import GCPGeoBox, GCPMapping
 from .geobox import Coordinate, GeoBox
 from .geom import Geometry
-from .math import affine_from_axis
+from .math import affine_from_axis, resolution_from_affine
 from .overlap import compute_output_geobox
-from .types import Resolution, resxy_, xy_
+from .types import Resolution, xy_
 
 # pylint: disable=import-outside-toplevel
 if have.rasterio:
     from ._cog import to_cog, write_cog
     from ._compress import compress
     from ._map import add_to
     from .warp import rio_reproject
@@ -54,14 +54,15 @@
 @dataclass
 class GeoState:
     """
     Geospatial information for xarray object.
     """
 
     spatial_dims: Optional[Tuple[str, str]] = None
+    crs_coord: Optional[xarray.DataArray] = None
     transform: Optional[Affine] = None
     crs: Optional[CRS] = None
     geobox: Optional[SomeGeoBox] = None
     gcp: Optional[GCPMapping] = None
 
 
 def _get_crs_from_attrs(obj: XarrayObject, sdims: Tuple[str, str]) -> Optional[CRS]:
@@ -150,24 +151,28 @@
     return None
 
 
 def _mk_crs_coord(
     crs: CRS,
     name: str = _DEFAULT_CRS_COORD_NAME,
     gcps=None,
+    transform: Optional[Affine] = None,
 ) -> xarray.DataArray:
     # pylint: disable=protected-access
 
     cf = crs.proj.to_cf()
     epsg = 0 if crs.epsg is None else crs.epsg
     crs_wkt = cf.get("crs_wkt", None) or crs.wkt
 
     if gcps is not None:
         cf["gcps"] = _gcps_to_json(gcps)
 
+    if transform is not None:
+        cf["GeoTransform"] = " ".join(map(str, transform.to_gdal()))
+
     return xarray.DataArray(
         numpy.asarray(epsg, "int32"),
         name=name,
         dims=(),
         attrs={"spatial_ref": crs_wkt, **cf},
     )
 
@@ -253,34 +258,39 @@
     """
     attrs = {}
     crs = gbox.crs
     if crs is not None:
         attrs["crs"] = str(crs)
 
     gcps = None
+    transform: Optional[Affine] = None
 
     if isinstance(gbox, GCPGeoBox):
         coords: Dict[Hashable, xarray.DataArray] = {
             name: _mk_pixel_coord(name, sz, None)
             for name, sz in zip(gbox.dimensions, gbox.shape)
         }
         gcps = gbox.gcps()
-    elif gbox.axis_aligned:
-        coords = {
-            name: _coord_to_xr(name, coord, **attrs)
-            for name, coord in gbox.coordinates.items()
-        }
     else:
-        coords = {
-            name: _mk_pixel_coord(name, sz, gbox.transform)
-            for name, sz in zip(gbox.dimensions, gbox.shape)
-        }
+        transform = gbox.transform
+        if gbox.axis_aligned:
+            coords = {
+                name: _coord_to_xr(name, coord, **attrs)
+                for name, coord in gbox.coordinates.items()
+            }
+        else:
+            coords = {
+                name: _mk_pixel_coord(name, sz, transform)
+                for name, sz in zip(gbox.dimensions, gbox.shape)
+            }
 
     if crs_coord_name is not None and crs is not None:
-        coords[crs_coord_name] = _mk_crs_coord(crs, crs_coord_name, gcps=gcps)
+        coords[crs_coord_name] = _mk_crs_coord(
+            crs, crs_coord_name, gcps=gcps, transform=transform
+        )
 
     return coords
 
 
 def _mk_pixel_coord(
     name: str,
     sz: int,
@@ -343,72 +353,107 @@
             for f in gcps["features"]
         ]
         return GCPMapping(pix, wld)
     except (IndexError, KeyError, ValueError):
         return None
 
 
-def _extract_transform(src: XarrayObject, sdims: Tuple[str, str]) -> Optional[Affine]:
+def _extract_geo_transform(crs_coord: xarray.DataArray) -> Optional[Affine]:
+    geo_transfrom_parts = crs_coord.attrs.get("GeoTransform", "").split(" ")
+    if len(geo_transfrom_parts) != 6:
+        return None
+    try:
+        c, a, b, f, d, e = map(float, geo_transfrom_parts)
+    except ValueError:
+        return None
+
+    return Affine.from_gdal(c, a, b, f, d, e)
+
+
+def _extract_transform(
+    src: XarrayObject,
+    sdims: Tuple[str, str],
+    crs_coord: Optional[xarray.DataArray],
+    gcp: bool,
+) -> Optional[Affine]:
     if any(dim not in src.coords for dim in sdims):
         # special case of no spatial dims at all
-        # happens for GCP sources loaded by rioxarray
-        return None
+        # happens for GCP/rotated sources loaded by rioxarray
+        if gcp or crs_coord is None:
+            return None
+        return _extract_geo_transform(crs_coord)
 
     _yy, _xx = (src[dim] for dim in sdims)
-    rx, ry = (coord.attrs.get("resolution", None) for coord in (_xx, _yy))
-    fallback_res = None
-    if rx is not None and ry is not None:
-        fallback_res = resxy_(float(rx), float(ry))
 
+    # First try to compute from 1-D X/Y coords
     try:
-        transform = affine_from_axis(_xx.values, _yy.values, fallback_res)
+        transform = affine_from_axis(_xx.values, _yy.values)
     except ValueError:
-        # this can fail when any dimension is shorter than 2 elements
-        return None
+        # This can fail when any dimension is shorter than 2 elements
+        # Figure out fallback resolution if possible and try again
+        if crs_coord is None:
+            return None
+        if (original_transform := _extract_geo_transform(crs_coord)) is None:
+            return None
+        try:
+            transform = affine_from_axis(
+                _xx.values,
+                _yy.values,
+                resolution_from_affine(original_transform),
+            )
+        except ValueError:
+            return None
 
-    _pix2world = _xx.encoding.get("_transform", None)
-    if _pix2world is not None:
+    if not gcp and (_pix2world := _xx.encoding.get("_transform", None)) is not None:
         # non-axis aligned geobox detected
         # adjust transform
         #  world <- pix' <- pix
         transform = Affine(*_pix2world) * transform
     return transform
 
 
 def _locate_geo_info(src: XarrayObject) -> GeoState:
     # pylint: disable=too-many-locals
     sdims = spatial_dims(src, relaxed=True)
     if sdims is None:
         return GeoState()
 
-    transform = _extract_transform(src, sdims)
+    crs_coord: Optional[xarray.DataArray] = None
     crs: Optional[CRS] = None
     geobox: Optional[SomeGeoBox] = None
     gcp: Optional[GCPMapping] = None
 
     ny, nx = (src.coords[dim].shape[0] for dim in sdims)
 
     _crs_coords = _locate_crs_coords(src)
     num_candidates = len(_crs_coords)
     if num_candidates > 0:
         if num_candidates > 1:
             warnings.warn("Multiple CRS coordinates are present")
-        crs = _extract_crs(_crs_coords[0])
-        gcp = _extract_gcps(_crs_coords[0])
+        crs_coord = _crs_coords[0]
+        crs = _extract_crs(crs_coord)
+        gcp = _extract_gcps(crs_coord)
     else:
         # try looking in attributes
         crs = _get_crs_from_attrs(src, sdims)
 
+    transform = _extract_transform(src, sdims, crs_coord, gcp is not None)
+
     if gcp is not None:
         geobox = GCPGeoBox((ny, nx), gcp, transform)
     elif transform is not None:
         geobox = GeoBox((ny, nx), transform, crs)
 
     return GeoState(
-        spatial_dims=sdims, transform=transform, crs=crs, geobox=geobox, gcp=gcp
+        spatial_dims=sdims,
+        crs_coord=crs_coord,
+        transform=transform,
+        crs=crs,
+        geobox=geobox,
+        gcp=gcp,
     )
 
 
 def _wrap_op(method: F) -> F:
     @functools.wraps(method, assigned=("__doc__",))
     def wrapped(*args, **kw):
         # pylint: disable=protected-access
@@ -501,40 +546,54 @@
         raise ValueError("Can not reproject non-georegistered array.")
 
     if isinstance(how, GeoBox):
         dst_geobox = how
     else:
         dst_geobox = src.odc.output_geobox(how)
 
-    if is_dask_collection(src):
-        raise NotImplementedError("Dask inputs are not yet supported.")
-
     # compute destination shape by replacing spatial dimensions shape
     ydim = src.odc.ydim
     assert ydim + 1 == src.odc.xdim
     dst_shape = (*src.shape[:ydim], *dst_geobox.shape, *src.shape[ydim + 2 :])
 
-    dst = numpy.empty(dst_shape, dtype=src.dtype)
     src_nodata = kw.pop("src_nodata", None)
     if src_nodata is None:
         src_nodata = src.odc.nodata
     if dst_nodata is None:
         dst_nodata = src_nodata
 
-    dst = rio_reproject(
-        src.values,
-        dst,
-        src_gbox,
-        dst_geobox,
-        resampling=resampling,
-        src_nodata=src_nodata,
-        dst_nodata=dst_nodata,
-        ydim=ydim,
-        **kw,
-    )
+    if is_dask_collection(src):
+        # raise NotImplementedError("Dask inputs are not yet supported.")
+
+        from ._dask import _dask_rio_reproject
+
+        dst: Any = _dask_rio_reproject(
+            src.data,
+            src_gbox,
+            dst_geobox,
+            resampling=resampling,
+            src_nodata=src_nodata,
+            dst_nodata=dst_nodata,
+            ydim=ydim,
+            **kw,
+        )
+    else:
+        dst = numpy.empty(dst_shape, dtype=src.dtype)
+
+        dst = rio_reproject(
+            src.values,
+            dst,
+            src_gbox,
+            dst_geobox,
+            resampling=resampling,
+            src_nodata=src_nodata,
+            dst_nodata=dst_nodata,
+            ydim=ydim,
+            **kw,
+        )
 
     attrs = src.attrs.copy()
     if dst_nodata is None:
         attrs.pop("nodata", None)
         attrs.pop("_FillValue", None)
     else:
         attrs.update(nodata=dst_nodata)
@@ -711,41 +770,55 @@
 def wrap_xr(
     im: Any,
     gbox: SomeGeoBox,
     *,
     time=None,
     nodata=None,
     crs_coord_name: Optional[str] = _DEFAULT_CRS_COORD_NAME,
+    axis: Optional[int] = None,
     **attrs,
 ) -> xarray.DataArray:
     """
     Wrap xarray around numpy array with CRS and x,y coords.
 
     :param im: numpy array to wrap, last two axes are Y,X
     :param gbox: Geobox, must same shape as last two axis of ``im``
     :param time: optional time axis value(s), defaults to None
     :param nodata: optional `nodata` value, defaults to None
     :param attrs: Any other attributes to set on the result
     :return: xarray DataArray
     """
-    assert im.shape[-2:] == gbox.shape
+    if axis is None:
+        axis = 1 if time is not None else 0
+
+    if im.ndim == 2 and axis == 1:
+        im = im[numpy.newaxis, ...]
 
-    prefix_dims: Tuple[str, ...] = ("time",) if im.ndim > 2 else ()
+    assert axis in (0, 1)  # upto 1 extra dimension on the left only
+    assert im.ndim - axis - 2 in (0, 1)  # upto 1 extra dimension on the right only
+    assert im.shape[axis : axis + 2] == gbox.shape
 
-    dims = (*prefix_dims, *gbox.dimensions)
+    prefix_dims: Tuple[str, ...] = ("time",) if axis == 1 else ()
+    postfix_dims: Tuple[str, ...] = ("band",) if im.ndim - axis > 2 else ()
+
+    dims = (*prefix_dims, *gbox.dimensions, *postfix_dims)
     coords = xr_coords(gbox, crs_coord_name=crs_coord_name)
 
     if time is not None:
         if not isinstance(time, xarray.DataArray):
             if len(prefix_dims) > 0 and isinstance(time, (str, datetime)):
                 time = [time]
 
             time = xarray.DataArray(time, dims=prefix_dims).astype("datetime64[ns]")
 
         coords["time"] = time
+    if postfix_dims:
+        coords["band"] = xarray.DataArray(
+            [f"b{i}" for i in range(im.shape[-1])], dims=postfix_dims
+        )
 
     if nodata is not None:
         attrs = dict(nodata=nodata, **attrs)
 
     out = xarray.DataArray(im, coords=coords, dims=dims, attrs=attrs)
     if crs_coord_name is not None:
         out.encoding["grid_mapping"] = crs_coord_name
```

### Comparing `odc-geo-0.3.3/odc/geo/converters.py` & `odc-geo-0.4.0a1/odc/geo/converters.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/crs.py` & `odc-geo-0.4.0a1/odc/geo/crs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/data/__init__.py` & `odc-geo-0.4.0a1/odc/geo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/data/gbox.css` & `odc-geo-0.4.0a1/odc/geo/data/gbox.css`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/data/ocean.geojson.xz` & `odc-geo-0.4.0a1/odc/geo/data/ocean.geojson.xz`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/gcp.py` & `odc-geo-0.4.0a1/odc/geo/gcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 from affine import Affine
 
 from .crs import CRS, MaybeCRS, SomeCRS, norm_crs
 from .geobox import GeoBox, GeoBoxBase
 from .geom import Geometry, multipoint
 from .math import Poly2d, affine_from_pts, align_up, resolution_from_affine, unstack_xy
-from .types import XY, MaybeInt, Resolution, SomeShape, wh_
+from .types import XY, MaybeInt, Resolution, SomeResolution, SomeShape, wh_
 
 SomePointSet = Union[np.ndarray, Geometry, List[Geometry], List[XY[float]]]
 
 
 def _points_to_array(pts: SomePointSet) -> Tuple[np.ndarray, Optional[CRS]]:
     if isinstance(pts, np.ndarray):
         return pts, None
@@ -251,24 +251,29 @@
 
         :returns:
            GCPGeoBox covering the same region but with different pixels (i.e. lower or higher resolution)
         """
         _shape, _affine = self.compute_zoom_out(factor)
         return GCPGeoBox(_shape, self._mapping, _affine)
 
-    def zoom_to(self, shape: Union[SomeShape, int, float]) -> "GCPGeoBox":
+    def zoom_to(
+        self,
+        shape: Union[SomeShape, int, float, None] = None,
+        *,
+        resolution: Optional[SomeResolution] = None,
+    ) -> "GCPGeoBox":
         """
         Compute :py:class:`~odc.geo.geobox.GCPGeoBox` with changed resolution.
 
         When supplied a single integer scale longest dimension to match that.
 
         :returns:
           GCPGeoBox covering the same region but with different number of pixels and therefore resolution.
         """
-        _shape, _affine = self.compute_zoom_to(shape)
+        _shape, _affine = self.compute_zoom_to(shape, resolution=resolution)
         return GCPGeoBox(_shape, self._mapping, _affine)
 
     def __str__(self):
         return self.__repr__()
 
     def __repr__(self) -> str:
         return f"GCPGeoBox({self._shape.xy!r}, {self.crs!r})"
```

### Comparing `odc-geo-0.3.3/odc/geo/geobox.py` & `odc-geo-0.4.0a1/odc/geo/geobox.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,46 +3,64 @@
 # Copyright (c) 2015-2020 ODC Contributors
 # SPDX-License-Identifier: Apache-2.0
 import importlib
 import itertools
 import math
 from collections import OrderedDict, namedtuple
 from enum import Enum
-from typing import Dict, Iterable, List, Literal, Optional, Tuple, Union
+from typing import (
+    Dict,
+    Iterable,
+    List,
+    Literal,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import numpy
 from affine import Affine
 
 from . import geom
-from .crs import CRS, CRSMismatchError, MaybeCRS, SomeCRS, norm_crs
-from .geom import BoundingBox, Geometry, bbox_intersection, bbox_union
+from .crs import CRS, MaybeCRS, SomeCRS, norm_crs
+from .geom import BoundingBox, Geometry, bbox_intersection, bbox_union, intersects
 from .math import (
     clamp,
     is_affine_st,
     is_almost_int,
     maybe_zero,
     resolution_from_affine,
     snap_grid,
     split_translation,
 )
-from .roi import Tiles as RoiTiles
-from .roi import align_up, roi_boundary, roi_normalise, roi_shape
+from .roi import (
+    RoiTiles,
+    align_up,
+    clip_tiles,
+    roi_boundary,
+    roi_normalise,
+    roi_shape,
+    roi_tiles,
+)
 from .types import (
+    ROI,
     XY,
-    Index2d,
+    Chunks2d,
     MaybeInt,
     NormalizedROI,
     OutlineMode,
     Resolution,
     Shape2d,
     SomeIndex2d,
     SomeResolution,
     SomeShape,
     Unset,
-    iyx_,
+    func2map,
     res_,
     shape_,
     xy_,
 )
 
 
 class AnchorEnum(Enum):
@@ -305,24 +323,35 @@
 
     def compute_zoom_out(self, factor: float) -> Tuple[Shape2d, Affine]:
         ny, nx = (max(1, math.ceil(s / factor)) for s in self.shape)
         A = self._affine * Affine.scale(factor, factor)
         return (shape_((ny, nx)), A)
 
     def compute_zoom_to(
-        self, shape: Union[SomeShape, int, float]
+        self,
+        shape: Union[SomeShape, int, float, None] = None,
+        *,
+        resolution: Optional[SomeResolution] = None,
     ) -> Tuple[Shape2d, Affine]:
         """
         Change GeoBox shape.
 
         When supplied a single integer scale longest dimension to match that.
 
         :returns:
           GeoBox covering the same region but with different number of pixels and therefore resolution.
         """
+        if shape is None:
+            if resolution is None:
+                raise ValueError("Have to supply shape or resolution")
+            new_geobox = GeoBox.from_bbox(
+                self.boundingbox, resolution=resolution, tight=True
+            )
+            return new_geobox.shape, new_geobox.affine
+
         if isinstance(shape, (int, float)):
             nmax = max(*self._shape)
             return self.compute_zoom_out(nmax / shape)
 
         shape = shape_(shape)
         sy, sx = (N / float(n) for N, n in zip(self._shape, shape.shape))
         A = self._affine * Affine.scale(sx, sy)
@@ -373,14 +402,17 @@
         References: http://extremelearning.com.au/unreasonable-effectiveness-of-quasirandom-sequences/
         """
         nx, ny = self._shape.xy
         return BoundingBox(0, 0, nx, ny, None).qr2sample(
             n, padding=padding, with_edges=with_edges, offset=offset
         )
 
+    def __getitem__(self, roi) -> "GeoBoxBase":
+        raise NotImplementedError()
+
 
 class GeoBox(GeoBoxBase):
     """
     Defines the location and resolution of a rectangular grid of data,
     including it's :py:class:`~odc.geo.crs.CRS`.
 
     :param shape: Shape in pixels ``(ny, nx)``
@@ -830,24 +862,29 @@
 
         :returns:
            GeoBox covering the same region but with different pixels (i.e. lower or higher resolution)
         """
         _shape, _affine = self.compute_zoom_out(factor)
         return GeoBox(_shape, _affine, self._crs)
 
-    def zoom_to(self, shape: Union[SomeShape, int, float]) -> "GeoBox":
+    def zoom_to(
+        self,
+        shape: Union[SomeShape, int, float, None] = None,
+        *,
+        resolution: Optional[SomeResolution] = None,
+    ) -> "GeoBox":
         """
         Change GeoBox shape.
 
         When supplied a single integer scale longest dimension to match that.
 
         :returns:
           GeoBox covering the same region but with different number of pixels and therefore resolution.
         """
-        _shape, _affine = self.compute_zoom_to(shape)
+        _shape, _affine = self.compute_zoom_to(shape, resolution=resolution)
         return GeoBox(_shape, _affine, self._crs)
 
     def flipy(self) -> "GeoBox":
         """
         Flip along Y axis.
 
         :returns: GeoBox covering the same region but with Y-axis flipped
@@ -1126,17 +1163,22 @@
 
 
 def zoom_out(gbox: GeoBox, factor: float) -> GeoBox:
     """Alias for :py:meth:`odc.geo.geobox.GeoBox.zoom_out`."""
     return gbox.zoom_out(factor)
 
 
-def zoom_to(gbox: GeoBox, shape: SomeShape) -> GeoBox:
+def zoom_to(
+    gbox: GeoBox,
+    shape: Union[SomeShape, int, float, None] = None,
+    *,
+    resolution: Optional[SomeResolution] = None,
+) -> GeoBox:
     """Alias for :py:meth:`odc.geo.geobox.GeoBox.zoom_to`."""
-    return gbox.zoom_to(shape)
+    return gbox.zoom_to(shape, resolution=resolution)
 
 
 def rotate(gbox: GeoBox, deg: float) -> GeoBox:
     """Alias for :py:meth:`odc.geo.geobox.GeoBox.`."""
     return gbox.rotate(deg)
 
 
@@ -1144,27 +1186,38 @@
     """Alias for :py:meth:`odc.geo.geobox.GeoBox.__mul__`."""
     return gbox * transform
 
 
 class GeoboxTiles:
     """Partition GeoBox into sub geoboxes."""
 
-    def __init__(self, box: GeoBox, tile_shape: SomeShape):
+    __slots__ = ("_gbox", "_tiles")
+
+    def __init__(
+        self,
+        box: GeoBoxBase,
+        tile_shape: Union[SomeShape, Chunks2d, None],
+        *,
+        _tiles: Optional[RoiTiles] = None,
+    ):
         """
         Construct from a :py:class:`~odc.geo.GeoBox`.
 
         :param box: source :py:class:`~odc.geo.GeoBox`
         :param tile_shape: Shape of sub-tiles in pixels ``(rows, cols)``
         """
         self._gbox = box
-        self._tiles = RoiTiles(box.shape, tile_shape)
-        self._cache: Dict[Index2d, GeoBox] = {}
+        if _tiles is not None:
+            self._tiles = _tiles
+        else:
+            assert tile_shape is not None
+            self._tiles = roi_tiles(box.shape, tile_shape)
 
     @property
-    def base(self) -> GeoBox:
+    def base(self) -> GeoBoxBase:
         """Access base Geobox"""
         return self._gbox
 
     @property
     def shape(self) -> Shape2d:
         """Number of tiles along each dimension."""
         return self._tiles.shape
@@ -1187,67 +1240,123 @@
 
         :param idx: ``(row, col)`` chunk index
         :returns: ``(nrows, ncols)`` shape of a tile (edge tiles might be smaller)
         :raises: :py:class:`IndexError` when index is outside of ``[(0,0) -> .shape)``.
         """
         return self._tiles.tile_shape(idx)
 
-    def __getitem__(self, idx: SomeIndex2d) -> GeoBox:
+    @property
+    def chunks(self) -> Chunks2d:
+        return self._tiles.chunks
+
+    def _crop(self, roi: ROI) -> "GeoboxTiles":
+        gbox_new = self.base[self._tiles[roi]]
+        return GeoboxTiles(gbox_new, (0, 0), _tiles=self._tiles.crop(roi))
+
+    def clip(
+        self, selection: Sequence[Tuple[int, int]]
+    ) -> Tuple["GeoboxTiles", List[Tuple[int, int]]]:
+        """
+        Crop to a set of tiles.
+
+        Returns cropped version of :py:class:`GeoboxTiles` and a list of
+        tile coordinates in the new, cropped space.
+        """
+        tiles, roi, new_idx = clip_tiles(self._tiles, selection)
+        return GeoboxTiles(self[roi], None, _tiles=tiles), new_idx
+
+    @property
+    def crop(self) -> Mapping[ROI, "GeoboxTiles"]:
+        return func2map(self._crop)
+
+    def __getitem__(self, idx: Union[SomeIndex2d, ROI]) -> GeoBoxBase:
         """
         Lookup tile by index, index is in matrix access order: ``(row, col)``.
 
         :param idx: ``(row, col)`` index
         :returns: GeoBox of a tile
         :raises: IndexError when index is outside of ``[(0,0) -> .shape)``
         """
-        idx = iyx_(idx)
-        sub_gbox = self._cache.get(idx, None)
-        if sub_gbox is not None:
-            return sub_gbox
-
-        roi = self._tiles[idx]
-        return self._cache.setdefault(idx, self._gbox[roi])
+        return self._gbox[self._tiles[idx]]
 
     def range_from_bbox(self, bbox: BoundingBox) -> Tuple[range, range]:
         """
         Intersect with a bounding box.
 
         Compute rows and columns overlapping with a given :py:class:`~odc.geo.geom.BoundingBox`.
         """
 
-        def clamped_range(v1: float, v2: float, N: int) -> range:
-            _in = clamp(math.floor(v1), 0, N)
-            _out = clamp(math.ceil(v2), 0, N)
-            return range(_in, _out)
-
-        if bbox.crs != self._gbox.crs:
-            raise CRSMismatchError()
-
-        sy, sx = self._tiles.tile_shape((0, 0)).yx
-        A = Affine.scale(1.0 / sx, 1.0 / sy) * (~self._gbox.transform)
-        # A maps from X,Y in meters to chunk index
-        bbox = bbox.transform(A)
-
-        NY, NX = self._tiles.shape.yx
-        xx = clamped_range(bbox.left, bbox.right, NX)
-        yy = clamped_range(bbox.bottom, bbox.top, NY)
-        return (yy, xx)
+        if bbox.crs is not None:
+            bbox = self._gbox.project(bbox.polygon).boundingbox
+
+        def _clamp(span: Tuple[float, float], N: int):
+            a1, a2 = span
+            a1 = int(clamp(math.floor(a1), 0, N - 1))
+            a2 = int(clamp(math.ceil(a2), 1, N)) - 1
+            return a1, a2
+
+        NY, NX = self._gbox.shape.yx
+        x1, x2 = _clamp(bbox.range_x, NX)
+        y1, y2 = _clamp(bbox.range_y, NY)
+
+        y1, x1 = self._tiles.locate((y1, x1))
+        y2, x2 = self._tiles.locate((y2, x2))
+
+        return range(y1, y2 + 1), range(x1, x2 + 1)
 
     def tiles(self, polygon: Geometry) -> Iterable[Tuple[int, int]]:
         """Return tile indexes overlapping with a given geometry."""
         target_crs = self._gbox.crs
         poly = polygon
         if target_crs is not None and poly.crs != target_crs:
             poly = poly.to_crs(target_crs)
 
         yy, xx = self.range_from_bbox(poly.boundingbox)
         for idx in itertools.product(yy, xx):
             gbox = self[idx]
-            if gbox.extent.intersects(poly):
+            if intersects(gbox.extent, poly):
                 yield idx
 
+    def grid_intersect(
+        self, src: "GeoboxTiles"
+    ) -> Dict[Tuple[int, int], List[Tuple[int, int]]]:
+        """
+        Figure out tile to tile overlap graph between two grids.
+
+        For every tile in this :py:class:`GeoboxTiles` find every tile in ``other`` that
+        intersects with this ``tile``.
+        """
+        if src.base.crs == self.base.crs:
+            src_footprint = src.base.extent
+        else:
+            # compute "robust" source footprint in CRS of self via espg:4326
+            src_footprint = (
+                src.base.footprint(4326, 2) & self.base.footprint(4326, 2)
+            ).to_crs(self.base.crs)
+
+        xy_chunks_with_data = list(self.tiles(src_footprint))
+        deps: Dict[Tuple[int, int], List[Tuple[int, int]]] = {}
+
+        for idx in xy_chunks_with_data:
+            geobox = self[idx]
+            deps[idx] = list(src.tiles(geobox.extent))
+
+        return deps
+
     def __dask_tokenize__(self):
         return (
             "odc.geo.geobox.GeoboxTiles",
-            *self._tiles.shape.yx,
             *self._gbox.__dask_tokenize__()[1:],
+            *self._tiles.__dask_tokenize__()[1:],
         )
+
+    def __str__(self):
+        return str(self.roi)
+
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, GeoboxTiles):
+            return False
+        if self is __value:
+            return True
+        return self._tiles == __value._tiles and self._gbox == __value._gbox
+
+    __repr__ = __str__
```

### Comparing `odc-geo-0.3.3/odc/geo/geom.py` & `odc-geo-0.4.0a1/odc/geo/geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     Iterator,
     List,
+    Literal,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 import numpy
@@ -629,15 +630,15 @@
     def _to_crs(self, crs: CRS) -> "Geometry":
         assert self.crs is not None
         return Geometry(ops.transform(self.crs.transformer_to_crs(crs), self.geom), crs)
 
     def to_crs(
         self,
         crs: SomeCRS,
-        resolution: Optional[float] = None,
+        resolution: Union[float, Literal["auto"], None] = None,
         wrapdateline: bool = False,
     ) -> "Geometry":
         """
         Convert geometry to a different Coordinate Reference System.
 
         :param crs:
           CRS to convert to
@@ -664,14 +665,17 @@
         crs = norm_crs_or_error(crs, self)
         if self.crs == crs:
             return self
 
         if self.crs is None:
             raise ValueError("Cannot project geometries without CRS")
 
+        if resolution == "auto":
+            resolution = _auto_resolution(self)
+
         if resolution is not None and math.isfinite(resolution):
             geom = self.segmented(resolution)
         else:
             geom = self
 
         eps = 1e-4
         if wrapdateline and crs.geographic:
@@ -1259,18 +1263,20 @@
         if crs != bb.crs:
             raise CRSMismatchError((crs, bb.crs))
 
     return BoundingBox(L, B, R, T, crs)
 
 
 def lonlat_bounds(
-    geom: Geometry, mode: str = "safe", resolution: Optional[float] = None
+    geom: Geometry,
+    mode: str = "safe",
+    resolution: Union[float, None, Literal["auto"]] = None,
 ) -> BoundingBox:
     """
-    Return the bounding box of a geometry.
+    Return the bounding box of a geometry in lon/lat.
 
     :param geom:
        Geometry in any projection
     :param mode:
        safe|quick
     :param resolution:
        If supplied will first segmentize input geometry to have no segment longer than
@@ -1279,14 +1285,17 @@
     assert mode in ("safe", "quick")
     if geom.crs is None:
         raise ValueError("lonlat_bounds can only operate on Geometry with CRS defined")
 
     if geom.crs.geographic:
         return geom.boundingbox
 
+    if resolution == "auto":
+        resolution = _auto_resolution(geom)
+
     if resolution is not None and math.isfinite(resolution):
         geom = geom.segmented(resolution)
 
     bbox = geom.to_crs("EPSG:4326").boundingbox
 
     xx_range = bbox.range_x
     if mode == "safe":
@@ -1302,16 +1311,21 @@
             #       to poles.
             xx_ = [x + 360 if x < 0 else x for x in bbox.range_x]
             xx_range_ = min(xx_), max(xx_)
             span_x_ = xx_range_[1] - xx_range_[0]
             if span_x_ < bbox.span_x:
                 xx_range = xx_range_
 
-    return BoundingBox.from_xy(xx_range, bbox.range_y)
+    return BoundingBox.from_xy(xx_range, bbox.range_y, crs=4326)
 
 
 def mid_longitude(geom: Geometry) -> float:
     """
     Compute longitude of the center point of a geometry.
     """
     ((lon,), _) = geom.centroid.to_crs("epsg:4326").xy
     return lon
+
+
+def _auto_resolution(g: Geometry) -> float:
+    # aim for ~100 points per side of a square
+    return math.sqrt(g.area) * 4 / 100
```

### Comparing `odc-geo-0.3.3/odc/geo/gridspec.py` & `odc-geo-0.4.0a1/odc/geo/gridspec.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/math.py` & `odc-geo-0.4.0a1/odc/geo/math.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/overlap.py` & `odc-geo-0.4.0a1/odc/geo/overlap.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
 
     (sx, _, tx, _, sy, ty, *_) = A_  # tx, ty are in dst pixel space
 
     # Expect identity for scale change
     if any(abs(abs(s) - 1) > stol for s in (sx, sy)):  # not equal scaling across axis?
         return False, "sx!=sy, probably"
 
-    # Check is sub-pixel translation is within bounds
+    # Check if sub-pixel translation within bounds
     if not all(is_almost_int(t, ttol) for t in (tx, ty)):
         return False, "sub-pixel translation"
 
     return True, None
 
 
 def _relative_rois(
@@ -606,15 +606,15 @@
         cp_bbox = cp.extent.to_crs(dst_crs).boundingbox
         dst_ = GeoBox.from_bbox(cp_bbox, dst_crs, shape=(1, 1), tight=True)
 
         # further adjust that via fitting
         #  Y = tr(X) => Y ~= s*X + t
         # where X is in `dst_` and Y is in `gbox`
         # .. so a better fit resolution is `_dst.res / s`
-        # .. but we want square pixels so pick average between x/y
+        # .. but we want square pixels, so pick average between x and y
         sx, sy = get_scale_at_point(xy_(0.5, 0.5), native_pix_transform(dst_, cp)).xy
 
         # always produces square pixels on output with inverted Y axis
         avg_res = (abs(dst_.resolution.x / sx) + abs(dst_.resolution.y / sy)) / 2
         res = res_(avg_res)
     else:
         raise ValueError(
```

### Comparing `odc-geo-0.3.3/odc/geo/testutils.py` & `odc-geo-0.4.0a1/odc/geo/testutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import xarray as xr
 from affine import Affine
 
 from . import CRS
 from .geobox import GeoBox
 from .gridspec import GridSpec
-from .math import apply_affine
+from .math import apply_affine, maybe_int
 
 # pylint: disable=invalid-name,
 
 epsg4326 = CRS("EPSG:4326")
 epsg3577 = CRS("EPSG:3577")
 epsg3857 = CRS("EPSG:3857")
 esri54019 = CRS("ESRI:54019")
@@ -197,14 +197,15 @@
 def purge_crs_info(xx: xr.DataArray) -> xr.DataArray:
     attributes_to_clear = ["crs", "wkt", "crs_wkt", "transform", "epsg", "resolution"]
 
     def _purge_attributes(_x: xr.DataArray) -> xr.DataArray:
         for attr in attributes_to_clear:
             _x.attrs.pop(attr, None)
         _x.encoding.pop("grid_mapping", None)
+        _x.encoding.pop("_transform", None)
         return _x
 
     # remove non-dimensional coordinate, which is CRS in our case
     to_drop = [name for name in xx.coords if name not in xx.dims]
     xx = xx.drop_vars(to_drop)
 
     # purge attributes from coords and xx
@@ -221,7 +222,19 @@
 
     return xr.DataArray(
         data=da.from_array(xx.data, **kw),
         dims=xx.dims,
         coords=xx.coords,
         attrs=xx.attrs,
     )
+
+
+def approx_equal_affine(a: Affine, b: Affine, tol: float = 1e-6) -> bool:
+    sx, z1, tx, z2, sy, ty = map(lambda v: maybe_int(v, tol), (~a * b)[:6])
+    return (sx, z1, tx, z2, sy, ty) == (1, 0, 0, 0, 1, 0)
+
+
+def approx_equal_geobox(a: GeoBox, b: GeoBox, tol: float = 1e-6) -> bool:
+    if a.shape != b.shape or a.crs != b.crs:
+        return False
+
+    return approx_equal_affine(a.transform, b.transform, tol)
```

### Comparing `odc-geo-0.3.3/odc/geo/types.py` & `odc-geo-0.4.0a1/odc/geo/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import (
     Callable,
     Generic,
     Iterable,
     Iterator,
     List,
     Literal,
+    Mapping,
     Optional,
     Protocol,
     Sequence,
     Tuple,
     TypeVar,
     Union,
     cast,
@@ -17,14 +18,16 @@
 )
 
 MaybeInt = Optional[int]
 MaybeFloat = Optional[float]
 T = TypeVar("T")
 T1 = TypeVar("T1")
 T2 = TypeVar("T2")
+TK = TypeVar("TK")
+TV = TypeVar("TV")
 
 
 class Unset:
     """
     Marker for unset values.
 
     Used where ``None`` can be a valid value.
@@ -218,14 +221,15 @@
     def __radd__(self, other):
         return other + self.shape
 
 
 SomeShape = Union[Tuple[int, int], XY[int], Shape2d, Index2d]
 SomeIndex2d = Union[Tuple[int, int], XY[int], Index2d]
 SomeResolution = Union[float, int, Resolution]
+Chunks2d = Tuple[Tuple[int, ...], Tuple[int, ...]]
 
 
 class SupportsCoords(Protocol[T]):
     """
     Needed for Point geometry -> XY conversion.
     """
 
@@ -393,15 +397,15 @@
 
 
 def wh_(w: int, h: int, /) -> Shape2d:
     """Shape from width/height."""
     return Shape2d(x=w, y=h)
 
 
-def shape_(x: SomeShape) -> Shape2d:
+def shape_(x: Union[SomeShape, Tuple[int, ...]]) -> Shape2d:
     """Normalise shape representation."""
     if isinstance(x, Shape2d):
         return x
     if isinstance(x, XY):
         nx, ny = x.map(int).xy
         return Shape2d(x=nx, y=ny)
     if isinstance(x, Sequence):
@@ -443,7 +447,41 @@
 
 NormalizedROI = Tuple[NormalizedSlice, NormalizedSlice]
 """Normalized 2d slice into an image plane."""
 
 OutlineMode = Union[
     Literal["native"], Literal["pixel"], Literal["geo"], Literal["auto"]
 ]
+
+
+class _Func2Map(Mapping[TK, TV]):
+    """
+    Turn ``f(K)`` into ``ff[K]``.
+    """
+
+    __slots__ = ("_func", "_keys")
+
+    def __init__(self, func: Callable[[TK], TV], keys: Sequence[TK]):
+        self._func = func
+        self._keys = keys
+
+    def __getitem__(self, idx: TK) -> TV:
+        return self._func(idx)
+
+    def __len__(self) -> int:
+        return len(self._keys)
+
+    def __iter__(self) -> Iterator[TK]:
+        yield from self._keys
+
+
+def func2map(
+    f: Callable[[TK], TV],
+    keys: Optional[Sequence[TK]] = None,
+) -> Mapping[TK, TV]:
+    """
+    Turn ``f(K) -> V`` into ``ff[K] -> V``.
+
+    :param f: Callable mapping ``K -> V``
+    :param keys: Optional sequence of valid keys
+    """
+    return _Func2Map(f, [] if keys is None else keys)
```

### Comparing `odc-geo-0.3.3/odc/geo/ui.py` & `odc-geo-0.4.0a1/odc/geo/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,14 @@
 
     def _display_bbox(self, pad_fraction: float = 0.1):
         bbox = self._src.geographic_extent.boundingbox
         pad_deg = max(bbox.span_x, bbox.span_y) * pad_fraction
         return bbox.buffered(pad_deg)
 
     def _render_svg(self, sz=360):
-
         if self._crs is None:
             bbox = self._src.extent.boundingbox
             margin = 0.1 * max(bbox.span_x, bbox.span_y)
             bbox = bbox.buffered(margin)
             return make_svg(
                 self,
                 bbox=bbox,
```

### Comparing `odc-geo-0.3.3/odc/geo/warp.py` & `odc-geo-0.4.0a1/odc/geo/warp.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc/geo/xr.py` & `odc-geo-0.4.0a1/odc/geo/xr.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.3.3/odc_geo.egg-info/PKG-INFO` & `odc-geo-0.4.0a1/odc_geo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.3.3
+Version: 0.4.0a1
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-geo-0.3.3/pyproject.toml` & `odc-geo-0.4.0a1/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
   "invalid-name",
   "fixme",
   "wrong-import-order",
   "cyclic-import",
   "ungrouped-imports",
   "wrong-import-position",
   "too-few-public-methods",
-]
+]
```

### Comparing `odc-geo-0.3.3/setup.cfg` & `odc-geo-0.4.0a1/setup.cfg`

 * *Files identical despite different names*

