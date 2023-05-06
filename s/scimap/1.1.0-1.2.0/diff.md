# Comparing `tmp/scimap-1.1.0.tar.gz` & `tmp/scimap-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-1.1.0.tar", max compression
+gzip compressed data, was "scimap-1.2.0.tar", max compression
```

## Comparing `scimap-1.1.0.tar` & `scimap-1.2.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.1.0/README.md
--rw-r--r--   0        0        0     2340 2023-04-22 02:10:04.104712 scimap-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/__init__.py
--rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/__main__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/cli/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-1.1.0/scimap/cli/_scimap_mcmicro.py
--rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-1.1.0/scimap/cli/test.py
--rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.1.0/scimap/helpers/__init__.py
--rwxr-xr-x   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.1.0/scimap/helpers/_addROI_omero.py
--rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.1.0/scimap/helpers/_add_roi_omero.py
--rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.1.0/scimap/helpers/_animate.py
--rwxr-xr-x   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.1.0/scimap/helpers/_classify.py
--rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.1.0/scimap/helpers/_dropFeatures.py
--rwxr-xr-x   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/helpers/_merge_adata_obs.py
--rwxr-xr-x   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/helpers/_rename.py
--rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.1.0/scimap/helpers/_scimap_to_csv.py
--rwxr-xr-x   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/helpers/add_roi_scatter.py
--rw-r--r--   0        0        0      463 2022-05-29 20:43:39.000000 scimap-1.1.0/scimap/plotting/__init__.py
--rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.1.0/scimap/plotting/_addROI_image.py
--rwxr-xr-x   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.1.0/scimap/plotting/_cluster_plots.py
--rwxr-xr-x   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/plotting/_foldchange.py
--rw-r--r--   0        0        0     8423 2022-05-26 00:26:48.000000 scimap-1.1.0/scimap/plotting/_gate_finder.py
--rw-r--r--   0        0        0     8999 2023-04-22 02:05:04.965847 scimap-1.1.0/scimap/plotting/_image_viewer.py
--rwxr-xr-x   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/plotting/_pie.py
--rwxr-xr-x   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.1.0/scimap/plotting/_spatial_distance.py
--rwxr-xr-x   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.1.0/scimap/plotting/_spatial_interaction.py
--rwxr-xr-x   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.1.0/scimap/plotting/_spatial_pscore.py
--rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/plotting/_spatial_scatter.py
--rwxr-xr-x   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.1.0/scimap/plotting/_stacked_barplot.py
--rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.1.0/scimap/plotting/_umap.py
--rwxr-xr-x   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.1.0/scimap/plotting/_voronoi.py
--rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.1.0/scimap/plotting/lasso_selector.py
--rw-r--r--   0        0        0      107 2023-04-20 01:30:26.953137 scimap-1.1.0/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     5078 2023-04-21 02:03:50.459976 scimap-1.1.0/scimap/preprocessing/_combat.py
--rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.1.0/scimap/preprocessing/_mcmicro_to_scimap.py
--rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.1.0/scimap/preprocessing/_rescale.py
--rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/tests/_data/phenotype_workflow.csv
--rwxr-xr-x   0        0        0     1269 2022-05-18 01:22:39.000000 scimap-1.1.0/scimap/tests/test_helpers.py
--rwxr-xr-x   0        0        0      985 2022-06-05 16:22:49.000000 scimap-1.1.0/scimap/tests/test_preprocessing.py
--rwxr-xr-x   0        0        0     4674 2022-04-02 14:45:20.000000 scimap-1.1.0/scimap/tests/test_tools.py
--rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.1.0/scimap/tools/__init__.py
--rwxr-xr-x   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.1.0/scimap/tools/_cluster.py
--rwxr-xr-x   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.1.0/scimap/tools/_foldchange.py
--rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/tools/_phenotype_cells.py
--rwxr-xr-x   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/tools/_spatial_aggregate.py
--rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.1.0/scimap/tools/_spatial_cluster.py
--rwxr-xr-x   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.1.0/scimap/tools/_spatial_count.py
--rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.1.0/scimap/tools/_spatial_distance.py
--rwxr-xr-x   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.1.0/scimap/tools/_spatial_expression.py
--rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.1.0/scimap/tools/_spatial_interaction.py
--rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.1.0/scimap/tools/_spatial_lda.py
--rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.1.0/scimap/tools/_spatial_pscore.py
--rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.1.0/scimap/tools/_spatial_similarity_search.py
--rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.1.0/scimap/tools/_umap.py
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 scimap-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2240 2023-04-15 12:35:07.000000 scimap-1.2.0/README.md
+-rw-r--r--   0        0        0     2369 2023-05-06 15:08:34.186630 scimap-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      299 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/__main__.py
+-rw-r--r--   0        0        0        0 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/cli/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-20 14:28:15.443473 scimap-1.2.0/scimap/cli/_scimap_mcmicro.py
+-rw-r--r--   0        0        0      592 2023-04-20 14:28:51.699589 scimap-1.2.0/scimap/cli/test.py
+-rw-r--r--   0        0        0      257 2022-07-04 23:50:44.000000 scimap-1.2.0/scimap/helpers/__init__.py
+-rwxr-xr-x   0        0        0     6454 2022-05-01 02:47:57.000000 scimap-1.2.0/scimap/helpers/_addROI_omero.py
+-rw-r--r--   0        0        0     6459 2022-05-01 03:13:26.000000 scimap-1.2.0/scimap/helpers/_add_roi_omero.py
+-rw-r--r--   0        0        0    17875 2022-06-01 15:52:05.000000 scimap-1.2.0/scimap/helpers/_animate.py
+-rwxr-xr-x   0        0        0     4944 2022-05-01 16:43:37.000000 scimap-1.2.0/scimap/helpers/_classify.py
+-rw-r--r--   0        0        0     4835 2022-07-06 00:37:53.000000 scimap-1.2.0/scimap/helpers/_dropFeatures.py
+-rwxr-xr-x   0        0        0     3830 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/helpers/_merge_adata_obs.py
+-rwxr-xr-x   0        0        0     2276 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/helpers/_rename.py
+-rw-r--r--   0        0        0     4855 2022-05-26 00:36:56.000000 scimap-1.2.0/scimap/helpers/_scimap_to_csv.py
+-rwxr-xr-x   0        0        0     3141 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/helpers/add_roi_scatter.py
+-rw-r--r--   0        0        0      504 2023-05-06 13:15:57.195162 scimap-1.2.0/scimap/plotting/__init__.py
+-rw-r--r--   0        0        0    16440 2022-05-30 03:05:13.000000 scimap-1.2.0/scimap/plotting/_addROI_image.py
+-rwxr-xr-x   0        0        0     5378 2021-07-02 16:14:28.000000 scimap-1.2.0/scimap/plotting/_cluster_plots.py
+-rwxr-xr-x   0        0        0     6356 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/plotting/_foldchange.py
+-rw-r--r--   0        0        0     8423 2022-05-26 00:26:48.000000 scimap-1.2.0/scimap/plotting/_gate_finder.py
+-rw-r--r--   0        0        0     9403 2023-04-22 02:17:49.145882 scimap-1.2.0/scimap/plotting/_image_viewer.py
+-rwxr-xr-x   0        0        0     6778 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/plotting/_pie.py
+-rwxr-xr-x   0        0        0    12247 2022-08-05 18:19:47.000000 scimap-1.2.0/scimap/plotting/_spatial_distance.py
+-rwxr-xr-x   0        0        0    10520 2022-07-28 19:28:59.000000 scimap-1.2.0/scimap/plotting/_spatial_interaction.py
+-rwxr-xr-x   0        0        0     2837 2023-04-14 19:18:24.000000 scimap-1.2.0/scimap/plotting/_spatial_pscore.py
+-rw-r--r--   0        0        0     1226 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/plotting/_spatial_scatter.py
+-rwxr-xr-x   0        0        0     8776 2021-07-15 16:39:53.000000 scimap-1.2.0/scimap/plotting/_stacked_barplot.py
+-rw-r--r--   0        0        0    11523 2022-05-29 22:46:02.000000 scimap-1.2.0/scimap/plotting/_umap.py
+-rwxr-xr-x   0        0        0    17378 2021-07-12 17:49:48.000000 scimap-1.2.0/scimap/plotting/_voronoi.py
+-rw-r--r--   0        0        0     8425 2023-05-06 15:02:41.773078 scimap-1.2.0/scimap/plotting/densityPlot2D.py
+-rw-r--r--   0        0        0     3341 2020-04-01 13:37:18.000000 scimap-1.2.0/scimap/plotting/lasso_selector.py
+-rw-r--r--   0        0        0      107 2023-04-20 01:30:26.953137 scimap-1.2.0/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5078 2023-04-21 02:03:50.459976 scimap-1.2.0/scimap/preprocessing/_combat.py
+-rw-r--r--   0        0        0     9716 2022-05-29 01:57:56.000000 scimap-1.2.0/scimap/preprocessing/_mcmicro_to_scimap.py
+-rw-r--r--   0        0        0    16550 2022-12-30 21:50:38.000000 scimap-1.2.0/scimap/preprocessing/_rescale.py
+-rw-r--r--   0        0        0  2003213 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1908 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tests/_data/phenotype_workflow.csv
+-rwxr-xr-x   0        0        0     1268 2023-05-06 14:45:48.623561 scimap-1.2.0/scimap/tests/test_helpers.py
+-rwxr-xr-x   0        0        0      984 2023-05-06 14:46:01.108135 scimap-1.2.0/scimap/tests/test_preprocessing.py
+-rwxr-xr-x   0        0        0     4673 2023-05-06 14:46:08.191066 scimap-1.2.0/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0      581 2022-05-29 01:02:42.000000 scimap-1.2.0/scimap/tools/__init__.py
+-rwxr-xr-x   0        0        0    20976 2021-07-02 14:30:55.000000 scimap-1.2.0/scimap/tools/_cluster.py
+-rwxr-xr-x   0        0        0     7389 2022-05-17 01:33:44.000000 scimap-1.2.0/scimap/tools/_foldchange.py
+-rw-r--r--   0        0        0    15522 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tools/_phenotype_cells.py
+-rwxr-xr-x   0        0        0     8047 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tools/_spatial_aggregate.py
+-rw-r--r--   0        0        0     7851 2022-05-05 01:01:59.000000 scimap-1.2.0/scimap/tools/_spatial_cluster.py
+-rwxr-xr-x   0        0        0     7229 2021-07-01 20:47:33.000000 scimap-1.2.0/scimap/tools/_spatial_count.py
+-rw-r--r--   0        0        0     4909 2022-05-26 23:45:54.000000 scimap-1.2.0/scimap/tools/_spatial_distance.py
+-rwxr-xr-x   0        0        0    10750 2022-05-15 00:55:32.000000 scimap-1.2.0/scimap/tools/_spatial_expression.py
+-rw-r--r--   0        0        0    11448 2022-04-28 19:44:16.000000 scimap-1.2.0/scimap/tools/_spatial_interaction.py
+-rw-r--r--   0        0        0     7863 2022-06-10 00:00:59.000000 scimap-1.2.0/scimap/tools/_spatial_lda.py
+-rw-r--r--   0        0        0     9275 2023-04-14 19:20:19.000000 scimap-1.2.0/scimap/tools/_spatial_pscore.py
+-rw-r--r--   0        0        0    18190 2022-06-04 15:12:26.000000 scimap-1.2.0/scimap/tools/_spatial_similarity_search.py
+-rw-r--r--   0        0        0     3939 2022-06-06 16:53:31.000000 scimap-1.2.0/scimap/tools/_umap.py
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 scimap-1.2.0/PKG-INFO
```

### Comparing `scimap-1.1.0/README.md` & `scimap-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/pyproject.toml` & `scimap-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "scimap"
-version = "1.1.0"
+version = "1.2.0"
 description = "Spatial Single-Cell Analysis Toolkit"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
