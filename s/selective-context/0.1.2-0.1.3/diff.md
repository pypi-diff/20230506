# Comparing `tmp/selective-context-0.1.2.tar.gz` & `tmp/selective-context-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selective-context-0.1.2.tar", last modified: Sat May  6 00:33:59 2023, max compression
+gzip compressed data, was "selective-context-0.1.3.tar", last modified: Sat May  6 00:39:27 2023, max compression
```

## Comparing `selective-context-0.1.2.tar` & `selective-context-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:33:59.821503 selective-context-0.1.2/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3817 2023-05-06 00:33:59.820109 selective-context-0.1.2/PKG-INFO
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      670 2023-05-06 00:33:50.000000 selective-context-0.1.2/pyproject.toml
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3318 2023-05-06 00:24:02.000000 selective-context-0.1.2/readme.md
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       38 2023-05-06 00:33:59.823051 selective-context-0.1.2/setup.cfg
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:33:59.764949 selective-context-0.1.2/src/
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:33:59.780127 selective-context-0.1.2/src/selective_context/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)    12993 2023-05-06 00:33:29.000000 selective-context-0.1.2/src/selective_context/__init__.py
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:33:59.812068 selective-context-0.1.2/src/selective_context.egg-info/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3817 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/PKG-INFO
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      282 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/SOURCES.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)        1 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/dependency_links.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       36 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/requires.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       18 2023-05-06 00:33:59.000000 selective-context-0.1.2/src/selective_context.egg-info/top_level.txt
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:39:27.357134 selective-context-0.1.3/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     4041 2023-05-06 00:39:27.355512 selective-context-0.1.3/PKG-INFO
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      670 2023-05-06 00:39:07.000000 selective-context-0.1.3/pyproject.toml
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3542 2023-05-06 00:38:46.000000 selective-context-0.1.3/readme.md
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       38 2023-05-06 00:39:27.358815 selective-context-0.1.3/setup.cfg
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:39:27.297281 selective-context-0.1.3/src/
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:39:27.313669 selective-context-0.1.3/src/selective_context/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)    12961 2023-05-06 00:36:47.000000 selective-context-0.1.3/src/selective_context/__init__.py
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:39:27.347362 selective-context-0.1.3/src/selective_context.egg-info/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     4041 2023-05-06 00:39:27.000000 selective-context-0.1.3/src/selective_context.egg-info/PKG-INFO
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      282 2023-05-06 00:39:27.000000 selective-context-0.1.3/src/selective_context.egg-info/SOURCES.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)        1 2023-05-06 00:39:27.000000 selective-context-0.1.3/src/selective_context.egg-info/dependency_links.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       36 2023-05-06 00:39:27.000000 selective-context-0.1.3/src/selective_context.egg-info/requires.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       18 2023-05-06 00:39:27.000000 selective-context-0.1.3/src/selective_context.egg-info/top_level.txt
```

### Comparing `selective-context-0.1.2/PKG-INFO` & `selective-context-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selective-context
-Version: 0.1.2
+Version: 0.1.3
 Summary: Compress your prompt and context to let LLMs deal with 2x more content.
 Author-email: Yucheng Li <liyucheng09@gmail.com>
 Project-URL: repository, https://github.com/liyucheng09/Selective_Context
 Keywords: nlp,llms,chatgpt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -46,18 +46,24 @@
 
 3. Compress your prompt and context:
    ```
    sc = SelectiveContext(model_type='gpt2', lang='en')
    context, reduced_content = sc(text)
    ```
 
-4. Or, if you prefer to try with web interface, try our streamlit app:
+4. You can also adjust the reduce ratio:
+   ```
+   context, reduced_content = sc(text, reduce_ratio = 0.5)
+   ```
+
+5. If you prefer to try with web interface, try our streamlit app:
    ```
    streamlit run app/app.py
    ```
