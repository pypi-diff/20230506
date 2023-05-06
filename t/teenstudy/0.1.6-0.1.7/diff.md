# Comparing `tmp/TeenStudy-0.1.6.tar.gz` & `tmp/TeenStudy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TeenStudy-0.1.6.tar", max compression
+gzip compressed data, was "TeenStudy-0.1.7.tar", max compression
```

## Comparing `TeenStudy-0.1.6.tar` & `TeenStudy-0.1.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1084 2023-03-01 02:44:19.173074 TeenStudy-0.1.6/LICENSE
--rw-r--r--   0        0        0      956 2023-04-12 08:07:28.967372 TeenStudy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     9823 2023-04-12 16:15:14.951000 TeenStudy-0.1.6/README.md
--rw-r--r--   0        0        0      673 2023-04-11 07:54:00.639322 TeenStudy-0.1.6/TeenStudy/__init__.py
--rw-r--r--   0        0        0       28 2023-02-20 07:31:58.077384 TeenStudy-0.1.6/TeenStudy/models/__init__.py
--rw-r--r--   0        0        0     3547 2023-04-11 15:19:07.641068 TeenStudy-0.1.6/TeenStudy/models/accuont.py
--rw-r--r--   0        0        0     3621 2023-02-26 10:27:44.170299 TeenStudy-0.1.6/TeenStudy/models/dxx.py
--rw-r--r--   0        0        0   881164 2022-04-16 12:05:27.915000 TeenStudy-0.1.6/TeenStudy/resource/answer.png
--rw-r--r--   0        0        0    52240 2022-06-07 16:13:22.153835 TeenStudy-0.1.6/TeenStudy/resource/backgroud1.jpg
--rw-r--r--   0        0        0    52119 2022-06-07 16:14:57.998789 TeenStudy-0.1.6/TeenStudy/resource/backgroud2.jpg
--rw-r--r--   0        0        0    52136 2022-06-07 16:15:11.806076 TeenStudy-0.1.6/TeenStudy/resource/backgroud3.jpg
--rw-r--r--   0        0        0    51874 2022-06-07 16:15:26.111059 TeenStudy-0.1.6/TeenStudy/resource/backgroud4.jpg
--rw-r--r--   0        0        0    51634 2022-06-07 16:15:39.887415 TeenStudy-0.1.6/TeenStudy/resource/backgroud5.jpg
--rw-r--r--   0        0        0 10424793 2023-04-12 08:29:49.497783 TeenStudy-0.1.6/TeenStudy/resource/dxx_jx.json
--rw-r--r--   0        0        0  7977480 2021-12-28 14:26:48.000000 TeenStudy-0.1.6/TeenStudy/resource/MiSans-Light.ttf
--rw-r--r--   0        0        0      121 2023-02-24 03:04:11.263388 TeenStudy-0.1.6/TeenStudy/utils/__init__.py
--rw-r--r--   0        0        0    38117 2023-04-12 04:25:01.681311 TeenStudy-0.1.6/TeenStudy/utils/dxx.py
--rw-r--r--   0        0        0    16706 2023-04-12 12:02:23.220059 TeenStudy-0.1.6/TeenStudy/utils/handle.py
--rw-r--r--   0        0        0     4016 2023-04-12 03:59:28.480060 TeenStudy-0.1.6/TeenStudy/utils/path.py
--rw-r--r--   0        0        0     2026 2023-03-17 16:29:23.697778 TeenStudy-0.1.6/TeenStudy/utils/rule.py
--rw-r--r--   0        0        0     9955 2023-04-11 15:38:04.186097 TeenStudy-0.1.6/TeenStudy/utils/update.py
--rw-r--r--   0        0        0    22347 2023-04-12 08:03:26.130929 TeenStudy-0.1.6/TeenStudy/utils/utils.py
--rw-r--r--   0        0        0     2185 2023-03-26 15:43:16.603440 TeenStudy-0.1.6/TeenStudy/web/__init__.py
--rw-r--r--   0        0        0      396 2023-03-01 05:03:46.707234 TeenStudy-0.1.6/TeenStudy/web/api/__init__.py
--rw-r--r--   0        0        0    30192 2023-04-12 05:27:59.958362 TeenStudy-0.1.6/TeenStudy/web/api/add.py
--rw-r--r--   0        0        0    11925 2023-04-12 07:34:22.146364 TeenStudy-0.1.6/TeenStudy/web/api/admin.py
--rw-r--r--   0        0        0     4706 2023-04-11 17:08:12.501307 TeenStudy-0.1.6/TeenStudy/web/api/home.py
--rw-r--r--   0        0        0     6283 2023-04-11 15:43:45.703050 TeenStudy-0.1.6/TeenStudy/web/api/login.py
--rw-r--r--   0        0        0       78 2023-03-01 04:59:13.766339 TeenStudy-0.1.6/TeenStudy/web/pages/__init__.py
--rw-r--r--   0        0        0    31191 2023-04-12 05:35:18.255316 TeenStudy-0.1.6/TeenStudy/web/pages/add.py
--rw-r--r--   0        0        0    63945 2023-04-12 07:46:44.160244 TeenStudy-0.1.6/TeenStudy/web/pages/admin.py
--rw-r--r--   0        0        0    17471 2023-04-12 03:54:19.788655 TeenStudy-0.1.6/TeenStudy/web/pages/home.py
--rw-r--r--   0        0        0     1731 2023-03-13 04:39:00.485882 TeenStudy-0.1.6/TeenStudy/web/pages/login.py
--rw-r--r--   0        0        0       24 2023-03-18 03:06:10.438593 TeenStudy-0.1.6/TeenStudy/web/utils/__init__.py
--rw-r--r--   0        0        0     1902 2023-02-25 14:14:03.511258 TeenStudy-0.1.6/TeenStudy/web/utils/add.py
--rw-r--r--   0        0        0     2240 2023-04-11 15:39:50.989195 TeenStudy-0.1.6/TeenStudy/web/utils/status.py
--rw-r--r--   0        0        0    11285 1970-01-01 00:00:00.000000 TeenStudy-0.1.6/setup.py
--rw-r--r--   0        0        0    11061 1970-01-01 00:00:00.000000 TeenStudy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-06 04:08:57.731309 TeenStudy-0.1.7/LICENSE
+-rw-r--r--   0        0        0      955 2023-05-06 09:11:05.637704 TeenStudy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9960 2023-05-06 08:45:54.744774 TeenStudy-0.1.7/README.md
+-rw-r--r--   0        0        0      666 2023-05-06 04:16:34.547526 TeenStudy-0.1.7/TeenStudy/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-06 04:08:57.732319 TeenStudy-0.1.7/TeenStudy/models/__init__.py
+-rw-r--r--   0        0        0     3547 2023-05-06 04:08:57.733777 TeenStudy-0.1.7/TeenStudy/models/accuont.py
+-rw-r--r--   0        0        0     3621 2023-05-06 04:08:57.733777 TeenStudy-0.1.7/TeenStudy/models/dxx.py
+-rw-r--r--   0        0        0   881164 2023-05-06 04:08:57.790011 TeenStudy-0.1.7/TeenStudy/resource/answer.png
+-rw-r--r--   0        0        0    52240 2023-05-06 04:08:57.791011 TeenStudy-0.1.7/TeenStudy/resource/backgroud1.jpg
+-rw-r--r--   0        0        0    52119 2023-05-06 04:08:57.792437 TeenStudy-0.1.7/TeenStudy/resource/backgroud2.jpg
+-rw-r--r--   0        0        0    52136 2023-05-06 04:08:57.792437 TeenStudy-0.1.7/TeenStudy/resource/backgroud3.jpg
+-rw-r--r--   0        0        0    51874 2023-05-06 04:08:57.793437 TeenStudy-0.1.7/TeenStudy/resource/backgroud4.jpg
+-rw-r--r--   0        0        0    51634 2023-05-06 04:08:57.793437 TeenStudy-0.1.7/TeenStudy/resource/backgroud5.jpg
+-rw-r--r--   0        0        0 10424793 2023-05-06 04:08:57.825443 TeenStudy-0.1.7/TeenStudy/resource/dxx_jx.json
+-rw-r--r--   0        0        0  7977480 2023-05-06 04:08:57.787010 TeenStudy-0.1.7/TeenStudy/resource/MiSans-Light.ttf
+-rw-r--r--   0        0        0      121 2023-05-06 04:08:57.826444 TeenStudy-0.1.7/TeenStudy/utils/__init__.py
+-rw-r--r--   0        0        0    41094 2023-05-06 08:22:07.953021 TeenStudy-0.1.7/TeenStudy/utils/dxx.py
+-rw-r--r--   0        0        0    18819 2023-05-06 06:32:36.543523 TeenStudy-0.1.7/TeenStudy/utils/handle.py
+-rw-r--r--   0        0        0     4331 2023-05-06 08:28:06.723801 TeenStudy-0.1.7/TeenStudy/utils/path.py
+-rw-r--r--   0        0        0     2026 2023-05-06 04:08:57.828444 TeenStudy-0.1.7/TeenStudy/utils/rule.py
+-rw-r--r--   0        0        0    10411 2023-05-06 06:39:01.954182 TeenStudy-0.1.7/TeenStudy/utils/update.py
+-rw-r--r--   0        0        0    23399 2023-05-06 08:27:27.912843 TeenStudy-0.1.7/TeenStudy/utils/utils.py
+-rw-r--r--   0        0        0     2185 2023-05-06 04:08:57.830444 TeenStudy-0.1.7/TeenStudy/web/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-06 04:08:57.830444 TeenStudy-0.1.7/TeenStudy/web/api/__init__.py
+-rw-r--r--   0        0        0    33714 2023-05-06 08:09:01.153218 TeenStudy-0.1.7/TeenStudy/web/api/add.py
+-rw-r--r--   0        0        0    11925 2023-05-06 04:08:57.831445 TeenStudy-0.1.7/TeenStudy/web/api/admin.py
+-rw-r--r--   0        0        0     4706 2023-05-06 04:08:57.831947 TeenStudy-0.1.7/TeenStudy/web/api/home.py
+-rw-r--r--   0        0        0     6317 2023-05-06 04:13:39.518045 TeenStudy-0.1.7/TeenStudy/web/api/login.py
+-rw-r--r--   0        0        0       78 2023-05-06 04:08:57.832963 TeenStudy-0.1.7/TeenStudy/web/pages/__init__.py
+-rw-r--r--   0        0        0    33787 2023-05-06 07:57:07.633870 TeenStudy-0.1.7/TeenStudy/web/pages/add.py
+-rw-r--r--   0        0        0    67310 2023-05-06 08:27:27.918859 TeenStudy-0.1.7/TeenStudy/web/pages/admin.py
+-rw-r--r--   0        0        0    17385 2023-05-06 06:46:36.426467 TeenStudy-0.1.7/TeenStudy/web/pages/home.py
+-rw-r--r--   0        0        0     1731 2023-05-06 04:08:57.834965 TeenStudy-0.1.7/TeenStudy/web/pages/login.py
+-rw-r--r--   0        0        0       24 2023-05-06 04:08:57.834965 TeenStudy-0.1.7/TeenStudy/web/utils/__init__.py
+-rw-r--r--   0        0        0     1902 2023-05-06 04:08:57.835965 TeenStudy-0.1.7/TeenStudy/web/utils/add.py
+-rw-r--r--   0        0        0     2240 2023-05-06 04:08:57.835965 TeenStudy-0.1.7/TeenStudy/web/utils/status.py
+-rw-r--r--   0        0        0    11422 1970-01-01 00:00:00.000000 TeenStudy-0.1.7/setup.py
+-rw-r--r--   0        0        0    11188 1970-01-01 00:00:00.000000 TeenStudy-0.1.7/PKG-INFO
```

### Comparing `TeenStudy-0.1.6/LICENSE` & `TeenStudy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/pyproject.toml` & `TeenStudy-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "TeenStudy"
-version = "0.1.6"
+version = "0.1.7"
 description = "基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图"
 authors = ["ZM25XC <xingling25@qq.com>"]
 license="MIT"
 readme="README.md"
 homepage="https://github.com/ZM25XC/TeenStudy"
 [tool.poetry.dependencies]
 python = "^3.8"
-amis-python="^1.0.6"
+amis-python="^1.0.7"
 anti-useragent="^1.0.10"
 beautifulsoup4="^4.11.2"
 bs4="^0.0.1"
 fastapi="^0.95.0,<1.0.0"
 httpx="^0.23.3,<1.0.0"
 Jinja2="^3.1.2"
 lxml="^4.9.2"
 nonebot-adapter-onebot="^2.2.1"
 nonebot-plugin-apscheduler="^0.2.0"
 nonebot2="^2.0.0rc2"
 Pillow="^9.4.0"
 python-jose="^3.3.0"
 tortoise-orm="^0.19.3"
 ujson="^5.7.0"
