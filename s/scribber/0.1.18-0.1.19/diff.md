# Comparing `tmp/scribber-0.1.18.tar.gz` & `tmp/scribber-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribber-0.1.18.tar", last modified: Sat Apr 29 12:02:02 2023, max compression
+gzip compressed data, was "scribber-0.1.19.tar", last modified: Sat May  6 13:37:52 2023, max compression
```

## Comparing `scribber-0.1.18.tar` & `scribber-0.1.19.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/
--rw-rw-r--   0 sem       (1000) sem       (1000)     1072 2023-04-23 07:58:01.000000 scribber-0.1.18/LICENSE
--rw-rw-r--   0 sem       (1000) sem       (1000)     3624 2023-04-29 12:02:02.055511 scribber-0.1.18/PKG-INFO
--rw-rw-r--   0 sem       (1000) sem       (1000)     3005 2023-04-29 11:50:33.000000 scribber-0.1.18/README.md
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/
--rw-rw-r--   0 sem       (1000) sem       (1000)      380 2023-04-29 10:43:17.000000 scribber-0.1.18/scribber/__init__.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/core/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:19:56.000000 scribber-0.1.18/scribber/core/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     3472 2023-04-29 11:36:25.000000 scribber-0.1.18/scribber/core/document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/examples/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2023-04-23 07:28:29.000000 scribber-0.1.18/scribber/examples/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2315 2023-04-29 11:26:35.000000 scribber-0.1.18/scribber/examples/usage.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:25:48.000000 scribber-0.1.18/scribber/formats/__init__.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/excel/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:12.000000 scribber-0.1.18/scribber/formats/excel/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2227 2023-04-29 10:32:51.000000 scribber-0.1.18/scribber/formats/excel/excel_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/markdown/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:59:05.000000 scribber-0.1.18/scribber/formats/markdown/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     3941 2023-04-29 11:06:26.000000 scribber-0.1.18/scribber/formats/markdown/markdown_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/text/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:02.000000 scribber-0.1.18/scribber/formats/text/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2946 2023-04-29 10:32:33.000000 scribber-0.1.18/scribber/formats/text/text_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/word/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:50.000000 scribber-0.1.18/scribber/formats/word/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     1878 2023-04-29 11:44:52.000000 scribber-0.1.18/scribber/formats/word/word_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber.egg-info/
--rw-rw-r--   0 sem       (1000) sem       (1000)     3624 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/PKG-INFO
--rw-rw-r--   0 sem       (1000) sem       (1000)      651 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/SOURCES.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)        1 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/dependency_links.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)      147 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/requires.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)        9 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/top_level.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)       38 2023-04-29 12:02:02.055511 scribber-0.1.18/setup.cfg
--rw-rw-r--   0 sem       (1000) sem       (1000)     1185 2023-04-29 12:00:10.000000 scribber-0.1.18/setup.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1072 2023-04-23 07:58:01.000000 scribber-0.1.19/LICENSE
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3663 2023-05-06 13:37:52.609873 scribber-0.1.19/PKG-INFO
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3044 2023-05-06 13:37:34.000000 scribber-0.1.19/README.md
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber/
+-rw-rw-r--   0 sem       (1000) sem       (1000)      380 2023-04-29 10:43:17.000000 scribber-0.1.19/scribber/__init__.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber/core/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:19:56.000000 scribber-0.1.19/scribber/core/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3654 2023-05-06 13:30:48.000000 scribber-0.1.19/scribber/core/document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber/examples/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2023-04-23 07:28:29.000000 scribber-0.1.19/scribber/examples/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2354 2023-05-06 13:37:34.000000 scribber-0.1.19/scribber/examples/usage.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber/formats/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:25:48.000000 scribber-0.1.19/scribber/formats/__init__.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber/formats/excel/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:12.000000 scribber-0.1.19/scribber/formats/excel/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2227 2023-04-29 10:32:51.000000 scribber-0.1.19/scribber/formats/excel/excel_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber/formats/markdown/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:59:05.000000 scribber-0.1.19/scribber/formats/markdown/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3941 2023-04-29 11:06:26.000000 scribber-0.1.19/scribber/formats/markdown/markdown_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber/formats/text/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:02.000000 scribber-0.1.19/scribber/formats/text/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2946 2023-04-29 10:32:33.000000 scribber-0.1.19/scribber/formats/text/text_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber/formats/word/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:50.000000 scribber-0.1.19/scribber/formats/word/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1878 2023-04-29 11:44:52.000000 scribber-0.1.19/scribber/formats/word/word_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-05-06 13:37:52.609873 scribber-0.1.19/scribber.egg-info/
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3663 2023-05-06 13:37:52.000000 scribber-0.1.19/scribber.egg-info/PKG-INFO
+-rw-rw-r--   0 sem       (1000) sem       (1000)      651 2023-05-06 13:37:52.000000 scribber-0.1.19/scribber.egg-info/SOURCES.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)        1 2023-05-06 13:37:52.000000 scribber-0.1.19/scribber.egg-info/dependency_links.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)      147 2023-05-06 13:37:52.000000 scribber-0.1.19/scribber.egg-info/requires.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)        9 2023-05-06 13:37:52.000000 scribber-0.1.19/scribber.egg-info/top_level.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)       38 2023-05-06 13:37:52.609873 scribber-0.1.19/setup.cfg
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1185 2023-05-06 13:37:34.000000 scribber-0.1.19/setup.py
```

### Comparing `scribber-0.1.18/LICENSE` & `scribber-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `scribber-0.1.18/PKG-INFO` & `scribber-0.1.19/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribber
-Version: 0.1.18
+Version: 0.1.19
 Summary: A simple document generator with not very rich functionality that can export a document to some formats such as text, docx, xlsx and markdown.
 Home-page: https://github.com/edelwi/scribber
 Author: Evgeniy Semenov
 Author-email: edelwi@yandex.ru
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
@@ -38,15 +38,15 @@
     Table,
     Director,
     CodeBlock,
     DocumentBuilder,
     ExcelDocument,
     MarkdownDocument,
     TextDocument,
-    WordDocument
+    WordDocument,
 )
 
 CODE_EXAMPLE = """
 import platform
 
 def main():
     print("Hello World!")
@@ -72,25 +72,29 @@
             content=[
                 (1, 2, 3, 4),
                 ("234", 345, 986, ""),
                 (89, 35, 587643, 8675),
             ],
         )
     )
-    doc.add(EmptyLine())
-    doc.add(Title(title="Code block", level=2))
-    doc.add(CodeBlock(style="python", code=CODE_EXAMPLE))
-    doc.add(CodeBlock(style="console", code=CODE_RESULT))
-    doc.add(Paragraph(text="It's Ok!"))
+    doc.extend(
+        (
+            EmptyLine(),
+            Title(title="Code block", level=2),
+            CodeBlock(style="python", code=CODE_EXAMPLE),
+            CodeBlock(style="console", code=CODE_RESULT),
+            Paragraph(text="It's Ok!"),
+        )
+    )
 
     director = Director()
     text_report_builder = DocumentBuilder(doc=TextDocument())
     word_report_builder = DocumentBuilder(doc=WordDocument())
     excel_report_builder = DocumentBuilder(doc=ExcelDocument())
-    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
+    markdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
 
     print("Make a Text Document")
     director.builder = text_report_builder
     director.build_report_from_doc(doc)
     text_report_builder.parts.save("test.txt")
 
     print("Make a Word Document")
@@ -99,18 +103,18 @@
     word_report_builder.parts.save("test.docx")
 
     print("Make a Excel Document")
     director.builder = excel_report_builder
     director.build_report_from_doc(doc)
     excel_report_builder.parts.save("test.xlsx")
 
-    print("Make a Marckdown Document")
-    director.builder = marckdown_report_builder
+    print("Make a Markdown Document")
+    director.builder = markdown_report_builder
     director.build_report_from_doc(doc)
-    marckdown_report_builder.parts.save("test.md")
+    markdown_report_builder.parts.save("test.md")
 
     print()
     print("Build without Director")
     text_report_builder.add_title(Title(title="Next report"))
     text_report_builder.add_paragraph(Paragraph(text="That is all!"))
     print(text_report_builder.parts.get_result())
```

