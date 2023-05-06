# Comparing `tmp/auto-eval-0.1.5.tar.gz` & `tmp/auto-eval-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.1.5.tar", last modified: Fri May  5 09:52:56 2023, max compression
+gzip compressed data, was "auto-eval-0.1.6.tar", last modified: Sat May  6 02:35:57 2023, max compression
```

## Comparing `auto-eval-0.1.5.tar` & `auto-eval-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.353049 auto-eval-0.1.5/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.5/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    11478 2023-05-05 09:52:56.352689 auto-eval-0.1.5/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    11052 2023-05-05 09:05:05.000000 auto-eval-0.1.5/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.347443 auto-eval-0.1.5/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    11478 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      445 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       54 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.347947 auto-eval-0.1.5/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.5/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3909 2023-05-05 08:12:59.000000 auto-eval-0.1.5/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.349718 auto-eval-0.1.5/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      131 2023-05-05 08:11:08.000000 auto-eval-0.1.5/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     7003 2023-05-05 09:26:08.000000 auto-eval-0.1.5/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.351443 auto-eval-0.1.5/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.5/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      773 2023-05-05 07:29:57.000000 auto-eval-0.1.5/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     2948 2023-05-05 08:21:30.000000 auto-eval-0.1.5/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-05 09:52:56.353126 auto-eval-0.1.5/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      940 2023-05-05 09:52:44.000000 auto-eval-0.1.5/setup.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.352121 auto-eval-0.1.5/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.5/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2911 2023-05-05 09:52:25.000000 auto-eval-0.1.5/utils/data_utils.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.660247 auto-eval-0.1.6/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.6/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11478 2023-05-06 02:35:57.660019 auto-eval-0.1.6/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11052 2023-05-05 09:05:05.000000 auto-eval-0.1.6/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.657363 auto-eval-0.1.6/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11478 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      445 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       54 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.657621 auto-eval-0.1.6/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.6/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3909 2023-05-06 02:28:33.000000 auto-eval-0.1.6/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.658261 auto-eval-0.1.6/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      131 2023-05-05 08:11:08.000000 auto-eval-0.1.6/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7001 2023-05-06 02:22:59.000000 auto-eval-0.1.6/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.659140 auto-eval-0.1.6/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.6/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      775 2023-05-06 02:34:00.000000 auto-eval-0.1.6/prompt_template/eval_prompt_template.json
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2949 2023-05-06 02:34:42.000000 auto-eval-0.1.6/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-06 02:35:57.660297 auto-eval-0.1.6/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      940 2023-05-06 02:35:01.000000 auto-eval-0.1.6/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.659644 auto-eval-0.1.6/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.6/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2911 2023-05-05 09:52:25.000000 auto-eval-0.1.6/utils/data_utils.py
```

### Comparing `auto-eval-0.1.5/LICENSE` & `auto-eval-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.5/PKG-INFO` & `auto-eval-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.5
+Version: 0.1.6
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.1.5/README.md` & `auto-eval-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.5/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.1.6/auto_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.5
+Version: 0.1.6
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.1.5/commands/auto_eval.py` & `auto-eval-0.1.6/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.5/eval/auto_llms_eval.py` & `auto-eval-0.1.6/eval/auto_llms_eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def eval_one_qa(
              api_tool: OneAPITool,
              eval_prompter: Prompter,
              question: str,
              candidate_answers: List[str],
-             target: Union[str, None]=None,
+             target: Union[str, None]='',
              model: str='',
              temperature=0.1,
              max_new_tokens=2048) -> Tuple[Union[List[float], None], str]:
     raw_response = ''
     eval_prompt = eval_prompter.generate_prompt(question, target,
                                                 candidate_answers)
     try:
```

### Comparing `auto-eval-0.1.5/prompt_template/eval_prompt_template.json` & `auto-eval-0.1.6/prompt_template/eval_prompt_template.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'eval_with_target_template'": "'[Question]: {question}\\n\\n[Correct answer]: "*

 * *                                '{target}\\n\\n[Candidate '*

 * *                                'answer]:\\n{answers}\\n\\n[System]:\\nPlease evaluate and comment '*

 * *                                'each [Candidate answer] based on the [Correct answer]. Then '*

 * *                                'output all [Candidate answer] scores (0-1) in a summary format of '*

 * *                                '{{"number": "score"}}, e.g, {{"A": "0.2" […]*

```diff
@@ -1,4 +1,4 @@
 {
-    "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}",
-    "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}"
+    "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}.",
+    "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}."
 }
```

### Comparing `auto-eval-0.1.5/prompt_template/prompter.py` & `auto-eval-0.1.6/prompt_template/prompter.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         Generate a prompt based on the given question, target, and candidate answers.
         """
         candidate_answer_numbers = generate_letters(len(candidate_answers))
         format_option_data = '\n'.join([
             f'**{candidate_answer_numbers[i]}**. {candidate_answers[i]}'
             for i in range(len(candidate_answers))
         ])
+
         if target:
             eval_prompt = self.eval_with_target_template.format(
                 question=question, target=target, answers=format_option_data)
         else:
             eval_prompt = self.eval_without_target_template.format(
                 question=question, answers=format_option_data)
         if self._verbose:
```

### Comparing `auto-eval-0.1.5/setup.py` & `auto-eval-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     package_data={
       "prompt_template":["eval_prompt_template.json"]  
     },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

### Comparing `auto-eval-0.1.5/utils/data_utils.py` & `auto-eval-0.1.6/utils/data_utils.py`

 * *Files identical despite different names*

