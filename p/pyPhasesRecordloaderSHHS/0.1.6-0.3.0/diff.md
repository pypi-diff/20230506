# Comparing `tmp/pyPhasesRecordloaderSHHS-0.1.6.tar.gz` & `tmp/pyPhasesRecordloaderSHHS-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesRecordloaderSHHS-0.1.6.tar", last modified: Fri Jan 27 09:56:48 2023, max compression
+gzip compressed data, was "pyPhasesRecordloaderSHHS-0.3.0.tar", last modified: Sat May  6 13:26:58 2023, max compression
```

## Comparing `pyPhasesRecordloaderSHHS-0.1.6.tar` & `pyPhasesRecordloaderSHHS-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 09:56:48.522661 pyPhasesRecordloaderSHHS-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1487 2023-01-27 09:56:48.522661 pyPhasesRecordloaderSHHS-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 09:56:48.519661 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4992 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/RecordManager.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 09:56:48.518661 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/configs/
--rw-rw-rw-   0 root         (0) root         (0)     3315 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/configs/shhs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3524 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/configs/shhs2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 09:56:48.521661 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/recordLoaders/
--rw-rw-rw-   0 root         (0) root         (0)     2800 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/recordLoaders/RecordLoaderSHHS.py
--rw-rw-rw-   0 root         (0) root         (0)     5185 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/recordLoaders/SHHSAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-27 09:56:24.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/recordLoaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 09:56:48.520661 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1487 2023-01-27 09:56:48.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      835 2023-01-27 09:56:48.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-27 09:56:48.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-01-27 09:56:48.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-01-27 09:56:48.000000 pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-27 09:56:48.522661 pyPhasesRecordloaderSHHS-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-01-27 09:56:25.000000 pyPhasesRecordloaderSHHS-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:26:58.672787 pyPhasesRecordloaderSHHS-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-05-06 13:26:58.672787 pyPhasesRecordloaderSHHS-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:26:58.669787 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/RecordManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:26:58.668787 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/configs/
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/configs/shhs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3524 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/configs/shhs2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:26:58.672787 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/recordLoaders/
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/recordLoaders/RecordLoaderSHHS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5185 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/recordLoaders/SHHSAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 13:26:34.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/recordLoaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:26:58.670787 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-05-06 13:26:58.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      835 2023-05-06 13:26:58.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 13:26:58.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-06 13:26:58.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-06 13:26:58.000000 pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 13:26:58.672787 pyPhasesRecordloaderSHHS-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-05-06 13:26:36.000000 pyPhasesRecordloaderSHHS-0.3.0/setup.py
```

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/.gitlab-ci.yml` & `pyPhasesRecordloaderSHHS-0.3.0/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,14 @@
                 path: cov/coverage.xml
 pypi:
     stage: release
     cache: {}
     variables:
         APP_VERSION: $CI_COMMIT_TAG
     script:
-        - sed -i "s/__VERSION__/${APP_VERSION}/g" setup.py
+        - sed -i "s/v0.0.0/${APP_VERSION}/g" setup.py
         - pip install -U -r requirements.txt
         - pip install -U twine
         - python setup.py sdist
         - twine upload dist/*
     rules:
         - if: '$CI_COMMIT_TAG =~ /^v\d+\.\d+(\.\d+)?(-\S*)?$/'
```

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/LICENSE` & `pyPhasesRecordloaderSHHS-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/PKG-INFO` & `pyPhasesRecordloaderSHHS-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloaderSHHS
-Version: 0.1.6
+Version: 0.3.0
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/README.md` & `pyPhasesRecordloaderSHHS-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/Plugin.py` & `pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/Plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 from pyPhases import PluginAdapter
 from pyPhasesRecordloader import RecordLoader
 
 
 class Plugin(PluginAdapter):
     def initPlugin(self):
         # self.project.loadConfig(self.project.loadConfig(pathlib.Path(__file__).parent.absolute().joinpath("config.yaml")))
-        RecordLoader.registerRecordLoader("RecordLoaderSHHS", "pyPhasesRecordloaderSHHS.recordLoaders")
-        RecordLoader.registerRecordLoader("SHHSAnnotationLoader", "pyPhasesRecordloaderSHHS.recordLoaders")
+        module = "pyPhasesRecordloaderSHHS"
+        rlPath = f"{module}.recordLoaders"
+        RecordLoader.registerRecordLoader("RecordLoaderSHHS", rlPath)
+        RecordLoader.registerRecordLoader("SHHSAnnotationLoader", rlPath)
         shhsPath = self.getConfig("shhs-path")
