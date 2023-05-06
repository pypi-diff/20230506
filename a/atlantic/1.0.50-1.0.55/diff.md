# Comparing `tmp/atlantic-1.0.50-py3-none-any.whl.zip` & `tmp/atlantic-1.0.55-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18679 bytes, number of entries: 12
+Zip file size: 18666 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Feb-20 00:15 atlantic/__init__.py
 -rw-rw-rw-  2.0 fat     5510 b- defN 23-Apr-17 10:17 atlantic/atl_feat_eng.py
 -rw-rw-rw-  2.0 fat     8704 b- defN 23-Apr-17 10:49 atlantic/atl_feat_selection.py
 -rw-rw-rw-  2.0 fat     1563 b- defN 23-Apr-17 09:56 atlantic/atl_metrics.py
--rw-rw-rw-  2.0 fat     2858 b- defN 23-Apr-17 10:11 atlantic/atl_performance.py
+-rw-rw-rw-  2.0 fat     2862 b- defN 23-May-06 15:26 atlantic/atl_performance.py
 -rw-rw-rw-  2.0 fat     8541 b- defN 23-Apr-17 10:17 atlantic/atl_pipeline.py
--rw-rw-rw-  2.0 fat    20614 b- defN 23-Apr-17 11:27 atlantic/atl_processing.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12367 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      969 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/RECORD
-12 files, 62694 bytes uncompressed, 17059 bytes compressed:  72.8%
+-rw-rw-rw-  2.0 fat    20571 b- defN 23-May-06 15:42 atlantic/atl_processing.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12316 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      969 b- defN 23-May-06 16:35 atlantic-1.0.55.dist-info/RECORD
+12 files, 62604 bytes uncompressed, 17046 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: atlantic/atl_pipeline.py
 Comment: 
 
 Filename: atlantic/atl_processing.py
 Comment: 
 
-Filename: atlantic-1.0.50.dist-info/LICENSE
+Filename: atlantic-1.0.55.dist-info/LICENSE
 Comment: 
 
-Filename: atlantic-1.0.50.dist-info/METADATA
+Filename: atlantic-1.0.55.dist-info/METADATA
 Comment: 
 
-Filename: atlantic-1.0.50.dist-info/WHEEL
+Filename: atlantic-1.0.55.dist-info/WHEEL
 Comment: 
 
-Filename: atlantic-1.0.50.dist-info/top_level.txt
+Filename: atlantic-1.0.55.dist-info/top_level.txt
 Comment: 
 
-Filename: atlantic-1.0.50.dist-info/RECORD
+Filename: atlantic-1.0.55.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atlantic/atl_performance.py

```diff
@@ -10,15 +10,15 @@
 from .atl_feat_eng import target_type, divide_dfs
 from .atl_metrics import metrics_regression, metrics_classification
 
 def pred_eval(train:pd.DataFrame, test:pd.DataFrame, target:str):
     
     X_train,X_test,y_train,y_test=divide_dfs(train,test,target)  
     
-    list_estimators,rf,et=[100],[],[]
+    list_estimators,rf,et=[100,150],[],[]
     pred_type, eval_metric=target_type(train, target)
     
     for estimators in list_estimators:
         
         if pred_type=='Reg': 
             regressor_RF = RandomForestRegressor(n_estimators=estimators, random_state=42)
             regressor_RF.fit(X_train, y_train)
```

## atlantic/atl_processing.py

