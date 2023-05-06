# Comparing `tmp/pandas-chat-0.0.2.tar.gz` & `tmp/pandas-chat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-chat-0.0.2.tar", last modified: Fri May  5 14:25:52 2023, max compression
+gzip compressed data, was "pandas-chat-0.0.3.tar", last modified: Sat May  6 16:55:46 2023, max compression
```

## Comparing `pandas-chat-0.0.2.tar` & `pandas-chat-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 mvm       (1000) mvm       (1000)        0 2023-05-05 14:25:52.568626 pandas-chat-0.0.2/
--rw-r--r--   0 mvm       (1000) mvm       (1000)     1799 2023-03-27 15:45:07.000000 pandas-chat-0.0.2/.gitignore
--rw-r--r--   0 mvm       (1000) mvm       (1000)     1495 2023-03-27 15:45:07.000000 pandas-chat-0.0.2/LICENSE
--rw-r--r--   0 mvm       (1000) mvm       (1000)      920 2023-05-05 14:25:52.568626 pandas-chat-0.0.2/PKG-INFO
--rw-r--r--   0 mvm       (1000) mvm       (1000)      596 2023-05-05 14:16:31.000000 pandas-chat-0.0.2/README.md
--rw-r--r--   0 mvm       (1000) mvm       (1000)      127 2023-05-01 20:01:33.000000 pandas-chat-0.0.2/TODO.md
-drwxr-xr-x   0 mvm       (1000) mvm       (1000)        0 2023-05-05 14:25:52.568626 pandas-chat-0.0.2/pandas_chat/
--rw-r--r--   0 mvm       (1000) mvm       (1000)        0 2023-04-28 14:50:39.000000 pandas-chat-0.0.2/pandas_chat/__init__.py
--rw-r--r--   0 mvm       (1000) mvm       (1000)     1007 2023-05-01 20:03:32.000000 pandas-chat-0.0.2/pandas_chat/action.py
--rw-r--r--   0 mvm       (1000) mvm       (1000)     1308 2023-05-01 17:06:43.000000 pandas-chat-0.0.2/pandas_chat/factory.py
--rw-r--r--   0 mvm       (1000) mvm       (1000)      137 2023-04-28 15:37:37.000000 pandas-chat-0.0.2/pandas_chat/utils.py
-drwxr-xr-x   0 mvm       (1000) mvm       (1000)        0 2023-05-05 14:25:52.568626 pandas-chat-0.0.2/pandas_chat.egg-info/
--rw-r--r--   0 mvm       (1000) mvm       (1000)      920 2023-05-05 14:25:52.000000 pandas-chat-0.0.2/pandas_chat.egg-info/PKG-INFO
--rw-r--r--   0 mvm       (1000) mvm       (1000)      348 2023-05-05 14:25:52.000000 pandas-chat-0.0.2/pandas_chat.egg-info/SOURCES.txt
--rw-r--r--   0 mvm       (1000) mvm       (1000)        1 2023-05-05 14:25:52.000000 pandas-chat-0.0.2/pandas_chat.egg-info/dependency_links.txt
--rw-r--r--   0 mvm       (1000) mvm       (1000)        7 2023-05-05 14:25:52.000000 pandas-chat-0.0.2/pandas_chat.egg-info/requires.txt
--rw-r--r--   0 mvm       (1000) mvm       (1000)       12 2023-05-05 14:25:52.000000 pandas-chat-0.0.2/pandas_chat.egg-info/top_level.txt
--rw-r--r--   0 mvm       (1000) mvm       (1000)       38 2023-05-05 14:25:52.568626 pandas-chat-0.0.2/setup.cfg
--rw-r--r--   0 mvm       (1000) mvm       (1000)      868 2023-05-05 14:25:31.000000 pandas-chat-0.0.2/setup.py
-drwxr-xr-x   0 mvm       (1000) mvm       (1000)        0 2023-05-05 14:25:52.568626 pandas-chat-0.0.2/tests/
--rw-r--r--   0 mvm       (1000) mvm       (1000)        0 2023-04-28 15:41:44.000000 pandas-chat-0.0.2/tests/__init__.py
--rw-r--r--   0 mvm       (1000) mvm       (1000)     1210 2023-05-05 14:19:09.000000 pandas-chat-0.0.2/tests/test_prompt.py
+drwxr-xr-x   0 mvm       (1000) mvm       (1000)        0 2023-05-06 16:55:46.717630 pandas-chat-0.0.3/
+-rw-r--r--   0 mvm       (1000) mvm       (1000)     1799 2023-03-27 15:45:07.000000 pandas-chat-0.0.3/.gitignore
+-rw-r--r--   0 mvm       (1000) mvm       (1000)     1495 2023-03-27 15:45:07.000000 pandas-chat-0.0.3/LICENSE
+-rw-r--r--   0 mvm       (1000) mvm       (1000)     2279 2023-05-06 16:55:46.717630 pandas-chat-0.0.3/PKG-INFO
+-rw-r--r--   0 mvm       (1000) mvm       (1000)     1915 2023-05-06 16:52:29.000000 pandas-chat-0.0.3/README.md
+-rw-r--r--   0 mvm       (1000) mvm       (1000)      127 2023-05-01 20:01:33.000000 pandas-chat-0.0.3/TODO.md
+drwxr-xr-x   0 mvm       (1000) mvm       (1000)        0 2023-05-06 16:55:46.707630 pandas-chat-0.0.3/pandas_chat/
+-rw-r--r--   0 mvm       (1000) mvm       (1000)        0 2023-04-28 14:50:39.000000 pandas-chat-0.0.3/pandas_chat/__init__.py
+-rw-r--r--   0 mvm       (1000) mvm       (1000)     1007 2023-05-06 16:52:46.000000 pandas-chat-0.0.3/pandas_chat/action.py
+-rw-r--r--   0 mvm       (1000) mvm       (1000)     1403 2023-05-06 16:29:50.000000 pandas-chat-0.0.3/pandas_chat/factory.py
+-rw-r--r--   0 mvm       (1000) mvm       (1000)      459 2023-05-06 16:04:45.000000 pandas-chat-0.0.3/pandas_chat/utils.py
+drwxr-xr-x   0 mvm       (1000) mvm       (1000)        0 2023-05-06 16:55:46.707630 pandas-chat-0.0.3/pandas_chat.egg-info/
+-rw-r--r--   0 mvm       (1000) mvm       (1000)     2279 2023-05-06 16:55:46.000000 pandas-chat-0.0.3/pandas_chat.egg-info/PKG-INFO
+-rw-r--r--   0 mvm       (1000) mvm       (1000)      327 2023-05-06 16:55:46.000000 pandas-chat-0.0.3/pandas_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 mvm       (1000) mvm       (1000)        1 2023-05-06 16:55:46.000000 pandas-chat-0.0.3/pandas_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 mvm       (1000) mvm       (1000)       15 2023-05-06 16:55:46.000000 pandas-chat-0.0.3/pandas_chat.egg-info/requires.txt
+-rw-r--r--   0 mvm       (1000) mvm       (1000)       12 2023-05-06 16:55:46.000000 pandas-chat-0.0.3/pandas_chat.egg-info/top_level.txt
+-rw-r--r--   0 mvm       (1000) mvm       (1000)       38 2023-05-06 16:55:46.717630 pandas-chat-0.0.3/setup.cfg
+-rw-r--r--   0 mvm       (1000) mvm       (1000)      938 2023-05-06 16:55:05.000000 pandas-chat-0.0.3/setup.py
+drwxr-xr-x   0 mvm       (1000) mvm       (1000)        0 2023-05-06 16:55:46.717630 pandas-chat-0.0.3/tests/
+-rw-r--r--   0 mvm       (1000) mvm       (1000)        0 2023-04-28 15:41:44.000000 pandas-chat-0.0.3/tests/__init__.py
```

### Comparing `pandas-chat-0.0.2/.gitignore` & `pandas-chat-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pandas-chat-0.0.2/LICENSE` & `pandas-chat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-chat-0.0.2/pandas_chat/action.py` & `pandas-chat-0.0.3/pandas_chat/action.py`

 * *Files identical despite different names*

### Comparing `pandas-chat-0.0.2/setup.py` & `pandas-chat-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,20 +13,22 @@
     print("Please run:", file=sys.stderr)
     print("", file=sys.stderr)
     print("  python -m pip install scikit-build")
     sys.exit(1)
 
 setup(
     name="pandas-chat",
-    version="0.0.2",
+    version="0.0.3",
     description="pandas-ai is a python library that uses ChatGPT prompts \
         to analyze and process pandas data in a conversational way.",
     long_description=long_description,
+    long_description_content_type='text/markdown',
     author="torshind",
     license="BSD 3-Clause",
     packages=find_packages(exclude=["tests.*", "tests"]),
     url="https://github.com/torshind/pandas-ai",
     keywords="pandas, chatgpt",
     install_requires=[
         "openai",
+        "hugchat",
     ],
 )
```

