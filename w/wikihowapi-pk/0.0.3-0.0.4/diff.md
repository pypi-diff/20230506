# Comparing `tmp/wikihowapi_pk-0.0.3.tar.gz` & `tmp/wikihowapi_pk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikihowapi_pk-0.0.3.tar", last modified: Wed May  3 16:06:48 2023, max compression
+gzip compressed data, was "wikihowapi_pk-0.0.4.tar", last modified: Sat May  6 13:54:04 2023, max compression
```

## Comparing `wikihowapi_pk-0.0.3.tar` & `wikihowapi_pk-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 16:06:48.126462 wikihowapi_pk-0.0.3/
--rw-r--r--   0 piko       (501) staff       (20)     1101 2023-05-03 09:56:00.000000 wikihowapi_pk-0.0.3/LICENSE
--rw-r--r--   0 piko       (501) staff       (20)     3863 2023-05-03 16:06:48.126331 wikihowapi_pk-0.0.3/PKG-INFO
--rw-r--r--   0 piko       (501) staff       (20)     3345 2023-05-03 15:06:46.000000 wikihowapi_pk-0.0.3/README.md
--rw-r--r--   0 piko       (501) staff       (20)       38 2023-05-03 16:06:48.126506 wikihowapi_pk-0.0.3/setup.cfg
--rw-r--r--   0 piko       (501) staff       (20)      791 2023-05-03 16:05:15.000000 wikihowapi_pk-0.0.3/setup.py
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 16:06:48.125227 wikihowapi_pk-0.0.3/tests/
--rw-r--r--   0 piko       (501) staff       (20)      351 2023-05-03 15:57:50.000000 wikihowapi_pk-0.0.3/tests/test.py
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 16:06:48.125556 wikihowapi_pk-0.0.3/wikihowapi_pk/
--rw-r--r--   0 piko       (501) staff       (20)    26271 2023-05-03 16:05:50.000000 wikihowapi_pk-0.0.3/wikihowapi_pk/__init__.py
--rw-r--r--   0 piko       (501) staff       (20)      194 2023-05-03 09:37:40.000000 wikihowapi_pk-0.0.3/wikihowapi_pk/exceptions.py
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 16:06:48.126178 wikihowapi_pk-0.0.3/wikihowapi_pk.egg-info/
--rw-r--r--   0 piko       (501) staff       (20)     3863 2023-05-03 16:06:48.000000 wikihowapi_pk-0.0.3/wikihowapi_pk.egg-info/PKG-INFO
--rw-r--r--   0 piko       (501) staff       (20)      278 2023-05-03 16:06:48.000000 wikihowapi_pk-0.0.3/wikihowapi_pk.egg-info/SOURCES.txt
--rw-r--r--   0 piko       (501) staff       (20)        1 2023-05-03 16:06:48.000000 wikihowapi_pk-0.0.3/wikihowapi_pk.egg-info/dependency_links.txt
--rw-r--r--   0 piko       (501) staff       (20)        9 2023-05-03 16:06:48.000000 wikihowapi_pk-0.0.3/wikihowapi_pk.egg-info/requires.txt
--rw-r--r--   0 piko       (501) staff       (20)       14 2023-05-03 16:06:48.000000 wikihowapi_pk-0.0.3/wikihowapi_pk.egg-info/top_level.txt
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:54:04.153714 wikihowapi_pk-0.0.4/
+-rw-r--r--   0 piko       (501) staff       (20)     1101 2023-05-03 09:56:00.000000 wikihowapi_pk-0.0.4/LICENSE
+-rw-r--r--   0 piko       (501) staff       (20)     9276 2023-05-06 13:54:04.153475 wikihowapi_pk-0.0.4/PKG-INFO
+-rw-r--r--   0 piko       (501) staff       (20)     8758 2023-05-06 13:52:37.000000 wikihowapi_pk-0.0.4/README.md
+-rw-r--r--   0 piko       (501) staff       (20)       38 2023-05-06 13:54:04.153764 wikihowapi_pk-0.0.4/setup.cfg
+-rw-r--r--   0 piko       (501) staff       (20)      791 2023-05-06 13:49:01.000000 wikihowapi_pk-0.0.4/setup.py
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:54:04.152094 wikihowapi_pk-0.0.4/tests/
+-rw-r--r--   0 piko       (501) staff       (20)      984 2023-05-06 13:02:39.000000 wikihowapi_pk-0.0.4/tests/test.py
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:54:04.152446 wikihowapi_pk-0.0.4/wikihowapi_pk/
+-rw-r--r--   0 piko       (501) staff       (20)    28292 2023-05-06 13:48:18.000000 wikihowapi_pk-0.0.4/wikihowapi_pk/__init__.py
+-rw-r--r--   0 piko       (501) staff       (20)      194 2023-05-03 09:37:40.000000 wikihowapi_pk-0.0.4/wikihowapi_pk/exceptions.py
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-06 13:54:04.153232 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/
+-rw-r--r--   0 piko       (501) staff       (20)     9276 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/PKG-INFO
+-rw-r--r--   0 piko       (501) staff       (20)      278 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/SOURCES.txt
+-rw-r--r--   0 piko       (501) staff       (20)        1 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/dependency_links.txt
+-rw-r--r--   0 piko       (501) staff       (20)        9 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/requires.txt
+-rw-r--r--   0 piko       (501) staff       (20)       14 2023-05-06 13:54:04.000000 wikihowapi_pk-0.0.4/wikihowapi_pk.egg-info/top_level.txt
```

### Comparing `wikihowapi_pk-0.0.3/LICENSE` & `wikihowapi_pk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wikihowapi_pk-0.0.3/setup.py` & `wikihowapi_pk-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='wikihowapi_pk',
-    version='0.0.3',
+    version='0.0.4',
     description='API to extract more data from wikiHow',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/p1k0pan/AdaptiveStoryFinder.git',
     author='p1k0pan',
     author_email='pan.jingheng1998@gmail.com',
     license='MIT',
