# Comparing `tmp/nkust-ucl-k12-bot-2.5.0.tar.gz` & `tmp/nkust-ucl-k12-bot-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.5.0.tar", last modified: Sat May  6 17:31:53 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.6.0.tar", last modified: Sat May  6 17:43:19 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.5.0.tar` & `nkust-ucl-k12-bot-2.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:31:53.986436 nkust-ucl-k12-bot-2.5.0/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.5.0/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 17:31:53.986193 nkust-ucl-k12-bot-2.5.0/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1532 2023-05-06 09:48:46.000000 nkust-ucl-k12-bot-2.5.0/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:31:53.983367 nkust-ucl-k12-bot-2.5.0/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     8299 2023-05-06 17:30:29.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:31:53.985253 nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/config.py
--rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/handler_sqllite.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:31:53.985964 nkust-ucl-k12-bot-2.5.0/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 17:31:53.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      402 2023-05-06 17:31:53.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 17:31:53.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 17:31:53.000000 nkust-ucl-k12-bot-2.5.0/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 17:31:53.986493 nkust-ucl-k12-bot-2.5.0/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 17:30:43.000000 nkust-ucl-k12-bot-2.5.0/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:43:19.880877 nkust-ucl-k12-bot-2.6.0/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.6.0/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     2365 2023-05-06 17:43:19.880623 nkust-ucl-k12-bot-2.6.0/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1952 2023-05-06 17:42:47.000000 nkust-ucl-k12-bot-2.6.0/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:43:19.877847 nkust-ucl-k12-bot-2.6.0/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     8299 2023-05-06 17:30:29.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:43:19.879613 nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/config.py
+-rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/handler_sqllite.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:43:19.880371 nkust-ucl-k12-bot-2.6.0/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     2365 2023-05-06 17:43:19.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      402 2023-05-06 17:43:19.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 17:43:19.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 17:43:19.000000 nkust-ucl-k12-bot-2.6.0/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 17:43:19.880937 nkust-ucl-k12-bot-2.6.0/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 17:43:16.000000 nkust-ucl-k12-bot-2.6.0/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.5.0/LICENSE` & `nkust-ucl-k12-bot-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.5.0/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.6.0/nkust_ucl/k12.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/handler_sqllite.py` & `nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/handler_sqllite.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.5.0/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.6.0/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.5.0/setup.py` & `nkust-ucl-k12-bot-2.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="2.5.0",
+    version="2.6.0",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

