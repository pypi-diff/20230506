# Comparing `tmp/nkust-ucl-k12-bot-2.6.2.tar.gz` & `tmp/nkust-ucl-k12-bot-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.6.2.tar", last modified: Sat May  6 17:51:48 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.6.3.tar", last modified: Sat May  6 17:53:13 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.6.2.tar` & `nkust-ucl-k12-bot-2.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:51:48.582733 nkust-ucl-k12-bot-2.6.2/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.6.2/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4050 2023-05-06 17:51:48.582472 nkust-ucl-k12-bot-2.6.2/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     3637 2023-05-06 17:51:36.000000 nkust-ucl-k12-bot-2.6.2/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:51:48.579437 nkust-ucl-k12-bot-2.6.2/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     8299 2023-05-06 17:30:29.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:51:48.581276 nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/config.py
--rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/handler_sqllite.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:51:48.582225 nkust-ucl-k12-bot-2.6.2/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4050 2023-05-06 17:51:48.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      402 2023-05-06 17:51:48.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 17:51:48.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 17:51:48.000000 nkust-ucl-k12-bot-2.6.2/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 17:51:48.582793 nkust-ucl-k12-bot-2.6.2/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 17:51:47.000000 nkust-ucl-k12-bot-2.6.2/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:53:13.216040 nkust-ucl-k12-bot-2.6.3/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.6.3/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-06 17:53:13.215781 nkust-ucl-k12-bot-2.6.3/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     3640 2023-05-06 17:52:32.000000 nkust-ucl-k12-bot-2.6.3/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:53:13.213201 nkust-ucl-k12-bot-2.6.3/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     8299 2023-05-06 17:30:29.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:53:13.214825 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/config.py
+-rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/handler_sqllite.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:53:13.215547 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-06 17:53:13.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      402 2023-05-06 17:53:13.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 17:53:13.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 17:53:13.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 17:53:13.216156 nkust-ucl-k12-bot-2.6.3/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 17:52:56.000000 nkust-ucl-k12-bot-2.6.3/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.6.2/LICENSE` & `nkust-ucl-k12-bot-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.2/PKG-INFO` & `nkust-ucl-k12-bot-2.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.6.2
+Version: 2.6.3
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -69,15 +69,15 @@
 # run要在最後面
 custom_k12.run()
 ```
 
 ### **初始化 K12 Bot**
 
 ```python
-from nkust_ucl_k12_bot import K12
+from nkust_ucl.k12 import BOT as K12
 custom_k12 = K12(config_file='config/k12.yaml')
 custom_k12.set_chat_bot_info(
     SendUserID="my_id",
     SendUserName="ChatGPT_ucl",
     SendUserImage="https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/512px-ChatGPT_logo.svg.png"
 )
```

### Comparing `nkust-ucl-k12-bot-2.6.2/README.md` & `nkust-ucl-k12-bot-2.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 # run要在最後面
 custom_k12.run()
 ```
 
 ### **初始化 K12 Bot**
 
 ```python
-from nkust_ucl_k12_bot import K12
+from nkust_ucl.k12 import BOT as K12
 custom_k12 = K12(config_file='config/k12.yaml')
 custom_k12.set_chat_bot_info(
     SendUserID="my_id",
     SendUserName="ChatGPT_ucl",
     SendUserImage="https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/512px-ChatGPT_logo.svg.png"
 )
```

### Comparing `nkust-ucl-k12-bot-2.6.2/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.6.3/nkust_ucl/k12.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/handler_sqllite.py` & `nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/handler_sqllite.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.2/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.2/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.6.2
+Version: 2.6.3
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -69,15 +69,15 @@
 # run要在最後面
 custom_k12.run()
 ```
 
 ### **初始化 K12 Bot**
 
 ```python
-from nkust_ucl_k12_bot import K12
+from nkust_ucl.k12 import BOT as K12
 custom_k12 = K12(config_file='config/k12.yaml')
 custom_k12.set_chat_bot_info(
     SendUserID="my_id",
     SendUserName="ChatGPT_ucl",
     SendUserImage="https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/512px-ChatGPT_logo.svg.png"
 )
```

### Comparing `nkust-ucl-k12-bot-2.6.2/setup.py` & `nkust-ucl-k12-bot-2.6.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="2.6.2",
+    version="2.6.3",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

