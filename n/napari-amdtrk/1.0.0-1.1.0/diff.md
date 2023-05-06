# Comparing `tmp/napari-amdtrk-1.0.0.tar.gz` & `tmp/napari-amdtrk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-amdtrk-1.0.0.tar", last modified: Sat Apr  8 07:20:34 2023, max compression
+gzip compressed data, was "napari-amdtrk-1.1.0.tar", last modified: Sat May  6 07:09:39 2023, max compression
```

## Comparing `napari-amdtrk-1.0.0.tar` & `napari-amdtrk-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-04-08 07:20:34.575728 napari-amdtrk-1.0.0/
--rw-r--r--   0 jefft      (501) staff       (20)     1072 2023-02-07 08:32:35.000000 napari-amdtrk-1.0.0/LICENSE
--rw-r--r--   0 jefft      (501) staff       (20)       96 2023-02-06 15:23:01.000000 napari-amdtrk-1.0.0/MANIFEST.in
--rw-r--r--   0 jefft      (501) staff       (20)     6094 2023-04-08 07:20:34.575955 napari-amdtrk-1.0.0/PKG-INFO
--rw-r--r--   0 jefft      (501) staff       (20)     4903 2023-04-08 07:15:40.000000 napari-amdtrk-1.0.0/README.md
--rw-r--r--   0 jefft      (501) staff       (20)      180 2023-02-06 15:23:01.000000 napari-amdtrk-1.0.0/pyproject.toml
--rw-r--r--   0 jefft      (501) staff       (20)     1659 2023-04-08 07:20:34.577156 napari-amdtrk-1.0.0/setup.cfg
-drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-04-08 07:20:34.551002 napari-amdtrk-1.0.0/src/
-drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-04-08 07:20:34.564132 napari-amdtrk-1.0.0/src/napari_amdtrk/
--rw-r--r--   0 jefft      (501) staff       (20)      221 2023-02-07 11:37:04.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/__init__.py
--rw-r--r--   0 jefft      (501) staff       (20)     6423 2023-04-04 07:32:38.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/_reader.py
--rw-r--r--   0 jefft      (501) staff       (20)      609 2023-02-21 09:51:55.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/_sample_data.py
-drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-04-08 07:20:34.575156 napari-amdtrk-1.0.0/src/napari_amdtrk/_tests/
--rw-r--r--   0 jefft      (501) staff       (20)        0 2023-02-06 15:23:01.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/_tests/__init__.py
--rw-r--r--   0 jefft      (501) staff       (20)      975 2023-02-06 15:23:01.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/_tests/test_reader.py
--rw-r--r--   0 jefft      (501) staff       (20)      316 2023-02-21 10:01:23.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/_tests/test_sample_data.py
--rw-r--r--   0 jefft      (501) staff       (20)     1246 2023-02-06 15:23:01.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/_tests/test_widget.py
--rw-r--r--   0 jefft      (501) staff       (20)     6832 2023-04-02 16:34:19.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/_utils.py
--rw-r--r--   0 jefft      (501) staff       (20)    46277 2023-04-08 06:45:57.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/_widget.py
--rw-r--r--   0 jefft      (501) staff       (20)      973 2023-02-21 09:51:44.000000 napari-amdtrk-1.0.0/src/napari_amdtrk/napari.yaml
-drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-04-08 07:20:34.569239 napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/
--rw-r--r--   0 jefft      (501) staff       (20)     6094 2023-04-08 07:20:34.000000 napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/PKG-INFO
--rw-r--r--   0 jefft      (501) staff       (20)      644 2023-04-08 07:20:34.000000 napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/SOURCES.txt
--rw-r--r--   0 jefft      (501) staff       (20)        1 2023-04-08 07:20:34.000000 napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/dependency_links.txt
--rw-r--r--   0 jefft      (501) staff       (20)       60 2023-04-08 07:20:34.000000 napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/entry_points.txt
--rw-r--r--   0 jefft      (501) staff       (20)      109 2023-04-08 07:20:34.000000 napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/requires.txt
--rw-r--r--   0 jefft      (501) staff       (20)       14 2023-04-08 07:20:34.000000 napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/top_level.txt
+drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-05-06 07:09:39.405480 napari-amdtrk-1.1.0/
+-rw-r--r--   0 jefft      (501) staff       (20)     1072 2023-02-07 08:32:35.000000 napari-amdtrk-1.1.0/LICENSE
+-rw-r--r--   0 jefft      (501) staff       (20)       96 2023-02-06 15:23:01.000000 napari-amdtrk-1.1.0/MANIFEST.in
+-rw-r--r--   0 jefft      (501) staff       (20)     6595 2023-05-06 07:09:39.405696 napari-amdtrk-1.1.0/PKG-INFO
+-rw-r--r--   0 jefft      (501) staff       (20)     5404 2023-05-06 07:05:46.000000 napari-amdtrk-1.1.0/README.md
+-rw-r--r--   0 jefft      (501) staff       (20)      180 2023-02-06 15:23:01.000000 napari-amdtrk-1.1.0/pyproject.toml
+-rw-r--r--   0 jefft      (501) staff       (20)     1659 2023-05-06 07:09:39.407141 napari-amdtrk-1.1.0/setup.cfg
+drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-05-06 07:09:39.216472 napari-amdtrk-1.1.0/src/
+drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-05-06 07:09:39.393034 napari-amdtrk-1.1.0/src/napari_amdtrk/
+-rw-r--r--   0 jefft      (501) staff       (20)      221 2023-02-07 11:37:04.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/__init__.py
+-rw-r--r--   0 jefft      (501) staff       (20)     7027 2023-05-05 17:47:53.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/_reader.py
+-rw-r--r--   0 jefft      (501) staff       (20)      609 2023-02-21 09:51:55.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/_sample_data.py
+drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-05-06 07:09:39.404860 napari-amdtrk-1.1.0/src/napari_amdtrk/_tests/
+-rw-r--r--   0 jefft      (501) staff       (20)        0 2023-02-06 15:23:01.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/_tests/__init__.py
+-rw-r--r--   0 jefft      (501) staff       (20)      975 2023-02-06 15:23:01.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/_tests/test_reader.py
+-rw-r--r--   0 jefft      (501) staff       (20)      316 2023-02-21 10:01:23.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/_tests/test_sample_data.py
+-rw-r--r--   0 jefft      (501) staff       (20)     1246 2023-02-06 15:23:01.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/_tests/test_widget.py
+-rw-r--r--   0 jefft      (501) staff       (20)     6832 2023-04-02 16:34:19.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/_utils.py
+-rw-r--r--   0 jefft      (501) staff       (20)    47558 2023-05-03 07:59:12.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/_widget.py
+-rw-r--r--   0 jefft      (501) staff       (20)      973 2023-02-21 09:51:44.000000 napari-amdtrk-1.1.0/src/napari_amdtrk/napari.yaml
+drwxr-xr-x   0 jefft      (501) staff       (20)        0 2023-05-06 07:09:39.397673 napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/
+-rw-r--r--   0 jefft      (501) staff       (20)     6595 2023-05-06 07:09:39.000000 napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/PKG-INFO
+-rw-r--r--   0 jefft      (501) staff       (20)      644 2023-05-06 07:09:39.000000 napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/SOURCES.txt
+-rw-r--r--   0 jefft      (501) staff       (20)        1 2023-05-06 07:09:39.000000 napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/dependency_links.txt
+-rw-r--r--   0 jefft      (501) staff       (20)       60 2023-05-06 07:09:39.000000 napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/entry_points.txt
+-rw-r--r--   0 jefft      (501) staff       (20)      109 2023-05-06 07:09:39.000000 napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/requires.txt
+-rw-r--r--   0 jefft      (501) staff       (20)       14 2023-05-06 07:09:39.000000 napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/top_level.txt
```

### Comparing `napari-amdtrk-1.0.0/LICENSE` & `napari-amdtrk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-amdtrk-1.0.0/PKG-INFO` & `napari-amdtrk-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-amdtrk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Manually amend segmentation and track within napari
 Home-page: https://github.com/Jeff-Gui/napari-amdtrk-plugin
 Author: Yifan Gui
 Author-email: jeffgui9912@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Jeff-Gui/napari-amdtrk-plugin/issues
 Project-URL: Documentation, https://github.com/Jeff-Gui/napari-amdtrk-plugin/blob/master/README.md
