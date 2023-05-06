# Comparing `tmp/inhandtest-0.0.41.tar.gz` & `tmp/inhandtest-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.41.tar", last modified: Thu May  4 02:53:57 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.42.tar", last modified: Sat May  6 07:40:04 2023, max compression
```

## Comparing `inhandtest-0.0.41.tar` & `inhandtest-0.0.42.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 02:53:57.000000 inhandtest-0.0.41/
--rw-rw-rw-   0        0        0      535 2023-05-04 02:53:57.000000 inhandtest-0.0.41/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.41/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 02:53:57.000000 inhandtest-0.0.41/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.41/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 02:53:57.000000 inhandtest-0.0.41/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.41/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.41/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.41/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.41/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.41/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.41/inhandtest/file.py
--rw-rw-rw-   0        0        0    11860 2023-04-28 07:50:11.000000 inhandtest-0.0.41/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.41/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.41/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    45529 2023-04-24 06:54:53.000000 inhandtest-0.0.41/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.41/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.41/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.41/inhandtest/ip.py
--rw-rw-rw-   0        0        0     4736 2023-05-04 02:38:53.000000 inhandtest-0.0.41/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.41/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32413 2023-04-21 10:20:01.000000 inhandtest-0.0.41/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25167 2023-04-28 06:14:33.000000 inhandtest-0.0.41/inhandtest/tools.py
--rw-rw-rw-   0        0        0      117 2023-04-28 07:34:58.000000 inhandtest-0.0.41/requirements.txt
--rw-rw-rw-   0        0        0     1421 2023-05-04 02:52:29.000000 inhandtest-0.0.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:40:04.000000 inhandtest-0.0.42/
+-rw-rw-rw-   0        0        0      535 2023-05-06 07:40:04.000000 inhandtest-0.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.42/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 07:40:04.000000 inhandtest-0.0.42/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.42/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:40:04.000000 inhandtest-0.0.42/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.42/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    37327 2023-05-06 07:36:45.000000 inhandtest-0.0.42/inhandtest/base_page/_ig902_contents_locators.py
+-rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.42/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    43975 2023-05-06 07:36:45.000000 inhandtest-0.0.42/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.42/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.42/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.42/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.42/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.42/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.42/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    45529 2023-04-24 06:54:53.000000 inhandtest-0.0.42/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.42/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.42/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6213 2023-05-06 01:08:13.000000 inhandtest-0.0.42/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.42/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11606 2023-05-06 06:45:39.000000 inhandtest-0.0.42/inhandtest/mail.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.42/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32728 2023-05-06 01:14:17.000000 inhandtest-0.0.42/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25206 2023-05-06 07:30:45.000000 inhandtest-0.0.42/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      123 2023-05-06 01:36:21.000000 inhandtest-0.0.42/requirements.txt
+-rw-rw-rw-   0        0        0     1438 2023-05-06 07:38:40.000000 inhandtest-0.0.42/setup.py
```

### Comparing `inhandtest-0.0.41/PKG-INFO` & `inhandtest-0.0.42/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inhandtest
-Version: 0.0.41
+Version: 0.0.42
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 License: UNKNOWN
 Description: 方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；
         映翰通出品，追尾必究！
```

### Comparing `inhandtest-0.0.41/README.md` & `inhandtest-0.0.42/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.42/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/base_page/base_page.py` & `inhandtest-0.0.42/inhandtest/base_page/base_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,68 +5,75 @@
 """
 base_page
 
 """
 import os.path
 import sys
 from os import path
+from inhandtest.base_page._ig902_contents_locators import IGContentsLocators
 from typing import List
-from inhandtest.exception import ModelError, ParameterValueError
+from inhandtest.exception import ModelError
 from inhandtest.tools import loop_inspector
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
 from inhandtest.base_page._vg710_contents_locators import VGContentsLocators
 from inhandtest.base_page.table_tr import Table
 import allure
 import logging
 import re
 
 
 class BasePage:
 
