# Comparing `tmp/easy-pil-0.2.0.tar.gz` & `tmp/easy-pil-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-pil-0.2.0.tar", last modified: Sat Apr 15 12:11:22 2023, max compression
+gzip compressed data, was "/home/runner/work/easy-pil/easy-pil/dist/.tmp-1z7na8nk/easy-pil-0.2.1.tar", last modified: Sat May  6 20:00:12 2023, max compression
```

## Comparing `easy-pil-0.2.0.tar` & `easy-pil-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1055 2023-04-14 18:03:37.000000 easy-pil-0.2.0/LICENSE
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)       62 2023-04-14 18:03:37.000000 easy-pil-0.2.0/MANIFEST.in
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1845 2023-04-15 12:11:22.039843 easy-pil-0.2.0/PKG-INFO
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      812 2023-04-14 18:03:37.000000 easy-pil-0.2.0/README.md
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.035843 easy-pil-0.2.0/easy_pil/
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      253 2023-04-14 18:28:11.000000 easy-pil-0.2.0/easy_pil/__init__.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      201 2023-04-14 18:15:55.000000 easy-pil-0.2.0/easy_pil/_version.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1082 2023-04-15 11:41:28.000000 easy-pil-0.2.0/easy_pil/canvas.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)    17851 2023-04-15 11:31:58.000000 easy-pil-0.2.0/easy_pil/editor.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     3339 2023-04-14 18:15:55.000000 easy-pil-0.2.0/easy_pil/font.py
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.035843 easy-pil-0.2.0/easy_pil/fonts/
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.035843 easy-pil-0.2.0/easy_pil/fonts/caveat/
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   256900 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/caveat/caveat.ttf
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/easy_pil/fonts/montserrat/
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   244468 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_bold.ttf
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   249088 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_italic.ttf
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   242068 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_light.ttf
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   245708 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_regular.ttf
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/easy_pil/fonts/poppins/
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   153900 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_bold.ttf
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   181972 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_italic.ttf
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   159848 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_light.ttf
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)   158192 2023-04-14 18:03:37.000000 easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_regular.ttf
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      807 2023-04-15 11:41:19.000000 easy-pil-0.2.0/easy_pil/text.py
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/easy_pil/types/
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 11:29:53.000000 easy-pil-0.2.0/easy_pil/types/__init__.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      106 2023-04-15 11:31:59.000000 easy-pil-0.2.0/easy_pil/types/common.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1012 2023-04-15 11:31:58.000000 easy-pil-0.2.0/easy_pil/types/workspace.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1373 2023-04-14 18:15:55.000000 easy-pil-0.2.0/easy_pil/utils.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     6490 2023-04-15 11:48:03.000000 easy-pil-0.2.0/easy_pil/workspace.py
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.035843 easy-pil-0.2.0/easy_pil.egg-info/
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     1845 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/PKG-INFO
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      897 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/SOURCES.txt
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        1 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/dependency_links.txt
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      121 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/requires.txt
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)        9 2023-04-15 12:11:22.000000 easy-pil-0.2.0/easy_pil.egg-info/top_level.txt
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      408 2023-04-15 12:08:59.000000 easy-pil-0.2.0/pyproject.toml
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)       38 2023-04-15 12:11:22.039843 easy-pil-0.2.0/setup.cfg
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     2085 2023-04-14 18:15:55.000000 easy-pil-0.2.0/setup.py
-drwxrwxr-x   0 shahriyar  (1000) shahriyar  (1000)        0 2023-04-15 12:11:22.039843 easy-pil-0.2.0/tests/
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      288 2023-04-04 09:25:35.000000 easy-pil-0.2.0/tests/test_canvas.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)     5152 2023-04-14 18:15:55.000000 easy-pil-0.2.0/tests/test_editor.py
--rw-rw-r--   0 shahriyar  (1000) shahriyar  (1000)      705 2023-04-14 18:15:55.000000 easy-pil-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-06 19:59:55.000000 easy-pil-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-06 19:59:55.000000 easy-pil-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-06 20:00:12.000000 easy-pil-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-06 19:59:55.000000 easy-pil-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-06 19:59:55.000000 easy-pil-0.2.1/easy_pil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-06 19:59:55.000000 easy-pil-0.2.1/easy_pil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-06 19:59:55.000000 easy-pil-0.2.1/easy_pil/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-05-06 19:59:55.000000 easy-pil-0.2.1/easy_pil/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-06 19:59:55.000000 easy-pil-0.2.1/easy_pil/font.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil/fonts/caveat/
+-rw-r--r--   0 runner    (1001) docker     (123)   256900 2023-05-06 19:59:55.000000 easy-pil-0.2.1/easy_pil/fonts/caveat/caveat.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil/fonts/montserrat/
+-rw-r--r--   0 runner    (1001) docker     (123)   244468 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/fonts/montserrat/montserrat_bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   249088 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/fonts/montserrat/montserrat_italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   242068 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/fonts/montserrat/montserrat_light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   245708 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/fonts/montserrat/montserrat_regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil/fonts/poppins/
+-rw-r--r--   0 runner    (1001) docker     (123)   153900 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/fonts/poppins/poppins_bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   181972 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/fonts/poppins/poppins_italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159848 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/fonts/poppins/poppins_light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158192 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/fonts/poppins/poppins_regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/types/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-06 19:59:56.000000 easy-pil-0.2.1/easy_pil/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 20:00:12.000000 easy-pil-0.2.1/easy_pil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-06 19:59:56.000000 easy-pil-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-06 19:59:56.000000 easy-pil-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 20:00:12.000000 easy-pil-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-06 19:59:56.000000 easy-pil-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:00:12.000000 easy-pil-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-06 19:59:56.000000 easy-pil-0.2.1/tests/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-06 19:59:56.000000 easy-pil-0.2.1/tests/test_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-06 19:59:56.000000 easy-pil-0.2.1/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `easy-pil-0.2.0/LICENSE` & `easy-pil-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/PKG-INFO` & `easy-pil-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-pil
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library to make common tasks of Pillow easy.
 Home-page: https://github.com/shahriyardx/easy-pil
 Author: Md Shahriyar Alam
 Author-email: contact@shahriyar.dev
 Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
 Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
 Project-URL: Source, https://github.com/shahriyardx/easy-pil/
@@ -19,20 +19,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Easy PIL
-A python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
+A Python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
 
 ## Getting Started
 Using this for the first time? Here are some links to help you get started.
 
-- Readt the [docs](https://easy-pil.readthedocs.io/en/latest/)
+- Read the [docs](https://easy-pil.readthedocs.io/en/latest/)
 - First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
 - Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
 - Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
 - [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
 
 ## Get help
 - Ask us in our [Discord server](https://discord.gg/4rd4JQWmsY)
```

