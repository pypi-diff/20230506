# Comparing `tmp/flatnet-0.1.0.tar.gz` & `tmp/flatnet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatnet-0.1.0.tar", last modified: Sat May  6 03:31:05 2023, max compression
+gzip compressed data, was "flatnet-0.1.1.tar", last modified: Fri May  5 21:55:11 2023, max compression
```

## Comparing `flatnet-0.1.0.tar` & `flatnet-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:31:05.475220 flatnet-0.1.0/
--rw-rw-rw-   0        0        0      277 2023-05-06 03:31:05.473218 flatnet-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2641 2023-05-05 20:45:34.000000 flatnet-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 03:31:05.399972 flatnet-0.1.0/flatnet/
--rw-rw-rw-   0        0        0       24 2023-05-06 03:00:44.000000 flatnet-0.1.0/flatnet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:31:05.429232 flatnet-0.1.0/flatnet/modules/
--rw-rw-rw-   0        0        0        0 2022-04-06 05:54:15.000000 flatnet-0.1.0/flatnet/modules/__init__.py
--rw-rw-rw-   0        0        0     3564 2023-05-05 20:51:08.000000 flatnet-0.1.0/flatnet/modules/flatnet_nn.py
--rw-rw-rw-   0        0        0    14157 2023-05-06 03:07:22.000000 flatnet-0.1.0/flatnet/train.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:31:05.423975 flatnet-0.1.0/flatnet.egg-info/
--rw-rw-rw-   0        0        0      277 2023-05-06 03:31:05.000000 flatnet-0.1.0/flatnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      668 2023-05-06 03:31:05.000000 flatnet-0.1.0/flatnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:31:05.000000 flatnet-0.1.0/flatnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      556 2023-05-06 03:31:05.000000 flatnet-0.1.0/flatnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-06 03:31:05.000000 flatnet-0.1.0/flatnet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 03:31:05.438218 flatnet-0.1.0/models/
--rw-rw-rw-   0        0        0        0 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/__init__.py
--rw-rw-rw-   0        0        0      410 2022-11-18 19:19:10.000000 flatnet-0.1.0/models/operators.py
--rw-rw-rw-   0        0        0      520 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/umap.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:31:05.458223 flatnet-0.1.0/models/umap_scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/umap_scripts/__init__.py
--rw-rw-rw-   0        0        0    36015 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/umap_scripts/distances.py
--rw-rw-rw-   0        0        0    34501 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/umap_scripts/layouts.py
--rw-rw-rw-   0        0        0    17347 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/umap_scripts/sparse.py
--rw-rw-rw-   0        0        0    12988 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/umap_scripts/spectral.py
--rw-rw-rw-   0        0        0   136753 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/umap_scripts/umap.py
--rw-rw-rw-   0        0        0     6896 2022-11-29 22:57:14.000000 flatnet-0.1.0/models/umap_scripts/utils.py
--rw-rw-rw-   0        0        0     8208 2022-11-21 18:44:42.000000 flatnet-0.1.0/models/vae.py
--rw-rw-rw-   0        0        0       42 2023-05-06 03:31:05.475220 flatnet-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1202 2023-05-06 03:31:01.000000 flatnet-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:31:05.471219 flatnet-0.1.0/tools/
--rw-rw-rw-   0        0        0        0 2022-04-06 05:54:39.000000 flatnet-0.1.0/tools/__init__.py
--rw-rw-rw-   0        0        0      608 2022-11-04 18:24:19.000000 flatnet-0.1.0/tools/gp_manifold_generator.py
--rw-rw-rw-   0        0        0     3433 2023-01-22 00:04:53.000000 flatnet-0.1.0/tools/manifold_generator.py
--rw-rw-rw-   0        0        0     3241 2022-10-28 03:06:50.000000 flatnet-0.1.0/tools/randman.py
--rw-rw-rw-   0        0        0        0 2022-03-31 21:46:28.000000 flatnet-0.1.0/tools/test_geodesics.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:25.978708 flatnet-0.1.1/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:10:25.963083 flatnet-0.1.1/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3012 2023-05-06 03:53:34.000000 flatnet-0.1.1/README.md
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:24.519713 flatnet-0.1.1/flatnet/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.1.1/flatnet/__init__.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:24.958895 flatnet-0.1.1/flatnet/modules/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.1.1/flatnet/modules/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.1.1/flatnet/modules/flatnet_nn.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    14293 2023-05-06 04:09:02.000000 flatnet-0.1.1/flatnet/train.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:24.818928 flatnet-0.1.1/flatnet.egg-info/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:10:23.000000 flatnet-0.1.1/flatnet.egg-info/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      668 2023-05-06 04:10:24.000000 flatnet-0.1.1/flatnet.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-06 04:10:23.000000 flatnet-0.1.1/flatnet.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      556 2023-05-06 04:10:23.000000 flatnet-0.1.1/flatnet.egg-info/requires.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       21 2023-05-06 04:10:23.000000 flatnet-0.1.1/flatnet.egg-info/top_level.txt
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:25.178467 flatnet-0.1.1/models/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      410 2022-11-18 19:19:10.000000 flatnet-0.1.1/models/operators.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      520 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:25.664951 flatnet-0.1.1/models/umap_scripts/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    36015 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/distances.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    34501 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/layouts.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    17347 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/sparse.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    12988 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/spectral.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)   136753 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/umap.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     6896 2022-11-29 22:57:14.000000 flatnet-0.1.1/models/umap_scripts/utils.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     8208 2022-11-21 18:44:42.000000 flatnet-0.1.1/models/vae.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-06 04:10:25.978708 flatnet-0.1.1/setup.cfg
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     1202 2023-05-06 04:08:32.000000 flatnet-0.1.1/setup.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:10:25.921306 flatnet-0.1.1/tools/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:39.000000 flatnet-0.1.1/tools/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      608 2022-11-04 18:24:19.000000 flatnet-0.1.1/tools/gp_manifold_generator.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3433 2023-01-22 00:04:53.000000 flatnet-0.1.1/tools/manifold_generator.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3241 2022-10-28 03:06:50.000000 flatnet-0.1.1/tools/randman.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-03-31 21:46:28.000000 flatnet-0.1.1/tools/test_geodesics.py
```

### Comparing `flatnet-0.1.0/README.md` & `flatnet-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,38 @@
 
 This is a research project focused on the automatic generation of autoencoders with minimal feature size, when the data is supported near an embedded submanifold. Using the geometric structure of the manifold, we can equivalently treat this problem as a manifold flattening problem when the manifold is flattenable[^1]. See our paper, [Representation Learning via Manifold Flattening and Reconstruction](https://arxiv.org/abs/2305.01777), for more details.
 
 [^1]: Geometric note: while flattenability is not general, there are some heuristic reasons we can motivate this assumption for real world data. For example, if a dataset permits a VAE-like autoencoder, where samples from the data distribution can be generated via a standard Gaussian in the latent space, then the samples lie close in probability to a flattenable manifold, as this VAE has constructed a single-chart atlas.
 
 ## Installation
 
-The project is written in Python. To install the appropriate dependencies, run the following command:
+The pure FlatNet construction (training) code is available as a pip package and can be installed in the following way:
+
+```
+pip install flatnet
+```
+
+This repo also contains a number of testing and illustrative files to both familiarize new users with the framework and show the experiments run in the main paper. To install the appropriate remaining dependencies for this repo, first navigate to the project directory, then run the following command:
 
 ```
 pip install -r requirements.txt
 ```
 
 ## Quickstart usage
 
 The script `flatnet.py` includes many example experiments to run FlatNet constructions on. To see an example experiment, simply run `python flatnet_test.py` in the main directory to see the flattening and reconstruction of a simple sine wave. Further experiments and options can be specified through command line arguments, managed through [tyro](https://github.com/brentyi/tyro); to see the full list of arguments, run `python flatnet_test.py --help`.
 
 
 ## Directory Structure
 
 - `flatnet_test.py`: main test script, as described in above section.
-- `flatnet.py`: contains the main FlatNet construction (training) code.
+- `flatnet/train.py`: contains the main FlatNet construction (training) code.
+- `flatnet/modules`: contains code for the neural network modules used in FlatNet.
 - `experiments-paper`: contains scripts and results from experiments done in the paper.
 - `models`: contains code for various models that FlatNet was compared against in the paper.
-- `modules`: contains code for the neural network modules used in FlatNet.
 - `tools`: contains auxillery tools for evaulating the method, such as random manifold generators.
 
 
 ## Citation
 
 If you use this work in your research, please cite the following paper:
 
@@ -37,8 +43,8 @@
   title = {Representation Learning via Manifold Flattening and Reconstruction},
   year = {2023},
   eprint = {2305.01777},
   url = {https://arxiv.org/abs/2305.01777},
 }
 ```
 
-We hope that you find this project useful. If you have any questions or suggestions, please feel free to contact us.
+We hope that you find this project useful. If you have any questions or suggestions, please feel free to contact us.
```

### Comparing `flatnet-0.1.0/flatnet/modules/flatnet_nn.py` & `flatnet-0.1.1/flatnet/modules/flatnet_nn.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/flatnet/train.py` & `flatnet-0.1.1/flatnet/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,20 @@
 
     ############# INIT GLOBAL VARIABLES##########
     # encoder network
     f = flatnet_nn.FlatteningNetwork()
     # decoder network
     g = flatnet_nn.FlatteningNetwork()
     Z = X.clone()
+
+    # normalize data
+    Z_mean = torch.mean(Z, dim=0)
+    Z = Z - Z_mean
+    Z_norm = Z.pow(2).mean().sqrt()
+    Z = Z / Z_norm
     # ################ MAIN LOOP #########################
     with trange(n_iter, unit="iters") as pbar:
         for j in pbar:
             # if j % 20 == 0:
             # 	plt.scatter(Z[:,0].detach().numpy(), Z[:,1].detach().numpy())
             # 	plt.show()
```

### Comparing `flatnet-0.1.0/flatnet.egg-info/SOURCES.txt` & `flatnet-0.1.1/flatnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/flatnet.egg-info/requires.txt` & `flatnet-0.1.1/flatnet.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+Jinja2>=3.1.2
+MarkupSafe>=2.1.2
 cmake>=3.26.3
 filelock>=3.12.0
 geoopt>=0.5.0
-Jinja2>=3.1.2
 lit>=16.0.2
-MarkupSafe>=2.1.2
 mpmath>=1.3.0
 networkx>=3.1
 numpy>=1.24.3
 nvidia-cublas-cu11>=11.10.3.66
 nvidia-cuda-cupti-cu11>=11.7.101
 nvidia-cuda-nvrtc-cu11>=11.7.99
 nvidia-cuda-runtime-cu11>=11.7.99
```

### Comparing `flatnet-0.1.0/models/umap.py` & `flatnet-0.1.1/models/umap.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/models/umap_scripts/distances.py` & `flatnet-0.1.1/models/umap_scripts/distances.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/models/umap_scripts/layouts.py` & `flatnet-0.1.1/models/umap_scripts/layouts.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/models/umap_scripts/sparse.py` & `flatnet-0.1.1/models/umap_scripts/sparse.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/models/umap_scripts/spectral.py` & `flatnet-0.1.1/models/umap_scripts/spectral.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/models/umap_scripts/umap.py` & `flatnet-0.1.1/models/umap_scripts/umap.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/models/umap_scripts/utils.py` & `flatnet-0.1.1/models/umap_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/models/vae.py` & `flatnet-0.1.1/models/vae.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/setup.py` & `flatnet-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flatnet',
-    version='0.1.0',
+    version='0.1.1',
     description='FlatNet implementation in PyTorch, from the paper \"Representation Learning via Manifold Flattening and Reconstruction\"',
     author='Michael Psenka',
     packages=find_packages(),
     install_requires=[ 
         'cmake>=3.26.3',
         'filelock>=3.12.0',
         'geoopt>=0.5.0',
```

### Comparing `flatnet-0.1.0/tools/gp_manifold_generator.py` & `flatnet-0.1.1/tools/gp_manifold_generator.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/tools/manifold_generator.py` & `flatnet-0.1.1/tools/manifold_generator.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.0/tools/randman.py` & `flatnet-0.1.1/tools/randman.py`

 * *Files identical despite different names*