-    def __init__(self, host: str, username: str, password: str, protocol='https',
-                 port=443, model='VG710', language='en', playwright_: sync_playwright = None, **kwargs):
+    def __init__(self, host: str, username: str, password: str, protocol='https', page: Page = None,
+                 port=443, model='VG710', language='en', **kwargs):
         """
 
         :param host:  设备主机地址
         :param username: 用户名
         :param password: 密码
         :param protocol: 协议
         :param port: 端口
         :param model: 'VG710'|'ER805'|'ER605'|'IR302'|'IG502'|'IG902'
-        :param playwright_: 当传入playwright时，自动打开浏览器及页面，如为None 需要传入对应的page
-        :param kwargs:  'page'|'http_credentials'|'browser'
+        :param page: 当page为None时，自动打开浏览器及页面，否则使用传入的page
+        :param kwargs:
                       browser: 当没有传入page时，可以选择浏览器
-                      page: 页面, 当没有playwright时，需要传入页面对象
                       dialog_massages: dict
                       tip_messages: dict
                       text_messages: dict
                       title_messages: dict
         """
-        self.page: Page = kwargs.get('page')
+        self.page = page
         self.host = host
         self.model = model.upper()
         self.protocol = protocol
         self.port = port
         self.__username = username
         self.__password = password
         self.language = language
-        self.__playwright = playwright_
         self.__browser_type = kwargs.get('browser')
-        self.page: Page = kwargs.get('page')
+        self.__http_credentials_model = ('VG710', )   # 需要使用http认证的设备, 没有登录页面 只有登录弹窗
+        if self.__browser_type is None:
+            self.__new_page()
         if self.model == 'VG710':
             self.content_locator = VGContentsLocators(self.page, language).tags_menu
-            self.__http_credentials = True
+        elif self.model == 'IG902':
+            self.content_locator = IGContentsLocators(self.page, language).tags_menu
         else:
             raise ModelError(f'not support this mode {model}')
