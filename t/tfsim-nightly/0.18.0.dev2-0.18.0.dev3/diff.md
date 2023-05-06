# Comparing `tmp/tfsim-nightly-0.18.0.dev2.tar.gz` & `tmp/tfsim-nightly-0.18.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfsim-nightly-0.18.0.dev2.tar", last modified: Fri Mar 31 03:11:38 2023, max compression
+gzip compressed data, was "tfsim-nightly-0.18.0.dev3.tar", last modified: Sat May  6 03:11:33 2023, max compression
```

## Comparing `tfsim-nightly-0.18.0.dev2.tar` & `tfsim-nightly-0.18.0.dev3.tar`

### file list

```diff
@@ -1,193 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.420971 tfsim-nightly-0.18.0.dev2/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-03-31 03:09:54.000000 tfsim-nightly-0.18.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-03-31 03:11:38.420971 tfsim-nightly-0.18.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-03-31 03:09:54.000000 tfsim-nightly-0.18.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 03:11:38.420971 tfsim-nightly-0.18.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.408971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-03-31 03:11:37.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.408971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.408971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.408971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.408971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/cropping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/barlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/base_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.408971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/binary_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/classification_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/false_positive_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/negative_predictive_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/distances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.408971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/evaluators/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/evaluators/memory_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.412971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/barlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/circle_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/metric_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/multinegrank_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/multisim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/pn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/softnn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/vicreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/xbm_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.412971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/classification_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/match_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/match_nearest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.412971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39080 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/models/contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    32242 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/models/similarity_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.412971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/bndcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/map_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/precision_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/retrieval_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.412971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/file_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/memory_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/tfdataset_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/tfrecords_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.412971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/faiss_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/linear_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/nmslib_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.412971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/cached_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.412971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/training_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/training_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/training_metrics/distance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/training_metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/confusion_matrix_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/neighbors_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/vizualize_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/architectures/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/architectures/test_resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/architectures/test_resnet50.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/classification_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/classification_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/classification_metrics/test_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/evaluators/test_memory_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/losses/test_pn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/losses/test_softnn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/losses/test_triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/losses/test_xbm_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/matchers/test_classification_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/matchers/test_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/matchers/test_match_nearest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/models/test_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/models/test_similarity_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_bndcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_map_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_precision_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_retrieval_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/samplers/test_file_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/samplers/test_memory_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/samplers/test_tfdataset_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/samplers/test_tfrecord_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.416971 tfsim-nightly-0.18.0.dev2/tests/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/search/test_faiss_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/search/test_linear_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/search/test_nmslib_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.420971 tfsim-nightly-0.18.0.dev2/tests/stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/stores/test_cached_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/stores/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/stores/test_redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/test_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/test_schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.420971 tfsim-nightly-0.18.0.dev2/tests/training_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/training_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/training_metrics/test_distance_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.420971 tfsim-nightly-0.18.0.dev2/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/visualization/test_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-03-31 03:09:55.000000 tfsim-nightly-0.18.0.dev2/tests/visualization/test_neighbors_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:11:38.420971 tfsim-nightly-0.18.0.dev2/tfsim_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-03-31 03:11:38.000000 tfsim-nightly-0.18.0.dev2/tfsim_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-03-31 03:11:38.000000 tfsim-nightly-0.18.0.dev2/tfsim_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 03:11:38.000000 tfsim-nightly-0.18.0.dev2/tfsim_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-31 03:11:38.000000 tfsim-nightly-0.18.0.dev2/tfsim_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 03:11:38.000000 tfsim-nightly-0.18.0.dev2/tfsim_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.264979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-06 03:11:31.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.264979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.264979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.264979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.264979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/cropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/barlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16121 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/base_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.264979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/binary_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/classification_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/false_positive_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/negative_predictive_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.264979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/evaluators/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/evaluators/memory_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.268979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/barlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/circle_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/metric_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/multinegrank_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/multisim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/pn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/softnn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/vicreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/xbm_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.268979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/classification_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/match_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/match_nearest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.268979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39080 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/models/contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/models/similarity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.268979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/bndcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/map_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/precision_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.268979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/file_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/memory_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/tfdata_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/tfdataset_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/tfrecords_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.268979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/faiss_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/linear_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/nmslib_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/cached_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/training_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/training_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/training_metrics/distance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/training_metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/confusion_matrix_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/neighbors_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/vizualize_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tests/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/architectures/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/architectures/test_resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/architectures/test_resnet50.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tests/classification_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/classification_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/classification_metrics/test_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tests/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/evaluators/test_memory_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tests/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/losses/test_pn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/losses/test_softnn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/losses/test_triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/losses/test_xbm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.272979 tfsim-nightly-0.18.0.dev3/tests/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/matchers/test_classification_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/matchers/test_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/matchers/test_match_nearest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/models/test_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/models/test_similarity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_bndcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_map_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_precision_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_retrieval_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/tests/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/samplers/test_file_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/samplers/test_memory_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/samplers/test_tfdata_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/samplers/test_tfdataset_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/samplers/test_tfrecord_samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/search/test_faiss_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/search/test_linear_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/search/test_nmslib_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/tests/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/stores/test_cached_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/stores/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/stores/test_redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/test_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/test_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/tests/training_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/training_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/training_metrics/test_distance_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/visualization/test_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-06 03:09:43.000000 tfsim-nightly-0.18.0.dev3/tests/visualization/test_neighbors_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:11:33.276979 tfsim-nightly-0.18.0.dev3/tfsim_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-06 03:11:33.000000 tfsim-nightly-0.18.0.dev3/tfsim_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-06 03:11:33.000000 tfsim-nightly-0.18.0.dev3/tfsim_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:11:33.000000 tfsim-nightly-0.18.0.dev3/tfsim_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-06 03:11:33.000000 tfsim-nightly-0.18.0.dev3/tfsim_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 03:11:33.000000 tfsim-nightly-0.18.0.dev3/tfsim_nightly.egg-info/top_level.txt
```

### Comparing `tfsim-nightly-0.18.0.dev2/LICENSE` & `tfsim-nightly-0.18.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/PKG-INFO` & `tfsim-nightly-0.18.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfsim-nightly
-Version: 0.18.0.dev2
+Version: 0.18.0.dev3
 Summary: Metric Learning for Humans
 Home-page: https://github.com/tensorflow/similarity
 Author: Tensorflow Similarity authors
 Author-email: tf-similarity@google.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tfsim-nightly-0.18.0.dev2/README.md` & `tfsim-nightly-0.18.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/setup.py` & `tfsim-nightly-0.18.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.18.0.dev2"
