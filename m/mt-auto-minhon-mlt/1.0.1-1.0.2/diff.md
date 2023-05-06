# Comparing `tmp/mt-auto-minhon-mlt-1.0.1.tar.gz` & `tmp/mt-auto-minhon-mlt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mt-auto-minhon-mlt-1.0.1.tar", last modified: Tue Apr 25 14:53:09 2023, max compression
+gzip compressed data, was "mt-auto-minhon-mlt-1.0.2.tar", last modified: Sat May  6 03:30:19 2023, max compression
```

## Comparing `mt-auto-minhon-mlt-1.0.1.tar` & `mt-auto-minhon-mlt-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:09.454667 mt-auto-minhon-mlt-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-25 14:53:09.454667 mt-auto-minhon-mlt-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-25 14:52:58.000000 mt-auto-minhon-mlt-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 14:52:58.000000 mt-auto-minhon-mlt-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:53:09.454667 mt-auto-minhon-mlt-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:09.454667 mt-auto-minhon-mlt-1.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:52:58.000000 mt-auto-minhon-mlt-1.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:09.454667 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 14:52:58.000000 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:09.454667 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    53482 2023-04-25 14:52:58.000000 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt/assets/support_translate.json
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-25 14:52:58.000000 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt/tranlator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:09.454667 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-25 14:53:09.000000 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 14:53:09.000000 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:53:09.000000 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 14:53:09.000000 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 14:53:09.000000 mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:09.454667 mt-auto-minhon-mlt-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 14:52:58.000000 mt-auto-minhon-mlt-1.0.1/tests/test_tranlator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    53482 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/assets/support_translate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/tranlator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/tests/test_tranlator.py
```

### Comparing `mt-auto-minhon-mlt-1.0.1/PKG-INFO` & `mt-auto-minhon-mlt-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: mt-auto-minhon-mlt
-Version: 1.0.1
+Version: 1.0.2
 Summary: みんなの自動翻訳 Python Library
 Project-URL: Homepage, https://github.com/MIDORIBIN/mt-auto-minhon-mlt
 Project-URL: Bug Tracker, https://github.com/MIDORIBIN/mt-auto-minhon-mlt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
+![](docs/assets/header.png)
+
 # みんなの自動翻訳 Python Library
 
 [![Python application](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml/badge.svg)](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml)
