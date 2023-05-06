# Comparing `tmp/edamame-0.49.tar.gz` & `tmp/edamame-0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.49.tar", last modified: Fri Apr 21 08:57:14 2023, max compression
+gzip compressed data, was "edamame-0.50.tar", last modified: Sat May  6 16:01:07 2023, max compression
```

## Comparing `edamame-0.49.tar` & `edamame-0.50.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.464614 edamame-0.49/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.49/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10798 2023-04-21 08:57:14.463685 edamame-0.49/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9044 2023-04-20 10:23:15.000000 edamame-0.49/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.456806 edamame-0.49/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-04-21 08:55:43.000000 edamame-0.49/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.459531 edamame-0.49/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      127 2023-04-16 11:13:18.000000 edamame-0.49/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21608 2023-04-16 11:09:39.000000 edamame-0.49/edamame/classifier/classification.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.461251 edamame-0.49/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.49/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.49/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3814 2023-03-25 15:57:39.000000 edamame-0.49/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.463037 edamame-0.49/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.49/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8324 2023-04-02 09:56:35.000000 edamame-0.49/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21361 2023-04-21 08:55:27.000000 edamame-0.49/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.458437 edamame-0.49/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10798 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      430 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-04-21 08:55:48.000000 edamame-0.49/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-21 08:57:14.464711 edamame-0.49/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.300432 edamame-0.50/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.50/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11829 2023-05-06 16:01:07.299512 edamame-0.50/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10075 2023-05-06 16:00:23.000000 edamame-0.50/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.286583 edamame-0.50/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-04 19:57:28.000000 edamame-0.50/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.291829 edamame-0.50/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.50/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21566 2023-05-03 19:38:54.000000 edamame-0.50/edamame/classifier/classification.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6106 2023-05-06 15:22:05.000000 edamame-0.50/edamame/classifier/diagnose.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.295079 edamame-0.50/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.50/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.50/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-06 14:05:21.000000 edamame-0.50/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.298152 edamame-0.50/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.50/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.50/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21361 2023-04-21 08:55:27.000000 edamame-0.50/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-06 16:01:07.289536 edamame-0.50/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11829 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-06 16:01:07.000000 edamame-0.50/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-04 19:57:33.000000 edamame-0.50/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-06 16:01:07.300564 edamame-0.50/setup.cfg
```

### Comparing `edamame-0.49/LICENSE` & `edamame-0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.49/PKG-INFO` & `edamame-0.50/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,50 @@
-Metadata-Version: 2.1
-Name: edamame
-Version: 0.49
-Summary: Exploratory data analysis tools
-Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
-License: Copyright (c) 2018 The Python Packaging Authority
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/marcosalvalaggio/edamame
-Project-URL: Bug Tracker, https://github.com/marcosalvalaggio/edamame/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Edamame
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
+- [Edamame](#edamame)
+  - [Functionalities](#functionalities)
+  - [Eda module](#eda-module)
+  - [Regressor module](#regressor-module)
+    - [Example:](#example)
+  - [Classifier module](#classifier-module)
+    - [Example:](#example-1)
+  - [Todos](#todos)
+
+
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
 ```
 
 the edamame package works correctly inside a jupyter-notebook. You can find the documentation of the package on the [edamame-documentation](https://edamame-doc.readthedocs.io/en/latest/index.html) page.
 
 <hr>
 
 
-## Edamame functionalities
+## Functionalities
 
 
-The package consists of three modules: eda, which performs exploratory data analysis; and regressor and classifier, which handle the training of machine learning models for regression and classification, respectively. To see examples of the uses of the edamame package, you can check out the [edamame-notebook](https://github.com/marcosalvalaggio/edamame-notebooks) repository.
+The package consists of three modules: eda, which performs exploratory data analysis; and regressor and classifier, which handle the training of machine learning models for regression and classification, respectively. To see examples of the uses of the edamame package, you can check out the [examples](https://github.com/marcosalvalaggio/edamame-notebooks) folder in the repository.
 
 <hr>
 
 ## Eda module
 
-
-``import edamame.eda as eda``
+```python
+import edamame.eda as eda
+```
 
 The **eda** module provides a wide range of functions for performing exploratory data analysis (EDA) on datasets. With this module you can easily explore and manipulate your data, conduct descriptive statistics, correlation analysis, and prepare your data for machine learning. The "eda" module offers the following functionalities:
 
 * Data Exploration and Manipulation functions:
 
    - **dimensions**: The function displays the number of rows and columns of a pandas dataframe passed. 
    - **identify_types**: Identify the data types of each column.
@@ -133,14 +111,37 @@
 * **coefficients**: Computes and prints the coefficients of the regression model.
 * **random_forest_fi**: Displays the feature importance plot for the random forest regression model. 
 * **random_forest_fi**: Displays the feature importance plot for the xgboost regression model. 
 * **prediction_error**: Computes and prints the prediction error of the regression model on the test data.
 * **residual_plot**: creates and displays a residual plot for the regression model.
 * **qqplot**: creates and displays a QQ plot for the regression model.
 
+
+### Example:
+
+```python
+from sklearn.datasets import make_regression
+from edamame.regressor import TrainRegressor
+import pandas as pd
+import edamame.eda as eda
+from edamame.regressor import RegressorDiagnose
+X, y = make_regression(n_samples=1000, n_features=5, n_targets=1, random_state=42)
+X = pd.DataFrame(X, columns=["f1", "f2", "f3", "f4", "f5"])
+y = pd.DataFrame(y, columns=["y"])
+X_train, y_train, X_test, y_test = eda.setup(X, y)
+X_train_s = eda.scaling(X_train)
+X_test_s = eda.scaling(X_test)
+regressor = TrainRegressor(X_train_s, y_train, X_test_s, y_test)
+rf = regressor.random_forest()
+regressor.model_metrics()
+diagnose = RegressorDiagnose(X_train_s, y_train, X_test_s, y_test)
+diagnose.random_forest_fi(model=rf)
+diagnose.prediction_error(model=rf)
+```
+
 <hr>
 
 ## Classifier module
 
 
 ```python
 from edamame.classifier import TrainClassifier
```

### Comparing `edamame-0.49/README.md` & `edamame-0.50/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,83 @@
+Metadata-Version: 2.1
+Name: edamame
+Version: 0.50
+Summary: Exploratory data analysis tools
+Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
+License: Copyright (c) 2018 The Python Packaging Authority
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/marcosalvalaggio/edamame
+Project-URL: Bug Tracker, https://github.com/marcosalvalaggio/edamame/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Edamame
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
+- [Edamame](#edamame)
+  - [Functionalities](#functionalities)
+  - [Eda module](#eda-module)
+  - [Regressor module](#regressor-module)
+    - [Example:](#example)
+  - [Classifier module](#classifier-module)
+    - [Example:](#example-1)
+  - [Todos](#todos)
+
+
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
 ```
 
 the edamame package works correctly inside a jupyter-notebook. You can find the documentation of the package on the [edamame-documentation](https://edamame-doc.readthedocs.io/en/latest/index.html) page.
 
 <hr>
 
 
-## Edamame functionalities
+## Functionalities
 
 
-The package consists of three modules: eda, which performs exploratory data analysis; and regressor and classifier, which handle the training of machine learning models for regression and classification, respectively. To see examples of the uses of the edamame package, you can check out the [edamame-notebook](https://github.com/marcosalvalaggio/edamame-notebooks) repository.
+The package consists of three modules: eda, which performs exploratory data analysis; and regressor and classifier, which handle the training of machine learning models for regression and classification, respectively. To see examples of the uses of the edamame package, you can check out the [examples](https://github.com/marcosalvalaggio/edamame-notebooks) folder in the repository.
 
 <hr>
 
 ## Eda module
 
-
-``import edamame.eda as eda``
+```python
+import edamame.eda as eda
+```
 
 The **eda** module provides a wide range of functions for performing exploratory data analysis (EDA) on datasets. With this module you can easily explore and manipulate your data, conduct descriptive statistics, correlation analysis, and prepare your data for machine learning. The "eda" module offers the following functionalities:
 
 * Data Exploration and Manipulation functions:
 
    - **dimensions**: The function displays the number of rows and columns of a pandas dataframe passed. 
    - **identify_types**: Identify the data types of each column.
@@ -100,14 +144,37 @@
 * **coefficients**: Computes and prints the coefficients of the regression model.
 * **random_forest_fi**: Displays the feature importance plot for the random forest regression model. 
 * **random_forest_fi**: Displays the feature importance plot for the xgboost regression model. 
 * **prediction_error**: Computes and prints the prediction error of the regression model on the test data.
 * **residual_plot**: creates and displays a residual plot for the regression model.
 * **qqplot**: creates and displays a QQ plot for the regression model.
 
+
+### Example:
+
+```python
+from sklearn.datasets import make_regression
+from edamame.regressor import TrainRegressor
+import pandas as pd
+import edamame.eda as eda
+from edamame.regressor import RegressorDiagnose
+X, y = make_regression(n_samples=1000, n_features=5, n_targets=1, random_state=42)
+X = pd.DataFrame(X, columns=["f1", "f2", "f3", "f4", "f5"])
+y = pd.DataFrame(y, columns=["y"])
+X_train, y_train, X_test, y_test = eda.setup(X, y)
+X_train_s = eda.scaling(X_train)
+X_test_s = eda.scaling(X_test)
+regressor = TrainRegressor(X_train_s, y_train, X_test_s, y_test)
+rf = regressor.random_forest()
+regressor.model_metrics()
+diagnose = RegressorDiagnose(X_train_s, y_train, X_test_s, y_test)
+diagnose.random_forest_fi(model=rf)
+diagnose.prediction_error(model=rf)
+```
+
 <hr>
 
 ## Classifier module
 
 
 ```python
 from edamame.classifier import TrainClassifier
```

### Comparing `edamame-0.49/edamame/classifier/classification.py` & `edamame-0.50/edamame/classifier/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#TODO - add classifier metrics function 
-
 import numpy as np
 import pandas as pd
 from  edamame.eda.tools import dataframe_review, dummy_control
 from sklearn.linear_model import LogisticRegression
 from sklearn.preprocessing import StandardScaler
 from sklearn.naive_bayes import GaussianNB
 from sklearn.neighbors import KNeighborsClassifier
```

### Comparing `edamame-0.49/edamame/eda/__init__.py` & `edamame-0.50/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.49/edamame/eda/eda.py` & `edamame-0.50/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.49/edamame/eda/tools.py` & `edamame-0.50/edamame/eda/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pickle
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 import pandas as pd
 from typing import Tuple
-
+import numpy as np
 
 
 def load_model(path: str):
     """
     The function load the model saved previously in the pickle format.
 
     Args:
@@ -15,15 +15,14 @@
 
     """
     with open(path, 'rb') as file:
         model = pickle.load(file)
     return model 
 
 
-
 def setup(X: pd.DataFrame, y: pd.DataFrame, dummy: bool = False, seed: int = 42, size: float = 0.25) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     """
     The function returns the following elements: X_train, y_train, X_test, y_test.
 
     Args: 
         X (pd.DataFrame): The model matrix X (features matrix).
         y (pd.DataFrame): The target variable.
@@ -43,15 +42,14 @@
     # split dataset in train and test
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=size, random_state=seed)
     X_train = pd.get_dummies(data=X_train, drop_first=dummy)
     X_test = pd.get_dummies(data=X_test, drop_first=dummy)
     return X_train, y_train, X_test, y_test
 
 
-
 def scaling(X: pd.DataFrame, minmaxscaler: bool = False) -> pd.DataFrame:
     """
     The function returns the normalised/standardized matrix.
 
     Args:
         X (pd.DataFrame): The model matrix X/X_train/X_test
     minmaxscaler (bool): Select the type of scaling to apply to the numerical columns. By default is setted to the StandardScaler. If minmaxscaler is set to True the numerical columns is trasfomed to [0,1].
@@ -75,14 +73,35 @@
     else: 
         scaler = StandardScaler()
     scaler.fit(X[quant_columns])
     X[quant_columns] = scaler.transform(X[quant_columns])
     return X
 
 
+def ohe(array: np.ndarray) -> np.ndarray:
+    """
+    Convert a NumPy array that represents the categorical label of the target variable and transform it using one-hot encoding.
+
+    Args:
+        array (np.ndarray): The target variables passed in input.
+
+    Return:
+        np.ndarray: The one-hot encoded NumPy array.
+    
+    Example: 
+        >>> import edamame.eda as eda
+        >>> from sklearn import datasets
+        >>> iris = datasets.load_iris()
+        >>> y = iris.target
+        >>> y_ohe = eda.ohe(y)
+    """
+    num_classes = len(np.unique(array))
+    ohe_array = np.eye(num_classes)[array]
+    return ohe_array
+
 
 def dummy_control(data: pd.DataFrame) -> None:
     """
     The function checks if the Pandas dataframe passed is encoded with dummy or OHE. 
     
     Args:
         data (pd.Dataframe): A pandas DataFrame passed in input.
@@ -97,15 +116,14 @@
     qual_col = types[types == 'object']
     if len(qual_col) != 0:
         raise TypeError('dataframe with non-numerical columns')
     else:
         pass
 
 
-
 def dataframe_review(data: pd.DataFrame) -> None:
     """
     The function checks if the object passed is a Pandas dataframe.
 
     Args:
         data (pd.Dataframe): A pandas DataFrame passed in input.
```

### Comparing `edamame-0.49/edamame/regressor/diagnose.py` & `edamame-0.50/edamame/regressor/diagnose.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
     Attributes:
         X_train (pd.DataFrame): The input training data.
         y_train (pd.Series): The target training data.
         X_test (pd.DataFrame): The input test data.
         y_test (pd.Series): The target test data.
 
     Example:
-        >>> from edamame.regressor import TrainRegressor, Diagnose
+        >>> from edamame.regressor import TrainRegressor, RegressorDiagnose
         >>> regressor = TrainRegressor(X_train, np.log(y_train), X_test, np.log(y_test))
         >>> linear = regressor.linear()
-        >>> diagnose = Diagnose(X_train, np.log(y_train), X_test, np.log(y_test))
+        >>> diagnose = RegressorDiagnose(X_train, np.log(y_train), X_test, np.log(y_test))
         >>> diagnose.coefficients()
         >>> diagnose.prediction_error(model=linear)
         >>> diagnose.residual_plot(model=linear)
         >>> diagnose.qqplot(model=linear)
     """
     def __init__(self, X_train: pd.DataFrame, y_train: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame) -> None:
         self.X_train = X_train
@@ -136,15 +136,15 @@
     
     def prediction_error(self, model: Union[LinearRegression, Lasso, Ridge, DecisionTreeRegressor, RandomForestRegressor, xgb.XGBRegressor], train_data: bool = True, figsize: Tuple[float, float] = (8.,6.)) -> None:
         """
         Define a scatterpolot with ygt and ypred of the model passed.
 
         Args:
             model (Union[LinearRegression, Lasso, Ridge, DecisionTreeRegressor, RandomForestRegressor, xgb.XGBRegressor]): The input model.
-            train (bool): Defines if you want to plot the scatterplot on train or test data (train by default).
+            train_data (bool): Defines if you want to plot the scatterplot on train or test data (train by default).
             figsize (Tuple[float, float]): Define the size of the prediction_erros plot.
 
         Returns:
             None
         """
         if train_data: 
             ypred = model.predict(self.X_train)
```

### Comparing `edamame-0.49/edamame/regressor/regression.py` & `edamame-0.50/edamame/regressor/regression.py`

 * *Files identical despite different names*

### Comparing `edamame-0.49/edamame.egg-info/PKG-INFO` & `edamame-0.50/edamame.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.49
+Version: 0.50
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -35,38 +35,49 @@
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
+- [Edamame](#edamame)
+  - [Functionalities](#functionalities)
+  - [Eda module](#eda-module)
+  - [Regressor module](#regressor-module)
+    - [Example:](#example)
+  - [Classifier module](#classifier-module)
+    - [Example:](#example-1)
+  - [Todos](#todos)
+
+
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
 ```
 
 the edamame package works correctly inside a jupyter-notebook. You can find the documentation of the package on the [edamame-documentation](https://edamame-doc.readthedocs.io/en/latest/index.html) page.
 
 <hr>
 
 
-## Edamame functionalities
+## Functionalities
 
 
-The package consists of three modules: eda, which performs exploratory data analysis; and regressor and classifier, which handle the training of machine learning models for regression and classification, respectively. To see examples of the uses of the edamame package, you can check out the [edamame-notebook](https://github.com/marcosalvalaggio/edamame-notebooks) repository.
+The package consists of three modules: eda, which performs exploratory data analysis; and regressor and classifier, which handle the training of machine learning models for regression and classification, respectively. To see examples of the uses of the edamame package, you can check out the [examples](https://github.com/marcosalvalaggio/edamame-notebooks) folder in the repository.
 
 <hr>
 
 ## Eda module
 
-
-``import edamame.eda as eda``
+```python
+import edamame.eda as eda
+```
 
 The **eda** module provides a wide range of functions for performing exploratory data analysis (EDA) on datasets. With this module you can easily explore and manipulate your data, conduct descriptive statistics, correlation analysis, and prepare your data for machine learning. The "eda" module offers the following functionalities:
 
 * Data Exploration and Manipulation functions:
 
    - **dimensions**: The function displays the number of rows and columns of a pandas dataframe passed. 
    - **identify_types**: Identify the data types of each column.
@@ -133,14 +144,37 @@
 * **coefficients**: Computes and prints the coefficients of the regression model.
 * **random_forest_fi**: Displays the feature importance plot for the random forest regression model. 
 * **random_forest_fi**: Displays the feature importance plot for the xgboost regression model. 
 * **prediction_error**: Computes and prints the prediction error of the regression model on the test data.
 * **residual_plot**: creates and displays a residual plot for the regression model.
 * **qqplot**: creates and displays a QQ plot for the regression model.
 
+
+### Example:
+
+```python
+from sklearn.datasets import make_regression
+from edamame.regressor import TrainRegressor
+import pandas as pd
+import edamame.eda as eda
+from edamame.regressor import RegressorDiagnose
+X, y = make_regression(n_samples=1000, n_features=5, n_targets=1, random_state=42)
+X = pd.DataFrame(X, columns=["f1", "f2", "f3", "f4", "f5"])
+y = pd.DataFrame(y, columns=["y"])
+X_train, y_train, X_test, y_test = eda.setup(X, y)
+X_train_s = eda.scaling(X_train)
+X_test_s = eda.scaling(X_test)
+regressor = TrainRegressor(X_train_s, y_train, X_test_s, y_test)
+rf = regressor.random_forest()
+regressor.model_metrics()
+diagnose = RegressorDiagnose(X_train_s, y_train, X_test_s, y_test)
+diagnose.random_forest_fi(model=rf)
+diagnose.prediction_error(model=rf)
+```
+
 <hr>
 
 ## Classifier module
 
 
 ```python
 from edamame.classifier import TrainClassifier
```

### Comparing `edamame-0.49/pyproject.toml` & `edamame-0.50/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.49"
+version = "0.50"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

