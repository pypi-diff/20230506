# Comparing `tmp/rulelearn-0.1.0.tar.gz` & `tmp/rulelearn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulelearn-0.1.0.tar", last modified: Tue Mar 28 18:47:10 2023, max compression
+gzip compressed data, was "rulelearn-0.1.1.tar", last modified: Sat May  6 21:09:25 2023, max compression
```

## Comparing `rulelearn-0.1.0.tar` & `rulelearn-0.1.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.639457 rulelearn-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-03-28 18:24:31.000000 rulelearn-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2316 2023-03-28 18:47:10.639457 rulelearn-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1586 2023-03-28 18:24:31.000000 rulelearn-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.562386 rulelearn-0.1.0/rulelearn/
--rw-rw-rw-   0        0        0       86 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.567386 rulelearn-0.1.0/rulelearn/algorithms/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.573543 rulelearn-0.1.0/rulelearn/algorithms/r2n/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/base.py
--rw-rw-rw-   0        0        0      707 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/functions.py
--rw-rw-rw-   0        0        0     1650 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/mask.py
--rw-rw-rw-   0        0        0     7153 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/preprocessing_layers.py
--rw-rw-rw-   0        0        0    12953 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/r2n_algo.py
--rw-rw-rw-   0        0        0     2616 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/simple_rulenet.py
--rw-rw-rw-   0        0        0     1116 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/training.py
--rw-rw-rw-   0        0        0     4368 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/r2n/utilities.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.575543 rulelearn-0.1.0/rulelearn/algorithms/rbm/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/__init__.py
--rw-rw-rw-   0        0        0     2280 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/boolean_rule_cg.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.581543 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/
--rw-rw-rw-   0        0        0     2588 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/BRCG.py
--rw-rw-rw-   0        0        0     3834 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/GLRM.py
--rw-rw-rw-   0        0        0      287 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/__init__.py
--rw-rw-rw-   0        0        0    13359 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/beam_search.py
--rw-rw-rw-   0        0        0    10152 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/boolean_rule_cg.py
--rw-rw-rw-   0        0        0    24097 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/features.py
--rw-rw-rw-   0        0        0    17987 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/linear_regression.py
--rw-rw-rw-   0        0        0    20260 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/logistic_regression.py
--rw-rw-rw-   0        0        0      325 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/rbm/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.586543 rulelearn-0.1.0/rulelearn/algorithms/ripper/
--rw-rw-rw-   0        0        0      167 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/ripper/__init__.py
--rw-rw-rw-   0        0        0     2647 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/ripper/base.py
--rw-rw-rw-   0        0        0    12461 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/ripper/binding.py
--rw-rw-rw-   0        0        0     2109 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/ripper/mdl.py
--rw-rw-rw-   0        0        0     4662 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/ripper/pruning.py
--rw-rw-rw-   0        0        0    22006 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/ripper/ripper.py
--rw-rw-rw-   0        0        0      919 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/algorithms/ripper/ripper_ruleset_generator.py
--rw-rw-rw-   0        0        0     2052 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/dise.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.587543 rulelearn-0.1.0/rulelearn/trxf/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.588544 rulelearn-0.1.0/rulelearn/trxf/classifier/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/classifier/__init__.py
--rw-rw-rw-   0        0        0     6429 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/classifier/ruleset_classifier.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.593543 rulelearn-0.1.0/rulelearn/trxf/core/
--rw-rw-rw-   0        0        0      198 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/core/__init__.py
--rw-rw-rw-   0        0        0      412 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/core/boolean_evaluator.py
--rw-rw-rw-   0        0        0     1580 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/core/conjunction.py
--rw-rw-rw-   0        0        0     2372 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/core/dnf_ruleset.py
--rw-rw-rw-   0        0        0     5229 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/core/feature.py
--rw-rw-rw-   0        0        0     3254 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/core/predicate.py
--rw-rw-rw-   0        0        0      838 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/core/ruleset_generator.py
--rw-rw-rw-   0        0        0     1282 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/core/utils.py
--rw-rw-rw-   0        0        0     4357 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/metrics.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.595543 rulelearn-0.1.0/rulelearn/trxf/pmml_export/
--rw-rw-rw-   0        0        0      184 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/__init__.py
--rw-rw-rw-   0        0        0       19 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/__version__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.601542 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/
--rw-rw-rw-   0        0        0     1005 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/__init__.py
--rw-rw-rw-   0        0        0      641 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/attribute.py
--rw-rw-rw-   0        0        0      401 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/characteristics.py
--rw-rw-rw-   0        0        0     1176 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/data_dictionary.py
--rw-rw-rw-   0        0        0      579 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/mining_schema.py
--rw-rw-rw-   0        0        0      451 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/pmml_ruleset_model.py
--rw-rw-rw-   0        0        0     1007 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/predicate.py
--rw-rw-rw-   0        0        0      831 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/rule.py
--rw-rw-rw-   0        0        0      791 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/ruleset.py
--rw-rw-rw-   0        0        0      412 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/ruleset_model.py
--rw-rw-rw-   0        0        0      834 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/scorecard.py
--rw-rw-rw-   0        0        0      794 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/pmml_exporter.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.602542 rulelearn-0.1.0/rulelearn/trxf/pmml_export/reader/
--rw-rw-rw-   0        0        0       82 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/reader/__init__.py
--rw-rw-rw-   0        0        0      327 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/reader/abstract_reader.py
--rw-rw-rw-   0        0        0     5575 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/reader/trxf_reader.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.604543 rulelearn-0.1.0/rulelearn/trxf/pmml_export/serializer/
--rw-rw-rw-   0        0        0      100 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/serializer/__init__.py
--rw-rw-rw-   0        0        0      257 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/serializer/abstract_serializer.py
--rw-rw-rw-   0        0        0     9010 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/pmml_export/serializer/nyoka_serializer.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.606543 rulelearn-0.1.0/rulelearn/trxf/scorecard/
--rw-rw-rw-   0        0        0      131 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/scorecard/__init__.py
--rw-rw-rw-   0        0        0    10585 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/scorecard/bins.py
--rw-rw-rw-   0        0        0     3162 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/scorecard/partition.py
--rw-rw-rw-   0        0        0     3014 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/trxf/scorecard/scorecard.py
--rw-rw-rw-   0        0        0       44 2023-03-28 18:24:31.000000 rulelearn-0.1.0/rulelearn/version.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.566386 rulelearn-0.1.0/rulelearn.egg-info/
--rw-rw-rw-   0        0        0     2316 2023-03-28 18:47:10.000000 rulelearn-0.1.0/rulelearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4277 2023-03-28 18:47:10.000000 rulelearn-0.1.0/rulelearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 18:47:10.000000 rulelearn-0.1.0/rulelearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-03-28 18:47:10.000000 rulelearn-0.1.0/rulelearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-28 18:47:10.000000 rulelearn-0.1.0/rulelearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 18:47:10.640457 rulelearn-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-03-28 18:47:03.000000 rulelearn-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.607543 rulelearn-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.610542 rulelearn-0.1.0/tests/r2n/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/r2n/__init__.py
--rw-rw-rw-   0        0        0      385 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/r2n/test_mask.py
--rw-rw-rw-   0        0        0     2872 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/r2n/test_preprocessing_layers.py
--rw-rw-rw-   0        0        0     9783 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/r2n/test_r2n_algo.py
--rw-rw-rw-   0        0        0     1959 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/r2n/test_simple_rulenet.py
--rw-rw-rw-   0        0        0     1905 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/r2n/test_utilities.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.614480 rulelearn-0.1.0/tests/rbm/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/rbm/__init__.py
--rw-rw-rw-   0        0        0     1952 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/rbm/test_Boolean_Rule_CG.py
--rw-rw-rw-   0        0        0    18619 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/rbm/test_Feature_Binarizer_From_Trees.py
--rw-rw-rw-   0        0        0     2875 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/rbm/test_Logistic_Rule_Regression.py
--rw-rw-rw-   0        0        0     2760 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/rbm/test_brcg.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.616457 rulelearn-0.1.0/tests/ripper/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/ripper/__init__.py
--rw-rw-rw-   0        0        0     1274 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/ripper/test_base.py
--rw-rw-rw-   0        0        0     1318 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/ripper/test_binding.py
--rw-rw-rw-   0        0        0     4732 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/ripper/test_ripper.py
--rw-rw-rw-   0        0        0     1336 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/ripper/test_ripper_ruleset_generator.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.623458 rulelearn-0.1.0/tests/trxf/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.625457 rulelearn-0.1.0/tests/trxf/classifier/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/classifier/__init__.py
--rw-rw-rw-   0        0        0     2532 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/classifier/test_ruleset_classifier.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.631458 rulelearn-0.1.0/tests/trxf/core/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/core/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/core/test_conjunction.py
--rw-rw-rw-   0        0        0     4227 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/core/test_dnfruleset.py
--rw-rw-rw-   0        0        0     2990 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/core/test_feature.py
--rw-rw-rw-   0        0        0     2935 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/core/test_predicate.py
--rw-rw-rw-   0        0        0     1465 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/core/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.636457 rulelearn-0.1.0/tests/trxf/pmml_export/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/pmml_export/__init__.py
--rw-rw-rw-   0        0        0     6200 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/pmml_export/test_nyoka_serialize_common.py
--rw-rw-rw-   0        0        0     7547 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/pmml_export/test_nyoka_serialize_integration.py
--rw-rw-rw-   0        0        0     4767 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/pmml_export/test_nyoka_serialize_ruleset.py
--rw-rw-rw-   0        0        0     9976 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/pmml_export/test_nyoka_serialize_scorecard.py
--rw-rw-rw-   0        0        0     8489 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/pmml_export/test_pmml_exporter.py
--rw-rw-rw-   0        0        0     1192 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/pmml_export/test_trxf_reader.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:47:10.638457 rulelearn-0.1.0/tests/trxf/scorecard/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/scorecard/__init__.py
--rw-rw-rw-   0        0        0     9889 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/scorecard/test_bins.py
--rw-rw-rw-   0        0        0     5752 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/scorecard/test_partition.py
--rw-rw-rw-   0        0        0     6120 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/scorecard/test_scorecard.py
--rw-rw-rw-   0        0        0     1892 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/test_metrics.py
--rw-rw-rw-   0        0        0     5831 2023-03-28 18:24:31.000000 rulelearn-0.1.0/tests/trxf/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.054362 rulelearn-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-03-28 18:24:31.000000 rulelearn-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1689 2023-05-06 21:09:25.053362 rulelearn-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2023-05-06 21:05:16.000000 rulelearn-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:24.983363 rulelearn-0.1.1/rulelearn/
+-rw-rw-rw-   0        0        0       86 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:24.987362 rulelearn-0.1.1/rulelearn/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:24.993363 rulelearn-0.1.1/rulelearn/algorithms/r2n/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/base.py
+-rw-rw-rw-   0        0        0      707 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/functions.py
+-rw-rw-rw-   0        0        0     1650 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/mask.py
+-rw-rw-rw-   0        0        0     7153 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/preprocessing_layers.py
+-rw-rw-rw-   0        0        0    12953 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/r2n_algo.py
+-rw-rw-rw-   0        0        0     2616 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/simple_rulenet.py
+-rw-rw-rw-   0        0        0     1116 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/training.py
+-rw-rw-rw-   0        0        0     4368 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/r2n/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:24.995363 rulelearn-0.1.1/rulelearn/algorithms/rbm/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/__init__.py
+-rw-rw-rw-   0        0        0     2280 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/boolean_rule_cg.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.000362 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/
+-rw-rw-rw-   0        0        0     2588 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/BRCG.py
+-rw-rw-rw-   0        0        0     3834 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/GLRM.py
+-rw-rw-rw-   0        0        0      287 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/__init__.py
+-rw-rw-rw-   0        0        0    13359 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/beam_search.py
+-rw-rw-rw-   0        0        0    10152 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/boolean_rule_cg.py
+-rw-rw-rw-   0        0        0    24097 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/features.py
+-rw-rw-rw-   0        0        0    17987 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/linear_regression.py
+-rw-rw-rw-   0        0        0    20260 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/logistic_regression.py
+-rw-rw-rw-   0        0        0      325 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/rbm/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.005363 rulelearn-0.1.1/rulelearn/algorithms/ripper/
+-rw-rw-rw-   0        0        0      167 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/ripper/__init__.py
+-rw-rw-rw-   0        0        0     2647 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/ripper/base.py
+-rw-rw-rw-   0        0        0    12461 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/ripper/binding.py
+-rw-rw-rw-   0        0        0     2109 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/ripper/mdl.py
+-rw-rw-rw-   0        0        0     4662 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/ripper/pruning.py
+-rw-rw-rw-   0        0        0    22006 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/ripper/ripper.py
+-rw-rw-rw-   0        0        0      919 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/algorithms/ripper/ripper_ruleset_generator.py
+-rw-rw-rw-   0        0        0     2052 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/dise.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.006362 rulelearn-0.1.1/rulelearn/trxf/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.007363 rulelearn-0.1.1/rulelearn/trxf/classifier/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/classifier/__init__.py
+-rw-rw-rw-   0        0        0     6429 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/classifier/ruleset_classifier.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.013363 rulelearn-0.1.1/rulelearn/trxf/core/
+-rw-rw-rw-   0        0        0      198 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/core/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/core/boolean_evaluator.py
+-rw-rw-rw-   0        0        0     1580 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/core/conjunction.py
+-rw-rw-rw-   0        0        0     2372 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/core/dnf_ruleset.py
+-rw-rw-rw-   0        0        0     5229 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/core/feature.py
+-rw-rw-rw-   0        0        0     3254 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/core/predicate.py
+-rw-rw-rw-   0        0        0      838 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/core/ruleset_generator.py
+-rw-rw-rw-   0        0        0     1282 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/core/utils.py
+-rw-rw-rw-   0        0        0     4357 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.014362 rulelearn-0.1.1/rulelearn/trxf/pmml_export/
+-rw-rw-rw-   0        0        0      184 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.022363 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/
+-rw-rw-rw-   0        0        0     1005 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/__init__.py
+-rw-rw-rw-   0        0        0      641 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/attribute.py
+-rw-rw-rw-   0        0        0      401 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/characteristics.py
+-rw-rw-rw-   0        0        0     1176 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/data_dictionary.py
+-rw-rw-rw-   0        0        0      579 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/mining_schema.py
+-rw-rw-rw-   0        0        0      451 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/pmml_ruleset_model.py
+-rw-rw-rw-   0        0        0     1007 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/predicate.py
+-rw-rw-rw-   0        0        0      831 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/rule.py
+-rw-rw-rw-   0        0        0      791 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/ruleset.py
+-rw-rw-rw-   0        0        0      412 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/ruleset_model.py
+-rw-rw-rw-   0        0        0      834 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/scorecard.py
+-rw-rw-rw-   0        0        0      794 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/pmml_exporter.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.024362 rulelearn-0.1.1/rulelearn/trxf/pmml_export/reader/
+-rw-rw-rw-   0        0        0       82 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/reader/__init__.py
+-rw-rw-rw-   0        0        0      327 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/reader/abstract_reader.py
+-rw-rw-rw-   0        0        0     5575 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/reader/trxf_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.026363 rulelearn-0.1.1/rulelearn/trxf/pmml_export/serializer/
+-rw-rw-rw-   0        0        0      100 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/serializer/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/serializer/abstract_serializer.py
+-rw-rw-rw-   0        0        0     9010 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/pmml_export/serializer/nyoka_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.028362 rulelearn-0.1.1/rulelearn/trxf/scorecard/
+-rw-rw-rw-   0        0        0      131 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/scorecard/__init__.py
+-rw-rw-rw-   0        0        0    10585 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/scorecard/bins.py
+-rw-rw-rw-   0        0        0     3162 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/scorecard/partition.py
+-rw-rw-rw-   0        0        0     3014 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/trxf/scorecard/scorecard.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 18:24:31.000000 rulelearn-0.1.1/rulelearn/version.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:24.986362 rulelearn-0.1.1/rulelearn.egg-info/
+-rw-rw-rw-   0        0        0     1689 2023-05-06 21:09:24.000000 rulelearn-0.1.1/rulelearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4277 2023-05-06 21:09:24.000000 rulelearn-0.1.1/rulelearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 21:09:24.000000 rulelearn-0.1.1/rulelearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-05-06 21:09:24.000000 rulelearn-0.1.1/rulelearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 21:09:24.000000 rulelearn-0.1.1/rulelearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 21:09:25.054362 rulelearn-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-05-06 21:09:16.000000 rulelearn-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.029362 rulelearn-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.032362 rulelearn-0.1.1/tests/r2n/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/r2n/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/r2n/test_mask.py
+-rw-rw-rw-   0        0        0     2872 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/r2n/test_preprocessing_layers.py
+-rw-rw-rw-   0        0        0     9783 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/r2n/test_r2n_algo.py
+-rw-rw-rw-   0        0        0     1959 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/r2n/test_simple_rulenet.py
+-rw-rw-rw-   0        0        0     1905 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/r2n/test_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.035362 rulelearn-0.1.1/tests/rbm/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/rbm/__init__.py
+-rw-rw-rw-   0        0        0     1952 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/rbm/test_Boolean_Rule_CG.py
+-rw-rw-rw-   0        0        0    18619 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/rbm/test_Feature_Binarizer_From_Trees.py
+-rw-rw-rw-   0        0        0     2875 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/rbm/test_Logistic_Rule_Regression.py
+-rw-rw-rw-   0        0        0     2760 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/rbm/test_brcg.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.039363 rulelearn-0.1.1/tests/ripper/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/ripper/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/ripper/test_base.py
+-rw-rw-rw-   0        0        0     1318 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/ripper/test_binding.py
+-rw-rw-rw-   0        0        0     4732 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/ripper/test_ripper.py
+-rw-rw-rw-   0        0        0     1336 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/ripper/test_ripper_ruleset_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.041363 rulelearn-0.1.1/tests/trxf/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.042362 rulelearn-0.1.1/tests/trxf/classifier/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/classifier/__init__.py
+-rw-rw-rw-   0        0        0     2532 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/classifier/test_ruleset_classifier.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.046362 rulelearn-0.1.1/tests/trxf/core/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/core/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/core/test_conjunction.py
+-rw-rw-rw-   0        0        0     4227 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/core/test_dnfruleset.py
+-rw-rw-rw-   0        0        0     2990 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/core/test_feature.py
+-rw-rw-rw-   0        0        0     2935 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/core/test_predicate.py
+-rw-rw-rw-   0        0        0     1465 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/core/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.050361 rulelearn-0.1.1/tests/trxf/pmml_export/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/pmml_export/__init__.py
+-rw-rw-rw-   0        0        0     6200 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/pmml_export/test_nyoka_serialize_common.py
+-rw-rw-rw-   0        0        0     7547 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/pmml_export/test_nyoka_serialize_integration.py
+-rw-rw-rw-   0        0        0     4767 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/pmml_export/test_nyoka_serialize_ruleset.py
+-rw-rw-rw-   0        0        0     9976 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/pmml_export/test_nyoka_serialize_scorecard.py
+-rw-rw-rw-   0        0        0     8489 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/pmml_export/test_pmml_exporter.py
+-rw-rw-rw-   0        0        0     1192 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/pmml_export/test_trxf_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:09:25.053362 rulelearn-0.1.1/tests/trxf/scorecard/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/scorecard/__init__.py
+-rw-rw-rw-   0        0        0     9889 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/scorecard/test_bins.py
+-rw-rw-rw-   0        0        0     5752 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/scorecard/test_partition.py
+-rw-rw-rw-   0        0        0     6120 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/scorecard/test_scorecard.py
+-rw-rw-rw-   0        0        0     1892 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/test_metrics.py
+-rw-rw-rw-   0        0        0     5831 2023-03-28 18:24:31.000000 rulelearn-0.1.1/tests/trxf/utilities.py
```

### Comparing `rulelearn-0.1.0/LICENSE` & `rulelearn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/PKG-INFO` & `rulelearn-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 Metadata-Version: 2.1
 Name: rulelearn
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package contains a rule induction toolkit to generate readable and editable rules from data.
 Home-page: https://github.com/IBM/rulelearn
 Author: Various
 Author-email: hvoelzer@acm.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rulelearn (v0.1)
 
