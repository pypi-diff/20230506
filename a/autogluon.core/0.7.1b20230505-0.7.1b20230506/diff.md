# Comparing `tmp/autogluon.core-0.7.1b20230505.tar.gz` & `tmp/autogluon.core-0.7.1b20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.7.1b20230505.tar", last modified: Fri May  5 09:04:09 2023, max compression
+gzip compressed data, was "autogluon.core-0.7.1b20230506.tar", last modified: Sat May  6 09:03:34 2023, max compression
```

## Comparing `autogluon.core-0.7.1b20230505.tar` & `autogluon.core-0.7.1b20230506.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.763787 autogluon.core-0.7.1b20230505/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-05 09:04:09.763787 autogluon.core-0.7.1b20230505/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:04:09.763787 autogluon.core-0.7.1b20230505/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.743787 autogluon.core-0.7.1b20230505/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.747787 autogluon.core-0.7.1b20230505/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.751787 autogluon.core-0.7.1b20230505/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.751787 autogluon.core-0.7.1b20230505/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.751787 autogluon.core-0.7.1b20230505/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.751787 autogluon.core-0.7.1b20230505/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.751787 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29490 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.751787 autogluon.core-0.7.1b20230505/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.755787 autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.755787 autogluon.core-0.7.1b20230505/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.755787 autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    94028 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.755787 autogluon.core-0.7.1b20230505/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.755787 autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59425 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.755787 autogluon.core-0.7.1b20230505/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.755787 autogluon.core-0.7.1b20230505/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.759787 autogluon.core-0.7.1b20230505/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.759787 autogluon.core-0.7.1b20230505/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.759787 autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.759787 autogluon.core-0.7.1b20230505/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.759787 autogluon.core-0.7.1b20230505/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.759787 autogluon.core-0.7.1b20230505/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169588 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.763787 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.763787 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.763787 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-05 09:03:33.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 09:04:09.000000 autogluon.core-0.7.1b20230505/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:09.747787 autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-05 09:04:09.000000 autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-05 09:04:09.000000 autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:04:09.000000 autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:04:09.000000 autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-05 09:04:09.000000 autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:04:09.000000 autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:04:09.000000 autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.149172 autogluon.core-0.7.1b20230506/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.153172 autogluon.core-0.7.1b20230506/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.153172 autogluon.core-0.7.1b20230506/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.153172 autogluon.core-0.7.1b20230506/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.153172 autogluon.core-0.7.1b20230506/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.153172 autogluon.core-0.7.1b20230506/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.153172 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94023 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59425 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.157172 autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169588 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.161171 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-06 09:03:19.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 09:03:34.000000 autogluon.core-0.7.1b20230506/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:03:34.153172 autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-06 09:03:34.000000 autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-06 09:03:34.000000 autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:03:34.000000 autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 09:03:34.000000 autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-06 09:03:34.000000 autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 09:03:34.000000 autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:03:34.000000 autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.7.1b20230505/PKG-INFO` & `autogluon.core-0.7.1b20230506/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
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

### Comparing `autogluon.core-0.7.1b20230505/setup.py` & `autogluon.core-0.7.1b20230506/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/constants.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/dataset.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/executors.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import copy
 import logging
 import math
 import os
 import pandas as pd
 import time
 
+from autogluon.common import space
+
 from abc import ABC, abstractmethod
 from typing import Any, Optional, List, Dict, Union, Callable, Tuple
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.s3_utils import is_s3_url
 
 from .constants import RAY_BACKEND, CUSTOM_BACKEND
 from .exceptions import EmptySearchSpace
-from .. import Space
 from ..ray.resources_calculator import ResourceCalculator
 from ..scheduler.scheduler_factory import scheduler_factory
 from ..utils.savers import save_pkl
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -370,22 +371,22 @@
         )
         if 'num_trials' not in hyperparameter_tune_kwargs and default_num_trials is not None:
             hyperparameter_tune_kwargs['num_trials'] = default_num_trials
         self.hyperparameter_tune_kwargs = copy.deepcopy(hyperparameter_tune_kwargs)
         
     def validate_search_space(self, search_space, model_name):
         from ray.tune.search.sample import Domain
-        if not any(isinstance(search_space[hyperparam], (Space, Domain)) for hyperparam in search_space):
+        if not any(isinstance(search_space[hyperparam], (space.Space, Domain)) for hyperparam in search_space):
             logger.warning(f"\tNo hyperparameter search space specified for {model_name}. Skipping HPO. "
                            f"Will train one model based on the provided hyperparameters.")
             raise EmptySearchSpace
         self.search_space = search_space
         logger.log(15, f"\tHyperparameter search space for {model_name}: ")
         for hyperparam in search_space:
