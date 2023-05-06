# Comparing `tmp/nlpashto-0.0.7.tar.gz` & `tmp/nlpashto-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpashto-0.0.7.tar", last modified: Wed Mar  1 08:13:49 2023, max compression
+gzip compressed data, was "nlpashto-0.0.8.tar", last modified: Wed Mar  1 11:29:51 2023, max compression
```

## Comparing `nlpashto-0.0.7.tar` & `nlpashto-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 08:13:49.940056 nlpashto-0.0.7/
--rw-rw-rw-   0        0        0     1096 2023-02-28 10:10:26.000000 nlpashto-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2005 2023-03-01 08:13:49.939056 nlpashto-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-03-01 07:54:59.000000 nlpashto-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 08:13:49.930069 nlpashto-0.0.7/nlpashto/
--rw-rw-rw-   0        0        0       58 2023-03-01 08:12:57.000000 nlpashto-0.0.7/nlpashto/__init__.py
--rw-rw-rw-   0        0        0      298 2023-03-01 06:05:39.000000 nlpashto-0.0.7/nlpashto/char_replace.py
--rw-rw-rw-   0        0        0      938 2023-03-01 08:12:54.000000 nlpashto-0.0.7/nlpashto/functions.py
--rw-rw-rw-   0        0        0     4450 2023-03-01 08:13:18.000000 nlpashto-0.0.7/nlpashto/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-01 08:13:49.938067 nlpashto-0.0.7/nlpashto.egg-info/
--rw-rw-rw-   0        0        0     2005 2023-03-01 08:13:49.000000 nlpashto-0.0.7/nlpashto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-03-01 08:13:49.000000 nlpashto-0.0.7/nlpashto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 08:13:49.000000 nlpashto-0.0.7/nlpashto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-01 08:13:49.000000 nlpashto-0.0.7/nlpashto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      545 2023-03-01 08:13:34.000000 nlpashto-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-01 08:13:49.940056 nlpashto-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-01 11:29:51.229967 nlpashto-0.0.8/
+-rw-rw-rw-   0        0        0     1096 2023-02-28 10:10:26.000000 nlpashto-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2005 2023-03-01 11:29:51.228966 nlpashto-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-03-01 07:54:59.000000 nlpashto-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-03-01 11:29:51.219052 nlpashto-0.0.8/nlpashto/
+-rw-rw-rw-   0        0        0       89 2023-03-01 11:28:52.000000 nlpashto-0.0.8/nlpashto/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-03-01 11:18:38.000000 nlpashto-0.0.8/nlpashto/char_replace.py
+-rw-rw-rw-   0        0        0     1608 2023-03-01 11:28:37.000000 nlpashto-0.0.8/nlpashto/functions.py
+-rw-rw-rw-   0        0        0     4881 2023-03-01 11:28:44.000000 nlpashto-0.0.8/nlpashto/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-01 11:29:51.227966 nlpashto-0.0.8/nlpashto.egg-info/
+-rw-rw-rw-   0        0        0     2005 2023-03-01 11:29:51.000000 nlpashto-0.0.8/nlpashto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-03-01 11:29:51.000000 nlpashto-0.0.8/nlpashto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-01 11:29:51.000000 nlpashto-0.0.8/nlpashto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-03-01 11:29:51.000000 nlpashto-0.0.8/nlpashto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      545 2023-03-01 11:29:20.000000 nlpashto-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-01 11:29:51.229967 nlpashto-0.0.8/setup.cfg
```

### Comparing `nlpashto-0.0.7/LICENSE` & `nlpashto-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpashto-0.0.7/PKG-INFO` & `nlpashto-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpashto
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pashto Natural Language Processing Toolkit
 Author-email: Ijazul Haq <ijazse@hotmail.com>
 Project-URL: Homepage, https://github.com/ijazul-haq/nlpashto
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `nlpashto-0.0.7/README.md` & `nlpashto-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nlpashto-0.0.7/nlpashto/functions.py` & `nlpashto-0.0.8/nlpashto/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,46 @@
-from nlpashto.utils import features_segmenter, features_pos, preprocess
+from nlpashto.utils import features_segmenter, features_pos, basic_preprocessing, preprocess, features_tokenizer
 import pickle, os
 
+def tokenizer(text):
+    text = preprocess(text)
+    text = text.replace(' ', '')
+    X_test = [features_tokenizer(text, index) for index in range(len(text))]
+    path_ = os.path.join(os.path.dirname(__file__), "tokenizer.sav")
+    model = pickle.load(open(path_, 'rb'))
+    y_pred = model.predict_single(X_test)
+    text_ = ''
+    for c, t in zip(text, y_pred):
+        text_ = text_ + c + t 
+    text_ = text_.strip(' J').replace('S', ' ')
+    text_ = text_.replace('J', '')
+    return text_
+
 def word_tokenizer(text):
     text = preprocess(text)
     text = text.split()
     X_test = [features_pos(text, index) for index in range(len(text))]
     path_ = os.path.join(os.path.dirname(__file__), "segmenter.sav")
     model = pickle.load(open(path_, 'rb'))
     y_pred = model.predict_single(X_test)
     text_ = ''
     for c, t in zip(text, y_pred):
         text_ = text_ + c + t 
     text_ = text_.strip(' SB')
     text_ = text_.replace('S', ' ').split('B')
     return text_
 
+def sentence_tokenizer(text):
+    text = basic_preprocessing(text)
+    text = text.split('.')
+    return text
+
 def pos_tagger(text):
     X_test = [features_pos(text, index) for index in range(len(text))]
     path_ = os.path.join(os.path.dirname(__file__), "pos_tagger.sav")
     model = pickle.load(open(path_, 'rb'))
     y_pred = model.predict_single(X_test)
     text_ = []
     for c, t in zip(text, y_pred):
         text_.append([c,t])
-    return text_
+    return text_
+
```

