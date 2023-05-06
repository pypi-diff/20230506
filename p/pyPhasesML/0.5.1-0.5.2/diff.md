# Comparing `tmp/pyPhasesML-0.5.1.tar.gz` & `tmp/pyPhasesML-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.5.1.tar", last modified: Sat Apr 29 13:58:16 2023, max compression
+gzip compressed data, was "pyPhasesML-0.5.2.tar", last modified: Sat May  6 13:02:02 2023, max compression
```

## Comparing `pyPhasesML-0.5.1.tar` & `pyPhasesML-0.5.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.513744 pyPhasesML-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-29 13:58:16.513744 pyPhasesML-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.506744 pyPhasesML-0.5.1/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.509744 pyPhasesML-0.5.1/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17785 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.511744 pyPhasesML-0.5.1/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.512745 pyPhasesML-0.5.1/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.513744 pyPhasesML-0.5.1/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19178 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.508744 pyPhasesML-0.5.1/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 13:58:16.514745 pyPhasesML-0.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-04-29 13:57:55.000000 pyPhasesML-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.435993 pyPhasesML-0.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-06 13:02:02.434993 pyPhasesML-0.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.427992 pyPhasesML-0.5.2/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3744 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.430992 pyPhasesML-0.5.2/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17785 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.432993 pyPhasesML-0.5.2/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.433993 pyPhasesML-0.5.2/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.434993 pyPhasesML-0.5.2/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    18633 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 13:02:02.429992 pyPhasesML-0.5.2/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-06 13:02:02.000000 pyPhasesML-0.5.2/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-06 13:01:42.000000 pyPhasesML-0.5.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 13:02:02.435993 pyPhasesML-0.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-05-06 13:01:44.000000 pyPhasesML-0.5.2/setup.py
```

### Comparing `pyPhasesML-0.5.1/LICENSE` & `pyPhasesML-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/PKG-INFO` & `pyPhasesML-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.5.1/README.md` & `pyPhasesML-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.5.2/pyPhasesML/DataAugmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from pyPhases import classLogger
 
 
 @classLogger
 class DataAugmentation:
+    """augment Data in shape of (batch, samples, channels)"""
     def __init__(self, config, splitName) -> None:
         self.segmentAugmentation = config["segmentAugmentation"]
         self.recordAugmentation = config["recordAugmentation"]
         self.config = config
         self.splitName = splitName
 
     def step(self, stepname, X, Y, index=None, **options):
```

### Comparing `pyPhasesML-0.5.1/pyPhasesML/DataSet.py` & `pyPhasesML-0.5.2/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.5.2/pyPhasesML/DataversionManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ast import main
 import numpy as np
 from pyPhases import classLogger
 
 
 class NotUniqueException(Exception):
     pass
```

### Comparing `pyPhasesML-0.5.1/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.5.2/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/Model.py` & `pyPhasesML-0.5.2/pyPhasesML/Model.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 
 from .DataSet import DataSet
 
 
 class MetricsDoesNotExist(Exception):
     pass
 
+class AdapterNotImplemented(Exception):
+    pass
+
 
 class Model(ABC, Optionizable):
     metrics = {
         "acc": {"name": "acc", "type": "max"},
         "binary_accuracy": {"name": "binary_accuracy", "type": "max"},
         "accuracy": {"name": "accuracy", "type": "max"},
         "kappa": {"name": "kappa", "type": "max"},
         "loss": {"name": "loss", "type": "min"},
     }
     optimizers = ["adams"]
     useGPU = True
 
-    def __init__(self, options={}) -> None:
+    def __init__(self, options=None) -> None:
+        options = options or {}
         super().__init__(options)
         self.logPath = "logs"
         self.csvLogFile = "log.csv"
         # segmentlength, channelSize
         self.inputShape = None
         self.numClasses = None
         self.classWeights = None
@@ -56,19 +60,19 @@
         self.startEpoch = 0
         self.useEventScorer = False
         self.predictionType = "classification"
 
         self.oneHotDecoded = False
 
     def getCsvPath(self):
-        return self.logPath + "/" + self.csvLogFile
+        return f"{self.logPath}/{self.csvLogFile}"
 
     def getMetric(self, name):
         if name not in Model.metrics:
-            raise MetricsDoesNotExist("The metrics with the name %s is not defined" % name)
+            raise MetricsDoesNotExist(f"The metrics with the name {name} is not defined")
         return Model.metrics[name]
 
     def init(self):
         pass
 
     def define(self):
         pass
@@ -79,31 +83,25 @@
 
     def prepareX(self, x, validation=False):
         return x
 
     def prepareY(self, y, validation=False):
         return y
 
