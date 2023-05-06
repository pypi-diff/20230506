# Comparing `tmp/parsel_get_selector_text-0.2.tar.gz` & `tmp/parsel_get_selector_text-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsel_get_selector_text-0.2.tar", last modified: Mon Apr 24 01:20:48 2023, max compression
+gzip compressed data, was "parsel_get_selector_text-0.3.tar", last modified: Sat May  6 20:08:27 2023, max compression
```

## Comparing `parsel_get_selector_text-0.2.tar` & `parsel_get_selector_text-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:20:48.556095 parsel_get_selector_text-0.2/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1089 2023-04-23 23:41:13.000000 parsel_get_selector_text-0.2/LICENSE
--rw-r--r--   0 andrei    (1000) andrei    (1000)      783 2023-04-24 01:20:48.556095 parsel_get_selector_text-0.2/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-23 22:53:37.000000 parsel_get_selector_text-0.2/README.md
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:20:48.549429 parsel_get_selector_text-0.2/parsel_get_selector_text/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2225 2023-04-24 01:19:56.000000 parsel_get_selector_text-0.2/parsel_get_selector_text/__init__.py
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:20:48.556095 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/
--rw-r--r--   0 andrei    (1000) andrei    (1000)      783 2023-04-24 01:20:48.000000 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)      270 2023-04-24 01:20:48.000000 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/SOURCES.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2023-04-24 01:20:48.000000 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/dependency_links.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       25 2023-04-24 01:20:48.000000 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/top_level.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-24 01:01:58.000000 parsel_get_selector_text-0.2/pyproject.toml
--rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2023-04-24 01:20:48.556095 parsel_get_selector_text-0.2/setup.cfg
--rw-r--r--   0 andrei    (1000) andrei    (1000)      957 2023-04-24 01:19:33.000000 parsel_get_selector_text-0.2/setup.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-06 20:08:27.049947 parsel_get_selector_text-0.3/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1089 2023-04-23 23:41:13.000000 parsel_get_selector_text-0.3/LICENSE
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      700 2023-05-06 20:08:27.049947 parsel_get_selector_text-0.3/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-23 22:53:37.000000 parsel_get_selector_text-0.3/README.md
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-06 20:08:27.046614 parsel_get_selector_text-0.3/parsel_get_selector_text/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2445 2023-05-06 20:05:07.000000 parsel_get_selector_text-0.3/parsel_get_selector_text/__init__.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-05-06 20:08:27.049947 parsel_get_selector_text-0.3/parsel_get_selector_text.egg-info/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      700 2023-05-06 20:08:27.000000 parsel_get_selector_text-0.3/parsel_get_selector_text.egg-info/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      270 2023-05-06 20:08:27.000000 parsel_get_selector_text-0.3/parsel_get_selector_text.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2023-05-06 20:08:27.000000 parsel_get_selector_text-0.3/parsel_get_selector_text.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       25 2023-05-06 20:08:27.000000 parsel_get_selector_text-0.3/parsel_get_selector_text.egg-info/top_level.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-24 01:01:58.000000 parsel_get_selector_text-0.3/pyproject.toml
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2023-05-06 20:08:27.049947 parsel_get_selector_text-0.3/setup.cfg
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      863 2023-05-06 20:06:46.000000 parsel_get_selector_text-0.3/setup.py
```

### Comparing `parsel_get_selector_text-0.2/LICENSE` & `parsel_get_selector_text-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parsel_get_selector_text-0.2/PKG-INFO` & `parsel_get_selector_text-0.3/parsel_get_selector_text.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: parsel_get_selector_text
-Version: 0.2
+Name: parsel-get-selector-text
+Version: 0.3
 Summary: Extracts all text results from an XPath query on a parsel Selector object.
 Home-page: https://github.com/carlosplanchon/parsel_get_selector_text
-Download-URL: https://github.com/carlosplanchon/parsel_get_selector_text/archive/v0.2.tar.gz
 Author: Carlos A. Planchón
 Author-email: carlosandresplanchonprestes@gmail.com
 License: MIT
-Keywords: comment,remover
+Keywords: dom,parsel,scraping,xpath
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `parsel_get_selector_text-0.2/parsel_get_selector_text/__init__.py` & `parsel_get_selector_text-0.3/parsel_get_selector_text/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,26 +14,30 @@
     text: list[str] = text.split()
     text: list[str] = [word for word in text if word != ""]
     text = " ".join(text)
     return text
 
 
 class ParselGetSelectorInText:
+    def __init__(self, fix_mojibake: bool):
+        self.fix_mojibake = fix_mojibake
+
     def traverse_soup(self, root) -> None:
         """
         Traverses a BeautifulSoup object recursively, extracting all NavigableStrings,
         removing mojibake and extracting their text.
         """
         children_list = list(root.children)
         for child in children_list:
             if isinstance(child, bs4.element.NavigableString):
                 text: str = child.get_text(separator=" ")
                 text = remove_trailing_chars(text=text)
                 if text != "":
-                    text = ftfy.fix_text(text=text)
+                    if self.fix_mojibake is True:
+                        text = ftfy.fix_text(text=text)
                     self.total_text += text + "\n"
             else:
                 self.traverse_soup(root=child)
         return None
 
     def get_sel_results(self, sel_results: parsel.SelectorList) -> None:
         """
@@ -58,19 +62,25 @@
         self.total_text: str = ""
         sel_results = parsel_sel.xpath(xpath)
         self.get_sel_results(sel_results=sel_results)
         self.total_text.rstrip("\n")
         return self.total_text
 
 
-def parsel_sel_get_text(parsel_sel: parsel.Selector, xpath: str) -> str:
+def parsel_sel_get_text(
+    parsel_sel: parsel.Selector,
+    xpath: str,
+    fix_mojibake=True
+        ) -> str:
     """
     Extracts all text results from an XPath
     query on a parsel Selector object.
     """
-    sel_text_obj = ParselGetSelectorInText()
+    sel_text_obj = ParselGetSelectorInText(
+        fix_mojibake=fix_mojibake
+    )
 
     total_text: str = sel_text_obj.get_xpath_results(
         parsel_sel=parsel_sel,
         xpath=xpath
     )
     return total_text
```

### Comparing `parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/PKG-INFO` & `parsel_get_selector_text-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: parsel-get-selector-text
-Version: 0.2
+Name: parsel_get_selector_text
+Version: 0.3
 Summary: Extracts all text results from an XPath query on a parsel Selector object.
 Home-page: https://github.com/carlosplanchon/parsel_get_selector_text
-Download-URL: https://github.com/carlosplanchon/parsel_get_selector_text/archive/v0.2.tar.gz
 Author: Carlos A. Planchón
 Author-email: carlosandresplanchonprestes@gmail.com
 License: MIT
-Keywords: comment,remover
+Keywords: dom,parsel,scraping,xpath
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `parsel_get_selector_text-0.2/setup.py` & `parsel_get_selector_text-0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="parsel_get_selector_text",
     packages=["parsel_get_selector_text"],
-    version="0.2",
+    version="0.3",
     license="MIT",
     description="Extracts all text results from an XPath "\
         "query on a parsel Selector object.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Carlos A. Planchón",
     author_email="carlosandresplanchonprestes@gmail.com",
     url="https://github.com/carlosplanchon/parsel_get_selector_text",
-    download_url="https://github.com/carlosplanchon/"
-        "parsel_get_selector_text/archive/v0.2.tar.gz",
-    keywords=["comment", "remover"],
+    keywords=["dom", "parsel", "scraping", "xpath"],
     classifiers=[
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.11",
     ],
 )
```

