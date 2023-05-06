# Comparing `tmp/m3u8_XZ-0.0.1.tar.gz` & `tmp/m3u8_XZ-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\m3u8_XZ-0.0.1.tar", last modified: Thu Mar 23 07:02:15 2023, max compression
+gzip compressed data, was "H:\PythonProject\XZlib\packaging_m3u8\dist\.tmp-bg_ye6g2\m3u8_XZ-0.0.2.tar", last modified: Sat May  6 04:17:13 2023, max compression
```

## Comparing `m3u8_XZ-0.0.1.tar` & `m3u8_XZ-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 07:02:15.506085 m3u8_XZ-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-03-23 03:00:43.000000 m3u8_XZ-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      459 2023-03-23 07:02:15.505091 m3u8_XZ-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-03-23 02:54:28.000000 m3u8_XZ-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 07:02:15.488138 m3u8_XZ-0.0.1/m3u8_XZ/
--rw-rw-rw-   0        0        0      120 2023-03-23 03:49:25.000000 m3u8_XZ-0.0.1/m3u8_XZ/__init__.py
--rw-rw-rw-   0        0        0     4616 2023-03-23 06:30:55.000000 m3u8_XZ-0.0.1/m3u8_XZ/xz.py
-drwxrwxrwx   0        0        0        0 2023-03-23 07:02:15.501096 m3u8_XZ-0.0.1/m3u8_XZ.egg-info/
--rw-rw-rw-   0        0        0      459 2023-03-23 07:02:15.000000 m3u8_XZ-0.0.1/m3u8_XZ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-03-23 07:02:15.000000 m3u8_XZ-0.0.1/m3u8_XZ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 07:02:15.000000 m3u8_XZ-0.0.1/m3u8_XZ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-23 07:02:15.000000 m3u8_XZ-0.0.1/m3u8_XZ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-03-23 06:48:11.000000 m3u8_XZ-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-23 07:02:15.506085 m3u8_XZ-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-03-23 07:01:48.000000 m3u8_XZ-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:17:13.608021 m3u8_XZ-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-03-23 03:00:43.000000 m3u8_XZ-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      736 2023-05-06 04:17:13.607023 m3u8_XZ-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-05-06 04:16:16.000000 m3u8_XZ-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 04:17:13.594062 m3u8_XZ-0.0.2/m3u8_XZ/
+-rw-rw-rw-   0        0        0      120 2023-03-23 03:49:25.000000 m3u8_XZ-0.0.2/m3u8_XZ/__init__.py
+-rw-rw-rw-   0        0        0      678 2023-05-05 05:15:21.000000 m3u8_XZ-0.0.2/m3u8_XZ/cryptoModel.py
+-rw-rw-rw-   0        0        0     6790 2023-05-06 03:59:07.000000 m3u8_XZ-0.0.2/m3u8_XZ/xz.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:17:13.604035 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/
+-rw-rw-rw-   0        0        0      736 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 04:17:13.000000 m3u8_XZ-0.0.2/m3u8_XZ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      522 2023-03-23 11:30:25.000000 m3u8_XZ-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 04:17:13.608021 m3u8_XZ-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      716 2023-05-06 04:04:36.000000 m3u8_XZ-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:17:13.606026 m3u8_XZ-0.0.2/test/
+-rw-rw-rw-   0        0        0       98 2023-05-06 03:29:10.000000 m3u8_XZ-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0      365 2023-05-06 04:16:49.000000 m3u8_XZ-0.0.2/test/test.py
```

### Comparing `m3u8_XZ-0.0.1/LICENSE` & `m3u8_XZ-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.1/m3u8_XZ/xz.py` & `m3u8_XZ-0.0.2/m3u8_XZ/xz.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # IED:PyCharm
 import time
 import aiohttp
 import asyncio
 import requests as req
 import re
 import os
+from ..m3u8_XZ.cryptoModel import DecodeByte
 
 
 class M3U8:
     """
         url: m3u8文件的url
         folder: 下载文件后存储的名字
         run(): 执行下载
     """
