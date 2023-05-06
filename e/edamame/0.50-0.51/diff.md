# Comparing `tmp/edamame-0.50.tar.gz` & `tmp/edamame-0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.50.tar", last modified: Sat May  6 16:01:07 2023, max compression
+gzip compressed data, was "edamame-0.51.tar", last modified: Sat May  6 16:08:18 2023, max compression
```

## Comparing `edamame-0.50.tar` & `edamame-0.51.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.300432 edamame-0.50/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.50/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11829 2023-05-06 16:01:07.299512 edamame-0.50/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10075 2023-05-06 16:00:23.000000 edamame-0.50/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.286583 edamame-0.50/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-04 19:57:28.000000 edamame-0.50/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.291829 edamame-0.50/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.50/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21566 2023-05-03 19:38:54.000000 edamame-0.50/edamame/classifier/classification.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6106 2023-05-06 15:22:05.000000 edamame-0.50/edamame/classifier/diagnose.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.295079 edamame-0.50/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.50/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.50/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-06 14:05:21.000000 edamame-0.50/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.298152 edamame-0.50/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.50/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.50/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21361 2023-04-21 08:55:27.000000 edamame-0.50/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.289536 edamame-0.50/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11829 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-04 19:57:33.000000 edamame-0.50/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-06 16:01:07.300564 edamame-0.50/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:08:18.094311 edamame-0.51/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.51/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11935 2023-05-06 16:08:18.093775 edamame-0.51/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10181 2023-05-06 16:05:55.000000 edamame-0.51/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:08:18.083884 edamame-0.51/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-06 16:04:41.000000 edamame-0.51/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:08:18.088978 edamame-0.51/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.51/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21566 2023-05-03 19:38:54.000000 edamame-0.51/edamame/classifier/classification.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6106 2023-05-06 15:22:05.000000 edamame-0.51/edamame/classifier/diagnose.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:08:18.091110 edamame-0.51/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.51/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.51/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-06 14:05:21.000000 edamame-0.51/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:08:18.093109 edamame-0.51/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.51/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.51/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21361 2023-04-21 08:55:27.000000 edamame-0.51/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:08:18.086734 edamame-0.51/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11935 2023-05-06 16:08:18.000000 edamame-0.51/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-06 16:08:18.000000 edamame-0.51/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-06 16:08:18.000000 edamame-0.51/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-06 16:08:18.000000 edamame-0.51/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-06 16:08:18.000000 edamame-0.51/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-06 16:04:37.000000 edamame-0.51/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-06 16:08:18.094421 edamame-0.51/setup.cfg
```

### Comparing `edamame-0.50/LICENSE` & `edamame-0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.50/PKG-INFO` & `edamame-0.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.50
+Version: 0.51
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -105,14 +105,15 @@
    - **correlation_phik**: Calculate the Phik correlation coefficient between all pairs of columns ([Paper link](https://arxiv.org/pdf/1811.11440.pdf)).
 
 * Useful functions:
 
    - **load_model**: The function load the model saved in the pickle format.
    - **setup**: The function returns the following elements: X_train, y_train, X_test, y_test.
    - **scaling**: The function returns the normalised/standardized matrix.
+   - **ohe**: The function returns the numpy array passed in as input, converted using one-hot encoding. 
 
 <hr>
 
 ## Regressor module
 
 ```python
 from edamame.regressor import TrainRegressor, regression_metrics
```

### Comparing `edamame-0.50/README.md` & `edamame-0.51/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
    - **correlation_phik**: Calculate the Phik correlation coefficient between all pairs of columns ([Paper link](https://arxiv.org/pdf/1811.11440.pdf)).
 
 * Useful functions:
 
    - **load_model**: The function load the model saved in the pickle format.
    - **setup**: The function returns the following elements: X_train, y_train, X_test, y_test.
    - **scaling**: The function returns the normalised/standardized matrix.
+   - **ohe**: The function returns the numpy array passed in as input, converted using one-hot encoding. 
 
 <hr>
 
 ## Regressor module
 
 ```python
 from edamame.regressor import TrainRegressor, regression_metrics
```

### Comparing `edamame-0.50/edamame/classifier/classification.py` & `edamame-0.51/edamame/classifier/classification.py`

 * *Files identical despite different names*

### Comparing `edamame-0.50/edamame/classifier/diagnose.py` & `edamame-0.51/edamame/classifier/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.50/edamame/eda/__init__.py` & `edamame-0.51/edamame/eda/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 correlation_categorical,
 correlation_phik,
 num_variable_study,
 interaction,
 inspection,
 split_and_scaling)
 
-from .tools import (load_model, setup, scaling)
+from .tools import (load_model, setup, scaling, ohe)
 
 
 __all__ = [
     "dimensions",
     "describe_distribution",
     "identify_types",
     "num_to_categorical",
@@ -38,8 +38,9 @@
     "num_variable_study",
     "interaction",
     "inspection",
     "split_and_scaling",
     "load_model",
     "setup",
     "scaling",
+    "ohe",
 ]
```

### Comparing `edamame-0.50/edamame/eda/eda.py` & `edamame-0.51/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.50/edamame/eda/tools.py` & `edamame-0.51/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.50/edamame/regressor/diagnose.py` & `edamame-0.51/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.50/edamame/regressor/regression.py` & `edamame-0.51/edamame/regressor/regression.py`

 * *Files identical despite different names*

### Comparing `edamame-0.50/edamame.egg-info/PKG-INFO` & `edamame-0.51/edamame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.50
+Version: 0.51
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -105,14 +105,15 @@
    - **correlation_phik**: Calculate the Phik correlation coefficient between all pairs of columns ([Paper link](https://arxiv.org/pdf/1811.11440.pdf)).
 
 * Useful functions:
 
    - **load_model**: The function load the model saved in the pickle format.
    - **setup**: The function returns the following elements: X_train, y_train, X_test, y_test.
    - **scaling**: The function returns the normalised/standardized matrix.
+   - **ohe**: The function returns the numpy array passed in as input, converted using one-hot encoding. 
 
 <hr>
 
 ## Regressor module
 
 ```python
 from edamame.regressor import TrainRegressor, regression_metrics
```

### Comparing `edamame-0.50/pyproject.toml` & `edamame-0.51/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.50"
+version = "0.51"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

