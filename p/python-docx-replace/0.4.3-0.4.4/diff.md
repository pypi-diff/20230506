# Comparing `tmp/python-docx-replace-0.4.3.tar.gz` & `tmp/python-docx-replace-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-docx-replace-0.4.3.tar", last modified: Tue Apr 11 23:02:21 2023, max compression
+gzip compressed data, was "python-docx-replace-0.4.4.tar", last modified: Sat May  6 21:16:06 2023, max compression
```

## Comparing `python-docx-replace-0.4.3.tar` & `python-docx-replace-0.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-04-11 23:02:21.055059 python-docx-replace-0.4.3/
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     1069 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/LICENSE
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     7236 2023-04-11 23:02:21.055149 python-docx-replace-0.4.3/PKG-INFO
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     6758 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/README.md
--rw-r--r--   0 ivanbicalho   (501) staff       (20)       84 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/pyproject.toml
--rw-r--r--   0 ivanbicalho   (501) staff       (20)      662 2023-04-11 23:02:21.055445 python-docx-replace-0.4.3/setup.cfg
-drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-04-11 23:02:21.052098 python-docx-replace-0.4.3/src/
-drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-04-11 23:02:21.053816 python-docx-replace-0.4.3/src/python_docx_replace/
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     6623 2023-04-11 23:00:27.000000 python-docx-replace-0.4.3/src/python_docx_replace/__init__.py
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     3676 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/src/python_docx_replace/block_handler.py
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     1161 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/src/python_docx_replace/exceptions.py
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     1571 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/src/python_docx_replace/key_changer.py
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     2638 2023-04-11 22:45:44.000000 python-docx-replace-0.4.3/src/python_docx_replace/paragraph.py
-drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-04-11 23:02:21.054920 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     7236 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/PKG-INFO
--rw-r--r--   0 ivanbicalho   (501) staff       (20)      467 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/SOURCES.txt
--rw-r--r--   0 ivanbicalho   (501) staff       (20)        1 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/dependency_links.txt
--rw-r--r--   0 ivanbicalho   (501) staff       (20)       12 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/requires.txt
--rw-r--r--   0 ivanbicalho   (501) staff       (20)       20 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/top_level.txt
+drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-05-06 21:16:06.200032 python-docx-replace-0.4.4/
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     1069 2022-10-31 14:53:42.000000 python-docx-replace-0.4.4/LICENSE
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     7513 2023-05-06 21:16:06.200110 python-docx-replace-0.4.4/PKG-INFO
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     7035 2023-05-06 21:15:14.000000 python-docx-replace-0.4.4/README.md
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)      115 2023-05-06 21:15:14.000000 python-docx-replace-0.4.4/pyproject.toml
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)      630 2023-05-06 21:16:06.200405 python-docx-replace-0.4.4/setup.cfg
+drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-05-06 21:16:06.197208 python-docx-replace-0.4.4/src/
+drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-05-06 21:16:06.199135 python-docx-replace-0.4.4/src/python_docx_replace/
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     7264 2023-05-06 21:15:14.000000 python-docx-replace-0.4.4/src/python_docx_replace/__init__.py
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     3760 2023-05-06 21:15:14.000000 python-docx-replace-0.4.4/src/python_docx_replace/block_handler.py
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     1161 2022-10-31 14:53:42.000000 python-docx-replace-0.4.4/src/python_docx_replace/exceptions.py
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     1599 2023-05-06 21:15:14.000000 python-docx-replace-0.4.4/src/python_docx_replace/key_changer.py
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     2697 2023-05-06 21:15:14.000000 python-docx-replace-0.4.4/src/python_docx_replace/paragraph.py
+drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-05-06 21:16:06.199816 python-docx-replace-0.4.4/src/python_docx_replace.egg-info/
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     7513 2023-05-06 21:16:06.000000 python-docx-replace-0.4.4/src/python_docx_replace.egg-info/PKG-INFO
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)      467 2023-05-06 21:16:06.000000 python-docx-replace-0.4.4/src/python_docx_replace.egg-info/SOURCES.txt
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)        1 2023-05-06 21:16:06.000000 python-docx-replace-0.4.4/src/python_docx_replace.egg-info/dependency_links.txt
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)       12 2023-05-06 21:16:06.000000 python-docx-replace-0.4.4/src/python_docx_replace.egg-info/requires.txt
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)       20 2023-05-06 21:16:06.000000 python-docx-replace-0.4.4/src/python_docx_replace.egg-info/top_level.txt
```

### Comparing `python-docx-replace-0.4.3/LICENSE` & `python-docx-replace-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-docx-replace-0.4.3/PKG-INFO` & `python-docx-replace-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docx-replace
-Version: 0.4.3
+Version: 0.4.4
 Summary: Replace words and remove blocks inside a Word document without losing format
 Home-page: https://github.com/ivanbicalho/python-docx-replace
 Author: Ivan Bicalho
 Author-email: ivanribeirob@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -120,14 +120,23 @@
 Indexes:         0   1   2   3   4   5   6      7  8  9 10 11 12  13  14  15  16  17  18  19  20  21  22
 Run Index:       0   0   0   0   0   0   0      0  0  0 1  1  1   1   1   1   1   1   1   1   1   1   1
 Run Char Index:  0   1   2   3   4   5   6      7  8  9 0  1  2   3   4   5   6   7   8   9   10  11  12
 ```
 
 All done, now you Word document is fully replaced keeping all the format.
 
+## Get document keys - docx_get_keys
+
+You can get all the keys present in the Word document by calling the function `docx_get_keys`:
+
+```python
+keys = docx_get_keys(doc) # Let's suppose the Word document has the keys: ${name} and ${phone}
+print(keys)  # ['name', 'phone']
+```
+
 ## Replace blocks - docx_blocks
 
 You can define a block in your Word document and set if it is going to be removed or not. The format required for key blocks are exactly like tags `HTML`, as following:
 
 - Initial of block: `<signature>`
 - End of the block: `</signature>`
```

