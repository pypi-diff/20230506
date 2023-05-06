# Comparing `tmp/odc-geo-0.4.0a2.tar.gz` & `tmp/odc-geo-0.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odc-geo-0.4.0a2.tar", last modified: Fri May  5 23:06:16 2023, max compression
+gzip compressed data, was "odc-geo-0.4.0a3.tar", last modified: Sat May  6 06:29:29 2023, max compression
```

## Comparing `odc-geo-0.4.0a2.tar` & `odc-geo-0.4.0a3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:06:16.902299 odc-geo-0.4.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-05 23:06:16.902299 odc-geo-0.4.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:06:16.894299 odc-geo-0.4.0a2/odc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:06:16.898299 odc-geo-0.4.0a2/odc/geo/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_rgba.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27139 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/_xr_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/crs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:06:16.898299 odc-geo-0.4.0a2/odc/geo/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/data/gbox.css
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/data/ocean.geojson.xz
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    42911 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/geobox.py
--rw-r--r--   0 runner    (1001) docker     (123)    42282 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/gridspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    18443 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/overlap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/odc/geo/xr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:06:16.898299 odc-geo-0.4.0a2/odc_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-05 23:06:16.000000 odc-geo-0.4.0a2/odc_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-05 23:06:16.000000 odc-geo-0.4.0a2/odc_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:06:16.000000 odc-geo-0.4.0a2/odc_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:06:16.000000 odc-geo-0.4.0a2/odc_geo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 23:06:16.000000 odc-geo-0.4.0a2/odc_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 23:06:16.000000 odc-geo-0.4.0a2/odc_geo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-05 23:06:16.902299 odc-geo-0.4.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:06:16.902299 odc-geo-0.4.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_dask_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_gbox_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_geobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_geoboxtiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    31468 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_gridspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_overlap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_rgba.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_rioxarray_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    17925 2023-05-05 23:06:04.000000 odc-geo-0.4.0a2/tests/test_xr_interop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:29:29.980272 odc-geo-0.4.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-06 06:29:29.980272 odc-geo-0.4.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:29:29.972272 odc-geo-0.4.0a3/odc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:29:29.976272 odc-geo-0.4.0a3/odc/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27222 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/_xr_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/crs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:29:29.976272 odc-geo-0.4.0a3/odc/geo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/data/gbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/data/ocean.geojson.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42911 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/geobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42282 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18443 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/odc/geo/xr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:29:29.976272 odc-geo-0.4.0a3/odc_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-06 06:29:29.000000 odc-geo-0.4.0a3/odc_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-06 06:29:29.000000 odc-geo-0.4.0a3/odc_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:29:29.000000 odc-geo-0.4.0a3/odc_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:29:29.000000 odc-geo-0.4.0a3/odc_geo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-06 06:29:29.000000 odc-geo-0.4.0a3/odc_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 06:29:29.000000 odc-geo-0.4.0a3/odc_geo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-06 06:29:29.980272 odc-geo-0.4.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:29:29.980272 odc-geo-0.4.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_dask_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_gbox_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_geobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_geoboxtiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31468 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_gridspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_rgba.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_rioxarray_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-05-06 06:29:17.000000 odc-geo-0.4.0a3/tests/test_xr_interop.py
```

### Comparing `odc-geo-0.4.0a2/LICENSE` & `odc-geo-0.4.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/PKG-INFO` & `odc-geo-0.4.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-geo-0.4.0a2/README.rst` & `odc-geo-0.4.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/__init__.py` & `odc-geo-0.4.0a3/odc/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/_blocks.py` & `odc-geo-0.4.0a3/odc/geo/_blocks.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/_cog.py` & `odc-geo-0.4.0a3/odc/geo/_cog.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/_compress.py` & `odc-geo-0.4.0a3/odc/geo/_compress.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/_dask.py` & `odc-geo-0.4.0a3/odc/geo/_dask.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/_interop.py` & `odc-geo-0.4.0a3/odc/geo/_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/_map.py` & `odc-geo-0.4.0a3/odc/geo/_map.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/_rgba.py` & `odc-geo-0.4.0a3/odc/geo/_rgba.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/_xr_interop.py` & `odc-geo-0.4.0a3/odc/geo/_xr_interop.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,15 +542,15 @@
 
     if have.rasterio is False:  # pragma: nocover
         raise RuntimeError("Please install `rasterio` to use this method")
 
     assert isinstance(src.odc, ODCExtensionDa)  # for mypy sake
     src_gbox = src.odc.geobox
 