@@ -47,14 +47,15 @@
 numba = ">=0.55.0"
 shapely = "^1.7.1"
 gensim = "^4.0"
 mkdocs-material = "^7.1.1"
 napari-ome-zarr = "^0.4.0"
 llvmlite = "^0.38.0"
 combat = "^0.3.3"
+mpl-scatter-density = "^0.7"
 
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "19.10b0"
 isort = "4.3.21"
```

### Comparing `scimap-1.1.0/scimap/cli/_scimap_mcmicro.py` & `scimap-1.2.0/scimap/cli/_scimap_mcmicro.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/cli/test.py` & `scimap-1.2.0/scimap/cli/test.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/_addROI_omero.py` & `scimap-1.2.0/scimap/helpers/_addROI_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/_add_roi_omero.py` & `scimap-1.2.0/scimap/helpers/_add_roi_omero.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/_animate.py` & `scimap-1.2.0/scimap/helpers/_animate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/_classify.py` & `scimap-1.2.0/scimap/helpers/_classify.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/_dropFeatures.py` & `scimap-1.2.0/scimap/helpers/_dropFeatures.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/_merge_adata_obs.py` & `scimap-1.2.0/scimap/helpers/_merge_adata_obs.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/_rename.py` & `scimap-1.2.0/scimap/helpers/_rename.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/_scimap_to_csv.py` & `scimap-1.2.0/scimap/helpers/_scimap_to_csv.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/helpers/add_roi_scatter.py` & `scimap-1.2.0/scimap/helpers/add_roi_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_addROI_image.py` & `scimap-1.2.0/scimap/plotting/_addROI_image.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_cluster_plots.py` & `scimap-1.2.0/scimap/plotting/_cluster_plots.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_foldchange.py` & `scimap-1.2.0/scimap/plotting/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_gate_finder.py` & `scimap-1.2.0/scimap/plotting/_gate_finder.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_image_viewer.py` & `scimap-1.2.0/scimap/plotting/_image_viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 !!! abstract "Short Description"
     `sm.pl.image_viewer`: The function allows users to open OME-TIFF images inside 
     Napari and overlay any any categorical column such as cluster annotation or phenotypes.
 
 ## Function
 """
 
-#%gui qt
+# %gui qt
 try:
     import napari
 except:
     pass
 import pandas as pd
 import random
 import tifffile as tiff
@@ -23,210 +23,256 @@
 from dask.cache import Cache
 import zarr
 import os
 
 cache = Cache(2e9)  # Leverage two gigabytes of memory
 cache.register()
 
-def image_viewer (image_path, adata, overlay=None, flip_y=True,
-                    overlay_category=None,markers=None,channel_names='default',
-                    x_coordinate='X_centroid',y_coordinate='Y_centroid',point_size=10,
-                    point_color=None,subset=None,imageid='imageid',seg_mask=None,**kwargs):
+
+def image_viewer(
+    image_path,
+    adata,
+    overlay=None,
+    flip_y=True,
+    overlay_category=None,
+    markers=None,
+    channel_names='default',
+    x_coordinate='X_centroid',
+    y_coordinate='Y_centroid',
+    point_size=10,
+    point_color=None,
+    subset=None,
+    imageid='imageid',
+    seg_mask=None,
+    **kwargs,
+):
     """
