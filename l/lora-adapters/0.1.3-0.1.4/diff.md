# Comparing `tmp/lora_adapters-0.1.3.tar.gz` & `tmp/lora_adapters-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lora_adapters-0.1.3.tar", last modified: Fri May  5 22:51:10 2023, max compression
+gzip compressed data, was "lora_adapters-0.1.4.tar", last modified: Fri May  5 23:55:43 2023, max compression
```

## Comparing `lora_adapters-0.1.3.tar` & `lora_adapters-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:51:10.265406 lora_adapters-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-05 22:51:10.265406 lora_adapters-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:51:10.265406 lora_adapters-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:51:10.265406 lora_adapters-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:51:10.265406 lora_adapters-0.1.3/src/lora_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/src/lora_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/src/lora_adapters/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/src/lora_adapters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:51:10.265406 lora_adapters-0.1.3/src/lora_adapters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-05 22:51:10.000000 lora_adapters-0.1.3/src/lora_adapters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-05 22:51:10.000000 lora_adapters-0.1.3/src/lora_adapters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:51:10.000000 lora_adapters-0.1.3/src/lora_adapters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 22:51:10.000000 lora_adapters-0.1.3/src/lora_adapters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:51:10.265406 lora_adapters-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/tests/test_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/tests/test_dolly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/tests/test_grads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-05 22:51:00.000000 lora_adapters-0.1.3/tests/test_resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:55:43.660198 lora_adapters-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-05 23:55:43.660198 lora_adapters-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 23:55:43.660198 lora_adapters-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:55:43.660198 lora_adapters-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:55:43.660198 lora_adapters-0.1.4/src/lora_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/src/lora_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/src/lora_adapters/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/src/lora_adapters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:55:43.660198 lora_adapters-0.1.4/src/lora_adapters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-05 23:55:43.000000 lora_adapters-0.1.4/src/lora_adapters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-05 23:55:43.000000 lora_adapters-0.1.4/src/lora_adapters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:55:43.000000 lora_adapters-0.1.4/src/lora_adapters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 23:55:43.000000 lora_adapters-0.1.4/src/lora_adapters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:55:43.660198 lora_adapters-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/tests/test_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/tests/test_dolly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/tests/test_grads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-05 23:55:34.000000 lora_adapters-0.1.4/tests/test_resnet.py
```

### Comparing `lora_adapters-0.1.3/LICENSE.md` & `lora_adapters-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lora_adapters-0.1.3/PKG-INFO` & `lora_adapters-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lora_adapters
-Version: 0.1.3
+Version: 0.1.4
 Summary: PyTorch implementation of low-rank adaptation (LoRA), a parameter-efficient approach to adapt a large pre-trained deep learning model which obtains performance on-par with full fine-tuning.
 Home-page: https://github.com/kiansierra/lora-adapters
 Author: Kian Sierra McGettigan
 Author-email: kiansierra90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lora_adapters-0.1.3/README.md` & `lora_adapters-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lora_adapters-0.1.3/pyproject.toml` & `lora_adapters-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lora_adapters-0.1.3/setup.py` & `lora_adapters-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="lora_adapters",
-    version="0.1.3",
+    version="0.1.4",
     author="Kian Sierra McGettigan",
     author_email="kiansierra90@gmail.com",
     description="PyTorch implementation of low-rank adaptation (LoRA), a parameter-efficient approach to adapt a large pre-trained deep learning model which obtains performance on-par with full fine-tuning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=find_packages("src"),