-
-    def __init__(self, url, folder='test'):
+    def __init__(self, url=None, folder='test', m3u8_file=None):
         # 下载文件名
         self.file_name = folder + '.mp4'
         # 下载存储文件夹
         self.path = './down_load/' + folder + '/'
         if not os.path.exists(self.path):
             os.makedirs(self.path)
         # 缓存文件夹
@@ -30,23 +30,34 @@
         if not os.path.exists(self.temp_path):
             os.makedirs(self.temp_path)
         # m3u8
         self.url = url
         self.headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
         }
+        self.m3u8_file = m3u8_file
         # 记录进度
         self.list_length = 0
         self.num = 0
         # 有序存储ts列表文件
         self.ts_list = list()
+        # 解密处理
+        self.cry = {
+            "key": "",
+            "iv": "",
+            "method": "",
+        }
 
     # 通过ts名称，转换ts网址
     @staticmethod
-    def get_full_ts_url(url, ts_name):
+    def get_full_ts_url(url, ts_name: str):
+        # 直接返回http地址
+        if ts_name.startswith("http"):
+            return ts_name
+        # 需要拼接完整url地址
         # 分割ts name
         tl = ts_name.split('/')
         #
         new_url = []
         # 循环url，去掉ts name中重复的部分
         for s in url.split('/')[:-1]:
             if s in tl:
@@ -56,78 +67,121 @@
         new_url.extend(tl)
         result = '/'.join(new_url)
         # 返回
         return result
 
     # 通过url，获取ts列表
     def get_ts_list(self) -> list:
-        res = req.get(self.url, headers=self.headers, verify=False)
-        if res.status_code != 200:
-            raise Exception('亲求失败,m3u8地址不存在')
-        text = res.text
+        # 通过本地文件获取
+        if self.m3u8_file:
+            with open(self.m3u8_file, 'r', encoding='utf8') as f:
+                text = f.read()
+        # 通过url获取m3u8文件内容
+        elif self.url:
+            res = req.get(self.url, headers=self.headers, verify=False)
+            if res.status_code != 200:
+                raise Exception('请求失败,m3u8地址不存在')
+            text = res.text
         # 去掉注释
         ts_str = re.sub('#.*?\n', '', text)
         # 转为列表
         self.ts_list = ts_str.split('\n')
         self.list_length = len(self.ts_list)
+        # 设置加密参数
+        self.set_cry(text, '/'.join(self.url.split('/')[:-1]) + '/')
+
         return self.ts_list
 
+    def set_cry(self, text, url=""):
+        # 获取加密参数
+        x_key = re.findall('#EXT-X-KEY:(.*?)\n', text)
+        cry_obj = dict()
+        if len(x_key) > 0:
+            # 提取
+            for item in x_key[0].split(','):
+                cry_obj[item.split('=')[0]] = item.split('=')[1].replace('"', '')
+            # format
+            if cry_obj['URI'] and not cry_obj['URI'].startswith('http'):
+                cry_obj['URI'] = url + cry_obj['URI']
+            # 获取key
+            res = req.get(cry_obj['URI'], headers=self.headers)
+            self.cry['key'] = res.content
+            # 加密方式
+            self.cry['method'] = cry_obj['METHOD']
+            # iv值
+            if cry_obj.get('IV'):
+                self.cry['iv'] = cry_obj['IV'][2:18]
+
+        else:
+            pass
+
     # 通过ts列表，异步缓存所有ts文件
     async def get_data(self):
         async with aiohttp.ClientSession(headers=self.headers) as session:
             tasks = []
-            for index, ts in enumerate(self.get_ts_list()):
+            for index, ts in enumerate(self.get_ts_list(), 1):
                 if ts:
                     # 给ts重命名，为了排序
                     temp_ts = str(index).zfill(6) + '.mp4'
                     # 创建task任务
                     task = asyncio.create_task(self.down_file(session, self.get_full_ts_url(self.url, ts), temp_ts))
                     tasks.append(task)
             # 添加到事件循环
             await asyncio.wait(tasks)
 
     # 异步下载二进制文件
     async def down_file(self, session, url, ts_name):
         async with session.get(url) as res:
             data = await res.read()
