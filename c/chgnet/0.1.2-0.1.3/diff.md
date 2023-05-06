# Comparing `tmp/chgnet-0.1.2.tar.gz` & `tmp/chgnet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chgnet-0.1.2.tar", last modified: Fri May  5 22:12:35 2023, max compression
+gzip compressed data, was "chgnet-0.1.3.tar", last modified: Sat May  6 09:35:08 2023, max compression
```

## Comparing `chgnet-0.1.2.tar` & `chgnet-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.082391 chgnet-0.1.2/
--rw-r--r--   0 bowendeng   (501) staff       (20)     2519 2023-02-23 00:52:46.000000 chgnet-0.1.2/LICENSE
--rw-r--r--   0 bowendeng   (501) staff       (20)    10656 2023-05-05 22:12:35.082156 chgnet-0.1.2/PKG-INFO
--rwxr-xr-x   0 bowendeng   (501) staff       (20)     9653 2023-05-05 22:10:13.000000 chgnet-0.1.2/README.md
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.073807 chgnet-0.1.2/chgnet/
--rw-r--r--   0 bowendeng   (501) staff       (20)      470 2023-03-28 22:55:28.000000 chgnet-0.1.2/chgnet/__init__.py
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.074837 chgnet-0.1.2/chgnet/data/
--rw-r--r--   0 bowendeng   (501) staff       (20)        0 2022-07-14 20:30:48.000000 chgnet-0.1.2/chgnet/data/__init__.py
--rw-r--r--   0 bowendeng   (501) staff       (20)    29046 2023-04-06 23:54:33.000000 chgnet-0.1.2/chgnet/data/dataset.py
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.075519 chgnet-0.1.2/chgnet/graph/
--rw-r--r--   0 bowendeng   (501) staff       (20)      197 2023-03-15 22:49:09.000000 chgnet-0.1.2/chgnet/graph/__init__.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     5813 2023-04-06 23:54:33.000000 chgnet-0.1.2/chgnet/graph/converter.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     6844 2023-03-29 20:46:04.000000 chgnet-0.1.2/chgnet/graph/crystalgraph.py
--rw-r--r--   0 bowendeng   (501) staff       (20)    13346 2023-03-29 09:36:58.000000 chgnet-0.1.2/chgnet/graph/graph.py
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.076601 chgnet-0.1.2/chgnet/model/
--rw-r--r--   0 bowendeng   (501) staff       (20)      243 2023-03-07 20:04:19.000000 chgnet-0.1.2/chgnet/model/__init__.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     6841 2023-04-25 22:26:43.000000 chgnet-0.1.2/chgnet/model/basis.py
--rw-r--r--   0 bowendeng   (501) staff       (20)    12947 2023-03-23 21:08:44.000000 chgnet-0.1.2/chgnet/model/composition_model.py
--rw-r--r--   0 bowendeng   (501) staff       (20)    20327 2023-04-20 21:41:19.000000 chgnet-0.1.2/chgnet/model/dynamics.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     5454 2023-03-30 00:52:39.000000 chgnet-0.1.2/chgnet/model/encoders.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     7244 2023-04-20 21:41:19.000000 chgnet-0.1.2/chgnet/model/functions.py
--rw-r--r--   0 bowendeng   (501) staff       (20)    16021 2023-04-18 00:42:11.000000 chgnet-0.1.2/chgnet/model/layers.py
--rw-r--r--   0 bowendeng   (501) staff       (20)    32417 2023-04-07 01:16:52.000000 chgnet-0.1.2/chgnet/model/model.py
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.076758 chgnet-0.1.2/chgnet/pretrained/
--rw-r--r--   0 bowendeng   (501) staff       (20)  4639235 2023-02-25 00:01:01.000000 chgnet-0.1.2/chgnet/pretrained/e30f77s348m32.pth.tar
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.080555 chgnet-0.1.2/chgnet/trainer/
--rw-r--r--   0 bowendeng   (501) staff       (20)      102 2023-03-07 20:04:19.000000 chgnet-0.1.2/chgnet/trainer/__init__.py
--rw-r--r--   0 bowendeng   (501) staff       (20)    26912 2023-04-20 21:41:19.000000 chgnet-0.1.2/chgnet/trainer/trainer.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     3437 2023-03-28 22:55:28.000000 chgnet-0.1.2/chgnet/utils.py
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.074586 chgnet-0.1.2/chgnet.egg-info/
--rw-r--r--   0 bowendeng   (501) staff       (20)    10656 2023-05-05 22:12:35.000000 chgnet-0.1.2/chgnet.egg-info/PKG-INFO
--rw-r--r--   0 bowendeng   (501) staff       (20)      885 2023-05-05 22:12:35.000000 chgnet-0.1.2/chgnet.egg-info/SOURCES.txt
--rw-r--r--   0 bowendeng   (501) staff       (20)        1 2023-05-05 22:12:35.000000 chgnet-0.1.2/chgnet.egg-info/dependency_links.txt
--rw-r--r--   0 bowendeng   (501) staff       (20)      134 2023-05-05 22:12:35.000000 chgnet-0.1.2/chgnet.egg-info/requires.txt
--rw-r--r--   0 bowendeng   (501) staff       (20)        7 2023-05-05 22:12:35.000000 chgnet-0.1.2/chgnet.egg-info/top_level.txt
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.080753 chgnet-0.1.2/examples/
--rw-r--r--   0 bowendeng   (501) staff       (20)     3380 2023-03-22 00:26:13.000000 chgnet-0.1.2/examples/make_graphs.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     2666 2023-05-05 22:11:12.000000 chgnet-0.1.2/pyproject.toml
--rw-r--r--   0 bowendeng   (501) staff       (20)       38 2023-05-05 22:12:35.082439 chgnet-0.1.2/setup.cfg
-drwxr-xr-x   0 bowendeng   (501) staff       (20)        0 2023-05-05 22:12:35.081965 chgnet-0.1.2/tests/
--rw-r--r--   0 bowendeng   (501) staff       (20)     3143 2023-04-06 23:54:33.000000 chgnet-0.1.2/tests/test_converter.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     6271 2023-03-29 20:47:40.000000 chgnet-0.1.2/tests/test_crystal_graph.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     2120 2023-05-04 06:17:34.000000 chgnet-0.1.2/tests/test_dataset.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     3580 2023-03-30 00:52:39.000000 chgnet-0.1.2/tests/test_encoders.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     3222 2023-05-04 06:16:22.000000 chgnet-0.1.2/tests/test_graph.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     3039 2023-04-01 01:29:27.000000 chgnet-0.1.2/tests/test_md.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     2049 2023-03-28 22:55:28.000000 chgnet-0.1.2/tests/test_model.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     1494 2023-03-28 22:55:28.000000 chgnet-0.1.2/tests/test_relaxation.py
--rw-r--r--   0 bowendeng   (501) staff       (20)     1530 2023-05-04 06:18:06.000000 chgnet-0.1.2/tests/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.189251 chgnet-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-06 09:34:58.000000 chgnet-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-06 09:35:08.189251 chgnet-0.1.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9380 2023-05-06 09:34:58.000000 chgnet-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/graph/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/graph/crystalgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/graph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/composition_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32417 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)  4639235 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/pretrained/e30f77s348m32.pth.tar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.185251 chgnet-0.1.3/chgnet/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26910 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/trainer/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-06 09:34:58.000000 chgnet-0.1.3/chgnet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.181251 chgnet-0.1.3/chgnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 09:35:08.000000 chgnet-0.1.3/chgnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-06 09:34:58.000000 chgnet-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 09:35:08.189251 chgnet-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:35:08.189251 chgnet-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_crystal_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-06 09:34:58.000000 chgnet-0.1.3/tests/test_trainer.py
```

### Comparing `chgnet-0.1.2/LICENSE` & `chgnet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/PKG-INFO` & `chgnet-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chgnet
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling
 Author-email: Bowen Deng <bowendeng@berkeley.edu>
 License: Modified BSD
 Project-URL: Source, https://github.com/CederGroupHub/chgnet
 Project-URL: Package, https://pypi.org/project/chgnet
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -52,26 +52,20 @@
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
-CHGnet is not on PyPI yet. We plan to publish it as a package once the API has matured. For now, please install `chgnet` from source:
+You can install `chgnet` through `pip`:
 
 ```sh
-pip install -U git+https://github.com/CederGroupHub/chgnet
+pip install chgnet
 ```
 
