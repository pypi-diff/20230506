# Comparing `tmp/decat-1.0.2.tar.gz` & `tmp/decat-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decat-1.0.2.tar", last modified: Mon Feb 14 15:02:43 2022, max compression
+gzip compressed data, was "decat-1.0.3.tar", last modified: Sat May  6 19:10:17 2023, max compression
```

## Comparing `decat-1.0.2.tar` & `decat-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.983644 decat-1.0.2/
--rw-r--r--   0 mandeepsingh   (501) staff       (20)     1069 2021-09-10 11:13:20.000000 decat-1.0.2/LICENSE
--rw-r--r--   0 mandeepsingh   (501) staff       (20)      124 2021-09-11 14:22:33.000000 decat-1.0.2/MANIFEST.in
--rw-r--r--   0 mandeepsingh   (501) staff       (20)     4392 2022-02-14 15:02:43.983749 decat-1.0.2/PKG-INFO
--rw-r--r--   0 mandeepsingh   (501) staff       (20)     3505 2021-09-11 16:56:24.000000 decat-1.0.2/README.md
--rw-r--r--   0 mandeepsingh   (501) staff       (20)      104 2021-09-11 14:22:33.000000 decat-1.0.2/pyproject.toml
--rw-r--r--   0 mandeepsingh   (501) staff       (20)     1020 2022-02-14 15:02:43.984185 decat-1.0.2/setup.cfg
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.963631 decat-1.0.2/src/
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.965376 decat-1.0.2/src/decat/
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.966344 decat-1.0.2/src/decat/.data/
--rw-r--r--   0 mandeepsingh   (501) staff       (20)        0 2021-09-11 14:22:33.000000 decat-1.0.2/src/decat/.data/__init__.py
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.963804 decat-1.0.2/src/decat/.data/vocabulary/
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.969926 decat-1.0.2/src/decat/.data/vocabulary/en/
--rw-r--r--   0 mandeepsingh   (501) staff       (20)  2799401 2021-09-11 14:22:33.000000 decat-1.0.2/src/decat/.data/vocabulary/en/frequency.json
--rw-r--r--   0 mandeepsingh   (501) staff       (20)  4156659 2021-09-11 14:22:33.000000 decat-1.0.2/src/decat/.data/vocabulary/en/tokens.json
--rw-r--r--   0 mandeepsingh   (501) staff       (20)     1441 2022-02-14 14:41:56.000000 decat-1.0.2/src/decat/__init__.py
--rw-r--r--   0 mandeepsingh   (501) staff       (20)      114 2022-01-30 19:22:13.000000 decat-1.0.2/src/decat/__main__.py
--rw-r--r--   0 mandeepsingh   (501) staff       (20)      742 2022-01-30 19:22:13.000000 decat-1.0.2/src/decat/__settings__.py
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.979752 decat-1.0.2/src/decat/core/
--rw-r--r--   0 mandeepsingh   (501) staff       (20)       57 2021-09-11 14:22:33.000000 decat-1.0.2/src/decat/core/__init__.py
--rw-r--r--   0 mandeepsingh   (501) staff       (20)     6738 2022-02-14 14:55:08.000000 decat-1.0.2/src/decat/core/model.py
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.979871 decat-1.0.2/src/decat/parsers/
--rw-r--r--   0 mandeepsingh   (501) staff       (20)       55 2021-09-11 14:22:33.000000 decat-1.0.2/src/decat/parsers/__init__.py
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.983496 decat-1.0.2/src/decat/parsers/input_parser/
--rw-r--r--   0 mandeepsingh   (501) staff       (20)       63 2021-09-11 14:22:33.000000 decat-1.0.2/src/decat/parsers/input_parser/__init__.py
--rw-r--r--   0 mandeepsingh   (501) staff       (20)     1668 2022-02-14 14:41:56.000000 decat-1.0.2/src/decat/parsers/input_parser/_parser.py
--rw-r--r--   0 mandeepsingh   (501) staff       (20)      391 2021-09-11 14:22:33.000000 decat-1.0.2/src/decat/parsers/input_parser/_validators.py
-drwxr-xr-x   0 mandeepsingh   (501) staff       (20)        0 2022-02-14 15:02:43.966220 decat-1.0.2/src/decat.egg-info/
--rw-r--r--   0 mandeepsingh   (501) staff       (20)     4392 2022-02-14 15:02:43.000000 decat-1.0.2/src/decat.egg-info/PKG-INFO
--rw-r--r--   0 mandeepsingh   (501) staff       (20)      619 2022-02-14 15:02:43.000000 decat-1.0.2/src/decat.egg-info/SOURCES.txt
--rw-r--r--   0 mandeepsingh   (501) staff       (20)        1 2022-02-14 15:02:43.000000 decat-1.0.2/src/decat.egg-info/dependency_links.txt
--rw-r--r--   0 mandeepsingh   (501) staff       (20)       37 2022-02-14 15:02:43.000000 decat-1.0.2/src/decat.egg-info/entry_points.txt
--rw-r--r--   0 mandeepsingh   (501) staff       (20)        6 2022-02-14 15:02:43.000000 decat-1.0.2/src/decat.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.106633 decat-1.0.3/
+-rw-r--r--   0 home       (501) staff       (20)     1069 2023-05-06 18:50:17.000000 decat-1.0.3/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)      124 2023-05-06 18:50:17.000000 decat-1.0.3/MANIFEST.in
+-rw-r--r--   0 home       (501) staff       (20)     4230 2023-05-06 19:10:17.106714 decat-1.0.3/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     3363 2023-05-06 18:57:39.000000 decat-1.0.3/README.md
+-rw-r--r--   0 home       (501) staff       (20)      104 2023-05-06 18:50:17.000000 decat-1.0.3/pyproject.toml
+-rw-r--r--   0 home       (501) staff       (20)     1020 2023-05-06 19:10:17.107078 decat-1.0.3/setup.cfg
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.089835 decat-1.0.3/src/
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.092175 decat-1.0.3/src/decat/
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.093181 decat-1.0.3/src/decat/.data/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/.data/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.090108 decat-1.0.3/src/decat/.data/vocabulary/
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.097138 decat-1.0.3/src/decat/.data/vocabulary/en/
+-rw-r--r--   0 home       (501) staff       (20)  2799401 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/.data/vocabulary/en/frequency.json
+-rw-r--r--   0 home       (501) staff       (20)  4156659 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/.data/vocabulary/en/tokens.json
+-rw-r--r--   0 home       (501) staff       (20)     1132 2023-05-06 18:52:37.000000 decat-1.0.3/src/decat/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)      114 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/__main__.py
+-rw-r--r--   0 home       (501) staff       (20)      742 2023-05-06 19:02:00.000000 decat-1.0.3/src/decat/__settings__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.104950 decat-1.0.3/src/decat/core/
+-rw-r--r--   0 home       (501) staff       (20)       57 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/core/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     6738 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/core/model.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.105761 decat-1.0.3/src/decat/parsers/
+-rw-r--r--   0 home       (501) staff       (20)       55 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/parsers/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.106460 decat-1.0.3/src/decat/parsers/input_parser/
+-rw-r--r--   0 home       (501) staff       (20)       63 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/parsers/input_parser/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     1668 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/parsers/input_parser/_parser.py
+-rw-r--r--   0 home       (501) staff       (20)      391 2023-05-06 18:50:17.000000 decat-1.0.3/src/decat/parsers/input_parser/_validators.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-06 19:10:17.093016 decat-1.0.3/src/decat.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)     4230 2023-05-06 19:10:17.000000 decat-1.0.3/src/decat.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      619 2023-05-06 19:10:17.000000 decat-1.0.3/src/decat.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-06 19:10:17.000000 decat-1.0.3/src/decat.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       37 2023-05-06 19:10:17.000000 decat-1.0.3/src/decat.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)        6 2023-05-06 19:10:17.000000 decat-1.0.3/src/decat.egg-info/top_level.txt
```

### Comparing `decat-1.0.2/LICENSE` & `decat-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decat-1.0.2/PKG-INFO` & `decat-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: decat
-Version: 1.0.2
+Version: 1.0.3
 Summary: De-concatenate strings that do not have white-spaces.
 Home-page: https://github.com/sudoMode/Decat
 Author: Mandeep Singh
 Author-email: singh.mandeep22207@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/sudoMode/Decat
 Project-URL: Bug Tracker, https://github.com/sudoMode/Decat/issues
 Keywords: nlp,text mining
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -125,18 +124,11 @@
 >> >> ATitleCaseString --> ['a', 'title', 'case', 'string']
 >>```
 > ❗️ Punctuation marks, numbers and special characters will be stripped from the input and
 > will not be preserved in the output
 >>```python
 >> >>  dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com']
 >>```
->
 
-## Credits
->> [Generic Human](https://stackoverflow.com/users/1515832/generic-human)
-> 
->> [Rachael Tatman](https://www.kaggle.com/rtatman)
 
 ## License
 > ### MIT
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: decat Version: 1.0.2 Summary: De-concatenate
+Metadata-Version: 2.1 Name: decat Version: 1.0.3 Summary: De-concatenate
 strings that do not have white-spaces. Home-page: https://github.com/sudoMode/
 Decat Author: Mandeep Singh Author-email: singh.mandeep22207@gmail.com License:
 MIT Project-URL: Source, https://github.com/sudoMode/Decat Project-URL: Bug
 Tracker, https://github.com/sudoMode/Decat/issues Keywords: nlp,text mining
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: MIT License Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # Decat ```python thisisawesome -->
-['this', 'is', 'awesome'] ``` --- [comment]: <> (badges 1)
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE # Decat ```python thisisawesome --> ['this',
+'is', 'awesome'] ``` --- [comment]: <> (badges 1)
     [https://forthebadge.com/images/badges/made-with-python.svg] [https://
   forthebadge.com/images/badges/60-percent-of-the-time-works-every-time.svg]
        [https://forthebadge.com/images/badges/open-source.svg] [https://
               forthebadge.com/images/badges/built-with-love.svg]
 --- [comment]: <> (badges 2)
         [https://img.shields.io/codefactor/grade/github/sudomode/decat/
 master?style=for-the-badge] [https://img.shields.io/github/v/release/sudomode/
@@ -43,11 +43,9 @@
 > >> ð An ever-expanding vocabulary, knows more than 300K English words > >>
 ðª Simplistic design, allows for easy expansion to new languages and custom
 vocabulary sets ## Dependencies > â­ï¸ ___None___ ð ## Limitations > â
 Requires Python >= 3.6 > > â ï¸All input will be treated as lower-case
 >>```python >> >> ATitleCaseString --> ['a', 'title', 'case', 'string'] >>``` >
 âï¸ Punctuation marks, numbers and special characters will be stripped from
 the input and > will not be preserved in the output >>```python >> >>
-dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com'] >>``` > ##
-Credits >> [Generic Human](https://stackoverflow.com/users/1515832/generic-
-human) > >> [Rachael Tatman](https://www.kaggle.com/rtatman) ## License > ###
-MIT
+dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com'] >>``` ##
+License > ### MIT
```

### Comparing `decat-1.0.2/README.md` & `decat-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -101,16 +101,11 @@
 >> >> ATitleCaseString --> ['a', 'title', 'case', 'string']
 >>```
 > ❗️ Punctuation marks, numbers and special characters will be stripped from the input and
 > will not be preserved in the output
 >>```python
 >> >>  dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com']
 >>```
->
 
-## Credits
->> [Generic Human](https://stackoverflow.com/users/1515832/generic-human)
-> 
->> [Rachael Tatman](https://www.kaggle.com/rtatman)
 
 ## License
 > ### MIT
```

#### html2text {}

```diff
@@ -32,11 +32,9 @@
 > >> ð An ever-expanding vocabulary, knows more than 300K English words > >>
 ðª Simplistic design, allows for easy expansion to new languages and custom
 vocabulary sets ## Dependencies > â­ï¸ ___None___ ð ## Limitations > â
 Requires Python >= 3.6 > > â ï¸All input will be treated as lower-case
 >>```python >> >> ATitleCaseString --> ['a', 'title', 'case', 'string'] >>``` >
 âï¸ Punctuation marks, numbers and special characters will be stripped from
 the input and > will not be preserved in the output >>```python >> >>
-dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com'] >>``` > ##
-Credits >> [Generic Human](https://stackoverflow.com/users/1515832/generic-
-human) > >> [Rachael Tatman](https://www.kaggle.com/rtatman) ## License > ###
-MIT
+dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com'] >>``` ##
+License > ### MIT
```

### Comparing `decat-1.0.2/setup.cfg` & `decat-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = decat
-version = 1.0.2
+version = 1.0.3
 author = Mandeep Singh
 author_email = singh.mandeep22207@gmail.com
 description = De-concatenate strings that do not have white-spaces.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sudoMode/Decat
 project_urls =
```

### Comparing `decat-1.0.2/src/decat/.data/vocabulary/en/frequency.json` & `decat-1.0.3/src/decat/.data/vocabulary/en/frequency.json`

 * *Files identical despite different names*

### Comparing `decat-1.0.2/src/decat/.data/vocabulary/en/tokens.json` & `decat-1.0.3/src/decat/.data/vocabulary/en/tokens.json`

 * *Files identical despite different names*

### Comparing `decat-1.0.2/src/decat/__init__.py` & `decat-1.0.3/src/decat/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 #!/usr/local/bin/python3.9
 # -*- coding: utf-8 -*-
 
-from sys import version_info as version
 
 from decat import __settings__ as settings
 from decat.core import Decat
 from decat.parsers import parse_user_args
 
-# check version compatibility
-major, minor, micro = version.major, version.minor, version.micro
-required = 3.6
-if float(f'{major}.{minor}') < required:
-    print(f'Required Python >= {required}, detected: {major}.{minor}.{micro}')
-    exit(0)
 
 # init client
 client = Decat(supported_languages=settings.SUPPORTED_LANGUAGES,
                vocabulary_map=settings.VOCABULARY_MAP)
 
 
 # decat user input
@@ -33,17 +26,17 @@
         print(f'Decat {settings.VERSION}')
     if args.input:
         print(decat(args.input,
                     preserve_special_characters=args.preserve_special_chars))
 
 
 __all__ = [
-            'main',
-            'decat',
-          ]
+    'main',
+    'decat',
+]
 
 
 def test():
     target = 'dummy.email@gmail.com'
     print('Standard conversion...')
     print(f'Target: {target} | Results: {decat(target)}')
     print('\nPreserving special characters...')
```

### Comparing `decat-1.0.2/src/decat/__settings__.py` & `decat-1.0.3/src/decat/__settings__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from os.path import join
 from pathlib import Path
 
 # version
 __major__ = 1
 __minor__ = 0
-__micro__ = 1
+__micro__ = 3
 
 
 VERSION = f'{__major__}.{__minor__}.{__micro__}'
 BASE = Path(__file__).parent.resolve()
 DATA = join(BASE, '.data')
 VOCABULARY = join(DATA, 'vocabulary')
 SUPPORTED_LANGUAGES = dict(english='en')
```

### Comparing `decat-1.0.2/src/decat/core/model.py` & `decat-1.0.3/src/decat/core/model.py`

 * *Files identical despite different names*

### Comparing `decat-1.0.2/src/decat/parsers/input_parser/_parser.py` & `decat-1.0.3/src/decat/parsers/input_parser/_parser.py`

 * *Files identical despite different names*

### Comparing `decat-1.0.2/src/decat.egg-info/PKG-INFO` & `decat-1.0.3/src/decat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: decat
-Version: 1.0.2
+Version: 1.0.3
 Summary: De-concatenate strings that do not have white-spaces.
 Home-page: https://github.com/sudoMode/Decat
 Author: Mandeep Singh
 Author-email: singh.mandeep22207@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/sudoMode/Decat
 Project-URL: Bug Tracker, https://github.com/sudoMode/Decat/issues
 Keywords: nlp,text mining
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -125,18 +124,11 @@
 >> >> ATitleCaseString --> ['a', 'title', 'case', 'string']
 >>```
 > ❗️ Punctuation marks, numbers and special characters will be stripped from the input and
 > will not be preserved in the output
 >>```python
 >> >>  dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com']
 >>```
->
 
-## Credits
->> [Generic Human](https://stackoverflow.com/users/1515832/generic-human)
-> 
->> [Rachael Tatman](https://www.kaggle.com/rtatman)
 
 ## License
 > ### MIT
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: decat Version: 1.0.2 Summary: De-concatenate
+Metadata-Version: 2.1 Name: decat Version: 1.0.3 Summary: De-concatenate
 strings that do not have white-spaces. Home-page: https://github.com/sudoMode/
 Decat Author: Mandeep Singh Author-email: singh.mandeep22207@gmail.com License:
 MIT Project-URL: Source, https://github.com/sudoMode/Decat Project-URL: Bug
 Tracker, https://github.com/sudoMode/Decat/issues Keywords: nlp,text mining
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: MIT License Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # Decat ```python thisisawesome -->
-['this', 'is', 'awesome'] ``` --- [comment]: <> (badges 1)
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE # Decat ```python thisisawesome --> ['this',
+'is', 'awesome'] ``` --- [comment]: <> (badges 1)
     [https://forthebadge.com/images/badges/made-with-python.svg] [https://
   forthebadge.com/images/badges/60-percent-of-the-time-works-every-time.svg]
        [https://forthebadge.com/images/badges/open-source.svg] [https://
               forthebadge.com/images/badges/built-with-love.svg]
 --- [comment]: <> (badges 2)
         [https://img.shields.io/codefactor/grade/github/sudomode/decat/
 master?style=for-the-badge] [https://img.shields.io/github/v/release/sudomode/
@@ -43,11 +43,9 @@
 > >> ð An ever-expanding vocabulary, knows more than 300K English words > >>
 ðª Simplistic design, allows for easy expansion to new languages and custom
 vocabulary sets ## Dependencies > â­ï¸ ___None___ ð ## Limitations > â
 Requires Python >= 3.6 > > â ï¸All input will be treated as lower-case
 >>```python >> >> ATitleCaseString --> ['a', 'title', 'case', 'string'] >>``` >
 âï¸ Punctuation marks, numbers and special characters will be stripped from
 the input and > will not be preserved in the output >>```python >> >>
-dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com'] >>``` > ##
-Credits >> [Generic Human](https://stackoverflow.com/users/1515832/generic-
-human) > >> [Rachael Tatman](https://www.kaggle.com/rtatman) ## License > ###
-MIT
+dummy.email1234@gmail.com --> ['dummy', 'email', 'gmail', 'com'] >>``` ##
+License > ### MIT
```

### Comparing `decat-1.0.2/src/decat.egg-info/SOURCES.txt` & `decat-1.0.3/src/decat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

