# Comparing `tmp/dataset-viewer-0.1.0.tar.gz` & `tmp/dataset-viewer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-viewer-0.1.0.tar", last modified: Sat May  6 07:52:11 2023, max compression
+gzip compressed data, was "dataset-viewer-0.1.1.tar", last modified: Sat May  6 08:08:08 2023, max compression
```

## Comparing `dataset-viewer-0.1.0.tar` & `dataset-viewer-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:52:11.836710 dataset-viewer-0.1.0/
--rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      866 2023-05-06 07:52:11.835710 dataset-viewer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.1.0/README.md
--rw-rw-rw-   0        0        0      746 2023-05-06 07:51:32.000000 dataset-viewer-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 07:52:11.836710 dataset-viewer-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:52:11.811200 dataset-viewer-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 07:52:11.818709 dataset-viewer-0.1.0/src/dataset_viewer/
--rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.1.0/src/dataset_viewer/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-05-06 07:41:14.000000 dataset-viewer-0.1.0/src/dataset_viewer/dataset.py
--rw-rw-rw-   0        0        0     1850 2023-05-06 07:51:37.000000 dataset-viewer-0.1.0/src/dataset_viewer/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:52:11.834739 dataset-viewer-0.1.0/src/dataset_viewer.egg-info/
--rw-rw-rw-   0        0        0      866 2023-05-06 07:52:11.000000 dataset-viewer-0.1.0/src/dataset_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-06 07:52:11.000000 dataset-viewer-0.1.0/src/dataset_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:52:11.000000 dataset-viewer-0.1.0/src/dataset_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 07:52:11.000000 dataset-viewer-0.1.0/src/dataset_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 07:52:11.000000 dataset-viewer-0.1.0/src/dataset_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 08:08:08.144076 dataset-viewer-0.1.1/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      866 2023-05-06 08:08:08.144076 dataset-viewer-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.1.1/README.md
+-rw-rw-rw-   0        0        0      746 2023-05-06 08:07:24.000000 dataset-viewer-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 08:08:08.144076 dataset-viewer-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:08:08.121238 dataset-viewer-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 08:08:08.129324 dataset-viewer-0.1.1/src/dataset_viewer/
+-rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.1.1/src/dataset_viewer/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-05-06 08:03:32.000000 dataset-viewer-0.1.1/src/dataset_viewer/dataset.py
+-rw-rw-rw-   0        0        0     1892 2023-05-06 08:07:04.000000 dataset-viewer-0.1.1/src/dataset_viewer/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:08:08.143077 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/
+-rw-rw-rw-   0        0        0      866 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/top_level.txt
```

### Comparing `dataset-viewer-0.1.0/LICENSE` & `dataset-viewer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.1.0/PKG-INFO` & `dataset-viewer-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataset-viewer-0.1.0/pyproject.toml` & `dataset-viewer-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset-viewer"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Hillpro", email="66534835+Hillpro@users.noreply.github.com" },
 ]
 description = "Allow to view a dataset image by image and edit their labels"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dataset-viewer-0.1.0/src/dataset_viewer/dataset.py` & `dataset-viewer-0.1.1/src/dataset_viewer/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 
 def empty_image(img):
     return fromarray(np.full(img.size[::-1], 0))
 
 
 class Dataset():
-    def __init__(self, data_path=DEFAULT_PATH):
+    def __init__(self, data_path: Path = None):
+        if data_path is None:
+            data_path = DEFAULT_PATH
+
         self.images_path = data_path / 'images'
         self.labels_path = data_path / 'labels'
 
         _images = [glob(f'{self.images_path}/*.{ext}') for ext in VALID_FILE_TYPES]
         self.images = [open(item) for i in _images for item in i]
 
         if len(self.images) == 0:
```

### Comparing `dataset-viewer-0.1.0/src/dataset_viewer/viewer.py` & `dataset-viewer-0.1.1/src/dataset_viewer/viewer.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from dataset_viewer.dataset import Dataset
 
 
 class Viewer():
     __image_idx = 0
 
-    def __init__(self, dataset = Dataset()):
+    def __init__(self, dataset: Dataset = None):
         self.viewer = NapariViewer()
-        self.dataset = dataset
+        self.dataset = dataset if dataset is not None else Dataset()
 
         self.labels_layer = None
         self.__set_bindings()
 
     def start(self):
         self.__show_image(0)
         napari.run()
```

### Comparing `dataset-viewer-0.1.0/src/dataset_viewer.egg-info/PKG-INFO` & `dataset-viewer-0.1.1/src/dataset_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