-        self.__new_context()
         self.__dialog_massages = kwargs.get('dialog_massages')
         self.__tip_messages = kwargs.get('tip_messages')
         self.__text_messages = kwargs.get('text_messages')
         self.__title_messages = kwargs.get('title_messages')
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+
     @property
     def __login_locator(self) -> dict:
         if self.model == 'VG710':
             return {'wait_locator': self.page.locator('#logo')}
         elif self.model in ('ER805', 'ER605'):
             return {'username': self.page.locator('#username'), 'password': self.page.locator('#password'),
                     'submit': self.page.locator('button'),
@@ -78,35 +85,35 @@
         elif self.model == 'IR302':
             return {'username': self.page.locator('#username'), 'password': self.page.locator('#passwd'),
                     'submit': self.page.locator('.login_button"]'),
                     'wait_locator': self.page.locator('#logo')}
         else:
             raise Exception(f'not support this model {self.model}')
 
-    def __new_context(self):
+    def __new_page(self):
         def dialog_(dialog):
             logging.info(f'dialog message is {dialog.message}, accepted')
             dialog.accept()
 
-        if self.__playwright:
-            if self.__browser_type == 'firefox':
-                firefox = self.__playwright.firefox
-            elif self.__browser_type == 'webkit':
-                firefox = self.__playwright.webkit
-            else:
-                firefox = self.__playwright.chromium
-            self.__browser = firefox.launch(headless=False)
-            http_credentials = {'username': self.__username,
-                                'password': self.__password} if self.__http_credentials else None
-            self.__context = self.__browser.new_context(ignore_https_errors=True, http_credentials=http_credentials)
-            logging.info('Start your journey browser is chrome')
-            self.page: Page = self.__context.new_page()
-            self.page.on("dialog", dialog_)
-        elif self.page is None:
-            raise ParameterValueError('init BasePage error, the page and playwright_ param is None')
+        self.__playwright = sync_playwright().start()
+        if self.__browser_type == 'firefox':
+            browser = self.__playwright.firefox
+        elif self.__browser_type == 'webkit':
+            browser = self.__playwright.webkit
+        else:
+            browser = self.__playwright.chromium
+        self.__browser = browser.launch(headless=False)
+        if self.model in self.__http_credentials_model:
+            http_credentials = {'username': self.__username, 'password': self.__password}
+        else:
+            http_credentials = None
+        self.__context = self.__browser.new_context(ignore_https_errors=True, http_credentials=http_credentials)
+        logging.info('Start your journey browser is chrome')
+        self.page = self.__context.new_page()
+        self.page.on("dialog", dialog_)
 
     @allure.step("用户登录")
     def login(self, username=None, password=None, status='success') -> None:
         """
 
         :param username:  如果不传使用默认的用户名
         :param password:  如果不传使用默认的密码
@@ -120,21 +127,21 @@
             device = "{}://{}:{}".format(self.protocol, self.host, self.port)
             try:
                 self.page.goto(device, timeout=120 * 1000)
             except Exception:
                 raise
             self.page.bring_to_front()
             self.page.wait_for_timeout(500)
-            if self.__http_credentials:
+            if self.model in self.__http_credentials_model:
                 logging.info(f'Open {self.host} device address {device} and login')
             else:
                 logging.info(f'Open {self.host} device address {device}')
 
         def _login():
-            if not self.__http_credentials:
+            if self.model not in self.__http_credentials_model:
                 self.__login_locator.get('username').fill(username)
                 logging.info('Device %s fill username %s' % (self.host, username))
                 self.__login_locator.get('password').fill(password)
                 logging.info('Device %s fill password %s' % (self.host, password))
                 self.__login_locator.get('submit').click()
                 logging.info("Device %s  login" % self.host)
                 if status == 'success':
@@ -788,31 +795,30 @@
                 else:
                     os.popen(command)
                 if not tag_result:
                     break
         return tag_result
 
     def close(self) -> None:
-        self.page.close()
-        self.__context.close()
-        self.__browser.close()
+        if self.__context and self.__browser and self.__playwright:
+            self.__context.close()
+            self.__browser.close()
+            self.__playwright.stop()
 
 
 if __name__ == '__main__':
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
-    with sync_playwright() as playwright:
-        my_base = BasePage('10.5.24.206', 'adm', '123456', 'http', 80, 'VG710', 'en', playwright,
-                           http_credentials=True, )
-        my_base.access_menu('administration_system_time.ntp_server')
-
+    with BasePage('10.5.24.96', 'adm', '123456', model='IG902') as my_page:
+        my_page.access_menu('system.system_network_tools')
+        my_page.page.wait_for_timeout(5 * 1000)
         # user_table = Table(
         #     [('mode', 'input'), ('status', 'input'), ('ssid', 'input'),  ('mac', 'input'),
         #      ('auth', 'input'), ('encry', 'input'), ('network', 'input'), ('gateway', 'input'), ('dns', 'input'), ('time', 'input')],
         #     my_base.page.frame_locator('#window_content').locator('#wifi-2g-grid'),
         #     ['mode', 'status', 'ssid', 'mac', 'auth', 'encry', 'network', 'gateway', 'dns', 'time'], None)
         # a = user_table.exists([{'mode': "'${value}'!='AP'", 'ssid': 'inhand-visitor-2g'}])
         # print(a)
         # print(user_table.exist(locale={'disable': 'Disabled'}, mode="'${value}'!='AP'", ssid='inhand-visitor-2g', status='disable'))
         # user_table.delete(name='test2', value='222')
         # my_base.page.wait_for_timeout(5 * 1000)
-        my_base.close()
+
```

### Comparing `inhandtest-0.0.41/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.42/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/exception.py` & `inhandtest-0.0.42/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/file.py` & `inhandtest-0.0.42/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/inmodbus.py` & `inhandtest-0.0.42/inhandtest/inmodbus.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 import ctypes
 import re
 from modbus_tk import modbus_rtu, modbus_tcp, utils
 
 
 class ModbusMaster:
-    __doc__ = "使用前需安装pyserial modbus-tk"
+    __doc__ = "使用前需安装pyserial, modbus-tk"
 
     def __init__(self, protocol: str, host: str, port=502, slave_id=1, baud_rate=9600, bytesize=8, parity='N',
                  stop_bits=1):
         """
         创建modbus master
         :param protocol: 协议类型| TCP| RTU
         :param host: 当协议为TCP时，填入IP地址，当协议为RTU时，填入串口号
```

### Comparing `inhandtest-0.0.41/inhandtest/inmongodb.py` & `inhandtest-0.0.42/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/inmqtt.py` & `inhandtest-0.0.42/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/inrequest.py` & `inhandtest-0.0.42/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/insocket.py` & `inhandtest-0.0.42/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/inssh.py` & `inhandtest-0.0.42/inhandtest/inssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,20 @@
         except AuthenticationException:
             raise AuthenticationException(f"ssh connect {self.__host} Username or Password error")
         except Exception:
             raise ConnectionError(f"ssh connect {self.__host} connect error")
         self.transport.connect(username=username, password=password)
         self.sftp = paramiko.SFTPClient.from_transport(self.transport)
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+
     def exec_command(self, command: str) -> str:
         """执行命令并返回结果
 
         :param command: 执行命令, 多条时使用分号隔开
         :return: 返回所有命令执行后的结果
         """
         result = None
```

### Comparing `inhandtest-0.0.41/inhandtest/ip.py` & `inhandtest-0.0.42/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/pytest_email.html` & `inhandtest-0.0.42/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.41/inhandtest/telnet.py` & `inhandtest-0.0.42/inhandtest/telnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,21 @@
         self.tn.write("{}\n".format(self.password).encode("cp936"))
         login_result = self.tn.read_until(login_spe.get(self.model).encode("cp936"), timeout=20).decode("cp936").strip()
         logging.info(login_result)
         if 'Login incorrect' in login_result:
             raise Exception('UsernameOrPasswordError')
         self.update_hostname(login_result.split('\r\n')[-1].split(' ')[-1][:-1])
         logging.info(f"Device {self.host} login success. user_tag: {self.user_tag}")
+        return self
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
 
     def __auto_login(function):
         """自动重新登录, 只能当装饰器使用， 不对外使用
 
         :param function:
         :return:
         """
@@ -630,12 +637,16 @@
         logging.info("Telnet 【%s:%s】 close connect session" % (self.host, self.port))
 
 
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO, stream=sys.stdout)
+    device = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
+    # device.send_cli('ifconfig', '/www #', 'super')
+
+        # device = Telnet('IG902', '
     # device = Telnet('VG710', '10.5.24.206', 'inhand', '64391099@inhand')
     # a = device.send_cli('ping www.baidu.com -c 4', '/www #', 'super')
