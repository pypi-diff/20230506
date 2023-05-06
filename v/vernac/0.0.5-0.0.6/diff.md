# Comparing `tmp/vernac-0.0.5.tar.gz` & `tmp/vernac-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernac-0.0.5.tar", last modified: Tue May  2 00:40:49 2023, max compression
+gzip compressed data, was "vernac-0.0.6.tar", last modified: Sat May  6 17:38:17 2023, max compression
```

## Comparing `vernac-0.0.5.tar` & `vernac-0.0.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.553106 vernac-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.533105 vernac-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.541105 vernac-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 00:40:37.000000 vernac-0.0.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 00:40:37.000000 vernac-0.0.5/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 00:40:37.000000 vernac-0.0.5/.github/workflows/test-some-examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-02 00:40:37.000000 vernac-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 00:40:37.000000 vernac-0.0.5/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 00:40:37.000000 vernac-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-02 00:40:49.553106 vernac-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-02 00:40:37.000000 vernac-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-02 00:40:37.000000 vernac-0.0.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.533105 vernac-0.0.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.541105 vernac-0.0.5/examples/reliable/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/benchmark.vn
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/emoji.vn
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/fizzbuzz-with-test-buggy.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/fizzbuzz-with-test.vn
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/fizzbuzz.vn
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/hngpt-with-test.vn
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/hngpt.vn
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/mergesort.vn
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/todo-cli.vn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.545106 vernac-0.0.5/examples/reliable/todo-tui/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/todo-tui/todo-storage.vn
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/todo-tui/todo-tui.vn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.545106 vernac-0.0.5/examples/unreliable/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/unreliable/count_gpt_titles.vn
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/unreliable/hntoday.vn
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/unreliable/snake.vn
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 00:40:37.000000 vernac-0.0.5/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-02 00:40:37.000000 vernac-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:40:49.553106 vernac-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.537105 vernac-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.545106 vernac-0.0.5/src/vernac/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.553106 vernac-0.0.5/src/vernac/stages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/check_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/check_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/document_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/generate_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/guess_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/map_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/read_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/run_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.553106 vernac-0.0.5/src/vernac/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.549106 vernac-0.0.5/src/vernac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.835316 vernac-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.827315 vernac-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.827315 vernac-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-06 17:38:04.000000 vernac-0.0.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-06 17:38:04.000000 vernac-0.0.6/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-06 17:38:04.000000 vernac-0.0.6/.github/workflows/test-some-examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-06 17:38:04.000000 vernac-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 17:38:04.000000 vernac-0.0.6/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 17:38:04.000000 vernac-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-06 17:38:17.835316 vernac-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-06 17:38:04.000000 vernac-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-06 17:38:04.000000 vernac-0.0.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.827315 vernac-0.0.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.831316 vernac-0.0.6/examples/reliable/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/benchmark.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/emoji.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/fizzbuzz-with-test-buggy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/fizzbuzz-with-test.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/fizzbuzz.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/hngpt-with-test.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/hngpt.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/mergesort.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/todo-cli.vn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.831316 vernac-0.0.6/examples/reliable/todo-tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/todo-tui/todo-storage.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/reliable/todo-tui/todo-tui.vn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.831316 vernac-0.0.6/examples/unreliable/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/unreliable/count_gpt_titles.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/unreliable/hntoday.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-06 17:38:04.000000 vernac-0.0.6/examples/unreliable/snake.vn
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-06 17:38:04.000000 vernac-0.0.6/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-06 17:38:04.000000 vernac-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 17:38:17.835316 vernac-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.827315 vernac-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.831316 vernac-0.0.6/src/vernac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.835316 vernac-0.0.6/src/vernac/stages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/check_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/check_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/document_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/generate_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/guess_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/map_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/read_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/stages/run_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.835316 vernac-0.0.6/src/vernac/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-06 17:38:04.000000 vernac-0.0.6/src/vernac/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:38:17.831316 vernac-0.0.6/src/vernac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-06 17:38:17.000000 vernac-0.0.6/src/vernac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-06 17:38:17.000000 vernac-0.0.6/src/vernac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 17:38:17.000000 vernac-0.0.6/src/vernac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-06 17:38:17.000000 vernac-0.0.6/src/vernac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-06 17:38:17.000000 vernac-0.0.6/src/vernac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 17:38:17.000000 vernac-0.0.6/src/vernac.egg-info/top_level.txt
```

### Comparing `vernac-0.0.5/.github/workflows/publish-to-pypi.yml` & `vernac-0.0.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/.github/workflows/test-some-examples.yml` & `vernac-0.0.6/.github/workflows/test-some-examples.yml`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/.gitignore` & `vernac-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/LICENSE` & `vernac-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/PKG-INFO` & `vernac-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vernac
-Version: 0.0.5
+Version: 0.0.6
 Summary: Write programs in English
 Project-URL: Homepage, https://github.com/bsilverthorn/vernac
 Project-URL: Repository, https://github.com/bsilverthorn/vernac
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -47,14 +47,19 @@
 The dream is that you check the _English_ into git, not the code.
 
 Every modern programmer already uses ChatGPT to generate code, then copies the code into their own source file. That’s a bit like writing your application in assembly and occasionally pasting in output from your compiler. Stay in the highest-level language you have for as long as you can! Today, in the GPT era, our highest-level language is English.
 
 Usage
 -----
 
+### Prerequisites
+
+- Python 3.10+
+- OpenAI API key with GPT-4
+
 ### Install
 
 - `pip install vernac` or (recommended →) `pipx install vernac`
 
 ### Run
 
 - `export OPENAI_API_KEY=<key>`
```