### Comparing `scribber-0.1.18/README.md` & `scribber-0.1.19/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Table,
     Director,
     CodeBlock,
     DocumentBuilder,
     ExcelDocument,
     MarkdownDocument,
     TextDocument,
-    WordDocument
+    WordDocument,
 )
 
 CODE_EXAMPLE = """
 import platform
 
 def main():
     print("Hello World!")
@@ -55,25 +55,29 @@
             content=[
                 (1, 2, 3, 4),
                 ("234", 345, 986, ""),
                 (89, 35, 587643, 8675),
             ],
         )
     )
-    doc.add(EmptyLine())
-    doc.add(Title(title="Code block", level=2))
-    doc.add(CodeBlock(style="python", code=CODE_EXAMPLE))
-    doc.add(CodeBlock(style="console", code=CODE_RESULT))
-    doc.add(Paragraph(text="It's Ok!"))
+    doc.extend(
+        (
+            EmptyLine(),
+            Title(title="Code block", level=2),
+            CodeBlock(style="python", code=CODE_EXAMPLE),
+            CodeBlock(style="console", code=CODE_RESULT),
+            Paragraph(text="It's Ok!"),
+        )
+    )
 
     director = Director()
     text_report_builder = DocumentBuilder(doc=TextDocument())
     word_report_builder = DocumentBuilder(doc=WordDocument())
     excel_report_builder = DocumentBuilder(doc=ExcelDocument())
-    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
+    markdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
 
     print("Make a Text Document")
     director.builder = text_report_builder
     director.build_report_from_doc(doc)
     text_report_builder.parts.save("test.txt")
 
     print("Make a Word Document")
@@ -82,18 +86,18 @@
     word_report_builder.parts.save("test.docx")
 
     print("Make a Excel Document")
     director.builder = excel_report_builder
     director.build_report_from_doc(doc)
     excel_report_builder.parts.save("test.xlsx")
 
-    print("Make a Marckdown Document")
-    director.builder = marckdown_report_builder
+    print("Make a Markdown Document")
+    director.builder = markdown_report_builder
     director.build_report_from_doc(doc)
-    marckdown_report_builder.parts.save("test.md")
+    markdown_report_builder.parts.save("test.md")
 
     print()
     print("Build without Director")
     text_report_builder.add_title(Title(title="Next report"))
     text_report_builder.add_paragraph(Paragraph(text="That is all!"))
     print(text_report_builder.parts.get_result())
```

### Comparing `scribber-0.1.18/scribber/core/document.py` & `scribber-0.1.19/scribber/core/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import abstractmethod
-from typing import Any, List, Protocol
+from typing import Any, List, Protocol, Iterable
 from pydantic import BaseModel, validator
 
 
 class Title(BaseModel):
     title: str
     level: int = 1
 
@@ -59,25 +59,32 @@
 class AbstractDocument(Protocol):
     def add(self, part: Any) -> None:
         ...
 
     def get_result(self) -> Any:
         ...
 
+    def extend(self, parts: Iterable[Any]) -> None:
+        ...
+
 
 class SimpleDocument:
     def __init__(self) -> None:
         self.parts = []
 
     def add(self, part: Any) -> None:
         self.parts.append(part)
 
     def get_result(self) -> List[Any]:
         return self.parts
 
+    def extend(self, parts: Iterable[Any]) -> None:
+        for item in parts:
+            self.add(item)
+
 
 class Builder(Protocol):
     @property
     @abstractmethod
     def parts(self) -> List:
         ...
```

### Comparing `scribber-0.1.18/scribber/examples/usage.py` & `scribber-0.1.19/scribber/examples/usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Table,
     Director,
     CodeBlock,
     DocumentBuilder,
     ExcelDocument,
     MarkdownDocument,
     TextDocument,
-    WordDocument
+    WordDocument,
 )
 
 CODE_EXAMPLE = """
 import platform
 
 def main():
     print("Hello World!")