@@ -50,24 +50,26 @@
 - An intensity image (`tif`) in txyc (or txy) format
 - An object mask (`tif`) in txy format
 - An object table (`csv`) with following essential columns:
     - frame: time frame
     - trackId: ID of the track, starting from 1
     - Center_of_the_object_0: x coordinate
     - Center_of_the_object_1: y coordinate
-    - continuous_label: the corresponding label (intensity value) of the object in the object mask (You may use `skimage.measure.label` to get it from a binary mask.)
+    - continuous_label: the corresponding label (intensity value) of the object in the object mask (You may use `skimage.measure.label` to get it from a binary mask).
 
 - A config file named `config.yaml` (_other names are not allowed_)
 
     Within the config file, there should be:
-    - intensity_suffix: suffix of the intensity image (e.g., for `foo_GFP.tif`, use `GFP` in the config)
+    - intensity_suffix: suffix of the intensity image (e.g., for `foo_GFP.tif`, use `GFP` in the config). For multiple intensity images, separate them with commas (e.g., `GFP, mCherry`)
     - mask_suffix: suffix of the mask image
     - track_suffix: suffix of the tracked object table
     - frame_base: index of the first frame (either `0` or `1`)
-    - stateCol: __optional__ column name for the cell state (e.g., cell cycle phase) in the object table. Leave blank if the object table does not contain it.
+    - stateCol: __optional__ column name for the cell state (e.g., cell cycle phase) in the object table. Leave blank if the object table does not contain it
+
+__Napari-amdtrk will modify mask and track files in place.__ Other files are not affected.
 
 ---
 ### Quick start
 
 1. Open `napari` GUI.
 2. `File` > `Open folder` > choose `Amend segmentation and track`
 3. `Plugins` > `napari-amdtrk: Amend track widget` > `Run`
