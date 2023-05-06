# Comparing `tmp/nalyst-0.2.7.tar.gz` & `tmp/nalyst-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.2.7.tar", last modified: Tue May  2 16:30:35 2023, max compression
+gzip compressed data, was "nalyst-0.3.0.tar", last modified: Sat May  6 07:01:50 2023, max compression
```

## Comparing `nalyst-0.2.7.tar` & `nalyst-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:30:35.799154 nalyst-0.2.7/
--rw-rw-rw-   0        0        0      146 2023-05-02 16:17:38.000000 nalyst-0.2.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.7/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4239 2023-05-02 16:30:35.798158 nalyst-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-05-02 16:16:51.000000 nalyst-0.2.7/README.md
--rw-rw-rw-   0        0        0     1298 2023-05-02 16:12:27.000000 nalyst-0.2.7/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:30:35.794171 nalyst-0.2.7/nalyst/
--rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.7/nalyst/BetaFive.py
--rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.7/nalyst/BetaMax.py
--rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-0.2.7/nalyst/CorrelationAnalysis.py
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.7/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.7/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.7/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.7/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.7/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.7/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.2.7/nalyst/MonteCarloSimulator.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.7/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.7/nalyst/RegressionPlot.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.7/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     2341 2023-05-02 16:29:32.000000 nalyst-0.2.7/nalyst/StockVolatility.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.7/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.7/nalyst/ThresholdClassifier.py
--rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-0.2.7/nalyst/TrendAnalyst.py
--rw-rw-rw-   0        0        0     1298 2023-05-02 16:11:56.000000 nalyst-0.2.7/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:30:35.797161 nalyst-0.2.7/nalyst.egg-info/
--rw-rw-rw-   0        0        0     4239 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 16:30:35.000000 nalyst-0.2.7/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 16:30:35.799154 nalyst-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-05-02 16:29:45.000000 nalyst-0.2.7/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.2.7/version.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:01:50.944313 nalyst-0.3.0/
+-rw-rw-rw-   0        0        0      185 2023-05-06 07:00:46.000000 nalyst-0.3.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4201 2023-05-06 07:01:50.944313 nalyst-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3039 2023-05-06 07:01:11.000000 nalyst-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1369 2023-05-06 07:00:07.000000 nalyst-0.3.0/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:01:50.940818 nalyst-0.3.0/nalyst/
+-rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.3.0/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.3.0/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-0.3.0/nalyst/CorrelationAnalysis.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.3.0/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.3.0/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.3.0/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.3.0/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.3.0/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.3.0/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-0.3.0/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.3.0/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.3.0/nalyst/RegressionPlot.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.3.0/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     3285 2023-05-06 06:46:38.000000 nalyst-0.3.0/nalyst/StockAnalyzer.py
+-rw-rw-rw-   0        0        0     2341 2023-05-02 16:29:32.000000 nalyst-0.3.0/nalyst/StockVolatility.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.3.0/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.3.0/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-0.3.0/nalyst/TrendAnalyst.py
+-rw-rw-rw-   0        0        0     1369 2023-05-06 07:00:18.000000 nalyst-0.3.0/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:01:50.942811 nalyst-0.3.0/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     4201 2023-05-06 07:01:50.000000 nalyst-0.3.0/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2023-05-06 07:01:50.000000 nalyst-0.3.0/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:01:50.000000 nalyst-0.3.0/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-06 07:01:50.000000 nalyst-0.3.0/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 07:01:50.000000 nalyst-0.3.0/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:01:50.945319 nalyst-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1536 2023-05-06 06:53:39.000000 nalyst-0.3.0/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 16:17:46.000000 nalyst-0.3.0/version.py
```

### Comparing `nalyst-0.2.7/LICENSE` & `nalyst-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/PKG-INFO` & `nalyst-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.7
-Summary: A small package for data analyst
+Version: 0.3.0
+Summary: Packages for quantative analyst
 Home-page: https://github.com/harryworlds/nalyst
-Author: Hemant Thapa
-Author-email: hemantthapa1998@gmail.com
+Author: Hemant Thapa, Kiran Basnet
+Author-email: hemantthapa1998@gmail.com, kiransbasnet@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
@@ -57,17 +57,17 @@
 ```text
 pip install nalyst
 
 pip install --upgrade nalyst
 
 pip show nalyst
 ```
-```
-4. IMPORT DEPENDENCY 
 
+4. IMPORT DEPENDENCY 
+```
 import numpy as np
 import matplotlib.pyplot as plt
 import yfinance as yf
 import pyttsx3
 import seaborn as sns
 import yfinance as yf
 import datetime