```diff
@@ -15,15 +15,15 @@
     
     :param df:pd.DataFrame: Specify the dataframe that you want to fit
     :param target:str: Specify the target variable
     :param strat:str: Specify the strategy to use when replacing missing values
     :return: A simpleimputer object
     """
     
-    df,df_=dataset.copy(),dataset.copy()
+    df=dataset.copy()
     df=df.loc[:, df.columns != target]
     input_cols= list(df.columns)
 
 
     imputer = SimpleImputer(missing_values=np.nan, strategy=strat)
     imputer.fit(df)
     
@@ -56,15 +56,15 @@
     
     return df_
 
 def fit_KnnImp(dataset:pd.DataFrame, 
                target:str, 
                neighbors:int=5):
     
-    df,df_=dataset.copy(),dataset.copy()
+    df=dataset.copy()
     df=df.loc[:, df.columns != target]
     imputer = KNNImputer(n_neighbors=neighbors)
     imputer.fit(df)
     
     return imputer
 
 def transform_KnnImp(dataset:pd.DataFrame,
@@ -83,15 +83,15 @@
     
     return df_
 
 def fit_IterImp(dataset:pd.DataFrame, 
                 target:str, 
                 order:str='ascending'):
     
-    df,df_=dataset.copy(),dataset.copy()
+    df=dataset.copy()
     
     df=df.loc[:, df.columns != target]
     imputer = IterativeImputer(imputation_order=order,max_iter=10,random_state=0,n_nearest_features=None)
     imputer=imputer.fit(df)
 
     return imputer
 
@@ -551,7 +551,14 @@
     elif list_encoding[0]==p_v4:
         enc_method='Encoding Version 4'
         print('Encoding Version 4 was choosen with an ', metric, ' of: ', round(p_v4, 4))
         print(' ')
         
     return enc_method
 
+
+
+
+
+
+
+
```

## Comparing `atlantic-1.0.50.dist-info/LICENSE` & `atlantic-1.0.55.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `atlantic-1.0.50.dist-info/METADATA` & `atlantic-1.0.55.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlantic
-Version: 1.0.50
+Version: 1.0.55
 Summary: Atlantic is an automated preprocessing framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/Atlantic
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data processing,predictive modeling,data preprocessing,automated data preprocessing,automated machine learning,automl
 Classifier: Intended Audience :: Education
@@ -14,15 +14,14 @@
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: numpy (>=1.19.5)
 Requires-Dist: cane (>=2.3.1)
 Requires-Dist: scikit-learn (>=1.2.2)
```

## Comparing `atlantic-1.0.50.dist-info/RECORD` & `atlantic-1.0.55.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 atlantic/__init__.py,sha256=aJxiUy0U6d3cxOQQo5m4ATN4A3xAGwAFCqCl21JTvhM,389
 atlantic/atl_feat_eng.py,sha256=qTxn3NxyT_GRR4gdmlLCIrNfL5xViqZEQ29iQpo8cug,5510
 atlantic/atl_feat_selection.py,sha256=r1H8N7DEbbNgo8jUT9kA-5JRmc9v1WVZ3Bf1zU-ACAI,8704
 atlantic/atl_metrics.py,sha256=ZbP98YCmgf0UTiCtozQDRzVARP4EWy9GvzqbQ1XcJ_s,1563
-atlantic/atl_performance.py,sha256=uhTLsE0yuzBGaCxisz30KdpqRSgpEIab3eYMMwsgd2w,2858
+atlantic/atl_performance.py,sha256=1O9718eY3Ppko1COIYO8MKMS7eaH0xP5fc2CKX0Hlaw,2862
 atlantic/atl_pipeline.py,sha256=Fn77_CUA09jZNXkgUJc3yqGWBu7KNBXmcC6eLJU-7qc,8541
-atlantic/atl_processing.py,sha256=QkSVuSFLb3JtvCZbEuDckn4MGjQdeLAQJ2ZifKCp3TA,20614
-atlantic-1.0.50.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
-atlantic-1.0.50.dist-info/METADATA,sha256=AvRNxZoe1bt1Aj9UBitNzqABMNyjvWkl5JXVIXPx6PU,12367
-atlantic-1.0.50.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-atlantic-1.0.50.dist-info/top_level.txt,sha256=RAc3T5Fn4vx9TZ0hPSO3jINJDLLfOOLdANbFmLJQAnU,9
-atlantic-1.0.50.dist-info/RECORD,,
+atlantic/atl_processing.py,sha256=R97TbF5_4p8XyilGFhWzViIHbwRd4XscXzbC8yBKRvs,20571
+atlantic-1.0.55.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
+atlantic-1.0.55.dist-info/METADATA,sha256=mCnocJuRSSHO4nFyP6jmtKtw1ocz74z0UqyQ35i99jo,12316
+atlantic-1.0.55.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+atlantic-1.0.55.dist-info/top_level.txt,sha256=RAc3T5Fn4vx9TZ0hPSO3jINJDLLfOOLdANbFmLJQAnU,9
+atlantic-1.0.55.dist-info/RECORD,,
```