### Comparing `python-docx-replace-0.4.3/README.md` & `python-docx-replace-0.4.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,23 @@
 Indexes:         0   1   2   3   4   5   6      7  8  9 10 11 12  13  14  15  16  17  18  19  20  21  22
 Run Index:       0   0   0   0   0   0   0      0  0  0 1  1  1   1   1   1   1   1   1   1   1   1   1
 Run Char Index:  0   1   2   3   4   5   6      7  8  9 0  1  2   3   4   5   6   7   8   9   10  11  12
 ```
 
 All done, now you Word document is fully replaced keeping all the format.
 
+## Get document keys - docx_get_keys
+
+You can get all the keys present in the Word document by calling the function `docx_get_keys`:
+
+```python
+keys = docx_get_keys(doc) # Let's suppose the Word document has the keys: ${name} and ${phone}
+print(keys)  # ['name', 'phone']
+```
+
 ## Replace blocks - docx_blocks
 
 You can define a block in your Word document and set if it is going to be removed or not. The format required for key blocks are exactly like tags `HTML`, as following:
 
 - Initial of block: `<signature>`
 - End of the block: `</signature>`
```

### Comparing `python-docx-replace-0.4.3/src/python_docx_replace/__init__.py` & `python-docx-replace-0.4.4/src/python_docx_replace/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Any
-
+import re
+from typing import Any, List
 from python_docx_replace.exceptions import EndTagNotFound, InitialTagNotFound, TableIndexNotFound
 from python_docx_replace.paragraph import Paragraph
 
 __all__ = ["docx_replace", "docx_blocks", "docx_remove_table"]
 
 
 def docx_replace(doc, **kwargs: str) -> None:
@@ -85,14 +85,32 @@
     try:
         table = doc.tables[index]
         table._element.getparent().remove(table._element)
     except IndexError:
         raise TableIndexNotFound(index, len(doc.tables))
 
 
+def docx_get_keys(doc: Any) -> List[str]:
+    """
+    Search for all keys in the Word document and return a list of unique elements
+
+    ATTENTION: The required format for the keys inside the Word document is: ${key}
+
+    For a document with the following content: "Hello ${name}, is your phone ${phone}?"
+    Result example: ["name", "phone"]
+    """
+    result = set()  # unique items
+    for p in Paragraph.get_all(doc):
+        paragraph = Paragraph(p)
+        matches = re.finditer(r"\$\{([^{}]+)\}", paragraph.get_text())
+        for match in matches:
+            result.add(match.groups()[0])
+    return list(result)
+
+
 def _handle_blocks(doc: Any, initial: str, end: str, keep_block: bool) -> bool:
     # The below process is a little bit complex, so I decided to comment each step
     look_for_initial = True
     for p in Paragraph.get_all(doc):
         paragraph = Paragraph(p)
         if look_for_initial:
             if paragraph.contains(initial):
```

### Comparing `python-docx-replace-0.4.3/src/python_docx_replace/block_handler.py` & `python-docx-replace-0.4.4/src/python_docx_replace/block_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             run_index = self.runs_indexes[index]
             run = self.p.runs[run_index]
             run_char_index = self.run_char_indexes[index]
 
             if not runs_to_change.get(run_index):
                 runs_to_change[run_index] = [char for char_index, char in enumerate(run.text)]
 
-            run_to_change: Dict = runs_to_change.get(run_index)
+            run_to_change: Dict = runs_to_change.get(run_index)  # type: ignore[assignment]
             if (
                 (not keep_block)
                 or (index in range(initial_index, initial_index_plus_key_length))
                 or (index in range(end_index, end_index_plus_key_length))
             ):
                 run_to_change[run_char_index] = ""
 