@@ -40,25 +40,29 @@
             content=[
                 (1, 2, 3, 4),
                 ("234", 345, 986, ""),
                 (89, 35, 587643, 8675),
             ],
         )
     )
-    doc.add(EmptyLine())
-    doc.add(Title(title="Code block", level=2))
-    doc.add(CodeBlock(style="python", code=CODE_EXAMPLE))
-    doc.add(CodeBlock(style="console", code=CODE_RESULT))
-    doc.add(Paragraph(text="It's Ok!"))
+    doc.extend(
+        (
+            EmptyLine(),
+            Title(title="Code block", level=2),
+            CodeBlock(style="python", code=CODE_EXAMPLE),
+            CodeBlock(style="console", code=CODE_RESULT),
+            Paragraph(text="It's Ok!"),
+        )
+    )
 
     director = Director()
     text_report_builder = DocumentBuilder(doc=TextDocument())
     word_report_builder = DocumentBuilder(doc=WordDocument())
     excel_report_builder = DocumentBuilder(doc=ExcelDocument())
-    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
+    markdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
 
     print("Make a Text Document")
     director.builder = text_report_builder
     director.build_report_from_doc(doc)
     text_report_builder.parts.save("test.txt")
 
     print("Make a Word Document")
@@ -67,17 +71,17 @@
     word_report_builder.parts.save("test.docx")
 
     print("Make a Excel Document")
     director.builder = excel_report_builder
     director.build_report_from_doc(doc)
     excel_report_builder.parts.save("test.xlsx")
 
