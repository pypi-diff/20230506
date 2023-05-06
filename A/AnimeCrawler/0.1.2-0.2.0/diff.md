# Comparing `tmp/AnimeCrawler-0.1.2.tar.gz` & `tmp/AnimeCrawler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnimeCrawler-0.1.2.tar", last modified: Wed May  3 03:36:47 2023, max compression
+gzip compressed data, was "AnimeCrawler-0.2.0.tar", last modified: Sat May  6 14:39:52 2023, max compression
```

## Comparing `AnimeCrawler-0.1.2.tar` & `AnimeCrawler-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.215752 AnimeCrawler-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.136797 AnimeCrawler-0.1.2/AnimeCrawler/
--rw-rw-rw-   0        0        0      353 2023-05-03 02:47:47.000000 AnimeCrawler-0.1.2/AnimeCrawler/__init__.py
--rw-rw-rw-   0        0        0      281 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/__main__.py
--rw-rw-rw-   0        0        0     2198 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/base_spider.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.185769 AnimeCrawler-0.1.2/AnimeCrawler/command/
--rw-rw-rw-   0        0        0       76 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/command/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-05-03 03:12:56.000000 AnimeCrawler-0.1.2/AnimeCrawler/command/run.py
--rw-rw-rw-   0        0        0      356 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/log.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.193771 AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/
--rw-rw-rw-   0        0        0      256 2023-05-03 02:47:31.000000 AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/downloader.py
--rw-rw-rw-   0        0        0     4172 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/spider.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.211754 AnimeCrawler-0.1.2/AnimeCrawler/utils/
--rw-rw-rw-   0        0        0      121 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/utils/decode.py
--rw-rw-rw-   0        0        0     2154 2023-05-03 02:47:10.000000 AnimeCrawler-0.1.2/AnimeCrawler/utils/file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:36:47.179773 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/
--rw-rw-rw-   0        0        0     3406 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 03:36:46.000000 AnimeCrawler-0.1.2/AnimeCrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3406 2023-05-03 03:36:47.213753 AnimeCrawler-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2957 2023-05-03 02:19:56.000000 AnimeCrawler-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 03:36:47.215752 AnimeCrawler-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-05-03 03:31:04.000000 AnimeCrawler-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.544256 AnimeCrawler-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.153479 AnimeCrawler-0.2.0/AnimeCrawler/
+-rw-rw-rw-   0        0        0      388 2023-05-06 14:06:08.000000 AnimeCrawler-0.2.0/AnimeCrawler/__init__.py
+-rw-rw-rw-   0        0        0     2682 2023-05-06 13:57:08.000000 AnimeCrawler-0.2.0/AnimeCrawler/base_spider.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.392346 AnimeCrawler-0.2.0/AnimeCrawler/command/
+-rw-rw-rw-   0        0        0      117 2023-05-03 05:18:04.000000 AnimeCrawler-0.2.0/AnimeCrawler/command/__init__.py
+-rw-rw-rw-   0        0        0     3250 2023-05-06 14:05:51.000000 AnimeCrawler-0.2.0/AnimeCrawler/command/run.py
+-rw-rw-rw-   0        0        0      356 2023-05-03 05:07:40.000000 AnimeCrawler-0.2.0/AnimeCrawler/log.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.493285 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/
+-rw-rw-rw-   0        0        0      286 2023-05-03 09:50:27.000000 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/__init__.py
+-rw-rw-rw-   0        0        0     2396 2023-05-06 13:55:26.000000 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/downloader.py
+-rw-rw-rw-   0        0        0     2084 2023-05-06 13:51:37.000000 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/searcher.py
+-rw-rw-rw-   0        0        0     4138 2023-05-06 13:58:10.000000 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/spider.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.499281 AnimeCrawler-0.2.0/AnimeCrawler/utils/
+-rw-rw-rw-   0        0        0      128 2023-05-03 15:03:17.000000 AnimeCrawler-0.2.0/AnimeCrawler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-05-03 02:47:10.000000 AnimeCrawler-0.2.0/AnimeCrawler/utils/decode.py
+-rw-rw-rw-   0        0        0     3017 2023-05-03 15:13:47.000000 AnimeCrawler-0.2.0/AnimeCrawler/utils/file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.348369 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/
+-rw-rw-rw-   0        0        0     3268 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3268 2023-05-06 14:39:52.505278 AnimeCrawler-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2819 2023-05-06 14:03:37.000000 AnimeCrawler-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 14:39:52.545255 AnimeCrawler-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      882 2023-05-06 14:21:26.000000 AnimeCrawler-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.503279 AnimeCrawler-0.2.0/test/
+-rw-rw-rw-   0        0        0      264 2023-05-03 13:36:29.000000 AnimeCrawler-0.2.0/test/test.py
```

### Comparing `AnimeCrawler-0.1.2/AnimeCrawler/base_spider.py` & `AnimeCrawler-0.2.0/AnimeCrawler/base_spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 import urllib.parse
 