-uvicorn="^0.20.0,<0.50.0"
+uvicorn="^0.21.0,<1.0.0"
 qrcode="^7.4.2"
 psutil="^5.9.4"
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `TeenStudy-0.1.6/README.md` & `TeenStudy-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 <div align="center">
     <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
     <h1>TeenStudy</h1>
-    <b>基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
+    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
     <br/>
     <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>
   	<a href="https://pypi.python.org/pypi/TeenStudy">
     <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>
-     <a href="https://github.com/ZM25XC/TeenStudy">
-    <img src="https://visitor-badge.glitch.me/badge?page_id=https://github.com/ZM25XC/TeenStudy" alt="Teenstudy"></a>
-	<a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
+	  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">
     <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">
   </a>
   </div>
 
 ## 说明
 
@@ -33,32 +31,32 @@
 
 <details>
 
 | 共青团名称 | 开发状态 | 备注 |
 |:-----:|:----:|:----:|
 |青春湖北|支持|无需抓包|
 |江西共青团|支持|无需抓包|
+|安徽共青团|支持|无需抓包|
 |青春上海|支持|微信扫码绑定|
 |青春浙江|支持|微信扫码绑定|
-|安徽共青团|支持|无需抓包|
 |江苏共青团|支持|需要自行抓包|
 |青春山东|支持|需要自行抓包|
 |重庆共青团|支持|需要自行抓包|
-|河南共青团|不支持|cookie时效小于1周|
+|吉青飞扬|支持|需要自行抓包|
 |天府新青年|支持|不进入公众号token时效大于1周|
+|河南共青团|不支持|cookie时效小于1周|
 |黑龙江共青团|待开发||
 |广西青年圈|待开发||
 |青春湖南|待开发||
 |甘肃青年|待开发||
 |山西青年|待开发||
 |河北共青团|待开发||
 |福建共青团|待开发||
 |内蒙古青年|待开发||
 |云南共青团|待开发||
-|吉青飞扬|待开发||
 |三秦青年|待开发||
 |青春北京|待开发||
 |海南共青团|待开发||
 |津彩青春|待开发||
 |青春黔言|待开发||
 |广东共青团|待开发||
 |青春柳州|待开发||
@@ -157,28 +155,39 @@
 
 - [ ] 增加更多地区支持
 - [ ] 优化 Bot
 
 
 ## 更新日志
 
-###2023/04/12
+### 2023/05/06
+
+- 增加吉林地区，需要自行抓包
+- 修复超管更改登录密码后用原密码能继续登录问题
+- 添加二维码转链接开关，需要自行在后台配置页面打开
+- 调整部分依赖
+
+
+<details>
+<summary> 2023/04/12</summary> 
+
 - 因河南地区cookie时效小于1周，移除河南地区
 - 添加`删除大学习`功能，用户可自行删除数据
 - 添加`导出用户数据`功能
 - 添加`更新用户数据`功能
 - 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据
 - 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改
 - 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改
 - 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改
 - 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法
 - 修复Web UI 首页公网IP显示异常
 - 修复浙江地区用户重复显示
 - 更新江西共青团团支部数据
-
+  
+</details>
 
 
 <details>
 <summary>2023/03/18</summary>
 
 - 适配河南地区，需要自行抓包
 - 适配四川地区，需要自行抓包
@@ -211,8 +220,8 @@
 <summary>2023/03/01</summary>
 
 - 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件
 - 上传基础代码
 - 适配湖北地区，无需抓包，安装即用
 - 适配江西地区，无需抓包，安装即用
 
-</details>
+</details>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
                                 [TeenStudy.png]
                             ****** TeenStudy ******
-åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
+                             åºäºnonebot2ågo-
+cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 
-     [GitHub_issues] [GitHub_forks] [GitHub_stars] [pypi] [pypi_download]
-                 [Teenstudy] [GitHub_license] [QQ_Chat_Group]
+ [GitHub_issues] [GitHub_forks] [GitHub_stars] [pypi] [pypi_download] [GitHub
+                           license] [QQ_Chat_Group]
 ## è¯´æ - æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/ZM25XC/
 nonebot_plugin_auto_teenstudy) `Web UI`ç - æ¬é¡¹ç®åºäº[nonebot2](https://
 github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£ -
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**
 -
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤
@@ -15,26 +16,27 @@
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸
 - æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã
 -
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯
 - è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars. ## å°åºç¶æ  | å±éå¢åç§° |
 å¼åç¶æ | å¤æ³¨ | |:-----:|:----:|:----:
 | |éæ¥æ¹å|æ¯æ|æ éæå| |æ±è¥¿å±éå¢|æ¯æ|æ éæå|
-|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
-|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®| |å®å¾½å±éå¢|æ¯æ|æ éæå|
+|å®å¾½å±éå¢|æ¯æ|æ éæå| |éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|
 |éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|
 |éåºå±éå¢|æ¯æ|éè¦èªè¡æå|
-|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
+|åéé£æ¬|æ¯æ|éè¦èªè¡æå|
 |å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|
+|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
 |é»é¾æ±å±éå¢|å¾å¼å|| |å¹¿è¥¿éå¹´å|å¾å¼å||
 |éæ¥æ¹å|å¾å¼å|| |çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
 |æ²³åå±éå¢|å¾å¼å|| |ç¦å»ºå±éå¢|å¾å¼å||
 |åèå¤éå¹´|å¾å¼å|| |äºåå±éå¢|å¾å¼å||
-|åéé£æ¬|å¾å¼å|| |ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
+|ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
 |æµ·åå±éå¢|å¾å¼å|| |æ´¥å½©éæ¥|å¾å¼å||
 |éæ¥é»è¨|å¾å¼å|| |å¹¿ä¸å±éå¢|å¾å¼å||
 |éæ¥æ³å·|å¾å¼å|| |è¾½å®å±éå¢|å¾å¼å||
 |å®å¤å±éå¢|å¾å¼å|| |æ°çå±éå¢|å¾å¼å||
 |è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°  ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) -
 ä½¿ç¨`git clone https://github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶   ç¬¬äºç§æ¹å¼
@@ -71,16 +73,20 @@
 | | éç½®éç½® | éç½®éç½®ãå·æ°éç½® | è¶ç®¡å¯ç¨ï¼å·æ°Web
 UIé»è®¤éç½® | | éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID |
 |å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|
 |å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|
 |æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|
 |æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|
-## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿
-###2023/04/12 - å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
+## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿ ###
+2023/05/06 - å¢å åæå°åºï¼éè¦èªè¡æå -
+ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢ -
+æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼ -
+è°æ´é¨åä¾èµ   2023/04/12 -
+å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ® -
 æ·»å `å¯¼åºç¨æ·æ°æ®`åè½ - æ·»å `æ´æ°ç¨æ·æ°æ®`åè½ -
 æ·»å `æ´æ°èµæºæ°æ®`åè½ï¼æ±è¥¿å°åºæ´æ°åè¯·ä½¿ç¨ä¸æ­¤åè½å·æ°å¢æ¯é¨æ°æ®
 - æ·»å æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹ -
 æ·»å å¤§å­¦ä¹ æéå¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹ -
```

### Comparing `TeenStudy-0.1.6/TeenStudy/models/accuont.py` & `TeenStudy-0.1.7/TeenStudy/models/accuont.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/models/dxx.py` & `TeenStudy-0.1.7/TeenStudy/models/dxx.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/resource/answer.png` & `TeenStudy-0.1.7/TeenStudy/resource/answer.png`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/resource/backgroud1.jpg` & `TeenStudy-0.1.7/TeenStudy/resource/backgroud1.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/resource/backgroud2.jpg` & `TeenStudy-0.1.7/TeenStudy/resource/backgroud2.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/resource/backgroud3.jpg` & `TeenStudy-0.1.7/TeenStudy/resource/backgroud3.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/resource/backgroud4.jpg` & `TeenStudy-0.1.7/TeenStudy/resource/backgroud4.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/resource/backgroud5.jpg` & `TeenStudy-0.1.7/TeenStudy/resource/backgroud5.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/resource/dxx_jx.json` & `TeenStudy-0.1.7/TeenStudy/resource/dxx_jx.json`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/resource/MiSans-Light.ttf` & `TeenStudy-0.1.7/TeenStudy/resource/MiSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/utils/dxx.py` & `TeenStudy-0.1.7/TeenStudy/utils/dxx.py`

 * *Files 1% similar despite different names*

```diff
@@ -831,8 +831,77 @@
                     "msg": "提交失败！"
                 }
         except Exception as e:
             logger.error(e)
             return {
                 "status": 500,
                 "msg": f"提交失败,{e}"
-            }
+            }
+
+
+async def jilin(user_id: int) -> dict:
+    """
+    吉青飞扬
+    :param user_id:
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        openid = result[0]["openid"]
+        dxx_id = result[0]["dxx_id"]
+        answer = await Answer.all().order_by("time").values()
+        title = answer[-1]["catalogue"]
+        headers.update(
+            {
+                "Host": "jqfy.jl54.org",
+                "Connection": "keep-alive",
+                "Upgrade-Insecure-Requests": "1",
+                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/wxpic,image/tpg,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+                "X-Requested-With": "com.tencent.mm",
+                "Accept-Encoding": "gzip, deflate",
+                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7"
+            }
+        )
+        try:
+            commit_url = f"http://jqfy.jl54.org/jltw/wechat/editStudyRecord/{dxx_id}"
+            data = {
+                "openid": openid
+            }
+            async with AsyncClient(headers=headers) as client:
+                response = await client.post(url=commit_url, params=data)
+            if response.status_code == 200:
+                response.encoding = response.charset_encoding
+                if response.json()["code"] == '0001':
+                    await User.filter(user_id=user_id).update(
+                        commit_time=time.time(),
+                        catalogue=title
+                    )
+                    await commit(user_id=user_id, catalogue=title, status=True)
+                    return {
+                        "status": 0,
+                        "catalogue": title,
+                        "msg": "提交成功！"
+                    }
+                else:
+                    await commit(user_id=user_id, catalogue=title, status=False)
+                    return {
+                        "status": 500,
+                        "msg": f"提交失败!"
+                    }
+            else:
+                await commit(user_id=user_id, catalogue=title, status=False)
+                return {
+                    "status": 500,
+                    "msg": "提交失败！"
+                }
+        except Exception as e:
+            logger.error(e)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
```

### Comparing `TeenStudy-0.1.6/TeenStudy/utils/handle.py` & `TeenStudy-0.1.7/TeenStudy/utils/handle.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,26 @@
 from ..models.accuont import User, AddUser
 from ..models.dxx import Area, Answer, PushList
 
 scheduler = require('nonebot_plugin_apscheduler').scheduler
 SUPERS = get_driver().config.superusers
 CONFIG = getConfig()
 
-end_pic = on_command("end_pic", aliases={"完成截图", "大学习截图"}, permission=SUPERUSER | GROUP, rule=Rule(must_command,must_group),
+end_pic = on_command("end_pic", aliases={"完成截图", "大学习截图"}, permission=SUPERUSER | GROUP,
+                     rule=Rule(must_command, must_group),
                      priority=50)
 
 submit = on_command("submit", aliases={"提交大学习"}, permission=SUPERUSER | GROUP, rule=Rule(must_command, must_group),
                     priority=50)
 add = on_command("add_dxx", aliases={"添加大学习"}, permission=GROUP, rule=must_group, priority=50)
-my_info = on_command("my_info", aliases={"我的大学习"}, permission=SUPERUSER | GROUP, rule=Rule(must_command,must_group), priority=50)
+my_info = on_command("my_info", aliases={"我的大学习"}, permission=SUPERUSER | GROUP,
+                     rule=Rule(must_command, must_group), priority=50)
 poke_notify = on_notice(priority=60, rule=check_poke)
-answer_pic = on_command("answer_pic", aliases={"答案截图", "大学习"}, rule=Rule(must_command,must_group), permission=SUPERUSER | GROUP,
+answer_pic = on_command("answer_pic", aliases={"答案截图", "大学习"}, rule=Rule(must_command, must_group),
+                        permission=SUPERUSER | GROUP,
                         priority=50)
 finish_dxx = on_command("finish_dxx", aliases={"完成大学习", "全员大学习"},
                         rule=Rule(must_command, must_group, must_leader), permission=GROUP | SUPERUSER, priority=50)
 reset_config = on_command("reset_config", aliases={"重置配置", "刷新配置"}, permission=SUPERUSER, rule=must_command,
                           priority=50)
 reset_password = on_command("reset_password", aliases={"重置密码"}, permission=GROUP,
                             rule=Rule(must_command, must_group), priority=50)
@@ -57,17 +60,24 @@
         if not await check_time():
             await submit.finish(
                 message=MessageSegment.text("当前时间段禁止提交青年大学习，请在周一11:00之后再提交哦(｡･ω･｡)"),
                 at_sender=True, reply_message=True)
         area = result[0]['area']
         data = await distribute_area(user_id=user_id, area=area)
         if data['status'] == 0:
-            message = f'青年大学习{data["catalogue"]}提交成功( ･´ω`･ )\n个人详细信息可扫码登录查看(｡･ω･｡)'
-            await submit.send(message=MessageSegment.text(message) + MessageSegment.image(await get_login_qrcode()),
-                              at_sender=True, reply_message=True)
+            message = f'青年大学习{data["catalogue"]}提交成功( ･´ω`･ )'
+            config = getConfig()
+            content = await get_login_qrcode()
+            if config["URL_STATUS"]:
+                await submit.send(message=MessageSegment.text(message) + MessageSegment.text(
+                    f"\n请点击链接登录查看,如QQ点击无法打开，请复制链接到浏览器打开\n{content['url']}"),
+                                  at_sender=True, reply_message=True)
+            else:
+                await submit.send(message=MessageSegment.text(message) + MessageSegment.image(content['content']),
+                                  at_sender=True, reply_message=True)
             await asyncio.sleep(1)
             await submit.finish(
                 message=MessageSegment.text("青年大学习最新一期完成截图") + MessageSegment.image(await get_end_pic()),
                 at_sender=True, reply_message=True)
         await submit.finish(message=MessageSegment.text(data['msg']), at_sender=True, reply_message=True)
     else:
         await submit.finish(message=MessageSegment.text("用户数据不存在！请使用 添加大学习 指令添加(｡･ω･｡)"),
@@ -84,28 +94,44 @@
         state['province'] = str(msg)
 
 
 @add.got(key="province", prompt="请输入需要添加的省份或回复 取消 停止操作！")
 async def add_(event: GroupMessageEvent, province: str = ArgStr("province")) -> None:
     group_id = event.group_id
     user_id = event.user_id
+    config = getConfig()
     if province in ["取消", "No", "停止", "NO"]:
         await add.finish(message=MessageSegment.text("操作取消！φ(>ω<*) "), at_sender=True, reply_message=True)
     if await Area.filter(area=province).count():
         url = await distribute_area_url(province=province, user_id=user_id, group_id=group_id)
         if province in ["上海", "浙江"]:
-            result = await add.send(
-                message=MessageSegment.text("请使用微信扫码进行绑定( ･´ω`･ )") + MessageSegment.image(
-                    await get_qrcode(user_id=user_id, group_id=group_id, area=province)), at_sender=True,
-                reply_message=True)
+            content = await get_qrcode(user_id=user_id, group_id=group_id, area=province)
+            if config["URL_STATUS"]:
+                result = await add.send(
+                    message=MessageSegment.text(f"请复制链接到微信点击打开进行绑定( ･´ω`･ )\n{content['url']}"),
+                    at_sender=True,
+                    reply_message=True)
+            else:
+                result = await add.send(
+                    message=MessageSegment.text("请使用微信扫码进行绑定( ･´ω`･ )") + MessageSegment.image(
+                        content["content"]), at_sender=True,
+                    reply_message=True)
         else:
-            result = await add.send(
-                message=MessageSegment.text(f"请扫码进入网页添加绑定( ･´ω`･ )") + MessageSegment.image(url),
-                at_sender=True,
-                reply_message=True)
+            if config["URL_STATUS"]:
+                result = await add.send(
+                    message=MessageSegment.text(
+                        f"请点击链接进入网页添加绑定，如QQ无法打开链接，请复制链接到浏览器( ･´ω`･ )\n{url['url']}"),
+                    at_sender=True,
+                    reply_message=True)
+            else:
+                result = await add.send(
+                    message=MessageSegment.text(f"请扫码进入网页添加绑定( ･´ω`･ )") + MessageSegment.image(
+                        url['content']),
+                    at_sender=True,
+                    reply_message=True)
         await AddUser.create(
             time=time.time(),
             user_id=user_id,
             group_id=group_id,
             area=province,
             message_id=result["message_id"],
             status="未通过"
@@ -117,18 +143,26 @@
             at_sender=True,
             reply_message=True)
 
 
 @my_info.handle()
 async def my_info_(event: MessageEvent) -> None:
     user_id = event.user_id
+    config = getConfig()
     if await User.filter(user_id=user_id).count():
-        await my_info.finish(
-            message=MessageSegment.text('请扫码登录查看哦(｡･ω･｡)') + MessageSegment.image(await get_login_qrcode()),
-            at_sender=True, reply_message=True)
+        content = await get_login_qrcode()
+        if config["URL_STATUS"]:
+            await my_info.finish(
+                message=MessageSegment.text(
+                    f'请点击链接登录查看哦，如QQ打不开链接，请复制链接到浏览器(｡･ω･｡)\n{content["url"]}'),
+                at_sender=True, reply_message=True)
+        else:
+            await my_info.finish(
+                message=MessageSegment.text('请扫码登录查看哦(｡･ω･｡)') + MessageSegment.image(content['content']),
+                at_sender=True, reply_message=True)
     else:
         await my_info.finish(
             message=MessageSegment.text("你还没有绑定大学习哦ヾ(ｏ･ω･)ﾉ，使用 添加大学习 指令进行绑定信息吧( • ̀ω•́ )✧"),
             at_sender=True, reply_message=True)
 
 
 @poke_notify.handle()
@@ -150,18 +184,25 @@
             if not await check_time():
                 await submit.finish(
                     message=MessageSegment.text("当前时间段禁止提交青年大学习，请在周一11:00之后再提交哦(｡･ω･｡)"),
                     at_sender=True)
             area = result[0]['area']
             data = await distribute_area(user_id=user_id, area=area)
             if data['status'] == 0:
-                message = f'青年大学习{data["catalogue"]}提交成功( ･´ω`･ )\n个人详细信息请扫码登录查看(｡･ω･｡)'
-                await poke_notify.send(
-                    message=MessageSegment.text(message) + MessageSegment.image(await get_login_qrcode()),
-                    at_sender=True)
+                message = f'青年大学习{data["catalogue"]}提交成功( ･´ω`･ )'
+                content = await get_login_qrcode()
+                if config["URL_STATUS"]:
+                    await poke_notify.send(
+                        message=MessageSegment.text(message) + MessageSegment.text(
+                            f"\n请点击链接登录查看,如QQ点击无法打开，请复制链接到浏览器打开\n{content['url']}"),
+                        at_sender=True)
+                else:
+                    await poke_notify.send(
+                        message=MessageSegment.text(message + "\n个人信息请扫码登录查看") + MessageSegment.image(
+                            content["content"]), at_sender=True)
                 await asyncio.sleep(1)
                 await poke_notify.finish(
                     message=MessageSegment.text("青年大学习最新一期完成截图") + MessageSegment.image(
                         await get_end_pic()), at_sender=True,
                     reply_message=True)
             await poke_notify.finish(message=MessageSegment.text(data['msg']), at_sender=True, reply_message=True)
         else:
@@ -188,15 +229,15 @@
 
 @finish_dxx.got(key="msg", prompt="是否提交团支部全体成员最新一期青年大学习？（是|否）")
 async def finish(event: GroupMessageEvent, msg: str = ArgStr("msg")) -> None:
     if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
         await finish_dxx.finish(message=MessageSegment.text("操作取消(*^▽^*)"), at_sender=True, reply_message=True)
     else:
         await finish_dxx.send(message=MessageSegment.text("开始提交(*￣︶￣)"), at_sender=True, reply_message=True)
-    self_id = event.self_id
+
     group_id = event.group_id
     user_id = event.user_id
     result = await User.filter(leader=user_id, group_id=group_id).values()
     if result:
         answer_result = await Answer.all().order_by('time').values()
         catalogue = answer_result[-1]["catalogue"]
         for item in result:
@@ -284,14 +325,15 @@
 async def push_dxx() -> None:
     config = getConfig()
     if not config["DXX_REMIND"]:
         return
     try:
         bot: Bot = get_bot()
     except ValueError as e:
+        logger.error(e)
         return None
     answer_result = await Answer.all().order_by('time').values()
     if (int(time.time()) - answer_result[-1]["time"]) > 259200:
         return None
     else:
         catalogue = answer_result[-1]["catalogue"]
         now_time = datetime.datetime.fromtimestamp(answer_result[-1]["time"]).strftime("%Y年%m月%d日 %H:%M:%S")
```

### Comparing `TeenStudy-0.1.6/TeenStudy/utils/path.py` & `TeenStudy-0.1.7/TeenStudy/utils/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     """戳一戳提交大学习状态"""
     AUTO_SUBMIT: bool = True
     """周一11:30自动提交状态"""
     AUTO_SUBMIT_HOUR: int = 11
     """大学习自动提交时间-小时，可选范围：0-23"""
     AUTO_SUBMIT_MINUTE: int = 30
     """大学习自动提交时间-分钟，可选范围：0-59"""
+    URL_STATUS: bool = False
+    """是否将二维码转链接发送，默认为False"""
 
 
 def saveConfig(data: dict) -> bool:
     try:
         config = Config().dict()
         config.update(**data)
         with open(CONFIG_PATH, "w", encoding="utf-8") as w:
@@ -74,20 +76,25 @@
     except Exception as e:
         logger.error(e)
         return False
 
 
 def getConfig() -> dict:
     if not Path(CONFIG_PATH).exists():
-        status = saveConfig({})
+        status = saveConfig({
+        })
         if status:
             return Config().dict()
     else:
         with open(CONFIG_PATH, "r", encoding="utf-8") as f:
             obj = json.load(f)
+        if "URL_STATUS" not in obj.keys():
+            obj["URL_STATUS"] = False
+            with open(CONFIG_PATH, "w", encoding="utf-8") as w:
+                json.dump(obj, w, indent=4, ensure_ascii=False)
         return obj
 
 
 def register_database(db_name: str, models: str, db_path: Optional[Union[str, Path]]):
     """
     注册数据库
     :param db_name: 数据库名称
