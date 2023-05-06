# Comparing `tmp/hyt-gpt-0.3.0.tar.gz` & `tmp/hyt-gpt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.3.0.tar", last modified: Fri May  5 18:28:51 2023, max compression
+gzip compressed data, was "hyt-gpt-0.3.1.tar", last modified: Sat May  6 03:14:37 2023, max compression
```

## Comparing `hyt-gpt-0.3.0.tar` & `hyt-gpt-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/PKG-INFO
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/hyt_gpt/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-04-19 01:16:56.000000 hyt-gpt-0.3.0/hyt_gpt/__init__.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     4000 2023-04-19 01:16:56.000000 hyt-gpt-0.3.0/hyt_gpt/gpt.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-04-19 01:16:56.000000 hyt-gpt-0.3.0/hyt_gpt/notion.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     6904 2023-05-05 18:26:17.000000 hyt-gpt-0.3.0/hyt_gpt/youtube.py
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/hyt_gpt.egg-info/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-05 18:28:51.000000 hyt-gpt-0.3.0/hyt_gpt.egg-info/PKG-INFO
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-05-05 18:28:51.000000 hyt-gpt-0.3.0/hyt_gpt.egg-info/SOURCES.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-05-05 18:28:51.000000 hyt-gpt-0.3.0/hyt_gpt.egg-info/dependency_links.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-05-05 18:28:51.000000 hyt-gpt-0.3.0/hyt_gpt.egg-info/top_level.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/setup.cfg
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-05-05 18:28:33.000000 hyt-gpt-0.3.0/setup.py
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/PKG-INFO
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/hyt_gpt/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-04-19 01:16:56.000000 hyt-gpt-0.3.1/hyt_gpt/__init__.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     4028 2023-05-06 02:42:26.000000 hyt-gpt-0.3.1/hyt_gpt/gpt.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-04-19 01:16:56.000000 hyt-gpt-0.3.1/hyt_gpt/notion.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     7271 2023-05-06 03:13:00.000000 hyt-gpt-0.3.1/hyt_gpt/youtube.py
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/hyt_gpt.egg-info/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:14:37.000000 hyt-gpt-0.3.1/hyt_gpt.egg-info/PKG-INFO
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-05-06 03:14:37.000000 hyt-gpt-0.3.1/hyt_gpt.egg-info/SOURCES.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-05-06 03:14:37.000000 hyt-gpt-0.3.1/hyt_gpt.egg-info/dependency_links.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-05-06 03:14:37.000000 hyt-gpt-0.3.1/hyt_gpt.egg-info/top_level.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/setup.cfg
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-05-06 03:14:22.000000 hyt-gpt-0.3.1/setup.py
```

### Comparing `hyt-gpt-0.3.0/PKG-INFO` & `hyt-gpt-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.0/hyt_gpt/gpt.py` & `hyt-gpt-0.3.1/hyt_gpt/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,27 @@
     response = requests.post(
         'https://api.openai.com/v1/chat/completions', headers=headers, json=json_data)
     # Return Error message if response is not 200
     if response.status_code != 200:
         logging.info('response:', response.content)
         return str(response.json()['error'])
 
+    print(response.json())
+
     return response.json()['choices'][0]['message']['content']
 
 
 def seg_transcript(transcript: List[str]) -> List[str]:
     transcript = [{"text": item["text"], "index": index,
                    "timestamp": item["start"]} for index, item in enumerate(transcript)]
     text = " ".join([x["text"]
                     for x in sorted(transcript, key=lambda x: x["index"])])
     enc = tiktoken.get_encoding("cl100k_base")
     len_original = len(enc.encode(text))
-    seg_length = 4000
+    seg_length = 3500
     if len_original >= seg_length:
         chunkedText = getChunckedTranscripts(transcript, transcript, enc)
         print(
             f'Transcript token length: {len_original} is too long, truncated via lossy compression to {len(enc.encode(chunkedText))}.')
         return [chunkedText]
     print(f'Processing text token length: {len_original}.')
     n = len_original // seg_length + 1
