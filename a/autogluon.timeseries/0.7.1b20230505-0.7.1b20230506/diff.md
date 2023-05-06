# Comparing `tmp/autogluon.timeseries-0.7.1b20230505.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230505.tar", last modified: Fri May  5 09:04:37 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230506.tar", last modified: Sat May  6 09:04:00 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230505.tar` & `autogluon.timeseries-0.7.1b20230506.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.788071 autogluon.timeseries-0.7.1b20230505/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.788071 autogluon.timeseries-0.7.1b20230505/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    46701 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.805012 autogluon.timeseries-0.7.1b20230506/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-06 09:04:00.805012 autogluon.timeseries-0.7.1b20230506/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 09:04:00.805012 autogluon.timeseries-0.7.1b20230506/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.797012 autogluon.timeseries-0.7.1b20230506/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.797012 autogluon.timeseries-0.7.1b20230506/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46702 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.801012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.805012 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-06 09:03:19.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 09:04:00.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:04:00.797012 autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-06 09:04:00.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-06 09:04:00.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:04:00.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 09:04:00.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-06 09:04:00.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 09:04:00.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:04:00.000000 autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230505/PKG-INFO` & `autogluon.timeseries-0.7.1b20230506/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230505
+Version: 0.7.1b20230506
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230505/setup.py` & `autogluon.timeseries-0.7.1b20230506/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import re
 import time
 from typing import Any, Dict, List, Optional, Union
 
-import autogluon.core as ag
+from autogluon.common import space
 from autogluon.common.loaders import load_pkl
 from autogluon.common.savers import save_pkl
 from autogluon.core.hpo.exceptions import EmptySearchSpace
 from autogluon.core.hpo.executors import HpoExecutor
 from autogluon.core.models import AbstractModel
 from autogluon.timeseries.dataset import TimeSeriesDataFrame
 from autogluon.timeseries.evaluator import TimeSeriesEvaluator
@@ -80,15 +80,15 @@
         freq: Optional[str] = None,
         prediction_length: int = 1,
         path: Optional[str] = None,
         name: Optional[str] = None,
         metadata: Optional[CovariateMetadata] = None,
         eval_metric: Optional[str] = None,
         eval_metric_seasonal_period: Optional[int] = None,
-        hyperparameters: Dict[str, Union[int, float, str, ag.Space]] = None,
+        hyperparameters: Dict[str, Union[int, float, str, space.Space]] = None,
         **kwargs,
     ):
         name = name or re.sub(r"Model$", "", self.__class__.__name__)
         super().__init__(
             path=path,
             name=name,
             problem_type=None,
@@ -249,15 +249,15 @@
         track of the time limit, etc.
         """
         # TODO: Make the models respect `num_cpus` and `num_gpus` parameters
         raise NotImplementedError
 
     def _check_fit_params(self):
         # gracefully handle hyperparameter specifications if they are provided to fit instead
-        if any(isinstance(v, ag.Space) for v in self.params.values()):
+        if any(isinstance(v, space.Space) for v in self.params.values()):
             raise ValueError(
                 "Hyperparameter spaces provided to `fit`. Please provide concrete values "
                 "as hyperparameters when initializing or use `hyperparameter_tune` instead."
             )
 
     def _check_predict_inputs(
         self,
```

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/models/presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import logging
 import re
 from typing import Any, Dict, List, Optional, Type, Union
 
-import autogluon.core as ag
 import autogluon.timeseries as agts
+from autogluon.common import space
+from autogluon.core import constants
 
 from . import (
     ARIMAModel,
     AutoARIMAModel,
     AutoETSModel,
     AutoGluonTabularModel,
     DeepARModel,
@@ -133,19 +134,19 @@
             "ETS": {},
             "AutoETS": {},
             "AutoARIMA": {},
             "DynamicOptimizedTheta": {},
             "Theta": {},
             "AutoGluonTabular": {},
             "DeepAR": {
-                "num_layers": ag.Int(1, 3, default=2),
-                "hidden_size": ag.Int(40, 80, default=40),
+                "num_layers": space.Int(1, 3, default=2),
+                "hidden_size": space.Int(40, 80, default=40),
             },
             "SimpleFeedForward": {
-                "hidden_dimensions": ag.Categorical([40], [40, 40], [120]),
+                "hidden_dimensions": space.Categorical([40], [40, 40], [120]),
             },
             "TemporalFusionTransformer": {},
         },
     }
 
     # update with MXNet if installed
     if agts.MXNET_INSTALLED:
@@ -219,15 +220,15 @@
             model_type = model
 
         model_hps_list = hyperparameters[model]
         if not isinstance(model_hps_list, list):
             model_hps_list = [model_hps_list]
 
         for model_hps in model_hps_list:
-            ag_args = model_hps.pop(ag.constants.AG_ARGS, {})
+            ag_args = model_hps.pop(constants.AG_ARGS, {})
             for key in ag_args:
                 if key not in VALID_AG_ARGS_KEYS:
                     raise ValueError(
                         f"Model {model_type} received unknown ag_args key: {key} (valid keys {VALID_AG_ARGS_KEYS})"
                     )
             model_name_base = get_model_name(ag_args, model_type)
 
@@ -268,15 +269,15 @@
         name_suffix = ag_args.get("name_suffix", "")
         name = name_prefix + name_stem + name_suffix
     return name
 
 
 def contains_searchspace(model_hyperparameters: Dict[str, Any]) -> bool:
     for hp_value in model_hyperparameters.values():
-        if isinstance(hp_value, ag.space.Space):
+        if isinstance(hp_value, space.Space):
             return True
     return False
 
 
 def verify_contains_at_least_one_searchspace(hyperparameters: Dict[str, Dict[str, Any]]):
     for model, model_hps_list in hyperparameters.items():
         if not isinstance(model_hps_list, list):
```

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,22 +401,22 @@
 
             Full list of available models and their hyperparameters is provided in :ref:`forecasting_zoo`.
 
             The hyperparameters for each model can be fixed values (as shown above), or search spaces over which
             hyperparameter optimization is performed. A search space should only be provided when
             ``hyperparameter_tune_kwargs`` is given (i.e., hyperparameter-tuning is utilized). For example::
 
-                import autogluon.core as ag
+                from autogluon.common import space
 
                 predictor.fit(
                     ...
                     hyperparameters={
                         "DeepAR": {
-                            "hidden_size": ag.space.Int(20, 100),
-                            "dropout_rate": ag.space.Categorical(0.1, 0.3),
+                            "hidden_size": space.Int(20, 100),
+                            "dropout_rate": space.Categorical(0.1, 0.3),
                         },
                     },
                     hyperparameter_tune_kwargs="auto",
                 )
 
             In the above example, multiple versions of the DeepAR model with different values of the parameters
             "hidden_size" and "dropout_rate" will be trained.
```

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230506/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230505
+Version: 0.7.1b20230506
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230506/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