```

### Comparing `TeenStudy-0.1.6/TeenStudy/utils/rule.py` & `TeenStudy-0.1.7/TeenStudy/utils/rule.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/utils/update.py` & `TeenStudy-0.1.7/TeenStudy/utils/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import time
 
 from bs4 import BeautifulSoup
 from httpx import AsyncClient
 from nonebot import logger, require, get_bot, get_driver
 from nonebot.adapters.onebot.v11 import Bot, MessageSegment
 
-from .utils import get_login_qrcode
 from .path import getConfig
+from .utils import get_login_qrcode
 from ..models.accuont import AddUser, User
 from ..models.dxx import Answer, Area
 
 scheduler = require('nonebot_plugin_apscheduler').scheduler
 super_id = get_driver().config.superusers  # 超管id
 headers = {
     "Host": "h5.cyol.com",
@@ -183,17 +183,22 @@
                     url=url,
                     end_url=end_url,
                     answer=answer,
                     cover=cover
                 )
                 logger.opt(colors=True).success(f"<u><y>青年大学习</y></u> <m>{catalogue}</m> <g>更新成功!</g>")
                 admin = getConfig()
+                content = await get_login_qrcode()
+                if admin["URL_STATUS"]:
+                    await bot.send_private_msg(user_id=admin["SUPERUSER"], message=MessageSegment.text(
+                        f"检测到青年大学习有更新，下周一为{catalogue},详细信息请点击链接登录后台查看，如打不开链接，请复制链接到浏览器d(´ω｀*)\n") + MessageSegment.text(
+                        content["url"]))
                 await bot.send_private_msg(user_id=admin["SUPERUSER"], message=MessageSegment.text(
                     f"检测到青年大学习有更新，下周一为{catalogue},详细信息请扫码登录后台查看d(´ω｀*)") + MessageSegment.image(
-                    await get_login_qrcode()))
+                    content["content"]))
             except Exception as e:
                 logger.error(e)
 
 
 @scheduler.scheduled_job('cron', second='*/15', misfire_grace_time=10)
 async def check_apply():
     try:
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 import asyncio import json import time from bs4 import BeautifulSoup from httpx
 import AsyncClient from nonebot import logger, require, get_bot, get_driver