@@ -55,15 +57,15 @@
 A helpful rule of thumb is that one token generally corresponds to ~4 
 characters of text for common English text. 
 
 This translates to roughly ¾ of a word (so 100 tokens ~= 75 words).
 """
 
 
-def getChunckedTranscripts(textData, textDataOriginal, enc, limit=4000) -> str:
+def getChunckedTranscripts(textData, textDataOriginal, enc, limit=3500) -> str:
 
     result = ""
     text = " ".join([x["text"]
                     for x in sorted(textData, key=lambda x: x["index"])])
 
     if len(enc.encode(text)) > limit:
         evenTextData = [t for i, t in enumerate(textData) if i % 2 == 0]
```

### Comparing `hyt-gpt-0.3.0/hyt_gpt/notion.py` & `hyt-gpt-0.3.1/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.0/hyt_gpt/youtube.py` & `hyt-gpt-0.3.1/hyt_gpt/youtube.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,112 @@
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Union, Tuple
 from .gpt import seg_transcript, chat_gpt
 from datetime import datetime
 from youtube_transcript_api import YouTubeTranscriptApi
 import traceback
 import re
 
 headers = {
-    'authority': 'api.youtube.com',
-    'accept': 'application/json, text/plain, */*',
-    'user-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3',
-    'accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
+    "authority": "api.youtube.com",
+    "accept": "application/json, text/plain, */*",
+    "user-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
+    "accept-Language": "zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6",
 }
 
+
 class HytGpt:
     def __init__(self, gpt_key: str, prompt: str):
         self.gpt_key = gpt_key
         self.prompt = prompt
-        
+
     def summary(self, ylink: str) -> Dict[str, str]:
         if not self.is_valid_youtube_url(ylink):
-            return {'status': 'failed', 'url': ylink, 'subtitles': [], 'summaries': 'Invalid youtube url'}
-        subtitles = self.__youtube_subtitle(ylink)
+            return {
+                "status": "failed",
+                "url": ylink,
+                "subtitles": [],
+                "summaries": "Invalid youtube url",
+            }
+        subtitles, language = self.__youtube_subtitle(ylink)
         if not subtitles:
-            return {'status': 'failed', 'url': ylink, 'subtitles': subtitles, 'summaries': 'Subtitle retrieval failed'}
+            return {
+                "status": "failed",
+                "url": ylink,
+                "subtitles": subtitles,
+                "summaries": "Subtitle retrieval failed",
+            }
 
         seged_text = seg_transcript(subtitles)
-        summaried_text = ''
+        print(seged_text)
+        summaried_text = ""
         i = 1
+
         for entry in seged_text:
             try:
-                response = chat_gpt(self.gpt_key, self.prompt, entry)
-                print(f'Completed the {str(i)} part summary')
+                response = chat_gpt(
+                    self.gpt_key, self.prompt.format(language=language), entry
+                )
+                print(f"Completed the {str(i)} part summary")
                 i += 1
             except Exception as e:
                 print(f"Exception occurred: {str(e)}")
                 traceback.print_exc()
-                response = 'Summary failed'
-            summaried_text += response + '\n'
+                response = "Summary failed"
+            summaried_text += response + "\n"
         response_data = {
-            'status': 'success',
-            'url': ylink,
-            'subtitles': subtitles,
-            'summaries': summaried_text,
+            "status": "success",
+            "url": ylink,
+            "subtitles": subtitles,
+            "summaries": summaried_text,
         }
         return response_data
 
     @staticmethod
     def is_valid_youtube_url(url):
         # Regular expression pattern for YouTube URLs
         youtube_url_pattern = re.compile(
-            r'(https?://)?(www\.)?(youtube\.com|youtu\.?be)/.+'
+            r"(https?://)?(www\.)?(youtube\.com|youtu\.?be)/.+"
         )
-        
+
         # Check if the URL matches the pattern
         if youtube_url_pattern.match(url):
             return True
         else:
             return False
-        
+
     @staticmethod
     def get_youtube_id(url: str) -> str:
-        youtube_id_match = re.search(r'(?<=v=)[^&#]+', url)
-        youtube_id_match = youtube_id_match or re.search(r'(?<=be/)[^&#]+', url)
+        youtube_id_match = re.search(r"(?<=v=)[^&#]+", url)
+        youtube_id_match = youtube_id_match or re.search(r"(?<=be/)[^&#]+", url)
         return youtube_id_match.group(0) if youtube_id_match else None
-    
+
     @staticmethod
     def build_youtube_url(youtube_id: str) -> str:
-        return f'https://www.youtube.com/watch?v={youtube_id}'
-    
+        return f"https://www.youtube.com/watch?v={youtube_id}"
+
     @staticmethod
     def get_timestamp_diff(start_time, end_time):
-        start_time = datetime.strptime(start_time, '%H:%M:%S.%f')
-        end_time = datetime.strptime(end_time, '%H:%M:%S.%f')
+        start_time = datetime.strptime(start_time, "%H:%M:%S.%f")
+        end_time = datetime.strptime(end_time, "%H:%M:%S.%f")
         diff = (end_time - start_time).total_seconds()
         return diff
-    
-    def __youtube_subtitle(self, url: str) -> List[Dict[str, str]]:
+
+    def __youtube_subtitle(
+        self, url: str
+    ) -> Tuple[Union[List[Dict[str, str]], None], str]:
         video_id = self.get_youtube_id(url)
         list = YouTubeTranscriptApi.list_transcripts(video_id)
-        en_transicript = list.find_transcript(['en'])
-        if 'zh-Hans' in en_transicript.translation_languages:
-            translated = en_transicript.translate('zh-Hans').fetch()
-            return translated
-        return en_transicript.fetch()        
+        for transcript in list:
+            if transcript.language_code in ["en", "zh-Hans", "zh-Hant"]:
+                return transcript.fetch(), transcript.language
+        # if 'zh-Hans' in transicript.translation_languages:
+        #     translated = transicript.translate('zh-Hans').fetch()
+        #     return translated
+        return None
+
 
 """
 5/5/23: Older version
 
     def __youtube_player_list(self, yvid):
         url = f"https://www.youtube.com/watch?v={yvid}"
         response = requests.request("GET", url, headers=headers)
@@ -173,8 +193,8 @@
 
     def __to_subtitle_list(self, subtitles):
         results = []
         for subtitle in subtitles:
             if 'text' in subtitle:
                 results.append(subtitle.get('text'))
         return results
-"""
+"""
```

### Comparing `hyt-gpt-0.3.0/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.3.1/hyt_gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.0/setup.py` & `hyt-gpt-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.3.0',
+    version='0.3.1',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