+   Or directly visit our [Space](https://huggingface.co/spaces/liyucheng/selective_context) on Hugging Face Hub.
 
 ## Code Structure
 
 - `selective_context.py`: A demo for performing context reduction using Selective Context.
 - `context_manager.py`: The main module for managing context and implementing the Selective Context algorithm.
 - `main.py`: The main script for running experiments and evaluating the effectiveness of Selective Context.
 - `qa_manager.py`: A helper module for managing question answering tasks during the experiments.
```

### Comparing `selective-context-0.1.2/pyproject.toml` & `selective-context-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "selective-context"
-version = "0.1.2"
+version = "0.1.3"
 description = "Compress your prompt and context to let LLMs deal with 2x more content."
 authors = [{name = "Yucheng Li", email = "liyucheng09@gmail.com"}]
 readme = "readme.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `selective-context-0.1.2/readme.md` & `selective-context-0.1.3/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,24 @@
 
 3. Compress your prompt and context:
    ```
    sc = SelectiveContext(model_type='gpt2', lang='en')
    context, reduced_content = sc(text)
    ```
 
-4. Or, if you prefer to try with web interface, try our streamlit app:
+4. You can also adjust the reduce ratio:
+   ```
+   context, reduced_content = sc(text, reduce_ratio = 0.5)
+   ```
+
+5. If you prefer to try with web interface, try our streamlit app:
    ```
    streamlit run app/app.py
    ```
+   Or directly visit our [Space](https://huggingface.co/spaces/liyucheng/selective_context) on Hugging Face Hub.
 
 ## Code Structure
 
 - `selective_context.py`: A demo for performing context reduction using Selective Context.
 - `context_manager.py`: The main module for managing context and implementing the Selective Context algorithm.
 - `main.py`: The main script for running experiments and evaluating the effectiveness of Selective Context.
 - `qa_manager.py`: A helper module for managing question answering tasks during the experiments.
```

### Comparing `selective-context-0.1.2/src/selective_context/__init__.py` & `selective-context-0.1.3/src/selective_context/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             sent_self_info = []
             all_noun_phrases = []
             all_noun_phrases_info = []
             all_tokens = []
             all_token_self_info = []
 
             for sent in sents:
-                print(sent)
+                # print(sent)
                 tokens, self_info = self.get_self_information(sent)
                 sent_self_info.append(np.mean(self_info))
 
                 all_tokens.extend(tokens)
                 all_token_self_info.extend(self_info)
 
                 noun_phrases, noun_phrases_info = self._calculate_lexical_unit(tokens, self_info)
@@ -273,15 +273,14 @@
 
         sents = re.split(self.sent_tokenize_pattern, context)
         sents = [sent.strip() for sent in sents if sent.strip()]
 
         # You want the reduce happen at sentence level, phrase level, or token level?
         assert reduce_level in ['sent', 'phrase', 'token'], f"reduce_level should be one of ['sent', 'phrase', 'token'], got {reduce_level}"
         sent_lus, phrase_lus, token_lus = self._lexical_unit(sents)
-        print(phrase_lus, '^^^^')
         lexical_level = {
             'sent': sent_lus,
             'phrase': phrase_lus,
             'token': token_lus
         }
 
         # context is the reduced context, masked_sents denotes what context has been filtered out
```

### Comparing `selective-context-0.1.2/src/selective_context.egg-info/PKG-INFO` & `selective-context-0.1.3/src/selective_context.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selective-context
-Version: 0.1.2
+Version: 0.1.3
 Summary: Compress your prompt and context to let LLMs deal with 2x more content.
 Author-email: Yucheng Li <liyucheng09@gmail.com>
 Project-URL: repository, https://github.com/liyucheng09/Selective_Context
 Keywords: nlp,llms,chatgpt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -46,18 +46,24 @@
 
 3. Compress your prompt and context:
    ```
    sc = SelectiveContext(model_type='gpt2', lang='en')
    context, reduced_content = sc(text)
    ```
 
-4. Or, if you prefer to try with web interface, try our streamlit app:
+4. You can also adjust the reduce ratio:
+   ```
+   context, reduced_content = sc(text, reduce_ratio = 0.5)
+   ```
+
+5. If you prefer to try with web interface, try our streamlit app:
    ```
    streamlit run app/app.py
    ```
+   Or directly visit our [Space](https://huggingface.co/spaces/liyucheng/selective_context) on Hugging Face Hub.
 
 ## Code Structure
 
 - `selective_context.py`: A demo for performing context reduction using Selective Context.
 - `context_manager.py`: The main module for managing context and implementing the Selective Context algorithm.
 - `main.py`: The main script for running experiments and evaluating the effectiveness of Selective Context.
 - `qa_manager.py`: A helper module for managing question answering tasks during the experiments.
```

