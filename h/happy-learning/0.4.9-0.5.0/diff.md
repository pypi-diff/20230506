# Comparing `tmp/happy_learning-0.4.9.tar.gz` & `tmp/happy_learning-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happy_learning-0.4.9.tar", last modified: Thu Apr 27 22:39:28 2023, max compression
+gzip compressed data, was "happy_learning-0.5.0.tar", last modified: Sat May  6 12:08:58 2023, max compression
```

## Comparing `happy_learning-0.4.9.tar` & `happy_learning-0.5.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-27 22:39:28.230883 happy_learning-0.4.9/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34966 2022-06-13 17:25:08.000000 happy_learning-0.4.9/LICENSE
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-27 22:39:28.231241 happy_learning-0.4.9/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     8494 2022-06-13 17:25:08.000000 happy_learning-0.4.9/README.md
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-27 22:39:28.121143 happy_learning-0.4.9/happy_learning/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/__init__.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4331 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/arbitrary_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2189 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/chaid_decision_tree.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    35170 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/data_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    60718 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/deep_q_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    26360 2023-04-16 23:16:10.000000 happy_learning-0.4.9/happy_learning/environment_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    31399 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/evaluate_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   350467 2023-04-24 16:52:19.000000 happy_learning-0.4.9/happy_learning/feature_engineer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    42132 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/feature_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    46706 2023-04-27 22:21:13.000000 happy_learning-0.4.9/happy_learning/feature_selector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   137255 2023-04-25 10:59:35.000000 happy_learning-0.4.9/happy_learning/genetic_algorithm.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     6461 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/missing_data_analysis.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    12205 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/multiple_imputation.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    74495 2023-04-16 17:16:09.000000 happy_learning-0.4.9/happy_learning/neural_network_generator_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34040 2023-04-16 17:16:33.000000 happy_learning-0.4.9/happy_learning/neural_network_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9223 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/sampler.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    22025 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/self_taught_short_text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   259606 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/supervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   136214 2023-04-25 13:55:53.000000 happy_learning-0.4.9/happy_learning/swarm_intelligence.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    30159 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    29520 2023-04-16 11:52:14.000000 happy_learning-0.4.9/happy_learning/text_clustering_generator.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    86060 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/text_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    44550 2022-06-13 17:25:08.000000 happy_learning-0.4.9/happy_learning/utils.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-27 22:39:28.128091 happy_learning-0.4.9/happy_learning.egg-info/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-27 22:39:27.000000 happy_learning-0.4.9/happy_learning.egg-info/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1745 2023-04-27 22:39:28.000000 happy_learning-0.4.9/happy_learning.egg-info/SOURCES.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-04-27 22:39:27.000000 happy_learning-0.4.9/happy_learning.egg-info/dependency_links.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      356 2023-04-27 22:39:27.000000 happy_learning-0.4.9/happy_learning.egg-info/requires.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       15 2023-04-27 22:39:27.000000 happy_learning-0.4.9/happy_learning.egg-info/top_level.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       92 2023-04-27 22:39:28.232520 happy_learning-0.4.9/setup.cfg
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3650 2023-04-27 12:48:30.000000 happy_learning-0.4.9/setup.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-27 22:39:28.229786 happy_learning-0.4.9/test/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_chaid_decision_tree.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4869 2023-04-24 23:30:40.000000 happy_learning-0.4.9/test/test_data_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    21152 2023-04-17 16:30:20.000000 happy_learning-0.4.9/test/test_deep_q_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3788 2023-04-17 00:38:08.000000 happy_learning-0.4.9/test/test_environment_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     5483 2023-04-17 00:42:31.000000 happy_learning-0.4.9/test/test_evaluate_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    39531 2023-04-24 17:12:05.000000 happy_learning-0.4.9/test/test_feature_engineer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    17611 2023-04-17 21:02:23.000000 happy_learning-0.4.9/test/test_feature_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4739 2023-04-27 22:24:30.000000 happy_learning-0.4.9/test/test_feature_selector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34272 2023-04-24 23:19:19.000000 happy_learning-0.4.9/test/test_genetic_algorithm.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2539 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_missing_data_analysis.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      754 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_multiple_imputation.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    12242 2023-04-16 01:08:43.000000 happy_learning-0.4.9/test/test_neural_network_generator_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     8949 2023-04-16 01:08:43.000000 happy_learning-0.4.9/test/test_neural_network_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1545 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_sampler.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      245 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_self_taught_short_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    16978 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_supervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34193 2023-04-26 17:28:30.000000 happy_learning-0.4.9/test/test_swarm_intelligence.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     7281 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    11994 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_text_clustering_generator.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4717 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_text_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.9/test/test_utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-05-06 12:08:58.232030 happy_learning-0.5.0/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34966 2022-06-13 17:25:08.000000 happy_learning-0.5.0/LICENSE
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-05-06 12:08:58.232357 happy_learning-0.5.0/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     8494 2022-06-13 17:25:08.000000 happy_learning-0.5.0/README.md
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-05-06 12:08:58.065186 happy_learning-0.5.0/happy_learning/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/__init__.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4331 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/arbitrary_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2189 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/chaid_decision_tree.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    35170 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/data_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    60718 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/deep_q_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    26360 2023-04-16 23:16:10.000000 happy_learning-0.5.0/happy_learning/environment_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    31399 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/evaluate_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   350467 2023-04-24 16:52:19.000000 happy_learning-0.5.0/happy_learning/feature_engineer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    42132 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/feature_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    46706 2023-04-27 22:21:13.000000 happy_learning-0.5.0/happy_learning/feature_selector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   137659 2023-05-05 12:24:53.000000 happy_learning-0.5.0/happy_learning/genetic_algorithm.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     6461 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/missing_data_analysis.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    12205 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/multiple_imputation.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    74495 2023-04-16 17:16:09.000000 happy_learning-0.5.0/happy_learning/neural_network_generator_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34040 2023-04-16 17:16:33.000000 happy_learning-0.5.0/happy_learning/neural_network_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9223 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/sampler.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    22025 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/self_taught_short_text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   259606 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/supervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   136618 2023-05-05 12:20:57.000000 happy_learning-0.5.0/happy_learning/swarm_intelligence.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    30159 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    29520 2023-04-16 11:52:14.000000 happy_learning-0.5.0/happy_learning/text_clustering_generator.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    86060 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/text_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    44550 2022-06-13 17:25:08.000000 happy_learning-0.5.0/happy_learning/utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-05-06 12:08:58.072217 happy_learning-0.5.0/happy_learning.egg-info/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-05-06 12:08:57.000000 happy_learning-0.5.0/happy_learning.egg-info/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1745 2023-05-06 12:08:57.000000 happy_learning-0.5.0/happy_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-05-06 12:08:57.000000 happy_learning-0.5.0/happy_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      356 2023-05-06 12:08:57.000000 happy_learning-0.5.0/happy_learning.egg-info/requires.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       15 2023-05-06 12:08:57.000000 happy_learning-0.5.0/happy_learning.egg-info/top_level.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       92 2023-05-06 12:08:58.233814 happy_learning-0.5.0/setup.cfg
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3650 2023-05-06 12:07:05.000000 happy_learning-0.5.0/setup.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-05-06 12:08:58.231088 happy_learning-0.5.0/test/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_chaid_decision_tree.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4869 2023-04-24 23:30:40.000000 happy_learning-0.5.0/test/test_data_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    21152 2023-04-17 16:30:20.000000 happy_learning-0.5.0/test/test_deep_q_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3788 2023-04-17 00:38:08.000000 happy_learning-0.5.0/test/test_environment_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     5483 2023-04-17 00:42:31.000000 happy_learning-0.5.0/test/test_evaluate_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    39531 2023-04-24 17:12:05.000000 happy_learning-0.5.0/test/test_feature_engineer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    17611 2023-04-17 21:02:23.000000 happy_learning-0.5.0/test/test_feature_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4687 2023-05-06 11:56:16.000000 happy_learning-0.5.0/test/test_feature_selector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34272 2023-04-24 23:19:19.000000 happy_learning-0.5.0/test/test_genetic_algorithm.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2539 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_missing_data_analysis.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      754 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_multiple_imputation.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    12242 2023-04-16 01:08:43.000000 happy_learning-0.5.0/test/test_neural_network_generator_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     8949 2023-04-16 01:08:43.000000 happy_learning-0.5.0/test/test_neural_network_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1545 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_sampler.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      245 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_self_taught_short_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    16978 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_supervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34193 2023-04-26 17:28:30.000000 happy_learning-0.5.0/test/test_swarm_intelligence.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     7281 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    11994 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_text_clustering_generator.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4717 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_text_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.5.0/test/test_utils.py
```

### Comparing `happy_learning-0.4.9/LICENSE` & `happy_learning-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/PKG-INFO` & `happy_learning-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy_learning
-Version: 0.4.9
+Version: 0.5.0
 Summary: Toolbox for reinforced developing of machine learning models (as proof-of-concept)
 Home-page: https://github.com/GianniBalistreri/happy_learning
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `happy_learning-0.4.9/README.md` & `happy_learning-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/arbitrary_modeling.py` & `happy_learning-0.5.0/happy_learning/arbitrary_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/chaid_decision_tree.py` & `happy_learning-0.5.0/happy_learning/chaid_decision_tree.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/data_miner.py` & `happy_learning-0.5.0/happy_learning/data_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/deep_q_learning.py` & `happy_learning-0.5.0/happy_learning/deep_q_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/environment_modeling.py` & `happy_learning-0.5.0/happy_learning/environment_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/evaluate_machine_learning.py` & `happy_learning-0.5.0/happy_learning/evaluate_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/feature_engineer.py` & `happy_learning-0.5.0/happy_learning/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/feature_learning.py` & `happy_learning-0.5.0/happy_learning/feature_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/feature_selector.py` & `happy_learning-0.5.0/happy_learning/feature_selector.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/genetic_algorithm.py` & `happy_learning-0.5.0/happy_learning/genetic_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1596,22 +1596,24 @@
                 DataVisualizer(df=_best_model_results,
                                title='Prediction Evaluation of final inherited ML Model:',
                                features=['obs', 'abs_diff', 'rel_diff', 'pred'],
                                color_feature='pred',
                                plot_type='parcoords',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'evaluation_coords.html'),
+                               render=False
                                ).run()
                 _file_paths.append(os.path.join(self.output_file_path, 'scatter_contour.html'))
                 DataVisualizer(df=_best_model_results,
                                title='Prediction vs. Observation of final inherited ML Model:',
                                features=['obs', 'pred'],
                                plot_type='joint',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'scatter_contour.html'),
+                               render=False
                                ).run()
             else:
                 _eval_clf: EvalClf = EvalClf(obs=self.data_set.get('y_test'),
                                              pred=self.data_set.get('pred'),
                                              labels=self.target_labels
                                              )
                 _confusion_matrix: pd.DataFrame = pd.DataFrame(data=_eval_clf.confusion(),
@@ -1627,44 +1629,48 @@
                 _file_paths.append(os.path.join(self.output_file_path, 'confusion_table.html'))
                 DataVisualizer(df=_confusion_matrix,
                                title='Confusion Matrix:',
                                features=_confusion_matrix.columns.to_list(),
                                plot_type='table',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'confusion_table.html'),
+                               render=False
                                ).run()
                 _file_paths.append(os.path.join(self.output_file_path, 'confusion_heatmap.html'))
                 DataVisualizer(df=_confusion_matrix,
                                title='Confusion Matrix Heatmap:',
                                features=_confusion_matrix.columns.to_list(),
                                plot_type='heat',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'confusion_heatmap.html'),
+                               render=False
                                ).run()
                 _confusion_matrix_normalized: pd.DataFrame = pd.DataFrame(data=EvalClf(obs=self.data_set.get('y_test'),
                                                                                        pred=self.data_set.get('pred')
                                                                                        ).confusion(normalize='pred'),
                                                                           # index=['obs', 'pred'],
                                                                           # columns=['obs', 'pred']
                                                                           )
                 _file_paths.append(os.path.join(self.output_file_path, 'confusion_normal_heatmap.html'))
                 DataVisualizer(df=_confusion_matrix_normalized,
                                title='Confusion Matrix Normalized Heatmap:',
                                features=_confusion_matrix_normalized.columns.to_list(),
                                plot_type='heat',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'confusion_normal_heatmap.html'),
+                               render=False
                                ).run()
                 _file_paths.append(os.path.join(self.output_file_path, 'clf_report_table.html'))
                 DataVisualizer(df=_best_model_results,
                                title='Classification Report:',
                                features=_best_model_results.columns.to_list(),
                                plot_type='table',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'clf_report_table.html'),
+                               render=False
                                ).run()
                 _classification_report: dict = _eval_clf.classification_report()
                 _confusion_metrics: dict = dict(precision=[], recall=[], f1=[])
                 for label in self.target_labels:
                     _confusion_metrics['precision'].append(_classification_report.get(label)['precision'])
                     _confusion_metrics['recall'].append(_classification_report.get(label)['recall'])
                     _confusion_metrics['f1'].append(_classification_report.get(label)['f1-score'])
@@ -1675,24 +1681,26 @@
                                                           )
                 DataVisualizer(df=_clf_metrics,
                                title='Classification Metrics:',
                                features=_clf_metrics.columns.to_list(),
                                plot_type='table',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'clf_metrics_table.html'),
+                               render=False
                                ).run()
                 if self.target_type == 'clf_multi':
                     _file_paths.append(os.path.join(self.output_file_path, 'evaluation_category.html'))
                     DataVisualizer(df=_best_model_results,
                                    title='Prediction Evaluation of final inherited ML Model:',
                                    features=['obs', 'abs_diff', 'pred'],
                                    color_feature='pred',
                                    plot_type='parcoords',
                                    file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                        self.output_file_path, 'evaluation_category.html'),
+                                   render=False
                                    ).run()
                 else:
                     _roc_curve = pd.DataFrame()
                     _roc_curve_values: dict = EvalClf(obs=_best_model_results['obs'],
                                                       pred=_best_model_results['pred']
                                                       ).roc_curve()
                     _roc_curve['roc_curve'] = _roc_curve_values['true_positive_rate'][1]
@@ -1704,14 +1712,15 @@
                                    time_features=['baseline'],
                                    plot_type='line',
                                    # xaxis_label=['False Positive Rate'],
                                    # yaxis_label=['True Positive Rate'],
                                    use_auto_extensions=False,
                                    file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                        self.output_file_path, 'roc_auc_curve.html'),
+                                   render=False
                                    ).run()
             for path in _file_paths:
                 _file_name: str = path.split('/')[-1].replace('.html', '')
                 try:
                     mlflow.log_artifact(local_path=path, artifact_path=_file_name)
                 except FileNotFoundError:
                     Log(write=self.log, logger_file_path=self.output_file_path).log(f'File artifact {path} not found')
```

