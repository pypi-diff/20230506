# Comparing `tmp/flatnet-0.1.3.tar.gz` & `tmp/flatnet-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatnet-0.1.3.tar", last modified: Fri May  5 22:15:39 2023, max compression
+gzip compressed data, was "flatnet-0.1.4.tar", last modified: Fri May  5 22:51:32 2023, max compression
```

## Comparing `flatnet-0.1.3.tar` & `flatnet-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:29:20.380452 flatnet-0.1.3/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:29:20.380452 flatnet-0.1.3/PKG-INFO
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:29:19.879272 flatnet-0.1.3/flatnet/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.1.3/flatnet/__init__.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:29:20.301887 flatnet-0.1.3/flatnet/modules/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.1.3/flatnet/modules/__init__.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.1.3/flatnet/modules/flatnet_nn.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    14293 2023-05-06 04:09:02.000000 flatnet-0.1.3/flatnet/train.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 04:29:20.160860 flatnet-0.1.3/flatnet.egg-info/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/PKG-INFO
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      257 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/SOURCES.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/dependency_links.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      556 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/requires.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-06 04:29:19.000000 flatnet-0.1.3/flatnet.egg-info/top_level.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-06 04:29:20.380452 flatnet-0.1.3/setup.cfg
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     1202 2023-05-06 04:28:06.000000 flatnet-0.1.3/setup.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 05:02:27.266479 flatnet-0.1.4/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 05:02:27.257483 flatnet-0.1.4/PKG-INFO
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 05:02:26.692868 flatnet-0.1.4/flatnet/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.1.4/flatnet/__init__.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 05:02:27.174946 flatnet-0.1.4/flatnet/modules/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.1.4/flatnet/modules/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.1.4/flatnet/modules/flatnet_nn.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    14367 2023-05-06 05:00:43.000000 flatnet-0.1.4/flatnet/train.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-06 05:02:27.005877 flatnet-0.1.4/flatnet.egg-info/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      299 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      257 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      556 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/requires.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-06 05:02:26.000000 flatnet-0.1.4/flatnet.egg-info/top_level.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-06 05:02:27.269479 flatnet-0.1.4/setup.cfg
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     1202 2023-05-06 04:40:41.000000 flatnet-0.1.4/setup.py
```

### Comparing `flatnet-0.1.3/flatnet/modules/flatnet_nn.py` & `flatnet-0.1.4/flatnet/modules/flatnet_nn.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.3/flatnet/train.py` & `flatnet-0.1.4/flatnet/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 def train(X,
        n_stop_to_converge=5,  # how many times of no progress do we call convergence?
        n_iter=500,  # number of flattening steps to perform
        n_iter_inner=1000,  # how many max steps for inner optimization of U, V
        thres_recon=1e-4,  # threshold for reconstruction loss being good enough
        alpha_max=0.5,  # global parameter for kernel
        r_dimcheck_coeff=0.15,  # # radius for checking dimension.
+       max_error_dimcheck_ratio=0.3,  # max l0 error with respect to r_dimcheck to stop dimension search
        r_min_coeff=0.15,  # minimum allowed radius for each flattening
        r_max_coeff=1.1,  # maximum allowed radius for each flattening
        r_step_min_coeff=1.0,  # max steps to take when finding biggest r
        n_iter_rsearch=1,  # max steps to take when finding biggest r
        ):
     N, D = X.shape
     # needed for dist-to-gamma conversion
@@ -71,19 +72,14 @@
     ############# INIT GLOBAL VARIABLES##########
     # encoder network
     f = flatnet_nn.FlatteningNetwork()
     # decoder network
     g = flatnet_nn.FlatteningNetwork()
     Z = X.clone()
 
-    # normalize data
-    Z_mean = torch.mean(Z, dim=0)
-    Z = Z - Z_mean
-    Z_norm = Z.pow(2).mean().sqrt()
-    Z = Z / Z_norm
     # ################ MAIN LOOP #########################
     with trange(n_iter, unit="iters") as pbar:
         for j in pbar:
             # if j % 20 == 0:
             # 	plt.scatter(Z[:,0].detach().numpy(), Z[:,1].detach().numpy())
             # 	plt.show()
 
@@ -92,15 +88,15 @@
             choice = torch.randint(N, (1,))
             z_c = Z[choice, :]
 
             # STEP 1: find minimal dimension d we can flatten neighborhood
             # to and still be able to reconstruct
 
             # note d is implicitly returned, as U, V are of shape (D, d)
-            U, loss_rdimcheck = find_d(Z, z_c, r_dimcheck, n_iter_inner, d_prev, max_error=thres_recon)
+            U, loss_rdimcheck = find_d(Z, z_c, r_dimcheck, n_iter_inner, d_prev, max_error=thres_recon, max_error_dimcheck_ratio=max_error_dimcheck_ratio)
 
             # STEP 2: use secant method to find maximal radius that achieves
             # desired reconstruction loss
 
             # get needed second observation
             U, V, loss_rmidpoint = opt_UV(Z, z_c, U, n_iter_inner, r=r_midpoint)
 
@@ -291,20 +287,20 @@
             if step_size < 1e-5:
                 break
     # if i >= n_iter_inner - 1:
     # 	print('Warning: U did not converge')
     return U.detach().data, V.detach().data, loss.detach()
 
 
-def find_d(Z, z_c, r_dimcheck, n_iter_inner, d_prev, max_error):
+def find_d(Z, z_c, r_dimcheck, n_iter_inner, d_prev, max_error, max_error_dimcheck_ratio=0.3):
     # We find the minimial d by iteratively fitting a model
     # for some size d, then increase d and repeat if the max
     # reconstruction error is too large
 
-    max_error = 0.2 * r_dimcheck
+    max_error = max_error_dimcheck_ratio * r_dimcheck
 
     N, D = Z.shape
     # init
     U_0 = torch.randn(D, d_prev)
     U_0 = torch.linalg.qr(U_0)[0]
 
     # TRACKING VARS
```

### Comparing `flatnet-0.1.3/flatnet.egg-info/requires.txt` & `flatnet-0.1.4/flatnet.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flatnet-0.1.3/setup.py` & `flatnet-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flatnet',
-    version='0.1.3',
+    version='0.1.4',
     description='FlatNet implementation in PyTorch, from the paper \"Representation Learning via Manifold Flattening and Reconstruction\"',
     author='Michael Psenka',
     packages=find_packages(),
     install_requires=[ 
         'cmake>=3.26.3',
         'filelock>=3.12.0',
         'geoopt>=0.5.0',
```