+__version__ = "0.18.0.dev3"
 
 
 from . import algebra  # noqa
 from . import architectures  # noqa
 from . import augmenters  # noqa
 from . import callbacks  # noqa
 from . import classification_metrics  # noqa
```

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/algebra.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/algebra.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/api/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/efficientnet.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/efficientnet.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/resnet18.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/resnet18.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/resnet50.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/resnet50.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/architectures/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/architectures/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/blur.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/blur.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/cropping.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/cropping.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/flip.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/flip.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmentation_utils/solarize.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmentation_utils/solarize.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/augmenter.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/augmenter.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/barlow.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/barlow.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/contrastive.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/contrastive.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/augmenters/simclr.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/augmenters/simclr.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/base_indexer.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/base_indexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from collections.abc import Mapping, MutableMapping, Sequence
-from typing import Optional, Union
 
 import numpy as np
 import tensorflow as tf
 from tabulate import tabulate
 from tqdm.auto import tqdm
 
 from .classification_metrics import (
@@ -22,18 +21,18 @@
 from .types import CalibrationResults, FloatTensor, Lookup, Tensor
 from .utils import unpack_lookup_distances, unpack_lookup_labels
 
 
 class BaseIndexer(ABC):
     def __init__(
         self,
-        distance: Union[Distance, str],
-        embedding_output: Optional[int],
+        distance: Distance | str,
+        embedding_output: int | None,
         embedding_size: int,
-        evaluator: Union[Evaluator, str],
+        evaluator: Evaluator | str,
         stat_buffer_size: int,
     ) -> None:
         distance = distance_canonicalizer(distance)
         self.distance = distance  # needed for save()/load()
         self.embedding_output = embedding_output
         self.embedding_size = embedding_size
 
@@ -280,15 +279,15 @@
         self.calibration_thresholds = calibration_results.thresholds
         return calibration_results
 
     def match(
         self,
         predictions: FloatTensor,
         no_match_label: int = -1,
-        k=1,
+        k: int = 1,
         matcher: str | ClassificationMatch = "match_nearest",
         verbose: int = 1,
     ) -> dict[str, list[int]]:
         """Match embeddings against the various cutpoints thresholds
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
```

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/callbacks.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/callbacks.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/binary_accuracy.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/binary_accuracy.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/classification_metric.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/classification_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/f1_score.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/f1_score.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/false_positive_rate.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/false_positive_rate.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/negative_predictive_value.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/precision.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/precision.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/recall.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/recall.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/classification_metrics/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/classification_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/distances.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/distances.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/evaluators/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/evaluators/evaluator.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/evaluators/evaluator.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/evaluators/memory_evaluator.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/evaluators/memory_evaluator.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/indexer.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/indexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 """Index the embeddings infered by the model to allow distance based
 sub-linear search"""
 from __future__ import annotations
 
 import json
 import os
 from collections import defaultdict, deque