### Comparing `happy_learning-0.4.9/happy_learning/missing_data_analysis.py` & `happy_learning-0.5.0/happy_learning/missing_data_analysis.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/multiple_imputation.py` & `happy_learning-0.5.0/happy_learning/multiple_imputation.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/neural_network_generator_torch.py` & `happy_learning-0.5.0/happy_learning/neural_network_generator_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/neural_network_torch.py` & `happy_learning-0.5.0/happy_learning/neural_network_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/sampler.py` & `happy_learning-0.5.0/happy_learning/sampler.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/self_taught_short_text_clustering.py` & `happy_learning-0.5.0/happy_learning/self_taught_short_text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/supervised_machine_learning.py` & `happy_learning-0.5.0/happy_learning/supervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/swarm_intelligence.py` & `happy_learning-0.5.0/happy_learning/swarm_intelligence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1517,22 +1517,24 @@
                 DataVisualizer(df=_best_model_results,
                                title='Prediction Evaluation of final inherited ML Model:',
                                features=['obs', 'abs_diff', 'rel_diff', 'pred'],
                                color_feature='pred',
                                plot_type='parcoords',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'evaluation_coords.html'),
+                               render=False
                                ).run()
                 _file_paths.append(os.path.join(self.output_file_path, 'scatter_contour.html'))
                 DataVisualizer(df=_best_model_results,
                                title='Prediction vs. Observation of final inherited ML Model:',
                                features=['obs', 'pred'],
                                plot_type='joint',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'scatter_contour.html'),