@@ -88,21 +88,18 @@
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
+from nalyst.StockAnalyzer import StockAnalyzer
 ```
 
 6. SUPPORT
 
 If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
 7. COMMUNICATION 
 
-LinkedIn: https://www.linkedin.com/in/thapahemant/
-
-YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
-
 Github: https://github.com/harryworlds/nalyst
```

### Comparing `nalyst-0.2.7/README.md` & `nalyst-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 ```text
 pip install nalyst
 
 pip install --upgrade nalyst
 
 pip show nalyst
 ```
-```
-4. IMPORT DEPENDENCY 
 
+4. IMPORT DEPENDENCY 
+```
 import numpy as np
 import matplotlib.pyplot as plt
 import yfinance as yf
 import pyttsx3
 import seaborn as sns
 import yfinance as yf
 import datetime
@@ -63,21 +63,18 @@
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
+from nalyst.StockAnalyzer import StockAnalyzer
 ```
 
 6. SUPPORT
 
 If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
 7. COMMUNICATION 
 
-LinkedIn: https://www.linkedin.com/in/thapahemant/
-
-YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
-
 Github: https://github.com/harryworlds/nalyst
```

### Comparing `nalyst-0.2.7/__init__.py` & `nalyst-0.3.0/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
+from nalyst.StockAnalyzer import StockAnalyzer
 
 __all__ = [
-    'LinearRegression',
-    'DecisionTree',
-    'KMeans',
-    'PCA',
-    'LogisticRegression',
-    'MaxAbsScaler',
-    'MinMaxScaler',
-    'StandardScaler',
-    'TestTrainSplit',
-    'MonteCarloSimulator',
-    'BetaFive',
-    'BetaMax',
-    'SharpRatio',
-    'ThresholdClassifier',
-    'LinearCorrelationVisualizer',
-    'LinearRegressionVisualizer',
-    'StockVolatility'
+    "LinearRegression",
+    "DecisionTree",
+    "KMeans",
+    "PCA",
+    "LogisticRegression",
+    "MaxAbsScaler",
+    "MinMaxScaler",
+    "StandardScaler",
+    "TestTrainSplit",
+    "MonteCarloSimulator",
+    "BetaFive",
+    "BetaMax",
+    "SharpRatio",
+    "ThresholdClassifier",
+    "LinearCorrelationVisualizer",
+    "LinearRegressionVisualizer",
+    "StockVolatility",
+    "StockAnalyzer",
 ]
```

### Comparing `nalyst-0.2.7/nalyst/BetaFive.py` & `nalyst-0.3.0/nalyst/BetaFive.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/BetaMax.py` & `nalyst-0.3.0/nalyst/BetaMax.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/CorrelationAnalysis.py` & `nalyst-0.3.0/nalyst/CorrelationAnalysis.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/DecisionTree.py` & `nalyst-0.3.0/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/KMeans.py` & `nalyst-0.3.0/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/LinearRegression.py` & `nalyst-0.3.0/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/LogisticRegression.py` & `nalyst-0.3.0/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/MaxAbsScaler.py` & `nalyst-0.3.0/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/MinMaxScaler.py` & `nalyst-0.3.0/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/MonteCarloSimulator.py` & `nalyst-0.3.0/nalyst/MonteCarloSimulator.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/PCA.py` & `nalyst-0.3.0/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/RegressionPlot.py` & `nalyst-0.3.0/nalyst/RegressionPlot.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/StandardScaler.py` & `nalyst-0.3.0/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/StockVolatility.py` & `nalyst-0.3.0/nalyst/StockVolatility.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/TestTrainSplit.py` & `nalyst-0.3.0/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/ThresholdClassifier.py` & `nalyst-0.3.0/nalyst/ThresholdClassifier.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/TrendAnalyst.py` & `nalyst-0.3.0/nalyst/TrendAnalyst.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.2.7/nalyst/__init__.py` & `nalyst-0.3.0/nalyst/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
+from nalyst.StockAnalyzer import StockAnalyzer
 
 __all__ = [
-    'LinearRegression',
-    'DecisionTree',
-    'KMeans',
-    'PCA',
-    'LogisticRegression',
-    'MaxAbsScaler',
-    'MinMaxScaler',
-    'StandardScaler',
-    'TestTrainSplit',
-    'MonteCarloSimulator',
-    'BetaFive',
-    'BetaMax',
-    'SharpRatio',
-    'ThresholdClassifier',
-    'LinearCorrelationVisualizer',
-    'LinearRegressionVisualizer',
-    'StockVolatility'
+    "LinearRegression",
+    "DecisionTree",
+    "KMeans",
+    "PCA",
+    "LogisticRegression",
+    "MaxAbsScaler",
+    "MinMaxScaler",
+    "StandardScaler",
+    "TestTrainSplit",
+    "MonteCarloSimulator",
+    "BetaFive",
+    "BetaMax",
+    "SharpRatio",
+    "ThresholdClassifier",
+    "LinearCorrelationVisualizer",
+    "LinearRegressionVisualizer",
+    "StockVolatility",
+    "StockAnalyzer",
 ]