-from ruia import Spider
+from ruia import Request, Spider
 
 from AnimeCrawler.log import get_logger
 from AnimeCrawler.utils import is_url
 
 
 class BaseSpider(Spider):
+    '''所有爬虫的基类，必须提供domain与downloader属性
+
+    Args:
+        Spider (ruia.Spider): 继承于ruia框架的爬虫
+
+    Raises:
+        ValueError: 未定义domain时报错
+        ValueError: 未定义downloader时报错
+
+    Returns:
+        cls: 为了链式调用ruia.Spider.start()
+    '''
+
     logger = get_logger('Spider')
 
+    def __init__(self, *args, **spider_kwargs) -> None:
+        super().__init__(*args, **spider_kwargs)
+        if not hasattr(self, 'domain'):
+            raise ValueError(f'{self.__class__.__name__} 未定义domain属性')
+        elif not hasattr(self, 'downloader'):
+            raise ValueError(f'{self.__class__.__name__} 未定义downloader下载器')
+
     @classmethod
     def init(cls):
-        if not hasattr(cls, 'domain'):
-            raise ValueError(f'{cls.__name__} 未定义domain属性')
-        if not hasattr(cls, 'downloader'):
-            raise ValueError(f'{cls.__name__} 未定义downloader下载器')
         cls.start_urls = [
             i if is_url(i) else urllib.parse.urljoin(cls.domain, i)
             for i in cls.start_urls
         ]  # 当url为相对路径时与域名拼接
         return cls
 
-    async def urljoin(self, base, url, avoid_collision: bool = False) -> str:
-        '''对urllib.parse.urljoin()的异步包装
+    def urljoin(self, base, url, avoid_collision: bool = False) -> str:
+        '''对urllib.parse.urljoin()的包装
 
         Args:
             base (str): 基础url
             url (str): 要拼接的url
             avoid_collision (bool, optional): 避免冲突，
 
             详情看：https://docs.python.org/zh-cn/3/library/urllib.parse.html#urllib.parse.urljoin