+                               render=False
                                ).run()
             else:
                 _eval_clf: EvalClf = EvalClf(obs=self.data_set.get('y_test'),
                                              pred=self.data_set.get('pred'),
                                              labels=self.target_labels
                                              )
                 _confusion_matrix: pd.DataFrame = pd.DataFrame(data=_eval_clf.confusion(),
@@ -1548,44 +1550,48 @@
                 _file_paths.append(os.path.join(self.output_file_path, 'confusion_table.html'))
                 DataVisualizer(df=_confusion_matrix,
                                title='Confusion Matrix:',
                                features=_confusion_matrix.columns.to_list(),
                                plot_type='table',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'confusion_table.html'),
+                               render=False
                                ).run()
                 _file_paths.append(os.path.join(self.output_file_path, 'confusion_heatmap.html'))
                 DataVisualizer(df=_confusion_matrix,
                                title='Confusion Matrix Heatmap:',
                                features=_confusion_matrix.columns.to_list(),
                                plot_type='heat',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'confusion_heatmap.html'),
+                               render=False
                                ).run()
                 _confusion_matrix_normalized: pd.DataFrame = pd.DataFrame(data=EvalClf(obs=self.data_set.get('y_test'),
                                                                                        pred=self.data_set.get('pred')
                                                                                        ).confusion(normalize='pred'),
                                                                           # index=['obs', 'pred'],
                                                                           # columns=['obs', 'pred']
                                                                           )
                 _file_paths.append(os.path.join(self.output_file_path, 'confusion_normal_heatmap.html'))
                 DataVisualizer(df=_confusion_matrix_normalized,
                                title='Confusion Matrix Normalized Heatmap:',
                                features=_confusion_matrix_normalized.columns.to_list(),
                                plot_type='heat',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'confusion_normal_heatmap.html'),