-This package contains a rule induction toolkit to generate readable and editable rules from data. The code was
-originally released within the larger [AIX 360 package](https://github.com/Trusted-AI/AIX360) and is provided and 
-extended here separately with less dependencies.
+This package contains a rule induction toolkit to generate readable and editable rules from data. The code was originally released within the larger AIX 360 package and is provided and extended here separately with less dependencies.
 
 It contains the following components:
 
-- Boolean Decision Rules via Column Generation (Light Edition) ([Dash et al., 2018](https://papers.nips.cc/paper/7716-boolean-decision-rules-via-column-generation))
-- Generalized Linear Rule Models ([Wei et al., 2019](http://proceedings.mlr.press/v97/wei19a.html))
-- Fast Effective Rule Induction (Ripper) ([William W Cohen, 1995](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.107.2612&rep=rep1&type=pdf))
-- Relational Rule Network (R2N) ([Kusters et al., 2022](https://arxiv.org/abs/2201.06515))
-- trxf - Technical Rule Interchange Format - Rule Set Interchange providing common evaluation tools and PMML export for 
-rule sets.
+Boolean Decision Rules via Column Generation (Light Edition) (Dash et al., 2018)
+Generalized Linear Rule Models (Wei et al., 2019)
+Fast Effective Rule Induction (Ripper) (William W Cohen, 1995)
+Relational Rule Network (R2N) (Kusters et al., 2022)
+trxf - Technical Rule Interchange Format - Rule Set Interchange providing common evaluation tools and PMML export for rule sets.
 
 
 ### Installation
 
 ```
-pip install -r requirements.txt
+pip install rulelearn
 ```
-to be completed.
+
 
 
 ## Acknowledgements
 
-AIX Rules is built with the help of several open source packages. All of these are listed in setup.py and some of these include:
+rulelearn is built with the help of several open source packages. All of these are listed in requirements.txt and include:
+
 * scikit-learn https://scikit-learn.org/stable/about.html
 
 ## License Information
 
-Please view both the [LICENSE](https://github.com/vijay-arya/AIX360/blob/master/LICENSE) file and the folder [supplementary license](https://github.com/vijay-arya/AIX360/tree/master/supplementary%20license) present in the root directory for license information. 
+Apache 2.0
```

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/r2n/base.py` & `rulelearn-0.1.1/rulelearn/algorithms/r2n/base.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/r2n/functions.py` & `rulelearn-0.1.1/rulelearn/algorithms/r2n/functions.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/r2n/mask.py` & `rulelearn-0.1.1/rulelearn/algorithms/r2n/mask.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/r2n/preprocessing_layers.py` & `rulelearn-0.1.1/rulelearn/algorithms/r2n/preprocessing_layers.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/r2n/r2n_algo.py` & `rulelearn-0.1.1/rulelearn/algorithms/r2n/r2n_algo.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/r2n/simple_rulenet.py` & `rulelearn-0.1.1/rulelearn/algorithms/r2n/simple_rulenet.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/r2n/training.py` & `rulelearn-0.1.1/rulelearn/algorithms/r2n/training.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/r2n/utilities.py` & `rulelearn-0.1.1/rulelearn/algorithms/r2n/utilities.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/rbm/boolean_rule_cg.py` & `rulelearn-0.1.1/rulelearn/algorithms/rbm/boolean_rule_cg.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/BRCG.py` & `rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/BRCG.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/GLRM.py` & `rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/GLRM.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/beam_search.py` & `rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/beam_search.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/boolean_rule_cg.py` & `rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/boolean_rule_cg.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/features.py` & `rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/features.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/linear_regression.py` & `rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/linear_regression.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/rbm/rbm/logistic_regression.py` & `rulelearn-0.1.1/rulelearn/algorithms/rbm/rbm/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/ripper/base.py` & `rulelearn-0.1.1/rulelearn/algorithms/ripper/base.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/ripper/binding.py` & `rulelearn-0.1.1/rulelearn/algorithms/ripper/binding.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/ripper/mdl.py` & `rulelearn-0.1.1/rulelearn/algorithms/ripper/mdl.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/ripper/pruning.py` & `rulelearn-0.1.1/rulelearn/algorithms/ripper/pruning.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/ripper/ripper.py` & `rulelearn-0.1.1/rulelearn/algorithms/ripper/ripper.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/algorithms/ripper/ripper_ruleset_generator.py` & `rulelearn-0.1.1/rulelearn/algorithms/ripper/ripper_ruleset_generator.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/dise.py` & `rulelearn-0.1.1/rulelearn/dise.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/classifier/ruleset_classifier.py` & `rulelearn-0.1.1/rulelearn/trxf/classifier/ruleset_classifier.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/core/conjunction.py` & `rulelearn-0.1.1/rulelearn/trxf/core/conjunction.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/core/dnf_ruleset.py` & `rulelearn-0.1.1/rulelearn/trxf/core/dnf_ruleset.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/core/feature.py` & `rulelearn-0.1.1/rulelearn/trxf/core/feature.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/core/predicate.py` & `rulelearn-0.1.1/rulelearn/trxf/core/predicate.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/core/ruleset_generator.py` & `rulelearn-0.1.1/rulelearn/trxf/core/ruleset_generator.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/core/utils.py` & `rulelearn-0.1.1/rulelearn/trxf/core/utils.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/metrics.py` & `rulelearn-0.1.1/rulelearn/trxf/metrics.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/__init__.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/attribute.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/attribute.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/data_dictionary.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/data_dictionary.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/mining_schema.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/mining_schema.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/predicate.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/predicate.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/rule.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/rule.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/ruleset.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/models/scorecard.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/models/scorecard.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/pmml_exporter.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/pmml_exporter.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/reader/trxf_reader.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/reader/trxf_reader.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/pmml_export/serializer/nyoka_serializer.py` & `rulelearn-0.1.1/rulelearn/trxf/pmml_export/serializer/nyoka_serializer.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/scorecard/bins.py` & `rulelearn-0.1.1/rulelearn/trxf/scorecard/bins.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/scorecard/partition.py` & `rulelearn-0.1.1/rulelearn/trxf/scorecard/partition.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn/trxf/scorecard/scorecard.py` & `rulelearn-0.1.1/rulelearn/trxf/scorecard/scorecard.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/rulelearn.egg-info/PKG-INFO` & `rulelearn-0.1.1/rulelearn.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 Metadata-Version: 2.1
 Name: rulelearn
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package contains a rule induction toolkit to generate readable and editable rules from data.
 Home-page: https://github.com/IBM/rulelearn
 Author: Various
 Author-email: hvoelzer@acm.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rulelearn (v0.1)
 
-This package contains a rule induction toolkit to generate readable and editable rules from data. The code was
-originally released within the larger [AIX 360 package](https://github.com/Trusted-AI/AIX360) and is provided and 
-extended here separately with less dependencies.
+This package contains a rule induction toolkit to generate readable and editable rules from data. The code was originally released within the larger AIX 360 package and is provided and extended here separately with less dependencies.
 
 It contains the following components:
 
-- Boolean Decision Rules via Column Generation (Light Edition) ([Dash et al., 2018](https://papers.nips.cc/paper/7716-boolean-decision-rules-via-column-generation))
-- Generalized Linear Rule Models ([Wei et al., 2019](http://proceedings.mlr.press/v97/wei19a.html))
-- Fast Effective Rule Induction (Ripper) ([William W Cohen, 1995](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.107.2612&rep=rep1&type=pdf))
-- Relational Rule Network (R2N) ([Kusters et al., 2022](https://arxiv.org/abs/2201.06515))
-- trxf - Technical Rule Interchange Format - Rule Set Interchange providing common evaluation tools and PMML export for 
-rule sets.
+Boolean Decision Rules via Column Generation (Light Edition) (Dash et al., 2018)
+Generalized Linear Rule Models (Wei et al., 2019)
+Fast Effective Rule Induction (Ripper) (William W Cohen, 1995)
+Relational Rule Network (R2N) (Kusters et al., 2022)
+trxf - Technical Rule Interchange Format - Rule Set Interchange providing common evaluation tools and PMML export for rule sets.
 
 
 ### Installation
 
 ```
-pip install -r requirements.txt
+pip install rulelearn
 ```
-to be completed.
+
 
 
 ## Acknowledgements
 
-AIX Rules is built with the help of several open source packages. All of these are listed in setup.py and some of these include:
+rulelearn is built with the help of several open source packages. All of these are listed in requirements.txt and include:
+
 * scikit-learn https://scikit-learn.org/stable/about.html
 
 ## License Information
 
-Please view both the [LICENSE](https://github.com/vijay-arya/AIX360/blob/master/LICENSE) file and the folder [supplementary license](https://github.com/vijay-arya/AIX360/tree/master/supplementary%20license) present in the root directory for license information. 
+Apache 2.0
```

### Comparing `rulelearn-0.1.0/rulelearn.egg-info/SOURCES.txt` & `rulelearn-0.1.1/rulelearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/setup.py` & `rulelearn-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="rulelearn",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
     
         "pandas",
         "numpy",
         "scipy",
         "numba",
```

### Comparing `rulelearn-0.1.0/tests/r2n/test_preprocessing_layers.py` & `rulelearn-0.1.1/tests/r2n/test_preprocessing_layers.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/r2n/test_r2n_algo.py` & `rulelearn-0.1.1/tests/r2n/test_r2n_algo.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/r2n/test_simple_rulenet.py` & `rulelearn-0.1.1/tests/r2n/test_simple_rulenet.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/r2n/test_utilities.py` & `rulelearn-0.1.1/tests/r2n/test_utilities.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/rbm/test_Boolean_Rule_CG.py` & `rulelearn-0.1.1/tests/rbm/test_Boolean_Rule_CG.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/rbm/test_Feature_Binarizer_From_Trees.py` & `rulelearn-0.1.1/tests/rbm/test_Feature_Binarizer_From_Trees.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/rbm/test_Logistic_Rule_Regression.py` & `rulelearn-0.1.1/tests/rbm/test_Logistic_Rule_Regression.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/rbm/test_brcg.py` & `rulelearn-0.1.1/tests/rbm/test_brcg.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/ripper/test_base.py` & `rulelearn-0.1.1/tests/ripper/test_base.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/ripper/test_binding.py` & `rulelearn-0.1.1/tests/ripper/test_binding.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/ripper/test_ripper.py` & `rulelearn-0.1.1/tests/ripper/test_ripper.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/ripper/test_ripper_ruleset_generator.py` & `rulelearn-0.1.1/tests/ripper/test_ripper_ruleset_generator.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/classifier/test_ruleset_classifier.py` & `rulelearn-0.1.1/tests/trxf/classifier/test_ruleset_classifier.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/core/test_conjunction.py` & `rulelearn-0.1.1/tests/trxf/core/test_conjunction.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/core/test_dnfruleset.py` & `rulelearn-0.1.1/tests/trxf/core/test_dnfruleset.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/core/test_feature.py` & `rulelearn-0.1.1/tests/trxf/core/test_feature.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/core/test_predicate.py` & `rulelearn-0.1.1/tests/trxf/core/test_predicate.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/core/test_utils.py` & `rulelearn-0.1.1/tests/trxf/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/pmml_export/test_nyoka_serialize_common.py` & `rulelearn-0.1.1/tests/trxf/pmml_export/test_nyoka_serialize_common.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/pmml_export/test_nyoka_serialize_integration.py` & `rulelearn-0.1.1/tests/trxf/pmml_export/test_nyoka_serialize_integration.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/pmml_export/test_nyoka_serialize_ruleset.py` & `rulelearn-0.1.1/tests/trxf/pmml_export/test_nyoka_serialize_ruleset.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/pmml_export/test_nyoka_serialize_scorecard.py` & `rulelearn-0.1.1/tests/trxf/pmml_export/test_nyoka_serialize_scorecard.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/pmml_export/test_pmml_exporter.py` & `rulelearn-0.1.1/tests/trxf/pmml_export/test_pmml_exporter.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/pmml_export/test_trxf_reader.py` & `rulelearn-0.1.1/tests/trxf/pmml_export/test_trxf_reader.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/scorecard/test_bins.py` & `rulelearn-0.1.1/tests/trxf/scorecard/test_bins.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/scorecard/test_partition.py` & `rulelearn-0.1.1/tests/trxf/scorecard/test_partition.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/scorecard/test_scorecard.py` & `rulelearn-0.1.1/tests/trxf/scorecard/test_scorecard.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/test_metrics.py` & `rulelearn-0.1.1/tests/trxf/test_metrics.py`

 * *Files identical despite different names*

### Comparing `rulelearn-0.1.0/tests/trxf/utilities.py` & `rulelearn-0.1.1/tests/trxf/utilities.py`

 * *Files identical despite different names*

