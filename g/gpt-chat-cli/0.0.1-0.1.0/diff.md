# Comparing `tmp/gpt-chat-cli-0.0.1.tar.gz` & `tmp/gpt-chat-cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-chat-cli-0.0.1.tar", last modified: Fri May  5 04:39:15 2023, max compression
+gzip compressed data, was "gpt-chat-cli-0.1.0.tar", last modified: Sat May  6 21:46:14 2023, max compression
```

## Comparing `gpt-chat-cli-0.0.1.tar` & `gpt-chat-cli-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 04:39:15.723428 gpt-chat-cli-0.0.1/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1052 2023-05-04 23:39:54.000000 gpt-chat-cli-0.0.1/LICENSE
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     7594 2023-05-05 04:39:15.723428 gpt-chat-cli-0.0.1/PKG-INFO
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     7065 2023-05-05 01:35:45.000000 gpt-chat-cli-0.0.1/README.md
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      587 2023-05-05 00:45:49.000000 gpt-chat-cli-0.0.1/pyproject.toml
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       38 2023-05-05 04:39:15.723428 gpt-chat-cli-0.0.1/setup.cfg
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      412 2023-05-05 00:45:50.000000 gpt-chat-cli-0.0.1/setup.py
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 04:39:15.720095 gpt-chat-cli-0.0.1/src/
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 04:39:15.723428 gpt-chat-cli-0.0.1/src/gpt_chat_cli/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 00:00:46.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli/__init__.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     6013 2023-05-05 01:50:16.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli/argparsing.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1979 2023-05-04 23:37:30.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli/color.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     4242 2023-05-05 01:07:49.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli/gcli.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1732 2023-05-04 23:37:39.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli/openai_wrappers.py
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 04:39:15.723428 gpt-chat-cli-0.0.1/src/gpt_chat_cli.egg-info/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     7594 2023-05-05 04:39:15.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli.egg-info/PKG-INFO
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      430 2023-05-05 04:39:15.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        1 2023-05-05 04:39:15.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       56 2023-05-05 04:39:15.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli.egg-info/entry_points.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       26 2023-05-05 04:39:15.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli.egg-info/requires.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       13 2023-05-05 04:39:15.000000 gpt-chat-cli-0.0.1/src/gpt_chat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1052 2023-05-04 23:39:54.000000 gpt-chat-cli-0.1.0/LICENSE
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10547 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/PKG-INFO
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10018 2023-05-06 21:42:48.000000 gpt-chat-cli-0.1.0/README.md
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      587 2023-05-06 10:51:01.000000 gpt-chat-cli-0.1.0/pyproject.toml
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       38 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/setup.cfg
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      441 2023-05-06 10:51:17.000000 gpt-chat-cli-0.1.0/setup.py
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.231331 gpt-chat-cli-0.1.0/src/
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.231331 gpt-chat-cli-0.1.0/src/gpt_chat_cli/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 05:27:20.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/__init__.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10360 2023-05-06 20:06:24.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/argparsing.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5690 2023-05-06 10:40:40.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/chat_colorizer.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1979 2023-05-06 19:56:25.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/color.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     8587 2023-05-06 19:57:38.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/gcli.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     2873 2023-05-06 21:24:43.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/openai_wrappers.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     9556 2023-05-06 10:41:58.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/streaming_lexer.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       18 2023-05-06 10:50:51.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/version.py
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10547 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      559 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        1 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       56 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       43 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/requires.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       13 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/tests/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5409 2023-05-06 07:11:24.000000 gpt-chat-cli-0.1.0/tests/test_streaming_lexer.py
```

### Comparing `gpt-chat-cli-0.0.1/LICENSE` & `gpt-chat-cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.0.1/pyproject.toml` & `gpt-chat-cli-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpt-chat-cli"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Flu0r1ne", email="flu0r1ne@flu0r1ne.net" },
 ]
 description = "A simple ChatGPT terminal CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gpt-chat-cli-0.0.1/src/gpt_chat_cli/color.py` & `gpt-chat-cli-0.1.0/src/gpt_chat_cli/color.py`

 * *Files identical despite different names*

