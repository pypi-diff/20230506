# Comparing `tmp/hyt-gpt-0.3.3.tar.gz` & `tmp/hyt-gpt-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.3.3.tar", last modified: Sat May  6 03:29:39 2023, max compression
+gzip compressed data, was "hyt-gpt-0.3.4.tar", last modified: Sat May  6 03:33:35 2023, max compression
```

## Comparing `hyt-gpt-0.3.3.tar` & `hyt-gpt-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:29:39.900530 hyt-gpt-0.3.3/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:29:39.900530 hyt-gpt-0.3.3/PKG-INFO
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:29:39.900530 hyt-gpt-0.3.3/hyt_gpt/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-04-19 01:16:56.000000 hyt-gpt-0.3.3/hyt_gpt/__init__.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     4000 2023-05-06 03:19:55.000000 hyt-gpt-0.3.3/hyt_gpt/gpt.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-04-19 01:16:56.000000 hyt-gpt-0.3.3/hyt_gpt/notion.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     7271 2023-05-06 03:28:54.000000 hyt-gpt-0.3.3/hyt_gpt/youtube.py
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:29:39.900530 hyt-gpt-0.3.3/hyt_gpt.egg-info/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:29:39.000000 hyt-gpt-0.3.3/hyt_gpt.egg-info/PKG-INFO
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-05-06 03:29:39.000000 hyt-gpt-0.3.3/hyt_gpt.egg-info/SOURCES.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-05-06 03:29:39.000000 hyt-gpt-0.3.3/hyt_gpt.egg-info/dependency_links.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-05-06 03:29:39.000000 hyt-gpt-0.3.3/hyt_gpt.egg-info/top_level.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-05-06 03:29:39.900530 hyt-gpt-0.3.3/setup.cfg
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-05-06 03:29:32.000000 hyt-gpt-0.3.3/setup.py
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/PKG-INFO
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/hyt_gpt/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-04-19 01:16:56.000000 hyt-gpt-0.3.4/hyt_gpt/__init__.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     4000 2023-05-06 03:19:55.000000 hyt-gpt-0.3.4/hyt_gpt/gpt.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-04-19 01:16:56.000000 hyt-gpt-0.3.4/hyt_gpt/notion.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     7325 2023-05-06 03:33:18.000000 hyt-gpt-0.3.4/hyt_gpt/youtube.py
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/hyt_gpt.egg-info/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:33:35.000000 hyt-gpt-0.3.4/hyt_gpt.egg-info/PKG-INFO
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-05-06 03:33:35.000000 hyt-gpt-0.3.4/hyt_gpt.egg-info/SOURCES.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-05-06 03:33:35.000000 hyt-gpt-0.3.4/hyt_gpt.egg-info/dependency_links.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-05-06 03:33:35.000000 hyt-gpt-0.3.4/hyt_gpt.egg-info/top_level.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-05-06 03:33:35.786681 hyt-gpt-0.3.4/setup.cfg
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-05-06 03:33:29.000000 hyt-gpt-0.3.4/setup.py
```

### Comparing `hyt-gpt-0.3.3/PKG-INFO` & `hyt-gpt-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.3
+Version: 0.3.4
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.3/hyt_gpt/gpt.py` & `hyt-gpt-0.3.4/hyt_gpt/gpt.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.3/hyt_gpt/notion.py` & `hyt-gpt-0.3.4/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.3/hyt_gpt/youtube.py` & `hyt-gpt-0.3.4/hyt_gpt/youtube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Any, List, Union, Tuple
 from .gpt import seg_transcript, chat_gpt
 from datetime import datetime
 from youtube_transcript_api import YouTubeTranscriptApi
 import traceback
+import logging
 import re
 
 headers = {
     "authority": "api.youtube.com",
     "accept": "application/json, text/plain, */*",
     "user-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
     "accept-Language": "zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6",
@@ -90,15 +91,16 @@
         return diff
 
     def __youtube_subtitle(
         self, url: str
     ) -> Tuple[Union[List[Dict[str, str]], None], str]:
         video_id = self.get_youtube_id(url)
         list = YouTubeTranscriptApi.list_transcripts(video_id)
-        print(list)
+        logging.debug("transcript_lists: ", list)
+        
         for transcript in list:
             if transcript.language_code in ["en", "zh", "zh-Hans", "zh-Hant"]:
                 return transcript.fetch(), transcript.language
         # if 'zh-Hans' in transicript.translation_languages:
         #     translated = transicript.translate('zh-Hans').fetch()
         #     return translated
         return None
```

### Comparing `hyt-gpt-0.3.3/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.3.4/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.3
+Version: 0.3.4
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.3/setup.py` & `hyt-gpt-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.3.3',
+    version='0.3.4',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