-or for an editable source install from a local clone:
-
-```sh
-git clone https://github.com/CederGroupHub/chgnet
-pip install -e ./chgnet
-```
 
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
```

### Comparing `chgnet-0.1.2/README.md` & `chgnet-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,20 @@
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
-CHGnet is not on PyPI yet. We plan to publish it as a package once the API has matured. For now, please install `chgnet` from source:
+You can install `chgnet` through `pip`:
 
 ```sh
-pip install -U git+https://github.com/CederGroupHub/chgnet
+pip install chgnet
 ```
 
-or for an editable source install from a local clone:
-
-```sh
-git clone https://github.com/CederGroupHub/chgnet
-pip install -e ./chgnet
-```
 
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
```

### Comparing `chgnet-0.1.2/chgnet/data/dataset.py` & `chgnet-0.1.3/chgnet/data/dataset.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/graph/converter.py` & `chgnet-0.1.3/chgnet/graph/converter.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/graph/crystalgraph.py` & `chgnet-0.1.3/chgnet/graph/crystalgraph.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/graph/graph.py` & `chgnet-0.1.3/chgnet/graph/graph.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/model/basis.py` & `chgnet-0.1.3/chgnet/model/basis.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/model/composition_model.py` & `chgnet-0.1.3/chgnet/model/composition_model.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/model/dynamics.py` & `chgnet-0.1.3/chgnet/model/dynamics.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/model/encoders.py` & `chgnet-0.1.3/chgnet/model/encoders.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/model/functions.py` & `chgnet-0.1.3/chgnet/model/functions.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/model/layers.py` & `chgnet-0.1.3/chgnet/model/layers.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/model/model.py` & `chgnet-0.1.3/chgnet/model/model.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/pretrained/e30f77s348m32.pth.tar` & `chgnet-0.1.3/chgnet/pretrained/e30f77s348m32.pth.tar`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet/trainer/trainer.py` & `chgnet-0.1.3/chgnet/trainer/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,17 +177,17 @@
         # mps is disabled until stable version of torch for mps is released
         # elif torch.backends.mps.is_available():
         #     self.device = "mps"
         else:
             self.device = "cpu"
 
         self.print_freq = print_freq
-        self.training_history = dict.fromkeys(
-            self.targets, {"train": [], "val": [], "test": []}
-        )
+        self.training_history = {
+            i: {"train": [], "val": [], "test": []} for i in self.targets
+        }
         self.best_model = None
 
     def train(
         self,
         train_loader: DataLoader,
         val_loader: DataLoader,
         test_loader: DataLoader = None,
```