@@ -87,14 +89,25 @@
 The above operations will download data to `~/.amd_trk/_sample_data/` (__~230MB__). After downloading is finished, sample data will be loaded.
 
 _Notes_
 - Please cite this repository if using the plugin in your work (try `About` > `Cite this repository` upper right of this homepage).
   
 - Sample data (cell track videos) have been published with [_pcnaDeep: a fast and robust single-cell tracking method using deep-learning mediated cell cycle profiling_](10.1093/bioinformatics/btac602). We acknowledge Dr Kuan Yoow Chan and members of his lab for generating the data. 
 
+----------------------------------
+
+### Keyboard shortcuts
+
+- <kbd>&uarr;</kbd> and <kbd>&darr;</kbd>: toggle different operations
+- <kbd>enter</kbd>: run the operation
+
+- Available to a selected object:
+  - <kbd>control</kbd> + <kbd>9</kbd>: shrink the object mask
+  - <kbd>control</kbd> + <kbd>0</kbd>: expand the object mask
+
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari-amdtrk-1.0.0/README.md` & `napari-amdtrk-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 - An intensity image (`tif`) in txyc (or txy) format
 - An object mask (`tif`) in txy format
 - An object table (`csv`) with following essential columns:
     - frame: time frame
     - trackId: ID of the track, starting from 1
     - Center_of_the_object_0: x coordinate
     - Center_of_the_object_1: y coordinate
-    - continuous_label: the corresponding label (intensity value) of the object in the object mask (You may use `skimage.measure.label` to get it from a binary mask.)
+    - continuous_label: the corresponding label (intensity value) of the object in the object mask (You may use `skimage.measure.label` to get it from a binary mask).
 
 - A config file named `config.yaml` (_other names are not allowed_)
 
     Within the config file, there should be:
-    - intensity_suffix: suffix of the intensity image (e.g., for `foo_GFP.tif`, use `GFP` in the config)
+    - intensity_suffix: suffix of the intensity image (e.g., for `foo_GFP.tif`, use `GFP` in the config). For multiple intensity images, separate them with commas (e.g., `GFP, mCherry`)
     - mask_suffix: suffix of the mask image
     - track_suffix: suffix of the tracked object table
     - frame_base: index of the first frame (either `0` or `1`)
-    - stateCol: __optional__ column name for the cell state (e.g., cell cycle phase) in the object table. Leave blank if the object table does not contain it.
+    - stateCol: __optional__ column name for the cell state (e.g., cell cycle phase) in the object table. Leave blank if the object table does not contain it
+
+__Napari-amdtrk will modify mask and track files in place.__ Other files are not affected.
 
 ---
 ### Quick start
 
 1. Open `napari` GUI.
 2. `File` > `Open folder` > choose `Amend segmentation and track`
 3. `Plugins` > `napari-amdtrk: Amend track widget` > `Run`
@@ -59,14 +61,25 @@
 The above operations will download data to `~/.amd_trk/_sample_data/` (__~230MB__). After downloading is finished, sample data will be loaded.
 
 _Notes_
 - Please cite this repository if using the plugin in your work (try `About` > `Cite this repository` upper right of this homepage).
   
 - Sample data (cell track videos) have been published with [_pcnaDeep: a fast and robust single-cell tracking method using deep-learning mediated cell cycle profiling_](10.1093/bioinformatics/btac602). We acknowledge Dr Kuan Yoow Chan and members of his lab for generating the data. 
 
+----------------------------------
+
+### Keyboard shortcuts
+
+- <kbd>&uarr;</kbd> and <kbd>&darr;</kbd>: toggle different operations
+- <kbd>enter</kbd>: run the operation
+
+- Available to a selected object:
+  - <kbd>control</kbd> + <kbd>9</kbd>: shrink the object mask
+  - <kbd>control</kbd> + <kbd>0</kbd>: expand the object mask
+
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari-amdtrk-1.0.0/setup.cfg` & `napari-amdtrk-1.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-amdtrk
-version = 1.0.0
+version = 1.1.0
 description = Manually amend segmentation and track within napari
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Yifan Gui
 author_email = jeffgui9912@gmail.com
 license = MIT
 license_files = LICENSE