-Parameters:
-    image_path (str):  
-        Location to the image file (TIFF, OME.TIFF, ZARR supported)
-
-    seg_mask (str, optional):    
-        Location to the segmentation mask file.
-
-    adata (Ann Data Object):  
-        
-    flip_y (bool, optional):  
-        Flip the Y-axis if needed. Some algorithms output the XY with the Y-coordinates flipped.
-        If the image overlays do not align to the cells, try again by setting this to `False`.
-
-    overlay (str, optional):  
-        Name of the column with any categorical data such as phenotypes or clusters.
-
-    overlay_category (list, optional):  
-        If only specfic categories within the overlay column is needed, pass their names as a list.
-        If None, all categories will be used.
-
-    markers (list, optional):  
-        Markers to be included. If none, all markers will be displayed.
-
-    channel_names (list, optional):  
-        List of channels in the image in the exact order as image. The default is `adata.uns['all_markers']`
-
-    x_coordinate (str, optional):    
-        X axis coordinate column name in AnnData object.
-
-    y_coordinate (str, optional):    
-        Y axis coordinate column name in AnnData object.
-
-    point_size (int, optional):    
-        point size in the napari plot.
-    
-    point_color (str, dict, optional):    
-        The default behavior is to assign auto colors, but you can also provide 
-        a color mapping using the point_color parameter. For instance, you can pass a 
-        dictionary that maps color values to specific categories (provided in the `overlay` parameter). 
-        Here is an example of such a color mapping: `point_color = {'cellTypeA': ['#FFFFFF'], 'cellTypeB': ['#000000']}`. 
-        A single color can also be provided like `point_color = 'white'`
-
-    imageid (str, optional):    
-        Column name of the column containing the image id. 
-
-    subset (str, optional):    
-        imageid of a single image to be subsetted for analyis. Only useful when multiple images are being analyzed together.
-
-    **kwargs  
-        Other arguments that can be passed to napari viewer
-    
-Returns:
-    Napari Viewer (image viewer):  
-
-Example:
-```python
-    image_path = '/Users/aj/Desktop/ptcl_tma/image.ome.tif'
-    sm.pl.image_viewer (image_path, adata, overlay='phenotype',overlay_category=None,
-                markers=['CD31', "CD3D","DNA11",'CD19','CD45','CD163','FOXP3'],
-                point_size=7,point_color='white')
-```
+    Parameters:
+        image_path (str):
+            Location to the image file (TIFF, OME.TIFF, ZARR supported)
+
+        seg_mask (str, optional):
+            Location to the segmentation mask file.
+
+        adata (Ann Data Object):
+
+        flip_y (bool, optional):
+            Flip the Y-axis if needed. Some algorithms output the XY with the Y-coordinates flipped.
+            If the image overlays do not align to the cells, try again by setting this to `False`.
+
+        overlay (str, optional):
+            Name of the column with any categorical data such as phenotypes or clusters.
+
+        overlay_category (list, optional):
+            If only specfic categories within the overlay column is needed, pass their names as a list.
+            If None, all categories will be used.
+
+        markers (list, optional):
+            Markers to be included. If none, all markers will be displayed.
+
+        channel_names (list, optional):
+            List of channels in the image in the exact order as image. The default is `adata.uns['all_markers']`
+
+        x_coordinate (str, optional):
+            X axis coordinate column name in AnnData object.
+
+        y_coordinate (str, optional):
+            Y axis coordinate column name in AnnData object.
+
+        point_size (int, optional):
+            point size in the napari plot.
+
+        point_color (str, dict, optional):
+            The default behavior is to assign auto colors, but you can also provide
+            a color mapping using the point_color parameter. For instance, you can pass a
+            dictionary that maps color values to specific categories (provided in the `overlay` parameter).
+            Here is an example of such a color mapping: `point_color = {'cellTypeA': '#FFFFFF', 'cellTypeB': '#000000'}`.
+            A single color can also be provided like `point_color = 'white'`
+
+        imageid (str, optional):
+            Column name of the column containing the image id.
+
+        subset (str, optional):
+            imageid of a single image to be subsetted for analyis. Only useful when multiple images are being analyzed together.
+
+        **kwargs
+            Other arguments that can be passed to napari viewer
+
+    Returns:
+        Napari Viewer (image viewer):
+
+    Example:
+    ```python
+        image_path = '/Users/aj/Desktop/ptcl_tma/image.ome.tif'
+        sm.pl.image_viewer (image_path, adata, overlay='phenotype',overlay_category=None,
+                    markers=['CD31', "CD3D","DNA11",'CD19','CD45','CD163','FOXP3'],
+                    point_size=7,point_color='white')
+    ```
     """
-    
-    #TODO
+
+    # TODO
     # - ADD Subset markers for ZARR ssection
     # - Ability to use ZARR metadata if available
-    
+
     # adding option to load just the image without an adata object
     if adata is None:
         channel_names = None
-    else: 
+    else:
         # All operations on the AnnData object is performed first
         # Plot only the Image that is requested
         if subset is not None:
             adata = adata[adata.obs[imageid] == subset]
-    
+
         # Recover the channel names from adata
         if channel_names == 'default':
             channel_names = adata.uns['all_markers']
         else:
             channel_names = channel_names
-    
+
         # Index of the marker of interest and corresponding names
         if markers is None:
             idx = list(range(len(channel_names)))
             channel_names = channel_names
         else:
             idx = []
             for i in markers:
                 idx.append(list(channel_names).index(i))
             channel_names = markers
-        
+
         # Load the segmentation mask
         if seg_mask is not None:
             seg_m = tiff.imread(seg_mask)
             if (len(seg_m.shape) > 2) and (seg_m.shape[0] > 1):
                 seg_m = seg_m[0]
-    
 
     # Operations on the OME TIFF image is performed next
     # check the format of image
-    if os.path.isfile(image_path) is True:  
-        image = tiff.TiffFile(image_path, is_ome=False) #is_ome=False
-        z = zarr.open(image.aszarr(), mode='r') # convert image to Zarr array
+    if os.path.isfile(image_path) is True:
+        image = tiff.TiffFile(image_path, is_ome=False)  # is_ome=False
+        z = zarr.open(image.aszarr(), mode='r')  # convert image to Zarr array
         # Identify the number of pyramids
-        n_levels = len(image.series[0].levels) # pyramid
-        
+        n_levels = len(image.series[0].levels)  # pyramid
+
         # If and if not pyramids are available
         if n_levels > 1:
             pyramid = [da.from_zarr(z[i]) for i in range(n_levels)]
             multiscale = True
         else:
             pyramid = da.from_zarr(z)
-            multiscale = False  
-   
+            multiscale = False
+
         # subset channels of interest
         if markers is not None:
             if n_levels > 1:
-                for i in range(n_levels-1):
+                for i in range(n_levels - 1):
                     pyramid[i] = pyramid[i][idx, :, :]
-                n_channels = pyramid[0].shape[0] # identify the number of channels
+                n_channels = pyramid[0].shape[0]  # identify the number of channels
             else:
                 pyramid = pyramid[idx, :, :]
-                n_channels = pyramid.shape[0] # identify the number of channels
+                n_channels = pyramid.shape[0]  # identify the number of channels
         else:
             if n_levels > 1:
                 n_channels = pyramid[0].shape[0]
             else:
                 n_channels = pyramid.shape[0]
-            
+
         # check if channel names have been passed to all channels
         if channel_names is not None:
             assert n_channels == len(channel_names), (
                 f'number of channel names ({len(channel_names)}) must '
                 f'match number of channels ({n_channels})'
             )
 
         # Load the viewer
         viewer = napari.view_image(
-            pyramid, multiscale=multiscale, channel_axis=0,
-            visible=False, 
-            name = None if channel_names is None else channel_names,
-            **kwargs
+            pyramid,
+            multiscale=multiscale,
+            channel_axis=0,
+            visible=False,
+            name=None if channel_names is None else channel_names,
+            **kwargs,
         )
-    
+
     # Operations on the ZARR image
     # check the format of image
-    if os.path.isfile(image_path) is False: 
-        #print(image_path)
+    if os.path.isfile(image_path) is False:
+        # print(image_path)
         viewer = napari.Viewer()
-        viewer.open(image_path, multiscale=True,
-                    visible=False,
-                    name = None if channel_names is None else channel_names)
-    
+        viewer.open(
+            image_path,
+            multiscale=True,
+            visible=False,
+            name=None if channel_names is None else channel_names,
+        )
+
     # Add the seg mask
     if seg_mask is not None:
         viewer.add_labels(seg_m, name='segmentation mask', visible=False)
 
     # Add phenotype layer function
-    def add_phenotype_layer (adata, overlay, phenotype_layer,x,y,viewer,point_size,point_color,available_phenotypes):
+    def add_phenotype_layer(
+        adata,
+        overlay,
+        phenotype_layer,
+        x,
+        y,
+        viewer,
+        point_size,
+        point_color,
+        available_phenotypes,
+    ):
         coordinates = adata[adata.obs[overlay] == phenotype_layer]
         # Flip Y AXIS if needed
         if flip_y is True:
-            coordinates = pd.DataFrame({'y': coordinates.obs[y],'x': coordinates.obs[x]})
-        else:  
-            coordinates = pd.DataFrame({'x': coordinates.obs[x],'y': coordinates.obs[y]})
+            coordinates = pd.DataFrame(
+                {'y': coordinates.obs[y], 'x': coordinates.obs[x]}
+            )
+        else:
+            coordinates = pd.DataFrame(
+                {'x': coordinates.obs[x], 'y': coordinates.obs[y]}
+            )
 
-        #points = coordinates.values.tolist()
+        # points = coordinates.values.tolist()
         points = coordinates.values
         if point_color is None:
-            r = lambda: random.randint(0,255) # random color generator
-            point_color = '#%02X%02X%02X' % (r(),r(),r()) # random color generator
+            r = lambda: random.randint(0, 255)  # random color generator
+            point_color = '#%02X%02X%02X' % (r(), r(), r())  # random color generator
         elif isinstance(point_color, dict):
             # if dict identify the color for the given phenotype
             # also if a color is not provided in the dict assign it to white
             try:
                 point_color = point_color[available_phenotypes]
             except KeyError:
                 point_color = 'white'
                 # if the dict has list, we need to account for it and so the following two lines
                 if isinstance(point_color, list):
                     point_color = point_color[0]
-            
+
         # check if point_color is a dict and if so isolate the color to the specific categoty
-        viewer.add_points(points, size=point_size,face_color=point_color,visible=False,name=phenotype_layer)
+        viewer.add_points(
+            points,
+            size=point_size,
+            face_color=point_color,
+            visible=False,
+            name=phenotype_layer,
+        )
 
     if overlay is not None:
         # categories under investigation
         if overlay_category is None:
             available_phenotypes = list(adata.obs[overlay].unique())
         else:
             available_phenotypes = overlay_category
 
         # Run the function on all phenotypes
         for i in available_phenotypes:
-            add_phenotype_layer (adata=adata, overlay=overlay,
-                                    phenotype_layer=i, x=x_coordinate, y=y_coordinate, viewer=viewer,
-                                    point_size=point_size,point_color=point_color,available_phenotypes=i)
+            add_phenotype_layer(
+                adata=adata,
+                overlay=overlay,
+                phenotype_layer=i,
+                x=x_coordinate,
+                y=y_coordinate,
+                viewer=viewer,
+                point_size=point_size,
+                point_color=point_color,
+                available_phenotypes=i,
+            )
```

### Comparing `scimap-1.1.0/scimap/plotting/_pie.py` & `scimap-1.2.0/scimap/plotting/_pie.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_spatial_distance.py` & `scimap-1.2.0/scimap/plotting/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_spatial_interaction.py` & `scimap-1.2.0/scimap/plotting/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_spatial_pscore.py` & `scimap-1.2.0/scimap/plotting/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_spatial_scatter.py` & `scimap-1.2.0/scimap/plotting/_spatial_scatter.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_stacked_barplot.py` & `scimap-1.2.0/scimap/plotting/_stacked_barplot.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_umap.py` & `scimap-1.2.0/scimap/plotting/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/_voronoi.py` & `scimap-1.2.0/scimap/plotting/_voronoi.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/plotting/lasso_selector.py` & `scimap-1.2.0/scimap/plotting/lasso_selector.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/preprocessing/_combat.py` & `scimap-1.2.0/scimap/preprocessing/_combat.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/preprocessing/_mcmicro_to_scimap.py` & `scimap-1.2.0/scimap/preprocessing/_mcmicro_to_scimap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/preprocessing/_rescale.py` & `scimap-1.2.0/scimap/preprocessing/_rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tests/_data/example_data.csv` & `scimap-1.2.0/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tests/_data/example_data.h5ad` & `scimap-1.2.0/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tests/_data/phenotype_workflow.csv` & `scimap-1.2.0/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tests/test_helpers.py` & `scimap-1.2.0/scimap/tests/test_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys, os
 
 #os.chdir ("/Users/aj/Dropbox (Partners HealthCare)/packages/scimap")
 
 @pytest.fixture
 def adata():
     import anndata as ad    
-    adata = ad.read(os. getcwd() + '/scimap/tests/_data/example_data.h5ad')
+    adata = ad.read(os.getcwd() + '/scimap/tests/_data/example_data.h5ad')
     return adata
 
 # test rename function 
 def test_rename (adata):
     from scimap.helpers._rename import rename
     name= {'T cells': ['CD8 T cells', 'CD4 T cells']}
     adata = rename (adata, name, from_column='phenotype', to_column='phenotype_renamed')
```

### Comparing `scimap-1.1.0/scimap/tests/test_preprocessing.py` & `scimap-1.2.0/scimap/tests/test_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys, os
 
 #os.chdir ("/Users/aj/Dropbox (Partners HealthCare)/packages/scimap")
 
 @pytest.fixture
 def adata():
     from scimap.preprocessing._mcmicro_to_scimap import mcmicro_to_scimap
-    image_path = [os. getcwd() + '/scimap/tests/_data/example_data.csv']
+    image_path = [os.getcwd() + '/scimap/tests/_data/example_data.csv']
     adata = mcmicro_to_scimap (image_path, split='X_position', drop_markers=['BG1', 'BG2', 'BG3'])
     return adata
 
 
 def test_mcmicro_to_scimap(adata):
     assert adata.shape == (3029, 33)
```

### Comparing `scimap-1.1.0/scimap/tests/test_tools.py` & `scimap-1.2.0/scimap/tests/test_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys, os
 import anndata as ad
 
 #os.chdir ("/Users/aj/Dropbox (Partners HealthCare)/packages/scimap")
 
 @pytest.fixture
 def adata():
-    image_path = os. getcwd() + '/scimap/tests/_data/example_data.h5ad'
+    image_path = os.getcwd() + '/scimap/tests/_data/example_data.h5ad'
     adata = ad.read(image_path)
     return adata
 
 # Testing the phenotyping function
 def test_phenotype(adata):
     import pandas as pd
     from scimap.tools._phenotype_cells import phenotype_cells
```

### Comparing `scimap-1.1.0/scimap/tools/__init__.py` & `scimap-1.2.0/scimap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_cluster.py` & `scimap-1.2.0/scimap/tools/_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_foldchange.py` & `scimap-1.2.0/scimap/tools/_foldchange.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_phenotype_cells.py` & `scimap-1.2.0/scimap/tools/_phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_aggregate.py` & `scimap-1.2.0/scimap/tools/_spatial_aggregate.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_cluster.py` & `scimap-1.2.0/scimap/tools/_spatial_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_count.py` & `scimap-1.2.0/scimap/tools/_spatial_count.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_distance.py` & `scimap-1.2.0/scimap/tools/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_expression.py` & `scimap-1.2.0/scimap/tools/_spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_interaction.py` & `scimap-1.2.0/scimap/tools/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_lda.py` & `scimap-1.2.0/scimap/tools/_spatial_lda.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_pscore.py` & `scimap-1.2.0/scimap/tools/_spatial_pscore.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_spatial_similarity_search.py` & `scimap-1.2.0/scimap/tools/_spatial_similarity_search.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/scimap/tools/_umap.py` & `scimap-1.2.0/scimap/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scimap-1.1.0/PKG-INFO` & `scimap-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimap
-Version: 1.1.0
+Version: 1.2.0
 Summary: Spatial Single-Cell Analysis Toolkit
 Home-page: https://pypi.org/project/scimap/
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.7,<3.11
@@ -24,14 +24,15 @@
 Requires-Dist: combat (>=0.3.3,<0.4.0)
 Requires-Dist: dask[array] (>=2.30.0,<3.0.0)
 Requires-Dist: gensim (>=4.0,<5.0)
 Requires-Dist: llvmlite (>=0.38.0,<0.39.0)
 Requires-Dist: matplotlib (>=3.2.1,<4.0.0)
 Requires-Dist: mkdocs (>=1.1.2,<2.0.0)
 Requires-Dist: mkdocs-material (>=7.1.1,<8.0.0)
+Requires-Dist: mpl-scatter-density (>=0.7,<0.8)
 Requires-Dist: napari (>=0.4.2,<0.5.0)
 Requires-Dist: napari-ome-zarr (>=0.4.0,<0.5.0)
 Requires-Dist: numba (>=0.55.0)
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.4,<2.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pytest (>=5.4.3,<6.0.0)
```

