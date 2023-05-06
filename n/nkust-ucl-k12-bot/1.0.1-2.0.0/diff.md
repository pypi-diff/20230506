# Comparing `tmp/nkust-ucl-k12-bot-1.0.1.tar.gz` & `tmp/nkust-ucl-k12-bot-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-1.0.1.tar", last modified: Sat May  6 09:49:58 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.0.0.tar", last modified: Sat May  6 15:59:21 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-1.0.1.tar` & `nkust-ucl-k12-bot-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:49:58.696314 nkust-ucl-k12-bot-1.0.1/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-1.0.1/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 09:49:58.696001 nkust-ucl-k12-bot-1.0.1/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1532 2023-05-06 09:48:46.000000 nkust-ucl-k12-bot-1.0.1/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:49:58.693997 nkust-ucl-k12-bot-1.0.1/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     5909 2023-05-06 09:33:09.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:49:58.695118 nkust-ucl-k12-bot-1.0.1/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl/utils/config.py
--rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl/utils/handler_sqllite.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 09:49:58.695729 nkust-ucl-k12-bot-1.0.1/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 09:49:58.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      372 2023-05-06 09:49:58.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 09:49:58.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 09:49:58.000000 nkust-ucl-k12-bot-1.0.1/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 09:49:58.696370 nkust-ucl-k12-bot-1.0.1/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 09:49:41.000000 nkust-ucl-k12-bot-1.0.1/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 15:59:21.951110 nkust-ucl-k12-bot-2.0.0/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.0.0/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 15:59:21.950865 nkust-ucl-k12-bot-2.0.0/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1532 2023-05-06 09:48:46.000000 nkust-ucl-k12-bot-2.0.0/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 15:59:21.948184 nkust-ucl-k12-bot-2.0.0/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     6105 2023-05-06 15:52:49.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 15:59:21.949805 nkust-ucl-k12-bot-2.0.0/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl/utils/config.py
+-rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl/utils/handler_sqllite.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 15:59:21.950625 nkust-ucl-k12-bot-2.0.0/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 15:59:21.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      372 2023-05-06 15:59:21.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 15:59:21.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 15:59:21.000000 nkust-ucl-k12-bot-2.0.0/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 15:59:21.951164 nkust-ucl-k12-bot-2.0.0/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 15:37:52.000000 nkust-ucl-k12-bot-2.0.0/setup.py
```

### Comparing `nkust-ucl-k12-bot-1.0.1/LICENSE` & `nkust-ucl-k12-bot-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-1.0.1/PKG-INFO` & `nkust-ucl-k12-bot-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 1.0.1
+Version: 2.0.0
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-1.0.1/README.md` & `nkust-ucl-k12-bot-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-1.0.1/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.0.0/nkust_ucl/k12.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 from .utils.config import K12Config
 from .utils.mqtt_client import K12MqttClient
 
 from .utils.log import setup_logger
 from .utils.handler_sqllite import SQLiteHandler
 
+class MsgType:
+    Text = "Text"
+    Image = "Image"
+    Audio = "audio"
+    Document = "Document"
+    Sticker = "Sticker"
+
+
 class ChatMessage:
     def __init__(self, data):
         self.mode = data.get("Mode", "")
         self.msg_id = data.get("MsgID", "")
         self.room_id = data.get("RoomID", "")
         self.msg_type = data.get("MsgType", "")
         self.msg_body = data.get("MsgBody", "")
@@ -45,14 +53,15 @@
         self.GetMsg = website['GetMsg']
         self.GetMsgHistory = website['GetMsgHistory']
         self.GetContent = website['GetContent']
         self.GetTicketID = website['GetTicketID']
         self.SendMeg = website['SendMeg']
         self.GetRoomInfo = website['GetRoomInfo']
         self.GetRoomName = website['GetRoomName']
+        self.ImageSave = website['ImageSave']
         self.logger.info('K12 website config loaded')
         # 這邊是存取mqtt的部分
         k12mqtt = self.config.get('mqtt', {})
         self.logger.info('K12 mqtt config loaded')
         # 建立mqtt client
         self.client = K12MqttClient(k12mqtt, client_id=str("mqttjs_daa97e1a"), transport=k12mqtt['transport'])
         # 初始化msg
@@ -82,23 +91,23 @@
         return requests.post(f"{self.host}{self.GetTicketID}", headers=self.header).json()
 
     def set_chat_bot_info(self, SendUserID, SendUserName, SendUserImage):
         self.SendUserID = SendUserID
         self.SendUserName = SendUserName
         self.SendUserImage = SendUserImage
 
-    def send_msg(self, roomid, text):
+    def send_msg(self, roomid, text, msg_type=MsgType.Text):
         tit = self.get_ticket()['Timestamp']
         payload = {
             "RoomID": f"{roomid}",
             "SendUserID": self.SendUserID,
             "SendUserName": self.SendUserName,
             "SendUserImage": self.SendUserImage,
             "id": f"{roomid}-{tit}",
-            "MsgType": "Text",
+            "MsgType": msg_type,
             "MsgBody": text,
             "Timestamp": tit
         }
         data = requests.post(f"{self.host}{self.SendMeg}",
                              headers={
                                  'Referer': f'{self.host}/chat/{roomid}'
                              }, json=payload).json()
```

### Comparing `nkust-ucl-k12-bot-1.0.1/nkust_ucl/utils/handler_sqllite.py` & `nkust-ucl-k12-bot-2.0.0/nkust_ucl/utils/handler_sqllite.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-1.0.1/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.0.0/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-1.0.1/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.0.0/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 1.0.1
+Version: 2.0.0
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-1.0.1/setup.py` & `nkust-ucl-k12-bot-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="1.0.1",
+    version="2.0.0",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