-from nonebot.adapters.onebot.v11 import Bot, MessageSegment from .utils import
-get_login_qrcode from .path import getConfig from ..models.accuont import
+from nonebot.adapters.onebot.v11 import Bot, MessageSegment from .path import
+getConfig from .utils import get_login_qrcode from ..models.accuont import
 AddUser, User from ..models.dxx import Answer, Area scheduler = require
 ('nonebot_plugin_apscheduler').scheduler super_id = get_driver
 ().config.superusers # è¶ç®¡id headers = { "Host": "h5.cyol.com",
 "Connection": "keep-alive", "Accept": "application/json, text/javascript, */*;
 q=0.01", "User-Agent": "Mozilla/5.0 (Linux; Android 10; PACM00 Build/
 QP1A.190711.020; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/
 86.0.4240.99 XWEB/3164 MMWEBSDK/20211001 Mobile Safari/537.36 MMWEBID/556
@@ -68,31 +68,36 @@
 (result)[-10:] for code in code_result: if await Answer.filter(code=code).count
 (): continue else: try: url = result[code]["url"] data = await crawl_answer
 (url=url) end_url = data["end_url"] answer = data["answer"] catalogue = data
 ["catalogue"] async with AsyncClient(headers=headers) as client: end_jpg =
 await client.get(end_url, timeout=10) cover = end_jpg.content await
 Answer.create( time=time.time(), code=code, catalogue=catalogue, url=url,
 end_url=end_url, answer=answer, cover=cover ) logger.opt(colors=True).success
-(f"éå¹´å¤§å­¦ä¹  {catalogue} æ´æ°æå!") admin = getConfig() await
+(f"éå¹´å¤§å­¦ä¹  {catalogue} æ´æ°æå!") admin = getConfig() content =
+await get_login_qrcode() if admin["URL_STATUS"]: await bot.send_private_msg
+(user_id=admin["SUPERUSER"], message=MessageSegment.text
+( f"æ£æµå°éå¹´å¤§å­¦ä¹ ææ´æ°ï¼ä¸å¨ä¸ä¸º
+{catalogue},è¯¦ç»ä¿¡æ¯è¯·ç¹å»é¾æ¥ç»å½åå°æ¥çï¼å¦æä¸å¼é¾æ¥ï¼è¯·å¤å¶é¾æ¥å°æµè§å¨d
+(Â´Ïï½*)\n") + MessageSegment.text( content["url"])) await
 bot.send_private_msg(user_id=admin["SUPERUSER"], message=MessageSegment.text
 ( f"æ£æµå°éå¹´å¤§å­¦ä¹ ææ´æ°ï¼ä¸å¨ä¸ä¸º
 {catalogue},è¯¦ç»ä¿¡æ¯è¯·æ«ç ç»å½åå°æ¥çd(Â´Ïï½*)") +
-MessageSegment.image( await get_login_qrcode())) except Exception as e:
-logger.error(e) @scheduler.scheduled_job('cron', second='*/15',
-misfire_grace_time=10) async def check_apply(): try: bot: Bot = get_bot()
-except ValueError as e: return apply_list = await AddUser.filter
-(status="æªéè¿").values() for item in apply_list: result = await
-User.filter(user_id=item["user_id"], group_id=item["group_id"]).count() if
-result: await AddUser.filter(id=item["id"]).update(status="å·²éè¿") await
-bot.send_group_msg(group_id=item["group_id"], message=MessageSegment.at
-(user_id=item["user_id"]) + MessageSegment.text( "ä¿¡æ¯ç»å®æå( â¢
-ÌÏâ¢Ì )â§")) await asyncio.sleep(2) continue now_time = int(time.time())
-if (now_time - item["time"]) > 180: await AddUser.filter(id=item["id"]).update
-(status="å·²è¿æ") await bot.send_group_msg(group_id=item["group_id"],
-message=MessageSegment.at(user_id=item["user_id"]) + MessageSegment.text
+MessageSegment.image( content["content"])) except Exception as e: logger.error
+(e) @scheduler.scheduled_job('cron', second='*/15', misfire_grace_time=10)
+async def check_apply(): try: bot: Bot = get_bot() except ValueError as e:
+return apply_list = await AddUser.filter(status="æªéè¿").values() for item
+in apply_list: result = await User.filter(user_id=item["user_id"],
+group_id=item["group_id"]).count() if result: await AddUser.filter(id=item
+["id"]).update(status="å·²éè¿") await bot.send_group_msg(group_id=item
+["group_id"], message=MessageSegment.at(user_id=item["user_id"]) +
+MessageSegment.text( "ä¿¡æ¯ç»å®æå( â¢ ÌÏâ¢Ì )â§")) await
+asyncio.sleep(2) continue now_time = int(time.time()) if (now_time - item
+["time"]) > 180: await AddUser.filter(id=item["id"]).update(status="å·²è¿æ")
+await bot.send_group_msg(group_id=item["group_id"], message=MessageSegment.at
+(user_id=item["user_id"]) + MessageSegment.text
 ( "æ·»å ç³è¯·å·²è¿æï¼è¯·éæ°å æ·»å å¤§å­¦ä¹  æä»¤è¿è¡ç³è¯·( â¢
 ÌÏâ¢Ì )â§")) await asyncio.sleep(2) else: continue
 @scheduler.scheduled_job('cron', day_of_week='0', hour='0', minute='0',
 id='clear', timezone="Asia/Shanghai") async def clear(): try: result = await
 Area.all().values() for item in result: await Area.filter(id=item["id"]).update
 (status=False) logger.opt(colors=True).success( f"[å¤§å­¦ä¹ æ°æ®åº]
 å°åºææ°ä¸æç¶æ éç½®æå!") except Exception as e: logger.opt
```

### Comparing `TeenStudy-0.1.6/TeenStudy/utils/utils.py` & `TeenStudy-0.1.7/TeenStudy/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from io import BytesIO
 from pathlib import Path
 
 import qrcode
 from PIL import Image, ImageDraw, ImageFont
 from httpx import AsyncClient
 from nonebot import logger, get_driver, on_command
+from nonebot.adapters.onebot.v11 import MessageEvent
 from nonebot.params import ArgStr
 from nonebot.permission import SUPERUSER
 from pydantic import BaseModel
 
 from . import dxx, path, rule
 from ..models.accuont import User
 from ..models.dxx import Area, Answer, Resource, JiangXi
@@ -156,14 +157,23 @@
         "host": "qndxx.cqyouths.com",
         "referer": None,
         "origin": "http://qndxx.cqyouths.com",
         "url": "http://qndxx.cqyouths.com/new_course.json?time=",
         "status": True,
         "catalogue": None
     },
+    {
+        "area": "吉林",
+        "host": "jqfy.jl54.org",
+        "referer": None,
+        "origin": "http://jqfy.jl54.org/jltw/wechat",
+        "url": "http://jqfy.jl54.org/jltw/wechat",
+        "status": True,
+        "catalogue": None
+    },
 ]
 RESOURCE = [
     {
         "name": "MiSans-Light.ttf",
         "url": "",
         "type": "字体",
         "size": "7.6 M"
@@ -218,22 +228,24 @@
         await JiangXi.all().delete()
         await Resource.all().delete()
         await resource_init()
         await update_resource.finish(message="资源数据载入成功(^_−)☆", at_sender=True, reply_message=True)
 
 
 @export_data.got(key="msg", prompt="是否导出用户数据至TeenStudy目录？（是|否）")
-async def export_user(msg: str = ArgStr("msg")) -> None:
+async def export_user(event: MessageEvent, msg: str = ArgStr("msg")) -> None:
+    self_id = event.self_id
     if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
         await export_data.finish(message="操作取消(*^▽^*)", at_sender=True, reply_message=True)
     else:
         result = await User.all().values()
         user_list = []
         for item in result:
             data = UserModel().dict()
+            item["self_id"] = self_id
             data.update(**item)
             user_list.append(data)
         with open(USERDATA, "w", encoding="utf-8") as w:
             json.dump(user_list, w, indent=4, ensure_ascii=False)
         await export_data.finish(message="用户数据成功导出至TeenStudy目录(*^▽^*)", at_sender=True,
                                  reply_message=True)
 
@@ -301,14 +313,15 @@
             logger.opt(colors=True).info(
                 f'<u><y>[大学习数据库]</y></u><g>加载配置公网IP成功，启动检测公网IP访问状态</g>ip:<m>{ip}</m>')
             url = f"http://{ip}:{get_driver().config.port}/TeenStudy/login"
             logger.info(url)
             try:
                 async with AsyncClient(headers=headers) as client:
                     response = await client.get(url=url)
+                logger.debug(f"公网请求状态：{response.status_code}")
                 if response.status_code != 200:
                     ip = ""
                     logger.opt(colors=True).info(
                         f'<u><y>[大学习数据库]</y></u><g>检测到配置公网ip地址无法通过外网访问，将自动获取公网IP</g>')
                 logger.opt(colors=True).success(
                     f'<u><y>[大学习提交 Web UI]</y></u><g>配置外网IP设置成功</g>，外网访问地址为:<m>http://{ip}:{get_driver().config.port}/TeenStudy/login</m>')
             except Exception as e:
@@ -324,26 +337,29 @@
             async with AsyncClient(headers=headers) as client:
                 response = await client.get("http://ip.42.pl/raw")
             if response.status_code == 200:
                 ip = response.text.strip()
                 logger.opt(colors=True).info(
                     f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP成功，启动检测公网IP访问状态</g>ip:<m>{ip}</m>')
                 url = f"http://{ip}:{get_driver().config.port}/TeenStudy/login"
+                logger.info(url)
                 try:
-                    async with AsyncClient(headers=headers) as client:
+                    async with AsyncClient(headers=headers, timeout=5) as client:
                         response = await client.get(url=url)
+                    logger.debug(f"公网请求状态:{response.status_code}")
                     if response.status_code != 200:
                         ip = ""
                         logger.opt(colors=True).warning(
                             f'<u><y>[大学习数据库]</y></u><g>检测到ip地址无法通过外网访问，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
                     else:
                         logger.opt(colors=True).success(
                             f'<u><y>[大学习提交 Web UI]</y></u><g>自动获取外网IP成功</g>，外网访问地址为:<m>http://{ip}:{get_driver().config.port}/TeenStudy/login</m>')
                 except Exception as e:
                     ip = ""
+                    logger.debug(e)
                     logger.opt(colors=True).warning(
                         f'<u><y>[大学习数据库]</y></u><g>检测到ip地址无法通过外网访问，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
             else:
                 ip = ""
                 logger.opt(colors=True).warning(
                     f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP失败，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
         if not ip:
@@ -484,17 +500,24 @@
         return await dxx.anhui(user_id=user_id)
     elif area == "四川":
         return await dxx.sichuan(user_id=user_id)
     elif area == "山东":
         return await dxx.shandong(user_id=user_id)
     elif area == "重庆":
         return await dxx.chongqing(user_id=user_id)
+    elif area == "吉林":
+        return await dxx.jilin(user_id=user_id)
+    else:
+        return {
+            "status": 404,
+            "msg": "该地区暂未支持！"
+        }
 
 
-async def distribute_area_url(province: str, user_id: int, group_id: int) -> str:
+async def distribute_area_url(province: str, user_id: int, group_id: int) -> dict:
     config = path.getConfig()
     if province == "湖北":
         province = "hubei"
     elif province == "江西":
         province = "jiangxi"
     elif province == "江苏":
         province = "jiangsu"
@@ -502,39 +525,50 @@
         province = "anhui"
     elif province == "四川":
         province = "sichuan"
     elif province == "山东":
         province = "shandong"
     elif province == "重庆":
         province = "chongqing"
+    elif province == "吉林":
+        province = "jilin"
     data = f"http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/{province}?user_id={user_id}&group_id={group_id}"
     img = qrcode.make(data=data)
     buf = BytesIO()
     img.save(buf, format="PNG")
     base64_str = base64.b64encode(buf.getbuffer()).decode()
     content = "base64://" + base64_str
-    return content
+    return {
+        "url": data,
+        "content": content
+    }
 
 
-async def get_login_qrcode() -> str:
+async def get_login_qrcode() -> dict:
     config = path.getConfig()
     data = f'http://{config["DXX_IP"]}:{config["DXX_PORT"]}/TeenStudy/login'
     img = qrcode.make(data=data)
     buf = BytesIO()
     img.save(buf, format="PNG")
     base64_str = base64.b64encode(buf.getbuffer()).decode()
     content = "base64://" + base64_str
-    return content
+    return {
+        "url": data,
+        "content": content
+    }
 
 
-async def get_qrcode(user_id: int, group_id: int, area: str) -> str:
+async def get_qrcode(user_id: int, group_id: int, area: str) -> dict:
     config = path.getConfig()
     if area == "浙江":
         data = f"https://open.weixin.qq.com/connect/oauth2/authorize?appid=wx56b888a1409a2920&redirect_uri=https://wx.yunban.cn/wx/oauthInfoCallback?r_uri=http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/zhejiang/{user_id}/{group_id}&source=common&response_type=code&scope=snsapi_userinfo&state=STATE&component_appid=wx0f0063354bfd3d19&connect_redirect=1"
     else:
         data = f"https://open.weixin.qq.com/connect/oauth2/authorize?appid=wxa693f4127cc93fad&redirect_uri=https://wx.yunban.cn/wx/oauthInfoCallback?r_uri=http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/shanghai/{user_id}/{group_id}&source=common&response_type=code&scope=snsapi_userinfo&state=STATE&component_appid=wx0f0063354bfd3d19&connect_redirect=1"
     img = qrcode.make(data=data)
     buf = BytesIO()
     img.save(buf, format="PNG")
     base64_str = base64.b64encode(buf.getbuffer()).decode()
     content = "base64://" + base64_str
-    return content
+    return {
+        "url": data,
+        "content": content
+    }
```

### Comparing `TeenStudy-0.1.6/TeenStudy/web/__init__.py` & `TeenStudy-0.1.7/TeenStudy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/web/api/add.py` & `TeenStudy-0.1.7/TeenStudy/web/api/add.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import json
 import re
 import time
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi.responses import HTMLResponse, JSONResponse, RedirectResponse
 from httpx import AsyncClient
 
 from ..pages.add import hubei_page, jiangxi_page, jiangsu_page, anhui_page, sichuan_page, shandong_page, \
-    chongqing_page
+    chongqing_page, jilin_page
 from ..utils.add import write_to_database
 from ...models.accuont import User, AddUser
 from ...models.dxx import JiangXi
 
 route = APIRouter()
 
 
@@ -639,7 +640,81 @@
         return chongqing_page.render(
             site_title='重庆共青团 | TeenStudy',
             site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
+
+
+@route.post("/jilin/add", response_class=HTMLResponse)
+async def jilin_add(data: dict) -> JSONResponse:
+    user_id = data["user_id"]
+    if await User.filter(user_id=user_id).count():
+        return JSONResponse({
+            "status": 0,
+            "msg": "添加失败！，用户信息存在！"
+        })
+    else:
+        try:
+            openid = data["openid"]
+            headers = {
+                "Host": "jqfy.jl54.org",
+                "Connection": "keep-alive",
+                "Upgrade-Insecure-Requests": "1",
+                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+                "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/wxpic,image/tpg,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+                "X-Requested-With": "com.tencent.mm",
+                "Accept-Encoding": "gzip, deflate",
+                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7"
+            }
+            url = "http://jqfy.jl54.org/jltw/wechat/updateStudentInfo"
+            params = {
+                "openid_u": openid
+            }
+            async with AsyncClient(headers=headers) as client:
+                response = await client.post(url=url, params=params)
+            if response.status_code == 200:
+                response.encoding = response.charset_encoding
+                start = "var studentInfo ="
+                end = 'var ctxPath = "\/jltw\/"'
+                content = json.loads(
+                    response.text[response.text.find(start):response.text.find(end)].split("=")[-1].replace(";",
+                                                                                                            "").strip())
+                data["mobile"] = content["telNum"]
+                data["name"] = content["name"]
+                data["organization_id"] = content["typeInfoId"]
+                data["dxx_id"] = content["id"]
+                data["gender"] = content["sex"]
+                status = await write_to_database(data=data)
+                if status:
+                    return JSONResponse(
+                        {
+                            "status": 0,
+                            "msg": "添加成功！"
+                        }
+                    )
+                else:
+                    return JSONResponse({
+                        "status": 500,
+                        "msg": "添加失败！"
+                    })
+            else:
+                return JSONResponse({"status": 500, "msg": "添加失败！"})
+        except Exception as e:
+            return JSONResponse({
+                "status": 500,
+                "msg": f"添加失败,{e}"
+            })
+
+
+@route.get("/jilin", response_class=HTMLResponse)
+async def jilin(user_id: int, group_id: int):
+    result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
+    if result:
+        return jilin_page.render(
+            site_title='吉青飞扬 | TeenStudy',
+            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+        )
+    return RedirectResponse(
+        url="/TeenStudy/login"
+    )
```

### Comparing `TeenStudy-0.1.6/TeenStudy/web/api/admin.py` & `TeenStudy-0.1.7/TeenStudy/web/api/admin.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/web/api/home.py` & `TeenStudy-0.1.7/TeenStudy/web/api/home.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/web/api/login.py` & `TeenStudy-0.1.7/TeenStudy/web/api/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @route.post('/login', response_class=JSONResponse)
 async def login(user: UserModel):
     user_id = user.user_id
     password = await to_hash(user.password)
     role = user.role
     if role:
         result = getConfig()
-        if result["SUPERUSER"] != user_id:
+        if result["SUPERUSER"] != user_id or result["PASSWORD"] != password:
             result = False
     else:
         result = await User.filter(user_id=user_id, password=password).count()
     if not result:
         return {
             'status': -100,
             'msg': '登录失败，请确认用户ID和密码无误'
```

### Comparing `TeenStudy-0.1.6/TeenStudy/web/pages/add.py` & `TeenStudy-0.1.7/TeenStudy/web/pages/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -745,7 +745,100 @@
             clearable=True,
         )
 
     ]
 )
 
 chongqing_page = Page(title='添加大学习', body=[logo, Divider(), chongqing_table, footer])
+
+jilin_table = Form(
+    title="吉青飞扬",
+    mode=DisplayModeEnum.horizontal,
+    api="post:/TeenStudy/api/jilin/add",
+    redirect="/TeenStudy/login",
+    body=[
+        InputText(
+            label="用户ID",
+            description="用户ID，为用户QQ号，无需填写",
+            name="user_id",
+            value="${user_id}",
+            disabled=True
+        ),
+        InputText(
+            label="通知群ID",
+            description="通知群号，无需填写",
+            name="group_id",
+            value="${group_id}",
+            disabled=True
+        ),
+        InputText(
+            label="地区",
+            description="所处省份",
+            name="area",
+            value="吉林",
+            disabled=True
+        ),
+        InputText(
+            label="登录密码",
+            type='input-password',
+            description="可不填，默认为用户ID",
+            name="password",
+            inline=False,
+            required=False,
+            value="",
+            clearable=True,
+            maxLength=16
+        ),
+        InputText(
+            label="姓名",
+            description="您的姓名",
+            name="name",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=8
+        ),
+        InputText(
+            label="openid",
+            description="自行抓包获取，结构为: ohz9xxxxxxxxxxxxlF0Io0uCnM",
+            name="openid",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+        ),
+        InputText(
+            label="学校",
+            description="你就读的高校",
+            name="university",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=24
+        ),
+        InputText(
+            label="学院",
+            description="学院名称",
+            name="college",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=32
+        ),
+        InputText(
+            label="团支部",
+            description="团支部|班级，没有可不填",
+            name="organization",
+            inline=False,
+            required=False,
+            value="",
+            clearable=True,
+            maxLength=32
+        )
+
+    ]
+)
+
+jilin_page = Page(title='添加大学习', body=[logo, Divider(), jilin_table, footer])
```

#### html2text {}

```diff
@@ -305,8 +305,31 @@
 required=False, value="", clearable=True, maxLength=16 ), InputText
 ( label="å§å", description="å¯¹åºéåºå±éå¢ä¸ªäººä¿¡æ¯é¡µ
 æ¨çå§å", name="name", inline=False, required=True, value="",
 clearable=True, maxLength=8 ), InputText( label="openid",
 description="èªè¡æåè·åï¼ç»æä¸º: ohz9xxxxxxxxxxxxlF0Io0uCnM",
 name="openid", inline=False, required=True, value="", clearable=True, ) ] )
 chongqing_page = Page(title='æ·»å å¤§å­¦ä¹ ', body=[logo, Divider(),
-chongqing_table, footer])
+chongqing_table, footer]) jilin_table = Form( title="åéé£æ¬",
+mode=DisplayModeEnum.horizontal, api="post:/TeenStudy/api/jilin/add",
+redirect="/TeenStudy/login", body=[ InputText( label="ç¨æ·ID",
+description="ç¨æ·IDï¼ä¸ºç¨æ·QQå·ï¼æ éå¡«å", name="user_id",
+value="${user_id}", disabled=True ), InputText( label="éç¥ç¾¤ID",
+description="éç¥ç¾¤å·ï¼æ éå¡«å", name="group_id", value="$
+{group_id}", disabled=True ), InputText( label="å°åº",
+description="æå¤çä»½", name="area", value="åæ", disabled=True ),
+InputText( label="ç»å½å¯ç ", type='input-password',
+description="å¯ä¸å¡«ï¼é»è®¤ä¸ºç¨æ·ID", name="password", inline=False,
+required=False, value="", clearable=True, maxLength=16 ), InputText
+( label="å§å", description="æ¨çå§å", name="name", inline=False,
+required=True, value="", clearable=True, maxLength=8 ), InputText
+( label="openid", description="èªè¡æåè·åï¼ç»æä¸º:
+ohz9xxxxxxxxxxxxlF0Io0uCnM", name="openid", inline=False, required=True,
+value="", clearable=True, ), InputText( label="å­¦æ ¡",
+description="ä½ å°±è¯»çé«æ ¡", name="university", inline=False,
+required=True, value="", clearable=True, maxLength=24 ), InputText
+( label="å­¦é¢", description="å­¦é¢åç§°", name="college", inline=False,
+required=True, value="", clearable=True, maxLength=32 ), InputText
+( label="å¢æ¯é¨", description="å¢æ¯é¨|ç­çº§ï¼æ²¡æå¯ä¸å¡«",
+name="organization", inline=False, required=False, value="", clearable=True,
+maxLength=32 ) ] ) jilin_page = Page(title='æ·»å å¤§å­¦ä¹ ', body=[logo,
+Divider(), jilin_table, footer])
```

### Comparing `TeenStudy-0.1.6/TeenStudy/web/pages/admin.py` & `TeenStudy-0.1.7/TeenStudy/web/pages/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     )]
 )
 """提交记录模板"""
 record_table = CRUD(mode='table',
                     title='',
                     syncLocation=False,
                     api='/TeenStudy/api/get_records',
-                    interval=12000,
+                    interval=60000,
                     type='crud',
                     headerToolbar=[ActionType.Ajax(label='删除所有提交记录',
                                                    level=LevelEnum.warning,
                                                    confirmText='确定要删除所有提交记录吗？',
                                                    api='delete:/TeenStudy/api/delete_all?type=records'),
                                    "bulkActions", "reload"],
                     itemActions=[
@@ -123,15 +123,14 @@
                                         level=LevelEnum.warning,
                                         confirmText="确定要批量删除？",
                                         api="delete:/TeenStudy/api/delete_records?ids=${ids|raw}")])
 answer_table = CRUD(mode='table',
                     title='',
                     syncLocation=False,
                     api='/TeenStudy/api/get_answers',
-                    interval=12000,
                     type='crud',
                     headerToolbar=[ActionType.Ajax(label='删除青年大学习期数',
                                                    level=LevelEnum.warning,
                                                    confirmText='确定要删除青年大学习期数吗？',
                                                    api='delete:/TeenStudy/api/delete_all?type=answers'),
                                    "bulkActions", "reload"],
                     itemActions=[
@@ -258,14 +257,22 @@
             showCounter=True,
             trimContents=True,
             resetValue=8080,
             required=True,
             clearable=True
         ),
         Switch(
+            name="URL_STATUS",
+            label="二维码转链接开关",
+            value="${URL_STATUS}",
+            onText='开启',
+            offText='关闭',
+            required=True,
+        ),
+        Switch(
             name="POKE_SUBMIT",
             label="戳一戳提交大学习开关",
             value="${POKE_SUBMIT}",
             onText='开启',
             offText='关闭',
             required=True,
         ),
@@ -302,15 +309,15 @@
     ]
 )
 """申请记录模板"""
 request_table = CRUD(mode='table',
                      title='',
                      syncLocation=False,
                      api='/TeenStudy/api/get_requests',
-                     interval=12000,
+                     interval=60000,
                      type='crud',
                      headerToolbar=[ActionType.Ajax(label='删除所有申请记录',
                                                     level=LevelEnum.warning,
                                                     confirmText='确定要删除所有申请记录吗？',
                                                     api='delete:/TeenStudy/api/delete_all?type=requests'),
                                     "bulkActions", "reload"],
                      itemActions=[
@@ -379,15 +386,15 @@
                   trimContents=True, clearable=True,
                   showCounter=True, maxLength=16, visibleOn="${password==null?false:true}",
                   description='登录Web UI的密码'),
         InputText(label='学校类型', name='university_type', value='${university_type}',
                   showCounter=True, maxLength=16, required=True, trimContents=True,
                   clearable=True,
                   visibleOn="${university_type==null?false:true}",
-                  description='四川地区学校类型，不清楚清无改动'),
+                  description='学校类型，不清楚清无改动'),
         InputText(label='学校ID', name='university_id', value='${university_id}',
                   required=True, trimContents=True, clearable=True,
                   showCounter=True, maxLength=24,
                   visibleOn="${university_id==null?false:true}",
                   description='学校ID，不清楚请勿改动'),
         InputText(label='学校名称', name='university', value='${university}', required=True,
                   trimContents=True, clearable=True,
@@ -1277,20 +1284,125 @@
             required=True,
             value="",
             clearable=True,
         )
 
     ]
 )