-    if src_gbox is None:
+    if src_gbox is None or src_gbox.crs is None:
         raise ValueError("Can not reproject non-georegistered array.")
 
     if isinstance(how, GeoBox):
         dst_geobox = how
     else:
         dst_geobox = src.odc.output_geobox(how)
 
@@ -597,15 +597,17 @@
     if dst_nodata is None:
         attrs.pop("nodata", None)
         attrs.pop("_FillValue", None)
     else:
         attrs.update(nodata=dst_nodata)
 
     # new set of coords (replace x,y dims)
-    coords = dict((k, v) for k, v in src.coords.items() if k not in src.dims)
+    sdims = src.odc.spatial_dims
+    assert sdims is not None
+    coords = dict((k, v) for k, v in src.coords.items() if k not in sdims)
     coords.update(xr_coords(dst_geobox))
 
     dims = (*src.dims[:ydim], *dst_geobox.dimensions, *src.dims[ydim + 2 :])
 
     out = xarray.DataArray(dst, coords=coords, dims=dims, attrs=attrs)
     out.encoding["grid_mapping"] = _DEFAULT_CRS_COORD_NAME
     return out
```

### Comparing `odc-geo-0.4.0a2/odc/geo/converters.py` & `odc-geo-0.4.0a3/odc/geo/converters.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/crs.py` & `odc-geo-0.4.0a3/odc/geo/crs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/data/__init__.py` & `odc-geo-0.4.0a3/odc/geo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/data/gbox.css` & `odc-geo-0.4.0a3/odc/geo/data/gbox.css`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/data/ocean.geojson.xz` & `odc-geo-0.4.0a3/odc/geo/data/ocean.geojson.xz`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/gcp.py` & `odc-geo-0.4.0a3/odc/geo/gcp.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/geobox.py` & `odc-geo-0.4.0a3/odc/geo/geobox.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/geom.py` & `odc-geo-0.4.0a3/odc/geo/geom.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/gridspec.py` & `odc-geo-0.4.0a3/odc/geo/gridspec.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/math.py` & `odc-geo-0.4.0a3/odc/geo/math.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/overlap.py` & `odc-geo-0.4.0a3/odc/geo/overlap.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/roi.py` & `odc-geo-0.4.0a3/odc/geo/roi.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/testutils.py` & `odc-geo-0.4.0a3/odc/geo/testutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,15 @@
         _x.encoding.pop("grid_mapping", None)
         _x.encoding.pop("_transform", None)
         return _x
 
     # remove non-dimensional coordinate, which is CRS in our case
     to_drop = [name for name in xx.coords if name not in xx.dims]
     xx = xx.drop_vars(to_drop)
+    xx.encoding.pop("grid_spatial", None)
 
     # purge attributes from coords and xx
     cc = {name: _purge_attributes(coord) for name, coord in xx.coords.items()}
     return _purge_attributes(xx.assign_coords(cc))
 
 
 def daskify(xx, **kw):
```

### Comparing `odc-geo-0.4.0a2/odc/geo/types.py` & `odc-geo-0.4.0a3/odc/geo/types.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/ui.py` & `odc-geo-0.4.0a3/odc/geo/ui.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/warp.py` & `odc-geo-0.4.0a3/odc/geo/warp.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc/geo/xr.py` & `odc-geo-0.4.0a3/odc/geo/xr.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/odc_geo.egg-info/PKG-INFO` & `odc-geo-0.4.0a3/odc_geo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odc-geo
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: Geometry Classes and Operations (opendatacube)
 Home-page: https://github.com/opendatacube/odc-geo/
 Author: Open Data Cube
 Author-email: 
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
```

### Comparing `odc-geo-0.4.0a2/odc_geo.egg-info/SOURCES.txt` & `odc-geo-0.4.0a3/odc_geo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/pyproject.toml` & `odc-geo-0.4.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/setup.cfg` & `odc-geo-0.4.0a3/setup.cfg`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_bbox.py` & `odc-geo-0.4.0a3/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_blocks.py` & `odc-geo-0.4.0a3/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_cog.py` & `odc-geo-0.4.0a3/tests/test_cog.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_converters.py` & `odc-geo-0.4.0a3/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_crs.py` & `odc-geo-0.4.0a3/tests/test_crs.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_dask_interop.py` & `odc-geo-0.4.0a3/tests/test_dask_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_datasets.py` & `odc-geo-0.4.0a3/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_gbox_ops.py` & `odc-geo-0.4.0a3/tests/test_gbox_ops.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_gcp.py` & `odc-geo-0.4.0a3/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_geobox.py` & `odc-geo-0.4.0a3/tests/test_geobox.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_geoboxtiles.py` & `odc-geo-0.4.0a3/tests/test_geoboxtiles.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_geom.py` & `odc-geo-0.4.0a3/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_gridspec.py` & `odc-geo-0.4.0a3/tests/test_gridspec.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_map.py` & `odc-geo-0.4.0a3/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_math.py` & `odc-geo-0.4.0a3/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_overlap.py` & `odc-geo-0.4.0a3/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_rgba.py` & `odc-geo-0.4.0a3/tests/test_rgba.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_rioxarray_interop.py` & `odc-geo-0.4.0a3/tests/test_rioxarray_interop.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_roi.py` & `odc-geo-0.4.0a3/tests/test_roi.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_types.py` & `odc-geo-0.4.0a3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_ui.py` & `odc-geo-0.4.0a3/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `odc-geo-0.4.0a2/tests/test_xr_interop.py` & `odc-geo-0.4.0a3/tests/test_xr_interop.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,29 @@
 @pytest.fixture
 def geobox_epsg4326():
     _box = geom.box(-20, -10, 20, 10, "epsg:4326")
     yield GeoBox.from_geopolygon(_box, 5)
 
 
 @pytest.fixture