```

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk/_reader.py` & `napari-amdtrk-1.1.0/src/napari_amdtrk/_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,25 +89,29 @@
     # look for config
     try:
         with open(os.path.join(path, cfgname), 'r') as f:
             cfg = yaml.safe_load(f.read())
     except:
         raise FileNotFoundError('Missing config file.')
     
-    intensity_path, mask_path, track_path = '', '', ''
+    intensity_path, mask_path, track_path = [], '', ''
+    its_list = cfg['intensity_suffix'].split(',')
+    for i in range(len(its_list)):
+        its_list[i] = its_list[i].strip()
+
     for fname in os.listdir(path):
         sfx = fname.split('.')[0].split('_')[-1]
-        if sfx == cfg['intensity_suffix']:
-            intensity_path = os.path.join(path, fname)
+        if sfx in its_list:
+            intensity_path.append(os.path.join(path, fname))
         if sfx == cfg['mask_suffix']:
             mask_path = os.path.join(path, fname)
         if sfx == cfg['track_suffix']:
             track_path = os.path.join(path, fname)
     
-    if intensity_path == '' or mask_path == '' or track_path == '':
+    if intensity_path == [] or mask_path == '' or track_path == '':
         raise ValueError('Missing input file, check if filenames match the config.')
         
     stateCol = cfg['stateCol']
     track = pd.read_csv(track_path)
 
     # if no state column specified, will use a dummy column.
     if stateCol is None:
@@ -137,21 +141,30 @@
         return track
     
     track = check_input_track(track, hasState, stateColName)
     track = track.sort_values(by=['trackId','frame'])
     mask = io.imread(mask_path)
 
     rt = []
+    i = 1
+    colors = ['green', 'red', 'yellow', 'blue', 'magenta', 'cyan']
+    if len(intensity_path) == 1:
+        colors[0] = 'gray'
     if intensity_path is not None:
-        comp = io.imread(intensity_path)
-        if len(comp.shape) > 3:
-            for i in range(comp.shape):
-                rt.append((comp[:, :, :, i], {'name':'intensity' + str(i)}, 'image'))
-        else:
-            rt.append((comp, {'name':'intensity0'}, 'image'))
+        for j in range(len(intensity_path)):
+            comp = io.imread(intensity_path[j])
+            if len(comp.shape) > 3:
+                for i in range(comp.shape):
+                    rt.append((comp[:, :, :, i], {'name':'intensity_' + str(i), 'blending':'additive',
+                                                  'colormap':colors[i-1] if i<7 else 'gray'}, 'image'))
+                    i += 1
+            else:
+                rt.append((comp, {'name':'intensity_' + str(i), 'blending':'additive',
+                                  'colormap':colors[i-1] if i<7 else 'gray'}, 'image'))
+                i += 1
 
     rt.append((mask, {'name':'segm','metadata':{'frame_base': cfg['frame_base'], 'stateCol': stateCol, 
                         'stateColName': stateColName, 'track_path': track_path, 'phaseVis': phaseVis,
                         'mask_path': mask_path, 'states':states, 'hasState':hasState}}, 'labels'))
     track_data = track.loc[:][['trackId', 'frame', 'Center_of_the_object_1', 'Center_of_the_object_0']]
     label_data = track.loc[:][['frame', 'Center_of_the_object_1', 'Center_of_the_object_0']]
     label_data = label_data.to_numpy()
```

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk/_sample_data.py` & `napari-amdtrk-1.1.0/src/napari_amdtrk/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk/_tests/test_reader.py` & `napari-amdtrk-1.1.0/src/napari_amdtrk/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk/_tests/test_widget.py` & `napari-amdtrk-1.1.0/src/napari_amdtrk/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk/_utils.py` & `napari-amdtrk-1.1.0/src/napari_amdtrk/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk/_widget.py` & `napari-amdtrk-1.1.0/src/napari_amdtrk/_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 see: https://napari.org/stable/plugins/guides.html?#widgets
 """
 from typing import TYPE_CHECKING
 import warnings
 from magicgui import magicgui
 from magicgui.widgets import RadioButtons, Container
 from qtpy.QtWidgets import QWidget
-from ._utils import get_current_time, get_layer_id_by_name, find_daugs, align_table_and_mask, get_annotation
+from ._utils import get_current_time, find_daugs, align_table_and_mask, get_annotation
 import numpy as np
 import skimage.io as io
 import skimage.measure as measure
+import skimage.morphology as morph
 import pandas as pd
 import trackpy
 
 if TYPE_CHECKING:
     import napari
 warnings.filterwarnings("ignore", category=DeprecationWarning) 
 
@@ -25,38 +26,35 @@
     # in one of two ways:
     # 1. use a parameter called `napari_viewer`, as done here
     # 2. use a type annotation of 'napari.viewer.Viewer' for any parameter
     def __init__(self, viewer : 'napari.viewer.Viewer'):
 
         super().__init__()
         self.viewer = viewer
-        self.segm_id = get_layer_id_by_name(self.viewer, 'segm')
-        self.track_id = get_layer_id_by_name(self.viewer, 'tracks')
-        self.name_id = get_layer_id_by_name(self.viewer, 'name')
         # meta: {'frame_base': int, 'stateCol': int, 'stateColName': str, 'track_path': str, 'mask_path': str}
-        meta = self.viewer.layers[self.segm_id].metadata
+        meta = self.viewer.layers['segm'].metadata
         self.frame_base = meta['frame_base']
         self.stateCol = meta['stateCol']
         self.stateColName = meta['stateColName']
         self.track_path = meta['track_path']
         self.mask_path = meta['mask_path']
         phaseVis = meta['phaseVis']
         states = meta['states']
         self.hasState = meta['hasState']
         self.states = meta['states']
 
-        self.track = self.viewer.layers[self.track_id].metadata['ori_data']
+        self.track = self.viewer.layers['tracks'].metadata['ori_data']
         self.saved = self.track.copy()
-        self.mask = self.viewer.layers[self.segm_id].data.copy()
+        self.mask = self.viewer.layers['segm'].data.copy()
         self.track_count = int(np.max(self.track['trackId']))
-        self.DILATE_FACTOR = int((self.viewer.layers[self.segm_id].data.shape[1] + 
-                                  self.viewer.layers[self.segm_id].data.shape[2]) / 2 / 240)
+        self.DILATE_FACTOR = int((self.viewer.layers['segm'].data.shape[1] + 
+                                  self.viewer.layers['segm'].data.shape[2]) / 2 / 240)
 
-        self.high = 255 if np.max(self.viewer.layers[self.segm_id].data) < 255 else 65536
-        self.select = {}  # register selected obj (key: frame-label, value: (mask,contour))
+        self.high = 255 if np.max(self.viewer.layers['segm'].data) < 255 else 65536
+        self.select = {}  # register selected obj (key: frame-label, value: (bbox, id in sel list, frame, label on mask))
         self.last_reg_id = 0
         self.label_unassigned = -1
 
 
         #================== Widget definitions =======================
 
         @magicgui(labels=False,
@@ -255,18 +253,18 @@
             keep_tracks.update({'IDs':''})
             copy_obj.update({'ID':0, 'fromFrame':0, 'toFrame':1})
             retrack.update({'distance':0, 'frame_gap':0})
         self.reset_widget = reset_widget
 
         self.viewer.add_shapes(name='[selection]', edge_width=2*self.DILATE_FACTOR, edge_color='coral', face_color=[0,0,0,0], ndim=3)
         
-        labels = self.viewer.layers[self.segm_id]
+        labels = self.viewer.layers['segm']
         #sels = self.viewer.layers['[selection]']
-        #trkly = self.viewer.layers[self.track_id]
-        #namely = self.viewer.layers[self.name_id]
+        #trkly = self.viewer.layers['tracks']
+        #namely = self.viewer.layers['name']
         
         #@sels.mouse_drag_callbacks.append
         @labels.mouse_drag_callbacks.append
         #@trkly.mouse_drag_callbacks.append
         #@namely.mouse_drag_callbacks.append
         def click_drag(layer, event):
             
@@ -323,19 +321,19 @@
                         # find the bounding box
                         msk = sle == lbl
                         minx, miny, maxx, maxy = measure.regionprops(measure.label(msk))[0].bbox
                         objBox = np.array([[pos[0], minx, miny], [pos[0], maxx, miny],
                                            [pos[0], maxx, maxy], [pos[0], minx, maxy]])
                         idx = len(viewer.layers['[selection]'].data)
                         new = viewer.layers['[selection]'].data.copy() + [objBox]
-                        self.select[ky] = (objBox, idx)
+                        self.select[ky] = (objBox, idx, pos[0], lbl)
 
                     else:  # delete object highlight (deselect)
                         
-                        _, idx = self.select[ky]
+                        _, idx, _, _ = self.select[ky]
                         new = viewer.layers['[selection]'].data.copy()
                         del new[idx]
 
                         # update widget default values according to selections
                         #  involves two selection
                         slk = list(self.select.keys())
                         if len(slk) > 1:
@@ -374,15 +372,15 @@
                     # update maximum label of the frame to title
                     vstatus = self.viewer.status
                     if isinstance(vstatus, dict):
                         vstatus = vstatus['coordinates']
                     fme = int(vstatus.split('[')[1].lstrip().split(' ')[0])
                     mxLabel = self.get_mx(fme)
                     self.viewer.title = 'AmdTrk | Max label of frame: ' + str(fme) + ' is ** ' + str(mxLabel) + ' **'
-                    self.viewer.layers[self.segm_id].selected_label = mxLabel + 1
+                    self.viewer.layers['segm'].selected_label = mxLabel + 1
                     self.clear_selection()
 
         @self.viewer.bind_key('Enter')
         def _resolve_key(self):
             # run widget from keyboard
             nonlocal btns, widget_map
             wig = widget_map[btns.value]
@@ -406,14 +404,54 @@
             else:
                 if not phaseVis and btns.value == 9:
                     btns.value = 1
                 else:
                     btns.value += 1
             return
 
+
+        def _run_dilate_sel(mode='dilate'):
+            nonlocal self
+            sel = list(self.select.keys())
+            if len(sel) == 0:
+                return
+            else:
+                mask = self.viewer.layers['segm'].data
+                bbox, _, fid, lbl = self.select[sel[0]]
+                frame = mask[fid,:,:].copy()
+                frame_copy = frame.copy()
+                frame[frame!=lbl] = 0
+                frame[frame==lbl] = 1
+                to_dilate = int(np.max([bbox[2,1] - bbox[0,1], bbox[2,2] - bbox[2,1]]) / 80) # What's good scaling here???
+                if mode == 'dilate':
+                    dilated = morph.binary_dilation(frame, footprint=morph.disk(radius=to_dilate))
+                elif mode == 'erode':
+                    dilated = morph.binary_erosion(frame, footprint=morph.disk(radius=to_dilate))
+                else:
+                    return
+                if mode == 'erode':
+                    frame_copy[frame_copy==lbl] = 0
+                frame_copy[dilated] = lbl
+                mask[fid,:,:] = frame_copy
+                self.viewer.layers['segm'].data = mask
+                #self.refresh()
+            return
+    
+        @self.viewer.bind_key('Control-0', overwrite=True)
+        def _dilate_sel(self):
+            nonlocal _run_dilate_sel
+            _run_dilate_sel(mode='dilate')
+            return
+
+        @self.viewer.bind_key('Control-9', overwrite=True)
+        def _erode_sel(self):
+            nonlocal _run_dilate_sel
+            _run_dilate_sel(mode='erode')
+            return
+
         # Update the layer dropdown menu when the layer list changes
         self.viewer.layers.events.changed.connect(container_ext.reset_choices)
         # Add plugin to the napari viewer
         # self.setLayout(QHBoxLayout())
         # self.layout().addWidget(container_ext)
         self.viewer.window.add_dock_widget(container_ext, area='left')
         return
@@ -427,15 +465,14 @@
     
     def check_assign(self, IDs_to_check):
         for i in IDs_to_check:
             if i == 0:
                 raise ValueError('Must first assign track ID to the object!')
         return
 
-
     #================== Widget functions =======================
 
     def create_or_replace(self, old_id, frame, new_id=None):
         """Create a new track ID or replace with some track ID
         after certain frame. If the old track has daughters, new track ID will be the parent.
 
         Args:
