# Comparing `tmp/kennard_stone-2.1.0.tar.gz` & `tmp/kennard_stone-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kennard_stone-2.1.0.tar", last modified: Mon May  1 14:30:08 2023, max compression
+gzip compressed data, was "kennard_stone-2.1.1.tar", last modified: Sat May  6 04:59:14 2023, max compression
```

## Comparing `kennard_stone-2.1.0.tar` & `kennard_stone-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-01 14:30:08.072441 kennard_stone-2.1.0/
--rw-r--r--   0 yu9824     (501) staff       (20)     1063 2022-04-23 07:40:26.000000 kennard_stone-2.1.0/LICENSE
--rw-r--r--   0 yu9824     (501) staff       (20)       71 2023-04-22 06:08:03.000000 kennard_stone-2.1.0/MANIFEST.in
--rw-r--r--   0 yu9824     (501) staff       (20)     6217 2023-05-01 14:30:08.072330 kennard_stone-2.1.0/PKG-INFO
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-01 14:30:08.071564 kennard_stone-2.1.0/kennard_stone/
--rw-r--r--   0 yu9824     (501) staff       (20)      360 2023-05-01 14:28:01.000000 kennard_stone-2.1.0/kennard_stone/__init__.py
--rw-r--r--   0 yu9824     (501) staff       (20)     3160 2023-04-22 05:20:01.000000 kennard_stone-2.1.0/kennard_stone/_deprecated.py
--rw-r--r--   0 yu9824     (501) staff       (20)    16105 2023-05-01 14:28:01.000000 kennard_stone-2.1.0/kennard_stone/kennard_stone.py
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-01 14:30:08.072176 kennard_stone-2.1.0/kennard_stone.egg-info/
--rw-r--r--   0 yu9824     (501) staff       (20)     6217 2023-05-01 14:30:07.000000 kennard_stone-2.1.0/kennard_stone.egg-info/PKG-INFO
--rw-r--r--   0 yu9824     (501) staff       (20)      315 2023-05-01 14:30:08.000000 kennard_stone-2.1.0/kennard_stone.egg-info/SOURCES.txt
--rw-r--r--   0 yu9824     (501) staff       (20)        1 2023-05-01 14:30:07.000000 kennard_stone-2.1.0/kennard_stone.egg-info/dependency_links.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-05-01 14:30:07.000000 kennard_stone-2.1.0/kennard_stone.egg-info/requires.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       14 2023-05-01 14:30:08.000000 kennard_stone-2.1.0/kennard_stone.egg-info/top_level.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-22 05:20:01.000000 kennard_stone-2.1.0/requirements.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       38 2023-05-01 14:30:08.072477 kennard_stone-2.1.0/setup.cfg
--rw-r--r--   0 yu9824     (501) staff       (20)     2645 2023-04-22 06:08:03.000000 kennard_stone-2.1.0/setup.py
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-06 04:59:14.602037 kennard_stone-2.1.1/
+-rw-r--r--   0 yu9824     (501) staff       (20)     1063 2022-04-23 07:40:26.000000 kennard_stone-2.1.1/LICENSE
+-rw-r--r--   0 yu9824     (501) staff       (20)       71 2023-04-22 06:08:03.000000 kennard_stone-2.1.1/MANIFEST.in
+-rw-r--r--   0 yu9824     (501) staff       (20)     6478 2023-05-06 04:59:14.601900 kennard_stone-2.1.1/PKG-INFO
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-06 04:59:14.600878 kennard_stone-2.1.1/kennard_stone/
+-rw-r--r--   0 yu9824     (501) staff       (20)      360 2023-05-04 07:44:31.000000 kennard_stone-2.1.1/kennard_stone/__init__.py
+-rw-r--r--   0 yu9824     (501) staff       (20)     3160 2023-04-22 05:20:01.000000 kennard_stone-2.1.1/kennard_stone/_deprecated.py
+-rw-r--r--   0 yu9824     (501) staff       (20)    16333 2023-05-06 04:51:27.000000 kennard_stone-2.1.1/kennard_stone/kennard_stone.py
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-05-06 04:59:14.601699 kennard_stone-2.1.1/kennard_stone.egg-info/
+-rw-r--r--   0 yu9824     (501) staff       (20)     6478 2023-05-06 04:59:14.000000 kennard_stone-2.1.1/kennard_stone.egg-info/PKG-INFO
+-rw-r--r--   0 yu9824     (501) staff       (20)      315 2023-05-06 04:59:14.000000 kennard_stone-2.1.1/kennard_stone.egg-info/SOURCES.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)        1 2023-05-06 04:59:14.000000 kennard_stone-2.1.1/kennard_stone.egg-info/dependency_links.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-05-06 04:59:14.000000 kennard_stone-2.1.1/kennard_stone.egg-info/requires.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       14 2023-05-06 04:59:14.000000 kennard_stone-2.1.1/kennard_stone.egg-info/top_level.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-22 05:20:01.000000 kennard_stone-2.1.1/requirements.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       38 2023-05-06 04:59:14.602079 kennard_stone-2.1.1/setup.cfg
+-rw-r--r--   0 yu9824     (501) staff       (20)     2645 2023-04-22 06:08:03.000000 kennard_stone-2.1.1/setup.py
```

### Comparing `kennard_stone-2.1.0/LICENSE` & `kennard_stone-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kennard_stone-2.1.0/PKG-INFO` & `kennard_stone-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kennard_stone
-Version: 2.1.0
+Version: 2.1.1
 Summary: A method for selecting samples by spreading the training data evenly.
 Home-page: https://github.com/yu9824/kennard_stone
 Author: yu9824
 Author-email: yu.9824.job@gmail.com
 Maintainer: yu9824
 Maintainer-email: yu.9824.job@gmail.com
 License: MIT
