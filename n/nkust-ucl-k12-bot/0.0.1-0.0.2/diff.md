# Comparing `tmp/nkust-ucl-k12-bot-0.0.1.tar.gz` & `tmp/nkust-ucl-k12-bot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-0.0.1.tar", last modified: Sat May  6 09:22:41 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-0.0.2.tar", last modified: Sat May  6 09:35:07 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-0.0.1.tar` & `nkust-ucl-k12-bot-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:22:41.044137 nkust-ucl-k12-bot-0.0.1/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-0.0.1/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      430 2023-05-06 09:22:41.043831 nkust-ucl-k12-bot-0.0.1/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       17 2023-05-06 09:19:46.000000 nkust-ucl-k12-bot-0.0.1/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:22:41.041424 nkust-ucl-k12-bot-0.0.1/k12_bot/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-0.0.1/k12_bot/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     5909 2023-05-06 08:44:08.000000 nkust-ucl-k12-bot-0.0.1/k12_bot/bot.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:22:41.042830 nkust-ucl-k12-bot-0.0.1/k12_bot/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-0.0.1/k12_bot/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-0.0.1/k12_bot/utils/config.py
--rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-0.0.1/k12_bot/utils/handler_sqllite.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-0.0.1/k12_bot/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-0.0.1/k12_bot/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:22:41.043579 nkust-ucl-k12-bot-0.0.1/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      430 2023-05-06 09:22:41.000000 nkust-ucl-k12-bot-0.0.1/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      358 2023-05-06 09:22:41.000000 nkust-ucl-k12-bot-0.0.1/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 09:22:41.000000 nkust-ucl-k12-bot-0.0.1/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        8 2023-05-06 09:22:41.000000 nkust-ucl-k12-bot-0.0.1/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 09:22:41.044203 nkust-ucl-k12-bot-0.0.1/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 09:20:55.000000 nkust-ucl-k12-bot-0.0.1/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:35:07.434847 nkust-ucl-k12-bot-0.0.2/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-0.0.2/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      430 2023-05-06 09:35:07.434703 nkust-ucl-k12-bot-0.0.2/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       17 2023-05-06 09:19:46.000000 nkust-ucl-k12-bot-0.0.2/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:35:07.432386 nkust-ucl-k12-bot-0.0.2/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     5909 2023-05-06 09:33:09.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:35:07.433671 nkust-ucl-k12-bot-0.0.2/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl/utils/config.py
+-rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl/utils/handler_sqllite.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:35:07.434405 nkust-ucl-k12-bot-0.0.2/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      430 2023-05-06 09:35:07.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      372 2023-05-06 09:35:07.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 09:35:07.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 09:35:07.000000 nkust-ucl-k12-bot-0.0.2/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 09:35:07.434906 nkust-ucl-k12-bot-0.0.2/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 09:34:24.000000 nkust-ucl-k12-bot-0.0.2/setup.py
```

### Comparing `nkust-ucl-k12-bot-0.0.1/LICENSE` & `nkust-ucl-k12-bot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-0.0.1/k12_bot/bot.py` & `nkust-ucl-k12-bot-0.0.2/nkust_ucl/k12.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.send_user_image = data.get("SendUserImage", "")
         self.timestamp = data.get("Timestamp", 0)
 
     def __str__(self):
         return f"ChatMessage(Mode={self.mode}, MsgID={self.msg_id}, RoomID={self.room_id}, MsgType={self.msg_type}, MsgBody={self.msg_body}, SendUserID={self.send_user_id}, SendUserName={self.send_user_name}, SendUserImage={self.send_user_image}, Timestamp={self.timestamp})"
 
 
-class K12:
+class BOT:
     # K12 class 的實現
     def __init__(self, config_file='config/k12.yaml') -> None:
         self.logger = setup_logger('chatbot')
 
         self.header = {
             'Referer': f'https://k12.54ucl.com/RoomSelection'}
```

### Comparing `nkust-ucl-k12-bot-0.0.1/k12_bot/utils/handler_sqllite.py` & `nkust-ucl-k12-bot-0.0.2/nkust_ucl/utils/handler_sqllite.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-0.0.1/k12_bot/utils/mqtt_client.py` & `nkust-ucl-k12-bot-0.0.2/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-0.0.1/setup.py` & `nkust-ucl-k12-bot-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="0.0.1",
+    version="0.0.2",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