@@ -666,15 +703,15 @@
         del_unreg_sel = False
         if trk_id not in self.track['trackId'].values:
             if trk_id == 0:
                 del_unreg_sel = True
             else:
                 raise ValueError('Selected track is not in the table.')
 
-        mask = self.viewer.layers[self.segm_id].data
+        mask = self.viewer.layers['segm'].data
         if not del_unreg_sel:
             del_trk = self.track[self.track['trackId'] == trk_id]
         if frame is None and not del_unreg_sel:
 
             if trk_id != 0:
                 # For all direct daughter of the track to delete, first remove association
                 dir_daugs = list(np.unique(self.track.loc[self.track['parentTrackId'] == trk_id, 'trackId']))
@@ -708,22 +745,22 @@
             elif not del_unreg_sel:
                 self.track = self.track.drop(index=self.track[(self.track['trackId'] == trk_id) &
                                                               (self.track['frame'] == frame) &
                                                               (self.track['continuous_label'] == lb)].index)
                 msg = 'Deleted unassigned object ' + str(lb) + ' at frame ' + str(frame) + '.'
             else:
                 msg = 'Deleted an unregistered object.'
-        self.viewer.layers[self.segm_id].data = mask
+        self.viewer.layers['segm'].data = mask
         print(msg)
         return msg
 
     def run_keep_tracks(self, trk_ids):
         """Only keep tracks specified in the input list.
         """
