# Comparing `tmp/vision_xformer-0.1.3.tar.gz` & `tmp/vision_xformer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_xformer-0.1.3.tar", last modified: Sat May  6 18:50:01 2023, max compression
+gzip compressed data, was "vision_xformer-0.1.4.tar", last modified: Sat May  6 18:57:27 2023, max compression
```

## Comparing `vision_xformer-0.1.3.tar` & `vision_xformer-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:50:01.700533 vision_xformer-0.1.3/
--rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3823 2023-05-06 18:50:01.697532 vision_xformer-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3085 2023-05-06 01:04:35.000000 vision_xformer-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 18:50:01.701540 vision_xformer-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-05-06 18:49:45.000000 vision_xformer-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:50:01.589163 vision_xformer-0.1.3/vision_xformer/
--rw-rw-rw-   0        0        0      157 2023-05-06 02:12:38.000000 vision_xformer-0.1.3/vision_xformer/__init__.py
--rw-rw-rw-   0        0        0     6575 2023-05-06 18:49:39.000000 vision_xformer-0.1.3/vision_xformer/vision_linformer.py
--rw-rw-rw-   0        0        0     7009 2023-05-06 01:29:58.000000 vision_xformer-0.1.3/vision_xformer/vision_nystromformer.py
--rw-rw-rw-   0        0        0    20185 2023-05-06 01:55:44.000000 vision_xformer-0.1.3/vision_xformer/vision_performer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:50:01.695529 vision_xformer-0.1.3/vision_xformer.egg-info/
--rw-rw-rw-   0        0        0     3823 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 18:57:27.076306 vision_xformer-0.1.4/
+-rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3823 2023-05-06 18:57:27.073309 vision_xformer-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3085 2023-05-06 01:04:35.000000 vision_xformer-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 18:57:27.076306 vision_xformer-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-05-06 18:57:06.000000 vision_xformer-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:57:26.979368 vision_xformer-0.1.4/vision_xformer/
+-rw-rw-rw-   0        0        0      157 2023-05-06 02:12:38.000000 vision_xformer-0.1.4/vision_xformer/__init__.py
+-rw-rw-rw-   0        0        0     6497 2023-05-06 18:56:56.000000 vision_xformer-0.1.4/vision_xformer/vision_linformer.py
+-rw-rw-rw-   0        0        0     7009 2023-05-06 01:29:58.000000 vision_xformer-0.1.4/vision_xformer/vision_nystromformer.py
+-rw-rw-rw-   0        0        0    20185 2023-05-06 01:55:44.000000 vision_xformer-0.1.4/vision_xformer/vision_performer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:57:27.071293 vision_xformer-0.1.4/vision_xformer.egg-info/
+-rw-rw-rw-   0        0        0     3823 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/top_level.txt
```

### Comparing `vision_xformer-0.1.3/LICENSE` & `vision_xformer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.3/PKG-INFO` & `vision_xformer-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_xformer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vision_xformer-0.1.3/README.md` & `vision_xformer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.3/setup.py` & `vision_xformer-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'vision_xformer',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.3',
+  version = '0.1.4',
   license='MIT',
   description = 'Vision Xformers',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/VisionXformer',
```

### Comparing `vision_xformer-0.1.3/vision_xformer/vision_linformer.py` & `vision_xformer-0.1.4/vision_xformer/vision_linformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         )
     def forward(self, x):
         return self.net(x)
 
 
 
 class Transformer(nn.Module):
-    def __init__(self, dim, depth, heads, dim_head, mlp_dim, seq_len, k = 64, one_kv_head = True, share_kv = True, reversible = False, dropout = 0.):
+    def __init__(self, dim, depth, heads, dim_head, mlp_dim, seq_len, k, one_kv_head, share_kv, dropout = 0.):
         super().__init__()
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
                 PreNorm(dim, LinformerSelfAttention(dim, seq_len, k = k, heads = heads, dim_head = dim_head, one_kv_head = one_kv_head, share_kv = share_kv, dropout = dropout)),
                 PreNorm(dim, FeedForward(dim, mlp_dim, dropout = dropout))
@@ -126,15 +126,15 @@
             x = attn(x) + x
             x = ff(x) + x
         return x
 
 
 
 class ViL(nn.Module):
-    def __init__(self, *, image_size, patch_size, num_classes, dim, depth, heads, mlp_dim, k = 64, one_kv_head = True, share_kv = True, reversible = False, pool = 'cls', channels = 3, dim_head = 64, dropout = 0., emb_dropout = 0.):
+    def __init__(self, *, image_size, patch_size, num_classes, dim, depth, heads, mlp_dim, k = 64, one_kv_head = True, share_kv = True, pool = 'cls', channels = 3, dim_head = 64, dropout = 0., emb_dropout = 0.):
         super().__init__()
         image_height, image_width = pair(image_size)
         patch_height, patch_width = pair(patch_size)
 
         assert image_height % patch_height == 0 and image_width % patch_width == 0, 'Image dimensions must be divisible by the patch size.'
 
         num_patches = (image_height // patch_height) * (image_width // patch_width)
@@ -148,15 +148,15 @@
             nn.LayerNorm(dim),
         )
 
         self.pos_embedding = nn.Parameter(torch.randn(1, num_patches + 1, dim))
         self.cls_token = nn.Parameter(torch.randn(1, 1, dim))
         self.dropout = nn.Dropout(emb_dropout)
 
-        self.transformer = Transformer(dim, depth, heads, dim_head, mlp_dim,seq_len = num_patches + 1, k = k, one_kv_head = one_kv_head, share_kv = share_kv, reversible = reversible, dropout = dropout)
+        self.transformer = Transformer(dim, depth, heads, dim_head, mlp_dim, seq_len = int(num_patches + 1), k = k, one_kv_head = one_kv_head, share_kv = share_kv, dropout = dropout)
 
         self.pool = pool
         self.to_latent = nn.Identity()
 
         self.mlp_head = nn.Sequential(
             nn.LayerNorm(dim),
             nn.Linear(dim, num_classes)
```

### Comparing `vision_xformer-0.1.3/vision_xformer/vision_nystromformer.py` & `vision_xformer-0.1.4/vision_xformer/vision_nystromformer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.3/vision_xformer/vision_performer.py` & `vision_xformer-0.1.4/vision_xformer/vision_performer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.3/vision_xformer.egg-info/PKG-INFO` & `vision_xformer-0.1.4/vision_xformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-xformer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```

