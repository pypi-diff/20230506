# Comparing `tmp/subsscraper-0.1.3.tar.gz` & `tmp/subsscraper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsscraper-0.1.3.tar", max compression
+gzip compressed data, was "subsscraper-0.1.4.tar", max compression
```

## Comparing `subsscraper-0.1.3.tar` & `subsscraper-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      506 2023-04-25 17:00:16.740268 subsscraper-0.1.3/README.md
--rw-r--r--   0        0        0      473 2023-04-25 17:00:27.936935 subsscraper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 16:15:03.420177 subsscraper-0.1.3/src/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 16:29:46.093540 subsscraper-0.1.3/src/conf/__init__.py
--rw-r--r--   0        0        0      349 2023-04-25 16:15:03.420177 subsscraper-0.1.3/src/conf/config.yaml
--rw-r--r--   0        0        0     1436 2023-04-25 16:15:03.420177 subsscraper-0.1.3/src/search.py
--rw-r--r--   0        0        0     2872 2023-04-25 16:40:48.026895 subsscraper-0.1.3/src/subscraper.py
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 subsscraper-0.1.3/setup.py
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 subsscraper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      664 2023-05-06 08:28:50.340231 subsscraper-0.1.4/README.md
+-rw-r--r--   0        0        0      473 2023-05-06 08:29:46.846900 subsscraper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 16:15:03.420177 subsscraper-0.1.4/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:29:46.093540 subsscraper-0.1.4/src/conf/__init__.py
+-rw-r--r--   0        0        0      403 2023-05-06 08:24:07.236888 subsscraper-0.1.4/src/conf/config.yaml
+-rw-r--r--   0        0        0     1436 2023-05-06 07:50:11.646818 subsscraper-0.1.4/src/search.py
+-rw-r--r--   0        0        0     3084 2023-05-06 08:22:10.556884 subsscraper-0.1.4/src/subscraper.py
+-rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 subsscraper-0.1.4/setup.py
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 subsscraper-0.1.4/PKG-INFO
```

### Comparing `subsscraper-0.1.3/src/search.py` & `subsscraper-0.1.4/src/search.py`

 * *Files identical despite different names*

### Comparing `subsscraper-0.1.3/src/subscraper.py` & `subsscraper-0.1.4/src/subscraper.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,44 +8,50 @@
 from omegaconf import DictConfig
 from yt_dlp import YoutubeDL
 
 
 @hydra.main(version_base=None, config_path="conf", config_name="config")
 def main(cfg: DictConfig) -> None:
     output_path = Path(cfg.scraper.output_folder)
-    output_path.mkdir(exist_ok=True)
+    output_path.mkdir(exist_ok=True, parents=True)
     tmp_path = output_path / 'tmp'
 
     urls_path = Path(cfg.search.output_folder) / cfg.search.result_file
-    with open(urls_path) as f:
-        urls = list(dict.fromkeys(s.strip() for s in f.readlines()))
+    try:
+        with open(urls_path) as f:
+            urls = list(dict.fromkeys(s.strip() for s in f.readlines()))
+    except FileNotFoundError:
+        logger.error(f'Urls file not found: {urls_path}')
+        return
+
+    audio_format: str = cfg.scraper.audio_format
+    download_lvl: str = cfg.scraper.lvl
 
     ydl_opts = {
-        # 'subtitleslangs': ['ru'],
-        # 'writesubtitles': True,
         'chapter': True,
         'format': 'm4a/bestaudio/best',
-        # 'postprocessors': [{  # Extract audio using ffmpeg
-        #     'key': 'FFmpegExtractAudio',
-        #     'preferredcodec': 'm4a',
-        # }]
+        'postprocessors': [{
+            'key': 'FFmpegExtractAudio',
+            'preferredcodec': f'{audio_format}',
+            # 'preferredquality': '10',
+        }],
         'paths': dict(home=str(tmp_path)),
         'outtmpl': 'audio.%(ext)s'
     }
     with YoutubeDL(ydl_opts) as ydl:
         for url in urls:
             if tmp_path.exists():
                 shutil.rmtree(tmp_path)
             tmp_path.mkdir()
 
             video_info = ydl.extract_info(url, download=False)
             video_id = video_info['id']
             path = output_path / video_id
             if path.exists():