+[![PyPI version](https://badge.fury.io/py/mt-auto-minhon-mlt.svg)](https://badge.fury.io/py/mt-auto-minhon-mlt)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mt-auto-minhon-mlt)](https://pypi.org/project/mt-auto-minhon-mlt/)
+
+「みんなの自動翻訳」をPythonから利用するためのライブラリです。  
+「みんなの自動翻訳」は日本語から英語、英語から日本語、そして多数の他の言語の間で自動翻訳を提供しています。  
+Pythonラッパーを使用することで、これらの翻訳機能をPythonプログラムから簡単に利用することができます。
 
 ## インストール
 
 ```shell
-pip install git+https://github.com/MIDORIBIN/mt-auto-minhon-mlt.git
+pip install mt-auto-minhon-mlt
 ```
 
 ## 必要条件
 
-本ライブラリは、Python バージョン 3.9.7 でテストされています。
+本ライブラリは、Python 3.7, 3.8, 3.9, 3.10でテストされています。
 
 ## 使用法
 
 1. [みんなの自動翻訳の設定画面](https://mt-auto-minhon-mlt.ucri.jgn-x.jp/content/setting/user/edit/)から `ユーザーID` 、 `API key` 、 `API secret` を取得
 2. `Translator` クラスのインスタンスを生成
 3. `Translator.translate_text` に翻訳対象の文章、翻訳前の言語、翻訳後の言語を指定
 
@@ -46,14 +54,17 @@
 en_actual = translator.translate_text('みんなの自動翻訳', source_lang='ja', target_lang='en')
 ```
 
 ## TODO
 
 - [x] ~~CI~~
 - [x] ~~linter, formatter~~
-- [ ] PyPI
+- [x] ~~PyPI~~
+- [x] ~~PyPI GitHub Actions~~
+- [x] ~~support other parameter~~
+- [x] ~~badge~~
+- [x] ~~docs~~
+- [x] ~~docs header~~
+- [ ] support file
 - [ ] CD
-- [ ] badge
 - [ ] CLI
-- [ ] docs
-- [ ] docs header
-- [ ] PyPI GitHub Actions
+
```

### Comparing `mt-auto-minhon-mlt-1.0.1/README.md` & `mt-auto-minhon-mlt-1.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+![](docs/assets/header.png)
+
 # みんなの自動翻訳 Python Library
 
 [![Python application](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml/badge.svg)](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml)
+[![PyPI version](https://badge.fury.io/py/mt-auto-minhon-mlt.svg)](https://badge.fury.io/py/mt-auto-minhon-mlt)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mt-auto-minhon-mlt)](https://pypi.org/project/mt-auto-minhon-mlt/)
+
+「みんなの自動翻訳」をPythonから利用するためのライブラリです。  
+「みんなの自動翻訳」は日本語から英語、英語から日本語、そして多数の他の言語の間で自動翻訳を提供しています。  
+Pythonラッパーを使用することで、これらの翻訳機能をPythonプログラムから簡単に利用することができます。
 
 ## インストール
 
 ```shell
-pip install git+https://github.com/MIDORIBIN/mt-auto-minhon-mlt.git
+pip install mt-auto-minhon-mlt
 ```
 
 ## 必要条件
 
-本ライブラリは、Python バージョン 3.9.7 でテストされています。
+本ライブラリは、Python 3.7, 3.8, 3.9, 3.10でテストされています。
 
 ## 使用法
 
 1. [みんなの自動翻訳の設定画面](https://mt-auto-minhon-mlt.ucri.jgn-x.jp/content/setting/user/edit/)から `ユーザーID` 、 `API key` 、 `API secret` を取得
 2. `Translator` クラスのインスタンスを生成
 3. `Translator.translate_text` に翻訳対象の文章、翻訳前の言語、翻訳後の言語を指定
 
@@ -31,14 +39,17 @@
 en_actual = translator.translate_text('みんなの自動翻訳', source_lang='ja', target_lang='en')
 ```
 
 ## TODO
 
 - [x] ~~CI~~
 - [x] ~~linter, formatter~~
-- [ ] PyPI
+- [x] ~~PyPI~~
+- [x] ~~PyPI GitHub Actions~~
+- [x] ~~support other parameter~~
+- [x] ~~badge~~
+- [x] ~~docs~~
+- [x] ~~docs header~~
+- [ ] support file
 - [ ] CD
-- [ ] badge
 - [ ] CLI
-- [ ] docs
-- [ ] docs header
-- [ ] PyPI GitHub Actions
+
```

### Comparing `mt-auto-minhon-mlt-1.0.1/pyproject.toml` & `mt-auto-minhon-mlt-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mt-auto-minhon-mlt"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.md"
 description = "みんなの自動翻訳 Python Library"
 requires-python = ">=3.7, <3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt/assets/support_translate.json` & `mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/assets/support_translate.json`

 * *Files identical despite different names*

### Comparing `mt-auto-minhon-mlt-1.0.1/src/mt_auto_minhon_mlt.egg-info/PKG-INFO` & `mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: mt-auto-minhon-mlt
-Version: 1.0.1
+Version: 1.0.2
 Summary: みんなの自動翻訳 Python Library
 Project-URL: Homepage, https://github.com/MIDORIBIN/mt-auto-minhon-mlt
 Project-URL: Bug Tracker, https://github.com/MIDORIBIN/mt-auto-minhon-mlt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
+![](docs/assets/header.png)
+
 # みんなの自動翻訳 Python Library
 
 [![Python application](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml/badge.svg)](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml)
+[![PyPI version](https://badge.fury.io/py/mt-auto-minhon-mlt.svg)](https://badge.fury.io/py/mt-auto-minhon-mlt)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mt-auto-minhon-mlt)](https://pypi.org/project/mt-auto-minhon-mlt/)
+
+「みんなの自動翻訳」をPythonから利用するためのライブラリです。  
+「みんなの自動翻訳」は日本語から英語、英語から日本語、そして多数の他の言語の間で自動翻訳を提供しています。  
+Pythonラッパーを使用することで、これらの翻訳機能をPythonプログラムから簡単に利用することができます。
 
 ## インストール
 
 ```shell
-pip install git+https://github.com/MIDORIBIN/mt-auto-minhon-mlt.git
+pip install mt-auto-minhon-mlt
 ```
 
 ## 必要条件
 
-本ライブラリは、Python バージョン 3.9.7 でテストされています。
+本ライブラリは、Python 3.7, 3.8, 3.9, 3.10でテストされています。
 
 ## 使用法
 
 1. [みんなの自動翻訳の設定画面](https://mt-auto-minhon-mlt.ucri.jgn-x.jp/content/setting/user/edit/)から `ユーザーID` 、 `API key` 、 `API secret` を取得
 2. `Translator` クラスのインスタンスを生成
 3. `Translator.translate_text` に翻訳対象の文章、翻訳前の言語、翻訳後の言語を指定
 
@@ -46,14 +54,17 @@
 en_actual = translator.translate_text('みんなの自動翻訳', source_lang='ja', target_lang='en')
 ```
 
 ## TODO
 
 - [x] ~~CI~~
 - [x] ~~linter, formatter~~
-- [ ] PyPI
+- [x] ~~PyPI~~
+- [x] ~~PyPI GitHub Actions~~
+- [x] ~~support other parameter~~
+- [x] ~~badge~~
+- [x] ~~docs~~
+- [x] ~~docs header~~
+- [ ] support file
 - [ ] CD
-- [ ] badge
 - [ ] CLI
-- [ ] docs
-- [ ] docs header
-- [ ] PyPI GitHub Actions
+
```

### Comparing `mt-auto-minhon-mlt-1.0.1/tests/test_tranlator.py` & `mt-auto-minhon-mlt-1.0.2/tests/test_tranlator.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,7 +26,19 @@
 
         jp_text = "みんなの自動翻訳"
         en_expected = "Minna no Jido Hon'"
         en_actual = self.translator.translate_text(
             jp_text, translate_type="voicetraNT", source_lang="ja", target_lang="en"
         )
         self.assertEqual(en_expected, en_actual)
+
+    def test_translate_text_error(self):
+        translator = Translator(
+            client_id=os.environ["CLIENT_ID"],
+            client_secret=os.environ["CLIENT_SECRET"],
+            user_name="invalid user name",
+        )
+        jp_text = "みんなの自動翻訳"
+
+        with self.assertRaises(ValueError) as cm:
+            translator.translate_text(jp_text, source_lang="ja", target_lang="en")
+        self.assertEqual('code: 501, message: ""', str(cm.exception))
```