-    def prepareRecordData(self, dataset: DataSet):
-        shapeY = dataset.y.shape
-        dataset.x = dataset.x.reshape(-1, self.inputShape[0], self.inputShape[1])
-        dataset.y = dataset.y.reshape(shapeY[0] * shapeY[1], shapeY[2])
-        return dataset
-
     def beforeTrain(self, dataset):
         pass
 
     def model(self):
         pass
 
     def summary(self):
         self.logWarning("No summary implemented in the model adapter")
 
     def getLossFunction(self):
-        self.logError("No loss function was specified in the model adapter!")
+        raise AdapterNotImplemented("No loss function was specified in the model adapter!")
 
     def getLossWeights(self):
         return None
 
     def getModelEval(self):
         model = self.model if self.modelEval is None else self.modelEval
         model.eval()
@@ -129,12 +127,12 @@
         return
 
     def save(self, path):
         return
 
     @abstractmethod
     def train(self, dataset: DataSet, validationDataset: DataSet = None):
-        raise Exception("required train method is not implemented in the model adapter!")
+        raise AdapterNotImplemented("required train method is not implemented in the model adapter!")
 
     @abstractmethod
     def predict(self, input, get_likelihood=False, returnNumpy=True):
-        raise Exception("required predict method is not implemented in the model adapter!")
+        raise AdapterNotImplemented("required predict method is not implemented in the model adapter!")
```

### Comparing `pyPhasesML-0.5.1/pyPhasesML/ModelManager.py` & `pyPhasesML-0.5.2/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/Plugin.py` & `pyPhasesML-0.5.2/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.5.2/pyPhasesML/SignalPreprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List
 
 import numpy as np
-from scipy.signal import resample
 
 from pyPhases import classLogger
 from pyPhasesRecordloader import ChannelsNotPresent, Event, RecordSignal, Signal
 
 
 class PreprocessSteMissingException(Exception):
     pass
@@ -98,12 +97,13 @@
         signal.signal += minValue
 
     def normalizePercentage(self, signal: Signal, recordSignal: RecordSignal):
         self.cut(signal, recordSignal, 0, 100)
         self.normalize(signal, recordSignal, 0, 1)
 
     def resample(self, signal: Signal, recordSignal: RecordSignal, targetFrequency=None):
+        from scipy.signal import resample
         targetFrequency = targetFrequency or recordSignal.targetFrequency
 
         signalLength = int(len(signal.signal) * targetFrequency / signal.frequency)
         signal.signal = resample(signal.signal, signalLength)
         signal.frequency = targetFrequency
```

### Comparing `pyPhasesML-0.5.1/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.5.2/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.5.2/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.5.2/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/config.yaml` & `pyPhasesML-0.5.2/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.5.2/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.5.2/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.5.2/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,21 @@
         array = np.expand_dims(array, 0)
 
         memmap = None
         if dataId not in self.currentArrayShapes:
             self.currentArrayShapes[dataId] = [[], np.array((1, 0, array.shape[2]))]
             memmap = self.stream(dataId, {"dtype": self.getOption("dtype"), "mode": "w+", "shape": array.shape})
 
-        shape = self.currentArrayShapes[dataId][1]
+        shape = self.currentArrayShapes[dataId][1].astype(np.int64)
         if array.shape[2] != shape[2]:
             raise Exception("The number of channels has to be constant, but was %s and is now %s" % (shape[2], array.shape[2]))
 
         lengths = shape[1]
 
