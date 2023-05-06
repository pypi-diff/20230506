# Comparing `tmp/vector_quantize_pytorch-1.2.3.tar.gz` & `tmp/vector_quantize_pytorch-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.2.3.tar", last modified: Fri May  5 17:31:27 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.4.0.tar", last modified: Sat May  6 16:36:50 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.2.3.tar` & `vector_quantize_pytorch-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-05-05 17:31:16.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:31:27.286077 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 17:31:27.000000 vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:36:50.746312 vector_quantize_pytorch-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 16:36:35.000000 vector_quantize_pytorch-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 16:36:50.746312 vector_quantize_pytorch-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-06 16:36:35.000000 vector_quantize_pytorch-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:36:50.746312 vector_quantize_pytorch-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-06 16:36:35.000000 vector_quantize_pytorch-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:36:50.746312 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-06 16:36:35.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-06 16:36:35.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-06 16:36:35.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-05-06 16:36:35.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:36:50.746312 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 16:36:50.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-06 16:36:50.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:36:50.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 16:36:50.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 16:36:50.000000 vector_quantize_pytorch-1.4.0/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.2.3/LICENSE` & `vector_quantize_pytorch-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.3/PKG-INFO` & `vector_quantize_pytorch-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.2.3
+Version: 1.4.0
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.2.3/README.md` & `vector_quantize_pytorch-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,36 @@
 x = torch.randn(1, 1024, 256)
 quantized, indices, commit_loss = residual_vq(x)
 
 # (1, 1024, 256), (8, 1, 1024), (8, 1)
 # (batch, seq, dim), (quantizer, batch, seq), (quantizer, batch)
 ```
 
+<a href="https://arxiv.org/abs/2305.02765">A recent paper</a> further proposes to do residual VQ on groups of the feature dimension, showing equivalent results to Encodec while using far fewer codebooks. You can use it by importing `GroupedResidualVQ`
+
+```python
+import torch
+from vector_quantize_pytorch import GroupedResidualVQ
+
+residual_vq = GroupedResidualVQ(
+    dim = 256,
+    num_quantizers = 8,      # specify number of quantizers
+    groups = 2,
+    codebook_size = 1024,    # codebook size
+)
+
+x = torch.randn(1, 1024, 256)
+
+quantized, indices, commit_loss = residual_vq(x)
+
+# (1, 1024, 256), (1, 1024, 8), (1, 8)
+# (batch, seq, dim), (groups, batch, seq, quantizer), (groups, batch, quantizer)
+
+```
+
 ## Initialization
 
 The SoundStream paper proposes that the codebook should be initialized by the kmeans centroids of the first batch. You can easily turn on this feature with one flag `kmeans_init = True`, for either `VectorQuantize` or `ResidualVQ` class
 
 ```python
 import torch
 from vector_quantize_pytorch import ResidualVQ
@@ -371,7 +393,16 @@
 ```bibtex
 @inproceedings{Shen2023NaturalSpeech2L,
     title   = {NaturalSpeech 2: Latent Diffusion Models are Natural and Zero-Shot Speech and Singing Synthesizers},
     author  = {Kai Shen and Zeqian Ju and Xu Tan and Yanqing Liu and Yichong Leng and Lei He and Tao Qin and Sheng Zhao and Jiang Bian},
     year    = {2023}
 }
 ```
