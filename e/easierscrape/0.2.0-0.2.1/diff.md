# Comparing `tmp/easierscrape-0.2.0.tar.gz` & `tmp/easierscrape-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierscrape-0.2.0.tar", last modified: Wed May  3 22:06:34 2023, max compression
+gzip compressed data, was "easierscrape-0.2.1.tar", last modified: Sat May  6 16:34:50 2023, max compression
```

## Comparing `easierscrape-0.2.0.tar` & `easierscrape-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.095369 easierscrape-0.2.0/
--rw-rw-rw-   0        0        0      550 2023-05-03 21:59:41.000000 easierscrape-0.2.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0      289 2023-04-04 16:46:22.000000 easierscrape-0.2.0/.readthedocs.yml
--rw-rw-rw-   0        0        0     1105 2023-04-04 01:00:40.000000 easierscrape-0.2.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-04-04 01:00:40.000000 easierscrape-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      610 2023-04-04 17:02:03.000000 easierscrape-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2745 2023-04-11 20:59:45.000000 easierscrape-0.2.0/Makefile
--rw-rw-rw-   0        0        0    18403 2023-05-03 22:06:34.094078 easierscrape-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4371 2023-05-03 21:17:56.000000 easierscrape-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.061998 easierscrape-0.2.0/docs/
--rw-rw-rw-   0        0        0      654 2023-04-04 17:30:23.000000 easierscrape-0.2.0/docs/Makefile
--rw-rw-rw-   0        0        0     1098 2023-05-03 21:59:41.000000 easierscrape-0.2.0/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.066963 easierscrape-0.2.0/docs/images/
--rw-rw-rw-   0        0        0   248542 2023-04-05 17:40:22.000000 easierscrape-0.2.0/docs/images/cli_recording.gif
--rw-rw-rw-   0        0        0   108334 2023-05-03 21:17:56.000000 easierscrape-0.2.0/docs/images/demo_recording.gif
--rw-rw-rw-   0        0        0     2377 2023-05-03 21:17:56.000000 easierscrape-0.2.0/docs/index.md
--rwxrwxrwx   0        0        0      800 2023-04-04 17:30:23.000000 easierscrape-0.2.0/docs/make.bat
--rw-rw-rw-   0        0        0      109 2023-05-03 21:59:41.000000 easierscrape-0.2.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.071333 easierscrape-0.2.0/docs/source/
--rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.2.0/docs/source/easierscrape.rst
--rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.2.0/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.079802 easierscrape-0.2.0/easierscrape/
--rw-rw-rw-   0        0        0       64 2023-04-04 01:00:40.000000 easierscrape-0.2.0/easierscrape/__init__.py
--rw-rw-rw-   0        0        0      699 2023-05-03 21:17:56.000000 easierscrape-0.2.0/easierscrape/__main__.py
--rw-rw-rw-   0        0        0       23 2023-05-03 21:59:41.000000 easierscrape-0.2.0/easierscrape/_version.py
--rw-rw-rw-   0        0        0     9469 2023-05-03 21:31:47.000000 easierscrape-0.2.0/easierscrape/easierscrape.py
-drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.091756 easierscrape-0.2.0/easierscrape/tests/
--rw-rw-rw-   0        0        0    11498 2023-05-03 21:17:56.000000 easierscrape-0.2.0/easierscrape/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-05-03 22:06:34.090603 easierscrape-0.2.0/easierscrape.egg-info/
--rw-rw-rw-   0        0        0    18403 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      246 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 22:06:33.000000 easierscrape-0.2.0/easierscrape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2434 2023-05-03 21:59:41.000000 easierscrape-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 22:06:34.095369 easierscrape-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-04-04 01:00:40.000000 easierscrape-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.477454 easierscrape-0.2.1/
+-rw-rw-rw-   0        0        0      550 2023-05-06 16:30:28.000000 easierscrape-0.2.1/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      289 2023-04-04 16:46:22.000000 easierscrape-0.2.1/.readthedocs.yml
+-rw-rw-rw-   0        0        0     1105 2023-04-04 01:00:40.000000 easierscrape-0.2.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-04-04 01:00:40.000000 easierscrape-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      610 2023-04-04 17:02:03.000000 easierscrape-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2745 2023-04-11 20:59:45.000000 easierscrape-0.2.1/Makefile
+-rw-rw-rw-   0        0        0    18493 2023-05-06 16:34:50.474191 easierscrape-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4461 2023-05-05 19:55:40.000000 easierscrape-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.380834 easierscrape-0.2.1/docs/
+-rw-rw-rw-   0        0        0      654 2023-04-04 17:30:23.000000 easierscrape-0.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0     1098 2023-05-06 16:30:28.000000 easierscrape-0.2.1/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.390833 easierscrape-0.2.1/docs/images/
+-rw-rw-rw-   0        0        0   242191 2023-05-06 16:10:24.000000 easierscrape-0.2.1/docs/images/cli_recording.gif
+-rw-rw-rw-   0        0        0    92263 2023-05-06 16:10:24.000000 easierscrape-0.2.1/docs/images/demo_recording.gif
+-rw-rw-rw-   0        0        0     2607 2023-05-06 16:10:24.000000 easierscrape-0.2.1/docs/index.md
+-rwxrwxrwx   0        0        0      800 2023-04-04 17:30:23.000000 easierscrape-0.2.1/docs/make.bat
+-rw-rw-rw-   0        0        0      109 2023-05-06 16:30:28.000000 easierscrape-0.2.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.398790 easierscrape-0.2.1/docs/source/
+-rw-rw-rw-   0        0        0      195 2023-04-11 22:02:58.000000 easierscrape-0.2.1/docs/source/easierscrape.rst
+-rw-rw-rw-   0        0        0       80 2023-04-04 17:22:56.000000 easierscrape-0.2.1/docs/source/modules.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.436680 easierscrape-0.2.1/easierscrape/
+-rw-rw-rw-   0        0        0       64 2023-04-04 01:00:40.000000 easierscrape-0.2.1/easierscrape/__init__.py
+-rw-rw-rw-   0        0        0      803 2023-05-06 16:10:24.000000 easierscrape-0.2.1/easierscrape/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-05-06 16:30:28.000000 easierscrape-0.2.1/easierscrape/_version.py
+-rw-rw-rw-   0        0        0    10744 2023-05-06 16:10:24.000000 easierscrape-0.2.1/easierscrape/easierscrape.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.467815 easierscrape-0.2.1/easierscrape/tests/
+-rw-rw-rw-   0        0        0    27216 2023-05-06 16:10:24.000000 easierscrape-0.2.1/easierscrape/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:34:50.457207 easierscrape-0.2.1/easierscrape.egg-info/
+-rw-rw-rw-   0        0        0    18493 2023-05-06 16:34:49.000000 easierscrape-0.2.1/easierscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-06 16:34:50.000000 easierscrape-0.2.1/easierscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 16:34:49.000000 easierscrape-0.2.1/easierscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      246 2023-05-06 16:34:49.000000 easierscrape-0.2.1/easierscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 16:34:49.000000 easierscrape-0.2.1/easierscrape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2434 2023-05-06 16:30:29.000000 easierscrape-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 16:34:50.477454 easierscrape-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-04-04 01:00:40.000000 easierscrape-0.2.1/setup.py
```

### Comparing `easierscrape-0.2.0/.bumpversion.cfg` & `easierscrape-0.2.1/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 commit = True
 tag = True
 
 [bumpversion:file:easierscrape/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `easierscrape-0.2.0/CONTRIBUTING.md` & `easierscrape-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.0/LICENSE` & `easierscrape-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.0/MANIFEST.in` & `easierscrape-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.0/Makefile` & `easierscrape-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.0/PKG-INFO` & `easierscrape-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierscrape
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library which does some basic web scraping operations
 Author-email: Daniel Greco <dag2226@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -275,26 +275,27 @@
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
 When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, get a screenshot, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
-usage: python -m easierscrape [-h] url depth
+usage: python -m easierscrape [-h] url depth download_path
 
 positional arguments:
-  url         the url to scrape
-  depth       the depth of the scrape tree
+  url            the url to scrape
+  depth          the depth of the scrape tree
+  download_path  the location to download files to
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 Usage example:
 ```
->>> python -m  easierscrape https://toscrape.com/ 1
+>>> python -m  easierscrape https://toscrape.com/ 1 example_down_path
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
```

### Comparing `easierscrape-0.2.0/README.md` & `easierscrape-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,26 +53,27 @@
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
 When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, get a screenshot, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
-usage: python -m easierscrape [-h] url depth
+usage: python -m easierscrape [-h] url depth download_path
 
 positional arguments:
-  url         the url to scrape
-  depth       the depth of the scrape tree
+  url            the url to scrape
+  depth          the depth of the scrape tree
+  download_path  the location to download files to
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 Usage example:
 ```
->>> python -m  easierscrape https://toscrape.com/ 1
+>>> python -m  easierscrape https://toscrape.com/ 1 example_down_path
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
```

### Comparing `easierscrape-0.2.0/docs/Makefile` & `easierscrape-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.0/docs/conf.py` & `easierscrape-0.2.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -- Path setup --------------------------------------------------------------
 sys.path.insert(0, os.path.abspath('../'))
 
 # -- Project information -----------------------------------------------------
 project = 'easierscrape'
 copyright = '2023, Daniel Greco'
 author = 'Daniel Greco'
-release = '0.2.0'
+release = '0.2.1'
 
 master_doc = 'index'
 
 # -- General configuration ---------------------------------------------------
 extensions = ['recommonmark', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages', 'sphinx.ext.napoleon']
 source_suffix = ['.rst', '.md']
```

### Comparing `easierscrape-0.2.0/docs/index.md` & `easierscrape-0.2.1/docs/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Welcome to easierscrape's documentation!
 
 ## Basic Usage
 Install with pip: `pip install easierscrape`
 
-Import `Scraper` from `easierscrape` and instantiate it with a url as seen below:
+Import `Scraper` from `easierscrape` and instantiate it with a url (and optionally a download_path) as seen below:
 ```python
 from easierscrape import Scraper
 
-scraper = Scraper("https://quotes.toscrape.com/login")
+scraper = Scraper("https://quotes.toscrape.com/login", "download_dir")
 ```
 From there, call class methods to scrape varying resources.
 
 Usage examples:
 ```
 >>> scraper.parse_text()
 ["Quotes to Scrape", "Quotes to Scrape", "Login", "Username", "Password", "Quotes by:", "GoodReads.com", "Made with", "❤", "by", "Scrapinghub",]
@@ -26,46 +26,47 @@
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ### Downloads
-Using `get_screenshot`, `parse_files`, `parse_images`, or `parse_tables` will result in an "easierscrape_downloads" directory being created in the working directory.
+Using `get_screenshot`, `parse_files`, `parse_images`, or `parse_tables` will result in downloads to the `download_path` specified in the `Scraper` instantiation. If no path is specified, it will default to downloading to an "easierscrape_downloads" folder.
 
 Usage example:
 ```eval_rst
 .. image:: images/demo_recording.gif
 ```
 
 ## Command Line Usage
 When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, get a screenshot, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
-usage: python -m easierscrape [-h] url depth
+usage: python -m easierscrape [-h] url depth download_path
 
 positional arguments:
-  url         the url to scrape
-  depth       the depth of the scrape tree
+  url            the url to scrape
+  depth          the depth of the scrape tree
+  download_path  the location to download files to
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 Usage example:
 ```
->>> python -m  easierscrape https://toscrape.com/ 1
+>>> python -m  easierscrape https://toscrape.com/ 1 example_down_path
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
 ├── http://quotes.toscrape.com/login
 ├── http://quotes.toscrape.com/search.aspx
-└── http://quotes.toscrape.com/random"
+└── http://quotes.toscrape.com/random
 ```
 ```eval_rst
 .. image:: images/cli_recording.gif
 ```
 
 
 ```eval_rst
```

### Comparing `easierscrape-0.2.0/docs/make.bat` & `easierscrape-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.0/easierscrape/easierscrape.py` & `easierscrape-0.2.1/easierscrape/easierscrape.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 from os import getcwd, makedirs
 from os.path import basename, exists, join
 from pandas import read_html, ExcelWriter
 from re import compile
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
+from shutil import rmtree
 from urllib.parse import urlparse
 from urllib.request import urlopen, url2pathname
 from uuid import uuid4
 
 
 class Scraper:
-    """Class for a scraper that targets `url`. A `Scraper` object acts as a "one-stop-shop" for
-    all scraping functions.
+    """Class for a scraper that targets a specific url and downloads all files to a download_path
+    relative to the current working directory. A `Scraper` object acts as a "one-stop-shop" for all
+    scraping functions.
     """
 
-    def __init__(self, url):
+    def __init__(self, url, download_path="easierscrape_downloads"):
         """
         Args:
             url (str): The url to scrape from.
+            download_path (str): The location to download parsed files to (defaults to
+                                 "easierscrape_downloads").
 
         """
         self.url = url
+        self.download_path = join(getcwd(), download_path)
 
         # hide GUI
         options = Options()
         options.add_argument("--headless")
         options.add_argument("--window-size=1920,1080")
         options.add_argument("start-maximized")
         options.add_experimental_option("excludeSwitches", ["enable-logging"])
@@ -51,41 +56,54 @@
         if not child_url.startswith("http"):
             child_url = base_url + "/" + child_url
         if child_url.endswith("/"):
             child_url = child_url[:-1]
         return child_url
 
     def _get_download_dir(self, type):
-        dir = join(getcwd(), "easierscrape_downloads", type, url2pathname(self.url)[3:])
+        dir = join(self.download_path, type, url2pathname(self.url)[3:])
         if not exists(dir):
             makedirs(dir)
         return dir
 
-    def _tree_gen_rec(self, url, maxdepth, tree, depth):
+    def _tree_gen_rec(self, url, maxdepth, tree, depth, blacklist, whitelist):
         if tree is None:
             url = url.replace("www.", "")
             if url.endswith("/"):
                 url = url[:-1]
             tree = Node(url, url=url)
         if depth < maxdepth:
             parent_node = tree
             self.driver.get(url)
             for a in BeautifulSoup(self.driver.page_source, "html.parser").find_all("a"):
                 try:
                     child_url = self._concat_urls(url, a.attrs["href"].replace("www.", ""))
-                    if find(tree.root, lambda node: node.url == child_url) is None:
-                        new_leaf = Node(child_url, url=child_url, parent=parent_node)
-                        tree = self._tree_gen_rec(child_url, maxdepth, new_leaf, depth + 1)
+                    domain = urlparse(child_url).netloc
+                    if (domain not in blacklist) and (len(whitelist) == 0 or domain in whitelist):
+                        if find(tree.root, lambda node: node.url == child_url) is None:
+                            new_leaf = Node(child_url, url=child_url, parent=parent_node)
+                            tree = self._tree_gen_rec(child_url, maxdepth, new_leaf, depth + 1, blacklist, whitelist)
                 except Exception:
                     pass
         return tree.root
 
+    def clear_downloads(self):
+        """Deletes the Scraper download directory.
+
+        Returns:
+            bool: True if the Scraper download directory exists and is deleted. False otherwise.
+
+        """
+        if exists(self.download_path):
+            rmtree(self.download_path)
+            return True
+        return False
+
     def get_screenshot(self):
-        """Downloads screenshot from the Scraper url to an "easierscrape_downloads" folder in the
-        current working directory.
+        """Downloads screenshot from the Scraper url to the Scraper download directory.
 
         Returns:
             bool: True
 
         """
         download_file = join(self._get_download_dir("images"), "easierscrape_screenshot.png")
 
@@ -99,16 +117,15 @@
         Returns:
             List[str]: List of anchor tags in the url.
 
         """
         return self.soup_url.find_all("a")
 
     def parse_files(self, filetypes=[]):
-        """Downloads provided filetypes from the Scraper url to an "easierscrape_downloads" folder
-        in the current working directory.
+        """Downloads provided filetypes from the Scraper url to the Scraper download directory.
 
         Args:
             filetypes (List[str]): List of filetypes ("pdf", "txt", etc.) to scrape.
 
         Returns:
             List[int]: List of number of files downloaded per filetype from url (so if
             filetypes=["pdf", "txt"] and the return value is [1, 30] this means that 1
@@ -119,28 +136,27 @@
             print("No filetype specified")
             return
         file_download_list = []
         for filetype in filetypes:
             file_download_count = 0
             for file in self.soup_url.find_all("a", href=compile(r"(." + filetype + ")")):
                 try:
-                    fileUrl = self._concat_urls(self.url, file.attrs["href"])
-                    response = urlopen(fileUrl)
-                    with open(join(self._get_download_dir(filetype), basename(fileUrl)), "wb") as file:
-                        file.write(response.read())
-                    file.close()
-                    file_download_count += 1
+                    response = urlopen(self._concat_urls(self.url, file.attrs["href"]))
+                    if not exists(join(self._get_download_dir(filetype), basename(response.url))):
+                        with open(join(self._get_download_dir(filetype), basename(response.url)), "wb") as file:
+                            file.write(response.read())
+                        file.close()
+                        file_download_count += 1
                 except Exception:
                     pass
             file_download_list.append(file_download_count)
         return file_download_list
 
     def parse_images(self):
-        """Downloads all images from the Scraper url to an "easierscrape_downloads" folder in the
-        current working directory.
+        """Downloads all images from the Scraper url to the Scraper download directory.
 
         Returns:
             int: Number of images downloaded from url.
 
         """
         image_download_count = 0
         for image in self.soup_url.findAll("img"):
@@ -167,16 +183,15 @@
         for list in self.soup_url.findAll(["ul", "ol"]):
             out.append([item for item in list.stripped_strings])
             if out[-1] == []:
                 out.pop()
         return out
 
     def parse_tables(self, output_type="csv"):
-        """Downloads all tables from the Scraper url to an "easierscrape_downloads" folder in the
-        current working directory.
+        """Downloads all tables from the Scraper url to the Scraper download directory.
 
         Supported output types are csv and xlsx (defaults to csv).
 
         - If downloaded as a csv file, each table will be stored in a separate csv.
         - If downloaded as an xlsx file, all tables will be stored as separate sheets in a
           "tables.xlsx" file.
 
@@ -220,30 +235,34 @@
 
         Returns:
             List[str]: List of text fragments in the url.
 
         """
         return [text for text in self.soup_url.stripped_strings]
 
-    def tree_gen(self, maxdepth):
-        """Generates a tree of depth=maxdepth starting at the Scraper url.
+    def tree_gen(self, maxdepth, blacklist=[], whitelist=[]):
+        """Generates a tree of depth=maxdepth starting at the Scraper url. If the blacklist argument
+        is used, none of the blacklisted domains will appear. If the whitelist argument is used, only
+        the whitelisted domains will appear.
 
         Args:
             maxdepth (int): The depth you want to generate the tree to.
+            blacklist (List[str]): A list of all domains to ignore in the tree generation
+            whitelist (List[str]): A list of only domains to include in the tree generation
 
         Returns:
             Node: Head node of an anytree hyperlink tree.
 
         """
-        return self._tree_gen_rec(self.url, maxdepth, None, 0)
+        return self._tree_gen_rec(self.url, maxdepth, None, 0, blacklist, whitelist)
 
-    def print_tree(self, maxdepth):
+    def print_tree(self, maxdepth, blacklist=[], whitelist=[]):
         """Prints a tree of depth=maxdepth starting at the Scraper url.
 
         Args:
             maxdepth (int): The depth you want to print the tree to.
 
         """
         tree_print = ""
-        for pre, fill, node in RenderTree(self.tree_gen(maxdepth)):
+        for pre, fill, node in RenderTree(self.tree_gen(maxdepth, blacklist, whitelist)):
             tree_print += "%s%s\n" % (pre, node.name)
         print(tree_print[:-1])
```

### Comparing `easierscrape-0.2.0/easierscrape.egg-info/PKG-INFO` & `easierscrape-0.2.1/easierscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierscrape
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library which does some basic web scraping operations
 Author-email: Daniel Greco <dag2226@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -275,26 +275,27 @@
 ├── http://quotes.toscrape.com/search.aspx
 └── http://quotes.toscrape.com/random
 ```
 
 ## Command Line Usage
 When installed, you can invoke easierscrape from the command-line to generate a hyperlink tree, get a screenshot, download all image, txt, and pdf files, and scrape any tables for a given url and depth:
 ```
-usage: python -m easierscrape [-h] url depth
+usage: python -m easierscrape [-h] url depth download_path
 
 positional arguments:
-  url         the url to scrape
-  depth       the depth of the scrape tree
+  url            the url to scrape
+  depth          the depth of the scrape tree
+  download_path  the location to download files to
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 Usage example:
 ```
->>> python -m  easierscrape https://toscrape.com/ 1
+>>> python -m  easierscrape https://toscrape.com/ 1 example_down_path
 https://toscrape.com
 ├── http://books.toscrape.com
 ├── http://quotes.toscrape.com
 ├── http://quotes.toscrape.com/scroll
 ├── http://quotes.toscrape.com/js
 ├── http://quotes.toscrape.com/js-delayed
 ├── http://quotes.toscrape.com/tableful
```

### Comparing `easierscrape-0.2.0/easierscrape.egg-info/SOURCES.txt` & `easierscrape-0.2.1/easierscrape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easierscrape-0.2.0/pyproject.toml` & `easierscrape-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "easierscrape"
 authors = [{name = "Daniel Greco", email = "dag2226@columbia.edu"}]
 description="A library which does some basic web scraping operations"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.7"
 
 dependencies = [
     "anytree",
     "beautifulsoup4",
     "lxml",
     "openpyxl",
```

