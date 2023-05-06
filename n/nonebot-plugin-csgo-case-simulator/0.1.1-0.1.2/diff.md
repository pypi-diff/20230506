# Comparing `tmp/nonebot-plugin-csgo-case-simulator-0.1.1.tar.gz` & `tmp/nonebot-plugin-csgo-case-simulator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-csgo-case-simulator-0.1.1.tar", max compression
+gzip compressed data, was "nonebot-plugin-csgo-case-simulator-0.1.2.tar", max compression
```

## Comparing `nonebot-plugin-csgo-case-simulator-0.1.1.tar` & `nonebot-plugin-csgo-case-simulator-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-06 16:52:29.595978 nonebot-plugin-csgo-case-simulator-0.1.1/LICENSE
--rw-r--r--   0        0        0     2931 2023-05-06 15:50:23.717223 nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/__init__.py
--rw-r--r--   0        0        0   274723 2023-05-06 15:50:23.752798 nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/background2.png
--rw-r--r--   0        0        0     2424 2023-05-06 15:50:23.776395 nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/cases.py
--rw-r--r--   0        0        0     1743 2023-05-06 15:50:23.779773 nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/skins.py
--rw-r--r--   0        0        0     2940 2023-05-06 16:34:30.795380 nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/utils.py
--rw-r--r--   0        0        0      519 2023-05-06 16:59:32.458473 nonebot-plugin-csgo-case-simulator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      770 2023-05-06 16:59:46.292678 nonebot-plugin-csgo-case-simulator-0.1.1/setup.py
--rw-r--r--   0        0        0      548 2023-05-06 16:59:46.292836 nonebot-plugin-csgo-case-simulator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-06 16:52:29.595978 nonebot-plugin-csgo-case-simulator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3194 2023-05-06 19:24:50.184276 nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/__init__.py
+-rw-r--r--   0        0        0   274723 2023-05-06 15:50:23.752798 nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/background2.png
+-rw-r--r--   0        0        0     2442 2023-05-06 19:24:19.879469 nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/cases.py
+-rw-r--r--   0        0        0     1846 2023-05-06 19:24:30.996173 nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/skins.py
+-rw-r--r--   0        0        0     3759 2023-05-06 19:24:38.310093 nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/utils.py
+-rw-r--r--   0        0        0      516 2023-05-06 19:24:57.674967 nonebot-plugin-csgo-case-simulator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-05-06 19:25:06.469348 nonebot-plugin-csgo-case-simulator-0.1.2/setup.py
+-rw-r--r--   0        0        0      546 2023-05-06 19:25:06.469477 nonebot-plugin-csgo-case-simulator-0.1.2/PKG-INFO
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/LICENSE` & `nonebot-plugin-csgo-case-simulator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/__init__.py` & `nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,30 @@
+import asyncio
 from enum import Enum
 import os
+import time
 from nonebot import on_command
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, MessageEvent
+import httpx
 from .cases import Cases
 from .skins import Skins
-from .utils import merge_images
+from .utils import Utils
 
 cases = Cases()
 skins = Skins()
