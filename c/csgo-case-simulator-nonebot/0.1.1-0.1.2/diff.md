# Comparing `tmp/csgo-case-simulator-nonebot-0.1.1.tar.gz` & `tmp/csgo-case-simulator-nonebot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csgo-case-simulator-nonebot-0.1.1.tar", max compression
+gzip compressed data, was "csgo-case-simulator-nonebot-0.1.2.tar", max compression
```

## Comparing `csgo-case-simulator-nonebot-0.1.1.tar` & `csgo-case-simulator-nonebot-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2931 2023-05-06 15:50:23.717223 csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/__init__.py
--rw-r--r--   0        0        0   274723 2023-05-06 15:50:23.752798 csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/background2.png
--rw-r--r--   0        0        0     2424 2023-05-06 15:50:23.776395 csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/cases.py
--rw-r--r--   0        0        0     1743 2023-05-06 15:50:23.779773 csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/skins.py
--rw-r--r--   0        0        0     2844 2023-05-06 16:13:09.001320 csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/utils.py
--rw-r--r--   0        0        0      484 2023-05-06 16:15:20.954833 csgo-case-simulator-nonebot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      728 2023-05-06 16:15:23.079427 csgo-case-simulator-nonebot-0.1.1/setup.py
--rw-r--r--   0        0        0      499 2023-05-06 16:15:23.079578 csgo-case-simulator-nonebot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2931 2023-05-06 15:50:23.717223 csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/__init__.py
+-rw-r--r--   0        0        0   274723 2023-05-06 15:50:23.752798 csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/background2.png
+-rw-r--r--   0        0        0     2424 2023-05-06 15:50:23.776395 csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/cases.py
+-rw-r--r--   0        0        0     1743 2023-05-06 15:50:23.779773 csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/skins.py
+-rw-r--r--   0        0        0     2940 2023-05-06 16:34:30.795380 csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/utils.py
+-rw-r--r--   0        0        0      484 2023-05-06 16:33:54.184925 csgo-case-simulator-nonebot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      728 2023-05-06 16:34:44.628227 csgo-case-simulator-nonebot-0.1.2/setup.py
+-rw-r--r--   0        0        0      499 2023-05-06 16:34:44.628364 csgo-case-simulator-nonebot-0.1.2/PKG-INFO
```

### Comparing `csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/__init__.py` & `csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/__init__.py`

 * *Files identical despite different names*

### Comparing `csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/background2.png` & `csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/background2.png`

 * *Files identical despite different names*

### Comparing `csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/cases.py` & `csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/cases.py`

 * *Files identical despite different names*

### Comparing `csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/skins.py` & `csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/skins.py`

 * *Files identical despite different names*

### Comparing `csgo-case-simulator-nonebot-0.1.1/csgo-case-simulator-nonebot/utils.py` & `csgo-case-simulator-nonebot-0.1.2/csgo-case-simulator-nonebot/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 from io import BytesIO
 import math
+import os
 from PIL import Image, ImageFont, ImageDraw, ImageFilter
 import requests
 
 rarity_color = {
     "工业级": (96, 152, 217),
     "军规级": (76, 105, 255),
     "受限": (136, 70, 255),
@@ -28,30 +29,32 @@
     height = image_list[0].height
     number = len(items)
     rows = math.ceil(number / 5)
     columns = number if number < 5 else 5
     padding = 200
     info_height = 200
     bg_color = (255, 255, 255)
-    font_color = (0, 0, 0)
+    font_color = (255, 255, 255)
 
-    # background_img = Image.open(
-    #     "src/plugins/csgo-case-simulator/background2.png")
-    # background_img = background_img.filter(ImageFilter.GaussianBlur(radius=50))
-    # background_img = background_img.resize((width * columns + padding,
-    #                                         (height + info_height) * rows + padding))
-
-    canvas = Image.new(
-        "RGBA",
-        (
-            width * columns + padding,
-            (height + info_height) * rows + padding
-        ),
-        bg_color
-    )
+    path = os.path.dirname(os.path.abspath(__file__))
+    bg_file = os.path.join(path, "background2.png")
+    background_img = Image.open(bg_file)
+    background_img = background_img.filter(ImageFilter.GaussianBlur(radius=50))
+    background_img = background_img.resize((width * columns + padding,
+                                            (height + info_height) * rows + padding))
+
+    canvas = background_img
+    # Image.new(
+    #     "RGBA",
+    #     (
+    #         width * columns + padding,
+    #         (height + info_height) * rows + padding
+    #     ),
+    #     bg_color
+    # )
 
     for i in range(len(items)):
         row = math.ceil((i + 1) / 5)
         canvas.paste(
             image_list[i],
             (
                 width * (i % 5)+100,
```

### Comparing `csgo-case-simulator-nonebot-0.1.1/setup.py` & `csgo-case-simulator-nonebot-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['Pillow>=9.5.0,<10.0.0',
  'nonebot-adapter-onebot>=2.2.3,<3.0.0',
  'nonebot2>=2.0.0-rc.4,<3.0.0']
 
 setup_kwargs = {
     'name': 'csgo-case-simulator-nonebot',
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

