# Comparing `tmp/dataset-viewer-0.0.5.tar.gz` & `tmp/dataset-viewer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-viewer-0.0.5.tar", last modified: Wed May  3 04:54:33 2023, max compression
+gzip compressed data, was "dataset-viewer-0.0.6.tar", last modified: Sat May  6 06:55:07 2023, max compression
```

## Comparing `dataset-viewer-0.0.5.tar` & `dataset-viewer-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 04:54:33.883098 dataset-viewer-0.0.5/
--rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      866 2023-05-03 04:54:33.881594 dataset-viewer-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.0.5/README.md
--rw-rw-rw-   0        0        0      746 2023-05-03 04:53:37.000000 dataset-viewer-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 04:54:33.883098 dataset-viewer-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      332 2023-05-03 04:51:32.000000 dataset-viewer-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 04:54:33.858395 dataset-viewer-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 04:54:33.866074 dataset-viewer-0.0.5/src/dataset_viewer/
--rw-rw-rw-   0        0        0        0 2023-05-03 03:38:08.000000 dataset-viewer-0.0.5/src/dataset_viewer/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-03 04:25:18.000000 dataset-viewer-0.0.5/src/dataset_viewer/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-03 04:54:33.880594 dataset-viewer-0.0.5/src/dataset_viewer.egg-info/
--rw-rw-rw-   0        0        0      866 2023-05-03 04:54:33.000000 dataset-viewer-0.0.5/src/dataset_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-05-03 04:54:33.000000 dataset-viewer-0.0.5/src/dataset_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 04:54:33.000000 dataset-viewer-0.0.5/src/dataset_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-03 04:54:33.000000 dataset-viewer-0.0.5/src/dataset_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 04:54:33.000000 dataset-viewer-0.0.5/src/dataset_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 06:55:07.948921 dataset-viewer-0.0.6/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      866 2023-05-06 06:55:07.948921 dataset-viewer-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.0.6/README.md
+-rw-rw-rw-   0        0        0      746 2023-05-06 06:54:08.000000 dataset-viewer-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 06:55:07.948921 dataset-viewer-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:55:07.926167 dataset-viewer-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 06:55:07.932173 dataset-viewer-0.0.6/src/dataset_viewer/
+-rw-rw-rw-   0        0        0        0 2023-05-03 03:38:08.000000 dataset-viewer-0.0.6/src/dataset_viewer/__init__.py
+-rw-rw-rw-   0        0        0     1348 2023-05-06 06:52:52.000000 dataset-viewer-0.0.6/src/dataset_viewer/dataset.py
+-rw-rw-rw-   0        0        0     1848 2023-05-06 06:52:27.000000 dataset-viewer-0.0.6/src/dataset_viewer/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:55:07.947390 dataset-viewer-0.0.6/src/dataset_viewer.egg-info/
+-rw-rw-rw-   0        0        0      866 2023-05-06 06:55:07.000000 dataset-viewer-0.0.6/src/dataset_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-06 06:55:07.000000 dataset-viewer-0.0.6/src/dataset_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 06:55:07.000000 dataset-viewer-0.0.6/src/dataset_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 06:55:07.000000 dataset-viewer-0.0.6/src/dataset_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 06:55:07.000000 dataset-viewer-0.0.6/src/dataset_viewer.egg-info/top_level.txt
```

### Comparing `dataset-viewer-0.0.5/LICENSE` & `dataset-viewer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.0.5/PKG-INFO` & `dataset-viewer-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataset-viewer-0.0.5/pyproject.toml` & `dataset-viewer-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset-viewer"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Hillpro", email="66534835+Hillpro@users.noreply.github.com" },
 ]
 description = "Allow to view a dataset image by image and edit their labels"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dataset-viewer-0.0.5/src/dataset_viewer.egg-info/PKG-INFO` & `dataset-viewer-0.0.6/src/dataset_viewer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