### Comparing `vernac-0.0.5/README.md` & `vernac-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 The dream is that you check the _English_ into git, not the code.
 
 Every modern programmer already uses ChatGPT to generate code, then copies the code into their own source file. That’s a bit like writing your application in assembly and occasionally pasting in output from your compiler. Stay in the highest-level language you have for as long as you can! Today, in the GPT era, our highest-level language is English.
 
 Usage
 -----
 
+### Prerequisites
+
+- Python 3.10+
+- OpenAI API key with GPT-4
+
 ### Install
 
 - `pip install vernac` or (recommended →) `pipx install vernac`
 
 ### Run
 
 - `export OPENAI_API_KEY=<key>`
```

### Comparing `vernac-0.0.5/dev-requirements.txt` & `vernac-0.0.6/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/examples/reliable/todo-tui/todo-tui.vn` & `vernac-0.0.6/examples/reliable/todo-tui/todo-tui.vn`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/examples/unreliable/hntoday.vn` & `vernac-0.0.6/examples/unreliable/hntoday.vn`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/pyproject.toml` & `vernac-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/compile.py` & `vernac-0.0.6/src/vernac/compile.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,21 +48,26 @@
     parser.add_argument(
         "-v",
         dest="verbose",
         action="store_true",
     )
     parser.add_argument(
         "--inject",
-        metavar="VN PY",
+        metavar="PATH",
         dest="injects_list",
         nargs=2,
         action="append",
         default=[],
+        help="use given source instead of generating (first pass only)"
+    )
+    parser.add_argument(
+        "--package-dir",
+        metavar="PATH",
+        help="write package source here instead of temp dir",
     )
-    parser.add_argument("--package-dir", metavar="PATH")
 
     args = parser.parse_args()
 
     return args
 
 def script_main():
     main_kwargs = vars(parse_args())
```

### Comparing `vernac-0.0.5/src/vernac/openai.py` & `vernac-0.0.6/src/vernac/openai.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/pipeline.py` & `vernac-0.0.6/src/vernac/pipeline.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/stages/check_help.py` & `vernac-0.0.6/src/vernac/stages/check_help.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/stages/check_tests.py` & `vernac-0.0.6/src/vernac/stages/check_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     StageOutput,
 )
 from vernac.stages.generate_code import TestFailure
 
 def extract_suggested_tests(context: StageContext, english: str) -> list[dict]:
     # prepare prompt
     system_prompt = """
-You are an expert programmer working on contract. The user, your client, will provide a description of program functionality. You will provide details of how to execute any tests listed in the spec.
+You are an expert programmer working on contract. The user, your client, will provide a description of program functionality. You will provide details of how to execute any tests listed in the spec. Relevant documentation might also be provided, but should be ignored. Only look at tests included with the program spec, not in any documentation.
 
 For each test listed in the spec, extract the arguments to run along with any description of correct output. List that information a single line of JSON in the following format:
 
 {"args": "--foo -x=bar", "description": "should print 10 lines"}
 
 Do not list the name of the program itself, only the arguments. If no tests are listed, write nothing.
 """
