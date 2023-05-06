# Comparing `tmp/flet_multi_page-1.2.1.tar.gz` & `tmp/flet_multi_page-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_multi_page-1.2.1.tar", last modified: Thu Apr 27 12:43:54 2023, max compression
+gzip compressed data, was "flet_multi_page-1.3.tar", last modified: Sat May  6 17:22:57 2023, max compression
```

## Comparing `flet_multi_page-1.2.1.tar` & `flet_multi_page-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-27 12:43:54.655085 flet_multi_page-1.2.1/
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-04-27 11:33:21.000000 flet_multi_page-1.2.1/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       24 2023-04-27 12:40:13.000000 flet_multi_page-1.2.1/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      605 2023-04-27 12:43:54.654959 flet_multi_page-1.2.1/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1970 2023-04-27 11:57:31.000000 flet_multi_page-1.2.1/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-27 12:43:54.654036 flet_multi_page-1.2.1/flet_multi_page/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       31 2023-04-27 10:57:12.000000 flet_multi_page-1.2.1/flet_multi_page/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1172 2023-04-27 11:52:33.000000 flet_multi_page-1.2.1/flet_multi_page/sub_page.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-27 12:43:54.654741 flet_multi_page-1.2.1/flet_multi_page.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      605 2023-04-27 12:43:54.000000 flet_multi_page-1.2.1/flet_multi_page.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      303 2023-04-27 12:43:54.000000 flet_multi_page-1.2.1/flet_multi_page.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-27 12:43:54.000000 flet_multi_page-1.2.1/flet_multi_page.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        5 2023-04-27 12:43:54.000000 flet_multi_page-1.2.1/flet_multi_page.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-27 12:43:54.000000 flet_multi_page-1.2.1/flet_multi_page.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-04-27 11:33:21.000000 flet_multi_page-1.2.1/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-27 12:43:54.655134 flet_multi_page-1.2.1/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      750 2023-04-27 12:41:05.000000 flet_multi_page-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:22:57.411017 flet_multi_page-1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-06 17:22:43.000000 flet_multi_page-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-06 17:22:43.000000 flet_multi_page-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-06 17:22:57.411017 flet_multi_page-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-06 17:22:43.000000 flet_multi_page-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:22:57.407017 flet_multi_page-1.3/flet_multi_page.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-06 17:22:57.000000 flet_multi_page-1.3/flet_multi_page.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-06 17:22:57.000000 flet_multi_page-1.3/flet_multi_page.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 17:22:57.000000 flet_multi_page-1.3/flet_multi_page.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 17:22:57.000000 flet_multi_page-1.3/flet_multi_page.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 17:22:57.000000 flet_multi_page-1.3/flet_multi_page.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:22:57.407017 flet_multi_page-1.3/flet_sub_page/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-06 17:22:43.000000 flet_multi_page-1.3/flet_sub_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-06 17:22:43.000000 flet_multi_page-1.3/flet_sub_page/sub_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 17:22:43.000000 flet_multi_page-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 17:22:57.411017 flet_multi_page-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-06 17:22:43.000000 flet_multi_page-1.3/setup.py
```

### Comparing `flet_multi_page-1.2.1/LICENSE` & `flet_multi_page-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_multi_page-1.2.1/PKG-INFO` & `flet_multi_page-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_multi_page
-Version: 1.2.1
+Version: 1.3
 Summary: A tool of creating new pages with flet library.
 Home-page: https://github.com/SKbarbon/flet_multi_page
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
```

### Comparing `flet_multi_page-1.2.1/README.md` & `flet_multi_page-1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # flet_multi_page
-until now, flet v0.6 does not support multi pages.
-With this tool, you can start new pages on the same script without the need of creating new `app` class.
+until now, flet does not support multi pages.
+With this tool, you can start new pages on the same script without the need of creating new `app` class or new cmd process etc...
 
 
 ## install
 
 ```
-pip install flet-multi-page==1.0
+pip install flet-multi-page --upgrade
 ```
 