+                               render=False
                                ).run()
                 _file_paths.append(os.path.join(self.output_file_path, 'clf_report_table.html'))
                 DataVisualizer(df=_best_model_results,
                                title='Classification Report:',
                                features=_best_model_results.columns.to_list(),
                                plot_type='table',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'clf_report_table.html'),
+                               render=False
                                ).run()
                 _classification_report: dict = _eval_clf.classification_report()
                 _confusion_metrics: dict = dict(precision=[], recall=[], f1=[])
                 for label in self.target_labels:
                     _confusion_metrics['precision'].append(_classification_report.get(label)['precision'])
                     _confusion_metrics['recall'].append(_classification_report.get(label)['recall'])
                     _confusion_metrics['f1'].append(_classification_report.get(label)['f1-score'])
@@ -1596,24 +1602,26 @@
                                                           )
                 DataVisualizer(df=_clf_metrics,
                                title='Classification Metrics:',
                                features=_clf_metrics.columns.to_list(),
                                plot_type='table',
                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                    self.output_file_path, 'clf_metrics_table.html'),
+                               render=False
                                ).run()
                 if self.target_type == 'clf_multi':
                     _file_paths.append(os.path.join(self.output_file_path, 'evaluation_category.html'))
                     DataVisualizer(df=_best_model_results,
                                    title='Prediction Evaluation of final inherited ML Model:',
                                    features=['obs', 'abs_diff', 'pred'],
                                    color_feature='pred',
                                    plot_type='parcoords',
                                    file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                        self.output_file_path, 'evaluation_category.html'),
