# Comparing `tmp/vision_xformer-0.1.2.tar.gz` & `tmp/vision_xformer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_xformer-0.1.2.tar", last modified: Sat May  6 18:44:24 2023, max compression
+gzip compressed data, was "vision_xformer-0.1.3.tar", last modified: Sat May  6 18:50:01 2023, max compression
```

## Comparing `vision_xformer-0.1.2.tar` & `vision_xformer-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:44:24.954941 vision_xformer-0.1.2/
--rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3823 2023-05-06 18:44:24.950959 vision_xformer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3085 2023-05-06 01:04:35.000000 vision_xformer-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 18:44:24.955943 vision_xformer-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-05-06 18:43:58.000000 vision_xformer-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:44:24.850811 vision_xformer-0.1.2/vision_xformer/
--rw-rw-rw-   0        0        0      157 2023-05-06 02:12:38.000000 vision_xformer-0.1.2/vision_xformer/__init__.py
--rw-rw-rw-   0        0        0     6524 2023-05-06 18:43:05.000000 vision_xformer-0.1.2/vision_xformer/vision_linformer.py
--rw-rw-rw-   0        0        0     7009 2023-05-06 01:29:58.000000 vision_xformer-0.1.2/vision_xformer/vision_nystromformer.py
--rw-rw-rw-   0        0        0    20185 2023-05-06 01:55:44.000000 vision_xformer-0.1.2/vision_xformer/vision_performer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:44:24.945939 vision_xformer-0.1.2/vision_xformer.egg-info/
--rw-rw-rw-   0        0        0     3823 2023-05-06 18:44:24.000000 vision_xformer-0.1.2/vision_xformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-06 18:44:24.000000 vision_xformer-0.1.2/vision_xformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:44:24.000000 vision_xformer-0.1.2/vision_xformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-06 18:44:24.000000 vision_xformer-0.1.2/vision_xformer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 18:44:24.000000 vision_xformer-0.1.2/vision_xformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 18:50:01.700533 vision_xformer-0.1.3/
+-rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3823 2023-05-06 18:50:01.697532 vision_xformer-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3085 2023-05-06 01:04:35.000000 vision_xformer-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 18:50:01.701540 vision_xformer-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-05-06 18:49:45.000000 vision_xformer-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:50:01.589163 vision_xformer-0.1.3/vision_xformer/
+-rw-rw-rw-   0        0        0      157 2023-05-06 02:12:38.000000 vision_xformer-0.1.3/vision_xformer/__init__.py
+-rw-rw-rw-   0        0        0     6575 2023-05-06 18:49:39.000000 vision_xformer-0.1.3/vision_xformer/vision_linformer.py
+-rw-rw-rw-   0        0        0     7009 2023-05-06 01:29:58.000000 vision_xformer-0.1.3/vision_xformer/vision_nystromformer.py
+-rw-rw-rw-   0        0        0    20185 2023-05-06 01:55:44.000000 vision_xformer-0.1.3/vision_xformer/vision_performer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:50:01.695529 vision_xformer-0.1.3/vision_xformer.egg-info/
+-rw-rw-rw-   0        0        0     3823 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 18:50:01.000000 vision_xformer-0.1.3/vision_xformer.egg-info/top_level.txt
```

### Comparing `vision_xformer-0.1.2/LICENSE` & `vision_xformer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.2/PKG-INFO` & `vision_xformer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_xformer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vision_xformer-0.1.2/README.md` & `vision_xformer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.2/setup.py` & `vision_xformer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'vision_xformer',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.2',
+  version = '0.1.3',
   license='MIT',
   description = 'Vision Xformers',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/VisionXformer',
```

### Comparing `vision_xformer-0.1.2/vision_xformer/vision_linformer.py` & `vision_xformer-0.1.3/vision_xformer/vision_linformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             nn.LayerNorm(dim),
         )
 
         self.pos_embedding = nn.Parameter(torch.randn(1, num_patches + 1, dim))
         self.cls_token = nn.Parameter(torch.randn(1, 1, dim))
         self.dropout = nn.Dropout(emb_dropout)
 
-        self.transformer = Transformer(dim, depth, heads, dim_head, mlp_dim, k, one_kv_head, share_kv, reversible, dropout, seq_len = num_patches + 1)
+        self.transformer = Transformer(dim, depth, heads, dim_head, mlp_dim,seq_len = num_patches + 1, k = k, one_kv_head = one_kv_head, share_kv = share_kv, reversible = reversible, dropout = dropout)
 
         self.pool = pool
         self.to_latent = nn.Identity()
 
         self.mlp_head = nn.Sequential(
             nn.LayerNorm(dim),
             nn.Linear(dim, num_classes)
```

### Comparing `vision_xformer-0.1.2/vision_xformer/vision_nystromformer.py` & `vision_xformer-0.1.3/vision_xformer/vision_nystromformer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.2/vision_xformer/vision_performer.py` & `vision_xformer-0.1.3/vision_xformer/vision_performer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.2/vision_xformer.egg-info/PKG-INFO` & `vision_xformer-0.1.3/vision_xformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-xformer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```