+            # 如果有加密，需要data解密后再存储
+            if self.cry['key']:
+                # 如果源文件有iv就读取，如果没有就用文件名
+                iv = self.cry["iv"] if self.cry["iv"] else ts_name.split('.')[0].zfill(16)
+                data = DecodeByte.do_decode(self.cry["key"], iv, data, self.cry["method"])
+                if not data:
+                    raise Exception('解密失败')
+            # 保存
             with open(self.temp_path + ts_name, 'wb') as f:
                 f.write(data)
                 # 打印进度
                 self.num += 1
                 print('\r下载中:{:3.0f}%| {}/{}'.format(self.num / self.list_length * 100, self.num, self.list_length),
                       end='', flush=True)
 
     # 通过名称按序读取ts文件，整合成一个ts文件
-    def combine_ts(self):
+    @staticmethod
+    def combine_ts(source_path, dest_file):
         # 获取所有缓存文件
-        file_list = os.listdir(self.temp_path)
+        file_list = os.listdir(source_path)
         if not file_list:
             return
-        # 排序
+        # 名称排序
         file_list.sort(key=lambda s: s.split('.')[0])
         # 文件总数
         length = len(file_list)
         # 开始合并文件
-        with open(self.path + self.file_name, 'ab') as f:
+        with open(dest_file, 'ab') as f:
             # 循环文件列表
             for i, file in enumerate(file_list):
                 # 读取每个文件
-                with open(self.temp_path + file, 'rb') as rf:
+                with open(source_path + file, 'rb') as rf:
                     # 把每个文件的内容 追加到同一个文件
                     data = rf.read()
                     f.write(data)
                 # 清除缓存文件
-                os.remove(self.temp_path + file)
+                os.remove(source_path + file)
                 # 打印进度
                 print('\r合并中:{:3.0f}%'.format(i / length * 100), end='', flush=True)
+        # 移除缓存文件夹
+        os.rmdir(source_path)
 
     # 异步启动器
     def run(self):
-        if self.url:
+        if self.url or self.m3u8_file:
             stime = time.time()
             loop = asyncio.get_event_loop()
             loop.run_until_complete(self.get_data())
             print('下载完成，准备合并...')
             time.sleep(2)
-            self.combine_ts()
+            self.combine_ts(self.temp_path, self.path + self.file_name)
             print('\nover time : ', time.time() - stime)
```

### Comparing `m3u8_XZ-0.0.1/pyproject.toml` & `m3u8_XZ-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -17,30 +17,8 @@
 #    "Operating System :: OS Independent",
 #]
 #dependencies = [
 #    "requests",
 #    'aiohttp',
 #]
 #
-#[build-system]
-#requires = ["setuptools>=61.0"]
-#build-backend = "setuptools.build_meta"
-#
-#[project]
-#name = "m3u8_XZ"
-#version = "0.0.1"
-#authors = [
-#  { name="XZ", email="345841407@qq.com" },
-#]
-#description = "download m3u8 video"
-#readme = "README.md"
-#requires-python = ">=3.7"
-#classifiers = [
-#    "Programming Language :: Python :: 3",
-#    "License :: OSI Approved :: MIT License",
-#    "Operating System :: OS Independent",
-#]
-#dependencies = [
-#    "requests",
-#    'aiohttp',
-#]
 #
```

### Comparing `m3u8_XZ-0.0.1/setup.py` & `m3u8_XZ-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="m3u8_XZ",
-    version="0.0.1",
+    version="0.0.2",
     author="XZ",
     author_email="345841407@qq.com",
     description="download m3u8 video",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    requires=["requests", "aiohttp"],
+    install_requires=["requests", "aiohttp", "pycryptodome"],
 )
```

