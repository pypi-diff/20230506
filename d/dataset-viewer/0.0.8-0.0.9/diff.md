# Comparing `tmp/dataset-viewer-0.0.8.tar.gz` & `tmp/dataset-viewer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-viewer-0.0.8.tar", last modified: Sat May  6 07:25:50 2023, max compression
+gzip compressed data, was "dataset-viewer-0.0.9.tar", last modified: Sat May  6 07:43:19 2023, max compression
```

## Comparing `dataset-viewer-0.0.8.tar` & `dataset-viewer-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:25:50.762869 dataset-viewer-0.0.8/
--rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      866 2023-05-06 07:25:50.762869 dataset-viewer-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.0.8/README.md
--rw-rw-rw-   0        0        0      746 2023-05-06 07:25:34.000000 dataset-viewer-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 07:25:50.762869 dataset-viewer-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:25:50.739259 dataset-viewer-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 07:25:50.748359 dataset-viewer-0.0.8/src/dataset_viewer/
--rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.0.8/src/dataset_viewer/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-05-06 07:24:43.000000 dataset-viewer-0.0.8/src/dataset_viewer/dataset.py
--rw-rw-rw-   0        0        0     1826 2023-05-06 07:22:58.000000 dataset-viewer-0.0.8/src/dataset_viewer/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:25:50.761868 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/
--rw-rw-rw-   0        0        0      866 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 07:43:19.948325 dataset-viewer-0.0.9/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      866 2023-05-06 07:43:19.947322 dataset-viewer-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.0.9/README.md
+-rw-rw-rw-   0        0        0      746 2023-05-06 07:42:57.000000 dataset-viewer-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:43:19.948325 dataset-viewer-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:43:19.925787 dataset-viewer-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 07:43:19.933298 dataset-viewer-0.0.9/src/dataset_viewer/
+-rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.0.9/src/dataset_viewer/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-05-06 07:41:14.000000 dataset-viewer-0.0.9/src/dataset_viewer/dataset.py
+-rw-rw-rw-   0        0        0     1850 2023-05-06 07:42:27.000000 dataset-viewer-0.0.9/src/dataset_viewer/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:43:19.946323 dataset-viewer-0.0.9/src/dataset_viewer.egg-info/
+-rw-rw-rw-   0        0        0      866 2023-05-06 07:43:19.000000 dataset-viewer-0.0.9/src/dataset_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-06 07:43:19.000000 dataset-viewer-0.0.9/src/dataset_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:43:19.000000 dataset-viewer-0.0.9/src/dataset_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 07:43:19.000000 dataset-viewer-0.0.9/src/dataset_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 07:43:19.000000 dataset-viewer-0.0.9/src/dataset_viewer.egg-info/top_level.txt
```

### Comparing `dataset-viewer-0.0.8/LICENSE` & `dataset-viewer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.0.8/PKG-INFO` & `dataset-viewer-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataset-viewer-0.0.8/pyproject.toml` & `dataset-viewer-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset-viewer"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Hillpro", email="66534835+Hillpro@users.noreply.github.com" },
 ]
 description = "Allow to view a dataset image by image and edit their labels"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dataset-viewer-0.0.8/src/dataset_viewer/dataset.py` & `dataset-viewer-0.0.9/src/dataset_viewer/dataset.py`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.0.8/src/dataset_viewer/viewer.py` & `dataset-viewer-0.0.9/src/dataset_viewer/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import napari
 from napari import Viewer as NapariViewer, layers
 import numpy as np
-from vispy.util import keys
 
 from dataset_viewer.dataset import Dataset
 
 
 class Viewer():
     __image_idx = 0
 
-    def __init__(self):
+    def __init__(self, dataset = Dataset()):
         self.viewer = NapariViewer()
-        self.dataset = Dataset()
+        self.dataset = dataset
 
         self.labels_layer = None
         self.__set_bindings()
 
     def start(self):
         self.__show_image(0)
         napari.run()
 
     def __set_bindings(self):
+        # Add reset option ('r')
         self.__bind_key('l', self.__current_label_name)
         self.__bind_key('Escape', self.__exit)
         self.__bind_key('Left', self.__previous)
         self.__bind_key('Right', self.__next)
 
     def __bind_key(self, key, func):
         self.viewer.bind_key(key, func)
```

### Comparing `dataset-viewer-0.0.8/src/dataset_viewer.egg-info/PKG-INFO` & `dataset-viewer-0.0.9/src/dataset_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