+from collections.abc import Sequence
 from pathlib import Path
 from time import time
-from typing import DefaultDict, Deque, List, Optional, Sequence, Union
 
 import numpy as np
 import tensorflow as tf
 from tabulate import tabulate
 from tqdm.auto import tqdm
 
 from .base_indexer import BaseIndexer
@@ -58,19 +58,19 @@
     LABELS = 2
     DATA = 3
     RANKS = 4
 
     def __init__(
         self,
         embedding_size: int,
-        distance: Union[Distance, str] = "cosine",
-        search: Union[Search, str] = "nmslib",
-        kv_store: Union[Store, str] = "memory",
-        evaluator: Union[Evaluator, str] = "memory",
-        embedding_output: Optional[int] = None,
+        distance: Distance | str = "cosine",
+        search: Search | str = "nmslib",
+        kv_store: Store | str = "memory",
+        evaluator: Evaluator | str = "memory",
+        embedding_output: int | None = None,
         stat_buffer_size: int = 1000,
     ) -> None:
         """Index embeddings to make them searchable via KNN
 
         Args:
             embedding_size: Size of the embeddings that will be stored.
             It is usually equivalent to the size of the output layer.
@@ -143,16 +143,16 @@
         self.kv_store.reset()
         self._init_structures()
 
     def _init_structures(self) -> None:
         "(re)initialize internal stats structure"
 
         # stats
-        self._stats: DefaultDict[str, int] = defaultdict(int)
-        self._lookup_timings_buffer: Deque[float] = deque([], maxlen=self.stat_buffer_size)
+        self._stats: defaultdict[str, int] = defaultdict(int)
+        self._lookup_timings_buffer: deque[float] = deque([], maxlen=self.stat_buffer_size)
 
         # calibration data
         self.is_calibrated = False
         self.calibration_metric = F1Score()
         self.cutpoints = {}
         self.calibration_thresholds = {}
 
@@ -192,26 +192,26 @@
         if isinstance(self.embedding_output, int):
             embeddings: FloatTensor = predictions[self.embedding_output]
         else:
             # needed for typing
             embeddings = predictions
         return embeddings
 
-    def _cast_label(self, label: Optional[int]) -> Optional[int]:
+    def _cast_label(self, label: int | None) -> int | None:
         if label is not None:
             label = int(label)
         return label
 
     def build_index(self, samples, **kwargss):
         self.search.build_index(samples)
 
     def add(
         self,
         prediction: FloatTensor,
-        label: Optional[int] = None,
+        label: int | None = None,
         data: Tensor = None,
         build: bool = True,
         verbose: int = 1,
     ):
         """Add a single embedding to the indexer
 
         Args:
@@ -240,16 +240,16 @@
 
         # add index to the embedding
         self.search.add(embedding, idx, build=build, verbose=verbose)
 
     def batch_add(
         self,
         predictions: FloatTensor,
-        labels: Optional[Sequence[int]] = None,
-        data: Optional[Tensor] = None,
+        labels: Sequence[int] | None = None,
+        data: Tensor | None = None,
         build: bool = True,
         verbose: int = 1,
     ):
         """Add a batch of embeddings to the indexer
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
@@ -271,15 +271,15 @@
 
         # store points
         if verbose:
             print("|-Storing data points in key value store")
         idxs = self.kv_store.batch_add(embeddings, labels, data)
         self.search.batch_add(embeddings, idxs, build=build, verbose=verbose)
 
-    def single_lookup(self, prediction: FloatTensor, k: int = 5) -> List[Lookup]:
+    def single_lookup(self, prediction: FloatTensor, k: int = 5) -> list[Lookup]:
         """Find the k closest matches of a given embedding
 
         Args:
             prediction: TF similarity model prediction, may be a multi-headed
             output.
 
             k: Number of nearest neighbors to lookup. Defaults to 5.
@@ -306,16 +306,15 @@
                     data=data[i],
                 )
             )
         self._lookup_timings_buffer.append(lookup_time)
         self._stats["num_lookups"] += 1
         return lookups
 
-    def batch_lookup(self, predictions: FloatTensor, k: int = 5, verbose: int = 1) -> List[List[Lookup]]:
-
+    def batch_lookup(self, predictions: FloatTensor, k: int = 5, verbose: int = 1) -> list[list[Lookup]]:
         """Find the k closest matches for a set of embeddings
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
             output.
 
             k: Number of nearest neighbors to lookup. Defaults to 5.
```

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/layers.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/layers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/barlow.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/barlow.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/circle_loss.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/circle_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/metric_loss.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/metric_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/multinegrank_loss.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/multinegrank_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/multisim_loss.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/multisim_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/pn_loss.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/pn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/simclr.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/simclr.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/simsiam.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/simsiam.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/softnn_loss.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/softnn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/triplet_loss.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/vicreg.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/vicreg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/losses/xbm_loss.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/losses/xbm_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/classification_match.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/classification_match.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/match_majority_vote.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/match_majority_vote.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/match_nearest.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/match_nearest.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/matchers/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/matchers/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/models/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/models/contrastive_model.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/models/contrastive_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/models/similarity_model.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/models/similarity_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,25 +194,25 @@
 
         Raises:
             ValueError: In case of invalid arguments for
                 `optimizer`, `loss` or `metrics`.
         """
         # Fetching the distance used from the first loss if auto
         if distance == "auto":
-            if isinstance(loss, list):
-                metric_loss = loss[0]
+            if loss is None:
+                distance = distance_canonicalizer("cosine")
             else:
-                metric_loss = loss
+                metric_loss = loss[0] if isinstance(loss, list) else loss
 
-            try:
-                distance = metric_loss.distance
-            except AttributeError:
-                msg = "distance='auto' only works if the first loss is a " "metric loss"
+                try:
+                    distance = metric_loss.distance
+                except AttributeError:
+                    msg = "distance='auto' only works if the first loss is a " "metric loss"
+                    raise ValueError(msg)
 