```

### Comparing `lora_adapters-0.1.3/src/lora_adapters/layers.py` & `lora_adapters-0.1.4/src/lora_adapters/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,19 @@
         """
         layer = nn.Embedding(**self.input_kwargs)
         layer.weight.data = self.weight.data
         if not self.merged:
             layer.weight.data += self.weight_delta
         return layer
 
+    def extra_repr(self) -> str:
+        s = nn.Embedding.extra_repr(self)
+        extra = ", rank={}".format(self.rank)
+        return s + extra
+
 
 class LoraLinear(nn.Linear, LoRALayer):
     # LoRA implemented in a dense layer
     def __init__(
         self,
         layer: nn.Linear,
         rank: int = 0,
@@ -196,14 +201,19 @@
         layer.weight.data = self.weight.data
         if not self.merged:
             layer.weight.data += self.weight_delta
         if self.input_kwargs["bias"]:
             layer.bias.data = self.bias.data
         return layer
 
+    def extra_repr(self) -> str:
+        s = nn.Linear.extra_repr(self)
+        extra = ", rank={}".format(self.rank)
+        return s + extra
+
 
 class LoraMergedLinear(nn.Linear, LoRALayer):
     # LoRA implemented in a dense layer
     def __init__(
         self,
         layer: nn.Linear,
         rank: int = 0,
@@ -307,14 +317,19 @@
         layer.weight.data = self.weight.data
         if not self.merged:
             layer.weight.data += self.weight_delta
         if self.input_kwargs["bias"]:
             layer.bias.data = self.bias.data
         return layer
 
+    def extra_repr(self) -> str:
+        s = nn.Linear.extra_repr(self)
+        extra = ", rank={}, enable_lora={}".format(self.rank, self.enable_lora)
+        return s + extra
+
 
 class LoraConv2d(nn.Conv2d, LoRALayer):
     # LoRA implemented in a dense layer
     def __init__(
         self,
         layer: nn.Conv2d,
         rank: int = 0,
@@ -392,13 +407,18 @@
         layer.weight.data = self.weight.data
         if not self.merged:
             layer.weight.data += self.weight_delta
         if self.input_kwargs["bias"]:
             layer.bias.data = self.bias.data
         return layer
 
+    def extra_repr(self) -> str:
+        s = nn.Conv2d.extra_repr(self)
+        extra = ", rank={}".format(self.rank)
+        return s + extra
+
 
 LoraEmbeddingType = Type[LoraEmbedding]
 LoraLinearType = Type[LoraLinear]
 LoraConv2dType = Type[LoraConv2d]
 LoraMergedLinearType = Type[LoraMergedLinear]
 LoraLayerType = Union[LoraEmbeddingType, LoraLinearType, LoraConv2dType, LoraMergedLinearType]
```

### Comparing `lora_adapters-0.1.3/src/lora_adapters/utils.py` & `lora_adapters-0.1.4/src/lora_adapters/utils.py`

 * *Files identical despite different names*

### Comparing `lora_adapters-0.1.3/src/lora_adapters.egg-info/PKG-INFO` & `lora_adapters-0.1.4/src/lora_adapters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lora-adapters
-Version: 0.1.3
+Version: 0.1.4
 Summary: PyTorch implementation of low-rank adaptation (LoRA), a parameter-efficient approach to adapt a large pre-trained deep learning model which obtains performance on-par with full fine-tuning.
 Home-page: https://github.com/kiansierra/lora-adapters
 Author: Kian Sierra McGettigan
 Author-email: kiansierra90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lora_adapters-0.1.3/tests/test_bert.py` & `lora_adapters-0.1.4/tests/test_bert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import pytest
 import torch
-from torch import nn
-from torch.optim import AdamW
-from transformers import AutoModel, AutoModelForSequenceClassification
-
 from lora_adapters import (
     LoraEmbedding,
     LoraLinear,
     apply_adapter,
     lora_state_dict,
     mark_only_lora_as_trainable,
     undo_lora,
 )
+from torch import nn
+from torch.optim import AdamW
+from transformers import AutoModel, AutoModelForSequenceClassification
 
 
 def test_bert_initialization():
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     input_tensor = torch.randint(0, 512, (1, 256)).to(device)
     model = AutoModelForSequenceClassification.from_pretrained("bert-base-uncased", num_labels=5).to(device)
     output = model(input_tensor).logits  # Output has to go before adapter because adapter changes model in place
@@ -43,15 +42,15 @@
     model = AutoModelForSequenceClassification.from_pretrained("bert-base-uncased", num_labels=5).to(device)
     model = apply_adapter(model, LoraEmbedding, rank=16, regex_pattern=".*word_embeddings")
     model = apply_adapter(model, LoraLinear, rank=16, regex_pattern=".*query")
     model = apply_adapter(model, LoraLinear, rank=16, regex_pattern=".*value")
     optimizer = AdamW((param for param in model.parameters() if param.requires_grad), lr=1e-3)
     inputs = torch.randint(0, 512, (1, 256)).to(device)
     targets = torch.randint(0, 5, (1,)).to(device)
-    for _ in range(4):
+    for _ in range(2):
         optimizer.zero_grad()
         outputs = model(inputs).logits
         loss = torch.nn.functional.cross_entropy(outputs, targets)
         loss.backward()
         optimizer.step()
 
     model.eval()
@@ -68,15 +67,15 @@
     model = AutoModel.from_pretrained("bert-base-uncased", num_labels=5).to(device)
     model = apply_adapter(model, LoraEmbedding, rank=16, regex_pattern=".*word_embeddings")
     model = apply_adapter(model, LoraLinear, rank=16, regex_pattern=".*query")
     model = apply_adapter(model, LoraLinear, rank=16, regex_pattern=".*value")
     model = mark_only_lora_as_trainable(model, bias=bias)
     optimizer = AdamW((param for param in model.parameters() if param.requires_grad), lr=1e-3)
     inputs = torch.randint(0, 512, (1, 256)).to(device)
-    for _ in range(4):
+    for _ in range(2):
         optimizer.zero_grad()
         outputs = model(inputs).last_hidden_state
         loss = outputs.mean()
         loss.backward()
         optimizer.step()
 
     model.eval()
```

### Comparing `lora_adapters-0.1.3/tests/test_dolly.py` & `lora_adapters-0.1.4/tests/test_dolly.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,41 +9,41 @@
     undo_lora,
 )
 from torch import nn
 from torch.optim import AdamW
 from transformers import AutoModelForCausalLM
 
 
-@pytest.mark.skip(reason="Dolly model is too large to download")
+@pytest.mark.skipif(not torch.cuda.is_available(), reason="Dolly model is too large to download")
 def test_dolly_initialization():
     input_tensor = torch.randint(0, 512, (1, 256)).to("cuda")
     model = AutoModelForCausalLM.from_pretrained(
         "databricks/dolly-v2-3b", device_map="auto", torch_dtype=torch.bfloat16
     )
     output = model(input_tensor).logits  # Output has to go before adapter because adapter changes model in place
     model = apply_adapter(model, LoraEmbedding, rank=16, regex_pattern=".*embed_in")
     model = apply_adapter(model, LoraMergedLinear, rank=16, regex_pattern=".*query_key_value")
     output_lora = model(input_tensor).logits
     assert torch.equal(output, output_lora), "Adapter returns different outputs than original model"
 
 
-@pytest.mark.skip(reason="Dolly model is too large to download")
+@pytest.mark.skipif(not torch.cuda.is_available(), reason="Dolly model is too large to download")
 def test_dolly_conversion():
     model = AutoModelForCausalLM.from_pretrained(
         "databricks/dolly-v2-3b", device_map="auto", torch_dtype=torch.bfloat16
     )
     lora_model = apply_adapter(model, LoraEmbedding, rank=16)
     lora_model = apply_adapter(model, LoraMergedLinear, rank=16, enable_lora=[True])
     original_linear_modules = [module for module in lora_model.modules() if type(module) == nn.Linear]
     assert len(original_linear_modules) == 0, "Adapter Hasn't converted all Linear layers"
     original_emb_modules = [module for module in lora_model.modules() if type(module) == nn.Embedding]
     assert len(original_emb_modules) == 0, "Adapter Hasn't converted all Embedding layers"
 
 
-@pytest.mark.skip(reason="Dolly model is too large to download")
+@pytest.mark.skipif(not torch.cuda.is_available(), reason="Dolly model is too large to download")
 @pytest.mark.parametrize("bias", ["all", "lora_only", "none"])
 def test_dolly_training(bias):
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     model = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-3b", torch_dtype=torch.bfloat16).to(device)
     model = apply_adapter(model, LoraEmbedding, rank=16, regex_pattern=".*embed_in")
     model = apply_adapter(model, LoraMergedLinear, rank=16, regex_pattern=".*0.*query_key_value")
     model = mark_only_lora_as_trainable(model, bias=bias)
@@ -60,15 +60,15 @@
     output_lora = model(inputs).logits
     model = undo_lora(model)
     output = model(inputs).logits
 
     assert torch.equal(output, output_lora), "Adapter returns different outputs than original model after training"
 
 
-@pytest.mark.skip(reason="Dolly model is too large to download")
+@pytest.mark.skipif(not torch.cuda.is_available(), reason="Dolly model is too large to download")
 @pytest.mark.parametrize("bias", ["all", "lora_only", "none"])
 def test_dolly_updates(bias):
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     model = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-3b", torch_dtype=torch.bfloat16).to(device)
     model = apply_adapter(model, LoraEmbedding, rank=16, regex_pattern=".*embed_in")
     model = apply_adapter(model, LoraMergedLinear, rank=16, regex_pattern=".*0.*query_key_value")
     model = mark_only_lora_as_trainable(model, bias=bias)
```

### Comparing `lora_adapters-0.1.3/tests/test_grads.py` & `lora_adapters-0.1.4/tests/test_grads.py`

 * *Files identical despite different names*

### Comparing `lora_adapters-0.1.3/tests/test_layers.py` & `lora_adapters-0.1.4/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `lora_adapters-0.1.3/tests/test_resnet.py` & `lora_adapters-0.1.4/tests/test_resnet.py`

 * *Files identical despite different names*