### Comparing `chgnet-0.1.2/chgnet/utils.py` & `chgnet-0.1.3/chgnet/utils.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/chgnet.egg-info/PKG-INFO` & `chgnet-0.1.3/chgnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chgnet
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling
 Author-email: Bowen Deng <bowendeng@berkeley.edu>
 License: Modified BSD
 Project-URL: Source, https://github.com/CederGroupHub/chgnet
 Project-URL: Package, https://pypi.org/project/chgnet
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -52,26 +52,20 @@
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
-CHGnet is not on PyPI yet. We plan to publish it as a package once the API has matured. For now, please install `chgnet` from source:
+You can install `chgnet` through `pip`:
 
 ```sh
-pip install -U git+https://github.com/CederGroupHub/chgnet
+pip install chgnet
 ```
 
-or for an editable source install from a local clone:
-
-```sh
-git clone https://github.com/CederGroupHub/chgnet
-pip install -e ./chgnet
-```
 
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
```

### Comparing `chgnet-0.1.2/chgnet.egg-info/SOURCES.txt` & `chgnet-0.1.3/chgnet.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 chgnet/model/encoders.py
 chgnet/model/functions.py
 chgnet/model/layers.py
 chgnet/model/model.py
 chgnet/pretrained/e30f77s348m32.pth.tar
 chgnet/trainer/__init__.py
 chgnet/trainer/trainer.py
-examples/make_graphs.py
 tests/test_converter.py
 tests/test_crystal_graph.py
 tests/test_dataset.py
 tests/test_encoders.py
 tests/test_graph.py
 tests/test_md.py
 tests/test_model.py
```

### Comparing `chgnet-0.1.2/pyproject.toml` & `chgnet-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chgnet"
-version = "0.1.02"
+version = "0.1.03"
 description = "Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling"
 authors = [{ name = "Bowen Deng", email = "bowendeng@berkeley.edu" }]
 requires-python = ">=3.8"
 readme = "README.md"
 license = { text = "Modified BSD" }
 dependencies = [
     "numpy>=1.21.6",
```

### Comparing `chgnet-0.1.2/tests/test_converter.py` & `chgnet-0.1.3/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/tests/test_crystal_graph.py` & `chgnet-0.1.3/tests/test_crystal_graph.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/tests/test_dataset.py` & `chgnet-0.1.3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/tests/test_encoders.py` & `chgnet-0.1.3/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/tests/test_graph.py` & `chgnet-0.1.3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/tests/test_md.py` & `chgnet-0.1.3/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/tests/test_model.py` & `chgnet-0.1.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/tests/test_relaxation.py` & `chgnet-0.1.3/tests/test_relaxation.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.2/tests/test_trainer.py` & `chgnet-0.1.3/tests/test_trainer.py`

 * *Files 21% similar despite different names*

```diff
@@ -44,8 +44,12 @@
     )
     dir_name = "test_tmp_dir"
     test_dir = tmp_path / dir_name
     trainer.train(train_loader, val_loader, save_dir=test_dir)
     assert test_dir.is_dir(), "Training dir was not created"
 
     saved_weight = [f for f in test_dir.iterdir() if f.name.startswith("epoch")]
+    bestE_weight = [f for f in test_dir.iterdir() if f.name.startswith("bestE")]
+    bestF_weight = [f for f in test_dir.iterdir() if f.name.startswith("bestF")]
     assert len(saved_weight) == 1
+    assert len(bestE_weight) == 1
+    assert len(bestF_weight) == 1
```