+
+```bibtex
+@inproceedings{Yang2023HiFiCodecGV,
+    title   = {HiFi-Codec: Group-residual Vector quantization for High Fidelity Audio Codec},
+    author  = {Dongchao Yang and Songxiang Liu and Rongjie Huang and Jinchuan Tian and Chao Weng and Yuexian Zou},
+    year    = {2023}
+}
+```
+
```

#### html2text {}

```diff
@@ -28,38 +28,46 @@
 arguments. ```python import torch from vector_quantize_pytorch import
 ResidualVQ residual_vq = ResidualVQ( dim = 256, num_quantizers = 8,
 codebook_size = 1024, sample_codebook_temp = 0.1, # temperature for
 stochastically sampling codes, 0 would be equivalent to non-stochastic
 shared_codebook = True # whether to share the codebooks for all quantizers or
 not ) x = torch.randn(1, 1024, 256) quantized, indices, commit_loss =
 residual_vq(x) # (1, 1024, 256), (8, 1, 1024), (8, 1) # (batch, seq, dim),
-(quantizer, batch, seq), (quantizer, batch) ``` ## Initialization The
-SoundStream paper proposes that the codebook should be initialized by the
-kmeans centroids of the first batch. You can easily turn on this feature with
-one flag `kmeans_init = True`, for either `VectorQuantize` or `ResidualVQ`
-class ```python import torch from vector_quantize_pytorch import ResidualVQ
-residual_vq = ResidualVQ( dim = 256, codebook_size = 256, num_quantizers = 4,
-kmeans_init = True, # set to True kmeans_iters = 10 # number of kmeans
-iterations to calculate the centroids for the codebook on init ) x =
-torch.randn(1, 1024, 256) quantized, indices, commit_loss = residual_vq(x) ```
-## Increasing codebook usage This repository will contain a few techniques from
-various papers to combat "dead" codebook entries, which is a common problem
-when using vector quantizers. ### Lower codebook dimension The Improved_VQGAN
-paper proposes to have the codebook kept in a lower dimension. The encoder
-values are projected down before being projected back to high dimensional after
-quantization. You can set this with the `codebook_dim` hyperparameter.
-```python import torch from vector_quantize_pytorch import VectorQuantize vq =
-VectorQuantize( dim = 256, codebook_size = 256, codebook_dim = 16 # paper
-proposes setting this to 32 or as low as 8 to increase codebook usage ) x =
-torch.randn(1, 1024, 256) quantized, indices, commit_loss = vq(x) ``` ###
-Cosine similarity The Improved_VQGAN_paper also proposes to l2 normalize the
-codes and the encoded vectors, which boils down to using cosine similarity for
-the distance. They claim enforcing the vectors on a sphere leads to
-improvements in code usage and downstream reconstruction. You can turn this on
-by setting `use_cosine_sim = True` ```python import torch from
+(quantizer, batch, seq), (quantizer, batch) ``` A_recent_paper further proposes
+to do residual VQ on groups of the feature dimension, showing equivalent
+results to Encodec while using far fewer codebooks. You can use it by importing
+`GroupedResidualVQ` ```python import torch from vector_quantize_pytorch import
+GroupedResidualVQ residual_vq = GroupedResidualVQ( dim = 256, num_quantizers =
+8, # specify number of quantizers groups = 2, codebook_size = 1024, # codebook
+size ) x = torch.randn(1, 1024, 256) quantized, indices, commit_loss =
+residual_vq(x) # (1, 1024, 256), (1, 1024, 8), (1, 8) # (batch, seq, dim),
+(groups, batch, seq, quantizer), (groups, batch, quantizer) ``` ##
+Initialization The SoundStream paper proposes that the codebook should be
+initialized by the kmeans centroids of the first batch. You can easily turn on
+this feature with one flag `kmeans_init = True`, for either `VectorQuantize` or
+`ResidualVQ` class ```python import torch from vector_quantize_pytorch import
+ResidualVQ residual_vq = ResidualVQ( dim = 256, codebook_size = 256,
+num_quantizers = 4, kmeans_init = True, # set to True kmeans_iters = 10 #
+number of kmeans iterations to calculate the centroids for the codebook on init
+) x = torch.randn(1, 1024, 256) quantized, indices, commit_loss = residual_vq
+(x) ``` ## Increasing codebook usage This repository will contain a few
+techniques from various papers to combat "dead" codebook entries, which is a
+common problem when using vector quantizers. ### Lower codebook dimension The
+Improved_VQGAN_paper proposes to have the codebook kept in a lower dimension.
+The encoder values are projected down before being projected back to high
+dimensional after quantization. You can set this with the `codebook_dim`
+hyperparameter. ```python import torch from vector_quantize_pytorch import
+VectorQuantize vq = VectorQuantize( dim = 256, codebook_size = 256,
+codebook_dim = 16 # paper proposes setting this to 32 or as low as 8 to
+increase codebook usage ) x = torch.randn(1, 1024, 256) quantized, indices,
+commit_loss = vq(x) ``` ### Cosine similarity The Improved_VQGAN_paper also
+proposes to l2 normalize the codes and the encoded vectors, which boils down to
+using cosine similarity for the distance. They claim enforcing the vectors on a
+sphere leads to improvements in code usage and downstream reconstruction. You
+can turn this on by setting `use_cosine_sim = True` ```python import torch from
 vector_quantize_pytorch import VectorQuantize vq = VectorQuantize( dim = 256,
 codebook_size = 256, use_cosine_sim = True # set this to True ) x = torch.randn
 (1, 1024, 256) quantized, indices, commit_loss = vq(x) ``` ### Expiring stale
 codes Finally, the SoundStream paper has a scheme where they replace codes that
 have hits below a certain threshold with randomly selected vector from the
 current batch. You can set this threshold with `threshold_ema_dead_code`
 keyword. ```python import torch from vector_quantize_pytorch import
@@ -163,8 +171,11 @@
 and Ginger Perng and Hagen Soltau and Trevor Strohman and Bhuvana Ramabhadran
 and Tara N. Sainath and Pedro J. Moreno and Chung-Cheng Chiu and Johan
 Schalkwyk and Franccoise Beaufays and Yonghui Wu}, year = {2023} } ```
 ```bibtex @inproceedings{Shen2023NaturalSpeech2L, title = {NaturalSpeech 2:
 Latent Diffusion Models are Natural and Zero-Shot Speech and Singing
 Synthesizers}, author = {Kai Shen and Zeqian Ju and Xu Tan and Yanqing Liu and
 Yichong Leng and Lei He and Tao Qin and Sheng Zhao and Jiang Bian}, year =
-{2023} } ```
+{2023} } ``` ```bibtex @inproceedings{Yang2023HiFiCodecGV, title = {HiFi-Codec:
+Group-residual Vector quantization for High Fidelity Audio Codec}, author =
+{Dongchao Yang and Songxiang Liu and Rongjie Huang and Jinchuan Tian and Chao
+Weng and Yuexian Zou}, year = {2023} } ```
```