-        mask = self.viewer.layers[self.segm_id].data
+        mask = self.viewer.layers['segm'].data
 
         for trk_id in trk_ids:
             if trk_id in self.track['trackId']:  # no warning if input track is not in the dataset.
                 # For all direct daughters of the track to keep, if not in input list, dissociate.
                 dir_daugs = list(np.unique(self.track.loc[self.track['parentTrackId'] == trk_id, 'trackId']))
                 for dd in dir_daugs:
                     if dd not in trk_ids:
@@ -738,24 +775,24 @@
             lb = list(self.track[self.track['frame'] == frame]['continuous_label'])
             msk_slice = mask[frame, :, :]
             new_mask = np.zeros(shape=msk_slice.shape, dtype=mask.dtype)
             for l in lb:
                 new_mask[msk_slice == l] = l
             mask[frame, :, :] = new_mask
     
-        self.viewer.layers[self.segm_id].data = mask
+        self.viewer.layers['segm'].data = mask
 
         msg = 'Tracks kept: ' + ','.join(list(map(lambda x:str(x), trk_ids))) + '.'
         print(msg)
         return msg
 
     def save(self, mask_flag=True):
         """Save current table.
         """
-        mask = self.viewer.layers[self.segm_id].data
+        mask = self.viewer.layers['segm'].data
         track = self.track.copy()
         if mask_flag:
             mask, track = align_table_and_mask(track, mask, align_morph=False, 
                                                phase_col=self.stateColName, phase_default=self.states[0])      # warning: align_morph=False
             if int(np.max(mask)) <= 255:
                 io.imsave(self.mask_path, mask.astype('uint8'))
             else:
