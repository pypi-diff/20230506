# Comparing `tmp/nkust-ucl-k12-bot-2.1.0.tar.gz` & `tmp/nkust-ucl-k12-bot-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.1.0.tar", last modified: Sat May  6 16:26:26 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.2.0.tar", last modified: Sat May  6 16:40:45 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.1.0.tar` & `nkust-ucl-k12-bot-2.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 16:26:26.025331 nkust-ucl-k12-bot-2.1.0/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.1.0/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 16:26:26.025078 nkust-ucl-k12-bot-2.1.0/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1532 2023-05-06 09:48:46.000000 nkust-ucl-k12-bot-2.1.0/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 16:26:26.022229 nkust-ucl-k12-bot-2.1.0/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     7056 2023-05-06 16:23:20.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 16:26:26.023963 nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      751 2023-05-06 16:16:43.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/config.py
--rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/handler_sqllite.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 16:26:26.024808 nkust-ucl-k12-bot-2.1.0/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 16:26:25.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      402 2023-05-06 16:26:26.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 16:26:25.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 16:26:25.000000 nkust-ucl-k12-bot-2.1.0/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 16:26:26.025389 nkust-ucl-k12-bot-2.1.0/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 16:26:23.000000 nkust-ucl-k12-bot-2.1.0/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 16:40:45.350187 nkust-ucl-k12-bot-2.2.0/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.2.0/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 16:40:45.349961 nkust-ucl-k12-bot-2.2.0/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1532 2023-05-06 09:48:46.000000 nkust-ucl-k12-bot-2.2.0/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 16:40:45.347458 nkust-ucl-k12-bot-2.2.0/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     7051 2023-05-06 16:39:42.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 16:40:45.349016 nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      751 2023-05-06 16:16:43.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/config.py
+-rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/handler_sqllite.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 16:40:45.349728 nkust-ucl-k12-bot-2.2.0/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1945 2023-05-06 16:40:45.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      402 2023-05-06 16:40:45.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 16:40:45.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 16:40:45.000000 nkust-ucl-k12-bot-2.2.0/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 16:40:45.350244 nkust-ucl-k12-bot-2.2.0/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 16:40:44.000000 nkust-ucl-k12-bot-2.2.0/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.1.0/LICENSE` & `nkust-ucl-k12-bot-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.1.0/PKG-INFO` & `nkust-ucl-k12-bot-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.1.0
+Version: 2.2.0
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.1.0/README.md` & `nkust-ucl-k12-bot-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.1.0/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.2.0/nkust_ucl/k12.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         self.SendUserID = SendUserID
         self.SendUserName = SendUserName
         self.SendUserImage = SendUserImage
 
     def image_saver(self, roomid, url):
         attachment = Attachment(url)
         attachment_data = attachment.get_attachment()
-        files = {"uploadFile": ("image.jpg", attachment_data, "image/jpeg")}
+        files = {"Image": ("image.jpg", attachment_data, "image/jpeg")}
         data = requests.post(f"{self.host}{self.ImageSave}",
                              headers={
                                  'Referer': f'{self.host}/Chat/{roomid}'
                              },files=files).json()
         #ErrorCode
         if data.get('ErrorCode', 0) == 0:
             return data.get('FileName', '')
```

### Comparing `nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/handler_sqllite.py` & `nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/handler_sqllite.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.1.0/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.2.0/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.1.0/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.2.0/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.1.0
+Version: 2.2.0
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.1.0/setup.py` & `nkust-ucl-k12-bot-2.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="2.1.0",
+    version="2.2.0",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