-                logger.warning(f'Video {video_info.get("id")} downloaded. Skipping.')
+                logger.warning(f'Audio {video_info.get("id")} downloaded. Skipping.')
                 continue
 
             chapters = video_info['chapters']
             auto_subs = True
             if video_info.get('subtitles') is None or video_info.get('subtitles').get('ru') is None:
                 subs_data = video_info['automatic_captions']['ru-orig']
             else:
@@ -71,14 +77,15 @@
                 chapters=chapters,
             )
             json.dump(summary, open(tmp_path / 'info.json', 'w', encoding='utf8'), ensure_ascii=False, indent=2)
 
             subs = requests.get(subs_link).json()
             json.dump(subs, open(tmp_path / 'subs.json', 'w', encoding='utf8'), ensure_ascii=False)
 
-            ydl.download(url)
+            if download_lvl != 'text':
+                ydl.download(url)
 
             shutil.move(tmp_path, path)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `subsscraper-0.1.3/setup.py` & `subsscraper-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['search = src.search:main',
                      'subscrape = src.subscraper:main']}
 
 setup_kwargs = {
     'name': 'subsscraper',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
-    'long_description': 'SubScraper\n---------\n\nRun command for generate urls\n```commandline\nsearch\nsearch search.cnt=2 # for 2 urls\nsearch \'search.query="лекции таймкоды"\' search.cnt=2 # override cyrillic (more quotes)\n```\n\nRun command for subscrape urls\n```commandline\nsubscrape\n```\n\nDefault configs\n```commandline\nsearch:\n  output_folder: data\n  result_file: urls.txt\n  cnt: 10\n  query: машинное обучение лекции таймкоды\n\nscraper:\n  output_folder: ${search.output_folder}/dataset\n```\n\n',
+    'long_description': 'SubsScraper\n---------\n\nRun command for generate urls\n```commandline\nsearch\nsearch search.cnt=2 # for 2 urls\nsearch \'search.query="лекции таймкоды"\' search.cnt=2 # override cyrillic (more quotes)\n```\n\nRun command for subscrape urls\n```commandline\nsubscrape\nsearch scraper.audio_format=mp3 # convert to audio format\nsearch scraper.lvl=text # download only text\n```\n\nDefault configs\n```commandline\nsearch:\n  output_folder: data\n  result_file: urls.txt\n  cnt: 10\n  query: машинное обучение лекции таймкоды\n\nscraper:\n  output_folder: ${search.output_folder}/dataset\n  audio_format: m4a\n  lvl: audio # text, audio, video\n```\n\n',
     'author': 'tupiznak',
     'author_email': 'akej-vonavi@mail.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `subsscraper-0.1.3/PKG-INFO` & `subsscraper-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: subsscraper
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: tupiznak
 Author-email: akej-vonavi@mail.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Description-Content-Type: text/markdown
 
-SubScraper
+SubsScraper
 ---------
 
 Run command for generate urls
 ```commandline
 search
 search search.cnt=2 # for 2 urls
 search 'search.query="лекции таймкоды"' search.cnt=2 # override cyrillic (more quotes)
 ```
 
 Run command for subscrape urls
 ```commandline
 subscrape
+search scraper.audio_format=mp3 # convert to audio format
+search scraper.lvl=text # download only text
 ```
 
 Default configs
 ```commandline
 search:
   output_folder: data
   result_file: urls.txt
   cnt: 10
   query: машинное обучение лекции таймкоды
 
 scraper:
   output_folder: ${search.output_folder}/dataset
+  audio_format: m4a
+  lvl: audio # text, audio, video
 ```
```

