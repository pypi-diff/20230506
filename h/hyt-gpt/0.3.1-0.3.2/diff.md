# Comparing `tmp/hyt-gpt-0.3.1.tar.gz` & `tmp/hyt-gpt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.3.1.tar", last modified: Sat May  6 03:14:37 2023, max compression
+gzip compressed data, was "hyt-gpt-0.3.2.tar", last modified: Sat May  6 03:20:49 2023, max compression
```

## Comparing `hyt-gpt-0.3.1.tar` & `hyt-gpt-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/PKG-INFO
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/hyt_gpt/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-04-19 01:16:56.000000 hyt-gpt-0.3.1/hyt_gpt/__init__.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     4028 2023-05-06 02:42:26.000000 hyt-gpt-0.3.1/hyt_gpt/gpt.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-04-19 01:16:56.000000 hyt-gpt-0.3.1/hyt_gpt/notion.py
--rw-r-----   0 haibinzh (778454) primarygroup (89939)     7271 2023-05-06 03:13:00.000000 hyt-gpt-0.3.1/hyt_gpt/youtube.py
-drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/hyt_gpt.egg-info/
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:14:37.000000 hyt-gpt-0.3.1/hyt_gpt.egg-info/PKG-INFO
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-05-06 03:14:37.000000 hyt-gpt-0.3.1/hyt_gpt.egg-info/SOURCES.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-05-06 03:14:37.000000 hyt-gpt-0.3.1/hyt_gpt.egg-info/dependency_links.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-05-06 03:14:37.000000 hyt-gpt-0.3.1/hyt_gpt.egg-info/top_level.txt
--rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-05-06 03:14:37.867675 hyt-gpt-0.3.1/setup.cfg
--rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-05-06 03:14:22.000000 hyt-gpt-0.3.1/setup.py
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:20:49.760743 hyt-gpt-0.3.2/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:20:49.760743 hyt-gpt-0.3.2/PKG-INFO
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:20:49.756743 hyt-gpt-0.3.2/hyt_gpt/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-04-19 01:16:56.000000 hyt-gpt-0.3.2/hyt_gpt/__init__.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     4000 2023-05-06 03:19:55.000000 hyt-gpt-0.3.2/hyt_gpt/gpt.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-04-19 01:16:56.000000 hyt-gpt-0.3.2/hyt_gpt/notion.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     7245 2023-05-06 03:20:17.000000 hyt-gpt-0.3.2/hyt_gpt/youtube.py
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-06 03:20:49.760743 hyt-gpt-0.3.2/hyt_gpt.egg-info/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-06 03:20:49.000000 hyt-gpt-0.3.2/hyt_gpt.egg-info/PKG-INFO
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-05-06 03:20:49.000000 hyt-gpt-0.3.2/hyt_gpt.egg-info/SOURCES.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-05-06 03:20:49.000000 hyt-gpt-0.3.2/hyt_gpt.egg-info/dependency_links.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-05-06 03:20:49.000000 hyt-gpt-0.3.2/hyt_gpt.egg-info/top_level.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-05-06 03:20:49.760743 hyt-gpt-0.3.2/setup.cfg
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-05-06 03:20:41.000000 hyt-gpt-0.3.2/setup.py
```

### Comparing `hyt-gpt-0.3.1/PKG-INFO` & `hyt-gpt-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.1/hyt_gpt/gpt.py` & `hyt-gpt-0.3.2/hyt_gpt/gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     response = requests.post(
         'https://api.openai.com/v1/chat/completions', headers=headers, json=json_data)
     # Return Error message if response is not 200
     if response.status_code != 200:
         logging.info('response:', response.content)
         return str(response.json()['error'])
 
-    print(response.json())
-
     return response.json()['choices'][0]['message']['content']
 
 
 def seg_transcript(transcript: List[str]) -> List[str]:
     transcript = [{"text": item["text"], "index": index,
                    "timestamp": item["start"]} for index, item in enumerate(transcript)]
     text = " ".join([x["text"]
```

### Comparing `hyt-gpt-0.3.1/hyt_gpt/notion.py` & `hyt-gpt-0.3.2/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.3.1/hyt_gpt/youtube.py` & `hyt-gpt-0.3.2/hyt_gpt/youtube.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                 "status": "failed",
                 "url": ylink,
                 "subtitles": subtitles,
                 "summaries": "Subtitle retrieval failed",
             }
 
         seged_text = seg_transcript(subtitles)
-        print(seged_text)
         summaried_text = ""
         i = 1
 
         for entry in seged_text:
             try:
                 response = chat_gpt(
                     self.gpt_key, self.prompt.format(language=language), entry
```

### Comparing `hyt-gpt-0.3.1/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.3.2/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.3.1/setup.py` & `hyt-gpt-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.3.1',
+    version='0.3.2',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