-                if isinstance(search_space[hyperparam], (Space, Domain)):
+                if isinstance(search_space[hyperparam], (space.Space, Domain)):
                     logger.log(15, f"{hyperparam}:   {search_space[hyperparam]}")
                     
     def execute(
             self,
             *,  # Force kwargs to avoid bugs
             model_trial: Callable,
             train_fn_kwargs: dict,
@@ -524,22 +525,22 @@
         super().register_resources(initialized_model, **kwargs)
         if self.hyperparameter_tune_kwargs.get('resources_per_trial', None) is not None:
             # Custom backend only run trials sequentially
             self.scheduler_options[1]['resource'] = self.hyperparameter_tune_kwargs['resources_per_trial']
         logger.debug(f'custom backend resource: {self.resources}, per trial resource: {self.hyperparameter_tune_kwargs}')
         
     def validate_search_space(self, search_space, model_name):
-        if not any(isinstance(search_space[hyperparam], Space) for hyperparam in search_space):
+        if not any(isinstance(search_space[hyperparam], space.Space) for hyperparam in search_space):
             logger.warning(f"\tNo hyperparameter search space specified for {model_name}. Skipping HPO. "
                            f"Will train one model based on the provided hyperparameters.")
             raise EmptySearchSpace
         self.search_space = search_space
         logger.log(15, f"\tHyperparameter search space for {model_name}: ")
         for hyperparam in search_space:
-                if isinstance(search_space[hyperparam], Space):
+                if isinstance(search_space[hyperparam], space.Space):
                     logger.log(15, f"{hyperparam}:   {search_space[hyperparam]}")
                     
     def execute(self, model_trial, train_fn_kwargs, **kwargs):
         assert self.scheduler_options is not None, 'Call `initialize()` before execute'
         scheduler_cls, scheduler_params = self.scheduler_options  # Unpack tuple
         if scheduler_cls is None or scheduler_params is None:
             raise ValueError("scheduler_cls and scheduler_params cannot be None for hyperparameter tuning")
```

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_hpo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import os
 import shutil
 
+from autogluon.common import space as ag_space
+
 from autogluon.common.utils.distribute_utils import DistributedContext
 from autogluon.common.utils.try_import import try_import_ray
 try_import_ray()  # try import ray before importing the remaining contents so we can give proper error messages
 import ray
 
 from autogluon.common.utils.resource_utils import ResourceManager
 from abc import ABC, abstractmethod
@@ -19,15 +21,14 @@
     SEARCHER_PRESETS,
     SCHEDULER_PRESETS
 )
 from .exceptions import EmptySearchSpace
 from .ray_tune_scheduler_factory import SchedulerFactory
 from .ray_tune_searcher_factory import SearcherFactory
 from .space_converter import RaySpaceConverterFactory
-from .. import Space
 from ..ray.resources_calculator import ResourceCalculatorFactory, ResourceCalculator
 
 from ray import tune
 from ray import air
 from ray.tune import PlacementGroupFactory, ExperimentAnalysis
 from ray.tune.search.sample import Domain
 from ray.tune.schedulers import TrialScheduler
@@ -216,15 +217,15 @@
     assert mode in [MIN, MAX], f'mode {mode} is not a valid option. Options are {[MIN, MAX]}'
     if isinstance(hyperparameter_tune_kwargs, str):
         assert hyperparameter_tune_kwargs in ray_tune_adapter.presets, f'{hyperparameter_tune_kwargs} is not a valid option. Options are {ray_tune_adapter.presets.keys()}'
         hyperparameter_tune_kwargs = ray_tune_adapter.presets.get(hyperparameter_tune_kwargs)
     num_samples = hyperparameter_tune_kwargs.get('num_trials', None)
     if num_samples is None:
         num_samples = 1 if time_budget_s is None else 1000  # if both num_samples and time_budget_s are None, we only run 1 trial
-    if not any(isinstance(search_space[hyperparam], (Space, Domain)) for hyperparam in search_space):
+    if not any(isinstance(search_space[hyperparam], (ag_space.Space, Domain)) for hyperparam in search_space):
         raise EmptySearchSpace
     search_space, default_hyperparameters = _convert_search_space(search_space)
 
     searcher = _get_searcher(
         hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
         metric=metric,
         mode=mode,
@@ -353,15 +354,15 @@
 
 
 def _convert_search_space(search_space: dict):
     """Convert the search space to Ray Tune search space if it's AG search space"""
     tune_search_space = search_space.copy()
     default_hyperparameters = dict()
     for hyperparameters, space in search_space.items():
-        if isinstance(space, Space):
+        if isinstance(space, ag_space.Space):
             tune_search_space[hyperparameters] = RaySpaceConverterFactory.get_space_converter(space.__class__.__name__).convert(space)
             default_hyperparameters[hyperparameters] = space.default
     default_hyperparameters = default_hyperparameters
     if len(default_hyperparameters) == 0:
         # hyperopt + ray have trouble taking in empty default_hyperparameters
         default_hyperparameters = None
     else:
```

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/hpo/space_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from autogluon.common import space as ag_space
+
 from abc import ABC, abstractmethod
 from ray import tune
 
-from .. import Categorical, Real, Int, Bool
-
 
 class RaySpaceConverter(ABC):
     
     @property
     @abstractmethod
     def space_type(self):
         """Type of the converter"""
@@ -19,55 +19,55 @@
         raise NotImplementedError
         
         
 class RayCategoricalSpaceConverter(RaySpaceConverter):
     
     @property
     def space_type(self):
-        return Categorical.__name__
+        return ag_space.Categorical.__name__
     
     @staticmethod
     def convert(space):
-        assert isinstance(space, Categorical)
+        assert isinstance(space, ag_space.Categorical)
         return tune.choice(space.data)
     
 
 class RayRealSpaceConverter(RaySpaceConverter):
     
     @property
     def space_type(self):
-        return Real.__name__
+        return ag_space.Real.__name__
     
     @staticmethod
     def convert(space):
-        assert isinstance(space, Real)
+        assert isinstance(space, ag_space.Real)
         if space.log:
             ray_space = tune.loguniform(space.lower, space.upper)
         else:
             ray_space = tune.uniform(space.lower, space.upper)
         return ray_space
     
     
 class RayIntSpaceConverter(RaySpaceConverter):
     
     @property
     def space_type(self):
-        return Int.__name__
+        return ag_space.Int.__name__
     
     @staticmethod
     def convert(space):
-        assert isinstance(space, Int)
+        assert isinstance(space, ag_space.Int)
         return tune.randint(space.lower, space.upper+1)
     
 
 class RayBoolSpaceConverter(RayIntSpaceConverter):
     
     @property
     def space_type(self):
-        return Bool.__name__
+        return ag_space.Bool.__name__
 
 
 class RaySpaceConverterFactory:
     
     __supported_converters = [
         RayCategoricalSpaceConverter,
         RayRealSpaceConverter,
```

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/_utils.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from autogluon.common.utils.log_utils import DuplicateFilter
 from autogluon.common.utils.resource_utils import ResourceManager, RayResourceManager
 from autogluon.common.utils.resource_utils import get_resource_manager
 from autogluon.common.utils.distribute_utils import DistributedContext
 
 from .model_trial import model_trial, skip_hpo
 from ._tags import _DEFAULT_CLASS_TAGS, _DEFAULT_TAGS
-from ... import metrics, Space
+from ... import metrics
 from ...constants import AG_ARG_PREFIX, AG_ARGS_FIT, BINARY, REGRESSION, QUANTILE, REFIT_FULL_SUFFIX, OBJECTIVES_TO_NORMALIZE
 from ...data.label_cleaner import LabelCleaner, LabelCleanerMulticlassToBinary
 from ...hpo.exceptions import EmptySearchSpace
 from ...hpo.constants import RAY_BACKEND, CUSTOM_BACKEND
 from ...hpo.executors import HpoExecutor, HpoExecutorFactory
 from ...ray.resources_calculator import ResourceCalculator
 from ...scheduler import LocalSequentialScheduler
@@ -319,15 +319,15 @@
             params = self.params
         if param_name not in params:
             params[param_name] = param_value
 
     def _get_default_searchspace(self) -> dict:
         """
         Get the default hyperparameter searchspace of the model.
-        See `autogluon.core.space` for available space classes.
+        See `autogluon.common.space` for available space classes.
         Returns
         -------
         dict of hyperparameter search spaces.
         """
         return {}
 
     def _get_search_space(self):
```

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 from typing import Dict
 
 import numpy as np
 from sklearn.model_selection import ParameterGrid
 
+from autogluon.common import space as ag_space
+
 from .local_searcher import LocalSearcher
-from ..space import Categorical, Space, Int, Real
+
 
 __all__ = ['LocalGridSearcher']
 
 logger = logging.getLogger(__name__)
 
 
 class LocalGridSearcher(LocalSearcher):
@@ -34,23 +36,23 @@
         self._params_grid = ParameterGrid(self._params_space)
         self._grid_index = 0
         self._grid_length = len(self._params_grid)
 
     def _get_params_space(self) -> dict:
         param_space = dict()
         for key, val in self.search_space.items():
-            if isinstance(val, Space):
+            if isinstance(val, ag_space.Space):
                 samples_num = self._get_samples_number(key)
-                if isinstance(val, Int):
+                if isinstance(val, ag_space.Int):
                     samples = min(val.upper - val.lower + 1, samples_num)
                     param_space[key] = np.linspace(val.lower, val.upper, samples, dtype=int)
-                elif isinstance(val, Real):
+                elif isinstance(val, ag_space.Real):
                     space = np.geomspace if val.log else np.linspace
                     param_space[key] = space(val.lower, val.upper, num=samples_num)
-                elif isinstance(val, Categorical):
+                elif isinstance(val, ag_space.Categorical):
                     sk = val.convert_to_sklearn()
                     param_space[key] = sk
                 else:
                     raise AssertionError(f'Only Categorical is supported, but parameter "{key}" is type: {type(val)}')
 
         return param_space
```

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 
 import numpy as np
 from sklearn.model_selection import ParameterSampler
 
+from autogluon.common import space
+
 from .local_searcher import LocalSearcher
 from .exceptions import ExhaustedSearchSpaceError
-from ..space import DiscreteSpace, Space
+
 
 __all__ = ['LocalRandomSearcher']
 
 logger = logging.getLogger(__name__)
 
 
 class LocalRandomSearcher(LocalSearcher):
@@ -23,24 +25,24 @@
         self.random_state = np.random.RandomState(random_seed)
         self._params_space = self._get_params_space()
         self._num_configs = self._get_num_configs()
 
     def _get_params_space(self) -> dict:
         param_space = dict()
         for key, val in self.search_space.items():
-            if isinstance(val, Space):
+            if isinstance(val, space.Space):
                 sk = val.convert_to_sklearn()
                 param_space[key] = sk
         return param_space
 
     def _get_num_configs(self) -> int:
         num_unique = 1
         for key, val in self.search_space.items():
-            if isinstance(val, Space):
-                if isinstance(val, DiscreteSpace):
+            if isinstance(val, space.Space):
+                if isinstance(val, space.DiscreteSpace):
                     num_unique *= len(val)
                 else:
                     num_unique = None
                     break
         return num_unique
 
     def _sample_config(self) -> dict:
```

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/local_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import pickle
+
+from autogluon.common import space
+
 from collections import OrderedDict
 
-from ..space import Categorical, Space
 
 __all__ = ['LocalSearcher']
 
 logger = logging.getLogger(__name__)
 
 
 class LocalSearcher(object):
@@ -144,38 +146,38 @@
 
     def _get_params_static(self) -> dict:
         """
         Gets a dictionary of static key values, where no search space is used and therefore the values are always the same in all configs.
         """
         params_static = dict()
         for key, val in self.search_space.items():
-            if not isinstance(val, Space):
+            if not isinstance(val, space.Space):
                 params_static[key] = val
         return params_static
 
     def _get_params_default(self, params_static: dict) -> dict:
         """
         Gets the default config by calling `val.default` on every search space parameter, plus the static key values.
         """
         params_default = dict()
         for key, val in self.search_space.items():
-            if isinstance(val, Space):
+            if isinstance(val, space.Space):
                 params_default[key] = val.default
         params_default.update(params_static)
         return params_default
 
     def _get_params_cat_dict(self) -> dict:
         """
         Gets the dictionary of pickled category value -> index mapping for Category search spaces.
         This is used in `self._pickle_config` to map values to idx when pickling the config. This compresses the size of the pkl file.
         When being later unpickled via `self._unpickle_config`, the idx can be used to get the key value via `self.search_space[key][idx]`.
         """
         params_cat_dict = dict()
         for key, val in self.search_space.items():
-            if isinstance(val, Categorical):
+            if isinstance(val, space.Categorical):
                 cat_map = dict()
                 for i, cat in enumerate(val.data):
                     cat_pkl = pickle.dumps(cat)
                     cat_map[cat_pkl] = i
 
                 params_cat_dict[key] = cat_map
         return params_cat_dict
```

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/files.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/plots.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/time.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/utils.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.7.1b20230506/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
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

### Comparing `autogluon.core-0.7.1b20230505/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.7.1b20230506/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

