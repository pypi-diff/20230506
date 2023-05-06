# Comparing `tmp/scikit_mol-0.2.0.tar.gz` & `tmp/scikit_mol-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_mol-0.2.0.tar", last modified: Sun Apr 30 08:56:11 2023, max compression
+gzip compressed data, was "scikit_mol-0.2.1.tar", last modified: Sat May  6 05:39:39 2023, max compression
```

## Comparing `scikit_mol-0.2.0.tar` & `scikit_mol-0.2.1.tar`

### file list

```diff
@@ -1,76 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.658783 scikit_mol-0.2.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/01_basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/01_basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    40949 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/02_descriptor_transformer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/02_descriptor_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.658783 scikit_mol-0.2.0/notebooks/02_descriptor_transformer_files/
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/03_example_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/03_example_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    30287 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/04_standardizer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/04_standardizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.658783 scikit_mol-0.2.0/notebooks/04_standardizer_files/
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/04_standardizer_files/04_standardizer_3_0.png
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/04_standardizer_files/04_standardizer_3_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/05_smiles_sanitaztion.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/05_smiles_sanitaztion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19466 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/06_hyperparameter_tuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/06_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/07_parallel_transforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/07_parallel_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/08_external_library_skopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.662783 scikit_mol-0.2.0/notebooks/images/
--rw-r--r--   0 runner    (1001) docker     (123)    66320 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/AtomPairFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60999 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/AtomPairFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    64259 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/Desc2DTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    58977 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/Desc2DTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    66054 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/MACCSTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60534 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/MACCSTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    65268 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/MorganTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    59856 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/MorganTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    65110 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/RDKitFPTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60176 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/RDKitFPTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    64025 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/SECFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60783 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/SECFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68278 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
--rw-r--r--   0 runner    (1001) docker     (123)    60915 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/Transformer_Widget.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    52959 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/max_speedup_vs_throughput.png
--rw-r--r--   0 runner    (1001) docker     (123)    46854 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/images/max_speedup_vs_throughput.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/pair_notebook.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/run_notebooks.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/notebooks/sync_notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.662783 scikit_mol-0.2.0/scikit_mol/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21524 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/scikit_mol/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.662783 scikit_mol-0.2.0/scikit_mol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 08:56:11.000000 scikit_mol-0.2.0/scikit_mol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:56:11.666782 scikit_mol-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/data/SLC6A4_active_excapedb_subset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_desctransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_fptransformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_parameter_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_scikit_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_smilestomol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-30 08:56:00.000000 scikit_mol-0.2.0/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.268298 scikit_mol-0.2.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/01_basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/01_basic_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40949 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/02_descriptor_transformer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/02_descriptor_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.268298 scikit_mol-0.2.1/notebooks/02_descriptor_transformer_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/03_example_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/03_example_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30287 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/04_standardizer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/04_standardizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.268298 scikit_mol-0.2.1/notebooks/04_standardizer_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/04_standardizer_files/04_standardizer_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/04_standardizer_files/04_standardizer_3_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/05_smiles_sanitaztion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/05_smiles_sanitaztion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19466 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/06_hyperparameter_tuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/06_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/07_parallel_transforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/07_parallel_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/08_external_library_skopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.272298 scikit_mol-0.2.1/notebooks/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    66320 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/AtomPairFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60999 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/AtomPairFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    64259 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/Desc2DTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58977 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/Desc2DTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    66054 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/MACCSTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60534 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/MACCSTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    65268 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/MorganTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59856 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/MorganTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    65110 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/RDKitFPTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60176 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/RDKitFPTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    64025 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/SECFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60783 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/SECFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68278 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60915 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/Transformer_Widget.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    52959 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/max_speedup_vs_throughput.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46854 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/images/max_speedup_vs_throughput.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/pair_notebook.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/run_notebooks.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/notebooks/sync_notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.264298 scikit_mol-0.2.1/ressources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.276298 scikit_mol-0.2.1/ressources/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)  1389097 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo.ai
+-rw-r--r--   0 runner    (1001) docker     (123)    70075 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33144 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG_300px.png
+-rw-r--r--   0 runner    (1001) docker     (123)   150544 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66674 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30449 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG_300px.png
+-rw-r--r--   0 runner    (1001) docker     (123)   143920 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/ressources/logo/ScikitMol_Logo_LightBG_600dpi.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.276298 scikit_mol-0.2.1/scikit_mol/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/scikit_mol/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/scikit_mol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 05:39:39.000000 scikit_mol-0.2.1/scikit_mol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:39:39.280298 scikit_mol-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/data/SLC6A4_active_excapedb_subset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_desctransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_fptransformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_scikit_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_smilestomol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-06 05:39:23.000000 scikit_mol-0.2.1/tests/test_transformers.py
```

### Comparing `scikit_mol-0.2.0/LICENSE` & `scikit_mol-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/PKG-INFO` & `scikit_mol-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_mol
-Version: 0.2.0
+Version: 0.2.1
 Summary: scikit-learn classes for molecule transformation
 Home-page: https://github.com/EBjerrum/scikit-mol
 Download-URL: https://github.com/EBjerrum/scikit-mol
 Author: Esben Jannik Bjerrum
 Author-email: esben@cheminformania.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