+utils = Utils()
+
+
+async def get_all_json():
+    res = await asyncio.gather(cases.get_cases_json(), skins.get_skins_json())
+    cases.cases = res[0].json()
+    skins.skins = res[1].json()
+
+asyncio.run(get_all_json())
 
 rarities = {
     "工业级": 1,
     "军规级": 2,
     "受限": 3,
     "保密": 4,
     "隐秘": 5,
@@ -61,15 +73,17 @@
         if case:
             await case_opening.send(MessageSegment.image(case["image"])+f"正在开启{case['name']}...")
             items = cases.open_case_multiple(case["id"], amount)
             opened_skins = []
             for item in items:
                 skin = skins.get_skins(item["name"])
                 opened_skins.append(skin)
-            image = merge_images(opened_skins)
+
+            image = await utils.merge_images(opened_skins)
+
             await case_opening.finish(MessageSegment.image(image))
         else:
             await case_opening.finish("箱子不存在")
     else:
         await case_opening.finish("请输入箱子名称")
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/background2.png` & `nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/background2.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/cases.py` & `nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/cases.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import random
-import requests
+import httpx
 
 
 class Cases:
     def __init__(self):
         self.cases_api = "https://bymykel.github.io/CSGO-API/api/zh-CN/crates/cases.json"
-        self.cases = requests.get(self.cases_api).json()
+
+        self.cases = []
+
         self.probabilities = {
             "工业级": 0.63435,
             "军规级": 0.16693,
             "受限": 0.15985,
             "保密": 0.03205,
             "隐秘": 0.00640,
         }
         self.probabilities2 = {
             "军规级": 0.80128,
             "受限": 0.15985,
             "保密": 0.03205,
             "隐秘": 0.00640,
         }
 
-    def refresh_cases(self):
-        self.cases = requests.get(self.cases_api).json()
+    async def get_cases_json(self):
+        async with httpx.AsyncClient() as client:
+            return await client.get(self.cases_api)
 
     def get_case_name_list(self) -> list:
         return [case["name"] for case in self.cases]
 
     def get_random_case(self) -> dict:
         return random.choice(self.cases)
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/skins.py` & `nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/skins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import random
-import requests
+import httpx
 
 
 class Skins:
     def __init__(self):
         self.skins_api = "https://bymykel.github.io/CSGO-API/api/zh-CN/skins.json"
-        self.skins = requests.get(self.skins_api).json()
+        self.skins = []
+
+    async def get_skins_json(self):
+        async with httpx.AsyncClient() as client:
+            return await client.get(self.skins_api)
 
     def get_skins(self, name: str) -> dict:
         # print(name)
         for skin in self.skins:
             if skin["name"] == name:
                 wear_rating = round(
                     random.uniform(skin["min_float"], skin["max_float"]), 5
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/nonebot-plugin-csgo-case-simulator/utils.py` & `nonebot-plugin-csgo-case-simulator-0.1.2/nonebot-plugin-csgo-case-simulator/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,116 @@
+import asyncio
 import base64
 from io import BytesIO
 import math
 import os
+import time
 from PIL import Image, ImageFont, ImageDraw, ImageFilter
-import requests
+import httpx
 
-rarity_color = {
-    "工业级": (96, 152, 217),
-    "军规级": (76, 105, 255),
-    "受限": (136, 70, 255),
-    "保密": (177, 46, 194),
-    "隐秘": (235, 75, 75),
-    "及其罕见的特殊物品": (201, 171, 5),
-    "非凡": (201, 171, 5),
-}
-
-
-def merge_images(items):
-    ttf_path = "仓耳舒圆体W03.ttf"
-    font = ImageFont.truetype(ttf_path, 40)
-    image_list = []
-    for i in range(len(items)):
-        img = Image.open(
-            BytesIO(requests.get(items[i]["image"]).content))
-        image_list.append(img)
-
-    width = image_list[0].width
-    height = image_list[0].height
-    number = len(items)
-    rows = math.ceil(number / 5)
-    columns = number if number < 5 else 5
-    padding = 200
-    info_height = 200
-    bg_color = (255, 255, 255)
-    font_color = (255, 255, 255)
-
-    path = os.path.dirname(os.path.abspath(__file__))
-    bg_file = os.path.join(path, "background2.png")
-    background_img = Image.open(bg_file)
-    background_img = background_img.filter(ImageFilter.GaussianBlur(radius=50))
-    background_img = background_img.resize((width * columns + padding,
-                                            (height + info_height) * rows + padding))
-
-    canvas = background_img
-    # Image.new(
-    #     "RGBA",
-    #     (
-    #         width * columns + padding,
-    #         (height + info_height) * rows + padding
-    #     ),
-    #     bg_color
-    # )
-
-    for i in range(len(items)):
-        row = math.ceil((i + 1) / 5)
-        canvas.paste(
-            image_list[i],
-            (
-                width * (i % 5)+100,
-                (height + info_height) * (row - 1) + 100
-            ),
-            image_list[i]
-        )
-
-    draw = ImageDraw.Draw(canvas)
-    for i in range(len(items)):
-        row = math.ceil((i + 1) / 5)
-        draw.text(
-            (
-                width * (i % 5)+100 + width / 4,
-                100 + height * row + (row - 1) * info_height
-            ),
-            items[i]["name"],
-            font=font,
-            fill=font_color
-        )
-        draw.text(
-            (
-                width * (i % 5)+100 + width / 4,
-                100 + height * row + (row - 1) * info_height + 50
-            ),
-            items[i]["rarity"],
-            font=font,
-            fill=rarity_color[items[i]["rarity"]]
-        )
-        draw.text(
-            (
-                width * (i % 5)+100 + width / 4,
-                100 + height * row + (row - 1) * info_height + 100
-            ),
-            f"磨损: {items[i]['wear_rating']}",
-            font=font,
-            fill=font_color
-        )
-
-    return img_to_b64(canvas)
-
-
-def img_to_b64(pic: Image.Image) -> str:
-    buf = BytesIO()
-    pic.save(buf, format="PNG")
-    base64_str = base64.b64encode(buf.getbuffer()).decode()
-    return "base64://" + base64_str
+
+class Utils:
+    def __init__(self):
+        self.client = httpx.Client()
+        self.rarity_color = {
+            "工业级": (96, 152, 217),
+            "军规级": (76, 105, 255),
+            "受限": (136, 70, 255),
+            "保密": (177, 46, 194),
+            "隐秘": (235, 75, 75),
+            "及其罕见的特殊物品": (201, 171, 5),
+            "非凡": (201, 171, 5),
+        }
+
+    async def merge_images(self, items):
+        ttf_path = "仓耳舒圆体W03.ttf"
+        font = ImageFont.truetype(ttf_path, 40)
+        image_list = []
+
+        time1 = time.time()
+        image_tasks = [self.download_image(item["image"]) for item in items]
+        image_list = await asyncio.gather(*image_tasks)
+        time2 = time.time()
+        print("下载图片耗时：", time2 - time1)
+
+        width = image_list[0].width
+        height = image_list[0].height
+        number = len(items)
+        rows = math.ceil(number / 5)
+        columns = number if number < 5 else 5
+        padding = 200
+        info_height = 200
+        bg_color = (255, 255, 255)
+        font_color = (255, 255, 255)
+
+        path = os.path.dirname(os.path.abspath(__file__))
+        bg_file = os.path.join(path, "background2.png")
+        background_img = Image.open(bg_file)
+        background_img = background_img.filter(
+            ImageFilter.GaussianBlur(radius=50))
+        background_img = background_img.resize((width * columns + padding,
+                                                (height + info_height) * rows + padding))
+
+        canvas = background_img
+        # Image.new(
+        #     "RGBA",
+        #     (
+        #         width * columns + padding,
+        #         (height + info_height) * rows + padding
+        #     ),
+        #     bg_color
+        # )
+        for i in range(len(items)):
+            row = math.ceil((i + 1) / 5)
+            canvas.paste(
+                image_list[i],
+                (
+                    width * (i % 5)+100,
+                    (height + info_height) * (row - 1) + 100
+                ),
+                image_list[i]
+            )
+
+        draw = ImageDraw.Draw(canvas)
+        for i in range(len(items)):
+            row = math.ceil((i + 1) / 5)
+            draw.text(
+                (
+                    width * (i % 5)+100 + width / 4,
+                    100 + height * row + (row - 1) * info_height
+                ),
+                items[i]["name"],
+                font=font,
+                fill=font_color
+            )
+            draw.text(
+                (
+                    width * (i % 5)+100 + width / 4,
+                    100 + height * row + (row - 1) * info_height + 50
+                ),
+                items[i]["rarity"],
+                font=font,
+                fill=self.rarity_color[items[i]["rarity"]]
+            )
+            draw.text(
+                (
+                    width * (i % 5)+100 + width / 4,
+                    100 + height * row + (row - 1) * info_height + 100
+                ),
+                f"磨损: {items[i]['wear_rating']}",
+                font=font,
+                fill=font_color
+            )
+
+        return self.img_to_b64(canvas)
+
+    async def download_image(self, url):
+        async with httpx.AsyncClient() as client:
+            response = await client.get(url)
+            img = Image.open(BytesIO(response.content))
+            return img
+
+    def img_to_b64(self, pic: Image.Image) -> str:
+        buf = BytesIO()
+        pic.save(buf, format="PNG")
+        base64_str = base64.b64encode(buf.getbuffer()).decode()
+        return "base64://" + base64_str
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/pyproject.toml` & `nonebot-plugin-csgo-case-simulator-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "nonebot-plugin-csgo-case-simulator"
-version = "0.1.1"
+version = "0.1.2"
 description = "a nonebot based csgo case simulator"
 authors = ["Roy <lyt2980999208@gmail.com>"]
 license = "MIT"
 packages = [{ include = "nonebot-plugin-csgo-case-simulator" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nonebot2 = "^2.0.0-rc.4"
 nonebot-adapter-onebot = "^2.2.3"
 Pillow = "^9.5.0"
-requests = "^2.30.0"
+httpx = "^0.24.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/setup.py` & `nonebot-plugin-csgo-case-simulator-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 ['nonebot-plugin-csgo-case-simulator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.5.0,<10.0.0',
+ 'httpx>=0.24.0,<0.25.0',
  'nonebot-adapter-onebot>=2.2.3,<3.0.0',
- 'nonebot2>=2.0.0-rc.4,<3.0.0',
- 'requests>=2.30.0,<3.0.0']
+ 'nonebot2>=2.0.0-rc.4,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-csgo-case-simulator',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'a nonebot based csgo case simulator',
     'long_description': None,
     'author': 'Roy',
     'author_email': 'lyt2980999208@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.1/PKG-INFO` & `nonebot-plugin-csgo-case-simulator-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-csgo-case-simulator
-Version: 0.1.1
+Version: 0.1.2
 Summary: a nonebot based csgo case simulator
 License: MIT
 Author: Roy
 Author-email: lyt2980999208@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Pillow (>=9.5.0,<10.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-rc.4,<3.0.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
```