+                                   render=False
                                    ).run()
                 else:
                     _roc_curve = pd.DataFrame()
                     _roc_curve_values: dict = EvalClf(obs=_best_model_results['obs'],
                                                       pred=_best_model_results['pred']
                                                       ).roc_curve()
                     _roc_curve['roc_curve'] = _roc_curve_values['true_positive_rate'][1]
@@ -1625,14 +1633,15 @@
                                    time_features=['baseline'],
                                    plot_type='line',
                                    # xaxis_label=['False Positive Rate'],
                                    # yaxis_label=['True Positive Rate'],
                                    use_auto_extensions=False,
                                    file_path=self.output_file_path if self.output_file_path is None else os.path.join(
                                        self.output_file_path, 'roc_auc_curve.html'),
+                                   render=False
                                    ).run()
             for path in _file_paths:
                 _file_name: str = path.split('/')[-1].replace('.html', '')
                 try:
                     mlflow.log_artifact(local_path=path, artifact_path=_file_name)
                 except FileNotFoundError:
                     Log(write=self.log, logger_file_path=self.output_file_path).log(f'File artifact {path} not found')
```

### Comparing `happy_learning-0.4.9/happy_learning/text_clustering.py` & `happy_learning-0.5.0/happy_learning/text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/text_clustering_generator.py` & `happy_learning-0.5.0/happy_learning/text_clustering_generator.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/text_miner.py` & `happy_learning-0.5.0/happy_learning/text_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning/utils.py` & `happy_learning-0.5.0/happy_learning/utils.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/happy_learning.egg-info/PKG-INFO` & `happy_learning-0.5.0/happy_learning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy-learning
-Version: 0.4.9
+Version: 0.5.0
 Summary: Toolbox for reinforced developing of machine learning models (as proof-of-concept)
 Home-page: https://github.com/GianniBalistreri/happy_learning
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `happy_learning-0.4.9/happy_learning.egg-info/SOURCES.txt` & `happy_learning-0.5.0/happy_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/setup.py` & `happy_learning-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 with open('requirements.txt', 'r') as _requirements:
     requires = _requirements.read()
 
 requires = [r.strip() for r in requires.split('\n') if ((r.strip()[0] != "#") and (len(r.strip()) > 3) and "-e git://" not in r)]
 
 setuptools.setup(
     name='happy_learning',
-    version='0.4.9',
+    version='0.5.0',
     author='Gianni Francesco Balistreri',
     author_email='gbalistreri@gmx.de',
     description='Toolbox for reinforced developing of machine learning models (as proof-of-concept)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch',
     license='GNU',
```

