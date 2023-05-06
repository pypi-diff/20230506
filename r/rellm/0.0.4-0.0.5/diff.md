# Comparing `tmp/rellm-0.0.4.tar.gz` & `tmp/rellm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rellm-0.0.4.tar", max compression
+gzip compressed data, was "rellm-0.0.5.tar", max compression
```

## Comparing `rellm-0.0.4.tar` & `rellm-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-05-05 02:22:49.141576 rellm-0.0.4/LICENSE
--rw-r--r--   0        0        0     3733 2023-05-05 20:38:55.654909 rellm-0.0.4/README.md
--rw-r--r--   0        0        0     1265 2023-05-06 01:55:32.151765 rellm-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-06 01:33:25.476799 rellm-0.0.4/rellm/__init__.py
--rw-r--r--   0        0        0     3374 2023-05-06 01:55:26.434270 rellm-0.0.4/rellm/rellm.py
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 rellm-0.0.4/setup.py
--rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 rellm-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-05 02:22:49.141576 rellm-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3691 2023-05-06 21:38:01.448274 rellm-0.0.5/README.md
+-rw-r--r--   0        0        0     1265 2023-05-06 21:39:31.895229 rellm-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-05-06 21:30:57.315833 rellm-0.0.5/rellm/__init__.py
+-rw-r--r--   0        0        0      549 2023-05-06 21:27:59.330686 rellm-0.0.5/rellm/logits_mask.py
+-rw-r--r--   0        0        0     1345 2023-05-06 21:28:37.107735 rellm-0.0.5/rellm/re_token_filter.py
+-rw-r--r--   0        0        0     1978 2023-05-06 21:30:38.269871 rellm-0.0.5/rellm/rellm.py
+-rw-r--r--   0        0        0     4596 1970-01-01 00:00:00.000000 rellm-0.0.5/setup.py
+-rw-r--r--   0        0        0     5197 1970-01-01 00:00:00.000000 rellm-0.0.5/PKG-INFO
```

### Comparing `rellm-0.0.4/LICENSE` & `rellm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rellm-0.0.4/README.md` & `rellm-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 How does it work? ReLLM filters non-matching tokens pre-generation. For each token, ReLLM tests every possible completion against a partial regex. For the potential completions that do not match the pattern, ReLLM masks the logits so that the language model does not generate them.
 
 ### Installation
 ```
 pip install rellm
 ```
 
-The preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the examples below (you can run them with [example.py](example.py))
+The preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the [examples](examples).
 
 ```python
 import regex
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from rellm import complete_re
```