-    print(eval('1==2'))
+    # print(eval('1==2'))
     # device.assert_cli('ifconfig |grep wifi', expect='Local', interface_replace_type='cli_expect_last_read')
     # print(device.re_match('ifconfig eth0', r'HWaddr(.*)inet6', key_replace={'\r\n':'', ' ': ''}))
```

### Comparing `inhandtest-0.0.41/inhandtest/tools.py` & `inhandtest-0.0.42/inhandtest/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     """
 
     def timeout_(func):
         @wraps(func)
         def inspector(*args, **kwargs):
             nonlocal timeout, interval
             timeout = kwargs.get('timeout') if kwargs.get('timeout') else timeout
-            interval = kwargs.get('timeout') if kwargs.get('interval') else interval
-            for i in range(0, timeout + 1, interval):
+            interval = kwargs.get('interval') if kwargs.get('interval') else interval
+            for i in range(0, timeout, interval):
                 result = func(*args, **kwargs)
                 if not result:
                     logging.info(f'{flag} assert failure, wait for {interval}s inspection')
                     time.sleep(interval)
                     continue
                 else:
                     logging.info(f'{flag} assert normal')
@@ -596,11 +596,12 @@
 
 
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
+    check_windows_process('sscom', True)
     # is_installed('Google Chrome123')
     # print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
     # print(generate_password(length=2, lowercase=True, uppercase=True, special_chars=True, chinese_chars=True))
     # print(get_time_stamp('2022-02-18T13:39:32Z', -2))
```

### Comparing `inhandtest-0.0.41/setup.py` & `inhandtest-0.0.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.41',
+    version='0.0.42',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
@@ -23,11 +23,11 @@
     package_data={'inhandtest': ['pytest_email.html']},
     url='https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》',
     long_description='方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；\n映翰通出品，追尾必究！',
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=['pytz', 'requests', 'playwright', 'pyserial', 'modbus-tk', 'paho-mqtt', 'urllib3', 'paramiko',
-                      'emails', 'Jinja2', 'pymongo',
+                      'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml'
                       # 这里是依赖列表，表示运行这个包的运行某些功能还需要你安装其他的包
                       ],
 )
```

