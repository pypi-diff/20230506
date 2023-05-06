# Comparing `tmp/mlimputer-1.0.1-py3-none-any.whl.zip` & `tmp/mlimputer-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9238 bytes, number of entries: 9
+Zip file size: 9285 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Feb-20 00:15 mlimputer/__init__.py
--rw-rw-rw-  2.0 fat     4690 b- defN 23-Apr-17 14:04 mlimputer/mli_imputation.py
--rw-rw-rw-  2.0 fat     6326 b- defN 23-Apr-17 14:00 mlimputer/mli_model_selection.py
+-rw-rw-rw-  2.0 fat     4834 b- defN 23-May-06 15:58 mlimputer/mli_imputation.py
+-rw-rw-rw-  2.0 fat     6325 b- defN 23-May-06 16:00 mlimputer/mli_model_selection.py
 -rw-rw-rw-  2.0 fat     1402 b- defN 23-Apr-17 14:19 mlimputer/mli_parameters.py
--rw-rw-rw-  2.0 fat     1090 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7003 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      730 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/RECORD
-9 files, 21732 bytes uncompressed, 7980 bytes compressed:  63.3%
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6952 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      730 b- defN 23-May-06 16:24 mlimputer-1.0.5.dist-info/RECORD
+9 files, 21824 bytes uncompressed, 8027 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mlimputer/mli_model_selection.py
 Comment: 
 
 Filename: mlimputer/mli_parameters.py
 Comment: 
 
-Filename: mlimputer-1.0.1.dist-info/LICENSE
+Filename: mlimputer-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: mlimputer-1.0.1.dist-info/METADATA
+Filename: mlimputer-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: mlimputer-1.0.1.dist-info/WHEEL
+Filename: mlimputer-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: mlimputer-1.0.1.dist-info/top_level.txt
+Filename: mlimputer-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mlimputer-1.0.1.dist-info/RECORD
+Filename: mlimputer-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlimputer/mli_imputation.py

```diff
@@ -24,14 +24,18 @@
     """      
     
     df=dataset.copy()
 
     df_md,c=missing_report(df),0
     imp_targets=list(df_md['columns']) 
         
+    for col in df.columns:
+        if df[col].isnull().all():
+            raise ValueError(f'Column {col} is filled with null values')
+    
     # Iterate over each column with missing data and fit the imputation method
     for col in tqdm(imp_targets, desc="Fitting Missing Data Columns", ncols=80): ## imp_targets:
         #print("**** Fitting Column:", col)
         target=col
         
         # Split the data into train and test sets
         total_index = df.index.tolist()
```

## mlimputer/mli_model_selection.py

```diff
@@ -38,15 +38,15 @@
     train=train[sel_cols]
     
     X_train = train.iloc[:, 0:(len(sel_cols)-1)].values
     y_train = train.iloc[:, (len(sel_cols)-1)].values
     
     if algo=='RandomForest':
         rf_params=parameters['RandomForest']
-        model = RandomForestRegressor(**rf_params) 
+        model = RandomForestRegressor(**rf_params)
         model.fit(X_train, y_train)
         
     elif algo=='ExtraTrees':
         et_params=parameters['ExtraTrees']
         model = ExtraTreesRegressor(**et_params)
         model.fit(X_train, y_train)
```

## Comparing `mlimputer-1.0.1.dist-info/LICENSE` & `mlimputer-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlimputer-1.0.1.dist-info/METADATA` & `mlimputer-1.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlimputer
-Version: 1.0.1
+Version: 1.0.5
 Summary: MLimputer - Null Imputation Framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/MLimputer
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data preprecessing,null imputation,predictive null imputation,multiple null imputation,automated machine learning
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
 Requires-Dist: scikit-learn (>=1.0.2)
 Requires-Dist: atlantic (>=1.0.50)
 Requires-Dist: catboost (>=1.1.1)
 Requires-Dist: xgboost (>=1.7.3)
```

## Comparing `mlimputer-1.0.1.dist-info/RECORD` & `mlimputer-1.0.5.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlimputer/__init__.py,sha256=aJxiUy0U6d3cxOQQo5m4ATN4A3xAGwAFCqCl21JTvhM,389
-mlimputer/mli_imputation.py,sha256=yENGhTnMbEUDsiVigut_vRbVURIfavzxX7wSkM8sSjc,4690
-mlimputer/mli_model_selection.py,sha256=s9LzNJawB09psQ6LRzRWSDAegB8LT6RPWv2lSRv51_E,6326
+mlimputer/mli_imputation.py,sha256=clFXtMhBr304RllNvIZ_McnCrHndlF9OfiBiZj3spOM,4834
+mlimputer/mli_model_selection.py,sha256=tEt55AYa4JSBm_zezov_2Or30w4Flj_56VjgKP1-a5U,6325
 mlimputer/mli_parameters.py,sha256=G6x291YIhf--4jdv4gaBNsaxknTKjnqBdl73KEmTPfU,1402
-mlimputer-1.0.1.dist-info/LICENSE,sha256=BMKwnVd_OgrW1_Ls-_WlfHpr-s7KFtcT6t9t9tfFk8g,1090
-mlimputer-1.0.1.dist-info/METADATA,sha256=FDlwms_ysLJsvbnOmYcLl48brhRYlIfbyI7JlnREFFo,7003
-mlimputer-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mlimputer-1.0.1.dist-info/top_level.txt,sha256=6qseujMDdh0A5GoDaKPU6kp9vnXciE1XKZIvz88dVzE,10
-mlimputer-1.0.1.dist-info/RECORD,,
+mlimputer-1.0.5.dist-info/LICENSE,sha256=BMKwnVd_OgrW1_Ls-_WlfHpr-s7KFtcT6t9t9tfFk8g,1090
+mlimputer-1.0.5.dist-info/METADATA,sha256=8f611ydtMyAZT9ykZxT4mZfP-Wja94v4VOkUmqPSYHE,6952
+mlimputer-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mlimputer-1.0.5.dist-info/top_level.txt,sha256=6qseujMDdh0A5GoDaKPU6kp9vnXciE1XKZIvz88dVzE,10
+mlimputer-1.0.5.dist-info/RECORD,,
```