@@ -768,22 +805,22 @@
         self.track = track.copy()
         msg = 'Saved: ' + get_current_time() + '.'
         return msg
 
     def revert(self):
         """Revert to last saved version.
         """
-        self.viewer.layers[self.segm_id].data = self.mask.copy()
+        self.viewer.layers['segm'].data = self.mask.copy()
         self.track = self.saved.copy()
         msg = 'Reverted: ' + get_current_time() + '.'
         return msg
     
     def retrack(self, distance, frame_gap):
         trk = self.track.copy()
-        mask = self.viewer.layers[self.segm_id].data
+        mask = self.viewer.layers['segm'].data
         mask, trk = align_table_and_mask(trk, mask, align_morph=False)   
         trk['index'] = trk.index
         t = trackpy.link(trk[['frame', 'Center_of_the_object_0', 'Center_of_the_object_1', 'index']], 
                          search_range=distance, memory=frame_gap, adaptive_stop=0.4*distance, 
                          pos_columns=['Center_of_the_object_0', 'Center_of_the_object_1'])
         cols = list(t.columns)
         cols[len(cols)-1] = 'trackId'
@@ -879,15 +916,15 @@
 
         Args:
             obj_id (int): Object ID of the drawn mask.
             frame (int): Frame location.
             trk_id (int): Track ID.
             cls (str): State id.
         """
-        mask = self.viewer.layers[self.segm_id].data
+        mask = self.viewer.layers['segm'].data
         msk_slice = mask[frame, :, :]
         trk_slice = self.track[self.track['frame'] == frame]
         untracked = False if int(trk_id) > 0 else True          # register as an untracked object
         if obj_id in list(trk_slice['continuous_label']):
             if list(trk_slice[trk_slice['continuous_label'] == obj_id]['trackId'])[0] == 0:
                 # assign information to untracked object
                 idx = list(trk_slice[trk_slice['continuous_label'] == obj_id]['trackId'].index)[0]
@@ -958,15 +995,15 @@
         return msg
 
     def run_copy_obj(self, ID, fromFrame, toFrame):
         # copy object (labeled as ID) from frame A to frame B, will overlap on existing objects on B.
         if fromFrame == toFrame:
             raise ValueError('Cannot copy object on the same frame.')
         row = self.track[(self.track['frame'] == fromFrame) & (self.track['continuous_label'] == ID)]
-        mask = self.viewer.layers[self.segm_id].data
+        mask = self.viewer.layers['segm'].data
         if row.shape[0] != 1:
             # If unassigned object found in fromFrame, register it first.
             if ID in np.unique(mask[fromFrame,:,:]):
                 self.register_obj(obj_id=ID, frame=fromFrame, trk_id=0, cls=self.states[0])
             else:
                 raise ValueError('ID not found in fromFrame.')
         
@@ -977,29 +1014,29 @@
         new_track = new_track.sort_values(by=['trackId','frame'])
         new_track.index = [_ for _ in range(new_track.shape[0])]
         self.track = new_track
         toMask = mask[toFrame,:,:].copy()
         fromMask = mask[fromFrame,:,:]
         toMask[fromMask==ID] = tar_mx + 1
         mask[toFrame,:,:] = toMask
-        self.viewer.layers[self.segm_id].data = mask
+        self.viewer.layers['segm'].data = mask
         msg = ''
         return msg
 
     def get_mx(self, frame):
-        mask = self.viewer.layers[self.segm_id].data
+        mask = self.viewer.layers['segm'].data
         return int(np.max(mask[frame,:,:]))
 
     def refresh(self):
         self.getAnn()
         track_data = self.track.loc[:][['trackId', 'frame', 'Center_of_the_object_1', 'Center_of_the_object_0']].copy()
         track_data = track_data[track_data['trackId']>0] # unassigned tracks have ID=0, not allowed for napari to plot.
         track_data = track_data.to_numpy().astype('float')
-        self.viewer.layers[self.track_id].data = track_data
+        self.viewer.layers['tracks'].data = track_data
         label_data = self.track.loc[:][['frame', 'Center_of_the_object_1', 'Center_of_the_object_0']]
         label_data = label_data.to_numpy()
         # self.layers[nm_idx].features.clear()
-        self.viewer.layers[self.name_id].data = label_data
-        self.viewer.layers[self.name_id].features['name'] = self.track.loc[:]['name'].to_numpy()
-        self.viewer.layers[self.name_id].refresh_text()
+        self.viewer.layers['name'].data = label_data
+        self.viewer.layers['name'].features['name'] = self.track.loc[:]['name'].to_numpy()
+        self.viewer.layers['name'].refresh_text()
         self.clear_selection()
         return
```

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk/napari.yaml` & `napari-amdtrk-1.1.0/src/napari_amdtrk/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/PKG-INFO` & `napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-amdtrk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Manually amend segmentation and track within napari
 Home-page: https://github.com/Jeff-Gui/napari-amdtrk-plugin
 Author: Yifan Gui
 Author-email: jeffgui9912@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Jeff-Gui/napari-amdtrk-plugin/issues
 Project-URL: Documentation, https://github.com/Jeff-Gui/napari-amdtrk-plugin/blob/master/README.md
@@ -50,24 +50,26 @@
 - An intensity image (`tif`) in txyc (or txy) format
 - An object mask (`tif`) in txy format
 - An object table (`csv`) with following essential columns:
     - frame: time frame
     - trackId: ID of the track, starting from 1
     - Center_of_the_object_0: x coordinate
     - Center_of_the_object_1: y coordinate
-    - continuous_label: the corresponding label (intensity value) of the object in the object mask (You may use `skimage.measure.label` to get it from a binary mask.)
+    - continuous_label: the corresponding label (intensity value) of the object in the object mask (You may use `skimage.measure.label` to get it from a binary mask).
 
 - A config file named `config.yaml` (_other names are not allowed_)
 
     Within the config file, there should be:
-    - intensity_suffix: suffix of the intensity image (e.g., for `foo_GFP.tif`, use `GFP` in the config)
+    - intensity_suffix: suffix of the intensity image (e.g., for `foo_GFP.tif`, use `GFP` in the config). For multiple intensity images, separate them with commas (e.g., `GFP, mCherry`)
     - mask_suffix: suffix of the mask image
     - track_suffix: suffix of the tracked object table
     - frame_base: index of the first frame (either `0` or `1`)
-    - stateCol: __optional__ column name for the cell state (e.g., cell cycle phase) in the object table. Leave blank if the object table does not contain it.
+    - stateCol: __optional__ column name for the cell state (e.g., cell cycle phase) in the object table. Leave blank if the object table does not contain it
+
+__Napari-amdtrk will modify mask and track files in place.__ Other files are not affected.
 
 ---
 ### Quick start
 
 1. Open `napari` GUI.
 2. `File` > `Open folder` > choose `Amend segmentation and track`
 3. `Plugins` > `napari-amdtrk: Amend track widget` > `Run`
@@ -87,14 +89,25 @@
 The above operations will download data to `~/.amd_trk/_sample_data/` (__~230MB__). After downloading is finished, sample data will be loaded.
 
 _Notes_
 - Please cite this repository if using the plugin in your work (try `About` > `Cite this repository` upper right of this homepage).
   
 - Sample data (cell track videos) have been published with [_pcnaDeep: a fast and robust single-cell tracking method using deep-learning mediated cell cycle profiling_](10.1093/bioinformatics/btac602). We acknowledge Dr Kuan Yoow Chan and members of his lab for generating the data. 
 
+----------------------------------
+
+### Keyboard shortcuts
+
+- <kbd>&uarr;</kbd> and <kbd>&darr;</kbd>: toggle different operations
+- <kbd>enter</kbd>: run the operation
+
+- Available to a selected object:
+  - <kbd>control</kbd> + <kbd>9</kbd>: shrink the object mask
+  - <kbd>control</kbd> + <kbd>0</kbd>: expand the object mask
+
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari-amdtrk-1.0.0/src/napari_amdtrk.egg-info/SOURCES.txt` & `napari-amdtrk-1.1.0/src/napari_amdtrk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