### Comparing `nlpashto-0.0.7/nlpashto/utils.py` & `nlpashto-0.0.8/nlpashto/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,37 +73,51 @@
         'next_1_sfx_1': '' if (not next_1 or len(next_1)<3) else next_1[-1],       
         'next_1_sfx_2': '' if (not next_1 or len(next_1)<4) else next_1[-2:],       
         'next_2': next_2,
       }
     return features
 
 
-def preprocess(c):
+def features_tokenizer(sentence, index):
+    char = sentence[index]
+    features = {
+        'c': char,
+        'is_first': index == 0,
+        'is_last': index == len(sentence)-1
+    }
+    for n in range(1,5):
+        features['prev_'+str(n)] = ''.join(sentence[index-n:index+1])
+        features['next_'+str(n)] = ''.join(sentence[index:index+n+1])
+    return features
+
+def basic_preprocessing(c):
     special_char_dict = {}
     for r in char_replace:
         old, new = r[0], r[1]
         special_char_dict[old] = new
     
     alphabits = 'اب پ ت ټ ث ج چ ح خ څ ځ دډذرړزژږس ش ښ ص ض ط ظ ع غ ف ق ک ګ ل م ن ڼ ں وؤ ه ۀ ي ې ی ےۍئء'
-    punc = '٪.،.\n'
+    punc = '٪،.\n'
     digits = '۰۱۲۳۴۵۶۷۸۹'
     uk = 'ـ'
 
     map_table = c.maketrans(special_char_dict)
     c = c.translate(map_table)
     c = c.replace(uk, '')
     
     res = [ele if (ele in alphabits) or (ele in digits) or (ele in punc) else  ' ' for ele in c]
     c = ''.join(res)
-    
     c = re.sub("["+digits+"]+", lambda ele: " " + ele[0] + " ", c)
-
-    c = c.replace('\n', ' ').replace('۔', '.')
+    c = c.replace('\n', ' ')
     c = re.sub('\.+', '.', c)
     c = re.sub('،+', '،', c)
-    c = re.sub('، ،', '،', c)
     c = re.sub('٪+', '٪', c)
-    c = re.sub('٪ ٪', '٪', c)
+    c = c.replace('، ،', '،').replace('٪ ٪', '٪')
+    c = re.sub(' +', ' ', c)
+    c = c.strip(' ،.')
+    return c
+
+def preprocess(c):
+    c = basic_preprocessing(c)
+    c = c.replace('.', ' ')
     c = re.sub(' +', ' ', c)
-    c = c.strip(' ،.').replace('.','\n')
-    c = re.sub('\n+', '\n', c)
     return c
```

### Comparing `nlpashto-0.0.7/nlpashto.egg-info/PKG-INFO` & `nlpashto-0.0.8/nlpashto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpashto
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pashto Natural Language Processing Toolkit
 Author-email: Ijazul Haq <ijazse@hotmail.com>
 Project-URL: Homepage, https://github.com/ijazul-haq/nlpashto
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `nlpashto-0.0.7/pyproject.toml` & `nlpashto-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nlpashto"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Ijazul Haq", email="ijazse@hotmail.com" },
 ]
 description = "Pashto Natural Language Processing Toolkit"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