+"""吉林添加成员面板"""
+jilin_table = Form(
+    title="吉青飞扬",
+    mode=DisplayModeEnum.horizontal,
+    api="post:/TeenStudy/api/jilin/add",
+    redirect="/TeenStudy/login",
+    body=[
+        Select(
+            label="群聊",
+            name="group_id",
+            description="需要添加的群组",
+            checkAll=False,
+            source="get:/TeenStudy/api/get_group_list",
+            value='',
+            multiple=False,
+            required=True,
+            searchable=True,
+            joinValues=False,
+            extractValue=True,
+            statistics=True,
+        ),
+        Select(
+            label="用户ID",
+            name="user_id",
+            description="需要添加的用户ID",
+            checkAll=False,
+            source="get:/TeenStudy/api/get_member_list?group_id=${group_id}",
+            value='',
+            multiple=False,
+            required=True,
+            searchable=True,
+            joinValues=False,
+            extractValue=True,
+            statistics=True,
+            hiddenOn="${group_id==''?true:false}"
+        ),
+        InputText(
+            label="地区",
+            description="所处省份",
+            name="area",
+            value="吉林",
+            disabled=True
+        ),
+        InputText(
+            label="登录密码",
+            type='input-password',
+            description="可不填，默认为用户ID",
+            name="password",
+            inline=False,
+            required=False,
+            value="",
+            clearable=True,
+            maxLength=16
+        ),
+        InputText(
+            label="姓名",
+            description="您的姓名",
+            name="name",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=8
+        ),
+        InputText(
+            label="openid",
+            description="自行抓包获取，结构为: ohz9xxxxxxxxxxxxlF0Io0uCnM",
+            name="openid",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+        ),
+        InputText(
+            label="学校",
+            description="你就读的高校",
+            name="university",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=24
+        ),
+        InputText(
+            label="学院",
+            description="学院名称",
+            name="college",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=32
+        ),
+        InputText(
+            label="团支部",
+            description="团支部|班级，没有可不填",
+            name="organization",
+            inline=False,
+            required=False,
+            value="",
+            clearable=True,
+            maxLength=32
+        )
+
+    ]
+)
 """推送群聊模板"""
 push_table = CRUD(mode='table',
                   title='',
                   syncLocation=False,
                   api='/TeenStudy/api/get_push_list',
-                  interval=12000,
                   type='crud',
                   headerToolbar=[ActionType.Ajax(label='删除所有推送群聊',
                                                  level=LevelEnum.warning,
                                                  confirmText='确定要删除所有推送群聊吗？',
                                                  api='delete:/TeenStudy/api/delete_all?type=push_list'),
                                  "bulkActions", "reload", ActionType.Dialog(
                           label='添加推送群聊',
@@ -1357,23 +1469,25 @@
                         schema=Page(title='安徽共青团', body=[anhui_table]))
 sichuan_page = PageSchema(url='/add/sichuan', icon='fa fa-pen-to-square', label='天府新青年',
                           schema=Page(title='天府新青年', body=[sichuan_table]))
 shandong_page = PageSchema(url='/add/shandong', icon='fa fa-pen-to-square', label='青春山东',
                            schema=Page(title='青春山东', body=[shandong_table]))
 chongqing_page = PageSchema(url='/add/chongqing', icon='fa fa-pen-to-square', label='重庆共青团',
                             schema=Page(title='重庆共青团', body=[chongqing_table]))
+jilin_page = PageSchema(url='/add/jilin', icon='fa fa-pen-to-square', label='吉青飞扬',
+                        schema=Page(title='吉青飞扬', body=[jilin_table]))
 admin_app = App(brandName='TeenStudy',
                 logo='https://i.328888.xyz/2023/02/23/xIh5k.png',
                 header=header,
                 pages=[{
                     'children': [
                         admin_page,
                         PageSchema(icon='fa fa-circle-user', label='成员管理',
                                    children=[list_page, hubei_page, jiangxi_page, jiangsu_page, anhui_page,
-                                             sichuan_page, shandong_page, chongqing_page]),
+                                             sichuan_page, shandong_page, chongqing_page, jilin_page]),
                         PageSchema(url="/notice", label='推送列表', icon='fa fa-bell',
                                    schema=Page(title='', body=[push_table])),
                         PageSchema(url="/request", label='申请记录', icon='fa fa-circle-info',
                                    schema=Page(title='', body=[request_table])),
                         PageSchema(url="/answer", label='大学习列表', icon='fa fa-book-open',
                                    schema=Page(title='', body=[answer_table])),
                         PageSchema(url="/records", label='提交记录', icon='fa fa-code-commit',
```

#### html2text {}

```diff
@@ -21,15 +21,15 @@
 ( label='æ¯æå°åºæ°é', content='${area_count}' ), Property.Item
 ( label='ææ°ä¸æå¤§å­¦ä¹ ', content='${catalogue}' ), Property.Item
 ( label='å¬ç½è®¿é®IP', content='${ip}' ), Property.Item
 ( label='CPUå ç¨ç', content='${cpu_percent}' ), Property.Item
 ( label='RAMå ç¨ç', content='${ram_percent}' ), Property.Item
 ( label='SWAPå ç¨ç', content='${swap_percent}', ), ] )] )
 """æäº¤è®°å½æ¨¡æ¿""" record_table = CRUD(mode='table', title='',
-syncLocation=False, api='/TeenStudy/api/get_records', interval=12000,
+syncLocation=False, api='/TeenStudy/api/get_records', interval=60000,
 type='crud', headerToolbar=[ActionType.Ajax(label='å é¤æææäº¤è®°å½',
 level=LevelEnum.warning, confirmText='ç¡®å®è¦å é¤æææäº¤è®°å½åï¼',
 api='delete:/TeenStudy/api/delete_all?type=records'), "bulkActions", "reload"],
 itemActions=[ ActionType.Ajax(tooltip='å é¤', icon='fa fa-times text-danger',
 confirmText='å é¤è¯¥æ¡æäº¤è®°å½', api='delete:/TeenStudy/api/
 delete_record?id=${id}') ], footable=True, columns=[ TableColumn
 (label='ç¨æ·ID', name='user_id', searchable=True), TableColumn
@@ -41,17 +41,17 @@
 (label='æäº¤ææ°', name='catalogue', searchable=True), TableColumn
 (label='æäº¤ç¶æ', name='${status==true?"æå":"å¤±è´¥"}',
 searchable=True), TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:
 mm\\:ss}', label='æäº¤æ¶é´', name='time', sortable=True) ], bulkActions=
 [ ActionType.Ajax(label='æ¹éå é¤', level=LevelEnum.warning,
 confirmText="ç¡®å®è¦æ¹éå é¤ï¼", api="delete:/TeenStudy/api/
 delete_records?ids=${ids|raw}")]) answer_table = CRUD(mode='table', title='',
-syncLocation=False, api='/TeenStudy/api/get_answers', interval=12000,
-type='crud', headerToolbar=[ActionType.Ajax
-(label='å é¤éå¹´å¤§å­¦ä¹ ææ°', level=LevelEnum.warning,
+syncLocation=False, api='/TeenStudy/api/get_answers', type='crud',
+headerToolbar=[ActionType.Ajax(label='å é¤éå¹´å¤§å­¦ä¹ ææ°',
+level=LevelEnum.warning,
 confirmText='ç¡®å®è¦å é¤éå¹´å¤§å­¦ä¹ ææ°åï¼', api='delete:/
 TeenStudy/api/delete_all?type=answers'), "bulkActions", "reload"], itemActions=
 [ ActionType.Ajax(tooltip='å é¤', icon='fa fa-times text-danger',
 confirmText='å é¤è¯¥æéå¹´å¤§å­¦ä¹ ', api='delete:/TeenStudy/api/
 delete_answer?id=${id}') ], footable=True, columns=[ TableColumn
 (label='æ°æ®åºID', name='id'), TableColumn(label='å¤§å­¦ä¹ ID',
 name='code'), TableColumn(label='å¤§å­¦ä¹ ææ°', name='catalogue',
@@ -91,26 +91,27 @@
 label="å¬ç½è®¿é®IP", value="${DXX_IP}",
 description="å¬ç½è®¿é®IPï¼ç¨äºå¤ç½è®¿é®", showCounter=True,
 trimContents=True, resetValue="0.0.0.0", required=True, clearable=True ),
 InputNumber( name="DXX_PORT", displayMode="enhance",
 label="å¬ç½è®¿é®ç«¯å£", value="${DXX_PORT}", min=0, max=65535,
 description="å¬ç½è®¿é®ç«¯å£ï¼ç¨äºå¤ç½è®¿é®ï¼ä¸éç½®åååååä»£çè¯·å¿ä¿®æ¹",
 showCounter=True, trimContents=True, resetValue=8080, required=True,
-clearable=True ), Switch( name="POKE_SUBMIT",
-label="æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³", value="${POKE_SUBMIT}",
-onText='å¼å¯', offText='å³é­', required=True, ), Switch( name="DXX_REMIND",
-label="å¤§å­¦ä¹ æéå¼å³", value="${DXX_REMIND}", onText='å¼å¯',
-offText='å³é­', required=True, ), InputTime( name="remind",
+clearable=True ), Switch( name="URL_STATUS", label="äºç»´ç è½¬é¾æ¥å¼å³",
+value="${URL_STATUS}", onText='å¼å¯', offText='å³é­', required=True, ),
+Switch( name="POKE_SUBMIT", label="æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³", value="$
+{POKE_SUBMIT}", onText='å¼å¯', offText='å³é­', required=True, ), Switch
+( name="DXX_REMIND", label="å¤§å­¦ä¹ æéå¼å³", value="${DXX_REMIND}",
+onText='å¼å¯', offText='å³é­', required=True, ), InputTime( name="remind",
 label="æéæ¶é´", type="input-time", required=True, value="${remind}", ),
 Switch( name="AUTO_SUBMIT", label="å¤§å­¦ä¹ èªå¨æäº¤å¼å³", value="$
 {AUTO_SUBMIT}", onText='å¼å¯', offText='å³é­', required=True, ), InputTime
 ( name="auto", label="èªå¨æäº¤æ¶é´", type="input-time", required=True,
 value="${auto}", ), ] ) """ç³è¯·è®°å½æ¨¡æ¿""" request_table = CRUD
 (mode='table', title='', syncLocation=False, api='/TeenStudy/api/get_requests',
-interval=12000, type='crud', headerToolbar=[ActionType.Ajax
+interval=60000, type='crud', headerToolbar=[ActionType.Ajax
 (label='å é¤ææç³è¯·è®°å½', level=LevelEnum.warning,
 confirmText='ç¡®å®è¦å é¤ææç³è¯·è®°å½åï¼', api='delete:/TeenStudy/
 api/delete_all?type=requests'), "bulkActions", "reload"], itemActions=
 [ ActionType.Ajax(tooltip='å é¤', icon='fa fa-times text-danger',
 confirmText='å é¤è¯¥æ¡ç³è¯·è®°å½', api='delete:/TeenStudy/api/
 delete_request?id=${id}') ], footable=True, columns=[ TableColumn
 (label='ç³è¯·ID', name='user_id', searchable=True), TableColumn
@@ -145,15 +146,15 @@
 description='å¾®ä¿¡è®¤è¯IDï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='ç»å½å¯ç ', name='Password', value='', type="input-password",
 trimContents=True, clearable=True, showCounter=True, maxLength=16, visibleOn="$
 {password==null?false:true}", description='ç»å½Web UIçå¯ç '), InputText
 (label='å­¦æ ¡ç±»å', name='university_type', value='${university_type}',
 showCounter=True, maxLength=16, required=True, trimContents=True,
 clearable=True, visibleOn="${university_type==null?false:true}",
-description='åå·å°åºå­¦æ ¡ç±»åï¼ä¸æ¸æ¥æ¸æ æ¹å¨'), InputText
+description='å­¦æ ¡ç±»åï¼ä¸æ¸æ¥æ¸æ æ¹å¨'), InputText
 (label='å­¦æ ¡ID', name='university_id', value='${university_id}',
 required=True, trimContents=True, clearable=True, showCounter=True,
 maxLength=24, visibleOn="${university_id==null?false:true}",
 description='å­¦æ ¡IDï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='å­¦æ ¡åç§°', name='university', value='${university}', required=True,
 trimContents=True, clearable=True, showCounter=True, maxLength=20, visibleOn="$
 {university==null?false:true}", description='å­¦æ ¡åç§°'), InputText
@@ -522,17 +523,43 @@
 description="å¯ä¸å¡«ï¼é»è®¤ä¸ºç¨æ·ID", name="password", inline=False,
 required=False, value="", clearable=True, maxLength=16 ), InputText
 ( label="å§å", description="å¯¹åºéåºå±éå¢ä¸ªäººä¿¡æ¯é¡µ
 æ¨çå§å", name="name", inline=False, required=True, value="",
 clearable=True, maxLength=8 ), InputText( label="openid",
 description="èªè¡æåè·åï¼ç»æä¸º: ohz9xxxxxxxxxxxxlF0Io0uCnM",
 name="openid", inline=False, required=True, value="", clearable=True, ) ] )
-"""æ¨éç¾¤èæ¨¡æ¿""" push_table = CRUD(mode='table', title='',
-syncLocation=False, api='/TeenStudy/api/get_push_list', interval=12000,
-type='crud', headerToolbar=[ActionType.Ajax(label='å é¤æææ¨éç¾¤è',
+"""åææ·»å æåé¢æ¿""" jilin_table = Form( title="åéé£æ¬",
+mode=DisplayModeEnum.horizontal, api="post:/TeenStudy/api/jilin/add",
+redirect="/TeenStudy/login", body=[ Select( label="ç¾¤è", name="group_id",
+description="éè¦æ·»å çç¾¤ç»", checkAll=False, source="get:/TeenStudy/
+api/get_group_list", value='', multiple=False, required=True, searchable=True,
+joinValues=False, extractValue=True, statistics=True, ), Select
+( label="ç¨æ·ID", name="user_id", description="éè¦æ·»å çç¨æ·ID",
+checkAll=False, source="get:/TeenStudy/api/get_member_list?group_id=$
+{group_id}", value='', multiple=False, required=True, searchable=True,
+joinValues=False, extractValue=True, statistics=True, hiddenOn="$
+{group_id==''?true:false}" ), InputText( label="å°åº",
+description="æå¤çä»½", name="area", value="åæ", disabled=True ),
+InputText( label="ç»å½å¯ç ", type='input-password',
+description="å¯ä¸å¡«ï¼é»è®¤ä¸ºç¨æ·ID", name="password", inline=False,
+required=False, value="", clearable=True, maxLength=16 ), InputText
+( label="å§å", description="æ¨çå§å", name="name", inline=False,
+required=True, value="", clearable=True, maxLength=8 ), InputText
+( label="openid", description="èªè¡æåè·åï¼ç»æä¸º:
+ohz9xxxxxxxxxxxxlF0Io0uCnM", name="openid", inline=False, required=True,
+value="", clearable=True, ), InputText( label="å­¦æ ¡",
+description="ä½ å°±è¯»çé«æ ¡", name="university", inline=False,
+required=True, value="", clearable=True, maxLength=24 ), InputText
+( label="å­¦é¢", description="å­¦é¢åç§°", name="college", inline=False,
+required=True, value="", clearable=True, maxLength=32 ), InputText
+( label="å¢æ¯é¨", description="å¢æ¯é¨|ç­çº§ï¼æ²¡æå¯ä¸å¡«",
+name="organization", inline=False, required=False, value="", clearable=True,
+maxLength=32 ) ] ) """æ¨éç¾¤èæ¨¡æ¿""" push_table = CRUD(mode='table',
+title='', syncLocation=False, api='/TeenStudy/api/get_push_list', type='crud',
+headerToolbar=[ActionType.Ajax(label='å é¤æææ¨éç¾¤è',
 level=LevelEnum.warning, confirmText='ç¡®å®è¦å é¤æææ¨éç¾¤èåï¼',
 api='delete:/TeenStudy/api/delete_all?type=push_list'), "bulkActions",
 "reload", ActionType.Dialog( label='æ·»å æ¨éç¾¤è', level=LevelEnum.info,
 icon='fa fa-plus', dialog=Dialog(title='æ·»å æ¨éç¾¤è', size='lg', body=
 [ Form(title='', api='post:/TeenStudy/api/add_push', submitText='æ·»å ',
 mode=DisplayModeEnum.horizontal, labelAlign='right', body=[Select
 ( label="ç¾¤è", name="groups", description="éè¦æ¨éçç¾¤ç»",
@@ -565,22 +592,25 @@
 pen-to-square', label='å®å¾½å±éå¢', schema=Page(title='å®å¾½å±éå¢',
 body=[anhui_table])) sichuan_page = PageSchema(url='/add/sichuan', icon='fa fa-
 pen-to-square', label='å¤©åºæ°éå¹´', schema=Page(title='å¤©åºæ°éå¹´',
 body=[sichuan_table])) shandong_page = PageSchema(url='/add/shandong', icon='fa
 fa-pen-to-square', label='éæ¥å±±ä¸', schema=Page(title='éæ¥å±±ä¸',
 body=[shandong_table])) chongqing_page = PageSchema(url='/add/chongqing',
 icon='fa fa-pen-to-square', label='éåºå±éå¢', schema=Page
-(title='éåºå±éå¢', body=[chongqing_table])) admin_app = App
+(title='éåºå±éå¢', body=[chongqing_table])) jilin_page = PageSchema
+(url='/add/jilin', icon='fa fa-pen-to-square', label='åéé£æ¬',
+schema=Page(title='åéé£æ¬', body=[jilin_table])) admin_app = App
 (brandName='TeenStudy', logo='https://i.328888.xyz/2023/02/23/xIh5k.png',
 header=header, pages=[{ 'children': [ admin_page, PageSchema(icon='fa fa-
 circle-user', label='æåç®¡ç', children=[list_page, hubei_page,
 jiangxi_page, jiangsu_page, anhui_page, sichuan_page, shandong_page,
-chongqing_page]), PageSchema(url="/notice", label='æ¨éåè¡¨', icon='fa fa-
-bell', schema=Page(title='', body=[push_table])), PageSchema(url="/request",
-label='ç³è¯·è®°å½', icon='fa fa-circle-info', schema=Page(title='', body=
-[request_table])), PageSchema(url="/answer", label='å¤§å­¦ä¹ åè¡¨', icon='fa
-fa-book-open', schema=Page(title='', body=[answer_table])), PageSchema(url="/
-records", label='æäº¤è®°å½', icon='fa fa-code-commit', schema=Page(title='',
-body=[record_table])), PageSchema(url="/setting", label='éç½®', icon='fa fa-
-gear', schema=Page(title='', body=[setting_table])), ]}], footer=Html( html=f'
+chongqing_page, jilin_page]), PageSchema(url="/notice", label='æ¨éåè¡¨',
+icon='fa fa-bell', schema=Page(title='', body=[push_table])), PageSchema(url="/
+request", label='ç³è¯·è®°å½', icon='fa fa-circle-info', schema=Page(title='',
+body=[request_table])), PageSchema(url="/answer", label='å¤§å­¦ä¹ åè¡¨',
+icon='fa fa-book-open', schema=Page(title='', body=[answer_table])), PageSchema
+(url="/records", label='æäº¤è®°å½', icon='fa fa-code-commit', schema=Page
+(title='', body=[record_table])), PageSchema(url="/setting", label='éç½®',
+icon='fa fa-gear', schema=Page(title='', body=[setting_table])), ]}],
+footer=Html( html=f'
 Copyright Â© 2022 - 2023 TeenStudy Xamis_v2.2.0
 '))
```

### Comparing `TeenStudy-0.1.6/TeenStudy/web/pages/home.py` & `TeenStudy-0.1.7/TeenStudy/web/pages/home.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                                             trimContents=True, clearable=True,
                                             showCounter=True, maxLength=16, visibleOn="${password==null?false:true}",
                                             description='登录Web UI的密码'),
                                   InputText(label='学校类型', name='university_type', value='${university_type}',
                                             showCounter=True, maxLength=16, required=True, trimContents=True,
                                             clearable=True,
                                             visibleOn="${university_type==null?false:true}",
-                                            description='四川地区学校类型，不清楚清无改动'),
+                                            description='学校类型，不清楚清无改动'),
                                   InputText(label='学校ID', name='university_id', value='${university_id}',
                                             required=True, trimContents=True, clearable=True,
                                             showCounter=True, maxLength=24,
                                             visibleOn="${university_id==null?false:true}",
                                             description='学校ID，不清楚请勿改动'),
                                   InputText(label='学校名称', name='university', value='${university}', required=True,
                                             trimContents=True, clearable=True,
@@ -235,15 +235,14 @@
     ]
 )
 """提交记录模板"""
 record_table = CRUD(mode='table',
                     title='',
                     syncLocation=False,
                     api='/TeenStudy/api/get_records?user_id=${user_id}',
-                    interval=12000,
                     type='crud',
                     headerToolbar=[],
                     itemActions=[],
                     footable=True,
                     columns=[
                         TableColumn(label='用户ID', name='user_id'),
                         TableColumn(label='姓名', name='name'),
@@ -257,15 +256,14 @@
                                     label='提交时间',
                                     name='time', sortable=True)
                     ])
 answer_table = CRUD(mode='table',
                     title='',
                     syncLocation=False,
                     api='/TeenStudy/api/get_answers',
-                    interval=12000,
                     type='crud',
                     headerToolbar=[],
                     itemActions=[],
                     footable=True,
                     columns=[
                         TableColumn(label='数据库ID', name='id'),
                         TableColumn(label='大学习ID', name='code'),
```

#### html2text {}

```diff
@@ -31,15 +31,15 @@
 description='å¾®ä¿¡è®¤è¯IDï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='ç»å½å¯ç ', name='Password', value='', type="input-password",
 trimContents=True, clearable=True, showCounter=True, maxLength=16, visibleOn="$
 {password==null?false:true}", description='ç»å½Web UIçå¯ç '), InputText
 (label='å­¦æ ¡ç±»å', name='university_type', value='${university_type}',
 showCounter=True, maxLength=16, required=True, trimContents=True,
 clearable=True, visibleOn="${university_type==null?false:true}",
-description='åå·å°åºå­¦æ ¡ç±»åï¼ä¸æ¸æ¥æ¸æ æ¹å¨'), InputText
+description='å­¦æ ¡ç±»åï¼ä¸æ¸æ¥æ¸æ æ¹å¨'), InputText
 (label='å­¦æ ¡ID', name='university_id', value='${university_id}',
 required=True, trimContents=True, clearable=True, showCounter=True,
 maxLength=24, visibleOn="${university_id==null?false:true}",
 description='å­¦æ ¡IDï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='å­¦æ ¡åç§°', name='university', value='${university}', required=True,
 trimContents=True, clearable=True, showCounter=True, maxLength=20, visibleOn="$
 {university==null?false:true}", description='å­¦æ ¡åç§°'), InputText
@@ -95,43 +95,42 @@
 Property.Item( label='å¢æ¯é¨ID', content='${organization_id}', visibleOn="$
 {organization_id==null?false:true}" ), Property.Item( label='openid',
 content='${openid}', visibleOn="${openid==null?false:true}" ), Property.Item
 ( label='token', content='${token}', visibleOn="${token==null?false:true}",
 span=2 ), Property.Item( label='cookie', content='${cookie}', visibleOn="$
 {cookie==null?false:true}", span=2 ) ] ) ] ) """æäº¤è®°å½æ¨¡æ¿"""
 record_table = CRUD(mode='table', title='', syncLocation=False, api='/
-TeenStudy/api/get_records?user_id=${user_id}', interval=12000, type='crud',
+TeenStudy/api/get_records?user_id=${user_id}', type='crud', headerToolbar=[],
+itemActions=[], footable=True, columns=[ TableColumn(label='ç¨æ·ID',
+name='user_id'), TableColumn(label='å§å', name='name'), TableColumn
+(label='æäº¤å°åº', name='area'), TableColumn(label='å­¦æ ¡åç§°',
+name='university'), TableColumn(label='å­¦é¢åç§°', name='college'),
+TableColumn(label='å¢æ¯é¨', name='organization'), TableColumn
+(label='æäº¤ææ°', name='catalogue', searchable=True), TableColumn
+(label='æäº¤ç¶æ', name='${status==true?"æå":"å¤±è´¥"}'), TableColumn
+(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='æäº¤æ¶é´',
+name='time', sortable=True) ]) answer_table = CRUD(mode='table', title='',
+syncLocation=False, api='/TeenStudy/api/get_answers', type='crud',
 headerToolbar=[], itemActions=[], footable=True, columns=[ TableColumn
-(label='ç¨æ·ID', name='user_id'), TableColumn(label='å§å', name='name'),
-TableColumn(label='æäº¤å°åº', name='area'), TableColumn
-(label='å­¦æ ¡åç§°', name='university'), TableColumn(label='å­¦é¢åç§°',
-name='college'), TableColumn(label='å¢æ¯é¨', name='organization'),
-TableColumn(label='æäº¤ææ°', name='catalogue', searchable=True),
-TableColumn(label='æäº¤ç¶æ', name='${status==true?"æå":"å¤±è´¥"}'),
-TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
-label='æäº¤æ¶é´', name='time', sortable=True) ]) answer_table = CRUD
-(mode='table', title='', syncLocation=False, api='/TeenStudy/api/get_answers',
-interval=12000, type='crud', headerToolbar=[], itemActions=[], footable=True,
-columns=[ TableColumn(label='æ°æ®åºID', name='id'), TableColumn
-(label='å¤§å­¦ä¹ ID', name='code'), TableColumn(label='å¤§å­¦ä¹ ææ°',
-name='catalogue', searchable=True), TableColumn(type='tpl', tpl='$
-{url|truncate:20}', label='å®æ¹ç½å', name='url', popOver={'mode':
-'dialog', 'title': 'å®æ´ç½å', 'className': 'break-all', 'body': {'type':
-'tpl', 'tpl': '${url}'}}, copyable=True), TableColumn(type='tpl', tpl='$
-{end_url|truncate:20}', label='å®ææªå¾ç½å', name='end_url', popOver=
-{'mode': 'dialog', 'title': 'å®æ´ç½å', 'className': 'break-all', 'body':
-{'type': 'tpl', 'tpl': '${end_url}'}}, copyable=True), TableColumn(type='tpl',
-tpl='${answer|truncate:20}', label='ç­æ¡', name='answer', popOver={'mode':
-'dialog', 'title': 'å®æ´ç­æ¡', 'className': 'break-all', 'body': {'type':
-'tpl', 'tpl': '${answer}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-MM-
-DD HH\\:mm\\:ss}', label='æ´æ°æ¶é´', name='time', sortable=True) ])
-page_detail = Page(title='', body=[logo, operation_button, Divider(),
-from_table]) home_page = PageSchema(url='/home', label='é¦é¡µ', icon='fa fa-
-home', isDefaultPage=True, schema=page_detail) home_app = App
-(brandName='TeenStudy', logo='https://i.328888.xyz/2023/02/23/xIh5k.png',
-header=header, pages=[{ 'children': [ home_page, PageSchema(url="answer",
-label='å¤§å­¦ä¹ åè¡¨', icon='fa fa-book-open', schema=Page(title='', body=
-[answer_table])), PageSchema(url="/records", label='æäº¤è®°å½', icon='fa fa-
-code-commit', schema=Page(title='', body=[record_table])) ]}], footer=Html
-( html=f'
+(label='æ°æ®åºID', name='id'), TableColumn(label='å¤§å­¦ä¹ ID',
+name='code'), TableColumn(label='å¤§å­¦ä¹ ææ°', name='catalogue',
+searchable=True), TableColumn(type='tpl', tpl='${url|truncate:20}',
+label='å®æ¹ç½å', name='url', popOver={'mode': 'dialog', 'title':
+'å®æ´ç½å', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
+{url}'}}, copyable=True), TableColumn(type='tpl', tpl='${end_url|truncate:20}',
+label='å®ææªå¾ç½å', name='end_url', popOver={'mode': 'dialog', 'title':
+'å®æ´ç½å', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
+{end_url}'}}, copyable=True), TableColumn(type='tpl', tpl='${answer|truncate:
+20}', label='ç­æ¡', name='answer', popOver={'mode': 'dialog', 'title':
+'å®æ´ç­æ¡', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
+{answer}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:
+ss}', label='æ´æ°æ¶é´', name='time', sortable=True) ]) page_detail = Page
+(title='', body=[logo, operation_button, Divider(), from_table]) home_page =
+PageSchema(url='/home', label='é¦é¡µ', icon='fa fa-home', isDefaultPage=True,
+schema=page_detail) home_app = App(brandName='TeenStudy', logo='https://
+i.328888.xyz/2023/02/23/xIh5k.png', header=header, pages=[{ 'children':
+[ home_page, PageSchema(url="answer", label='å¤§å­¦ä¹ åè¡¨', icon='fa fa-
+book-open', schema=Page(title='', body=[answer_table])), PageSchema(url="/
+records", label='æäº¤è®°å½', icon='fa fa-code-commit', schema=Page(title='',
+body=[record_table])) ]}], footer=Html( html=f'
 Copyright Â© 2022 - 2023 TeenStudy Xamis_v2.2.0
 '))
```

### Comparing `TeenStudy-0.1.6/TeenStudy/web/pages/login.py` & `TeenStudy-0.1.7/TeenStudy/web/pages/login.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/web/utils/add.py` & `TeenStudy-0.1.7/TeenStudy/web/utils/add.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/TeenStudy/web/utils/status.py` & `TeenStudy-0.1.7/TeenStudy/web/utils/status.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.6/setup.py` & `TeenStudy-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 
 package_data = \
 {'': ['*'], 'teenstudy': ['resource/*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
  'Pillow>=9.4.0,<10.0.0',
- 'amis-python>=1.0.6,<2.0.0',
+ 'amis-python>=1.0.7,<2.0.0',
  'anti-useragent>=1.0.10,<2.0.0',
  'beautifulsoup4>=4.11.2,<5.0.0',
  'bs4>=0.0.1,<0.0.2',
  'fastapi>=0.95.0,<0.96.0',
  'httpx>=0.23.3,<0.24.0',
  'lxml>=4.9.2,<5.0.0',
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
  'nonebot2>=2.0.0rc2,<3.0.0',
  'psutil>=5.9.4,<6.0.0',
  'python-jose>=3.3.0,<4.0.0',
  'qrcode>=7.4.2,<8.0.0',
  'tortoise-orm>=0.19.3,<0.20.0',
  'ujson>=5.7.0,<6.0.0',
- 'uvicorn>=0.20.0,<0.21.0']
+ 'uvicorn>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'teenstudy',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图',
-    'long_description': '<div align="center">\n    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>\n    <h1>TeenStudy</h1>\n    <b>基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>\n    <br/>\n    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>\n  \t<a href="https://pypi.python.org/pypi/TeenStudy">\n    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>\n     <a href="https://github.com/ZM25XC/TeenStudy">\n    <img src="https://visitor-badge.glitch.me/badge?page_id=https://github.com/ZM25XC/TeenStudy" alt="Teenstudy"></a>\n\t<a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  </div>\n\n## 说明\n\n- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版\n- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档\n-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**\n- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交\n- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常\n- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。\n- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试\n\n- 觉得项目不错，不妨点个stars.\n\n## 地区状态\n\n<details>\n\n| 共青团名称 | 开发状态 | 备注 |\n|:-----:|:----:|:----:|\n|青春湖北|支持|无需抓包|\n|江西共青团|支持|无需抓包|\n|青春上海|支持|微信扫码绑定|\n|青春浙江|支持|微信扫码绑定|\n|安徽共青团|支持|无需抓包|\n|江苏共青团|支持|需要自行抓包|\n|青春山东|支持|需要自行抓包|\n|重庆共青团|支持|需要自行抓包|\n|河南共青团|不支持|cookie时效小于1周|\n|天府新青年|支持|不进入公众号token时效大于1周|\n|黑龙江共青团|待开发||\n|广西青年圈|待开发||\n|青春湖南|待开发||\n|甘肃青年|待开发||\n|山西青年|待开发||\n|河北共青团|待开发||\n|福建共青团|待开发||\n|内蒙古青年|待开发||\n|云南共青团|待开发||\n|吉青飞扬|待开发||\n|三秦青年|待开发||\n|青春北京|待开发||\n|海南共青团|待开发||\n|津彩青春|待开发||\n|青春黔言|待开发||\n|广东共青团|待开发||\n|青春柳州|待开发||\n|辽宁共青团|待开发||\n|宁夏共青团|待开发||\n|新疆共青团|待开发||\n|西藏共青团|待开发||\n</details>\n\n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n1、使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新\n2、使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 TeenStudy\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`\n\n</details>\n\n## 机器人配置\n\n- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP\n\n  ```py\n  HOST = "0.0.0.0"  #nonebot2监听的IP\n  SUPERUSERS = [""] # 超级用户\n  COMMAND_START=[""] # 命令前缀,根据需要自行修改\n  DXX_IP = ""\n  ```\n\n## 使用方式\n\n- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）\n- 在管理后台的推送列表中添加需要开启大学习使用的群聊\n\n## 功能列表\n|    指令    |               指令格式               |                               说明                               |\n| :--------: | :----------------------------------: | :--------------------------------------------------------------: |\n| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |\n| 我的大学习 |              我的大学习              |                           查询个人信息                           |\n| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |\n|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |\n|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |\n| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |\n|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |\n|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |\n|删除大学习|删除大学习|用户申请清除数据库的信息|\n|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|\n|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|\n|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|\n\n\n## ToDo\n\n\n- [ ] 增加更多地区支持\n- [ ] 优化 Bot\n\n\n## 更新日志\n\n###2023/04/12\n- 因河南地区cookie时效小于1周，移除河南地区\n- 添加`删除大学习`功能，用户可自行删除数据\n- 添加`导出用户数据`功能\n- 添加`更新用户数据`功能\n- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据\n- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改\n- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改\n- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改\n- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法\n- 修复Web UI 首页公网IP显示异常\n- 修复浙江地区用户重复显示\n- 更新江西共青团团支部数据\n\n\n\n<details>\n<summary>2023/03/18</summary>\n\n- 适配河南地区，需要自行抓包\n- 适配四川地区，需要自行抓包\n- 适配山东地区，需要自行抓包\n- 适配重庆地区，需要自行抓包\n- 添加自动获取公网IP功能，别再问如何配置公网IP啦\n- 添加重置密码功能，指令`重置密码`\n- 添加重置配置功能，指令`重置配置`，`刷新配置`\n- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`\n- 管理后台开放添加用户权限（浙江，上海地区无法添加）\n- 优化用户信息页\n- 优化登录界面提示\n- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些\n- 修复Ubuntu系统导入资源失败BUG\n  \n</details>\n\n<details>\n\n<summary>2023/03/05</summary>\n\n- 适配浙江地区，使用微信扫码进行绑定\n- 适配上海地区，使用微信扫码进行绑定\n- 适配江苏地区，需要自行抓包\n- 适配安徽地区，需要自行抓包\n\n</details>\n\n<details>\n<summary>2023/03/01</summary>\n\n- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件\n- 上传基础代码\n- 适配湖北地区，无需抓包，安装即用\n- 适配江西地区，无需抓包，安装即用\n\n</details>',
+    'long_description': '<div align="center">\n    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>\n    <h1>TeenStudy</h1>\n    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>\n    <br/>\n    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>\n  \t<a href="https://pypi.python.org/pypi/TeenStudy">\n    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>\n\t  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  </div>\n\n## 说明\n\n- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版\n- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档\n-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**\n- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交\n- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常\n- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。\n- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试\n\n- 觉得项目不错，不妨点个stars.\n\n## 地区状态\n\n<details>\n\n| 共青团名称 | 开发状态 | 备注 |\n|:-----:|:----:|:----:|\n|青春湖北|支持|无需抓包|\n|江西共青团|支持|无需抓包|\n|安徽共青团|支持|无需抓包|\n|青春上海|支持|微信扫码绑定|\n|青春浙江|支持|微信扫码绑定|\n|江苏共青团|支持|需要自行抓包|\n|青春山东|支持|需要自行抓包|\n|重庆共青团|支持|需要自行抓包|\n|吉青飞扬|支持|需要自行抓包|\n|天府新青年|支持|不进入公众号token时效大于1周|\n|河南共青团|不支持|cookie时效小于1周|\n|黑龙江共青团|待开发||\n|广西青年圈|待开发||\n|青春湖南|待开发||\n|甘肃青年|待开发||\n|山西青年|待开发||\n|河北共青团|待开发||\n|福建共青团|待开发||\n|内蒙古青年|待开发||\n|云南共青团|待开发||\n|三秦青年|待开发||\n|青春北京|待开发||\n|海南共青团|待开发||\n|津彩青春|待开发||\n|青春黔言|待开发||\n|广东共青团|待开发||\n|青春柳州|待开发||\n|辽宁共青团|待开发||\n|宁夏共青团|待开发||\n|新疆共青团|待开发||\n|西藏共青团|待开发||\n</details>\n\n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n1、使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新\n2、使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 TeenStudy\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`\n\n</details>\n\n## 机器人配置\n\n- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP\n\n  ```py\n  HOST = "0.0.0.0"  #nonebot2监听的IP\n  SUPERUSERS = [""] # 超级用户\n  COMMAND_START=[""] # 命令前缀,根据需要自行修改\n  DXX_IP = ""\n  ```\n\n## 使用方式\n\n- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）\n- 在管理后台的推送列表中添加需要开启大学习使用的群聊\n\n## 功能列表\n|    指令    |               指令格式               |                               说明                               |\n| :--------: | :----------------------------------: | :--------------------------------------------------------------: |\n| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |\n| 我的大学习 |              我的大学习              |                           查询个人信息                           |\n| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |\n|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |\n|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |\n| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |\n|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |\n|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |\n|删除大学习|删除大学习|用户申请清除数据库的信息|\n|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|\n|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|\n|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|\n\n\n## ToDo\n\n\n- [ ] 增加更多地区支持\n- [ ] 优化 Bot\n\n\n## 更新日志\n\n### 2023/05/06\n\n- 增加吉林地区，需要自行抓包\n- 修复超管更改登录密码后用原密码能继续登录问题\n- 添加二维码转链接开关，需要自行在后台配置页面打开\n- 调整部分依赖\n\n\n<details>\n<summary> 2023/04/12</summary> \n\n- 因河南地区cookie时效小于1周，移除河南地区\n- 添加`删除大学习`功能，用户可自行删除数据\n- 添加`导出用户数据`功能\n- 添加`更新用户数据`功能\n- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据\n- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改\n- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改\n- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改\n- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法\n- 修复Web UI 首页公网IP显示异常\n- 修复浙江地区用户重复显示\n- 更新江西共青团团支部数据\n  \n</details>\n\n\n<details>\n<summary>2023/03/18</summary>\n\n- 适配河南地区，需要自行抓包\n- 适配四川地区，需要自行抓包\n- 适配山东地区，需要自行抓包\n- 适配重庆地区，需要自行抓包\n- 添加自动获取公网IP功能，别再问如何配置公网IP啦\n- 添加重置密码功能，指令`重置密码`\n- 添加重置配置功能，指令`重置配置`，`刷新配置`\n- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`\n- 管理后台开放添加用户权限（浙江，上海地区无法添加）\n- 优化用户信息页\n- 优化登录界面提示\n- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些\n- 修复Ubuntu系统导入资源失败BUG\n  \n</details>\n\n<details>\n\n<summary>2023/03/05</summary>\n\n- 适配浙江地区，使用微信扫码进行绑定\n- 适配上海地区，使用微信扫码进行绑定\n- 适配江苏地区，需要自行抓包\n- 适配安徽地区，需要自行抓包\n\n</details>\n\n<details>\n<summary>2023/03/01</summary>\n\n- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件\n- 上传基础代码\n- 适配湖北地区，无需抓包，安装即用\n- 适配江西地区，无需抓包，安装即用\n\n</details>\n',
     'author': 'ZM25XC',
     'author_email': 'xingling25@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ZM25XC/TeenStudy',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,42 +1,42 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['teenstudy',
 'teenstudy.models', 'teenstudy.utils', 'teenstudy.web', 'teenstudy.web.api',
 'teenstudy.web.pages', 'teenstudy.web.utils'] package_data = \ {'': ['*'],
 'teenstudy': ['resource/*']} install_requires = \ ['Jinja2>=3.1.2,<4.0.0',
-'Pillow>=9.4.0,<10.0.0', 'amis-python>=1.0.6,<2.0.0', 'anti-
+'Pillow>=9.4.0,<10.0.0', 'amis-python>=1.0.7,<2.0.0', 'anti-
 useragent>=1.0.10,<2.0.0', 'beautifulsoup4>=4.11.2,<5.0.0',
 'bs4>=0.0.1,<0.0.2', 'fastapi>=0.95.0,<0.96.0', 'httpx>=0.23.3,<0.24.0',
 'lxml>=4.9.2,<5.0.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0', 'nonebot-plugin-
 apscheduler>=0.2.0,<0.3.0', 'nonebot2>=2.0.0rc2,<3.0.0',
 'psutil>=5.9.4,<6.0.0', 'python-jose>=3.3.0,<4.0.0', 'qrcode>=7.4.2,<8.0.0',
 'tortoise-orm>=0.19.3,<0.20.0', 'ujson>=5.7.0,<6.0.0',
-'uvicorn>=0.20.0,<0.21.0'] setup_kwargs = { 'name': 'teenstudy', 'version':
-'0.1.6', 'description':
+'uvicorn>=0.21.0,<0.22.0'] setup_kwargs = { 'name': 'teenstudy', 'version':
+'0.1.7', 'description':
 'åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾',
 'long_description': '
                              \n [TeenStudy.png]\n
                             ****** TeenStudy ******
-                                      \n
-åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾\n
+                            \n åºäºnonebot2ågo-
+cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾\n
 
   \n [GitHub_issues]\n [GitHub_forks]\n [GitHub_stars]\n [pypi]\n \t\n_[pypi
-    download]\n \n_[Teenstudy]\n\t[GitHub_license]\n \n_[QQ_Chat_Group]\n\n
+            download]\n\t [GitHub_license]\n \n_[QQ_Chat_Group]\n\n
 \n\n## è¯´æ\n\n- æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/
 ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`ç\n- æ¬é¡¹ç®åºäº[nonebot2]
 (https://github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/
 go-cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£\n-
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**\n-
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤\n-
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸\n-
 æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/
 ?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã\n-
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯\n\n-
 è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars.\n\n## å°åºç¶æ\n\n\n\n|
 å±éå¢åç§° | å¼åç¶æ | å¤æ³¨ |\n|:-----:|:----:|:----:
-|\n|éæ¥æ¹å|æ¯æ|æ éæå|\n|æ±è¥¿å±éå¢|æ¯æ|æ éæå|\n|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|å®å¾½å±éå¢|æ¯æ|æ éæå|\n|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|\n|éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|\n|éåºå±éå¢|æ¯æ|éè¦èªè¡æå|\n|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|\n|å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|\n|é»é¾æ±å±éå¢|å¾å¼å||\n|å¹¿è¥¿éå¹´å|å¾å¼å||\n|éæ¥æ¹å|å¾å¼å||\n|çèéå¹´|å¾å¼å||\n|å±±è¥¿éå¹´|å¾å¼å||\n|æ²³åå±éå¢|å¾å¼å||\n|ç¦å»ºå±éå¢|å¾å¼å||\n|åèå¤éå¹´|å¾å¼å||\n|äºåå±éå¢|å¾å¼å||\n|åéé£æ¬|å¾å¼å||\n|ä¸ç§¦éå¹´|å¾å¼å||\n|éæ¥åäº¬|å¾å¼å||\n|æµ·åå±éå¢|å¾å¼å||\n|æ´¥å½©éæ¥|å¾å¼å||\n|éæ¥é»è¨|å¾å¼å||\n|å¹¿ä¸å±éå¢|å¾å¼å||\n|éæ¥æ³å·|å¾å¼å||\n|è¾½å®å±éå¢|å¾å¼å||\n|å®å¤å±éå¢|å¾å¼å||\n|æ°çå±éå¢|å¾å¼å||\n|è¥¿èå±éå¢|å¾å¼å||\n\n\n\n##
+|\n|éæ¥æ¹å|æ¯æ|æ éæå|\n|æ±è¥¿å±éå¢|æ¯æ|æ éæå|\n|å®å¾½å±éå¢|æ¯æ|æ éæå|\n|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|\n|éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|\n|éåºå±éå¢|æ¯æ|éè¦èªè¡æå|\n|åéé£æ¬|æ¯æ|éè¦èªè¡æå|\n|å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|\n|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|\n|é»é¾æ±å±éå¢|å¾å¼å||\n|å¹¿è¥¿éå¹´å|å¾å¼å||\n|éæ¥æ¹å|å¾å¼å||\n|çèéå¹´|å¾å¼å||\n|å±±è¥¿éå¹´|å¾å¼å||\n|æ²³åå±éå¢|å¾å¼å||\n|ç¦å»ºå±éå¢|å¾å¼å||\n|åèå¤éå¹´|å¾å¼å||\n|äºåå±éå¢|å¾å¼å||\n|ä¸ç§¦éå¹´|å¾å¼å||\n|éæ¥åäº¬|å¾å¼å||\n|æµ·åå±éå¢|å¾å¼å||\n|æ´¥å½©éæ¥|å¾å¼å||\n|éæ¥é»è¨|å¾å¼å||\n|å¹¿ä¸å±éå¢|å¾å¼å||\n|éæ¥æ³å·|å¾å¼å||\n|è¾½å®å±éå¢|å¾å¼å||\n|å®å¤å±éå¢|å¾å¼å||\n|æ°çå±éå¢|å¾å¼å||\n|è¥¿èå±éå¢|å¾å¼å||\n\n\n\n##
 å®è£åæ´æ°\n\n\nç¬¬ä¸ç§æ¹å¼(ä¸æ¨è)\n\n- ä½¿ç¨`git clone https://
 github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶\n\n\n\n\nç¬¬äºç§æ¹å¼
 (äºéä¸)\n\n1ãä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip
 install TeenStudy -U`è¿è¡æ´æ°\n2ãä½¿ç¨`nb plugin install
 TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`nb plugin install TeenStudy -
 U`è¿è¡æ´æ°\n\n\n\n\n##
@@ -68,29 +68,32 @@
 å®æå¤§å­¦ä¹  | å®æå¤§å­¦ä¹ ãå¨åå¤§å­¦ä¹  |
 å¢æ¯ä¹¦å¯ç¨ï¼éè¦æåå¡«åå¢æ¯ä¹¦IDï¼å¡«ååå¢æ¯ä¹¦å¯åæä»¤æäº¤å¤§å­¦ä¹ 
 |\n| éç½®éç½® | éç½®éç½®ãå·æ°éç½® | è¶ç®¡å¯ç¨ï¼å·æ°Web
 UIé»è®¤éç½® |\n| éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID
 |\n|å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|\n|å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|\n|æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|\n|æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|\n\n\n##
 ToDo\n\n\n- [ ] å¢å æ´å¤å°åºæ¯æ\n- [ ] ä¼å Bot\n\n\n##
-æ´æ°æ¥å¿\n\n###2023/04/12\n-
+æ´æ°æ¥å¿\n\n### 2023/05/06\n\n- å¢å åæå°åºï¼éè¦èªè¡æå\n-
+ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢\n-
+æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼\n-
+è°æ´é¨åä¾èµ\n\n\n\n 2023/04/12 \n\n-
 å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº\n-
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ®\n-
 æ·»å `å¯¼åºç¨æ·æ°æ®`åè½\n- æ·»å `æ´æ°ç¨æ·æ°æ®`åè½\n-
 æ·»å `æ´æ°èµæºæ°æ®`åè½ï¼æ±è¥¿å°åºæ´æ°åè¯·ä½¿ç¨ä¸æ­¤åè½å·æ°å¢æ¯é¨æ°æ®\n-
 æ·»å æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹\n-
 æ·»å å¤§å­¦ä¹ æéå¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹\n-
 æ·»å èªå¨æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
 UIåå°è¿è¡ä¿®æ¹\n- è°æ´å®å¾½å°åºæ·»å æ¹å¼[#9](https://github.com/
 ZM25XC/TeenStudy/issues/9)ï¼æ éæåï¼æè°¢[@yhzcake](https://
 github.com/yhzcake)æµè¯æä¾æ¹æ³\n- ä¿®å¤Web UI
 é¦é¡µå¬ç½IPæ¾ç¤ºå¼å¸¸\n- ä¿®å¤æµæ±å°åºç¨æ·éå¤æ¾ç¤º\n-
-æ´æ°æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®\n\n\n\n\n2023/03/18\n\n-
+æ´æ°æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®\n \n\n\n\n\n2023/03/18\n\n-
 ééæ²³åå°åºï¼éè¦èªè¡æå\n-
 ééåå·å°åºï¼éè¦èªè¡æå\n-
 ééå±±ä¸å°åºï¼éè¦èªè¡æå\n-
 éééåºå°åºï¼éè¦èªè¡æå\n-
 æ·»å èªå¨è·åå¬ç½IPåè½ï¼å«åé®å¦ä½éç½®å¬ç½IPå¦\n-
 æ·»å éç½®å¯ç åè½ï¼æä»¤`éç½®å¯ç `\n-
 æ·»å éç½®éç½®åè½ï¼æä»¤`éç½®éç½®`ï¼`å·æ°éç½®`\n-
@@ -102,12 +105,12 @@
 ééæµæ±å°åºï¼ä½¿ç¨å¾®ä¿¡æ«ç è¿è¡ç»å®\n-
 ééä¸æµ·å°åºï¼ä½¿ç¨å¾®ä¿¡æ«ç è¿è¡ç»å®\n-
 ééæ±èå°åºï¼éè¦èªè¡æå\n-
 ééå®å¾½å°åºï¼éè¦èªè¡æå\n\n\n\n\n2023/03/01\n\n-
 å°ä»£ç ä¸ä¼ è³pypiï¼å¯ä½¿ç¨`pip install
 TeenStudy`æä»¤å®è£æ¬æä»¶\n- ä¸ä¼ åºç¡ä»£ç \n-
 ééæ¹åå°åºï¼æ éæåï¼å®è£å³ç¨\n-
-ééæ±è¥¿å°åºï¼æ éæåï¼å®è£å³ç¨\n\n', 'author': 'ZM25XC',
+ééæ±è¥¿å°åºï¼æ éæåï¼å®è£å³ç¨\n\n\n', 'author': 'ZM25XC',
 'author_email': 'xingling25@qq.com', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'https://github.com/ZM25XC/TeenStudy', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `TeenStudy-0.1.6/PKG-INFO` & `TeenStudy-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 Metadata-Version: 2.1
 Name: teenstudy
-Version: 0.1.6
+Version: 0.1.7
 Summary: 基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图
 Home-page: https://github.com/ZM25XC/TeenStudy
 License: MIT
 Author: ZM25XC
 Author-email: xingling25@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: Pillow (>=9.4.0,<10.0.0)
-Requires-Dist: amis-python (>=1.0.6,<2.0.0)
+Requires-Dist: amis-python (>=1.0.7,<2.0.0)
 Requires-Dist: anti-useragent (>=1.0.10,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: tortoise-orm (>=0.19.3,<0.20.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
-Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
+Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
     <h1>TeenStudy</h1>
-    <b>基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
+    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
     <br/>
     <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>
   	<a href="https://pypi.python.org/pypi/TeenStudy">
     <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>
-     <a href="https://github.com/ZM25XC/TeenStudy">
-    <img src="https://visitor-badge.glitch.me/badge?page_id=https://github.com/ZM25XC/TeenStudy" alt="Teenstudy"></a>
-	<a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
+	  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">
     <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">
   </a>
   </div>
 
 ## 说明
 
@@ -67,32 +65,32 @@
 
 <details>
 
 | 共青团名称 | 开发状态 | 备注 |
 |:-----:|:----:|:----:|
 |青春湖北|支持|无需抓包|
 |江西共青团|支持|无需抓包|
+|安徽共青团|支持|无需抓包|
 |青春上海|支持|微信扫码绑定|
 |青春浙江|支持|微信扫码绑定|
-|安徽共青团|支持|无需抓包|
 |江苏共青团|支持|需要自行抓包|
 |青春山东|支持|需要自行抓包|
 |重庆共青团|支持|需要自行抓包|
-|河南共青团|不支持|cookie时效小于1周|
+|吉青飞扬|支持|需要自行抓包|
 |天府新青年|支持|不进入公众号token时效大于1周|
+|河南共青团|不支持|cookie时效小于1周|
 |黑龙江共青团|待开发||
 |广西青年圈|待开发||
 |青春湖南|待开发||
 |甘肃青年|待开发||
 |山西青年|待开发||
 |河北共青团|待开发||
 |福建共青团|待开发||
 |内蒙古青年|待开发||
 |云南共青团|待开发||
-|吉青飞扬|待开发||
 |三秦青年|待开发||
 |青春北京|待开发||
 |海南共青团|待开发||
 |津彩青春|待开发||
 |青春黔言|待开发||
 |广东共青团|待开发||
 |青春柳州|待开发||
@@ -191,28 +189,39 @@
 
 - [ ] 增加更多地区支持
 - [ ] 优化 Bot
 
 
 ## 更新日志
 
-###2023/04/12
+### 2023/05/06
+
+- 增加吉林地区，需要自行抓包
+- 修复超管更改登录密码后用原密码能继续登录问题
+- 添加二维码转链接开关，需要自行在后台配置页面打开
+- 调整部分依赖
+
+
+<details>
+<summary> 2023/04/12</summary> 
+
 - 因河南地区cookie时效小于1周，移除河南地区
 - 添加`删除大学习`功能，用户可自行删除数据
 - 添加`导出用户数据`功能
 - 添加`更新用户数据`功能
 - 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据
 - 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改
 - 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改
 - 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改
 - 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法
 - 修复Web UI 首页公网IP显示异常
 - 修复浙江地区用户重复显示
 - 更新江西共青团团支部数据
-
+  
+</details>
 
 
 <details>
 <summary>2023/03/18</summary>
 
 - 适配河南地区，需要自行抓包
 - 适配四川地区，需要自行抓包
@@ -246,7 +255,8 @@
 
 - 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件
 - 上传基础代码
 - 适配湖北地区，无需抓包，安装即用
 - 适配江西地区，无需抓包，安装即用
 
 </details>
+
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: teenstudy Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: teenstudy Version: 0.1.7 Summary:
 åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 Home-page: https://github.com/ZM25XC/TeenStudy License: MIT Author: ZM25XC
 Author-email: xingling25@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: Pillow (>=9.4.0,<10.0.0)
-Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist: anti-useragent
+Requires-Dist: amis-python (>=1.0.7,<2.0.0) Requires-Dist: anti-useragent
 (>=1.0.10,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-
 Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: fastapi (>=0.95.0,<0.96.0) Requires-
 Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot-plugin-
 apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0) Requires-Dist: python-jose
 (>=3.3.0,<4.0.0) Requires-Dist: qrcode (>=7.4.2,<8.0.0) Requires-Dist:
 tortoise-orm (>=0.19.3,<0.20.0) Requires-Dist: ujson (>=5.7.0,<6.0.0) Requires-
-Dist: uvicorn (>=0.20.0,<0.21.0) Description-Content-Type: text/markdown
+Dist: uvicorn (>=0.21.0,<0.22.0) Description-Content-Type: text/markdown
                                 [TeenStudy.png]
                             ****** TeenStudy ******
-åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
+                             åºäºnonebot2ågo-
+cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 
-     [GitHub_issues] [GitHub_forks] [GitHub_stars] [pypi] [pypi_download]
-                 [Teenstudy] [GitHub_license] [QQ_Chat_Group]
+ [GitHub_issues] [GitHub_forks] [GitHub_stars] [pypi] [pypi_download] [GitHub
+                           license] [QQ_Chat_Group]
 ## è¯´æ - æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/ZM25XC/
 nonebot_plugin_auto_teenstudy) `Web UI`ç - æ¬é¡¹ç®åºäº[nonebot2](https://
 github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£ -
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**
 -
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤
@@ -33,26 +34,27 @@
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸
 - æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã
 -
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯
 - è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars. ## å°åºç¶æ  | å±éå¢åç§° |
 å¼åç¶æ | å¤æ³¨ | |:-----:|:----:|:----:
 | |éæ¥æ¹å|æ¯æ|æ éæå| |æ±è¥¿å±éå¢|æ¯æ|æ éæå|
-|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
-|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®| |å®å¾½å±éå¢|æ¯æ|æ éæå|
+|å®å¾½å±éå¢|æ¯æ|æ éæå| |éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|
 |éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|
 |éåºå±éå¢|æ¯æ|éè¦èªè¡æå|
-|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
+|åéé£æ¬|æ¯æ|éè¦èªè¡æå|
 |å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|
+|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
 |é»é¾æ±å±éå¢|å¾å¼å|| |å¹¿è¥¿éå¹´å|å¾å¼å||
 |éæ¥æ¹å|å¾å¼å|| |çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
 |æ²³åå±éå¢|å¾å¼å|| |ç¦å»ºå±éå¢|å¾å¼å||
 |åèå¤éå¹´|å¾å¼å|| |äºåå±éå¢|å¾å¼å||
-|åéé£æ¬|å¾å¼å|| |ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
+|ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
 |æµ·åå±éå¢|å¾å¼å|| |æ´¥å½©éæ¥|å¾å¼å||
 |éæ¥é»è¨|å¾å¼å|| |å¹¿ä¸å±éå¢|å¾å¼å||
 |éæ¥æ³å·|å¾å¼å|| |è¾½å®å±éå¢|å¾å¼å||
 |å®å¤å±éå¢|å¾å¼å|| |æ°çå±éå¢|å¾å¼å||
 |è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°  ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) -
 ä½¿ç¨`git clone https://github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶   ç¬¬äºç§æ¹å¼
@@ -89,16 +91,20 @@
 | | éç½®éç½® | éç½®éç½®ãå·æ°éç½® | è¶ç®¡å¯ç¨ï¼å·æ°Web
 UIé»è®¤éç½® | | éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID |
 |å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|
 |å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|
 |æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|
 |æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|
-## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿
-###2023/04/12 - å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
+## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿ ###
+2023/05/06 - å¢å åæå°åºï¼éè¦èªè¡æå -
+ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢ -
+æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼ -
+è°æ´é¨åä¾èµ   2023/04/12 -
+å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ® -
 æ·»å `å¯¼åºç¨æ·æ°æ®`åè½ - æ·»å `æ´æ°ç¨æ·æ°æ®`åè½ -
 æ·»å `æ´æ°èµæºæ°æ®`åè½ï¼æ±è¥¿å°åºæ´æ°åè¯·ä½¿ç¨ä¸æ­¤åè½å·æ°å¢æ¯é¨æ°æ®
 - æ·»å æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹ -
 æ·»å å¤§å­¦ä¹ æéå¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹ -
```