### Comparing `easy-pil-0.2.0/README.md` & `easy-pil-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Easy PIL
-A python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
+A Python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
 
 ## Getting Started
 Using this for the first time? Here are some links to help you get started.
 
-- Readt the [docs](https://easy-pil.readthedocs.io/en/latest/)
+- Read the [docs](https://easy-pil.readthedocs.io/en/latest/)
 - First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
 - Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
 - Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
 - [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
 
 ## Get help
 - Ask us in our [Discord server](https://discord.gg/4rd4JQWmsY)
```

### Comparing `easy-pil-0.2.0/easy_pil/canvas.py` & `easy-pil-0.2.1/easy_pil/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Union
+from typing import Tuple
 
 from PIL import Image
 
 from .types.common import Color
 
 
 class Canvas:
```

### Comparing `easy-pil-0.2.0/easy_pil/editor.py` & `easy-pil-0.2.1/easy_pil/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from io import BytesIO
-from typing import List, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 from PIL import Image, ImageDraw, ImageFilter, ImageFont
 from typing_extensions import Literal
 
 from .canvas import Canvas
 from .font import Font
 from .text import Text
@@ -226,14 +226,16 @@
     def text(
         self,
         position: Tuple[float, float],
         text: str,
         font: Union[ImageFont.FreeTypeFont, Font] = None,
         color: Color = "black",
         align: Literal["left", "center", "right"] = "left",
+        stroke_width: int = None,
+        stroke_fill: Color = "black"
     ) -> Editor:
         """Draw text into image
 
         Parameters
         ----------
         position : Tuple[float, float]
             Position to draw text
@@ -241,22 +243,33 @@
             Text to draw
         font : Union[ImageFont.FreeTypeFont, Font], optional
             Font used for text, by default None
         color : Color, optional
             Color of the font, by default "black"
         align : Literal["left", "center", "right"], optional
             Align text, by default "left"
+        stroke_width : int, optional
+            Whether there should be any stroke. Defaults to
+            None. It represents the width of the said stroke.
+        stroke_fill : Color, optional
+            Color of the stroke, if any stroke is applied to the
+            text. Defaults to "black"
         """
         if isinstance(font, Font):
             font = font.font
 
         anchors = {"left": "lt", "center": "mt", "right": "rt"}
 
         draw = ImageDraw.Draw(self.image)
-        draw.text(position, text, color, font=font, anchor=anchors[align])
+
+        if stroke_width:
+            draw.text(position, text, color, font=font, anchor=anchors[align],
+                      stroke_width=stroke_width, stroke_fill=stroke_fill)
+        else:
+            draw.text(position, text, color, font=font, anchor=anchors[align])
 
         return self
 
     def multi_text(
         self,
         position: Tuple[float, float],
         texts: List[Text],
```

### Comparing `easy-pil-0.2.0/easy_pil/font.py` & `easy-pil-0.2.1/easy_pil/font.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/caveat/caveat.ttf` & `easy-pil-0.2.1/easy_pil/fonts/caveat/caveat.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_bold.ttf` & `easy-pil-0.2.1/easy_pil/fonts/montserrat/montserrat_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_italic.ttf` & `easy-pil-0.2.1/easy_pil/fonts/montserrat/montserrat_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_light.ttf` & `easy-pil-0.2.1/easy_pil/fonts/montserrat/montserrat_light.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/montserrat/montserrat_regular.ttf` & `easy-pil-0.2.1/easy_pil/fonts/montserrat/montserrat_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_bold.ttf` & `easy-pil-0.2.1/easy_pil/fonts/poppins/poppins_bold.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_italic.ttf` & `easy-pil-0.2.1/easy_pil/fonts/poppins/poppins_italic.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_light.ttf` & `easy-pil-0.2.1/easy_pil/fonts/poppins/poppins_light.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/fonts/poppins/poppins_regular.ttf` & `easy-pil-0.2.1/easy_pil/fonts/poppins/poppins_regular.ttf`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/text.py` & `easy-pil-0.2.1/easy_pil/text.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil/types/workspace.py` & `easy-pil-0.2.1/easy_pil/types/workspace.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from typing import List, Tuple, TypedDict, Union
+from typing import List, Tuple, Union
+
+try:
+    from typing import TypedDict
+except ImportError:
+    from typing_extensions import TypedDict
 
 from PIL.Image import Image
 from PIL.ImageFont import FreeTypeFont
 from typing_extensions import Literal
 
 from ..canvas import Canvas
 from ..editor import Editor
```

### Comparing `easy-pil-0.2.0/easy_pil/utils.py` & `easy-pil-0.2.1/easy_pil/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import functools
 from io import BytesIO
 
 import aiohttp
 import requests
-from memoization import cached
 from PIL import Image
 
 
 async def run_in_executor(func, **kwargs):
     """Run function in executor
 
     Parameters
@@ -17,15 +16,14 @@
         Function to run
     """
     func = functools.partial(func, **kwargs)
     data = await asyncio.get_event_loop().run_in_executor(None, func)
     return data
 
 
-@cached(max_size=50)
 def load_image(link: str) -> Image.Image:
     """Load image from link
 
     Parameters
     ----------
     link : str
         Image link
@@ -37,15 +35,14 @@
     """
     _bytes = BytesIO(requests.get(link).content)
     image = Image.open(_bytes).convert("RGBA")
 
     return image
 
 
-@cached(max_size=50)
 async def load_image_async(link: str) -> Image.Image:
     """Load image from link (async)
 
     Parameters
     ----------
     link : str
         Image from the provided link (if any)
```

### Comparing `easy-pil-0.2.0/easy_pil/workspace.py` & `easy-pil-0.2.1/easy_pil/workspace.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/easy_pil.egg-info/PKG-INFO` & `easy-pil-0.2.1/easy_pil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-pil
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library to make common tasks of Pillow easy.
 Home-page: https://github.com/shahriyardx/easy-pil
 Author: Md Shahriyar Alam
 Author-email: contact@shahriyar.dev
 Project-URL: Documentation, https://easy-pil.readthedocs.io/en/latest/
 Project-URL: Bug Reports, https://github.com/shahriyardx/easy-pil/issues
 Project-URL: Source, https://github.com/shahriyardx/easy-pil/
@@ -19,20 +19,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Easy PIL
-A python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
+A Python library built on top of [PIL](https://github.com/python-pillow/Pillow) to easily edit/modify images. 
 
 ## Getting Started
 Using this for the first time? Here are some links to help you get started.
 
-- Readt the [docs](https://easy-pil.readthedocs.io/en/latest/)
+- Read the [docs](https://easy-pil.readthedocs.io/en/latest/)
 - First steps [Introduction](https://easy-pil.readthedocs.io/en/latest/pages/intro.html)
 - Integrate in a [Discord bot](https://easy-pil.readthedocs.io/en/latest/pages/discordbot.html)
 - Some premade [Examples](https://github.com/shahriyardx/easy-pil/tree/master/examples)
 - [Report bugs](https://github.com/shahriyardx/easy-pil/issues/)
 
 ## Get help
 - Ask us in our [Discord server](https://discord.gg/4rd4JQWmsY)
```

### Comparing `easy-pil-0.2.0/easy_pil.egg-info/SOURCES.txt` & `easy-pil-0.2.1/easy_pil.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.py
 easy_pil/__init__.py
 easy_pil/_version.py
 easy_pil/canvas.py
 easy_pil/editor.py
 easy_pil/font.py
 easy_pil/text.py
```

### Comparing `easy-pil-0.2.0/setup.py` & `easy-pil-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 current_directory = Path(__file__).parent.resolve()
 
 
 def _get_requirements() -> list:
-    with open("requirements.txt") as f:
+    with open(current_directory / "requirements.txt") as f:
         return f.read().splitlines()
 
 
 def _get_long_desc() -> str:
     return (current_directory / "README.md").read_text(encoding="utf-8")
```

### Comparing `easy-pil-0.2.0/tests/test_editor.py` & `easy-pil-0.2.1/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `easy-pil-0.2.0/tests/test_utils.py` & `easy-pil-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