### Comparing `rellm-0.0.4/pyproject.toml` & `rellm-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rellm"
-version = "0.0.4"
+version = "0.0.5"
 description = "Get exact structure out of any language models with regular expressions."
 authors = ["Matt Rickard <pypi@matt-rickard.com>"]
 maintainers = ["Matt Rickard <pypi@matt-rickard.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = [
   "llm",
```

### Comparing `rellm-0.0.4/setup.py` & `rellm-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['numpy>=1.24.3,<2.0.0',
  'regex>=2023.5.5,<2024.0.0',
  'torch>=2.0.0,<3.0.0',
  'transformers>=4.28.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'rellm',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Get exact structure out of any language models with regular expressions.',
-    'long_description': '# ReLLM\nRegular Expressions for Language Model Completions.\n\n> *Some people, when confronted with a problem, think\n“I know, I\'ll use regular expressions.”   Now they have two problems.*\n\nExact structure out of any language model completion with regular expressions.\n\nReturn specific syntactic structure (e.g. JSON or XML), or specific semantic structure (e.g. a date or a number), or even complete templates (e.g. a sentence with a blank to fill in).\n\nHow does it work? ReLLM filters non-matching tokens pre-generation. For each token, ReLLM tests every possible completion against a partial regex. For the potential completions that do not match the pattern, ReLLM masks the logits so that the language model does not generate them.\n\n### Installation\n```\npip install rellm\n```\n\nThe preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the examples below (you can run them with [example.py](example.py))\n\n```python\nimport regex\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom rellm import complete_re\n\nmodel = AutoModelForCausalLM.from_pretrained("gpt2")\ntokenizer = AutoTokenizer.from_pretrained("gpt2")\n\nprompt = "ReLLM, the best way to get structured data out of LLMs, is an acronym for "\npattern = regex.compile(r\'Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+\')\noutput = complete_re(tokenizer=tokenizer, \n                     model=model, \n                     prompt=prompt,\n                     pattern=pattern,\n                     do_sample=True,\n                     max_new_tokens=80)\nprint(output)\n```\n\n```\n> Realized Logistic Logistics Model\n```\n\n\n## Examples using GPT2 (124 million parameters)\n\n#\n\nUsing GPT2 (124m)\n\n**Prompt**: ReLLM, the best way to get structured data out of LLMs, is an acronym for\n\n**Pattern**: Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+\n\n**ReLLM**: Realized Logistic Logistics Model\n\n**Without ReLLM**: Largest Largest Address Space (MELSP), which has its roots in the  Internet network, at least when compared\n#\n\n**Prompt**: Return the first three letters of the alphabet in a json array:\n\n**Pattern** \\[\\"[a-z]\\", \\"[a-z]\\", \\"[a-z]\\"\\]\n\n**ReLLM**: ["a", "b", "c"]\n\n**Without ReLLM**: { "index": 0, "id":"1", "description":"", "text": "[{ "id": 0, "name":\n#\n**Prompt**: Fill in the sentence with an interesting story about the dentist:\n\n**Pattern**: Today I\\\'m going to the [a-z]+ to [a-z]+ because ([a-z]+ )*\\.\n\n**ReLLM**: Today I\'m going to the dentist to see because it is a very important day for me\n\n**Without ReLLM**: \'My family bought me an appointment with a dentist when I was 15. The dentist gave me one a year and then I was told on\n#\n\n**Prompt**: Is this a good demo?\n\n**Pattern**: (Yes|No)\n\n**ReLLM**: No.\n\n**Without ReLLM**: I don\'t know, but this is amazing! Even more amazing is how the design can take place on a small stage that uses LEDs.\nAs\n\n#\n\n**Prompt**: Convert the date May 4, 2023 to the format mm/dd/yyyy:\n\n**Pattern**: [0-9]{2}/[0-9]{2}/[0-9]{4}\n\n**ReLLM**: 00/00/0045\n\n**Without ReLLM**:  mm:ss\n\nA-Z, Z-A, W-H (0-9:9:19)\n\nZ-R\n\n#\n\n**Prompt**: Jeff Dean is a\n\n**Pattern** (Programmer|Computer Scientist|AGI)\n\n**ReLLM**: Computer Scientist\n\n**Without ReLLM**: former national basketball champion and a former professional basketball player. He currently serves as general counsel for the NCAA Office of the Vice President for Academic Affairs.\n\n#\n\n**Prompt**: I can eat \n\n**Pattern**: [0-9]{1,10} [a-z]* of [a-z]*\n\n**ReLLM**: 800 calories of coffee\n\n**Without ReLLM**: iced coffee here on the west side and do this, so can you?"\n\n"Why, I don\'t understand. What did you mean by',
+    'long_description': '# ReLLM\nRegular Expressions for Language Model Completions.\n\n> *Some people, when confronted with a problem, think\n“I know, I\'ll use regular expressions.”   Now they have two problems.*\n\nExact structure out of any language model completion with regular expressions.\n\nReturn specific syntactic structure (e.g. JSON or XML), or specific semantic structure (e.g. a date or a number), or even complete templates (e.g. a sentence with a blank to fill in).\n\nHow does it work? ReLLM filters non-matching tokens pre-generation. For each token, ReLLM tests every possible completion against a partial regex. For the potential completions that do not match the pattern, ReLLM masks the logits so that the language model does not generate them.\n\n### Installation\n```\npip install rellm\n```\n\nThe preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the [examples](examples).\n\n```python\nimport regex\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom rellm import complete_re\n\nmodel = AutoModelForCausalLM.from_pretrained("gpt2")\ntokenizer = AutoTokenizer.from_pretrained("gpt2")\n\nprompt = "ReLLM, the best way to get structured data out of LLMs, is an acronym for "\npattern = regex.compile(r\'Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+\')\noutput = complete_re(tokenizer=tokenizer, \n                     model=model, \n                     prompt=prompt,\n                     pattern=pattern,\n                     do_sample=True,\n                     max_new_tokens=80)\nprint(output)\n```\n\n```\n> Realized Logistic Logistics Model\n```\n\n\n## Examples using GPT2 (124 million parameters)\n\n#\n\nUsing GPT2 (124m)\n\n**Prompt**: ReLLM, the best way to get structured data out of LLMs, is an acronym for\n\n**Pattern**: Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+\n\n**ReLLM**: Realized Logistic Logistics Model\n\n**Without ReLLM**: Largest Largest Address Space (MELSP), which has its roots in the  Internet network, at least when compared\n#\n\n**Prompt**: Return the first three letters of the alphabet in a json array:\n\n**Pattern** \\[\\"[a-z]\\", \\"[a-z]\\", \\"[a-z]\\"\\]\n\n**ReLLM**: ["a", "b", "c"]\n\n**Without ReLLM**: { "index": 0, "id":"1", "description":"", "text": "[{ "id": 0, "name":\n#\n**Prompt**: Fill in the sentence with an interesting story about the dentist:\n\n**Pattern**: Today I\\\'m going to the [a-z]+ to [a-z]+ because ([a-z]+ )*\\.\n\n**ReLLM**: Today I\'m going to the dentist to see because it is a very important day for me\n\n**Without ReLLM**: \'My family bought me an appointment with a dentist when I was 15. The dentist gave me one a year and then I was told on\n#\n\n**Prompt**: Is this a good demo?\n\n**Pattern**: (Yes|No)\n\n**ReLLM**: No.\n\n**Without ReLLM**: I don\'t know, but this is amazing! Even more amazing is how the design can take place on a small stage that uses LEDs.\nAs\n\n#\n\n**Prompt**: Convert the date May 4, 2023 to the format mm/dd/yyyy:\n\n**Pattern**: [0-9]{2}/[0-9]{2}/[0-9]{4}\n\n**ReLLM**: 00/00/0045\n\n**Without ReLLM**:  mm:ss\n\nA-Z, Z-A, W-H (0-9:9:19)\n\nZ-R\n\n#\n\n**Prompt**: Jeff Dean is a\n\n**Pattern** (Programmer|Computer Scientist|AGI)\n\n**ReLLM**: Computer Scientist\n\n**Without ReLLM**: former national basketball champion and a former professional basketball player. He currently serves as general counsel for the NCAA Office of the Vice President for Academic Affairs.\n\n#\n\n**Prompt**: I can eat \n\n**Pattern**: [0-9]{1,10} [a-z]* of [a-z]*\n\n**ReLLM**: 800 calories of coffee\n\n**Without ReLLM**: iced coffee here on the west side and do this, so can you?"\n\n"Why, I don\'t understand. What did you mean by',
     'author': 'Matt Rickard',
     'author_email': 'pypi@matt-rickard.com',
     'maintainer': 'Matt Rickard',
     'maintainer_email': 'pypi@matt-rickard.com',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `rellm-0.0.4/PKG-INFO` & `rellm-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rellm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get exact structure out of any language models with regular expressions.
 License: MIT
 Keywords: llm,ai,prompt,large language models,gpt-3,chatgpt
 Author: Matt Rickard
 Author-email: pypi@matt-rickard.com
 Maintainer: Matt Rickard
 Maintainer-email: pypi@matt-rickard.com
@@ -46,15 +46,15 @@
 How does it work? ReLLM filters non-matching tokens pre-generation. For each token, ReLLM tests every possible completion against a partial regex. For the potential completions that do not match the pattern, ReLLM masks the logits so that the language model does not generate them.
 
 ### Installation
 ```
 pip install rellm
 ```
 
-The preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the examples below (you can run them with [example.py](example.py))
+The preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the [examples](examples).
 
 ```python
 import regex
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from rellm import complete_re
```