+## little peek
+
+![Screen Recording 2023-04-27 at 3 22 44 PM](https://user-images.githubusercontent.com/86029286/234861120-f2dcc22d-169c-4161-8e40-a20455250f99.GIF)
+
 ## usage
 Its very simple, you just need to import the package and import the class `subPage`.
 This is an example code:
 
 ```python
-from flet_sub_page import subPage
+from flet_multi_page import subPage
 import flet
 
 def main (page:flet.Page):
     def start_new_page (e):
         p = subPage(controls=[flet.Text("Hello from the new page!!")], page_props={"bgcolor":"blue"})
         p.start()
     
@@ -29,15 +33,15 @@
 if __name__ == "__main__": #? This is so important, there will be errors without it.
     flet.app(target=main)
 ```
 
 Or if you want a second `target` function for the page you can just add `target` argument like this:
 
 ```python
-from flet_sub_page import subPage
+from flet_multi_page import subPage
 import flet
 import random
 
 def second_target (page:flet.Page): #? This is the target function of the second page.
     colors = ["blue", "pink", "black", "red", "green"]
     page.bgcolor = random.choice(colors)
     page.add(flet.Text("Hello new page!", color="white"))
@@ -55,8 +59,9 @@
 if __name__ == "__main__": #? This is so important, there will be errors without it.
     flet.app(target=main)
 ```
 
 ## `subPage` properties
 - `controls` argument (optional): You can add the controls you need directly to the new page.
 - `page_props` argument (optional): You can add the page properties you want as dict.
-- `target` argument (optional): You can set a target function to call for the new page, and get `page` class as an argument.
+- `target` argument (optional): You can set a target function to call for the new page, and get `page` class as an argument.
+- `view` argument (optional): The default is `FLET_APP` which is a desktop app view, you can change it to `flet.WEB_BROWSER` or `web_browser` to make the page open in a web_browser.
```

### Comparing `flet_multi_page-1.2.1/flet_multi_page/sub_page.py` & `flet_multi_page-1.3/flet_sub_page/sub_page.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,22 +20,23 @@
                     setattr(page, P, sub_page_class.page_props[P])
                     page.update()
         page.update()
         if sub_page_class.target != None:
             sub_page_class.target (page)
         page.update()
     
-    flet.app(target=APP)
+    flet.app(target=APP, view=sub_page_class.view)
 
 
 
 class subPage (object):
-    def __init__ (self, controls=None, page_props=None, target=None):
+    def __init__ (self, controls=None, page_props=None, target=None, view=flet.FLET_APP):
         self.controls = controls
         self.page_props = page_props
         self.target = target
+        self.view = view
     
     def start (self):
         with concurrent.futures.ProcessPoolExecutor() as executor:
             # future = executor.submit(push_new_app)
             # future.result()
             multiprocessing.Process(target=_s_, args=[self]).start()
```

### Comparing `flet_multi_page-1.2.1/flet_multi_page.egg-info/PKG-INFO` & `flet_multi_page-1.3/flet_multi_page.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-multi-page
-Version: 1.2.1
+Version: 1.3
 Summary: A tool of creating new pages with flet library.
 Home-page: https://github.com/SKbarbon/flet_multi_page
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
```

### Comparing `flet_multi_page-1.2.1/setup.py` & `flet_multi_page-1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='flet_multi_page',
-    version='1.2.1',
+    version='1.3',
     author='SKbarbon',
     description='A tool of creating new pages with flet library.',
     long_description="until now, flet v0.6 does not support multi pages.\n With this tool, you can start new pages on the same script without the need of creating new `app` class.\n visit the github repo for more: [github](https://github.com/SKbarbon/flet_multi_page)",
     url='https://github.com/SKbarbon/flet_multi_page',
     install_requires=["flet"],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"
     ],
-)
+)
```

