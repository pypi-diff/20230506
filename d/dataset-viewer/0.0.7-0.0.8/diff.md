# Comparing `tmp/dataset-viewer-0.0.7.tar.gz` & `tmp/dataset-viewer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-viewer-0.0.7.tar", last modified: Sat May  6 07:21:19 2023, max compression
+gzip compressed data, was "dataset-viewer-0.0.8.tar", last modified: Sat May  6 07:25:50 2023, max compression
```

## Comparing `dataset-viewer-0.0.7.tar` & `dataset-viewer-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:21:19.628434 dataset-viewer-0.0.7/
--rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      866 2023-05-06 07:21:19.627438 dataset-viewer-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.0.7/README.md
--rw-rw-rw-   0        0        0      746 2023-05-06 07:19:21.000000 dataset-viewer-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 07:21:19.628434 dataset-viewer-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:21:19.608749 dataset-viewer-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 07:21:19.616288 dataset-viewer-0.0.7/src/dataset_viewer/
--rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.0.7/src/dataset_viewer/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-05-06 07:17:40.000000 dataset-viewer-0.0.7/src/dataset_viewer/dataset.py
--rw-rw-rw-   0        0        0     1826 2023-05-06 07:20:37.000000 dataset-viewer-0.0.7/src/dataset_viewer/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:21:19.626461 dataset-viewer-0.0.7/src/dataset_viewer.egg-info/
--rw-rw-rw-   0        0        0      866 2023-05-06 07:21:19.000000 dataset-viewer-0.0.7/src/dataset_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-06 07:21:19.000000 dataset-viewer-0.0.7/src/dataset_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:21:19.000000 dataset-viewer-0.0.7/src/dataset_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 07:21:19.000000 dataset-viewer-0.0.7/src/dataset_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 07:21:19.000000 dataset-viewer-0.0.7/src/dataset_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 07:25:50.762869 dataset-viewer-0.0.8/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      866 2023-05-06 07:25:50.762869 dataset-viewer-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.0.8/README.md
+-rw-rw-rw-   0        0        0      746 2023-05-06 07:25:34.000000 dataset-viewer-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:25:50.762869 dataset-viewer-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:25:50.739259 dataset-viewer-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 07:25:50.748359 dataset-viewer-0.0.8/src/dataset_viewer/
+-rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.0.8/src/dataset_viewer/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-05-06 07:24:43.000000 dataset-viewer-0.0.8/src/dataset_viewer/dataset.py
+-rw-rw-rw-   0        0        0     1826 2023-05-06 07:22:58.000000 dataset-viewer-0.0.8/src/dataset_viewer/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:25:50.761868 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/
+-rw-rw-rw-   0        0        0      866 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 07:25:50.000000 dataset-viewer-0.0.8/src/dataset_viewer.egg-info/top_level.txt
```

### Comparing `dataset-viewer-0.0.7/LICENSE` & `dataset-viewer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.0.7/PKG-INFO` & `dataset-viewer-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataset-viewer-0.0.7/pyproject.toml` & `dataset-viewer-0.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset-viewer"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Hillpro", email="66534835+Hillpro@users.noreply.github.com" },
 ]
 description = "Allow to view a dataset image by image and edit their labels"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dataset-viewer-0.0.7/src/dataset_viewer/dataset.py` & `dataset-viewer-0.0.8/src/dataset_viewer/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __init__(self, data_path=DEFAULT_PATH):
         self.images_path = data_path / 'images'
         self.labels_path = data_path / 'labels'
 
         _images = [glob(f'{self.images_path}/*.{ext}') for ext in VALID_FILE_TYPES]
         self.images = [open(item) for i in _images for item in i]
 
-        if len(self.images == 0):
+        if len(self.images) == 0:
             raise Exception('No images were found')
 
     def get(self, index: int) -> tuple[Image, str]:
         index %= len(self.images)
         image = self.images[index]
         return image, image_name(image)
```

### Comparing `dataset-viewer-0.0.7/src/dataset_viewer/viewer.py` & `dataset-viewer-0.0.8/src/dataset_viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.0.7/src/dataset_viewer.egg-info/PKG-INFO` & `dataset-viewer-0.0.8/src/dataset_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