### Comparing `vector_quantize_pytorch-1.2.3/setup.py` & `vector_quantize_pytorch-1.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.2.3',
+  version = '1.4.0',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.4.0/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.4.0/vector_quantize_pytorch/residual_vq.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from math import ceil
 from functools import partial
+from itertools import zip_longest
 from random import randrange
 
 import torch
 from torch import nn
 import torch.nn.functional as F
 from vector_quantize_pytorch.vector_quantize_pytorch import VectorQuantize
 
 from einops import rearrange, repeat, pack, unpack
 
 # helper functions
 
 def exists(val):
     return val is not None
 
+def default(val, d):
+    return val if exists(val) else d
+
 def round_up_multiple(num, mult):
     return ceil(num / mult) * mult
 
 # main class
 
 class ResidualVQ(nn.Module):
     """ Follows Algorithm 1. in https://arxiv.org/pdf/2107.03312.pdf """
@@ -179,7 +183,81 @@
             # whether to return all codes from all codebooks across layers
             all_codes = self.get_codes_from_indices(all_indices)
 
             # will return all codes in shape (quantizer, batch, sequence length, codebook dimension)
             ret = (*ret, all_codes)
 
         return ret
+
+# grouped residual vq
+
+class GroupedResidualVQ(nn.Module):
+    def __init__(
+        self,
+        *,
+        dim,
+        groups = 1,
+        accept_image_fmap = False,
+        **kwargs
+    ):
+        super().__init__()
+        self.dim = dim
+        self.groups = groups
+        assert (dim % groups) == 0
+        dim_per_group = dim // groups
+
+        self.accept_image_fmap = accept_image_fmap
+
+        self.rvqs = nn.ModuleList([])
+
+        for _ in range(groups):
+            self.rvqs.append(ResidualVQ(
+                dim = dim_per_group,
+                accept_image_fmap = accept_image_fmap,
+                **kwargs
+            ))
+
+    @property
+    def codebooks(self):
+        return torch.stack(tuple(rvq.codebooks for rvq in self.rvqs))
+
+    def forward(
+        self,
+        x,
+        indices = None,
+        return_all_codes = False
+    ):
+        shape = x.shape
+        split_dim = 1 if self.accept_image_fmap else -1
+        assert shape[split_dim] == self.dim
+
+        # split the feature dimension into groups
+
+        x = x.chunk(self.groups, dim = split_dim)
+
+        indices = default(indices, tuple())
+        return_ce_loss = len(indices) > 0
+        assert len(indices) == 0 or len(indices) == self.groups
+
+        forward_kwargs = dict(return_all_codes = return_all_codes)
+
+        # invoke residual vq on each group
+
+        out = tuple(rvq(chunk, indices = chunk_indices, **forward_kwargs) for rvq, chunk, chunk_indices in zip_longest(self.rvqs, x, indices))
+        out = tuple(zip(*out))
+
+        # if returning cross entropy loss to rvq codebooks
+
+        if return_ce_loss:
+            quantized, ce_losses = out
+            return torch.cat(quantized, dim = split_dim), sum(ce_losses)
+
+        # otherwise, get all the zipped outputs and combine them
+
+        quantized, all_indices, commit_losses, *maybe_all_codes = out
+
+        quantized = torch.cat(quantized, dim = split_dim)
+        all_indices = torch.stack(all_indices)
+        commit_losses = torch.stack(commit_losses)
+
+        ret = (quantized, all_indices, commit_losses, *maybe_all_codes)
+        return ret
```

### Comparing `vector_quantize_pytorch-1.2.3/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.4.0/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.2.3/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.4.0/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.2.3
+Version: 1.4.0
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