-                raise ValueError(msg)
             print(f"Distance metric automatically set to {distance} use the " "distance arg to override.")
         else:
             distance = distance_canonicalizer(distance)
 
         # init index
         self.create_index(
             distance=distance,
@@ -261,15 +261,15 @@
 
     @_index.setter
     def _index(self, index: Indexer) -> None:
         self._ix = index
 
     def create_index(
         self,
-        distance: Distance | str = "auto",
+        distance: Distance | str = "cosine",
         search: Search | str = "nmslib",
         kv_store: Store | str = "memory",
         evaluator: Evaluator | str = "memory",
         embedding_output: int | None = None,
         stat_buffer_size: int = 1000,
     ) -> None:
         """Create the model index to make embeddings searchable via KNN.
@@ -356,18 +356,16 @@
             when calling indexing repeatidly without the need to search between
             the indexing requests. Defaults to True.
 
             verbose: Output indexing progress info. Defaults to 1.
         """
 
         if verbose:
-            print("[Indexing {tf.shape(x)} points]")
+            print(f"[Indexing {len(x)} points]")
             print("|-Computing embeddings")
-        with tf.device("/cpu:0"):
-            x = tf.convert_to_tensor(np.array(x))
 
         predictions = self.predict(x)
 
         self._index.batch_add(
             predictions=predictions,
             labels=y,
             data=data,
@@ -426,16 +424,14 @@
 
             verbose: display progress. Default to 1.
 
         Returns
             list of list of k nearest neighboors:
             list[list[Lookup]]
         """
-        with tf.device("/cpu:0"):
-            x = tf.convert_to_tensor(np.array(x))
         predictions = self.predict(x)
 
         return self._index.batch_lookup(predictions=predictions, k=k, verbose=verbose)
 
     def single_lookup(self, x: Tensor, k: int = 5) -> list[Lookup]:
         """Find the k closest matches in the index for a given sample.
 
@@ -512,16 +508,14 @@
         Returns:
             CalibrationResults containing the thresholds and cutpoints Dicts.
         """
         if thresholds_targets is None:
             thresholds_targets = {}
 
         # predict
-        with tf.device("/cpu:0"):
-            x = tf.convert_to_tensor(np.array(x))
         predictions = self.predict(x)
 
         # calibrate
         return self._index.calibrate(
             predictions=predictions,
             target_labels=y,
             thresholds_targets=thresholds_targets,
@@ -578,16 +572,14 @@
 
         """
         # basic checks
         if not self._index.is_calibrated:
             raise ValueError("Uncalibrated model: run model.calibration()")
 
         # get predictions
-        with tf.device("/cpu:0"):
-            x = tf.convert_to_tensor(np.array(x))
         predictions = self.predict(x)
 
         # matching
         matches = self._index.match(
             predictions,
             no_match_label=no_match_label,
             k=k,
@@ -630,16 +622,14 @@
         """
         if self._index.size() == 0:
             raise IndexError("Index must contain embeddings but is " "currently empty. Have you run model.index()?")
 
         # get embeddings
         if verbose:
             print("|-Computing embeddings")
-        with tf.device("/cpu:0"):
-            x = tf.convert_to_tensor(np.array(x))
         predictions = self.predict(x)
 
         if verbose:
             print("|-Computing retrieval metrics")
 
         results = self._index.evaluate_retrieval(
             predictions=predictions,
@@ -709,16 +699,14 @@
             raise ValueError("Uncalibrated model: run model.calibration()")
 
         cal_metric = self._index.get_calibration_metric()
 
         # get embeddings
         if verbose:
             print("|-Computing embeddings")
-        with tf.device("/cpu:0"):
-            x = tf.convert_to_tensor(np.array(x))
         predictions = self.predict(x)
 
         results: defaultdict[str, dict[str, str | np.ndarray]] = defaultdict(dict)
 
         if verbose:
             pb = tqdm(total=len(self._index.cutpoints), desc="Evaluating cutpoints")
```

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/bndcg.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/bndcg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/map_at_k.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/map_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/precision_at_k.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/precision_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/recall_at_k.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/recall_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/retrieval_metric.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/retrieval_metrics/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/retrieval_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/file_samplers.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/file_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/memory_samplers.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/memory_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/samplers.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/tfdataset_samplers.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/tfdataset_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/tfrecords_samplers.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/tfrecords_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/samplers/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/schedules.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/schedules.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,11 +34,11 @@
 """
 import logging
 
 # Disable the INFO logging from NMSLIB
 logging.getLogger("nmslib").setLevel(logging.WARNING)
 
 from .faiss_search import FaissSearch  # noqa
-from .linear_search import LinearSearch
+from .linear_search import LinearSearch  # noqa
 from .nmslib_search import NMSLibSearch  # noqa
 from .search import Search  # noqa
 from .utils import make_search  # noqa
```

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/faiss_search.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/faiss_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/linear_search.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/linear_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/nmslib_search.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/nmslib_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/search.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/search/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/search/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/cached_store.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/cached_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/memory_store.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/memory_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/redis_store.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/redis_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/store.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/stores/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/stores/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/training_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/training_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/training_metrics/distance_metrics.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/training_metrics/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/training_metrics/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/training_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/types.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/types.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/utils.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/__init__.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/confusion_matrix_viz.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/confusion_matrix_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/neighbors_viz.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/neighbors_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/projector.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/projector.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tensorflow_similarity/visualization/vizualize_views.py` & `tfsim-nightly-0.18.0.dev3/tensorflow_similarity/visualization/vizualize_views.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/architectures/test_efficientnet.py` & `tfsim-nightly-0.18.0.dev3/tests/architectures/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/architectures/test_resnet18.py` & `tfsim-nightly-0.18.0.dev3/tests/architectures/test_resnet18.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/architectures/test_resnet50.py` & `tfsim-nightly-0.18.0.dev3/tests/architectures/test_resnet50.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/classification_metrics/test_classification_metrics.py` & `tfsim-nightly-0.18.0.dev3/tests/classification_metrics/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/evaluators/test_memory_evaluator.py` & `tfsim-nightly-0.18.0.dev3/tests/evaluators/test_memory_evaluator.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/losses/test_pn_loss.py` & `tfsim-nightly-0.18.0.dev3/tests/losses/test_pn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/losses/test_softnn_loss.py` & `tfsim-nightly-0.18.0.dev3/tests/losses/test_softnn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/losses/test_triplet_loss.py` & `tfsim-nightly-0.18.0.dev3/tests/losses/test_triplet_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/losses/test_xbm_loss.py` & `tfsim-nightly-0.18.0.dev3/tests/losses/test_xbm_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/losses/utils.py` & `tfsim-nightly-0.18.0.dev3/tests/losses/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/matchers/test_classification_match.py` & `tfsim-nightly-0.18.0.dev3/tests/matchers/test_classification_match.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/matchers/test_majority_vote.py` & `tfsim-nightly-0.18.0.dev3/tests/matchers/test_majority_vote.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/matchers/test_match_nearest.py` & `tfsim-nightly-0.18.0.dev3/tests/matchers/test_match_nearest.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/models/test_contrastive_model.py` & `tfsim-nightly-0.18.0.dev3/tests/models/test_contrastive_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/models/test_similarity_model.py` & `tfsim-nightly-0.18.0.dev3/tests/models/test_similarity_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_bndcg.py` & `tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_bndcg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_map_at_k.py` & `tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_map_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_precision_at_k.py` & `tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_precision_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_recall_at_k.py` & `tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_recall_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/retrieval_metrics/test_retrieval_metric.py` & `tfsim-nightly-0.18.0.dev3/tests/retrieval_metrics/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/samplers/test_file_samplers.py` & `tfsim-nightly-0.18.0.dev3/tests/samplers/test_file_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/samplers/test_memory_samplers.py` & `tfsim-nightly-0.18.0.dev3/tests/samplers/test_memory_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/samplers/test_tfdataset_samplers.py` & `tfsim-nightly-0.18.0.dev3/tests/samplers/test_tfdataset_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/samplers/test_tfrecord_samplers.py` & `tfsim-nightly-0.18.0.dev3/tests/samplers/test_tfrecord_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/search/test_faiss_search.py` & `tfsim-nightly-0.18.0.dev3/tests/search/test_faiss_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/search/test_linear_search.py` & `tfsim-nightly-0.18.0.dev3/tests/search/test_linear_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/search/test_nmslib_search.py` & `tfsim-nightly-0.18.0.dev3/tests/search/test_nmslib_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/stores/test_cached_store.py` & `tfsim-nightly-0.18.0.dev3/tests/stores/test_cached_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/stores/test_memory_store.py` & `tfsim-nightly-0.18.0.dev3/tests/stores/test_memory_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/stores/test_redis_store.py` & `tfsim-nightly-0.18.0.dev3/tests/stores/test_redis_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/test_algebra.py` & `tfsim-nightly-0.18.0.dev3/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/test_callbacks.py` & `tfsim-nightly-0.18.0.dev3/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/test_distances.py` & `tfsim-nightly-0.18.0.dev3/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/test_indexer.py` & `tfsim-nightly-0.18.0.dev3/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/test_layers.py` & `tfsim-nightly-0.18.0.dev3/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/test_schedules.py` & `tfsim-nightly-0.18.0.dev3/tests/test_schedules.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/test_types.py` & `tfsim-nightly-0.18.0.dev3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/test_utils.py` & `tfsim-nightly-0.18.0.dev3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/training_metrics/test_distance_metrics.py` & `tfsim-nightly-0.18.0.dev3/tests/training_metrics/test_distance_metrics.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/visualization/test_confusion_matrix.py` & `tfsim-nightly-0.18.0.dev3/tests/visualization/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tests/visualization/test_neighbors_viz.py` & `tfsim-nightly-0.18.0.dev3/tests/visualization/test_neighbors_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev2/tfsim_nightly.egg-info/PKG-INFO` & `tfsim-nightly-0.18.0.dev3/tfsim_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfsim-nightly
-Version: 0.18.0.dev2
+Version: 0.18.0.dev3
 Summary: Metric Learning for Humans
 Home-page: https://github.com/tensorflow/similarity
 Author: Tensorflow Similarity authors
 Author-email: tf-similarity@google.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tfsim-nightly-0.18.0.dev2/tfsim_nightly.egg-info/SOURCES.txt` & `tfsim-nightly-0.18.0.dev3/tfsim_nightly.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 tensorflow_similarity/retrieval_metrics/recall_at_k.py
 tensorflow_similarity/retrieval_metrics/retrieval_metric.py
 tensorflow_similarity/retrieval_metrics/utils.py
 tensorflow_similarity/samplers/__init__.py
 tensorflow_similarity/samplers/file_samplers.py
 tensorflow_similarity/samplers/memory_samplers.py
 tensorflow_similarity/samplers/samplers.py
+tensorflow_similarity/samplers/tfdata_sampler.py
 tensorflow_similarity/samplers/tfdataset_samplers.py
 tensorflow_similarity/samplers/tfrecords_samplers.py
 tensorflow_similarity/samplers/utils.py
 tensorflow_similarity/search/__init__.py
 tensorflow_similarity/search/faiss_search.py
 tensorflow_similarity/search/linear_search.py
 tensorflow_similarity/search/nmslib_search.py
@@ -134,14 +135,15 @@
 tests/retrieval_metrics/test_map_at_k.py
 tests/retrieval_metrics/test_precision_at_k.py
 tests/retrieval_metrics/test_recall_at_k.py
 tests/retrieval_metrics/test_retrieval_metric.py
 tests/samplers/__init__.py
 tests/samplers/test_file_samplers.py
 tests/samplers/test_memory_samplers.py
+tests/samplers/test_tfdata_sampler.py
 tests/samplers/test_tfdataset_samplers.py
 tests/samplers/test_tfrecord_samplers.py
 tests/search/__init__.py
 tests/search/test_faiss_search.py
 tests/search/test_linear_search.py
 tests/search/test_nmslib_search.py
 tests/stores/__init__.py
```