-        shape[1] += array.shape[1]
+        shape[1] += np.array(array.shape[1])
 
         if memmap is None:
             memmap = self.stream(
                 dataId,
                 {
                     "dtype": self.getOption("dtype"),
                     "mode": "readwrite",
```

### Comparing `pyPhasesML-0.5.1/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.5.2/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.5.2/pyPhasesML/scorer/Scorer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
     return confmat
 
 
 class Scorer:
     title = "Segmentbasiert"
     cmScaleByClass = 4
-
-    metricNameMap = {}
     addedMetrics = {}
 
     def __init__(self, numClasses=2, classNames=None, trace=False, threshold=None) -> None:
         self.metrics = ["kappa", "accuracy"]
         self.ignoreClasses = []
         self.numClasses = numClasses if classNames is None else len(classNames)
         self.classNames = list(range(numClasses)) if classNames is None else classNames
@@ -71,16 +69,14 @@
             "combine": combineFunction,
             "biggerIsBetter": biggerIsBetter,
             "useAsBest": useAsBest,
             "initValue": initValue if initValue is not None else 0.0 if biggerIsBetter else np.inf,
         }
 
     def getMetricName(self, metricName):
-        if metricName in Scorer.metricNameMap:
-            metricName = Scorer.metricNameMap[metricName]
         return metricName
 
     def prepareInput(self, inputArray):
         """can be overwritten to tranform tensors to numpy"""
         return inputArray
 
     def preparePrediction(self, inputArray):
@@ -116,40 +112,21 @@
             self.recordResult[recordName] = self.recordEntry(truthOrg, predictionOrg, self.results, recordName)
 
             self.recordIndex += 1
 
         return metrics
 
     def recordEntry(self, truth, prediction, metrics, recordName=None):
-        # prediction = self.flattenPrediction(prediction)
-
-        # if "confusion" in metrics and self.addEvents:
-        #     events = self.getValidationEvents(truth, prediction, recordName=recordName)
-        # else:
-        #     events = None
-
         entry = {
             "truth": truth,
             "prediction": prediction,
-            # "events": events,
         }
         entry.update(metrics)
         return entry
 
-    def getRecords(self):
-        return self.recordResult.values()
-
-    def getRecordsAsDataframe(self):
-        import pandas as pd
-
-        return pd.DataFrame(
-            self.getRecords(),
-            index=list(self.recordResult.keys()),
-        )
-
     def combineMetric(self, metricName):
         metricName = self.getMetricName(metricName)
 
         result = None
 
         if metricName in self.addedMetrics:
             truth = np.concatenate([self.recordResult[id]["truth"] for id in self.recordResult], axis=0)
@@ -211,17 +188,17 @@
     def scoreAllRecords(self):
         if self.trace is False:
             raise Exception("The scorer does not keep the scored record, set the scorer.trace to True to keep all the results")
         self.combineMetrics()
         return self.results
 
     def maskedIgnoredValues(self, truth, prediction):
+        """remove all values that are ignored (by ignoreClasses) from the truth and prediction, truth needs to be non one hot encoded"""
+
         for ignore in self.ignoreClasses:
-            # if self.isHotEncoded(truth):
-            #     ignore =
             keep = truth != ignore
 
             truth = truth[keep]
             prediction = prediction[keep]
 
         return truth, prediction
 
@@ -254,18 +231,14 @@
             acc = 1
         else:
             k = 1 - (nonDiag / np.sum(w_mat * expected))
             acc = 1 - (nonDiag / np.sum(confusion))
 
         return k, acc
 
-    def maskArgMax(self, a, threshold):
-        masked = np.ma.MaskedArray(a, a < threshold)
-        return np.ma.argmax(masked)
-
     def getClassLikelyhood(self, prediction):
         max = np.max(prediction, axis=1, keepdims=True)
         if self.isHotEncoded(prediction):
             e_x = np.exp(prediction - max)
             sum = np.sum(e_x, axis=1, keepdims=True)  # returns sum of each row and keeps same dims
             predictionSoftMax = e_x / sum
             classLikelyhood = predictionSoftMax[:, 1]
@@ -289,15 +262,17 @@
 
         if self.isHotEncoded(prediction):
             prediction = prediction.argmax(-1)
         else:
             threshhold = self.threshold if useThreshold is None else 0.5
             prediction = prediction.reshape(-1)
             if self.numClasses > 2:
-                return prediction
+                prediction = np.floor(prediction)
+                prediction[prediction == self.numClasses] = self.numClasses - 1
+                return np.floor(prediction)
             else:
                 prediction[prediction >= threshhold] = 1
                 prediction[prediction < threshhold] = 0
         return prediction
 
     def getMetricScorer(self, metricName):
         def score(truth, prediction):
@@ -340,18 +315,19 @@
                 f1s.append(f1)
             self.results["f1"] = np.mean(f1s)
         elif metricName == "confusion":
             prediction = self.flattenPrediction(prediction, threshold=self.threshold)
             result = confusion_matrix(
                 truth, prediction, labels=range(self.numClasses)
             )  # , labels=range(self.numClasses) # HPC comp
+            assert result.sum() == len(truth)
         elif metricName in ["auprc", "auroc"]:
             classLikelyhood = self.getClassLikelyhood(prediction)
 
-            scale = 10 ** 3
+            scale = 10**3
             b = scale + 1
             r = (-0.5 / scale, 1.0 + 0.5 / scale)
 
             self.results["all_values"] = np.histogram(classLikelyhood, bins=b, range=r)[0]
 
             pred_pos = classLikelyhood[truth > 0]
             self.results["pos_values"] = np.histogram(pred_pos, bins=b, range=r)[0]
```

### Comparing `pyPhasesML-0.5.1/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.5.2/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.5.1/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.5.2/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.1/setup.py` & `pyPhasesML-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.5.1"[1:],
+    version="v0.5.2"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

