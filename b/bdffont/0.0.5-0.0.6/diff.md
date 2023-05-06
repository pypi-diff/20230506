# Comparing `tmp/bdffont-0.0.5.tar.gz` & `tmp/bdffont-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdffont-0.0.5.tar", last modified: Fri May  5 20:05:26 2023, max compression
+gzip compressed data, was "bdffont-0.0.6.tar", last modified: Sat May  6 08:41:47 2023, max compression
```

## Comparing `bdffont-0.0.5.tar` & `bdffont-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.479815 bdffont-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 20:05:11.000000 bdffont-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 20:05:26.479815 bdffont-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-05 20:05:11.000000 bdffont-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-05 20:05:11.000000 bdffont-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:05:26.479815 bdffont-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.475815 bdffont-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.475815 bdffont-0.0.5/src/bdffont/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.479815 bdffont-0.0.5/src/bdffont.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 20:05:26.000000 bdffont-0.0.5/src/bdffont.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 20:05:26.000000 bdffont-0.0.5/src/bdffont.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:05:26.000000 bdffont-0.0.5/src/bdffont.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 20:05:26.000000 bdffont-0.0.5/src/bdffont.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.479815 bdffont-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-05 20:05:11.000000 bdffont-0.0.5/tests/test_damaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-05 20:05:11.000000 bdffont-0.0.5/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-05 20:05:11.000000 bdffont-0.0.5/tests/test_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.890764 bdffont-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 08:41:31.000000 bdffont-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-06 08:41:47.890764 bdffont-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-06 08:41:31.000000 bdffont-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-06 08:41:31.000000 bdffont-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:41:47.890764 bdffont-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.886763 bdffont-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.890764 bdffont-0.0.6/src/bdffont/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-06 08:41:31.000000 bdffont-0.0.6/src/bdffont/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.890764 bdffont-0.0.6/src/bdffont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-06 08:41:47.000000 bdffont-0.0.6/src/bdffont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-06 08:41:47.000000 bdffont-0.0.6/src/bdffont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:41:47.000000 bdffont-0.0.6/src/bdffont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 08:41:47.000000 bdffont-0.0.6/src/bdffont.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:41:47.890764 bdffont-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-06 08:41:31.000000 bdffont-0.0.6/tests/test_damaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-06 08:41:31.000000 bdffont-0.0.6/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-06 08:41:31.000000 bdffont-0.0.6/tests/test_type.py
```

### Comparing `bdffont-0.0.5/LICENSE` & `bdffont-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.5/PKG-INFO` & `bdffont-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
@@ -36,25 +36,29 @@
 import bdffont
 from bdffont import BdfGlyph
 from examples import assets_dir, outputs_dir
 
 
 def main():
     font = bdffont.load_bdf(os.path.join(assets_dir, 'example.bdf'))