### Comparing `happy_learning-0.4.9/test/test_data_miner.py` & `happy_learning-0.5.0/test/test_data_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_deep_q_learning.py` & `happy_learning-0.5.0/test/test_deep_q_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_environment_modeling.py` & `happy_learning-0.5.0/test/test_environment_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_evaluate_machine_learning.py` & `happy_learning-0.5.0/test/test_evaluate_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_feature_engineer.py` & `happy_learning-0.5.0/test/test_feature_engineer.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_feature_learning.py` & `happy_learning-0.5.0/test/test_feature_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_feature_selector.py` & `happy_learning-0.5.0/test/test_feature_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """
     def test_select(self):
         _features: List[str] = ['Total Volume', 'Total Bags', 'Small Bags', 'Large Bags', 'XLarge Bags', '4046', '4225']
         _feature_selector: FeatureSelector = FeatureSelector(df=DATA_SET,
                                                              target='AveragePrice',
                                                              features=_features,
                                                              force_target_type=None,
-                                                             model_name='cat',
+                                                             model_name='xgb',
                                                              init_pairs=3,
                                                              init_games=5,
                                                              increasing_pair_size_factor=0.5,
                                                              games=3,
                                                              penalty_factor=0.1,
                                                              max_iter=50,
                                                              max_players=-1,
@@ -50,25 +50,24 @@
                                             random_sample=True,
                                             stratification=False,
                                             seed=1234
                                             ).train_test_sampling(validation_split=0.1)
         _model_reg_all_features: ModelGeneratorReg = ModelGeneratorReg(model_name='xgb')
         _model_reg_all_features.generate_model()
         _model_reg_all_features.train(x=_train_test_split['x_train'], y=_train_test_split['y_train'])
-        _pred_all_features = _model_reg_all_features.predict(x=_train_test_split['y_test'])
+        _pred_all_features = _model_reg_all_features.predict(x=_train_test_split['x_test'])
         _model_reg_all_features.eval(obs=_train_test_split['y_test'], pred=_pred_all_features)
         _model_reg_imp_features: ModelGeneratorReg = ModelGeneratorReg(model_name='xgb',
                                                                        reg_params=_model_reg_all_features.model_param
                                                                        )
         _model_reg_imp_features.generate_model()
         _model_reg_imp_features.train(x=_train_test_split['x_train'][_imp_features],
-                                      y=_train_test_split['y_train'][_imp_features]
+                                      y=_train_test_split['y_train']
                                       )
         _pred_imp_features = _model_reg_imp_features.predict(x=_train_test_split['x_test'][_imp_features])
-        _model_reg_all_features.eval(obs=_train_test_split['y_test'][_imp_features], pred=_pred_imp_features)
-        self.assertAlmostEqual(first=_model_reg_all_features.fitness['test']['rmse_norm'],
-                               second=_model_reg_imp_features.fitness['test']['rmse_norm']
-                               )
+        _model_reg_imp_features.eval(obs=_train_test_split['y_test'], pred=_pred_imp_features)
+        _differences: float = abs(_model_reg_imp_features.fitness['test']['rmse_norm'] - _model_reg_all_features.fitness['test']['rmse_norm'])
+        self.assertTrue(expr=_differences <= 0.1)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `happy_learning-0.4.9/test/test_genetic_algorithm.py` & `happy_learning-0.5.0/test/test_genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_missing_data_analysis.py` & `happy_learning-0.5.0/test/test_missing_data_analysis.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_multiple_imputation.py` & `happy_learning-0.5.0/test/test_multiple_imputation.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_neural_network_generator_torch.py` & `happy_learning-0.5.0/test/test_neural_network_generator_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_neural_network_torch.py` & `happy_learning-0.5.0/test/test_neural_network_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_sampler.py` & `happy_learning-0.5.0/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_supervised_machine_learning.py` & `happy_learning-0.5.0/test/test_supervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_swarm_intelligence.py` & `happy_learning-0.5.0/test/test_swarm_intelligence.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_text_clustering.py` & `happy_learning-0.5.0/test/test_text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_text_clustering_generator.py` & `happy_learning-0.5.0/test/test_text_clustering_generator.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.9/test/test_text_miner.py` & `happy_learning-0.5.0/test/test_text_miner.py`

 * *Files identical despite different names*

