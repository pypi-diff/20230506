# Comparing `tmp/MaMMUT-pytorch-0.0.2.tar.gz` & `tmp/MaMMUT-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MaMMUT-pytorch-0.0.2.tar", last modified: Fri May  5 20:24:01 2023, max compression
+gzip compressed data, was "MaMMUT-pytorch-0.0.3.tar", last modified: Sat May  6 01:19:28 2023, max compression
```

## Comparing `MaMMUT-pytorch-0.0.2.tar` & `MaMMUT-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:24:01.079718 MaMMUT-pytorch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 20:23:49.000000 MaMMUT-pytorch-0.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:24:01.079718 MaMMUT-pytorch-0.0.2/MaMMUT_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-05 20:24:01.000000 MaMMUT-pytorch-0.0.2/MaMMUT_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-05 20:24:01.000000 MaMMUT-pytorch-0.0.2/MaMMUT_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:24:01.000000 MaMMUT-pytorch-0.0.2/MaMMUT_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 20:24:01.000000 MaMMUT-pytorch-0.0.2/MaMMUT_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 20:24:01.000000 MaMMUT-pytorch-0.0.2/MaMMUT_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-05 20:24:01.079718 MaMMUT-pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-05 20:23:49.000000 MaMMUT-pytorch-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:24:01.079718 MaMMUT-pytorch-0.0.2/mammut_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 20:23:49.000000 MaMMUT-pytorch-0.0.2/mammut_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14073 2023-05-05 20:23:49.000000 MaMMUT-pytorch-0.0.2/mammut_pytorch/mammut_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:24:01.079718 MaMMUT-pytorch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-05 20:23:49.000000 MaMMUT-pytorch-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/mammut_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/mammut_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/mammut_pytorch/mammut_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/setup.py
```

### Comparing `MaMMUT-pytorch-0.0.2/LICENSE` & `MaMMUT-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MaMMUT-pytorch-0.0.2/MaMMUT_pytorch.egg-info/PKG-INFO` & `MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MaMMUT-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: MaMMUT - Pytorch
 Home-page: https://github.com/lucidrains/MaMMUT-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,multimodal,attention mechanism,contrastive learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MaMMUT-pytorch-0.0.2/PKG-INFO` & `MaMMUT-pytorch-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MaMMUT-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: MaMMUT - Pytorch
 Home-page: https://github.com/lucidrains/MaMMUT-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,multimodal,attention mechanism,contrastive learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MaMMUT-pytorch-0.0.2/README.md` & `MaMMUT-pytorch-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `MaMMUT-pytorch-0.0.2/mammut_pytorch/mammut_pytorch.py` & `MaMMUT-pytorch-0.0.3/mammut_pytorch/mammut_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,25 +420,27 @@
         return_embeddings=False
     ):
         batch, device = text.shape[0], text.device
 
         if return_loss and not exists(labels):
             text, labels = text[:, :-1], text[:, 1:]
 
-        text_embeds, text_tokens = self.embed_text(text)
+        text_embeds, _ = self.embed_text(text)
 
         image_embeds, image_tokens = self.embed_image(images=images, image_tokens=image_tokens)
 
         # return embeddings if that is what the researcher wants
 
         if return_embeddings:
             return text_embeds, image_embeds
 
         # go through layers
 
+        text_tokens = self.token_emb(text)
+
         for attn_ff, cross_attn in self.layers:
             text_tokens = attn_ff(text_tokens)
 
             if exists(cross_attn):
                 text_tokens = cross_attn(text_tokens, image_tokens)
 
         logits = self.to_logits(text_tokens)
```

### Comparing `MaMMUT-pytorch-0.0.2/setup.py` & `MaMMUT-pytorch-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MaMMUT-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'MaMMUT - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/MaMMUT-pytorch',
   keywords = [
```