-    print("Make a Marckdown Document")
-    director.builder = marckdown_report_builder
+    print("Make a Markdown Document")
+    director.builder = markdown_report_builder
     director.build_report_from_doc(doc)
-    marckdown_report_builder.parts.save("test.md")
+    markdown_report_builder.parts.save("test.md")
 
     print()
     print("Build without Director")
     text_report_builder.add_title(Title(title="Next report"))
     text_report_builder.add_paragraph(Paragraph(text="That is all!"))
     print(text_report_builder.parts.get_result())
```

### Comparing `scribber-0.1.18/scribber/formats/excel/excel_document.py` & `scribber-0.1.19/scribber/formats/excel/excel_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.18/scribber/formats/markdown/markdown_document.py` & `scribber-0.1.19/scribber/formats/markdown/markdown_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.18/scribber/formats/text/text_document.py` & `scribber-0.1.19/scribber/formats/text/text_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.18/scribber/formats/word/word_document.py` & `scribber-0.1.19/scribber/formats/word/word_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.18/scribber.egg-info/PKG-INFO` & `scribber-0.1.19/scribber.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribber
-Version: 0.1.18
+Version: 0.1.19
 Summary: A simple document generator with not very rich functionality that can export a document to some formats such as text, docx, xlsx and markdown.
 Home-page: https://github.com/edelwi/scribber
 Author: Evgeniy Semenov
 Author-email: edelwi@yandex.ru
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
@@ -38,15 +38,15 @@
     Table,
     Director,
     CodeBlock,
     DocumentBuilder,
     ExcelDocument,
     MarkdownDocument,
     TextDocument,
-    WordDocument
+    WordDocument,
 )
 
 CODE_EXAMPLE = """
 import platform
 
 def main():
     print("Hello World!")
@@ -72,25 +72,29 @@
             content=[
                 (1, 2, 3, 4),
                 ("234", 345, 986, ""),
                 (89, 35, 587643, 8675),
             ],
         )
     )
-    doc.add(EmptyLine())
-    doc.add(Title(title="Code block", level=2))
-    doc.add(CodeBlock(style="python", code=CODE_EXAMPLE))
-    doc.add(CodeBlock(style="console", code=CODE_RESULT))
-    doc.add(Paragraph(text="It's Ok!"))
+    doc.extend(
+        (
+            EmptyLine(),
+            Title(title="Code block", level=2),
+            CodeBlock(style="python", code=CODE_EXAMPLE),
+            CodeBlock(style="console", code=CODE_RESULT),
+            Paragraph(text="It's Ok!"),
+        )
+    )
 
     director = Director()
     text_report_builder = DocumentBuilder(doc=TextDocument())
     word_report_builder = DocumentBuilder(doc=WordDocument())
     excel_report_builder = DocumentBuilder(doc=ExcelDocument())
-    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
+    markdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
 
     print("Make a Text Document")
     director.builder = text_report_builder
     director.build_report_from_doc(doc)
     text_report_builder.parts.save("test.txt")
 
     print("Make a Word Document")
@@ -99,18 +103,18 @@
     word_report_builder.parts.save("test.docx")
 
     print("Make a Excel Document")
     director.builder = excel_report_builder
     director.build_report_from_doc(doc)
     excel_report_builder.parts.save("test.xlsx")
 
-    print("Make a Marckdown Document")
-    director.builder = marckdown_report_builder
+    print("Make a Markdown Document")
+    director.builder = markdown_report_builder
     director.build_report_from_doc(doc)
-    marckdown_report_builder.parts.save("test.md")
+    markdown_report_builder.parts.save("test.md")
 
     print()
     print("Build without Director")
     text_report_builder.add_title(Title(title="Next report"))
     text_report_builder.add_paragraph(Paragraph(text="That is all!"))
     print(text_report_builder.parts.get_result())
```

### Comparing `scribber-0.1.18/scribber.egg-info/SOURCES.txt` & `scribber-0.1.19/scribber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scribber-0.1.18/setup.py` & `scribber-0.1.19/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scribber",
-    version="v0.1.18",
+    version="v0.1.19",
     author="Evgeniy Semenov",
     author_email="edelwi@yandex.ru",
     license="MIT",
     description="A simple document generator with not very rich functionality "
                 "that can export a document to some formats such as text, docx, "
                 "xlsx and markdown.",
     long_description=long_description,
```

