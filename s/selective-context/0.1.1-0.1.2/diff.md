# Comparing `tmp/selective-context-0.1.1.tar.gz` & `tmp/selective-context-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selective-context-0.1.1.tar", last modified: Sat May  6 00:26:26 2023, max compression
+gzip compressed data, was "selective-context-0.1.2.tar", last modified: Sat May  6 00:33:59 2023, max compression
```

## Comparing `selective-context-0.1.1.tar` & `selective-context-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:26:26.252134 selective-context-0.1.1/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3817 2023-05-06 00:26:26.250274 selective-context-0.1.1/PKG-INFO
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      670 2023-05-06 00:26:16.000000 selective-context-0.1.1/pyproject.toml
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3318 2023-05-06 00:24:02.000000 selective-context-0.1.1/readme.md
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       38 2023-05-06 00:26:26.253973 selective-context-0.1.1/setup.cfg
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:26:26.186926 selective-context-0.1.1/src/
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:26:26.205498 selective-context-0.1.1/src/selective_context/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)    12988 2023-05-06 00:22:50.000000 selective-context-0.1.1/src/selective_context/__init__.py
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:26:26.241848 selective-context-0.1.1/src/selective_context.egg-info/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3817 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/PKG-INFO
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      282 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/SOURCES.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)        1 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/dependency_links.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       36 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/requires.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       18 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/top_level.txt
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:33:59.821503 selective-context-0.1.2/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3817 2023-05-06 00:33:59.820109 selective-context-0.1.2/PKG-INFO
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      670 2023-05-06 00:33:50.000000 selective-context-0.1.2/pyproject.toml
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3318 2023-05-06 00:24:02.000000 selective-context-0.1.2/readme.md
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       38 2023-05-06 00:33:59.823051 selective-context-0.1.2/setup.cfg
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:33:59.764949 selective-context-0.1.2/src/
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:33:59.780127 selective-context-0.1.2/src/selective_context/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)    12993 2023-05-06 00:33:29.000000 selective-context-0.1.2/src/selective_context/__init__.py
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:33:59.812068 selective-context-0.1.2/src/selective_context.egg-info/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3817 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/PKG-INFO
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      282 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/SOURCES.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)        1 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/dependency_links.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       36 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/requires.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       18 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/top_level.txt
```

### Comparing `selective-context-0.1.1/PKG-INFO` & `selective-context-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selective-context
-Version: 0.1.1
+Version: 0.1.2
 Summary: Compress your prompt and context to let LLMs deal with 2x more content.
 Author-email: Yucheng Li <liyucheng09@gmail.com>
 Project-URL: repository, https://github.com/liyucheng09/Selective_Context
 Keywords: nlp,llms,chatgpt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `selective-context-0.1.1/pyproject.toml` & `selective-context-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "selective-context"
-version = "0.1.1"
+version = "0.1.2"
 description = "Compress your prompt and context to let LLMs deal with 2x more content."
 authors = [{name = "Yucheng Li", email = "liyucheng09@gmail.com"}]
 readme = "readme.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `selective-context-0.1.1/readme.md` & `selective-context-0.1.2/readme.md`

 * *Files identical despite different names*

### Comparing `selective-context-0.1.1/src/selective_context/__init__.py` & `selective-context-0.1.2/src/selective_context/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     def _get_self_info_via_gpt2(self, text: str) -> Tuple[List[str], List[float]]:
         if self.lang == 'en':
             text = f"<|endoftext|>{text}"
         elif self.lang == 'zh':
             text = f"[CLS]{text}"
         with torch.no_grad():
             encoding = self.tokenizer(text, add_special_tokens=False, return_tensors='pt')
-            encoding = encoding.to(DEVICE)
+            encoding = encoding.to(self.device)
             outputs = self.model(**encoding)
             logits = outputs.logits
             probs = torch.softmax(logits, dim=-1)
             self_info = -torch.log(probs)
         
         input_ids = encoding['input_ids']
         input_ids_expaned = input_ids[:, 1:].unsqueeze(-1)
```

### Comparing `selective-context-0.1.1/src/selective_context.egg-info/PKG-INFO` & `selective-context-0.1.2/src/selective_context.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selective-context
-Version: 0.1.1
+Version: 0.1.2
 Summary: Compress your prompt and context to let LLMs deal with 2x more content.
 Author-email: Yucheng Li <liyucheng09@gmail.com>
 Project-URL: repository, https://github.com/liyucheng09/Selective_Context
 Keywords: nlp,llms,chatgpt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

