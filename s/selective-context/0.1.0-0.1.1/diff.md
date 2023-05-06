# Comparing `tmp/selective-context-0.1.0.tar.gz` & `tmp/selective-context-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selective-context-0.1.0.tar", last modified: Sat May  6 00:12:38 2023, max compression
+gzip compressed data, was "selective-context-0.1.1.tar", last modified: Sat May  6 00:26:26 2023, max compression
```

## Comparing `selective-context-0.1.0.tar` & `selective-context-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:12:38.854716 selective-context-0.1.0/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3719 2023-05-06 00:12:38.851866 selective-context-0.1.0/PKG-INFO
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      670 2023-05-06 00:12:28.000000 selective-context-0.1.0/pyproject.toml
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3220 2023-05-05 22:02:39.000000 selective-context-0.1.0/readme.md
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       38 2023-05-06 00:12:38.857358 selective-context-0.1.0/setup.cfg
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:12:38.762572 selective-context-0.1.0/src/
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:12:38.786571 selective-context-0.1.0/src/selective_context/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)    12900 2023-05-05 23:58:42.000000 selective-context-0.1.0/src/selective_context/__init__.py
-drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:12:38.837968 selective-context-0.1.0/src/selective_context.egg-info/
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3719 2023-05-06 00:12:38.000000 selective-context-0.1.0/src/selective_context.egg-info/PKG-INFO
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      282 2023-05-06 00:12:38.000000 selective-context-0.1.0/src/selective_context.egg-info/SOURCES.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)        1 2023-05-06 00:12:38.000000 selective-context-0.1.0/src/selective_context.egg-info/dependency_links.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       36 2023-05-06 00:12:38.000000 selective-context-0.1.0/src/selective_context.egg-info/requires.txt
--rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       18 2023-05-06 00:12:38.000000 selective-context-0.1.0/src/selective_context.egg-info/top_level.txt
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:26:26.252134 selective-context-0.1.1/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3817 2023-05-06 00:26:26.250274 selective-context-0.1.1/PKG-INFO
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      670 2023-05-06 00:26:16.000000 selective-context-0.1.1/pyproject.toml
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3318 2023-05-06 00:24:02.000000 selective-context-0.1.1/readme.md
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       38 2023-05-06 00:26:26.253973 selective-context-0.1.1/setup.cfg
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:26:26.186926 selective-context-0.1.1/src/
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:26:26.205498 selective-context-0.1.1/src/selective_context/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)    12988 2023-05-06 00:22:50.000000 selective-context-0.1.1/src/selective_context/__init__.py
+drwxr-xr-x   0 yl02706  (306860) A-EE00-PGR (5000093)        0 2023-05-06 00:26:26.241848 selective-context-0.1.1/src/selective_context.egg-info/
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)     3817 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/PKG-INFO
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)      282 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/SOURCES.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)        1 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/dependency_links.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       36 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/requires.txt
+-rw-r--r--   0 yl02706  (306860) A-EE00-PGR (5000093)       18 2023-05-06 00:26:26.000000 selective-context-0.1.1/src/selective_context.egg-info/top_level.txt
```

### Comparing `selective-context-0.1.0/PKG-INFO` & `selective-context-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: selective-context
-Version: 0.1.0
+Version: 0.1.1
 Summary: Compress your prompt and context to let LLMs deal with 2x more content.
 Author-email: Yucheng Li <liyucheng09@gmail.com>
 Project-URL: repository, https://github.com/liyucheng09/Selective_Context
 Keywords: nlp,llms,chatgpt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="results/sc.png" alt="Logo of Selective Context" width="auto" height="150" />