-def xx_epsg4326(geobox_epsg4326: GeoBox):
-    yield xr_zeros(geobox_epsg4326, dtype="uint16")
+def xx_chunks():
+    yield None
+
+
+@pytest.fixture
+def xx_time():
+    yield None
+
+
+@pytest.fixture
+def xx_epsg4326(geobox_epsg4326: GeoBox, xx_time, xx_chunks):
+    if xx_time is not None and xx_chunks is not None:
+        if len(xx_chunks) < 3:
+            xx_chunks = (-1, *xx_chunks)
+    yield xr_zeros(geobox_epsg4326, dtype="uint16", chunks=xx_chunks, time=xx_time)
 
 
 def test_geobox_xr_coords():
     A = mkA(0, scale=(10, -10), translation=(-48800, -2983006))
 
     w, h = 512, 256
     _shape = h, w
@@ -360,14 +373,16 @@
     assert xx.time.dt.month.values[0] == 2
 
     xx = wrap_xr(data[..., np.newaxis], gbox)
     assert xx.shape == (*gbox.shape, 1)
     assert xx.band.data.tolist() == ["b0"]
 
 
+@pytest.mark.parametrize("xx_time", [None, ["2020-01-30"]])
+@pytest.mark.parametrize("xx_chunks", [None, (-1, -1), (4, 4)])
 def test_xr_reproject(xx_epsg4326: xr.DataArray):
     assert isinstance(xx_epsg4326.odc, ODCExtensionDa)
     xx0 = xx_epsg4326
     xx0.attrs["crs"] = "epsg:4326"
     # smoke-test only
     assert isinstance(xx_epsg4326.odc.geobox, GeoBox)
     assert xx_epsg4326.odc.nodata is None
@@ -407,18 +422,21 @@
     assert xx.odc.nodata is None
 
     # check dst_nodata override
     xx = xx_epsg4326.odc.reproject("epsg:3857", dst_nodata=255)
     assert xx.odc.nodata == 255
 
     # multi-time should work just the same
-    xx2 = xx_epsg4326.expand_dims(time=2).odc.reproject("epsg:3857", dst_nodata=255)
-    assert xx2.shape[0] == 2
-    np.testing.assert_array_equal(xx2[0], xx)
-    np.testing.assert_array_equal(xx2[1], xx)
+    if "time" in xx_epsg4326.dims:
+        assert (xx_epsg4326.time == xx.time).all()
+    else:
+        xx2 = xx_epsg4326.expand_dims(time=2).odc.reproject("epsg:3857", dst_nodata=255)
+        assert xx2.shape[0] == 2
+        np.testing.assert_array_equal(xx2[0], xx)
+        np.testing.assert_array_equal(xx2[1], xx)
 
     xx_i8 = xx_epsg4326.astype("int8")
     assert xx_i8.odc.reproject("epsg:3857").dtype == "int8"
 
     # non-georegistered case
     with pytest.raises(ValueError):
         _ = purge_crs_info(xx_epsg4326).odc.reproject(dst_gbox)
```