-        self.project.setConfig("loader.shhs.dataset.downloader.basePath", shhsPath + "/polysomnography/edfs/shhs1")
+        self.project.setConfig("loader.shhs.filePath", shhsPath)
+        self.project.setConfig(
+            "loader.shhs.dataset.downloader.basePath",
+            shhsPath + "/polysomnography/edfs/shhs1",
+        )
         self.project.setConfig(
             "loader.shhs.dataset.downloader.basePathExtensionwise",
-            [shhsPath + "polysomnography/edfs/shhs1", shhsPath + "polysomnography/annotations-events-nsrr/shhs1"],
+            [
+                shhsPath + "polysomnography/edfs/shhs1",
+                shhsPath + "polysomnography/annotations-events-nsrr/shhs1",
+            ],
         )
 
-        self.project.setConfig("loader.shhs2.dataset.downloader.basePath", shhsPath + "/polysomnography/edfs/shhs2")
+        self.project.setConfig(
+            "loader.shhs2.dataset.downloader.basePath",
+            shhsPath + "/polysomnography/edfs/shhs2",
+        )
         self.project.setConfig(
             "loader.shhs2.dataset.downloader.basePathExtensionwise",
-            [shhsPath + "polysomnography/edfs/shhs2", shhsPath + "polysomnography/annotations-events-nsrr/shhs2"],
+            [
+                shhsPath + "polysomnography/edfs/shhs2",
+                shhsPath + "polysomnography/annotations-events-nsrr/shhs2",
+            ],
         )
```

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/RecordManager.py` & `pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/RecordManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from teleschlafmedizin.model.PSGSignal import PSGSignal
 from teleschlafmedizin.model.Annotation import Annotation
-from teleschlafmedizin.model.recordManager.RecordMeta import Channel, Record, RecordAnnotation, RecordChannel
+from teleschlafmedizin.model.recordManager.RecordMeta import (
+    Channel,
+    Record,
+    RecordAnnotation,
+    RecordChannel,
+)
 from pyPhases.util.Logger import classLogger
 from teleschlafmedizin.model.util.DynamicModule import DynamicModule
 from . import recordManager as recordManagerPath
 
 
 class ParseError(Exception):
     pass
@@ -39,15 +44,22 @@
         self.channels = channels
 
 
 @classLogger
 class RecordLoader:
     recordLoader = DynamicModule(recordManagerPath)
 
-    def __init__(self, filePath="", targetFrequency=50, targetSignals=[], targetSignalTypes=[], optionalSignals=[]) -> None:
+    def __init__(
+        self,
+        filePath="",
+        targetFrequency=50,
+        targetSignals=[],
+        targetSignalTypes=[],
+        optionalSignals=[],
+    ) -> None:
         self.filePath = filePath
         self.targetFrequency = targetFrequency
         self.optionalSignals = optionalSignals
         self.targetSignals = targetSignals
         self.targetSignalTypes = targetSignalTypes
         # lightOff and lightOn are in seconds !
         self.lightOff = 0
```

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/configs/shhs.yaml` & `pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/configs/shhs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     dataset:
       loaderName: RecordLoaderSHHS
       fromFiles: True # if the records are read from files or sql-database
       downloader:
         type: nsrr
         listFilter: null
-        canReadRemote: False
+        canReadRemote: True
         basePath: shhs\polysomnography\edfs\shhs1
         extensions: [.edf, -nsrr.xml]
         basePathExtensionwise:
           [
             shhs\polysomnography\edfs\shhs1,
             shhs\polysomnography\annotations-events-nsrr\shhs1,
           ]
```

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/configs/shhs2.yaml` & `pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/configs/shhs2.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS/recordLoaders/SHHSAnnotationLoader.py` & `pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS/recordLoaders/SHHSAnnotationLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS.egg-info/PKG-INFO` & `pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesRecordloaderSHHS
-Version: 0.1.6
+Version: 0.3.0
 Summary: Adds a record loaders to the pyPhases package
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt` & `pyPhasesRecordloaderSHHS-0.3.0/pyPhasesRecordloaderSHHS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesRecordloaderSHHS-0.1.6/setup.py` & `pyPhasesRecordloaderSHHS-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesRecordloaderSHHS",
-    version="v0.1.6"[1:],
+    version="v0.3.0"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="Adds a record loaders to the pyPhases package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesrecordloader/",
     packages=setuptools.find_packages(),
     include_package_data=True,
-    package_data={'pyPhasesRecordloaderSHHS': ['**/*.yaml']},
+    package_data={"pyPhasesRecordloaderSHHS": ["**/*.yaml"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["pyPhases", "pyPhasesRecordloader", "pyedflib"],
     python_requires=">=3.5",
```