@@ -37,31 +53,31 @@
             str: 拼接后的url
         '''
         if avoid_collision:
             url_parts = urllib.parse.urlsplit(url)
             url = urllib.parse.urlunsplit(url_parts._replace(scheme='', netloc=''))
         return urllib.parse.urljoin(base, url)
 
-    async def follow(self, next_url: str = None, **kwargs):
+    async def follow(self, next_url: str = None, **kwargs) -> Request:
         '''爬取下一个页面
 
         Args:
             next_url (str, optional): 下一个url的相对路径. Defaults to None.
 
         Returns:
             ruia.Request: 可被yield
         '''
-        return self.request(await self.urljoin(self.domain, next_url), **kwargs)
+        return self.request(self.urljoin(self.domain, next_url), **kwargs)
 
-    def get_domain(self, url: str):
+    def get_domain(self, url: str) -> str:
         url_parts = urllib.parse.urlsplit(url)
         print(url)
         return '://'.join(url_parts[:2])  # e.g. https://docs.python.org/
 
-    def get_path(self, url: str):
+    def get_path(self, url: str) -> str:
         url_parts = urllib.parse.urlsplit(url)
         return url_parts.path
 
 
 if __name__ == '__main__':
     BaseSpider().get_domain(
         'https://docs.python.org/zh-cn/3/library/urllib.parse.html#urllib.parse.urljoin'
```

### Comparing `AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/downloader.py` & `AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import asyncio
+from typing import Any, Union
 
 import aiohttp
 import tqdm.asyncio
 
 from AnimeCrawler.log import get_logger
 from AnimeCrawler.utils import write
 
 
 class Downloader:
     session = None
     logger = get_logger('Downloader')
 
     @property
-    def current_session(self):
+    def current_session(self) -> aiohttp.ClientSession:
         if not self.session:
             self.session = aiohttp.ClientSession(
-                connector = aiohttp.TCPConnector(verify_ssl=False)
+                connector=aiohttp.TCPConnector(verify_ssl=False)
             )
             self.logger.debug('创建了session')
         return self.session
 
     @property
-    def set_url(self, urls):
+    def set_url(self, urls) -> str:
         return urls
 
     @set_url.setter
-    def set_url(self, urls):
+    def set_url(self, urls) -> None:
         self.urls = urls
 
-    async def close_session(self):
+    async def close_session(self) -> None:
         await self.current_session.close()
 
     async def get_ts_file(
         self,
         session: aiohttp.ClientSession,
         title: str,
         url: str,
         error_times: int = 1,
-    ):
+    ) -> Union[tuple[bytes, str], Any]:
         resp = await session.get(
             url=url,
             headers={'User-Agent': 'Mozilla/5.0', ' Transfer-Encoding': 'chunked'},
         )
         try:
             text = await resp.content.read()
             await asyncio.sleep(0)
```

### Comparing `AnimeCrawler-0.1.2/AnimeCrawler/mhyyy/spider.py` & `AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from pathlib import Path
+from typing import AsyncGenerator
 
-from ruia import Item, Response, TextField
+from ruia import Item, Request, Response, TextField
 
 from AnimeCrawler.base_spider import BaseSpider
-from AnimeCrawler.log import get_logger
 from AnimeCrawler.utils import (
     base64_decode,
     folder_path,
     get_video_path,
     merge_ts2mp4,
     unescape,
     write,
@@ -26,17 +26,18 @@
 
 
 class AnimeSpider(BaseSpider):
     _base_ts_url = None
     _mixed_m3u8 = None
     downloader = Downloader()
     headers = {'User-Agent': 'Mozilla/5.0'}
+    concurrency: int = 5
 
     @classmethod
-    def init(cls, anime_title: str, urls: str, del_ts: bool = False):
+    def init(cls, anime_title: str, urls: str, del_ts: bool = False) -> BaseSpider:
         '''初始化爬虫
 
         Args:
             anime_title (str): 动漫标题，用于取文件夹的名称，利于管理动漫
             urls (str): 第一页的网址
 
         Returns:
@@ -49,38 +50,40 @@
         return super().init()
 
     async def _mixed_m3u8_url_parse(self, index_m3u8_url: str, item: AnimeItem) -> None:
         resp = await self.request(index_m3u8_url).fetch()
         text = await resp.text()
         if self._mixed_m3u8 is None:
             self._mixed_m3u8 = text.split('\n')[-1]