@@ -57,15 +57,15 @@
             run_index = self.runs_indexes[index]
             run = self.p.runs[run_index]
             run_char_index = self.run_char_indexes[index]
 
             if not runs_to_change.get(run_index):
                 runs_to_change[run_index] = [char for char_index, char in enumerate(run.text)]
 
-            run_to_change: Dict = runs_to_change.get(run_index)
+            run_to_change: Dict = runs_to_change.get(run_index)  # type: ignore[assignment]
             if (not keep_block) or (index in range(key_index, key_index_plus_key_length)):
                 run_to_change[run_char_index] = ""
 
         self._real_replace(runs_to_change)
 
     def clear_key_and_before(self, key: str, keep_block: bool) -> None:
         key_index = self.run_text.find(key)
@@ -77,15 +77,15 @@
             run_index = self.runs_indexes[index]
             run = self.p.runs[run_index]
             run_char_index = self.run_char_indexes[index]
 
             if not runs_to_change.get(run_index):
                 runs_to_change[run_index] = [char for char_index, char in enumerate(run.text)]
 
-            run_to_change: Dict = runs_to_change.get(run_index)
+            run_to_change: Dict = runs_to_change.get(run_index)  # type: ignore[assignment]
             if (not keep_block) or (index in range(key_index, key_index_plus_key_length)):
                 run_to_change[run_char_index] = ""
 
         self._real_replace(runs_to_change)
 
     def _real_replace(self, runs_to_change: dict):
         # make the real replace
```

### Comparing `python-docx-replace-0.4.3/src/python_docx_replace/exceptions.py` & `python-docx-replace-0.4.4/src/python_docx_replace/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-docx-replace-0.4.3/src/python_docx_replace/key_changer.py` & `python-docx-replace-0.4.4/src/python_docx_replace/key_changer.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             run_index = self.runs_indexes[index]
             run = self.p.runs[run_index]
             run_char_index = self.run_char_indexes[index]
 
             if not self.runs_to_change.get(run_index):
                 self.runs_to_change[run_index] = [char for char_index, char in enumerate(run.text)]
 
-            run_to_change: Dict = self.runs_to_change.get(run_index)
+            run_to_change: Dict = self.runs_to_change.get(run_index)  # type: ignore[assignment]
             if index == index_to_replace:
                 run_to_change[run_char_index] = self.value
             else:
                 run_to_change[run_char_index] = ""
 
         # make the real replace
         for index, text in self.runs_to_change.items():
```

### Comparing `python-docx-replace-0.4.3/src/python_docx_replace/paragraph.py` & `python-docx-replace-0.4.4/src/python_docx_replace/paragraph.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,14 +58,17 @@
         block_handler = BlockHandler(self.p)
         block_handler.clear_key_and_before(key, keep_block)
 
     def clear_tag_and_after(self, key, keep_block) -> None:
         block_handler = BlockHandler(self.p)
         block_handler.clear_key_and_after(key, keep_block)
 
+    def get_text(self) -> str:
+        return self.p.text
+
     def _simple_replace_key(self, key, value) -> None:
         # try to replace a key in the paragraph runs, simpler alternative
         for run in self.p.runs:
             if key in run.text:
                 run.text = run.text.replace(key, value)
 
     def _complex_replace_key(self, key, value) -> None:
```

### Comparing `python-docx-replace-0.4.3/src/python_docx_replace.egg-info/PKG-INFO` & `python-docx-replace-0.4.4/src/python_docx_replace.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docx-replace
-Version: 0.4.3
+Version: 0.4.4
 Summary: Replace words and remove blocks inside a Word document without losing format
 Home-page: https://github.com/ivanbicalho/python-docx-replace
 Author: Ivan Bicalho
 Author-email: ivanribeirob@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -120,14 +120,23 @@
 Indexes:         0   1   2   3   4   5   6      7  8  9 10 11 12  13  14  15  16  17  18  19  20  21  22
 Run Index:       0   0   0   0   0   0   0      0  0  0 1  1  1   1   1   1   1   1   1   1   1   1   1
 Run Char Index:  0   1   2   3   4   5   6      7  8  9 0  1  2   3   4   5   6   7   8   9   10  11  12
 ```
 
 All done, now you Word document is fully replaced keeping all the format.
 
+## Get document keys - docx_get_keys
+
+You can get all the keys present in the Word document by calling the function `docx_get_keys`:
+
+```python
+keys = docx_get_keys(doc) # Let's suppose the Word document has the keys: ${name} and ${phone}
+print(keys)  # ['name', 'phone']
+```
+
 ## Replace blocks - docx_blocks
 
 You can define a block in your Word document and set if it is going to be removed or not. The format required for key blocks are exactly like tags `HTML`, as following:
 
 - Initial of block: `<signature>`
 - End of the block: `</signature>`
```