```

### Comparing `wikihowapi_pk-0.0.3/wikihowapi_pk/__init__.py` & `wikihowapi_pk-0.0.4/wikihowapi_pk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 wikihowAPI_pk
 
 API to extract data from wikiHow.
 """
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 __author__ = 'Aniket Sharma, Ashok Arora, p1k0pan'
 __credits__ = 'Aniket Sharma & Ashok Arora & p1k0pan'
 
 from bs4 import BeautifulSoup
 import urllib.request
 from wikihowapi_pk.exceptions import *
 from datetime import datetime
@@ -787,14 +787,70 @@
             except ParseError:
                 continue
             yield how_to
             count += 1
             if 0 < max_results < count:
                 return
 
+    @ staticmethod
+    def search_homepage(search_term, max_results=10, lang='en') -> list:
+        lang = lang.split('-')[0].lower()
+        if lang not in WikiHow.lang2url:
+            raise UnsupportedLanguage
+        search_url = WikiHow.lang2url[lang] + \
+            'wikiHowTo?search='+urllib.parse.quote(search_term)
+        content = urllib.request.urlopen(search_url)
+        read_content = content.read()
+        soup = BeautifulSoup(read_content, 'html.parser').findAll('a', attrs={
+            'class': 'result_link'})
+
+        result: list = [None]*max_results
+        count = 0
+        for link in soup:
+            result_dict: dict= {}
+            if (count >=max_results):
+                break
+
+            url = link.get('href')
+            if not url.startswith('http'):
+                url = 'http://' + url
+
+            img = link.find('div', {'class': 'result_thumb'})
+            style_attr = img.get('style')
+            img_rul = style_attr.split('url(')[1].split(')')[0]
+
+
+            result_data = link.find('div', {'class': 'result_data'})
+            title = result_data.find('div',{'class': 'result_title'}).text
+            views = result_data.find('li', {'class': 'sr_view'}).text.strip()
+            update = result_data.find('li', {'class': 'sr_updated'}).text
+            update = update[:8].lstrip()+" "+update[8:].strip()
+            sp_verif = result_data.find('li', {'class': 'sp_verif'})
+            if sp_verif:
+                sp_verif = sp_verif.text.strip()
+            else:
+                sp_verif = None
+
+
+
+            result_dict["url"]=url
+            result_dict["img_url"]=img_rul
+            result_dict["title"]=title
+            result_dict["update"] = update
+            result_dict['views'] = views
+            result_dict['sp_verif'] = sp_verif
+
+            result[count] = result_dict
+            count+=1
+
+        return result
+
+
+
+
 
 def random_article(lang='en'):
     """Method to return a random wikiHow article.
 
     Args:
         lang(str, optional): Language of the wikiHow article. Defaults to 'en'.
 
@@ -814,12 +870,15 @@
         lang(str, optional): Language of the wikiHow articles. Defaults to 'en'.
 
     Returns:
         list: A list containing the names of the Wikhow articles from the search result.
     """
     return list(WikiHow.search(query, max_results, lang))
 
+def search_wikihow_link(query, max_results=10, lang='en'):
+    return list(WikiHow.search_homepage(query, max_results, lang))
+
 
 if __name__ == '__main__':
     """This file can only be loaded as a module."""
     exit()
```

