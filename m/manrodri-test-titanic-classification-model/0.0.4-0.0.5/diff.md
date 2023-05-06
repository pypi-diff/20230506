# Comparing `tmp/manrodri-test-titanic-classification-model-0.0.4.tar.gz` & `tmp/manrodri-test-titanic-classification-model-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manrodri-test-titanic-classification-model-0.0.4.tar", last modified: Sat May  6 14:33:05 2023, max compression
+gzip compressed data, was "manrodri-test-titanic-classification-model-0.0.5.tar", last modified: Sat May  6 14:52:50 2023, max compression
```

## Comparing `manrodri-test-titanic-classification-model-0.0.4.tar` & `manrodri-test-titanic-classification-model-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.245830 manrodri-test-titanic-classification-model-0.0.4/
--rw-r--r--   0 manuel     (501) staff       (20)      528 2023-05-06 14:31:22.000000 manrodri-test-titanic-classification-model-0.0.4/MANIFEST.in
--rw-r--r--   0 manuel     (501) staff       (20)      980 2023-05-06 14:33:05.245217 manrodri-test-titanic-classification-model-0.0.4/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)      963 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/README.md
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.234766 manrodri-test-titanic-classification-model-0.0.4/classification_model/
--rw-r--r--   0 manuel     (501) staff       (20)        6 2023-05-06 14:31:58.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/VERSION
--rw-r--r--   0 manuel     (501) staff       (20)      862 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/__init__.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.235577 manrodri-test-titanic-classification-model-0.0.4/classification_model/config/
--rw-r--r--   0 manuel     (501) staff       (20)        0 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/config/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)     2068 2023-05-06 08:56:12.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/config/core.py
--rw-r--r--   0 manuel     (501) staff       (20)      724 2023-05-06 13:08:42.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/config.yml
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.236536 manrodri-test-titanic-classification-model-0.0.4/classification_model/datasets/
--rw-r--r--   0 manuel     (501) staff       (20)        0 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/datasets/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)   117743 2023-05-06 08:47:03.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/datasets/raw.csv
--rw-r--r--   0 manuel     (501) staff       (20)     2155 2023-05-06 13:35:57.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/pipeline.py
--rw-r--r--   0 manuel     (501) staff       (20)     1035 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/predict.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.239725 manrodri-test-titanic-classification-model-0.0.4/classification_model/processing/
--rw-r--r--   0 manuel     (501) staff       (20)        0 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/processing/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)     3115 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/processing/data_manager.py
--rw-r--r--   0 manuel     (501) staff       (20)      660 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/processing/features.py
--rw-r--r--   0 manuel     (501) staff       (20)     1389 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/processing/validation.py
--rw-r--r--   0 manuel     (501) staff       (20)     1060 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/train_pipeline.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.240396 manrodri-test-titanic-classification-model-0.0.4/classification_model/trained_models/
--rw-r--r--   0 manuel     (501) staff       (20)        0 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/classification_model/trained_models/__init__.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.242962 manrodri-test-titanic-classification-model-0.0.4/manrodri_test_titanic_classification_model.egg-info/
--rw-r--r--   0 manuel     (501) staff       (20)      980 2023-05-06 14:33:05.000000 manrodri-test-titanic-classification-model-0.0.4/manrodri_test_titanic_classification_model.egg-info/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)     1075 2023-05-06 14:33:05.000000 manrodri-test-titanic-classification-model-0.0.4/manrodri_test_titanic_classification_model.egg-info/SOURCES.txt
--rw-r--r--   0 manuel     (501) staff       (20)        1 2023-05-06 14:33:05.000000 manrodri-test-titanic-classification-model-0.0.4/manrodri_test_titanic_classification_model.egg-info/dependency_links.txt
--rw-r--r--   0 manuel     (501) staff       (20)      195 2023-05-06 14:33:05.000000 manrodri-test-titanic-classification-model-0.0.4/manrodri_test_titanic_classification_model.egg-info/requires.txt
--rw-r--r--   0 manuel     (501) staff       (20)       21 2023-05-06 14:33:05.000000 manrodri-test-titanic-classification-model-0.0.4/manrodri_test_titanic_classification_model.egg-info/top_level.txt
--rw-r--r--   0 manuel     (501) staff       (20)     1914 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/pyproject.toml
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.231647 manrodri-test-titanic-classification-model-0.0.4/requirements/
--rw-r--r--   0 manuel     (501) staff       (20)      556 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/requirements/requirements.txt
--rw-r--r--   0 manuel     (501) staff       (20)       65 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/requirements/test_requirements.txt
--rw-r--r--   0 manuel     (501) staff       (20)       38 2023-05-06 14:33:05.246001 manrodri-test-titanic-classification-model-0.0.4/setup.cfg
--rw-r--r--   0 manuel     (501) staff       (20)     2412 2023-05-06 09:09:16.000000 manrodri-test-titanic-classification-model-0.0.4/setup.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:33:05.244311 manrodri-test-titanic-classification-model-0.0.4/tests/
--rw-r--r--   0 manuel     (501) staff       (20)      491 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/tests/test_features.py
--rw-r--r--   0 manuel     (501) staff       (20)      766 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.4/tests/test_prediction.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.462285 manrodri-test-titanic-classification-model-0.0.5/
+-rw-r--r--   0 manuel     (501) staff       (20)      528 2023-05-06 14:31:22.000000 manrodri-test-titanic-classification-model-0.0.5/MANIFEST.in
+-rw-r--r--   0 manuel     (501) staff       (20)      980 2023-05-06 14:52:50.461748 manrodri-test-titanic-classification-model-0.0.5/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)      963 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/README.md
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.450199 manrodri-test-titanic-classification-model-0.0.5/classification_model/
+-rw-r--r--   0 manuel     (501) staff       (20)        6 2023-05-06 14:52:00.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/VERSION
+-rw-r--r--   0 manuel     (501) staff       (20)      862 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/__init__.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.451424 manrodri-test-titanic-classification-model-0.0.5/classification_model/config/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/config/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     2068 2023-05-06 08:56:12.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/config/core.py
+-rw-r--r--   0 manuel     (501) staff       (20)      724 2023-05-06 13:08:42.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/config.yml
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.452477 manrodri-test-titanic-classification-model-0.0.5/classification_model/datasets/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/datasets/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)   117743 2023-05-06 08:47:03.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/datasets/raw.csv
+-rw-r--r--   0 manuel     (501) staff       (20)     2155 2023-05-06 14:52:11.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/pipeline.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1035 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/predict.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.455290 manrodri-test-titanic-classification-model-0.0.5/classification_model/processing/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/processing/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     3115 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/processing/data_manager.py
+-rw-r--r--   0 manuel     (501) staff       (20)      660 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/processing/features.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1389 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/processing/validation.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1060 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/train_pipeline.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.456437 manrodri-test-titanic-classification-model-0.0.5/classification_model/trained_models/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/trained_models/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     3742 2023-05-06 14:52:08.000000 manrodri-test-titanic-classification-model-0.0.5/classification_model/trained_models/titanic_classification_model_output_v0.0.5.pkl
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.459813 manrodri-test-titanic-classification-model-0.0.5/manrodri_test_titanic_classification_model.egg-info/
+-rw-r--r--   0 manuel     (501) staff       (20)      980 2023-05-06 14:52:50.000000 manrodri-test-titanic-classification-model-0.0.5/manrodri_test_titanic_classification_model.egg-info/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)     1158 2023-05-06 14:52:50.000000 manrodri-test-titanic-classification-model-0.0.5/manrodri_test_titanic_classification_model.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel     (501) staff       (20)        1 2023-05-06 14:52:50.000000 manrodri-test-titanic-classification-model-0.0.5/manrodri_test_titanic_classification_model.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel     (501) staff       (20)      195 2023-05-06 14:52:50.000000 manrodri-test-titanic-classification-model-0.0.5/manrodri_test_titanic_classification_model.egg-info/requires.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       21 2023-05-06 14:52:50.000000 manrodri-test-titanic-classification-model-0.0.5/manrodri_test_titanic_classification_model.egg-info/top_level.txt
+-rw-r--r--   0 manuel     (501) staff       (20)     1914 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/pyproject.toml
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.447267 manrodri-test-titanic-classification-model-0.0.5/requirements/
+-rw-r--r--   0 manuel     (501) staff       (20)      556 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/requirements/requirements.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       65 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/requirements/test_requirements.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       38 2023-05-06 14:52:50.462458 manrodri-test-titanic-classification-model-0.0.5/setup.cfg
+-rw-r--r--   0 manuel     (501) staff       (20)     2412 2023-05-06 09:09:16.000000 manrodri-test-titanic-classification-model-0.0.5/setup.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-05-06 14:52:50.460986 manrodri-test-titanic-classification-model-0.0.5/tests/
+-rw-r--r--   0 manuel     (501) staff       (20)      491 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/tests/test_features.py
+-rw-r--r--   0 manuel     (501) staff       (20)      766 2023-05-01 15:08:14.000000 manrodri-test-titanic-classification-model-0.0.5/tests/test_prediction.py
```

### Comparing `manrodri-test-titanic-classification-model-0.0.4/MANIFEST.in` & `manrodri-test-titanic-classification-model-0.0.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/PKG-INFO` & `manrodri-test-titanic-classification-model-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manrodri-test-titanic-classification-model
-Version: 0.0.4
+Version: 0.0.5
 Summary: Example Titanic dataset classification model package from Train In Data.
 Home-page: https://github.com/manrodri/titanic-deployment-practice
 Author: manrodri
 Author-email: man.rodri.barr@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `manrodri-test-titanic-classification-model-0.0.4/README.md` & `manrodri-test-titanic-classification-model-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/__init__.py` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/__init__.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/config/core.py` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/config/core.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/config.yml` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/config.yml`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/datasets/raw.csv` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/datasets/raw.csv`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/pipeline.py` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/predict.py` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/predict.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/processing/data_manager.py` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/processing/features.py` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/processing/validation.py` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/processing/validation.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/classification_model/train_pipeline.py` & `manrodri-test-titanic-classification-model-0.0.5/classification_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/manrodri_test_titanic_classification_model.egg-info/PKG-INFO` & `manrodri-test-titanic-classification-model-0.0.5/manrodri_test_titanic_classification_model.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manrodri-test-titanic-classification-model
