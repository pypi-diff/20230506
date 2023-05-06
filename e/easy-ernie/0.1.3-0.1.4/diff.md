# Comparing `tmp/easy-ernie-0.1.3.tar.gz` & `tmp/easy-ernie-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-ernie-0.1.3.tar", last modified: Thu Apr 27 03:41:12 2023, max compression
+gzip compressed data, was "easy-ernie-0.1.4.tar", last modified: Sat May  6 11:25:52 2023, max compression
```

## Comparing `easy-ernie-0.1.3.tar` & `easy-ernie-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-27 03:41:12.382001 easy-ernie-0.1.3/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.3/LICENSE
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1654 2023-04-27 03:41:12.381861 easy-ernie-0.1.3/PKG-INFO
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1041 2023-04-27 03:38:01.000000 easy-ernie-0.1.3/README.md
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)       38 2023-04-27 03:41:12.382044 easy-ernie-0.1.3/setup.cfg
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      936 2023-04-26 13:00:36.000000 easy-ernie-0.1.3/setup.py
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-27 03:41:12.380411 easy-ernie-0.1.3/src/
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-27 03:41:12.381157 easy-ernie-0.1.3/src/easy_ernie/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      126 2023-04-26 09:22:07.000000 easy-ernie-0.1.3/src/easy_ernie/__init__.py
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     7272 2023-04-27 03:36:55.000000 easy-ernie-0.1.3/src/easy_ernie/ernie.py
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      985 2023-04-27 03:36:51.000000 easy-ernie-0.1.3/src/easy_ernie/fast_ernie.py
-drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-04-27 03:41:12.381697 easy-ernie-0.1.3/src/easy_ernie.egg-info/
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1654 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/PKG-INFO
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)      311 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)        1 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)        9 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/requires.txt
--rw-r--r--   0 xiaoxinyo   (501) staff       (20)       11 2023-04-27 03:41:12.000000 easy-ernie-0.1.3/src/easy_ernie.egg-info/top_level.txt
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-05-06 11:25:52.825613 easy-ernie-0.1.4/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.4/LICENSE
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1960 2023-05-06 11:25:52.825431 easy-ernie-0.1.4/PKG-INFO
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1347 2023-04-29 09:02:38.000000 easy-ernie-0.1.4/README.md
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)       38 2023-05-06 11:25:52.825659 easy-ernie-0.1.4/setup.cfg
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      936 2023-04-29 09:58:19.000000 easy-ernie-0.1.4/setup.py
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-05-06 11:25:52.818039 easy-ernie-0.1.4/src/
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-05-06 11:25:52.819390 easy-ernie-0.1.4/src/easy_ernie/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      126 2023-04-27 13:27:18.000000 easy-ernie-0.1.4/src/easy_ernie/__init__.py
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     7146 2023-05-06 10:46:35.000000 easy-ernie-0.1.4/src/easy_ernie/ernie.py
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      985 2023-05-06 11:25:07.000000 easy-ernie-0.1.4/src/easy_ernie/fast_ernie.py
+drwxr-xr-x   0 xiaoxinyo   (501) staff       (20)        0 2023-05-06 11:25:52.820228 easy-ernie-0.1.4/src/easy_ernie.egg-info/
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)     1960 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)      311 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)        1 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)        9 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/requires.txt
+-rw-r--r--   0 xiaoxinyo   (501) staff       (20)       11 2023-05-06 11:25:52.000000 easy-ernie-0.1.4/src/easy_ernie.egg-info/top_level.txt
```

### Comparing `easy-ernie-0.1.3/LICENSE` & `easy-ernie-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-ernie-0.1.3/PKG-INFO` & `easy-ernie-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.1.3
+Version: 0.1.4
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -12,39 +12,51 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Release](https://img.shields.io/badge/Release-0.1.3-blue)
+![Release](https://img.shields.io/badge/Release-0.1.4-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
 ## 安装
-pip3 install easy-ernie
+pip3 install easy-ernie --upgrade
 ## Cookie
 ![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
 1. 访问[文心一言](https://yiyan.baidu.com).
 2. 打开开发者工具.
 3. 找到应用程序(Application).
 4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
 5. 在列表中点击BAIDUID.
 6. 复制下方Cookie Value的值.
 7. BDUSS_BFESS同理.
 ## 使用
+### Ernie
+```python
+from easy_ernie import Ernie
+
+if __name__ == '__main__':
+    ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
+    sessionId = ernie.newConversation('测试')
+    print(ernie.ask(question, '你好', '0'))
+    ernie.deleteConversation(sessionId)
+```
+### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好'))
+    fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## Acs-Token
 由于文心一言的Acs-Token算法中的参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy-ernie-0.1.3/README.md` & `easy-ernie-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,44 @@
-![Release](https://img.shields.io/badge/Release-0.1.3-blue)
+![Release](https://img.shields.io/badge/Release-0.1.4-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
 ## 安装
-pip3 install easy-ernie
+pip3 install easy-ernie --upgrade
 ## Cookie
 ![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
 1. 访问[文心一言](https://yiyan.baidu.com).
 2. 打开开发者工具.
 3. 找到应用程序(Application).
 4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
 5. 在列表中点击BAIDUID.
 6. 复制下方Cookie Value的值.
 7. BDUSS_BFESS同理.
 ## 使用
+### Ernie
+```python
+from easy_ernie import Ernie
+
+if __name__ == '__main__':
+    ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
+    sessionId = ernie.newConversation('测试')
+    print(ernie.ask(question, '你好', '0'))
+    ernie.deleteConversation(sessionId)
+```
+### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好'))
+    fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## Acs-Token
 由于文心一言的Acs-Token算法中的参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy-ernie-0.1.3/setup.py` & `easy-ernie-0.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='easy-ernie',
-    version='0.1.3',
+    version='0.1.4',
     description='简洁的调用文心一言的WebAPI',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='XiaoXinYo',
     url='https://github.com/XiaoXinYo/Easy-Ernie',
     packages=find_packages('./src'),
     license='MIT',
```

### Comparing `easy-ernie-0.1.3/src/easy_ernie/ernie.py` & `easy-ernie-0.1.4/src/easy_ernie/ernie.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 def getTimestamp():
     return int(time.time() * 1000)
 
 class Ernie:
     def __init__(self, BAIDUID: str, BDUSS_BFESS: str):
         self.BAIDUID = BAIDUID
-        self.BDUSS_BFESS = BDUSS_BFESS
-        self.header = {
+        self.session = requests.Session()
+        self.session.headers = {
             'Host': 'yiyan.baidu.com',
             'Connection': 'keep-alive',
             'Content-Length': '0',
             'sec-ch-ua': '"Chromium";v="112", "Microsoft Edge";v="112", "Not:A-Brand";v="99"',
             'Content-Type': 'application/json',
             'Acs-Token': '',
             'sec-ch-ua-mobile': '?0',
@@ -27,78 +27,79 @@
             'Origin': 'https://yiyan.baidu.com',
             'Sec-Fetch-Site': 'same-site',
             'Sec-Fetch-Mode': 'cors',
             'Sec-Fetch-Dest': 'empty',
             'Referer': 'https://yiyan.baidu.com/',
             'Accept-Encoding': 'gzip, deflate, br',
             'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
-            'Cookie': f'BDUSS_BFESS={self.BDUSS_BFESS};'
+            'Cookie': f'BDUSS_BFESS={BDUSS_BFESS};'
         }
     
     def getSign(self) -> str:
         data = requests.get(f'https://api.hack-er.cn/ernie/acs_token?BAIDUID={self.BAIDUID}',).json()
-        return data.get('data')
+        return data['data']
     
     def checkRequest(self) -> None:
         if self.request.status_code != 200:
             raise Exception('请求失败,请检查网络')
         
         try:
             self.request.json()
         except:
             raise Exception('请求失败,响应格式错误')
         
-        if self.request.json().get('msg') == '请先登录':
-            raise Exception('请求失败,请先登录')
-        elif self.request.json().get('msg') == '用户访问被限制':
-            raise Exception('请求失败,用户访问被限制')
-
-    def get(self, url: str) -> requests:
-        self.request = requests.get(url, headers=self.header)
-        self.checkRequest()
+        if self.request.json()['code'] != 0:
+            raise Exception(f'请求失败,{self.request.json()["msg"]}')
+
+    def get(self, url: str, check=True) -> requests:
+        self.request = self.session.get(url)
+        if check:
+            self.checkRequest()
         return self.request
     
-    def post(self, url: str, data: dict) -> requests:
-        self.header['Content-Length'] = str(len(data))
-        self.request = requests.post(url, headers=self.header, json=data)
-        self.checkRequest()
+    def post(self, url: str, data: dict, check=True) -> requests:
+        self.session.headers['Content-Length'] = str(len(data))
+        self.request = self.session.post(url, json=data)
+        if check:
+            self.checkRequest()
         return self.request
     
     def getConversation(self) -> Union[None, list]:
         data = self.post(
             f'https://yiyan.baidu.com/eb/session/list',
             {
                 'pageSize': 1000,
                 'deviceType': 'pc',
                 'timestamp': getTimestamp()
             }
         ).json()
-        return data.get('data').get('sessions')
+        return data['data']['sessions']
 
     def newConversation(self, name: str) -> str:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/new',
             {
                 'sessionName': name,
                 'timestamp': getTimestamp(),
                 'deviceType': 'pc'
             }
         ).json()
-        return data.get('data').get('sessionId')
+        return data['data']['sessionId']
     
     def deleteConversation(self, sessionId: str) -> bool:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/delete',
             {
                 'sessionId': sessionId,
                 'timestamp': getTimestamp(),
                 'deviceType': 'pc'
-            }
+            },
+            False
         ).json()
-        return True if data.get('code') == 0 else False
+        return True if data['code'] == 0 else False
 
     def renameConversation(self, sessionId: str, name: str) -> bool:
         self.post(
             'https://yiyan.baidu.com/eb/session/new',
             {
                 'sessionId': sessionId,
                 'sessionName': name,
@@ -114,28 +115,28 @@
             {
                 'sessionId': sessionId,
                 'pageSize': 2000,
                 'timestamp': getTimestamp(),
                 'deviceType': 'pc'
             }
         ).json()
-        return data.get('data').get('currentChatId')
+        return data['data']['currentChatId']
 
     def askStream(self, question: str, sessionId: str, parentChatId: str) -> Generator:
         self.post(
             'https://yiyan.baidu.com/eb/chat/check',
             {
                 'text': question,
                 'timestamp': getTimestamp(),
                 'deviceType': 'pc'
             }
         )
 
         sign = self.getSign()
-        self.header['Acs-Token'] = sign
+        self.session.headers['Acs-Token'] = sign
         data = self.post(
             'https://yiyan.baidu.com/eb/chat/new',
             {
                 'sessionId': sessionId,
                 'text': question,
                 'parentChatId': parentChatId,
                 'type': 10,
@@ -143,40 +144,40 @@
                 'deviceType': 'pc',
                 'code': 0,
                 'msg': '',
                 'jt': '',
                 'sign': sign
             }
         ).json()
-        botChatId = data.get('data').get('botChat').get('id')
-        botParentChatId = data.get('data').get('botChat').get('parent')
+        botChatId = data['data']['botChat']['id']
+        botParentChatId = data['data']['botChat']['parent']
 
         fullAnswer = ''
         pattern = r'<img[^>]*\ssrc=[\'"]([^\'"]+)[\'"][^>]*\s/>'
         urls = []
         sentenceId = 0
         while True:
             sign = self.getSign()
-            self.header['Acs-Token'] = sign
+            self.session.headers['Acs-Token'] = sign
             data = self.post(
                 'https://yiyan.baidu.com/eb/chat/query',
                 {
                     'chatId': botChatId,
                     'parentChatId': botParentChatId,
                     'sentenceId': sentenceId,
                     'sessionId': '',
                     'stop': 0,
                     'timestamp': getTimestamp(),
                     'deviceType': 'pc',
                     'sign': sign
                 }
             ).json()
-            data = data.get('data')
-            sentenceId = data.get('sent_id')
-            content = data.get('content')
+            data = data['data']
+            sentenceId = data['sent_id']
+            content = data['content']
             
             if content.strip():
                 fullAnswer += content
                 content = re.sub(pattern, '', content)
                 content = content.replace('<br>', '\n')
                 content = content.strip()
 
@@ -184,15 +185,15 @@
                     'answer': content,
                     'urls': urls,
                     'sessionId': sessionId,
                     'botChatId': botChatId,
                     'done': False
                 }
 
-            if data.get('stop') == 1 or data.get('is_end') == 1:
+            if data['stop'] == 1 or data['is_end'] == 1:
                 break
         
         urls.extend(re.findall(pattern, fullAnswer))
         fullAnswer = re.sub(pattern, '', fullAnswer)
         fullAnswer = fullAnswer.replace('<br>', '\n')
         fullAnswer = fullAnswer.strip()
         
@@ -202,11 +203,11 @@
             'sessionId': sessionId,
             'botChatId': botChatId,
             'done': True
         }
 
     def ask(self, question: str, sessionId: str='', parentChatId: str='') -> dict:
         result = {}
-        for item in self.askStream(question, sessionId, parentChatId):
-            result = item
+        for data in self.askStream(question, sessionId, parentChatId):
+            result = data
         del result['done']
         return result
```

### Comparing `easy-ernie-0.1.3/src/easy_ernie/fast_ernie.py` & `easy-ernie-0.1.4/src/easy_ernie/fast_ernie.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from typing import Generator
 from .ernie import Ernie
 
 class FastErnie:
     def __init__(self, BAIDUID: str, BDUSS_BFESS: str):
         self.ernie = Ernie(BAIDUID, BDUSS_BFESS)
         self.sessionId = ''
-        self.parentChatId = 0
+        self.parentChatId = '0'
 
     def askStream(self, question: str) -> Generator:
         if not self.sessionId:
             self.sessionId = self.ernie.newConversation(question)
-        for item in self.ernie.askStream(question, self.sessionId, self.parentChatId):
-            self.parentChatId = item.get('botChatId')
-            yield item
+        for data in self.ernie.askStream(question, self.sessionId, self.parentChatId):
+            self.parentChatId = data['botChatId']
+            yield data
     
     def ask(self, question: str) -> dict:
         result = {}
-        for item in self.askStream(question):
-            result = item
+        for data in self.askStream(question):
+            result = data
         del result['done']
         return result
     
     def close(self) -> bool:
         if self.ernie.deleteConversation(self.sessionId):
             self.sessionId = ''
-            self.parentChatId = 0
+            self.parentChatId = '0'
             return True
         return False
```

### Comparing `easy-ernie-0.1.3/src/easy_ernie.egg-info/PKG-INFO` & `easy-ernie-0.1.4/src/easy_ernie.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.1.3
+Version: 0.1.4
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -12,39 +12,51 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Release](https://img.shields.io/badge/Release-0.1.3-blue)
+![Release](https://img.shields.io/badge/Release-0.1.4-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
 ## 安装
-pip3 install easy-ernie
+pip3 install easy-ernie --upgrade
 ## Cookie
 ![图片1](https://s1.ax1x.com/2023/04/26/p9KDUYR.md.png)
 1. 访问[文心一言](https://yiyan.baidu.com).
 2. 打开开发者工具.
 3. 找到应用程序(Application).
 4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
 5. 在列表中点击BAIDUID.
 6. 复制下方Cookie Value的值.
 7. BDUSS_BFESS同理.
 ## 使用
+### Ernie
+```python
+from easy_ernie import Ernie
+
+if __name__ == '__main__':
+    ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
+    sessionId = ernie.newConversation('测试')
+    print(ernie.ask(question, '你好', '0'))
+    ernie.deleteConversation(sessionId)
+```
+### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好'))
+    fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## Acs-Token
 由于文心一言的Acs-Token算法中的参数不定时的变化,所以包里调用了API.感兴趣的可以联系我.
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