+    <img src="https://github.com/liyucheng09/Selective_Context/blob/main/results/sc.png" alt="Logo of Selective Context" width="auto" height="150" />
 </p>
 
 # Selective Context for Large Language Models
 
 Selective Context is a novel approach for optimizing the usage of context in Large Language Models (LLMs) by filtering out less informative content. This approach allows LLMs to process long documents and maintain extended conversations more efficiently without compromising their performance on various tasks. 
 
 This repository contains the code and data for the paper: [Unlocking Context Constraints of LLMs: Enhancing Context Efficiency of LLMs with Self-Information-Based Content Filtering](https://arxiv.org/abs/2304.12102).
@@ -30,31 +30,31 @@
 - **Informativeness Evaluation**: Our method employs a base language model to compute self-information for lexical units (sentences, phrases, or tokens) in a context and use it to evaluate their informativeness.
 - **Extensive Evaluation**: We provide extensive evaluations of Selective Context on three data sources (arxiv papers, BBC news articles, and conversation transcripts) and four different NLP tasks (summarization, question answering, original context reconstruction, and conversation).
 
 ## Getting Started
 
 To get started, follow these steps:
 
-1. Clone the repository:
+1. Install `selective-context` via Pypi:
    ```
-   git clone https://github.com/liyucheng09/Selective_Context.git
-   cd Selective_Context
+   pip install selective-context
    ```
 
-2. Install the required packages:
+2. Import `SelectiveContext`:
    ```
-   pip install -r requirements.txt
+   from selective_context import SelectiveContext
    ```
 
-3. Run the Selective Context demo:
+3. Compress your prompt and context:
    ```
-   python selective_context.py
+   sc = SelectiveContext(model_type='gpt2', lang='en')
+   context, reduced_content = sc(text)
    ```
 
-4. If you prefer to try with web interface, try our streamlit app:
+4. Or, if you prefer to try with web interface, try our streamlit app:
    ```
    streamlit run app/app.py
    ```
 
 ## Code Structure
 
 - `selective_context.py`: A demo for performing context reduction using Selective Context.
```

### Comparing `selective-context-0.1.0/pyproject.toml` & `selective-context-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "selective-context"
-version = "0.1.0"
+version = "0.1.1"
 description = "Compress your prompt and context to let LLMs deal with 2x more content."
 authors = [{name = "Yucheng Li", email = "liyucheng09@gmail.com"}]
 readme = "readme.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `selective-context-0.1.0/readme.md` & `selective-context-0.1.1/src/selective_context.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+Metadata-Version: 2.1
+Name: selective-context
+Version: 0.1.1
+Summary: Compress your prompt and context to let LLMs deal with 2x more content.
+Author-email: Yucheng Li <liyucheng09@gmail.com>
+Project-URL: repository, https://github.com/liyucheng09/Selective_Context
+Keywords: nlp,llms,chatgpt
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 <p align="center">
-    <img src="results/sc.png" alt="Logo of Selective Context" width="auto" height="150" />
+    <img src="https://github.com/liyucheng09/Selective_Context/blob/main/results/sc.png" alt="Logo of Selective Context" width="auto" height="150" />
 </p>
 
 # Selective Context for Large Language Models
 
 Selective Context is a novel approach for optimizing the usage of context in Large Language Models (LLMs) by filtering out less informative content. This approach allows LLMs to process long documents and maintain extended conversations more efficiently without compromising their performance on various tasks. 
 
 This repository contains the code and data for the paper: [Unlocking Context Constraints of LLMs: Enhancing Context Efficiency of LLMs with Self-Information-Based Content Filtering](https://arxiv.org/abs/2304.12102).
@@ -17,31 +30,31 @@
 - **Informativeness Evaluation**: Our method employs a base language model to compute self-information for lexical units (sentences, phrases, or tokens) in a context and use it to evaluate their informativeness.
 - **Extensive Evaluation**: We provide extensive evaluations of Selective Context on three data sources (arxiv papers, BBC news articles, and conversation transcripts) and four different NLP tasks (summarization, question answering, original context reconstruction, and conversation).
 
 ## Getting Started
 
 To get started, follow these steps:
 
-1. Clone the repository:
+1. Install `selective-context` via Pypi:
    ```
-   git clone https://github.com/liyucheng09/Selective_Context.git
-   cd Selective_Context
+   pip install selective-context
    ```
 
-2. Install the required packages:
+2. Import `SelectiveContext`:
    ```
-   pip install -r requirements.txt
+   from selective_context import SelectiveContext
    ```
 
-3. Run the Selective Context demo:
+3. Compress your prompt and context:
    ```
-   python selective_context.py
+   sc = SelectiveContext(model_type='gpt2', lang='en')
+   context, reduced_content = sc(text)
    ```
 
-4. If you prefer to try with web interface, try our streamlit app:
+4. Or, if you prefer to try with web interface, try our streamlit app:
    ```
    streamlit run app/app.py
    ```
 
 ## Code Structure
 
 - `selective_context.py`: A demo for performing context reduction using Selective Context.
@@ -72,8 +85,8 @@
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `selective-context-0.1.0/src/selective_context/__init__.py` & `selective-context-0.1.1/src/selective_context/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 class SelectiveContext:
 
     def __init__(self, model_type = 'gpt2', lang = 'en'):
 
         self.model_type = model_type
         self.lang = lang
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
         # this means we calculate self-information sentence by sentence
         self.sent_level_self_info = True
 
         self._prepare_phrase_tokenizer()
         self.sent_tokenize_pattern = r"(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?)\s"
         self.phrase_mask_token = ''
@@ -69,15 +70,15 @@
             raise NotImplementedError()
         
         if self.model_type == 'gpt2':
             if self.lang == 'zh':
                 self.model = GPT2LMHeadModel.from_pretrained('uer/gpt2-chinese-cluecorpussmall')
             else:
                 self.model = GPT2LMHeadModel.from_pretrained('gpt2')
-            self.model.to(DEVICE)
+            self.model.to(self.device)
             self.model.eval()
 
             print('model loaded')
 
             self.max_token_length = self.model.config.n_positions
             self.get_self_information = self._get_self_info_via_gpt2
```

### Comparing `selective-context-0.1.0/src/selective_context.egg-info/PKG-INFO` & `selective-context-0.1.1/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-Metadata-Version: 2.1
-Name: selective-context
-Version: 0.1.0
-Summary: Compress your prompt and context to let LLMs deal with 2x more content.
-Author-email: Yucheng Li <liyucheng09@gmail.com>
-Project-URL: repository, https://github.com/liyucheng09/Selective_Context
-Keywords: nlp,llms,chatgpt
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 <p align="center">
-    <img src="results/sc.png" alt="Logo of Selective Context" width="auto" height="150" />
+    <img src="https://github.com/liyucheng09/Selective_Context/blob/main/results/sc.png" alt="Logo of Selective Context" width="auto" height="150" />
 </p>
 
 # Selective Context for Large Language Models
 
 Selective Context is a novel approach for optimizing the usage of context in Large Language Models (LLMs) by filtering out less informative content. This approach allows LLMs to process long documents and maintain extended conversations more efficiently without compromising their performance on various tasks. 
 
 This repository contains the code and data for the paper: [Unlocking Context Constraints of LLMs: Enhancing Context Efficiency of LLMs with Self-Information-Based Content Filtering](https://arxiv.org/abs/2304.12102).
@@ -30,31 +17,31 @@
 - **Informativeness Evaluation**: Our method employs a base language model to compute self-information for lexical units (sentences, phrases, or tokens) in a context and use it to evaluate their informativeness.
 - **Extensive Evaluation**: We provide extensive evaluations of Selective Context on three data sources (arxiv papers, BBC news articles, and conversation transcripts) and four different NLP tasks (summarization, question answering, original context reconstruction, and conversation).
 
 ## Getting Started
 
 To get started, follow these steps:
 
-1. Clone the repository:
+1. Install `selective-context` via Pypi:
    ```
-   git clone https://github.com/liyucheng09/Selective_Context.git
-   cd Selective_Context
+   pip install selective-context
    ```
 
-2. Install the required packages:
+2. Import `SelectiveContext`:
    ```
-   pip install -r requirements.txt
+   from selective_context import SelectiveContext
    ```
 
-3. Run the Selective Context demo:
+3. Compress your prompt and context:
    ```
-   python selective_context.py
+   sc = SelectiveContext(model_type='gpt2', lang='en')
+   context, reduced_content = sc(text)
    ```
 
-4. If you prefer to try with web interface, try our streamlit app:
+4. Or, if you prefer to try with web interface, try our streamlit app:
    ```
    streamlit run app/app.py
    ```
 
 ## Code Structure
 
 - `selective_context.py`: A demo for performing context reduction using Selective Context.
@@ -85,8 +72,8 @@
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