-Version: 0.0.4
+Version: 0.0.5
 Summary: Example Titanic dataset classification model package from Train In Data.
 Home-page: https://github.com/manrodri/titanic-deployment-practice
 Author: manrodri
 Author-email: man.rodri.barr@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `manrodri-test-titanic-classification-model-0.0.4/manrodri_test_titanic_classification_model.egg-info/SOURCES.txt` & `manrodri-test-titanic-classification-model-0.0.5/manrodri_test_titanic_classification_model.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 classification_model/datasets/__init__.py
 classification_model/datasets/raw.csv
 classification_model/processing/__init__.py
 classification_model/processing/data_manager.py
 classification_model/processing/features.py
 classification_model/processing/validation.py
 classification_model/trained_models/__init__.py
+classification_model/trained_models/titanic_classification_model_output_v0.0.5.pkl
 manrodri_test_titanic_classification_model.egg-info/PKG-INFO
 manrodri_test_titanic_classification_model.egg-info/SOURCES.txt
 manrodri_test_titanic_classification_model.egg-info/dependency_links.txt
 manrodri_test_titanic_classification_model.egg-info/requires.txt
 manrodri_test_titanic_classification_model.egg-info/top_level.txt
 tests/test_features.py
 tests/test_prediction.py
```

### Comparing `manrodri-test-titanic-classification-model-0.0.4/pyproject.toml` & `manrodri-test-titanic-classification-model-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/requirements/requirements.txt` & `manrodri-test-titanic-classification-model-0.0.5/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/setup.py` & `manrodri-test-titanic-classification-model-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `manrodri-test-titanic-classification-model-0.0.4/tests/test_prediction.py` & `manrodri-test-titanic-classification-model-0.0.5/tests/test_prediction.py`

 * *Files identical despite different names*