```

### Comparing `vernac-0.0.5/src/vernac/stages/document_module.py` & `vernac-0.0.6/src/vernac/stages/document_module.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/stages/generate_code.py` & `vernac-0.0.6/src/vernac/stages/generate_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     expected: str
     actual: str
 
 def get_main_prompts(english: str) -> tuple[str, str]:
     system_prompt = (
         "You are an expert programmer working on contract. "
         "The user, your client, will provide a description of program functionality. "
-        "Respond with Python 3 source code implementing that description. " 
+        "Respond with Python 3 source code implementing that description.\n\n" 
+        "Write one comment listing any dependencies to be `pip install`ed: `# DEPENDENCIES: ...`.\n\n"
         "Respond only with the source code inside a Markdown code block. "
         "Do not add commentary."
     )
     user_prompt = (
         "Please write the following program in Python 3. "
         "Include a `main` function that takes no arguments and returns nothing. "
         "Use `argparse` to parse command line arguments."
@@ -36,15 +37,16 @@
 
     return (system_prompt, user_prompt)
 
 def get_module_prompts(english: str) -> tuple[str, str]:
     system_prompt = (
         "You are an expert programmer working on contract. "
         "The user, your client, will provide a description of one specific module. "
-        "Respond with Python 3 source code implementing that module. "
+        "Respond with Python 3 source code implementing that module.\n\n"
+        "Write one comment listing any dependencies to be `pip install`ed: `# DEPENDENCIES: ...`.\n\n"
         "Respond only with the source code inside a Markdown code block. "
         "Do not add commentary."
     )
     user_prompt = english
 
     return (system_prompt, user_prompt)
```

### Comparing `vernac-0.0.5/src/vernac/stages/guess_dependencies.py` & `vernac-0.0.6/src/vernac/stages/guess_dependencies.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/stages/interface.py` & `vernac-0.0.6/src/vernac/stages/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self._progress.update(self._progress_task, completed=completed)
 
 class StageAction(Enum):
     NEXT = auto()
     LOOP = auto()
 
     @classmethod
-    def out(cls, **state: dict) -> "StageOutput":
+    def out(cls, **state: Any) -> "StageOutput":
         return StageOutput(
             action=cls.NEXT,
             state=state,
         )
 
 @dataclass
 class StageOutput:
```

### Comparing `vernac-0.0.5/src/vernac/stages/map_modules.py` & `vernac-0.0.6/src/vernac/stages/map_modules.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     MAIN = auto()
     MODULE = auto()
 
 def classify_source_type(
         context: StageContext,
         filename: str,
         english: str,
-    ) -> str | None:
+    ) -> SourceType:
     # prepare prompt
     system_prompt = """
 You are an expert programmer working on contract. The user, your client, has created specs for various modules. You need to start by identifying which spec describes the main module for the program.
 
 The user will provide the spec. Please respond with MAIN if the spec appears to describe the main module. Otherwise respond with MODULE.
 
 Only write MAIN or MODULE. Do not write any other text.
@@ -61,18 +61,22 @@
 class MapModulesStage(VernacStage):
     steps = 1
 
     def __init__(self, title: str):
         self.title = title
 
     def run(self, context: StageContext, english_all: dict[str, str]) -> StageOutput:
-        english_types = {
-            fn: classify_source_type(context, fn, e)
-            for fn, e in english_all.items()
-        }
+        if len(english_all) == 1:
+            english_types = {fn: SourceType.MAIN for fn in english_all}
+        else:
+            english_types = {
+                fn: classify_source_type(context, fn, e)
+                for fn, e in english_all.items()
+            }
+
         (main,) = [fn for fn, t in english_types.items() if t == SourceType.MAIN]
         modules = [fn for fn, t in english_types.items() if t == SourceType.MODULE]
 
         return StageAction.NEXT.out(
             main_name=main,
             module_names=modules,
         )
```

### Comparing `vernac-0.0.5/src/vernac/stages/package.py` & `vernac-0.0.6/src/vernac/stages/package.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/stages/read_source.py` & `vernac-0.0.6/src/vernac/stages/read_source.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/stages/run_pipelines.py` & `vernac-0.0.6/src/vernac/stages/run_pipelines.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/test/test_util.py` & `vernac-0.0.6/src/vernac/test/test_util.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac/util.py` & `vernac-0.0.6/src/vernac/util.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.5/src/vernac.egg-info/PKG-INFO` & `vernac-0.0.6/src/vernac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vernac
-Version: 0.0.5
+Version: 0.0.6
 Summary: Write programs in English
 Project-URL: Homepage, https://github.com/bsilverthorn/vernac
 Project-URL: Repository, https://github.com/bsilverthorn/vernac
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -47,14 +47,19 @@
 The dream is that you check the _English_ into git, not the code.
 
 Every modern programmer already uses ChatGPT to generate code, then copies the code into their own source file. That’s a bit like writing your application in assembly and occasionally pasting in output from your compiler. Stay in the highest-level language you have for as long as you can! Today, in the GPT era, our highest-level language is English.
 
 Usage
 -----
 
+### Prerequisites
+
+- Python 3.10+
+- OpenAI API key with GPT-4
+
 ### Install
 
 - `pip install vernac` or (recommended →) `pipx install vernac`
 
 ### Run
 
 - `export OPENAI_API_KEY=<key>`
```

### Comparing `vernac-0.0.5/src/vernac.egg-info/SOURCES.txt` & `vernac-0.0.6/src/vernac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