@@ -137,15 +137,17 @@
 ```python
 from sklearn.model_selection import KFold
 from sklearn.model_selection import cross_validate
 
 kf = KFold(n_splits=5, shuffle=True, random_state=334)
 print(cross_validate(estimator, X, y, cv=kf))
 ```
+
 OR
+
 ```python
 from sklearn.model_selection import cross_validate
 
 print(cross_validate(estimator, X, y, cv=5))
 ```
 
 
@@ -154,18 +156,28 @@
 There is no notion of `random_state` or `shuffle` because the partitioning is determined uniquely for the dataset.
 If these arguments are included, they do not cause an error. They simply have no effect on the result. Please be careful.
 
 If you want to run the notebook in example directory, you will need to additionally download `pandas`, `matplotlib`, `seaborn`, `tqdm`, and `jupyter` other than the packages in requirements.txt.
 
 ## Parallelization (since v2.1.0)
 
-This algorithm is very computationally intensive and takes a lot of computation time.
-To solve this problem, we have implemented parallelization and optimized the algorithm since v2.1.0.
+This algorithm is very computationally intensive and takes a lot of time.
+To solve this problem, I have implemented parallelization and optimized the algorithm since v2.1.0.
 `n_jobs` can be specified for parallelization as in the scikit-learn-like api.
 
+```python
+# parallelization KFold
+kf = KFold(n_splits=5, n_jobs=-1)
+
+# parallelization train_test_split
+X_train, X_test, y_train, y_test = train_test_split(
+    X, y, test_size=0.2, n_jobs=-1
+)
+```
+
 
 ## LICENSE
 
 MIT Licence
 
 Copyright (c) 2021 yu9824
 
@@ -194,11 +206,15 @@
 - Fix bug with Python3.7.
 
 ### v2.1.0
 
 - Optimize algorithm
 - Deal with Large number of data.
   - parallel calculation when calculating distance (Add `n_jobs` argument)
-  - recursion number settings
+  - replacing recursive functions with for-loops
 - Add other than "euclidean" calculation methods (Add `metric` argument)
 
