# Comparing `tmp/enex2notion-0.2.8.tar.gz` & `tmp/enex2notion-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enex2notion-0.2.8.tar", max compression
+gzip compressed data, was "enex2notion-0.2.9.tar", max compression
```

## Comparing `enex2notion-0.2.8.tar` & `enex2notion-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,40 @@
--rw-r--r--   0        0        0     7894 2022-04-08 11:04:10.702819 enex2notion-0.2.8/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2022-04-08 11:04:10.702819 enex2notion-0.2.8/LICENSE
--rw-r--r--   0        0        0     7827 2022-04-08 11:04:10.702819 enex2notion-0.2.8/README.md
--rw-r--r--   0        0        0        0 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/__init__.py
--rw-r--r--   0        0        0       92 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/__main__.py
--rw-r--r--   0        0        0     8922 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/cli.py
--rw-r--r--   0        0        0      961 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/cli_wkhtmltopdf.py
--rw-r--r--   0        0        0     4689 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/colors.py
--rw-r--r--   0        0        0     3783 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/enex_parser.py
--rw-r--r--   0        0        0     1239 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/enex_types.py
--rw-r--r--   0        0        0     2292 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/enex_uploader.py
--rw-r--r--   0        0        0     2829 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/enex_uploader_modes.py
--rw-r--r--   0        0        0     5285 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser.py
--rw-r--r--   0        0        0     2496 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_blocks.py
--rw-r--r--   0        0        0     1325 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_e_div.py
--rw-r--r--   0        0        0     2594 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_e_media.py
--rw-r--r--   0        0        0      865 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_e_table.py
--rw-r--r--   0        0        0     2928 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_elements.py
--rw-r--r--   0        0        0     3222 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_helpers.py
--rw-r--r--   0        0        0     2775 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_indented.py
--rw-r--r--   0        0        0     6816 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_webclip.py
--rw-r--r--   0        0        0     2825 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_parser_webclip_pdf.py
--rw-r--r--   0        0        0     1827 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/note_uploader.py
--rw-r--r--   0        0        0     2130 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/notion_blocks.py
--rw-r--r--   0        0        0      486 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/notion_blocks_container.py
--rw-r--r--   0        0        0     1069 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/notion_blocks_embeddable.py
--rw-r--r--   0        0        0      317 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/notion_blocks_header.py
--rw-r--r--   0        0        0      439 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/notion_blocks_list.py
--rw-r--r--   0        0        0     1074 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/notion_blocks_table.py
--rw-r--r--   0        0        0      869 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/notion_blocks_uploadable.py
--rw-r--r--   0        0        0      453 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/notion_filetypes.py
--rw-r--r--   0        0        0      376 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/rand_id.py
--rw-r--r--   0        0        0     4002 2022-04-08 11:04:10.702819 enex2notion-0.2.8/enex2notion/string_extractor.py
--rw-r--r--   0        0        0     1318 2022-04-08 11:04:10.706819 enex2notion-0.2.8/enex2notion/string_extractor_properties.py
--rw-r--r--   0        0        0       22 2022-04-08 11:04:10.706819 enex2notion-0.2.8/enex2notion/version.py
--rw-r--r--   0        0        0     3349 2022-04-08 11:04:10.706819 enex2notion-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     9105 2022-04-08 11:04:18.951082 enex2notion-0.2.8/setup.py
--rw-r--r--   0        0        0     9421 2022-04-08 11:04:18.951946 enex2notion-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     8155 2022-04-11 12:36:35.096647 enex2notion-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2022-04-11 12:36:35.096647 enex2notion-0.2.9/LICENSE
+-rw-r--r--   0        0        0     7827 2022-04-11 12:36:35.096647 enex2notion-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/__init__.py
+-rw-r--r--   0        0        0       92 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/__main__.py
+-rw-r--r--   0        0        0     8922 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/cli.py
+-rw-r--r--   0        0        0      961 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/cli_wkhtmltopdf.py
+-rw-r--r--   0        0        0     4689 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/colors.py
+-rw-r--r--   0        0        0     3783 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/enex_parser.py
+-rw-r--r--   0        0        0     1239 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/enex_types.py
+-rw-r--r--   0        0        0     2292 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/enex_uploader.py
+-rw-r--r--   0        0        0     2829 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/enex_uploader_modes.py
+-rw-r--r--   0        0        0     3490 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser.py
+-rw-r--r--   0        0        0     2538 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_blocks.py
+-rw-r--r--   0        0        0     2222 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_condense.py
+-rw-r--r--   0        0        0     1367 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_e_div.py
+-rw-r--r--   0        0        0     2594 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_e_media.py
+-rw-r--r--   0        0        0      870 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_e_table.py
+-rw-r--r--   0        0        0     2933 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_elements.py
+-rw-r--r--   0        0        0     3222 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_helpers.py
+-rw-r--r--   0        0        0     2775 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_indented.py
+-rw-r--r--   0        0        0     6816 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_webclip.py
+-rw-r--r--   0        0        0     2825 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_parser_webclip_pdf.py
+-rw-r--r--   0        0        0     1827 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/note_uploader.py
+-rw-r--r--   0        0        0      989 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_blocks.py
+-rw-r--r--   0        0        0      491 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_blocks_container.py
+-rw-r--r--   0        0        0     1069 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_blocks_embeddable.py
+-rw-r--r--   0        0        0      322 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_blocks_header.py
+-rw-r--r--   0        0        0      444 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_blocks_list.py
+-rw-r--r--   0        0        0     1116 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_blocks_table.py
+-rw-r--r--   0        0        0     2454 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_blocks_text.py
+-rw-r--r--   0        0        0      869 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_blocks_uploadable.py
+-rw-r--r--   0        0        0      453 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/notion_filetypes.py
+-rw-r--r--   0        0        0      376 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/rand_id.py
+-rw-r--r--   0        0        0     4007 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/string_extractor.py
+-rw-r--r--   0        0        0     1318 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/string_extractor_properties.py
+-rw-r--r--   0        0        0       22 2022-04-11 12:36:35.096647 enex2notion-0.2.9/enex2notion/version.py
+-rw-r--r--   0        0        0     3349 2022-04-11 12:36:35.096647 enex2notion-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     9105 2022-04-11 12:36:42.931666 enex2notion-0.2.9/setup.py
+-rw-r--r--   0        0        0     9421 2022-04-11 12:36:42.932448 enex2notion-0.2.9/PKG-INFO
```

### Comparing `enex2notion-0.2.8/CHANGELOG.md` & `enex2notion-0.2.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+### [0.2.9](https://github.com/vzhd1701/enex2notion/compare/v0.2.8...v0.2.9) (2022-04-11)
+
+### Bug Fixes
+
+- trim paragraphs when condense lines option is used ([9403e47](https://github.com/vzhd1701/enex2notion/commit/9403e470363e18719eded106ba61962e01eb6c38))
+
 ### [0.2.8](https://github.com/vzhd1701/enex2notion/compare/v0.2.7...v0.2.8) (2022-04-08)
 
 ### Features
 
 - add option to condense lines into paragraphs (sparse) ([58b9a95](https://github.com/vzhd1701/enex2notion/commit/58b9a95f73e36f0d6fcccaf3e2419d8a0f39f62d))
 - add option to set custom root page name ([2a7b2ce](https://github.com/vzhd1701/enex2notion/commit/2a7b2cee315703d1fce26a3fda77c4e213eeea60))
 - add option to set custom tag for uploaded pages ([1c385e1](https://github.com/vzhd1701/enex2notion/commit/1c385e1b2a42f04a6475c44a8b9c0af3bf2a69d7)), closes [#23](https://github.com/vzhd1701/enex2notion/issues/23)
```

### Comparing `enex2notion-0.2.8/LICENSE` & `enex2notion-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/README.md` & `enex2notion-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/cli.py` & `enex2notion-0.2.9/enex2notion/cli.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/cli_wkhtmltopdf.py` & `enex2notion-0.2.9/enex2notion/cli_wkhtmltopdf.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/colors.py` & `enex2notion-0.2.9/enex2notion/colors.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/enex_parser.py` & `enex2notion-0.2.9/enex2notion/enex_parser.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/enex_types.py` & `enex2notion-0.2.9/enex2notion/enex_types.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/enex_uploader.py` & `enex2notion-0.2.9/enex2notion/enex_uploader.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/enex_uploader_modes.py` & `enex2notion-0.2.9/enex2notion/enex_uploader_modes.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_blocks.py` & `enex2notion-0.2.9/enex2notion/note_parser_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from enex2notion.note_parser_helpers import extract_nested_blocks, flatten_root
 from enex2notion.note_parser_indented import (
     group_blocks_by_indent,
     is_indentation_inconsistent,
     parse_indented,
     parse_indented_plain,
 )
-from enex2notion.notion_blocks import NotionDividerBlock, NotionTextBlock, TextProp
+from enex2notion.notion_blocks import NotionDividerBlock
+from enex2notion.notion_blocks_text import NotionTextBlock, TextProp
 
 logger = logging.getLogger(__name__)
 
 
 def parse_note_blocks(note: Tag):
     flatten_root(note)
```

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_e_div.py` & `enex2notion-0.2.9/enex2notion/note_parser_e_div.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import re
 
 from bs4 import Tag
 
-from enex2notion.notion_blocks import NotionBookmarkBlock, NotionTextBlock
+from enex2notion.notion_blocks import NotionBookmarkBlock
 from enex2notion.notion_blocks_container import NotionCodeBlock
 from enex2notion.notion_blocks_list import NotionTodoBlock
+from enex2notion.notion_blocks_text import NotionTextBlock
 from enex2notion.string_extractor import extract_string
 
 logger = logging.getLogger(__name__)
 
 
 def parse_div(element: Tag):
     style = element.get("style", "")
```

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_e_media.py` & `enex2notion-0.2.9/enex2notion/note_parser_e_media.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_e_table.py` & `enex2notion-0.2.9/enex2notion/note_parser_e_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bs4 import Tag
 
-from enex2notion.notion_blocks import TextProp
 from enex2notion.notion_blocks_table import NotionTableBlock
+from enex2notion.notion_blocks_text import TextProp
 from enex2notion.string_extractor import extract_string
 
 
 def parse_table(element):
     rows = _convert_table_into_rows(element)
 
     if not rows:
```

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_elements.py` & `enex2notion-0.2.9/enex2notion/note_parser_elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 
 from bs4 import NavigableString, Tag
 
 from enex2notion.note_parser_e_media import parse_img, parse_media
-from enex2notion.notion_blocks import NotionTextBlock, TextProp
 from enex2notion.notion_blocks_header import (
     NotionHeaderBlock,
     NotionSubheaderBlock,
     NotionSubsubheaderBlock,
 )
 from enex2notion.notion_blocks_list import (
     NotionBulletedListBlock,
     NotionNumberedListBlock,
     NotionTodoBlock,
 )
+from enex2notion.notion_blocks_text import NotionTextBlock, TextProp
 from enex2notion.string_extractor import extract_string
 
 logger = logging.getLogger(__name__)
 
 
 def parse_encrypt(element: Tag):
     logger.warning("Skipping encrypted block")
```

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_helpers.py` & `enex2notion-0.2.9/enex2notion/note_parser_helpers.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_indented.py` & `enex2notion-0.2.9/enex2notion/note_parser_indented.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_webclip.py` & `enex2notion-0.2.9/enex2notion/note_parser_webclip.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/note_parser_webclip_pdf.py` & `enex2notion-0.2.9/enex2notion/note_parser_webclip_pdf.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/note_uploader.py` & `enex2notion-0.2.9/enex2notion/note_uploader.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/notion_blocks.py` & `enex2notion-0.2.9/enex2notion/notion_blocks_text.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 from notion import block
 
+from enex2notion.notion_blocks import NotionBaseBlock
+
+
+def _lstrip_properties(properties):
+    strip_properties = []
+
+    for i, prop in enumerate(properties):
+        if not prop[0].strip():
+            continue
+
+        if len(prop) == 1:
+            strip_properties.append([prop[0].lstrip()])
+        else:
+            strip_properties.append([prop[0].lstrip(), prop[1]])
+
+        strip_properties.extend(properties[i + 1 :])
+
+        break
+
+    return strip_properties
+
+
+def _rstrip_properties(properties):
+    strip_properties = []
+
+    for i, prop in sorted(enumerate(properties), reverse=True):
+        if not prop[0].strip():
+            continue
+
+        strip_properties.extend(properties[:i])
+
+        if len(prop) == 1:
+            strip_properties.append([prop[0].rstrip()])
+        else:
+            strip_properties.append([prop[0].rstrip(), prop[1]])
+
+        break
+
+    return strip_properties
+
 
 class TextProp(object):
     def __init__(self, text, properties=None):
         self.text = text
 
         self.properties = [[text]] if properties is None else properties
 
         if properties is None:
             self.properties = [[text]] if text else []
 
-    def __eq__(self, other):
-        return self.text == other.text and self.properties == other.properties
-
-    def __repr__(self):  # pragma: no cover
-        return "<{0}> {1}".format(self.__class__.__name__, self.text)
-
-
-class NotionBaseBlock(object):
-    type = None
+    def strip(self):
+        strip_properties = _rstrip_properties(_lstrip_properties(self.properties))
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-        self.attrs = {}
-        self.properties = {}
-        self.children = []
+        return TextProp(text=self.text.strip(), properties=strip_properties)
 
     def __eq__(self, other):
-        return (
-            self.type == other.type
-            and self.attrs == other.attrs
-            and self.properties == other.properties
-            and self.children == other.children
-        )
+        return self.text == other.text and self.properties == other.properties
 
     def __repr__(self):  # pragma: no cover
-        return "<{class_name}> {type} C:{c_count} {attrs}".format(
-            class_name=self.__class__.__name__,
-            type=self.type,
-            c_count=len(self.children),
-            attrs=self.attrs,
-        )
+        return "<{0}> {1}".format(self.__class__.__name__, self.text)
 
 
 class NotionTextBased(NotionBaseBlock):
     def __init__(self, text_prop: TextProp = None, **kwargs):
         super().__init__(**kwargs)
 
         if text_prop:
@@ -58,23 +76,15 @@
     @property
     def text_prop(self):
         return TextProp(
             text=self.attrs["title_plaintext"],
             properties=self.properties["properties.title"],
         )
 
+    @text_prop.setter
+    def text_prop(self, text_prop: TextProp):
+        self.attrs["title_plaintext"] = text_prop.text
+        self.properties["properties.title"] = text_prop.properties
+
 
 class NotionTextBlock(NotionTextBased):
     type = block.TextBlock
-
-
-class NotionDividerBlock(NotionBaseBlock):
-    type = block.DividerBlock
-
-
-class NotionBookmarkBlock(NotionBaseBlock):
-    type = block.BookmarkBlock
-
-    def __init__(self, url, **kwargs):
-        super().__init__(**kwargs)
-
-        self.attrs["link"] = url
```

### Comparing `enex2notion-0.2.8/enex2notion/notion_blocks_embeddable.py` & `enex2notion-0.2.9/enex2notion/notion_blocks_embeddable.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/notion_blocks_table.py` & `enex2notion-0.2.9/enex2notion/notion_blocks_table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Iterable
 
 from notion.block import BasicBlock
 
-from enex2notion.notion_blocks import NotionBaseBlock, NotionTextBased, TextProp
+from enex2notion.notion_blocks import NotionBaseBlock
+from enex2notion.notion_blocks_text import NotionTextBased, TextProp
 from enex2notion.rand_id import rand_id_list
 
 
 class TableBlock(BasicBlock):
 
     _type = "table"
```

### Comparing `enex2notion-0.2.8/enex2notion/notion_blocks_uploadable.py` & `enex2notion-0.2.9/enex2notion/notion_blocks_uploadable.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/enex2notion/string_extractor.py` & `enex2notion-0.2.9/enex2notion/string_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 from typing import List
 
 from bs4 import NavigableString, Tag
 
-from enex2notion.notion_blocks import TextProp
+from enex2notion.notion_blocks_text import TextProp
 from enex2notion.string_extractor_properties import resolve_string_properties
 
 STANDALONES = ("h1", "h2", "h3", "div")
 
 
 def extract_string(tag: Tag) -> TextProp:
     """Convert a block content into a string with properties
```

### Comparing `enex2notion-0.2.8/enex2notion/string_extractor_properties.py` & `enex2notion-0.2.9/enex2notion/string_extractor_properties.py`

 * *Files identical despite different names*

### Comparing `enex2notion-0.2.8/pyproject.toml` & `enex2notion-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "enex2notion"
-version = "0.2.8"
+version = "0.2.9"
 description = "Import Evernote ENEX files to Notion"
 authors = ["vzhd1701 <vzhd1701@gmail.com>"]
 readme = "README.md"
 include = ["CHANGELOG.md"]
 license = "MIT"
 repository = "https://github.com/vzhd1701/enex2notion"
 keywords = ["evernote", "enex", "notion", "import"]
```

### Comparing `enex2notion-0.2.8/setup.py` & `enex2notion-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {':python_version < "3.7"': ['dataclasses>=0.6']}
 
 entry_points = \
 {'console_scripts': ['enex2notion = enex2notion.cli:main']}
 
 setup_kwargs = {
     'name': 'enex2notion',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Import Evernote ENEX files to Notion',
     'long_description': '# enex2notion\n\n[![PyPI version](https://img.shields.io/pypi/v/enex2notion?label=version)](https://pypi.python.org/pypi/enex2notion)\n[![Python Version](https://img.shields.io/pypi/pyversions/enex2notion.svg)](https://pypi.org/project/enex2notion/)\n[![tests](https://github.com/vzhd1701/enex2notion/actions/workflows/test.yml/badge.svg)](https://github.com/vzhd1701/enex2notion/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/vzhd1701/enex2notion/branch/master/graph/badge.svg)](https://codecov.io/gh/vzhd1701/enex2notion)\n\nEasy way to import [Evernote\'s](https://www.evernote.com/) `*.enex` files to [Notion.so](https://notion.so)\n\nNotion\'s native Evernote importer doesn\'t do it for me, so I decided to write my own. Thanks to **Cobertos** and [md2notion](https://github.com/Cobertos/md2notion) for inspiration and **Jamie Alexandre** for [notion-py](https://github.com/jamalex/notion-py).\n\nYou can either use Evernote native export or try out my other tool, [evernote-backup](https://github.com/vzhd1701/evernote-backup), to export `*.enex` files from Evernote.\n\n### What is preserved\n\n- Embedded files and images are uploaded to Notion\n  - nested images will appear after paragraph\n- Text formatting (**bold**, _italic_, etc) and colors\n- Tables are converted to the new format (no colspans though)\n- Web Clips\n  - as plain text or PDFs, see [below](#web-clips)\n- Everything else basically\n\n### What is lost\n\n- Paragraph alignment\n- Subscript and superscript formatting\n- Custom fonts and font sizes\n- Tasks\n- Encrypted blocks\n  - just decrypt them before export\n\n## Installation\n\n[**Download the latest binary release**](https://github.com/vzhd1701/enex2notion/releases/latest) for your OS.\n\n### With PIP\n\n```bash\n$ pip install enex2notion\n```\n\n**Python 3.6 or later required.**\n\nOr, since **enex2notion** is a standalone tool, it might be more convenient to install it using [**pipx**](https://github.com/pipxproject/pipx):\n\n```shell\n$ pipx install enex2notion\n```\n\n### From source\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management and packaging. You will have to install it first. See [poetry official documentation](https://python-poetry.org/docs/) for instructions.\n\n```shell\n$ git clone https://github.com/vzhd1701/enex2notion.git\n$ cd enex2notion/\n$ poetry install --no-dev\n$ poetry run enex2notion\n```\n\n## Usage\n\n```shell\n$ enex2notion --help\nusage: enex2notion [-h] [--token TOKEN] [--root-page NAME] [--mode {DB,PAGE}] [--mode-webclips {TXT,PDF}] [--add-pdf-preview] [--add-meta] [--tag TAG] [--condense-lines] [--condense-lines-sparse] [--done-file FILE] [--log FILE]\n                   [--verbose] [--version]\n                   FILE/DIR [FILE/DIR ...]\n\nUploads ENEX files to Notion\n\npositional arguments:\n  FILE/DIR              ENEX files or directories to upload\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --token TOKEN         Notion token, stored in token_v2 cookie for notion.so [NEEDED FOR UPLOAD]\n  --root-page NAME      root page name for the imported notebooks, it will be created if it does not exist (default: "Evernote ENEX Import")\n  --mode {DB,PAGE}      upload each ENEX as database (DB) or page with children (PAGE) (default: DB)\n  --mode-webclips {TXT,PDF}\n                        convert web clips to text (TXT) or pdf (PDF) before upload (default: TXT)\n  --add-pdf-preview     include preview image with PDF webclips for gallery view thumbnail (works only with --mode-webclips=PDF)\n  --add-meta            include metadata (created, tags, etc) in notes, makes sense only with PAGE mode\n  --tag TAG             add custom tag to uploaded notes\n  --condense-lines      condense text lines together into paragraphs to avoid making block per line\n  --condense-lines-sparse\n                        like --condense-lines but leaves gaps between paragraphs\n  --done-file FILE      file for uploaded notes hashes to resume interrupted upload\n  --log FILE            file to store program log\n  --verbose             output debug information\n  --version             show program\'s version number and exit\n```\n\n### Input\n\nYou can pass single `*.enex` files or directories. The program will recursively scan directories for `*.enex` files.\n\n### Token & dry run mode\n\nThe upload requires you to have a `token_v2` cookie for the Notion website. For information on how to get it, see [this article](https://vzhd1701.notion.site/Find-Your-Notion-Token-5f57951434c1414d84ac72f88226eede).\n\nThe program can run without `--token` provided though. It will not make any network requests without it. Executing a dry run with `--verbose` is an excellent way to check if your `*.enex` files are parsed correctly before uploading.\n\n### Upload continuation\n\nThe upload will take some time since each note is uploaded block-by-block, so you\'ll probably need some way of resuming it. `--done-file` is precisely for that. All uploaded note hashes will be stored there, so the next time you start, the upload will continue from where you left off.\n\nAll uploaded notebooks will appear under the automatically created `Evernote ENEX Import` page. You can change that name with the `--root-page` option. The program will mark unfinished notes with `[UNFINISHED UPLOAD]` text in the title. After successful upload, the mark will be removed.\n\n### Upload modes\n\nThe `--mode` option allows you to choose how to upload your notebooks: as databases or pages. `DB` mode is the default since Notion itself uses this mode when importing from Evernote. `PAGE` mode makes the tree feel like the original Evernote notebooks hierarchy.\n\nSince `PAGE` mode does not benefit from having separate space for metadata, you can still preserve the note\'s original meta with the `--add-meta` option. It will attach a callout block with all meta info as a first block in each note [like this](https://imgur.com/a/lJTbprH).\n\n### Web Clips\n\nDue to Notion\'s limitations Evernote web clips cannot be uploaded as-is. `enex2notion` provides two modes with the `--mode-webclips` option:\n\n- `TXT`, converting them to text, stripping all HTML formatting \\[Default\\]\n\n  - similar to Evernote\'s "Simplify & Make Editable"\n\n- `PDF`, converting them to PDF, keeping HTML formatting as close as possible\n\n  - web clips are converted using [wkhtmltopdf](https://wkhtmltopdf.org/), see [this page](https://github.com/JazzCore/python-pdfkit/wiki/Installing-wkhtmltopdf) on how to install it\n\nSince Notion\'s gallery view does not provide thumbnails for embedded PDFs, you have the `--add-pdf-preview` option to extract the first page of generated PDF as a preview for the web clip page.\n\n### Misc\n\nThe `--condense-lines` option is helpful if you want to save up some space and make notes look more compact. [Example](https://imgur.com/a/sV0X8z7).\n\nThe `--condense-lines-sparse` does the same thing as `--condense-lines`, but leaves gaps between paragraphs. [Example](https://imgur.com/a/OBzeqn7).\n\nThe `--tag` option allows you to add a custom tag to all uploaded notes. It will add this tag to existing tags if the note already has any.\n\n## Examples\n\n### Checking notes before upload\n\n```shell\n$ enex2notion --verbose my_notebooks/\n```\n\n### Uploading notes from a single notebook\n\n```shell\n$ enex2notion --token <YOUR_TOKEN_HERE> "notebook.enex"\n```\n\n### Uploading with the option to continue later\n\n```shell\n$ enex2notion --token <YOUR_TOKEN_HERE> --done-file done.txt "notebook.enex"\n```\n\n## Getting help\n\nIf you have encountered a bug or have an idea about a new feature, please [open a new issue](https://github.com/vzhd1701/enex2notion/issues/new/choose). If you have a question about the program or have difficulty using it, you are welcome to [the discussions page](https://github.com/vzhd1701/enex2notion/discussions). You can also mail me directly, I\'m always happy to help.\n',
     'author': 'vzhd1701',
     'author_email': 'vzhd1701@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/vzhd1701/enex2notion',
```

### Comparing `enex2notion-0.2.8/PKG-INFO` & `enex2notion-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enex2notion
-Version: 0.2.8
+Version: 0.2.9
 Summary: Import Evernote ENEX files to Notion
 Home-page: https://github.com/vzhd1701/enex2notion
 License: MIT
 Keywords: evernote,enex,notion,import
 Author: vzhd1701
 Author-email: vzhd1701@gmail.com
 Requires-Python: >=3.6.1,<4.0.0
```