+    font.name = 'my-new-font'
+    font.bounding_box_size = 16, 16
+    font.bounding_box_offset = 0, -2
     font.properties.font_version = '1.0.0'
     font.properties.font_ascent = 7
     font.properties.font_descent = 2
     font.properties.x_height = 5
     font.properties.cap_height = 7
     font.add_glyph(BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(500, 0),
         device_width=(8, 0),
-        bounding_box=(8, 16, 0, -2),
+        bounding_box_size=(8, 16),
+        bounding_box_offset=(0, -2),
         bitmap=[
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 1, 1, 0, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
```

### Comparing `bdffont-0.0.5/README.md` & `bdffont-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,25 +18,29 @@
 import bdffont
 from bdffont import BdfGlyph
 from examples import assets_dir, outputs_dir
 
 
 def main():
     font = bdffont.load_bdf(os.path.join(assets_dir, 'example.bdf'))
+    font.name = 'my-new-font'
+    font.bounding_box_size = 16, 16
+    font.bounding_box_offset = 0, -2
     font.properties.font_version = '1.0.0'
     font.properties.font_ascent = 7
     font.properties.font_descent = 2
     font.properties.x_height = 5
     font.properties.cap_height = 7
     font.add_glyph(BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(500, 0),
         device_width=(8, 0),
-        bounding_box=(8, 16, 0, -2),
+        bounding_box_size=(8, 16),
+        bounding_box_offset=(0, -2),
         bitmap=[
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 1, 1, 0, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
```

### Comparing `bdffont-0.0.5/pyproject.toml` & `bdffont-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdffont"
-version = "0.0.5"
+version = "0.0.6"
 description = "A library for manipulating '.bdf' format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `bdffont-0.0.5/src/bdffont/parser.py` & `bdffont-0.0.6/src/bdffont/parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -72,66 +72,72 @@
     raise BdfMissingLine('ENDCHAR')
 
 
 def _decode_glyph_segment(lines: Iterator[str], name: str) -> BdfGlyph:
     code_point = None
     scalable_width = None
     device_width = None
-    bounding_box = None
+    bounding_box_size = None
+    bounding_box_offset = None
     bitmap = None
     comments = []
     while line_params := _next_word_line(lines):
         word, tail = line_params
         if word == 'ENCODING':
             code_point = int(tail)
         elif word == 'SWIDTH':
             tokens = _convert_tail_to_ints(tail)
             scalable_width = tokens[0], tokens[1]
         elif word == 'DWIDTH':
             tokens = _convert_tail_to_ints(tail)
             device_width = tokens[0], tokens[1]
         elif word == 'BBX':
             tokens = _convert_tail_to_ints(tail)
-            bounding_box = tokens[0], tokens[1], tokens[2], tokens[3]
+            bounding_box_size = tokens[0], tokens[1]
+            bounding_box_offset = tokens[2], tokens[3]
         elif word == 'COMMENT':
             comments.append(tail)
         elif word == 'BITMAP' or word == 'ENDCHAR':
             if word == 'BITMAP':
                 bitmap = _decode_bitmap_segment(lines, comments)
             if code_point is None:
                 raise BdfMissingLine('ENCODING')
             if scalable_width is None:
                 raise BdfMissingLine('SWIDTH')
             if device_width is None:
                 raise BdfMissingLine('DWIDTH')
-            if bounding_box is None:
+            if bounding_box_size is None or bounding_box_offset is None:
                 raise BdfMissingLine('BBX')
-            return BdfGlyph(name, code_point, scalable_width, device_width, bounding_box, bitmap, comments)
+            return BdfGlyph(name, code_point, scalable_width, device_width, bounding_box_size, bounding_box_offset, bitmap, comments)
     raise BdfMissingLine('ENDCHAR')
 
 
 def _decode_font_segment(lines: Iterator[str]) -> BdfFont:
     name = None
-    size = None
-    bounding_box = None
+    point_size = None
+    dpi_xy = None
+    bounding_box_size = None
+    bounding_box_offset = None
     properties = None
     glyph_count = None
     glyphs = []
     alphabet = set()
     comments = []
     while line_params := _next_word_line(lines):
         word, tail = line_params
         if word == 'FONT':
             name = tail
         elif word == 'SIZE':
             tokens = _convert_tail_to_ints(tail)
-            size = tokens[0], tokens[1], tokens[2]
+            point_size = tokens[0]
+            dpi_xy = tokens[1], tokens[2]
         elif word == 'FONTBOUNDINGBOX':
             tokens = _convert_tail_to_ints(tail)
-            bounding_box = tokens[0], tokens[1], tokens[2], tokens[3]
+            bounding_box_size = tokens[0], tokens[1]
+            bounding_box_offset = tokens[2], tokens[3]
         elif word == 'STARTPROPERTIES':
             properties = _decode_properties_segment(lines, int(tail))
         elif word == 'CHARS':
             glyph_count = int(tail)
         elif word == 'STARTCHAR':
             glyph = _decode_glyph_segment(lines, tail)
             if glyph.code_point in alphabet:
@@ -139,23 +145,23 @@
             glyphs.append(glyph)
             alphabet.add(glyph.code_point)
         elif word == 'COMMENT':
             comments.append(tail)
         elif word == 'ENDFONT':
             if name is None:
                 raise BdfMissingLine('FONT')
-            if size is None:
+            if point_size is None or dpi_xy is None:
                 raise BdfMissingLine('SIZE')
-            if bounding_box is None:
+            if bounding_box_size is None or bounding_box_offset is None:
                 raise BdfMissingLine('FONTBOUNDINGBOX')
             if glyph_count is None:
                 raise BdfMissingLine('CHARS')
             if glyph_count != len(glyphs) or glyph_count != len(alphabet):
                 raise BdfValueIncorrect('CHARS')
-            return BdfFont(name, size, bounding_box, properties, glyphs, comments)
+            return BdfFont(name, point_size, dpi_xy, bounding_box_size, bounding_box_offset, properties, glyphs, comments)
     raise BdfMissingLine('ENDFONT')
 
 
 def decode_bdf(lines: Iterator[str]) -> BdfFont:
     while line_params := _next_word_line(lines):
         word, tail = line_params
         if word == 'STARTFONT':
```

### Comparing `bdffont-0.0.5/src/bdffont/properties.py` & `bdffont-0.0.6/src/bdffont/properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections import UserDict
 
-from bdffont.error import BdfPropertiesIllegalKey, BdfPropertiesIllegalValue
+from bdffont.error import BdfIllegalPropertiesKey, BdfIllegalPropertiesValue
 
 
 def _check_key(key: str):
     if not key.isupper():
-        raise BdfPropertiesIllegalKey(f'Properties key must be upper')
+        raise BdfIllegalPropertiesKey(f'Properties key must be upper')
     if not key.replace('_', '').isalpha():
-        raise BdfPropertiesIllegalKey(f"Illegal properties key '{key}'")
+        raise BdfIllegalPropertiesKey(f"Illegal properties key '{key}'")
 
 
 def _check_value(value: str | int):
     if not isinstance(value, str) and not isinstance(value, int):
-        raise BdfPropertiesIllegalValue("Properties value must be 'str' or 'int'")
+        raise BdfIllegalPropertiesValue("Properties value must be 'str' or 'int'")
 
 
 class BdfProperties(UserDict):
     # Comments.
     comments: list[str] = []
 
     def __getitem__(self, key: str) -> str | int:
```

### Comparing `bdffont-0.0.5/src/bdffont.egg-info/PKG-INFO` & `bdffont-0.0.6/src/bdffont.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
@@ -36,25 +36,29 @@
 import bdffont
 from bdffont import BdfGlyph
 from examples import assets_dir, outputs_dir
 
 
 def main():
     font = bdffont.load_bdf(os.path.join(assets_dir, 'example.bdf'))
+    font.name = 'my-new-font'
+    font.bounding_box_size = 16, 16
+    font.bounding_box_offset = 0, -2
     font.properties.font_version = '1.0.0'
     font.properties.font_ascent = 7
     font.properties.font_descent = 2
     font.properties.x_height = 5
     font.properties.cap_height = 7
     font.add_glyph(BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(500, 0),
         device_width=(8, 0),
-        bounding_box=(8, 16, 0, -2),
+        bounding_box_size=(8, 16),
+        bounding_box_offset=(0, -2),
         bitmap=[
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 1, 1, 0, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
```

### Comparing `bdffont-0.0.5/tests/test_damaged.py` & `bdffont-0.0.6/tests/test_damaged.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import pytest
 
 import bdffont
 from bdffont.error import BdfMissingLine, BdfValueIncorrect
 from tests import assets_dir
 
 
-def load_damaged_bdf(bdf_file_name: str | bytes | os.PathLike[str] | os.PathLike[bytes]):
-    bdf_file_path = os.path.join(assets_dir, 'damaged', bdf_file_name)
-    bdffont.load_bdf(bdf_file_path)
+def load_damaged_bdf(file_name: str):
+    file_path = os.path.join(assets_dir, 'damaged', file_name)
+    bdffont.load_bdf(file_path)
 
 
 def test_not_a_bdf():
     with pytest.raises(Exception) as info:
         load_damaged_bdf('not_a_bdf.bdf')
     assert info.type == BdfMissingLine
     assert info.value.word == 'STARTFONT'
```

### Comparing `bdffont-0.0.5/tests/test_demo.py` & `bdffont-0.0.6/tests/test_demo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import os
 
 import bdffont
 from bdffont import BdfFont
 from tests import assets_dir, outputs_dir
 
 
-def load_bdf(bdf_file_name: str | bytes | os.PathLike[str] | os.PathLike[bytes]) -> tuple[BdfFont, str]:
-    bdf_file_path = os.path.join(assets_dir, bdf_file_name)
-    with open(bdf_file_path, 'r', encoding='utf-8') as file:
+def load_bdf(file_name: str) -> tuple[BdfFont, str]:
+    file_path = os.path.join(assets_dir, file_name)
+    with open(file_path, 'r', encoding='utf-8') as file:
         bdf_text = file.read()
     font = bdffont.decode_bdf_str(bdf_text)
     return font, bdf_text
 
 
 def test_example():
     font, bdf_text = load_bdf('example.bdf')
     assert font.encode_str() == bdf_text
+    assert font.spec_version == '2.1'
     assert font.name == '-Adobe-Helvetica-Bold-R-Normal--24-240-75-75-P-65-ISO8859-1'
-    assert font.size == (24, 75, 75)
     assert font.point_size == 24
-    assert font.xy_dpi == (75, 75)
-    assert font.x_dpi == 75
-    assert font.y_dpi == 75
-    assert font.bounding_box == (9, 24, -2, -6)
-    assert font.bounding_box_size == (9, 24)
+    assert font.dpi_x == 75
+    assert font.dpi_y == 75
+    assert font.dpi_xy == (75, 75)
     assert font.bounding_box_width == 9
     assert font.bounding_box_height == 24
-    assert font.bounding_box_origin == (-2, -6)
-    assert font.bounding_box_origin_x == -2
-    assert font.bounding_box_origin_y == -6
+    assert font.bounding_box_size == (9, 24)
+    assert font.bounding_box_offset_x == -2
+    assert font.bounding_box_offset_y == -6
+    assert font.bounding_box_offset == (-2, -6)
+    assert font.bounding_box == (9, 24, -2, -6)
     assert len(font.properties) == 19
     assert font.properties.foundry == 'Adobe'
     assert font.properties['FAMILY'] == 'Helvetica'
     assert font.properties.weight_name == 'Bold'
     assert font.properties.slant == 'R'
     assert font.properties['SETWIDTH_NAME'] == 'Normal'
     assert font.properties['ADD_STYLE_NAME'] == ''
@@ -49,27 +49,27 @@
     assert font.properties.font_descent == 7
     assert font.properties.copyright == 'Copyright (c) 1987 Adobe Systems, Inc.'
     assert font.properties.notice == 'Helvetica is a registered trademark of Linotype Inc.'
     assert len(font.code_point_to_glyph) == 2
     glyph = font.get_glyph(39)
     assert glyph.name == 'quoteright'
     assert glyph.code_point == 39
-    assert glyph.scalable_width == (223, 0)
     assert glyph.scalable_width_x == 223
     assert glyph.scalable_width_y == 0
-    assert glyph.device_width == (5, 0)
+    assert glyph.scalable_width == (223, 0)
     assert glyph.device_width_x == 5
     assert glyph.device_width_y == 0
-    assert glyph.bounding_box == (4, 6, 2, 12)
-    assert glyph.bounding_box_size == (4, 6)
+    assert glyph.device_width == (5, 0)
     assert glyph.bounding_box_width == 4
     assert glyph.bounding_box_height == 6
-    assert glyph.bounding_box_origin == (2, 12)
-    assert glyph.bounding_box_origin_x == 2
-    assert glyph.bounding_box_origin_y == 12
+    assert glyph.bounding_box_size == (4, 6)
+    assert glyph.bounding_box_offset_x == 2
+    assert glyph.bounding_box_offset_y == 12
+    assert glyph.bounding_box_offset == (2, 12)
+    assert glyph.bounding_box == (4, 6, 2, 12)
     assert len(glyph.bitmap) == 6
     glyph_data = [
         '_###____',
         '_###____',
         '_###____',
         '_##_____',
         '###_____',
@@ -78,9 +78,13 @@
     for i, bitmap_row in enumerate(glyph.bitmap):
         assert ''.join(map(str, bitmap_row)).replace('0', '_').replace('1', '#') == glyph_data[i]
     font.save(os.path.join(outputs_dir, 'example-output.bdf'))
 
 
 def test_unifont():
     font = load_bdf('unifont-15.0.01.bdf')[0]
-    font = bdffont.decode_bdf(iter(font.encode()))
     font.save(os.path.join(outputs_dir, 'unifont-output.bdf'))
+
+
+def test_galmuri9():
+    font = load_bdf('galmuri9.bdf')[0]
+    font.save(os.path.join(outputs_dir, 'galmuri9-output.bdf'))
```

### Comparing `bdffont-0.0.5/tests/test_type.py` & `bdffont-0.0.6/tests/test_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 import pytest
 
 from bdffont import BdfFont, BdfProperties, BdfGlyph
-from bdffont.error import BdfPropertiesIllegalKey, BdfPropertiesIllegalValue
+from bdffont.error import BdfIllegalPropertiesKey, BdfIllegalPropertiesValue
 
 
 def test_font():
     font = BdfFont(
         name='',
-        size=(0, 0, 0),
-        bounding_box=(0, 0, 0, 0),
+        point_size=0,
+        dpi_xy=(0, 0),
+        bounding_box_size=(0, 0),
+        bounding_box_offset=(0, 0),
     )
 
-    font.point_size = 1
-    assert font.point_size == 1
-    assert font.size == (1, 0, 0)
-    font.xy_dpi = (2, 3)
-    assert font.xy_dpi == (2, 3)
-    assert font.size == (1, 2, 3)
-    font.x_dpi = 4
-    assert font.x_dpi == 4
-    assert font.size == (1, 4, 3)
-    font.y_dpi = 5
-    assert font.y_dpi == 5
-    assert font.size == (1, 4, 5)
-
-    font.bounding_box_size = (6, 7)
-    assert font.bounding_box_size == (6, 7)
-    assert font.bounding_box == (6, 7, 0, 0)
-    font.bounding_box_width = 8
-    assert font.bounding_box_width == 8
-    assert font.bounding_box == (8, 7, 0, 0)
-    font.bounding_box_height = 9
-    assert font.bounding_box_height == 9
-    assert font.bounding_box == (8, 9, 0, 0)
-    font.bounding_box_origin = (10, 11)
-    assert font.bounding_box_origin == (10, 11)
-    assert font.bounding_box == (8, 9, 10, 11)
-    font.bounding_box_origin_x = 12
-    assert font.bounding_box_origin_x == 12
-    assert font.bounding_box == (8, 9, 12, 11)
-    font.bounding_box_origin_y = 13
-    assert font.bounding_box_origin_y == 13
-    assert font.bounding_box == (8, 9, 12, 13)
+    font.dpi_xy = 1, 2
+    assert font.dpi_xy == (1, 2)
+    assert font.dpi_x == 1
+    assert font.dpi_y == 2
+
+    font.bounding_box_size = 3, 4
+    assert font.bounding_box_size == (3, 4)
+    assert font.bounding_box_width == 3
+    assert font.bounding_box_height == 4
+
+    font.bounding_box_offset = 5, 6
+    assert font.bounding_box_offset == (5, 6)
+    assert font.bounding_box_offset_x == 5
+    assert font.bounding_box_offset_y == 6
+
+    assert font.bounding_box == (3, 4, 5, 6)
+    font.bounding_box = 7, 8, 9, 10
+    assert font.bounding_box == (7, 8, 9, 10)
+    assert font.bounding_box_width == 7
+    assert font.bounding_box_height == 8
+    assert font.bounding_box_offset_x == 9
+    assert font.bounding_box_offset_y == 10
 
 
 def test_properties():
     properties = BdfProperties()
 
     properties.default_char = 1
     assert properties.default_char == 1
@@ -115,55 +108,51 @@
     assert properties.notice == 'H'
     assert 'NOTICE' in properties
 
     assert len(properties) == 17
 
     with pytest.raises(Exception) as info:
         properties['abc'] = 'def'
-    assert info.type == BdfPropertiesIllegalKey
+    assert info.type == BdfIllegalPropertiesKey
 
     with pytest.raises(Exception) as info:
         properties['TEST_KEY'] = float(1.2)
-    assert info.type == BdfPropertiesIllegalValue
+    assert info.type == BdfIllegalPropertiesValue
 
 
 def test_glyph():
     glyph = BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(0, 0),
         device_width=(0, 0),
-        bounding_box=(0, 0, 0, 0),
+        bounding_box_size=(0, 0),
+        bounding_box_offset=(0, 0),
     )
 
-    glyph.scalable_width_x = 1
+    glyph.scalable_width = 1, 2
+    assert glyph.scalable_width == (1, 2)
     assert glyph.scalable_width_x == 1
-    assert glyph.scalable_width == (1, 0)
-    glyph.scalable_width_y = 2
     assert glyph.scalable_width_y == 2
-    assert glyph.scalable_width == (1, 2)
 
-    glyph.device_width_x = 3
+    glyph.device_width = 3, 4
+    assert glyph.device_width == (3, 4)
     assert glyph.device_width_x == 3
-    assert glyph.device_width == (3, 0)
-    glyph.device_width_y = 4
     assert glyph.device_width_y == 4
-    assert glyph.device_width == (3, 4)
 
-    glyph.bounding_box_size = (5, 6)
+    glyph.bounding_box_size = 5, 6
     assert glyph.bounding_box_size == (5, 6)
-    assert glyph.bounding_box == (5, 6, 0, 0)
-    glyph.bounding_box_width = 7
-    assert glyph.bounding_box_width == 7
-    assert glyph.bounding_box == (7, 6, 0, 0)
-    glyph.bounding_box_height = 8
-    assert glyph.bounding_box_height == 8
-    assert glyph.bounding_box == (7, 8, 0, 0)
-    glyph.bounding_box_origin = (9, 10)
-    assert glyph.bounding_box_origin == (9, 10)
-    assert glyph.bounding_box == (7, 8, 9, 10)
-    glyph.bounding_box_origin_x = 11
-    assert glyph.bounding_box_origin_x == 11
-    assert glyph.bounding_box == (7, 8, 11, 10)
-    glyph.bounding_box_origin_y = 12
-    assert glyph.bounding_box_origin_y == 12
-    assert glyph.bounding_box == (7, 8, 11, 12)
+    assert glyph.bounding_box_width == 5
+    assert glyph.bounding_box_height == 6
+
+    glyph.bounding_box_offset = 7, 8
+    assert glyph.bounding_box_offset == (7, 8)
+    assert glyph.bounding_box_offset_x == 7
+    assert glyph.bounding_box_offset_y == 8
+
+    assert glyph.bounding_box == (5, 6, 7, 8)
+    glyph.bounding_box = 9, 10, 11, 12
+    assert glyph.bounding_box == (9, 10, 11, 12)
+    assert glyph.bounding_box_width == 9
+    assert glyph.bounding_box_height == 10
+    assert glyph.bounding_box_offset_x == 11
+    assert glyph.bounding_box_offset_y == 12
```