+### v2.1.1
+
+- Fix bug when `metric="nan_euclidean"`.
+
```

### Comparing `kennard_stone-2.1.0/kennard_stone/_deprecated.py` & `kennard_stone-2.1.1/kennard_stone/_deprecated.py`

 * *Files identical despite different names*

### Comparing `kennard_stone-2.1.0/kennard_stone/kennard_stone.py` & `kennard_stone-2.1.1/kennard_stone/kennard_stone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Copyright © 2021 yu9824
 """
 
 from typing import overload, Union, Optional, Generator
 
-# deprecated in Python >= 3.9
+# The fllowing has deprecated in Python >= 3.9
 from typing import List, Set
+
 from itertools import chain
 import warnings
 
 import numpy as np
-
 from sklearn.model_selection._split import BaseShuffleSplit
 from sklearn.model_selection._split import _BaseKFold
 from sklearn.model_selection._split import _validate_shuffle_split
 from sklearn.utils.validation import _num_samples
 from sklearn.utils import indexable
 from sklearn.utils import _safe_indexing
 from sklearn.preprocessing import StandardScaler
@@ -40,15 +40,16 @@
 
     def __init__(
         self,
         n_splits: int = 5,
         *,
         metric: str = "euclidean",
         n_jobs: Optional[int] = None,
-        **kwargs,
+        random_state: None = None,
+        shuffle: None = None,
     ) -> None:
         """K-Folds cross-validator using the Kennard-Stone algorithm.
 
         Parameters
         ----------
         n_splits : int, optional
             Number of folds. Must be at least 2., by default 5
@@ -74,23 +75,23 @@
         n_jobs : int, optional
             The number of parallel jobs., by default None
         """
         super().__init__(n_splits=n_splits, shuffle=False, random_state=None)
         self.metric = metric
         self.n_jobs = n_jobs
 
-        if "shuffle" in kwargs:
+        if shuffle is not None:
             warnings.warn(
                 "`shuffle` is unnecessary because it is always shuffled"
                 " in this algorithm.",
                 UserWarning,
             )
         del self.shuffle
 
-        if "random_state" in kwargs:
+        if random_state is not None:
             warnings.warn(
                 "`random_state` is unnecessary since it is uniquely determined"
                 " in this algorithm.",
                 UserWarning,
             )
         del self.random_state
 
@@ -162,15 +163,16 @@
 
 def train_test_split(
     *arrays,
     test_size: Optional[Union[float, int]] = None,
     train_size: Optional[Union[float, int]] = None,
     metric: str = "euclidean",
     n_jobs: Optional[int] = None,
-    **kwargs,
+    random_state: None = None,
+    shuffle: None = None,
 ) -> list:
     """Split arrays or matrices into train and test subsets using the
     Kennard-Stone algorithm.
 
     Data partitioning by the Kennard-Stone algorithm is performed based on the
      first element to be input.
 