-        item.mixed_m3u8_url = await self.urljoin(item._base_m3u8_url, self._mixed_m3u8)
+        item.mixed_m3u8_url = self.urljoin(item._base_m3u8_url, self._mixed_m3u8)
 
     def _parse_mixed_m3u8(self, item: AnimeItem):
         '''解析mixed.m3u8文件，获得ts文件下载地址
 
         Returns:
             str：ts_url
         '''
         base_ts_file = item.mixed_m3u8_url[:-10]
         with open(self.PATH / f'{item.episodes}\\mixed.m3u8', 'r') as fp:
             for i in fp:
                 if '#' not in i:
                     yield base_ts_file + i
 
-    async def have_next_page(self, link_next: str):
+    async def have_next_page(self, link_next: str) -> Request:
         # 当有下一页时
         link_next = link_next.replace('\\', '')
         return await self.follow(
-            await self.urljoin(self.domain, link_next),
+            link_next,
             callback=self.parse,
             headers=self.headers,
         )
 
-    async def parse(self, response: Response):
+    async def parse(
+        self, response: Response
+    ) -> AsyncGenerator[Request | AnimeItem, None]:
         async for item in AnimeItem.get_items(html=await response.text()):
             profile = item.profile
             player_aaaa = eval(re.search('{.*}', profile).group())
             item.episodes = re.findall('\d+', response.url)[2]
             encoded_url = player_aaaa['url']
             index_m3u8_url = unescape(
                 base64_decode(encoded_url)
@@ -89,27 +92,23 @@
             await self._mixed_m3u8_url_parse(index_m3u8_url, item)
 
             link_next = player_aaaa.get('link_next', None)
             if link_next:
                 yield await self.have_next_page(link_next)
             yield item
 
-    async def process_item(self, item: AnimeItem):
+    async def process_item(self, item: AnimeItem) -> None:
         resp = await self.request(item.mixed_m3u8_url, headers=self.headers).fetch()
         text = await resp.text()
         episodes = item.episodes
         folder_path = self.PATH / f'{episodes}'
         self.logger.info('\033[0;32;40m写入mixed.m3u8\033[0m')
         await write(folder_path, text, 'mixed', 'm3u8', 'w+')
         urls = self._parse_mixed_m3u8(item)
         self.downloader.set_url = urls
         await self.downloader.download_ts_files(folder_path, episodes)
         self.logger.info(f"正在把第 {episodes} 集的ts文件转码成 mp4")
         await merge_ts2mp4(folder_path, episodes, self.del_ts)
 
-    async def stop(self, _signal):
+    async def stop(self, _signal) -> None:
         await self.downloader.close_session()
         return await super().stop(_signal)
-
-
-if __name__ == '__main__':
-    AnimeSpider.init('魔女之旅', ['https://www.mhyyy.com/play/166269-1-1.html']).start()
```

### Comparing `AnimeCrawler-0.1.2/AnimeCrawler/utils/decode.py` & `AnimeCrawler-0.2.0/AnimeCrawler/utils/decode.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.1.2/AnimeCrawler.egg-info/PKG-INFO` & `AnimeCrawler-0.2.0/AnimeCrawler.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.1.2
+Version: 0.2.0
 Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,16 +27,16 @@
 
 
 这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
-3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
-4. 最后，打开命令提示符，输入 <code>AnimeCrawler download -t "动漫名称" -u "url"</code> 回车就可以下载啦
+3. 其次，输入 <code>AnimeCrawler search -t "动漫标题"</code>，来搜索动漫
+4. 最后，复制输出的下载命令，粘贴回车就可以下载啦
     - 输入 <code>AnimeCrawler -h</code> 会有详细的说明
 > 下载后的文件在您的视频文件夹里
 
 如果您想体验最新的功能，请转到dev分支~
 
 ## 🚀我想帮忙
 十分感谢您有这个想法。这个项目仍在青涩年华，总会有一些跌跌撞撞的时候，也许您的举手之劳，能造就更好的它
@@ -53,15 +53,15 @@
 - [ ] 可更换下载源
 - [ ] 支持上传网盘
 - [ ] <span style="text-decoration: line-through">甚至是GUI</span>
 
 ## 🧱从源码搭建
 1. 点击[这里](https://github.com/Senvlin/AnimeCrawler/releases)找到最新版本，下载源码
 2. 转到项目目录，使用 <code>pip install -r requirement.txt</code> 安装依赖库
-3. 随后使用 <code>python -m AnimeCrawler "动漫名称" "url"</code> 或打开 <code>AnimeCrawler\mhyyy\spider.py</code>运行即可
+3. 随后使用 <code>python -m AnimeCrawler download -t "动漫标题" -u "URL"</code> 运行即可
 
 ## ❗ 声明
 此项目只因个人兴趣而开发，仅供学习交流使用，无任何商业用途
 
 下载的资源均来自可搜索到的、各网站提供的公开引用资源，所有视频版权均归原作者及网站所有
 
 您应该自行承担使用此项目有可能的风险，我不保证您下载的资源的安全性，合法性，公正性。网络信息良莠不齐，请自行甄别，谢谢
```

### Comparing `AnimeCrawler-0.1.2/AnimeCrawler.egg-info/SOURCES.txt` & `AnimeCrawler-0.2.0/AnimeCrawler.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 LICENSE
 README.md
 setup.py
 AnimeCrawler/__init__.py
-AnimeCrawler/__main__.py
 AnimeCrawler/base_spider.py
 AnimeCrawler/log.py
 AnimeCrawler.egg-info/PKG-INFO
 AnimeCrawler.egg-info/SOURCES.txt
 AnimeCrawler.egg-info/dependency_links.txt
 AnimeCrawler.egg-info/entry_points.txt
 AnimeCrawler.egg-info/requires.txt
 AnimeCrawler.egg-info/top_level.txt
 AnimeCrawler/command/__init__.py
 AnimeCrawler/command/run.py
 AnimeCrawler/mhyyy/__init__.py
 AnimeCrawler/mhyyy/downloader.py
+AnimeCrawler/mhyyy/searcher.py
 AnimeCrawler/mhyyy/spider.py
 AnimeCrawler/utils/__init__.py
 AnimeCrawler/utils/decode.py
-AnimeCrawler/utils/file.py
+AnimeCrawler/utils/file.py
+test/test.py
```

### Comparing `AnimeCrawler-0.1.2/LICENSE` & `AnimeCrawler-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.1.2/PKG-INFO` & `AnimeCrawler-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.1.2
+Version: 0.2.0
 Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,16 +27,16 @@
 
 
 这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
-3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
-4. 最后，打开命令提示符，输入 <code>AnimeCrawler download -t "动漫名称" -u "url"</code> 回车就可以下载啦
+3. 其次，输入 <code>AnimeCrawler search -t "动漫标题"</code>，来搜索动漫
+4. 最后，复制输出的下载命令，粘贴回车就可以下载啦
     - 输入 <code>AnimeCrawler -h</code> 会有详细的说明
 > 下载后的文件在您的视频文件夹里
 
 如果您想体验最新的功能，请转到dev分支~
 
 ## 🚀我想帮忙
 十分感谢您有这个想法。这个项目仍在青涩年华，总会有一些跌跌撞撞的时候，也许您的举手之劳，能造就更好的它
@@ -53,15 +53,15 @@
 - [ ] 可更换下载源
 - [ ] 支持上传网盘
 - [ ] <span style="text-decoration: line-through">甚至是GUI</span>
 
 ## 🧱从源码搭建
 1. 点击[这里](https://github.com/Senvlin/AnimeCrawler/releases)找到最新版本，下载源码
 2. 转到项目目录，使用 <code>pip install -r requirement.txt</code> 安装依赖库
-3. 随后使用 <code>python -m AnimeCrawler "动漫名称" "url"</code> 或打开 <code>AnimeCrawler\mhyyy\spider.py</code>运行即可
+3. 随后使用 <code>python -m AnimeCrawler download -t "动漫标题" -u "URL"</code> 运行即可
 
 ## ❗ 声明
 此项目只因个人兴趣而开发，仅供学习交流使用，无任何商业用途
 
 下载的资源均来自可搜索到的、各网站提供的公开引用资源，所有视频版权均归原作者及网站所有
 
 您应该自行承担使用此项目有可能的风险，我不保证您下载的资源的安全性，合法性，公正性。网络信息良莠不齐，请自行甄别，谢谢
```

### Comparing `AnimeCrawler-0.1.2/README.md` & `AnimeCrawler-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
 这是一款在Windows平台下基于轻量级框架<code>[**Ruia**](https://github.com/howie6879/ruia)</code>、专门爬取免费动漫的爬虫，底层使用<code>aiohttp</code>库，使用异步模式，大幅增加爬取及下载速度。可**离线播放**各大动漫，支持**命令行输入**，立志成为最实用，最轻量的动漫管理及下载助手
 
 ## ❓如何使用
 1. 首先来到[这里](https://www.python.org/downloads)下载Python解释器, 要求Python3.8及以上版本，安装即可
 2. 然后，打开命令提示符，输入 <code>pip install AnimeCrawler</code>
-3. 其次，来到[这个网站](https://www.mhyyy.com/),搜索您喜欢的动漫，点击播放页，将第一页的url复制一下
-4. 最后，打开命令提示符，输入 <code>AnimeCrawler download -t "动漫名称" -u "url"</code> 回车就可以下载啦
+3. 其次，输入 <code>AnimeCrawler search -t "动漫标题"</code>，来搜索动漫
+4. 最后，复制输出的下载命令，粘贴回车就可以下载啦
     - 输入 <code>AnimeCrawler -h</code> 会有详细的说明
 > 下载后的文件在您的视频文件夹里
 
 如果您想体验最新的功能，请转到dev分支~
 
 ## 🚀我想帮忙
 十分感谢您有这个想法。这个项目仍在青涩年华，总会有一些跌跌撞撞的时候，也许您的举手之劳，能造就更好的它
@@ -39,15 +39,15 @@
 - [ ] 可更换下载源
 - [ ] 支持上传网盘
 - [ ] <span style="text-decoration: line-through">甚至是GUI</span>
 
 ## 🧱从源码搭建
 1. 点击[这里](https://github.com/Senvlin/AnimeCrawler/releases)找到最新版本，下载源码
 2. 转到项目目录，使用 <code>pip install -r requirement.txt</code> 安装依赖库
-3. 随后使用 <code>python -m AnimeCrawler "动漫名称" "url"</code> 或打开 <code>AnimeCrawler\mhyyy\spider.py</code>运行即可
+3. 随后使用 <code>python -m AnimeCrawler download -t "动漫标题" -u "URL"</code> 运行即可
 
 ## ❗ 声明
 此项目只因个人兴趣而开发，仅供学习交流使用，无任何商业用途
 
 下载的资源均来自可搜索到的、各网站提供的公开引用资源，所有视频版权均归原作者及网站所有
 
 您应该自行承担使用此项目有可能的风险，我不保证您下载的资源的安全性，合法性，公正性。网络信息良莠不齐，请自行甄别，谢谢
```

### Comparing `AnimeCrawler-0.1.2/setup.py` & `AnimeCrawler-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AnimeCrawler",
-    version="v0.1.2",
+    version="v0.2.0",
     author="Senvlin",
     author_email="2994515402@qq.com",
     description="一个可免费下载动漫的爬虫",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Senvlin/AnimeCrawler",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=['ruia', 'tqdm', 'aiofiles', 'aiohttp'],
+    install_requires=['ruia', 'tqdm', 'aiofiles', 'wheel'],
     entry_points={
         'console_scripts': [
             'animecrawler = AnimeCrawler.command.run:main',
         ],
     },
     python_requires='>=3.8',
 )
```