```

### Comparing `nalyst-0.2.7/nalyst.egg-info/PKG-INFO` & `nalyst-0.3.0/nalyst.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.2.7
-Summary: A small package for data analyst
+Version: 0.3.0
+Summary: Packages for quantative analyst
 Home-page: https://github.com/harryworlds/nalyst
-Author: Hemant Thapa
-Author-email: hemantthapa1998@gmail.com
+Author: Hemant Thapa, Kiran Basnet
+Author-email: hemantthapa1998@gmail.com, kiransbasnet@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
@@ -57,17 +57,17 @@
 ```text
 pip install nalyst
 
 pip install --upgrade nalyst
 
 pip show nalyst
 ```
-```
-4. IMPORT DEPENDENCY 
 
+4. IMPORT DEPENDENCY 
+```
 import numpy as np
 import matplotlib.pyplot as plt
 import yfinance as yf
 import pyttsx3
 import seaborn as sns
 import yfinance as yf
 import datetime
@@ -88,21 +88,18 @@
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
+from nalyst.StockAnalyzer import StockAnalyzer
 ```
 
 6. SUPPORT
 
 If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
 7. COMMUNICATION 
 
-LinkedIn: https://www.linkedin.com/in/thapahemant/
-
-YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
-
 Github: https://github.com/harryworlds/nalyst
```

### Comparing `nalyst-0.2.7/nalyst.egg-info/SOURCES.txt` & `nalyst-0.3.0/nalyst.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 nalyst/LogisticRegression.py
 nalyst/MaxAbsScaler.py
 nalyst/MinMaxScaler.py
 nalyst/MonteCarloSimulator.py
 nalyst/PCA.py
 nalyst/RegressionPlot.py
 nalyst/StandardScaler.py
+nalyst/StockAnalyzer.py
 nalyst/StockVolatility.py
 nalyst/TestTrainSplit.py
 nalyst/ThresholdClassifier.py
 nalyst/TrendAnalyst.py
 nalyst/__init__.py
 nalyst.egg-info/PKG-INFO
 nalyst.egg-info/SOURCES.txt
```

### Comparing `nalyst-0.2.7/setup.py` & `nalyst-0.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 from setuptools import setup, find_packages
 import io
 from os import path
 
-with io.open('README.md', 'r', encoding='utf-8') as f:
+with io.open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='nalyst',
-    version='0.2.7',
-    author='Hemant Thapa',
-    author_email='hemantthapa1998@gmail.com',
-    description='A small package for data analyst',
+    name="nalyst",
+    version="0.3.0",
+    author="Hemant Thapa, Kiran Basnet",
+    author_email="hemantthapa1998@gmail.com, kiransbasnet@gmail.com",
+    description="Packages for quantative analyst",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/harryworlds/nalyst',
+    long_description_content_type="text/markdown",
+    url="https://github.com/harryworlds/nalyst",
     packages=find_packages(),
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Education',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Education",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
-    keywords='pandas, random, numpy, pandas datareader, seaborn, matplotlib',
+    keywords="pandas, random, numpy, pandas datareader, seaborn, matplotlib",
     install_requires=[
-        'pandas>=1.3.0',
-        'numpy>=1.16.5',
-        'requests>=2.26.0',
-        'seaborn>=0.11.0',
-        'matplotlib>=3.4.0',
+        "pandas>=1.3.0",
+        "numpy>=1.16.5",
+        "requests>=2.26.0",
+        "seaborn>=0.11.0",
+        "matplotlib>=3.4.0",
     ],
-    extras_require={
-        'test': [
-            'pytest>=6.2.4',
-            'coverage>=5.5'
-        ]
-    },
-    python_requires='>=3.6',
+    extras_require={"test": ["pytest>=6.2.4", "coverage>=5.5"]},
+    python_requires=">=3.6",
 )
```