@@ -219,22 +221,22 @@
     splitting : list, length=2 * len(arrays)
         List containing train-test split of inputs
 
     Raises
     ------
     ValueError
     """
-    if "shuffle" in kwargs:
+    if shuffle is not None:
         warnings.warn(
             "`shuffle` is unnecessary because it is always shuffled"
             " in this algorithm.",
             UserWarning,
         )
 
-    if "random_state" in kwargs:
+    if random_state is not None:
         warnings.warn(
             "`random_state` is unnecessary since it is uniquely determined"
             " in this algorithm.",
             UserWarning,
         )
 
     n_arrays = len(arrays)
@@ -304,15 +306,22 @@
         self.n_groups = n_groups
         self.scale = scale
         self.metric = metric
         self.n_jobs = n_jobs
 
     def get_indexes(self, X) -> List[List[int]]:
         # check input array
-        X: np.ndarray = check_array(X, ensure_2d=True, dtype="numeric")
+        X: np.ndarray = check_array(
+            X,
+            ensure_2d=True,
+            dtype="numeric",
+            force_all_finite="allow-nan"
+            if self.metric == "nan_euclidean"
+            else True,
+        )
         n_samples = X.shape[0]
 
         # drop no variance
         vselector = VarianceThreshold(threshold=0.0)
         X = vselector.fit_transform(X)
 
         if self.scale:
@@ -339,16 +348,14 @@
         # 最大値を取るサンプル (平均からの距離が一番遠い) のindex_numberを保存
         idx_farthest: List[int] = np.argsort(distance_to_ave)[::-1][
             : self.n_groups
         ].tolist()
 
         distance_min = self.distance_matrix[idx_farthest, :]
 
-        # recursion limit settings
-
         # params
         indexes_selected = idx_farthest
         lst_indexes_selected_prev = [[] for _ in range(self.n_groups)]
         indexes_remaining_prev = list(range(n_samples))
 
         for _ in range(
             n_samples // self.n_groups + bool(n_samples % self.n_groups) - 1
```

### Comparing `kennard_stone-2.1.0/kennard_stone.egg-info/PKG-INFO` & `kennard_stone-2.1.1/kennard_stone.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kennard-stone
-Version: 2.1.0
+Version: 2.1.1
 Summary: A method for selecting samples by spreading the training data evenly.
 Home-page: https://github.com/yu9824/kennard_stone
 Author: yu9824
 Author-email: yu.9824.job@gmail.com
 Maintainer: yu9824
 Maintainer-email: yu.9824.job@gmail.com
 License: MIT
@@ -137,15 +137,17 @@
 ```python
 from sklearn.model_selection import KFold
 from sklearn.model_selection import cross_validate
 
 kf = KFold(n_splits=5, shuffle=True, random_state=334)
 print(cross_validate(estimator, X, y, cv=kf))
 ```
+
 OR
+
 ```python
 from sklearn.model_selection import cross_validate
 
 print(cross_validate(estimator, X, y, cv=5))
 ```
 
 
@@ -154,18 +156,28 @@
 There is no notion of `random_state` or `shuffle` because the partitioning is determined uniquely for the dataset.
 If these arguments are included, they do not cause an error. They simply have no effect on the result. Please be careful.
 
 If you want to run the notebook in example directory, you will need to additionally download `pandas`, `matplotlib`, `seaborn`, `tqdm`, and `jupyter` other than the packages in requirements.txt.
 
 ## Parallelization (since v2.1.0)
 
-This algorithm is very computationally intensive and takes a lot of computation time.
-To solve this problem, we have implemented parallelization and optimized the algorithm since v2.1.0.
+This algorithm is very computationally intensive and takes a lot of time.
+To solve this problem, I have implemented parallelization and optimized the algorithm since v2.1.0.
 `n_jobs` can be specified for parallelization as in the scikit-learn-like api.
 
+```python
+# parallelization KFold
+kf = KFold(n_splits=5, n_jobs=-1)
+
+# parallelization train_test_split
+X_train, X_test, y_train, y_test = train_test_split(
+    X, y, test_size=0.2, n_jobs=-1
+)
+```
+
 
 ## LICENSE
 
 MIT Licence
 
 Copyright (c) 2021 yu9824
 
@@ -194,11 +206,15 @@
 - Fix bug with Python3.7.
 
 ### v2.1.0
 
 - Optimize algorithm
 - Deal with Large number of data.
   - parallel calculation when calculating distance (Add `n_jobs` argument)
-  - recursion number settings
+  - replacing recursive functions with for-loops
 - Add other than "euclidean" calculation methods (Add `metric` argument)
 
+### v2.1.1
+
+- Fix bug when `metric="nan_euclidean"`.
+
```

### Comparing `kennard_stone-2.1.0/setup.py` & `kennard_stone-2.1.1/setup.py`

 * *Files identical despite different names*