@@ -24,16 +24,17 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # scikit-mol
-
-Scikit-Learn classes for molecular vectorization using RDKit
+![Fancy logo](./ressources/logo/ScikitMol_Logo_DarkBG_300px.png#gh-dark-mode-only)
+![Fancy logo](./ressources/logo/ScikitMol_Logo_LightBG_300px.png#gh-light-mode-only)
+## Scikit-Learn classes for molecular vectorization using RDKit
 
 The intended usage is to be able to add molecular vectorization directly into scikit-learn pipelines, so that the final model directly predict on RDKit molecules or SMILES strings
 
 As example with the needed scikit-learn and -mol imports and RDKit mol objects in the mol_list_train and _test lists:
 
     pipe = Pipeline([('mol_transformer', MorganTransformer()), ('Regressor', Ridge())])
     pipe.fit(mol_list_train, y_train)
@@ -44,28 +45,37 @@
 
 The scikit-learn compatibility should also make it easier to include the fingerprinting step in hyperparameter tuning with scikit-learns utilities
 
 The first draft for the project was created at the [RDKIT UGM 2022 hackathon](https://github.com/rdkit/UGM_2022) 2022-October-14
 
 
 ## Implemented
-* Transformer Classes
-    * SmilesToMol
-    * Desc2DTransformer
-    * MACCSTransformer
-    * RDKitFPTransformer
+* descriptors
+    * MolecularDescriptorTransformer
+<br>
+* fingerprints
+    * MorganFingerprintTransformer
+    * MACCSKeysFingerprintTransformer
+    * RDKitFingerprintTransformer
     * AtomPairFingerprintTransformer
     * TopologicalTorsionFingerprintTransformer
-    * MorganTransformer
+    * MHFingerprintTransformer
     * SECFingerprintTransformer
+    * AvalonFingerprintTransformer
 <br>
-
-* Utilities
+* conversions
+    * SmilesToMol
+<br>
+* standardizer
+    * Standardizer
+<br>
+* utilities
     * CheckSmilesSanitazion
 
+
 ## Installation
 Users can install latest tagged release from pip
 
     pip install scikit-mol
 
 Bleeding edge
```

### Comparing `scikit_mol-0.2.0/README.md` & `scikit_mol-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # scikit-mol
-
-Scikit-Learn classes for molecular vectorization using RDKit
+![Fancy logo](./ressources/logo/ScikitMol_Logo_DarkBG_300px.png#gh-dark-mode-only)
+![Fancy logo](./ressources/logo/ScikitMol_Logo_LightBG_300px.png#gh-light-mode-only)
+## Scikit-Learn classes for molecular vectorization using RDKit
 
 The intended usage is to be able to add molecular vectorization directly into scikit-learn pipelines, so that the final model directly predict on RDKit molecules or SMILES strings
 
 As example with the needed scikit-learn and -mol imports and RDKit mol objects in the mol_list_train and _test lists:
 
     pipe = Pipeline([('mol_transformer', MorganTransformer()), ('Regressor', Ridge())])
     pipe.fit(mol_list_train, y_train)
@@ -15,28 +16,37 @@
 
 The scikit-learn compatibility should also make it easier to include the fingerprinting step in hyperparameter tuning with scikit-learns utilities
 
 The first draft for the project was created at the [RDKIT UGM 2022 hackathon](https://github.com/rdkit/UGM_2022) 2022-October-14
 
 
 ## Implemented
-* Transformer Classes
-    * SmilesToMol
-    * Desc2DTransformer
-    * MACCSTransformer
-    * RDKitFPTransformer
+* descriptors
+    * MolecularDescriptorTransformer
+<br>
+* fingerprints
+    * MorganFingerprintTransformer
+    * MACCSKeysFingerprintTransformer
+    * RDKitFingerprintTransformer
     * AtomPairFingerprintTransformer
     * TopologicalTorsionFingerprintTransformer
-    * MorganTransformer
+    * MHFingerprintTransformer
     * SECFingerprintTransformer
+    * AvalonFingerprintTransformer
 <br>
-
-* Utilities
+* conversions
+    * SmilesToMol
+<br>
+* standardizer
+    * Standardizer
+<br>
+* utilities
     * CheckSmilesSanitazion
 
+
 ## Installation
 Users can install latest tagged release from pip
 
     pip install scikit-mol
 
 Bleeding edge
```

### Comparing `scikit_mol-0.2.0/notebooks/01_basic_usage.ipynb` & `scikit_mol-0.2.1/notebooks/01_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/01_basic_usage.py` & `scikit_mol-0.2.1/notebooks/01_basic_usage.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/02_descriptor_transformer.ipynb` & `scikit_mol-0.2.1/notebooks/02_descriptor_transformer.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/02_descriptor_transformer.py` & `scikit_mol-0.2.1/notebooks/02_descriptor_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png` & `scikit_mol-0.2.1/notebooks/02_descriptor_transformer_files/02_descriptor_transformer_5_0.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/03_example_pipeline.ipynb` & `scikit_mol-0.2.1/notebooks/03_example_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/03_example_pipeline.py` & `scikit_mol-0.2.1/notebooks/03_example_pipeline.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/04_standardizer.ipynb` & `scikit_mol-0.2.1/notebooks/04_standardizer.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/04_standardizer.py` & `scikit_mol-0.2.1/notebooks/04_standardizer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/04_standardizer_files/04_standardizer_3_0.png` & `scikit_mol-0.2.1/notebooks/04_standardizer_files/04_standardizer_3_0.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/04_standardizer_files/04_standardizer_3_1.png` & `scikit_mol-0.2.1/notebooks/04_standardizer_files/04_standardizer_3_1.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/05_smiles_sanitaztion.ipynb` & `scikit_mol-0.2.1/notebooks/05_smiles_sanitaztion.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/05_smiles_sanitaztion.py` & `scikit_mol-0.2.1/notebooks/05_smiles_sanitaztion.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/06_hyperparameter_tuning.ipynb` & `scikit_mol-0.2.1/notebooks/06_hyperparameter_tuning.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/06_hyperparameter_tuning.py` & `scikit_mol-0.2.1/notebooks/06_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/07_parallel_transforms.ipynb` & `scikit_mol-0.2.1/notebooks/07_parallel_transforms.ipynb`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/07_parallel_transforms.py` & `scikit_mol-0.2.1/notebooks/07_parallel_transforms.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/08_external_library_skopt.py` & `scikit_mol-0.2.1/notebooks/08_external_library_skopt.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/README.md` & `scikit_mol-0.2.1/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/AtomPairFingerprintTransformer_par.png` & `scikit_mol-0.2.1/notebooks/images/AtomPairFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/AtomPairFingerprintTransformer_par.svg` & `scikit_mol-0.2.1/notebooks/images/AtomPairFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/Desc2DTransformer_par.png` & `scikit_mol-0.2.1/notebooks/images/Desc2DTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/Desc2DTransformer_par.svg` & `scikit_mol-0.2.1/notebooks/images/Desc2DTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/MACCSTransformer_par.png` & `scikit_mol-0.2.1/notebooks/images/MACCSTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/MACCSTransformer_par.svg` & `scikit_mol-0.2.1/notebooks/images/MACCSTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/MorganTransformer_par.png` & `scikit_mol-0.2.1/notebooks/images/MorganTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/MorganTransformer_par.svg` & `scikit_mol-0.2.1/notebooks/images/MorganTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/RDKitFPTransformer_par.png` & `scikit_mol-0.2.1/notebooks/images/RDKitFPTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/RDKitFPTransformer_par.svg` & `scikit_mol-0.2.1/notebooks/images/RDKitFPTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/SECFingerprintTransformer_par.png` & `scikit_mol-0.2.1/notebooks/images/SECFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/SECFingerprintTransformer_par.svg` & `scikit_mol-0.2.1/notebooks/images/SECFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png` & `scikit_mol-0.2.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg` & `scikit_mol-0.2.1/notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/Transformer_Widget.jpg` & `scikit_mol-0.2.1/notebooks/images/Transformer_Widget.jpg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/max_speedup_vs_throughput.png` & `scikit_mol-0.2.1/notebooks/images/max_speedup_vs_throughput.png`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/notebooks/images/max_speedup_vs_throughput.svg` & `scikit_mol-0.2.1/notebooks/images/max_speedup_vs_throughput.svg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/scikit_mol/conversions.py` & `scikit_mol-0.2.1/scikit_mol/conversions.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/scikit_mol/descriptors.py` & `scikit_mol-0.2.1/scikit_mol/descriptors.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/scikit_mol/fingerprints.py` & `scikit_mol-0.2.1/scikit_mol/fingerprints.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Union
 from rdkit import Chem
 from rdkit import DataStructs
 #from rdkit.Chem.AllChem import GetMorganFingerprintAsBitVect
 from rdkit.Chem import rdMolDescriptors
 from rdkit.Chem import rdFingerprintGenerator
 from rdkit.Chem import rdMHFPFingerprint
+from rdkit.Avalon import pyAvalonTools
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import lil_matrix
 from scipy.sparse import vstack
 
 from sklearn.base import BaseEstimator, TransformerMixin
@@ -444,15 +445,53 @@
             )
         else:
             return rdMolDescriptors.GetMorganFingerprintAsBitVect(
                 mol,int(self.radius),nBits=int(self.nBits), useFeatures=bool(self.useFeatures),
                 useChirality=bool(self.useChirality), useBondTypes=bool(self.useBondTypes)
             )
         
+class AvalonFingerprintTransformer(FpsTransformer):
+    # Fingerprint from the Avalon toolkeit, https://doi.org/10.1021/ci050413p
+    def __init__(self, nBits:int = 512, isQuery:bool = False, resetVect:bool = False, bitFlags:int = 15761407, useCounts:bool = False, parallel: Union[bool, int] = False,):
+        """ Transform RDKit mols into Count or bit-based Avalon Fingerprints
 
+        Parameters
+        ----------
+        nBits : int, optional
+            Size of the fingerprint, by default 512
+        isQuery : bool, optional
+            use the fingerprint for a query structure, by default False
+        resetVect : bool, optional
+            reset vector, by default False      NB: only used in GetAvalonFP (not for GetAvalonCountFP)
+        bitFlags : int, optional
+            Substructure fingerprint (32767) or similarity fingerprint (15761407) by default 15761407
+        useCounts : bool, optional
+            If toggled will create the count and not bit-based fingerprint, by default False
+        """
+        super().__init__(parallel = parallel)
+        self.nBits = nBits
+        self.isQuery = isQuery
+        self.resetVect = resetVect
+        self.bitFlags = bitFlags
+        self.useCounts = useCounts
+        
+    def _mol2fp(self, mol):
+        if self.useCounts:
+            return pyAvalonTools.GetAvalonCountFP(mol,
+                                                  nBits=int(self.nBits),
+                                                  isQuery=bool(self.isQuery),
+                                                  bitFlags=int(self.bitFlags)
+            )
+        else:
+            return pyAvalonTools.GetAvalonFP(mol,
+                                             nBits=int(self.nBits),
+                                             isQuery=bool(self.isQuery),
+                                             resetVect=bool(self.resetVect),
+                                             bitFlags=int(self.bitFlags)                      
+            )
 
 
 def parallel_helper(args):
     """Parallel_helper takes a tuple with classname, the objects parameters and the mols to process.
     Then instantiates the class with the parameters and processes the mol.
     Intention is to be able to do this in chilcprocesses as some classes can't be pickled"""
     classname, parameters, X_mols = args
```

### Comparing `scikit_mol-0.2.0/scikit_mol/standardizer.py` & `scikit_mol-0.2.1/scikit_mol/standardizer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/scikit_mol/utilities.py` & `scikit_mol-0.2.1/scikit_mol/utilities.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/scikit_mol.egg-info/PKG-INFO` & `scikit_mol-0.2.1/scikit_mol.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-mol
-Version: 0.2.0
+Version: 0.2.1
 Summary: scikit-learn classes for molecule transformation
 Home-page: https://github.com/EBjerrum/scikit-mol
 Download-URL: https://github.com/EBjerrum/scikit-mol
 Author: Esben Jannik Bjerrum
 Author-email: esben@cheminformania.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
@@ -24,16 +24,17 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # scikit-mol
-
-Scikit-Learn classes for molecular vectorization using RDKit
+![Fancy logo](./ressources/logo/ScikitMol_Logo_DarkBG_300px.png#gh-dark-mode-only)
+![Fancy logo](./ressources/logo/ScikitMol_Logo_LightBG_300px.png#gh-light-mode-only)
+## Scikit-Learn classes for molecular vectorization using RDKit
 
 The intended usage is to be able to add molecular vectorization directly into scikit-learn pipelines, so that the final model directly predict on RDKit molecules or SMILES strings
 
 As example with the needed scikit-learn and -mol imports and RDKit mol objects in the mol_list_train and _test lists:
 
     pipe = Pipeline([('mol_transformer', MorganTransformer()), ('Regressor', Ridge())])
     pipe.fit(mol_list_train, y_train)
@@ -44,28 +45,37 @@
 
 The scikit-learn compatibility should also make it easier to include the fingerprinting step in hyperparameter tuning with scikit-learns utilities
 
 The first draft for the project was created at the [RDKIT UGM 2022 hackathon](https://github.com/rdkit/UGM_2022) 2022-October-14
 
 
 ## Implemented
-* Transformer Classes
-    * SmilesToMol
-    * Desc2DTransformer
-    * MACCSTransformer
-    * RDKitFPTransformer
+* descriptors
+    * MolecularDescriptorTransformer
+<br>
+* fingerprints
+    * MorganFingerprintTransformer
+    * MACCSKeysFingerprintTransformer
+    * RDKitFingerprintTransformer
     * AtomPairFingerprintTransformer
     * TopologicalTorsionFingerprintTransformer
-    * MorganTransformer
+    * MHFingerprintTransformer
     * SECFingerprintTransformer
+    * AvalonFingerprintTransformer
 <br>
-
-* Utilities
+* conversions
+    * SmilesToMol
+<br>
+* standardizer
+    * Standardizer
+<br>
+* utilities
     * CheckSmilesSanitazion
 
+
 ## Installation
 Users can install latest tagged release from pip
 
     pip install scikit-mol
 
 Bleeding edge
```

### Comparing `scikit_mol-0.2.0/scikit_mol.egg-info/SOURCES.txt` & `scikit_mol-0.2.1/scikit_mol.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,21 @@
 notebooks/images/SECFingerprintTransformer_par.png
 notebooks/images/SECFingerprintTransformer_par.svg
 notebooks/images/TopologicalTorsionFingerprintTransformer_par.png
 notebooks/images/TopologicalTorsionFingerprintTransformer_par.svg
 notebooks/images/Transformer_Widget.jpg
 notebooks/images/max_speedup_vs_throughput.png
 notebooks/images/max_speedup_vs_throughput.svg
+ressources/logo/ScikitMol_Logo.ai
+ressources/logo/ScikitMol_Logo_DarkBG.png
+ressources/logo/ScikitMol_Logo_DarkBG_300px.png
+ressources/logo/ScikitMol_Logo_DarkBG_600dpi.png
+ressources/logo/ScikitMol_Logo_LightBG.png
+ressources/logo/ScikitMol_Logo_LightBG_300px.png
+ressources/logo/ScikitMol_Logo_LightBG_600dpi.png
 scikit_mol/__init__.py
 scikit_mol/_version.py
 scikit_mol/conversions.py
 scikit_mol/descriptors.py
 scikit_mol/fingerprints.py
 scikit_mol/standardizer.py
 scikit_mol/utilities.py
```

### Comparing `scikit_mol-0.2.0/setup.cfg` & `scikit_mol-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/tests/conftest.py` & `scikit_mol-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/tests/data/SLC6A4_active_excapedb_subset.csv` & `scikit_mol-0.2.1/tests/data/SLC6A4_active_excapedb_subset.csv`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/tests/fixtures.py` & `scikit_mol-0.2.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/tests/test_desctransformer.py` & `scikit_mol-0.2.1/tests/test_desctransformer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/tests/test_fptransformers.py` & `scikit_mol-0.2.1/tests/test_fptransformers.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 import numpy as np
 import pandas as pd
 from rdkit import Chem
 from fixtures import mols_list, smiles_list, fingerprint, chiral_smiles_list, chiral_mols_list
 from sklearn import clone
 
-from scikit_mol.fingerprints import MorganFingerprintTransformer, MACCSKeysFingerprintTransformer, RDKitFingerprintTransformer, AtomPairFingerprintTransformer, TopologicalTorsionFingerprintTransformer, SECFingerprintTransformer, MHFingerprintTransformer
+from scikit_mol.fingerprints import MorganFingerprintTransformer, MACCSKeysFingerprintTransformer, RDKitFingerprintTransformer, AtomPairFingerprintTransformer, TopologicalTorsionFingerprintTransformer, SECFingerprintTransformer, MHFingerprintTransformer, AvalonFingerprintTransformer
 
 
 
 @pytest.fixture
 def morgan_transformer():
     return MorganFingerprintTransformer()
 
@@ -35,14 +35,17 @@
 def secfp_transformer():
     return SECFingerprintTransformer()
 
 @pytest.fixture
 def mhfp_transformer():
     return MHFingerprintTransformer()
 
+@pytest.fixture
+def avalon_transformer():
+    return AvalonFingerprintTransformer()
 
 def test_fpstransformer_fp2array(morgan_transformer, fingerprint):
     fp = morgan_transformer._fp2array(fingerprint)
     #See that fp is the correct type, shape and bit count
     assert(type(fp) == type(np.array([0])))
     assert(fp.shape == (1000,))
     assert(fp.sum() == 25)
@@ -50,26 +53,26 @@
 def test_fpstransformer_transform_mol(morgan_transformer, mols_list):
     fp = morgan_transformer._transform_mol(mols_list[0])
     #See that fp is the correct type, shape and bit count
     assert(type(fp) == type(np.array([0])))
     assert(fp.shape == (2048,))
     assert(fp.sum() == 14)
 
-def test_clonability(maccs_transformer, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer):
-    for t in [maccs_transformer, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer]:
+def test_clonability(maccs_transformer, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer, avalon_transformer):
+    for t in [maccs_transformer, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer, avalon_transformer]:
         params   = t.get_params()
         t2 = clone(t)
         params_2 = t2.get_params()
         #Parameters of cloned transformers should be the same
         assert all([ params[key] == params_2[key] for key in params.keys()])
         #Cloned transformers should not be the same object
         assert t2 != t
 
-def test_set_params(morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer):
-    for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer]:
+def test_set_params(morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, secfp_transformer, mhfp_transformer, avalon_transformer):
+    for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, avalon_transformer]:
         params   = t.get_params()
         #change extracted dictionary
         params['nBits'] = 4242
         #change params in transformer
         t.set_params(nBits = 4242)
         # get parameters as dictionary and assert that it is the same
         params_2 = t.get_params()
@@ -92,19 +95,19 @@
     for t in [mhfp_transformer]:
         params   = t.get_params()
         params['n_permutations'] = 4242
         t.set_params(n_permutations = 4242)
         params_2 = t.get_params()
         assert all([ params[key] == params_2[key] for key in params.keys()])
 
-def test_transform(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer):
+def test_transform(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer, avalon_transformer):
     #Test different types of input
     for mols in [mols_list, np.array(mols_list), pd.Series(mols_list)]:
         #Test the different transformers
-        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer]:
+        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer, avalon_transformer]:
             params   = t.get_params()
             fps = t.transform(mols)
             #Assert that the same length of input and output
             assert len(fps) == len(mols_list)
 
             # assert that the size of the fingerprint is the expected size
             if type(t) == type(maccs_transformer) or type(t) == type(secfp_transformer) or type(t) == type(mhfp_transformer):
@@ -112,19 +115,19 @@
             elif type(t) == type(rdkit_transformer):
                 fpsize = params['fpSize']
             else:
                 fpsize = params['nBits']
             
             assert len(fps[0]) == fpsize
 
-def test_transform_parallel(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer):
+def test_transform_parallel(mols_list, morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, mhfp_transformer, avalon_transformer):
     #Test different types of input
     for mols in [mols_list, np.array(mols_list), pd.Series(mols_list)]:
         #Test the different transformers
-        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer]:
+        for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, mhfp_transformer, avalon_transformer]:
             t.set_params(parallel=True)
             params   = t.get_params()
             fps = t.transform(mols)
             #Assert that the same length of input and output
             assert len(fps) == len(mols_list)
 
             # assert that the size of the fingerprint is the expected size
@@ -134,17 +137,17 @@
                 fpsize = params['fpSize']
             else:
                 fpsize = params['nBits']
             
             assert len(fps[0]) == fpsize
 
 
-def test_picklable(morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer):
+def test_picklable(morgan_transformer, rdkit_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, secfp_transformer, avalon_transformer):
     #Test the different transformers
-    for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer]:
+    for t in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, maccs_transformer, rdkit_transformer, secfp_transformer, avalon_transformer]:
         with tempfile.NamedTemporaryFile() as f:
             pickle.dump(t, f)
             f.seek(0)
             t2 = pickle.load(f)
             assert(t.get_params() == t2.get_params())
         
 
@@ -244,8 +247,14 @@
                 'kekulize': True,
                 'min_radius': 2,
                 'n_permutations': 4096, 
                 'seed': 44
                 }
     assert_transformer_set_params(MHFingerprintTransformer, new_params, chiral_mols_list)
 
-
+def test_AvalonFingerprintTransformer(chiral_mols_list):
+    new_params = {'nBits': 1024,
+                'isQuery': True,
+                # 'resetVect': True, #TODO: this doesn't change the FP
+                'bitFlags': 32767
+                }
+    assert_transformer_set_params(AvalonFingerprintTransformer, new_params, chiral_mols_list)
```

### Comparing `scikit_mol-0.2.0/tests/test_parameter_types.py` & `scikit_mol-0.2.1/tests/test_parameter_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 import numpy as np
 from rdkit import Chem
 from fixtures import mols_list, smiles_list
-from test_fptransformers import morgan_transformer, atompair_transformer, topologicaltorsion_transformer, rdkit_transformer
+from test_fptransformers import morgan_transformer, atompair_transformer, topologicaltorsion_transformer, rdkit_transformer, avalon_transformer
 
 
-def test_Transformer_exotic_types(mols_list, morgan_transformer,atompair_transformer, topologicaltorsion_transformer):
-    for transformer in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer]:
+def test_Transformer_exotic_types(mols_list, morgan_transformer,atompair_transformer, topologicaltorsion_transformer, avalon_transformer):
+    for transformer in [morgan_transformer, atompair_transformer, topologicaltorsion_transformer, avalon_transformer]:
         params = transformer.get_params()
 
         for useCounts in [np.bool_(True), np.bool_(False)]:
             
             for key, value in params.items():
                 if isinstance(value, int):
                     exotic_type_value = np.int64(value)
```

### Comparing `scikit_mol-0.2.0/tests/test_sanitizer.py` & `scikit_mol-0.2.1/tests/test_sanitizer.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/tests/test_smilestomol.py` & `scikit_mol-0.2.1/tests/test_smilestomol.py`

 * *Files identical despite different names*

### Comparing `scikit_mol-0.2.0/tests/test_transformers.py` & `scikit_mol-0.2.1/tests/test_transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pytest
 import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.ensemble import RandomForestRegressor
 from scikit_mol.conversions import SmilesToMolTransformer
 from scikit_mol.fingerprints import MACCSKeysFingerprintTransformer, RDKitFingerprintTransformer, AtomPairFingerprintTransformer, \
                                     TopologicalTorsionFingerprintTransformer, MorganFingerprintTransformer, SECFingerprintTransformer, \
-                                    MHFingerprintTransformer
+                                    MHFingerprintTransformer, AvalonFingerprintTransformer
 
 
 from fixtures import SLC6A4_subset
 
 def test_transformer(SLC6A4_subset):
     # load some toy data for quick testing on a small number of samples
     X_smiles, Y = SLC6A4_subset.SMILES, SLC6A4_subset.pXC50
@@ -30,15 +30,16 @@
                "AtomPairFingerprintTransformer": [AtomPairFingerprintTransformer, False],
                "AtomPairFingerprintTransformer useCounts": [AtomPairFingerprintTransformer, True],
                "TopologicalTorsionFingerprintTransformer": [TopologicalTorsionFingerprintTransformer, False],
                "TopologicalTorsionFingerprintTransformer useCounts": [TopologicalTorsionFingerprintTransformer, True],
                "MorganTransformer": [MorganFingerprintTransformer, False],
                "MorganTransformer useCounts": [MorganFingerprintTransformer, True],
                "SECFingerprintTransformer": [SECFingerprintTransformer, None],
-               "MHFingerprintTransformer": [MHFingerprintTransformer, None]}
+               "MHFingerprintTransformer": [MHFingerprintTransformer, None],
+               'AvalonFingerprintTransformer': [AvalonFingerprintTransformer, None]}
 
     # fit on toy data and print train/test score if successful or collect the failed FP
     failed_FP = []
     for FP_name, (FP, useCounts) in FP_dict.items():
         try:
             print(f"\nrunning pipeline fitting and scoring for {FP_name} with useCounts={useCounts}")
             if useCounts is None:
```

