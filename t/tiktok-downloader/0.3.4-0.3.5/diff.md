# Comparing `tmp/tiktok_downloader-0.3.4.tar.gz` & `tmp/tiktok_downloader-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok_downloader-0.3.4.tar", last modified: Sat Aug  6 10:16:41 2022, max compression
+gzip compressed data, was "tiktok_downloader-0.3.5.tar", last modified: Sat May  6 00:35:36 2023, max compression
```

## Comparing `tiktok_downloader-0.3.4.tar` & `tiktok_downloader-0.3.5.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-06 10:16:41.445483 tiktok_downloader-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-08-06 10:16:41.445483 tiktok_downloader-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5431 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-06 10:16:41.445483 tiktok_downloader-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-06 10:16:41.441483 tiktok_downloader-0.3.4/tiktok_downloader/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/Except.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/mdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/scrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/snaptik.py
--rw-r--r--   0 runner    (1001) docker     (121)     3486 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/ssstik.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-06 10:16:41.445483 tiktok_downloader-0.3.4/tiktok_downloader/static/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/static/loading.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/static/script.js
--rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/static/tiktok.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-06 10:16:41.445483 tiktok_downloader-0.3.4/tiktok_downloader/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/tikdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/tikmate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/ttdownloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-08-06 10:16:33.000000 tiktok_downloader-0.3.4/tiktok_downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-06 10:16:41.441483 tiktok_downloader-0.3.4/tiktok_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-08-06 10:16:41.000000 tiktok_downloader-0.3.4/tiktok_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-08-06 10:16:41.000000 tiktok_downloader-0.3.4/tiktok_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-06 10:16:41.000000 tiktok_downloader-0.3.4/tiktok_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-08-06 10:16:41.000000 tiktok_downloader-0.3.4/tiktok_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-06 10:16:41.000000 tiktok_downloader-0.3.4/tiktok_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:35:36.102436 tiktok_downloader-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-06 00:35:36.102436 tiktok_downloader-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:35:36.102436 tiktok_downloader-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-06 00:35:19.000000 tiktok_downloader-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:35:36.098436 tiktok_downloader-0.3.5/tiktok_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/Except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/mdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/scrapper_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/snaptik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/ssstik.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:35:36.102436 tiktok_downloader-0.3.5/tiktok_downloader/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/static/loading.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/static/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/static/tiktok.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:35:36.102436 tiktok_downloader-0.3.5/tiktok_downloader/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/tikdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/tikmate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/tiktok_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/tikwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/ttdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-06 00:35:18.000000 tiktok_downloader-0.3.5/tiktok_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:35:36.098436 tiktok_downloader-0.3.5/tiktok_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-06 00:35:36.000000 tiktok_downloader-0.3.5/tiktok_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-06 00:35:36.000000 tiktok_downloader-0.3.5/tiktok_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:35:36.000000 tiktok_downloader-0.3.5/tiktok_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 00:35:36.000000 tiktok_downloader-0.3.5/tiktok_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 00:35:36.000000 tiktok_downloader-0.3.5/tiktok_downloader.egg-info/top_level.txt
```

### Comparing `tiktok_downloader-0.3.4/README.md` & `tiktok_downloader-0.3.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,40 +31,40 @@
 
 </details>
 
 <details>
 <summary>Snaptik</summary>
 
 ```python
->>> from tiktok_downloader import Snaptik
+>>> from tiktok_downloader import snaptik
 >>> d=Snaptik('https://vt.tiktok.com/xxxxxx/')
 >>> d
 [<[type: "video" watermark: False]>]
 >>> d[0].download('video.mp4')
 ```
 </details>
 
 <details>
 <summary>Musically Down</summary>
 
 ```python
->>> from tiktok_downloader import Mdown
->>> d=Mdown('https://vt.tiktok.com/xxxxxx/')
+>>> from tiktok_downloader import mdown
+>>> d=mdown('https://vt.tiktok.com/xxxxxx/')
 >>> d
 [<[type: "video" watermark: False]>]
 >>> d[0].download('video.mp4')
 ```
 </details>
 
 <details>
 <summary>Tikdown</summary>
 
 ```python
->>> from tiktok_downloader import TikDown
->>> d=TikDown('https://vt.tiktok.com/xxxxxx/')
+>>> from tiktok_downloader import tikdown
+>>> d=tikdown('https://vt.tiktok.com/xxxxxx/')
 >>> d
 [<[type: "video" watermark: False]>]
 >>> d[0].download('video.mp4')
 ```
 </details>
 
 <details>
@@ -76,51 +76,64 @@
 >>> d
 [<[type: "video" watermark: False]>]
 >>> d[0].download('video.mp4')
 ```
 </details>
 
 <details>
+<summary>Tikwm</summary>
+
+```python
+>>> from tiktok_downloader import tikwm
+>>> d=tikwm('https://vt.tiktok.com/xxxxxx/')
+>>> d
+[<[type: "video" watermark: False]>]
+>>> d[0].download('video.mp4')
+```
+</details>
+
+<details>
 <summary>Tiktok</summary>
 
 ```python
->>> from tiktok_downloader import info_post
->>> d=info_post.service('https://vt.tiktok.com/xxxxxx/')
+>>> from tiktok_downloader import VideoInfo
+>>> d=VideoInfo.service('https://vt.tiktok.com/xxxxxx/')
 >>> d
 [<[type: "video" watermark: False]>]
 >>> d[0].download('video.mp4')
 ```
 </details>
 
 <details>
 <summary>Get Info</summary>
 
 ```python
->>> from tiktok_downloader import info_post
->>> info_post('https://vt.tiktok.com/xxxxxx/')
+>>> from tiktok_downloader import VideoInfo
+>>> VideoInfo.get_info('https://vt.tiktok.com/xxxxxx/')
 ```
 </details>
 
 # Command line
 
 ```
-usage: python3 -m tiktok_downloader [-h] [--snaptik | --ssstik | --tikmate | --mdown | --ttdownloader | --tikdown | --tiktok] [--host HOST] [--debug] [--port PORT] (--server | --url URL) [--info] [--json | --save SAVE]
+usage: python3 -m tiktok_downloader [-h] [--snaptik | --ssstik | --tikmate | --mdown | --ttdownloader | --tikwm | --tikdown | --tiktok] [--host HOST] [--debug] [--port PORT] (--server | --url URL) [--info] [--json | --save SAVE]
 
 Tiktok Downloader [CLI]
 
 options:
   -h, --help      show this help message and exit
 
 List Of Services:
   --snaptik
   --ssstik
   --tikmate
   --mdown
   --ttdownloader
   --tikdown
+  --tikwm
   --tiktok
 
 Web Configuration:
   --host HOST     Set host to run this web
   --debug         Set flask mode to debug
   --port PORT     Set port
 
@@ -179,21 +192,22 @@
 $ wget -O result.mp4 $(curl -sG http://127.0.0.1:8000/snaptik -d url=https://vm.tiktok.com/xxxxxxxx/|jq .[0].url -r)
 ```
 ## you can direct Download using browser or curl
 ```
 http://127.0.0.1:8000/snaptik?url=https://vm.tiktok.com/xxxxxxxx/&type=embed
 ```
 ### Endpoint 
-| Name | Endpoint | Status|
-|----|---------|--------|
-| <a href="https://snaptik.app">Snaptik</a> | /snaptik | ✓
-| <a href="https://tikmate.online">Tikmate</a> | /tikmate |✓
-| <a href="https://musicaldown.com/">MusicalDown | /mdown|✓
-| <a href="https://ssstik.io">ssstik</a> | /ssstik | x
+| Name                                                 | Endpoint      | Status|
+|------------------------------------------------------|---------------|--------|
+| <a href="https://snaptik.app">Snaptik</a>            | /snaptik      | ✓
+| <a href="https://tikmate.online">Tikmate</a>         | /tikmate      |✓
+| <a href="https://musicaldown.com/">MusicalDown       | /mdown        |✓
+| <a href="https://ssstik.io">ssstik</a>               | /ssstik       | ✓
 | <a href="https://ttdownloader.com/">ttdownloader</a> | /ttdownloader | ✓
-| <a href="https://tikdown.org/">tikdown</a> | /tikdown | ✓
-| <a href="https://tiktok.com/">tiktok</a> | /tiktok | ✓
+| <a href="https://www.tikwm.com/">tikwm</a>           | /tikwm        | ✓
+| <a href="https://tikdown.org/">tikdown</a>           | /tikdown      | x
+| <a href="https://tiktok.com/">tiktok</a>             | /tiktok       | ✓
 # Donasi
 <p align="center"><img src="https://svgur.com/i/Vtt.svg">
 
 </p>
 <ul><li><a href="https://saweria.co/kryptonbyte">Saweria</a><li><a href="https://wa.me/6283172366463">Whatsapp</a></li><li><a href="https://trakteer.id/krypton-byte-z8vbo">Trakteer</a></li></ul>
```

### Comparing `tiktok_downloader-0.3.4/setup.py` & `tiktok_downloader-0.3.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 from os import path
 base_dir = path.abspath(path.dirname(__file__))
 setup(
   name='tiktok_downloader',
   packages=['tiktok_downloader'],
   include_package_data=True,
-  version='0.3.4',
+  version='0.3.5',
   license='MIT',
   description='Tiktok Downloader&Scraper using bs4&requests',
   author='Krypton Byte',
   author_email='galaxyvplus6434@gmail.com',
   url='https://github.com/krypton-byte/tiktok_downloader',
   keywords=[
     'tiktok',
@@ -21,15 +21,17 @@
   ],
   install_requires=[
           'bs4',
           'flask',
           'cloudscraper',
           'requests',
           'rich',
-          'tqdm'
+          'tqdm',
+          'httpx',
+          'aiohttp'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.9',
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/__init__.py` & `tiktok_downloader-0.3.5/tiktok_downloader/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from .snaptik import snaptik, Snaptik
-from .ssstik import ssstik, Ssstik
-from .scrapper import info_post
+from .ssstik import ssstik
+from .scrapper import VideoInfo
 from .tikmate import tikmate, Tikmate
 from .mdown import mdown, Mdown
 from .Except import InvalidUrl
-from .ttdownloader import ttdownloader
-from .tikdown import TikDown
+from .ttdownloader import ttdownloader, TTDownloader
+from .tikdown import tikdown, Tikdown
+from .tikwm import tikwm, TikWM
 
 __all__ = [
     'snaptik',
+    'Snaptik',
     'ssstik',
-    'info_post',
+    'VideoInfo',
     'tikmate',
+    'Tikmate',
     'mdown',
+    'Mdown',
     'InvalidUrl',
     'ttdownloader',
-    'TikDown'
+    'tikdown',
+    'Tikdown',
+    'TTDownloader',
+    'tikwm',
+    'TikWM'
 ]
 services = {
-    'snaptik': Snaptik,
-    'ssstik': Ssstik,
-    'tikmate': Tikmate,
-    'mdown': Mdown,
+    'snaptik': snaptik,
+    'ssstik': ssstik,
+    'tikmate': tikmate,
+    'mdown': mdown,
     'ttdownloader': ttdownloader,
-    'tikdown': TikDown,
-    'tiktok': info_post.service
+    'tikdown': tikdown,
+    'tiktok': VideoInfo.service,
+    'tikwm': tikwm
 }
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/__main__.py` & `tiktok_downloader-0.3.5/tiktok_downloader/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import argparse
 import json
 import os
 import sys
 import requests
 from . import services
-from .scrapper import info_post
+from .scrapper import VideoInfo
 from sys import stderr
 from rich import print as print_
 from rich.panel import Panel
 from typing import Optional
 
 
 arg = argparse.ArgumentParser(
     prog=f"python3 -m {os.path.dirname(__file__).split('/')[-1]}",
     description='Tiktok Downloader [CLI]'
 )
 
 # Services
 servgroup = arg.add_argument_group('List Of Services')
 serg = servgroup.add_mutually_exclusive_group()
-for key in services.keys():
-    serg.add_argument(f'--{key}', action='store_true')
+for key, value in services.items():
+    serg.add_argument(f'--{key}', dest='service', const=value, action='store_const')
 
 # Web Configuration
 servconf = arg.add_argument_group('Web Configuration')
 servconf.add_argument(
     '--host',
     type=str,
     default='127.0.0.1',
@@ -62,15 +62,15 @@
     '--save',
     type=argparse.FileType('wb'),
     help='Write the result to file')
 parse = arg.parse_args()
 
 
 def info(url: str, js: Optional[bool] = False):
-    infojson = info_post(url)
+    infojson = VideoInfo.get_info(url)
     if js:
         print(json.dumps({
             "id": infojson.id,
             "desc": infojson.desc,
             "duration": infojson.duration,
             "author": infojson.author.username,
             "wm": infojson.downloadLink(True),
@@ -88,48 +88,45 @@
             border_style='bold magenta'))
 
 
 if parse.server:
     from .server import app
     app.run(host=parse.host, port=parse.port, debug=parse.debug)
 elif parse.url:
-    for key, val in services.items():
-        if getattr(parse, key):
-            service = val
-            try:
-                ok = service(parse.url)
-                if parse.json or not(parse.save):
-                    print(
-                        json.dumps(
-                            [
-                                {
-                                    'type': i.type,
-                                    'url': i.json,
-                                    'watermark': i.watermark
-                                } for i in ok
-                            ],
-                            indent=4
-                        )
-                    )
-                elif parse.save:
-                    if parse.info:
-                        info(parse.url, js=parse.json)
-                    ok[0].download(parse.save, bar=True)
-                else:
-                    os.system("python3 -m tiktok_downloader --help")
-            except Exception as e:
-                print(e)
-                stderr.write('Post Not Found\n')
-                stderr.flush()
-                sys.exit(1)
-            except requests.exceptions.ConnectionError:
-                stderr.write('[x] offline\n')
-                stderr.flush()
-                sys.exit(1)
-            except (KeyError, AttributeError):
-                stderr.write('Post Not Found\n')
-                stderr.flush()
-                sys.exit(1)
+    try:
+        ok = parse.service(parse.url)
+        if parse.json or not parse.save:
+            print(
+                json.dumps(
+                    [
+                        {
+                            'type': i.type,
+                            'url': i.json,
+                            'watermark': i.watermark
+                        } for i in ok
+                    ],
+                    indent=4
+                )
+            )
+        elif parse.save:
+            if parse.info:
+                info(parse.url, js=parse.json)
+            ok[0].download(parse.save, bar=True)
+        else:
+            os.system("python3 -m tiktok_downloader --help")
+    except requests.exceptions.ConnectionError:
+        stderr.write('[x] offline\n')
+        stderr.flush()
+        sys.exit(1)
+    except (KeyError, AttributeError):
+        stderr.write('Post Not Found\n')
+        stderr.flush()
+        sys.exit(1)
+    except Exception as e:
+        print(e)
+        stderr.write('Post Not Found\n')
+        stderr.flush()
+        sys.exit(1)
 elif parse.info and parse.url:
     info(parse.url, js=False)
 else:
     os.system("python3 -m tiktok_downloader --help")
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/decoder.py` & `tiktok_downloader-0.3.5/tiktok_downloader/decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Menghadeh Convert dari Js ke Py
 # Decryptor For Snaptik/Tikmate Obfuscate
 
 from typing import Union
-
+from ast import literal_eval
+from re import findall
 alpha = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ+/"
 
 
 def search(d: Union[str, list], q: str):
     try:
         return d.index(q)
     except Exception:
@@ -25,14 +26,21 @@
     j = reduces(freduce, list(d)[::-1], 0)
     k = ""
     while j > 0:
         k = i[j % f] + k
         j = int((j - (j % f)) / f)
     return int(k) or 0
 
+def from_string(text: str):
+    return decoder(*literal_eval(
+            findall(
+                r'\(\".*?,.*?,.*?,.*?,.*?.*?\)',
+                text
+            )[0]
+        ))
 
 def reduces(function, iterable, initializer=None) -> int:
     """
     [!] modified reduce function like js
     :https://www.geeksforgeeks.org/reduce-in-python/
     """
     it = iter(iterable)
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/scrapper.py` & `tiktok_downloader-0.3.5/tiktok_downloader/scrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from __future__ import annotations
+from httpx import AsyncClient
 from requests import Session, get
 from re import findall
 from typing import Callable, Optional, Union
-from io import BytesIO
+from io import BufferedWriter, BytesIO
 from datetime import datetime
+import requests
 from .Except import InvalidUrl
-from .utils import info_videotiktok
+from .utils import Download, DownloadAsync
 import re
 
 
 def extract_id(
-    initf: Callable[[info_post, str], None]
-) -> Callable[[info_post, str], None]:
+    initf: Callable[[VideoInfo, str], VideoInfo]
+) -> Callable[[VideoInfo, str], VideoInfo]:
     subdo_redirect = ['vt', 'vm']
 
     def regex(url: str) -> str:
         if not findall(r'[0-9]{19}', url):
             raise InvalidUrl()
         return findall(r'[0-9]{19}', url)[0]
 
-    def apply(cls: info_post, url: str):
+    def apply(cls: VideoInfo, url: str) -> VideoInfo:
         subdo = re.findall(r'://(\w+)\.', url)
         if subdo and subdo[0] in subdo_redirect:
             url = get(
                 url,
                 allow_redirects=False).text
-        initf(cls, regex(url))
+        return initf(cls, regex(url))
     return apply
 
 
 class Author:
     def __init__(self, ascp: dict):
         self.username = ascp['unique_id']
         self.region = ascp['region']
@@ -41,22 +43,87 @@
         self.create_time = datetime.fromtimestamp(
             ascp['create_time']) if ascp['create_time'] else None
 
     def __repr__(self):
         return f"<[ @{self.username} ]>"
 
 
-class info_post(Session):
-    @extract_id
-    def __init__(self, id: str):
+class VideoInfoAsync(AsyncClient):
+    def __init__(self, js: dict, id: str):
         super().__init__()
-        self.id = findall(r'[0-9]{19}', id)[0]
-        self.aweme = self.get(
+        self.id = id
+        self.aweme = js
+        self.height = (
+            js['aweme_detail']['video']
+            ['download_addr']['height'])
+        self.width = (
+            js['aweme_detail']['video']
+            ['download_addr']['width'])
+        self.size = (
+            js['aweme_detail']
+            ['video']['download_addr']['data_size'])
+        self.desc = js['aweme_detail']['desc']
+        self.cover = (
+            js['aweme_detail']
+            ['video']['origin_cover']['url_list'][0])
+        self.create_time = datetime.fromtimestamp(
+            js['aweme_detail']['create_time'])
+        self.author = Author(js['aweme_detail']['author'])
+        self.music_title = js['aweme_detail']['music']['title']
+        self.music_author = js['aweme_detail']['music']['author']
+        self.music_duration = js['aweme_detail']['music']['duration']
+        self.duration = int(
+            js['aweme_detail']['video']['duration']/1000)
+
+    @classmethod
+    async def url_to_id(cls, url: str, client: AsyncClient):
+        ids = findall(r'[0-9]{19}', url)
+        if ids:
+            return ids[0]
+        url_ = (await client.get(url, follow_redirects=True)).url.__str__()
+        ids = findall(r'[0-9]{19}', url_)
+        if ids:
+            return ids[0]
+        raise InvalidUrl()
+
+    @classmethod
+    async def get_info(cls, url: str):
+        client = AsyncClient()
+        id = await cls.url_to_id(url, client)
+        return cls((await client.get(
             'https://api.tiktokv.com/aweme/v1/aweme/detail/',
-            params={'aweme_id': self.id}).json()
+            params={'aweme_id': id})).json(), id)
+
+    def downloadLink(self, watermark: bool = False) -> str:
+        return self.aweme['aweme_detail']['video'][
+            ['play_addr', 'download_addr'][watermark]
+        ]['url_list'][0]
+
+    def utils(self) -> list[DownloadAsync]:
+        return [
+            DownloadAsync(
+                self.downloadLink(False), self),
+            DownloadAsync(
+                self.downloadLink(True), self, watermark=True),
+            DownloadAsync(
+                self.aweme['aweme_detail']['music']['play_url']['uri'],
+                self,
+                "music"
+            )
+        ]
+
+    def __repr__(self):
+        return f'<[{self.id} {self.duration}s]>'
+
+
+class VideoInfo(Session):
+    def __init__(self, js: dict, id: str):
+        super().__init__()
+        self.id = id
+        self.aweme = js
         self.height = (
             self.aweme['aweme_detail']['video']
             ['download_addr']['height'])
         self.width = (
             self.aweme['aweme_detail']['video']
             ['download_addr']['width'])
         self.size = (
@@ -71,53 +138,61 @@
         self.author = Author(self.aweme['aweme_detail']['author'])
         self.music_title = self.aweme['aweme_detail']['music']['title']
         self.music_author = self.aweme['aweme_detail']['music']['author']
         self.music_duration = self.aweme['aweme_detail']['music']['duration']
         self.duration = int(
             self.aweme['aweme_detail']['video']['duration']/1000)
 
-    def utils(self) -> list[info_videotiktok]:
+    @classmethod
+    @extract_id
+    def get_info(cls, id: str) -> VideoInfo:
+        print('id: ', id)
+        return cls((requests.get(
+            'https://api.tiktokv.com/aweme/v1/aweme/detail/',
+            params={'aweme_id': id})).json(), id)
+
+    def utils(self) -> list[Download]:
         return [
-            info_videotiktok(
+            Download(
                 self.downloadLink(False), self),
-            info_videotiktok(
+            Download(
                 self.downloadLink(True), self, watermark=True),
-            info_videotiktok(
+            Download(
                 self.aweme['aweme_detail']['music']['play_url']['uri'],
                 self,
                 "music"
             )
         ]
 
     @classmethod
-    def service(cls, url: str) -> list[info_videotiktok]:
-        return cls(url).utils()
+    def service(cls, url: str) -> list[Download]:
+        return cls.get_info(url).utils()
 
-    def downloadLink(self, watermark: Optional[bool] = False) -> str:
+    def downloadLink(self, watermark: bool = False) -> str:
         return self.aweme['aweme_detail']['video'][
             ['play_addr', 'download_addr'][watermark]
         ]['url_list'][0]
 
     def download(
         self,
         out: Optional[str] = None,
-        watermark: Optional[bool] = False,
+        watermark: bool = False,
         chunk_size: int = 1024
-    ) -> Union[None, BytesIO]:
+    ) -> Union[None, BytesIO, BufferedWriter]:
         request = self.get(self.downloadLink(watermark), stream=True)
         stream = open(out, 'wb') if isinstance(out, str) else BytesIO()
         for i in request.iter_content(chunk_size):
             stream.write(i)
         return None if isinstance(out, str) else stream
 
     def download_music(
         self,
         out: Optional[str] = None,
         chunk_size: int = 1024
-    ) -> Union[None, BytesIO]:
+    ) -> Union[None, BytesIO, BufferedWriter]:
         request = self.get(
             self.aweme['aweme_detail']['music']['play_url']['uri'],
             stream=True)
         stream = open(out, 'wb') if isinstance(out, str) else BytesIO()
         for i in request.iter_content(chunk_size):
             stream.write(i)
         return None if isinstance(out, str) else stream
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/server.py` & `tiktok_downloader-0.3.5/tiktok_downloader/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from io import BytesIO
 from flask import (
     Flask,
     request,
-    render_template,
-    Response
+    render_template
 )
+from flask.wrappers import Response
 from typing import List
+
+from tiktok_downloader.scrapper_v2 import VideoInfoV2
 from . import services
 from .snaptik import Snaptik
-from .scrapper import info_post
-from .utils import info_videotiktok
+from .scrapper import VideoInfo
+from .utils import Download
 import json
 import os
 
 
 app = Flask(
     __name__,
     template_folder=os.path.abspath(__file__+'/../templates'),
@@ -36,25 +39,26 @@
                     {'msg': 'url parameter required'},
                     indent=4
                 ),
                 content_type='application/json'
             )
         for name, service in serv.items():
             try:
-                b: List[info_videotiktok] = service(request.args.get('url'))
+                b: List[Download] = service(request.args.get('url'))
                 if request.args.get('type') in ['direct', 'embed']:
                     for video in filter(
                         lambda v: v.watermark and v.type == 'video',
                         b
                     ):
                         fvid = video.download()
-                        return Response(
-                            fvid.getvalue(),
-                            content_type='video/mp4'
-                        )
+                        if isinstance(fvid, BytesIO):
+                            return Response(
+                                fvid.getvalue(),
+                                content_type='video/mp4'
+                            )
                 else:
                     return Response(
                         json.dumps(
                             list(
                                 map(lambda x: {
                                     "url": x.json,
                                     "type": x.type,
@@ -92,22 +96,31 @@
     if path == 'info':
         try:
             if not request.args.get('url'):
                 return json.dumps(
                     {'msg': 'url parameter required'},
                     indent=4
                 )
-            resp = info_post(request.args['url'])
-            return Response(
-                    json.dumps(
-                        resp.aweme,
-                        indent=4
-                    ),
-                    content_type='application/json'
-                )
+            if request.args.get('legacy'):
+                resp = VideoInfo.get_info(request.args['url'])
+                return Response(
+                        json.dumps(
+                            {'legacy': True, **resp.aweme},
+                            indent=4
+                        ),
+                        content_type='application/json'
+                    )
+            else:
+                resp = VideoInfoV2.get_info(request.args['url'])
+                return Response(json.dumps({
+                    'id': resp.aweme_id,
+                    'author': resp.username,
+                    'cover': resp.cover,
+                    'caption': resp.caption
+                }))
         except Exception as e:
             print(e)
             return Response(json.dumps({
                 'msg': 'Url is invalid'
             }), headers={'Content-Type': 'application/json'})
     elif path not in services:
         return Response(
@@ -118,18 +131,20 @@
     if request.args.get('url'):
         try:
             service = services.get(path, Snaptik)
             res = service(request.args['url'])
             if request.args.get('type') in ['embed', 'direct']:
                 for i in res:
                     if i.type == 'video':
-                        return Response(
-                            i.download().getvalue(),
-                            content_type='video/mp4'
-                        )
+                        fvid = i.download()
+                        if isinstance(fvid, BytesIO):
+                            return Response(
+                                fvid.getvalue(),
+                                content_type='video/mp4'
+                            )
             return Response(
                 json.dumps(
                     [
                         {
                             'type': i.type,
                             'url': i.json,
                             'watermark': i.watermark
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/ssstik.py` & `tiktok_downloader-0.3.5/tiktok_downloader/snaptik.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,140 @@
-import time
-from bs4 import BeautifulSoup
-from cloudscraper import (
-    create_scraper,
-    Session
-)
-import re
-from .utils import info_videotiktok
-from requests.models import InvalidURL
+from httpx import AsyncClient
+from sys import stderr
+from ast import literal_eval
+from .utils import Download, DownloadAsync
+from .Except import InvalidUrl
+from requests import Session
+from re import findall
+from .decoder import decoder
+import cloudscraper
 
 
-class ssstik(Session):
+class Snaptik(Session):
     '''
-    :param delay:
+    :param tiktok_url:
     ```python
-    >>> tik=ssstik()
-    >>> tik.get_media('....')
-    [<[type:video]>, <[type:video]>, <[type:music]>]
+    >>> tik=snaptik('url')
+    >>> tik.get_media()
+    [<[type:video]>, <[type:video]>]
     ```
     '''
-    BASE = "https://ssstik.io"
-    HEADERS = {
-        "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
-        "hx-active-element": "submit",
-        "hx-current-url": "https://ssstik.io/",
-        "hx-request": "true",
-        "hx-target": "target",
-        "origin": "https://ssstik.io",
-        "sec-fetch-dest": "",
-        "sec-fetch-mode": "cors",
-        "sec-fetch-site": "same-origin",
-        "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 "
-        "(KHTML, like Gecko) Chrome/86.0.4240.111 Safari/537.36"}
-
-    def __init__(self, delay: int = 10, **kwargs) -> None:
-        super().__init__(**kwargs)
-        self.headers = self.HEADERS
-        self.cf = create_scraper(delay=delay)
-        self.html = self.cf.get(self.BASE)
-        while True:
-            if self.html.status_code == 403:
-                print('retrying request')
-                self.cf = create_scraper(delay=delay)
-                self.html = self.cf.get(self.BASE)
-                time.sleep(5)
-            else:
-                break
 
-    def get_media(self, url: str) -> list[info_videotiktok]:
+    def __init__(self, tiktok_url: str) -> None:
+        super().__init__()
+        self.headers: dict[str, str] = {
+                'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) '
+                'AppleWebKit/537.36 (KHTML, like Gecko) '
+                'Chrome/86.0.4240.111 Safari/537.36'
+            }
+        self.tiktok_url = tiktok_url
+
+    def get_media(self) -> list[Download]:
+        '''
+        ```python
+        >>> <snaptik object>.get_media()
+        [<[type:video]>, <[type:video]>]
+        ```
+        '''
+        resp = cloudscraper.create_scraper().get(
+            'https://snaptik.app/abc2.php',
+            params={
+                'url': self.tiktok_url,
+                'lang': 'en',
+                **dict(
+                    findall(
+                        'name="(token)" value="(.*?)"',
+                        self.get('https://snaptik.app/en').text))}
+        )
+        if 'error_api_web;' in resp.text or 'Error:' in resp.text:
+            raise InvalidUrl()
+        stderr.flush()
+        dec = decoder(*literal_eval(
+            findall(
+                r'\(\".*?,.*?,.*?,.*?,.*?.*?\)',
+                resp.text
+            )[0]
+        ))
+
+        stderr.flush()
+        return [
+            Download(
+                i,
+                self
+            ) for i in findall(r'<a href=\\"(https?://[\w\./\-&?=]+)', dec)
+        ]
+
+    def __iter__(self):
+        yield from self.get_media()
+
+
+class SnaptikAsync(AsyncClient):
+    '''
+    :param tiktok_url:
+    ```python
+    >>> tik=snaptik('url')
+    >>> tik.get_media()
+    [<[type:video]>, <[type:video]>]
+    ```
+    '''
+
+    def __init__(self, tiktok_url: str) -> None:
+        super().__init__()
+        self.headers: dict[str, str] = {
+                'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) '
+                'AppleWebKit/537.36 (KHTML, like Gecko) '
+                'Chrome/86.0.4240.111 Safari/537.36'
+            }
+        self.tiktok_url = tiktok_url
+
+    async def get_media(self) -> list[DownloadAsync]:
         '''
-        :param url:
         ```python
-        >>> <ssstik object>.get_media('....')
+        >>> <snaptik object>.get_media()
         [<[type:video]>, <[type:video]>]
         ```
         '''
-        try:
-            post = self.cf.post(
-                self.BASE+re.findall(
-                    'hx-post=\"(.*?)\"',
-                    self.html.text
-                )[0],
-                data={
-                    "id": url,
-                    "locale": "en",
-                    "tt": 0,
-                    "ts": 0
-                }
+        resp = await self.get(
+            'https://snaptik.app/abc2.php',
+            params={
+                'url': self.tiktok_url,
+                'lang': 'en',
+                **dict(
+                    findall(
+                        'name="(token)" value="(.*?)"',
+                        (await self.get('https://snaptik.app/en')).text))},
+        )
+        if 'error_api_web;' in resp.text or 'Error:' in resp.text:
+            raise InvalidUrl()
+        stderr.flush()
+        dec = decoder(*literal_eval(
+            findall(
+                r'\(\".*?,.*?,.*?,.*?,.*?.*?\)',
+                resp.text
+            )[0]
+        ))
+
+        stderr.flush()
+        return [
+            DownloadAsync(
+                i,
+                self
             )
-            respon = BeautifulSoup(post.text, "html.parser")
-            hasil = [
-                *[
-                    info_videotiktok(
-                        url=i,
-                        Session=self.cf,
-                        type='video'
-                    )
-                    for i in [
-                        self.BASE+respon.find_all(
-                            "a",
-                            class_="pure-button pure-button-primary \
-                                is-center u-bl dl-button download_link \
-                                without_watermark")[0].get("href"),
-                        respon.find_all(
-                            "a",
-                            class_="pure-button pure-button-primary \
-                                is-center u-bl dl-button download_link \
-                                without_watermark_direct")[0].get("href")
-                        ]
-                ],
-                info_videotiktok(
-                    respon.find_all(
-                        "a",
-                        class_="pure-button pure-button-primary is-center \
-                            u-bl dl-button download_link music"
-                    )[0].get("href"),
-                    Session=self.cf,
-                    type='music'
-                )
-            ]
-            return hasil
-        except IndexError:
-            raise InvalidURL()
+            for i in set(['https://snaptik.app'+x.strip('\\') for x in findall(
+                r'(/file.php?.*?)\"',
+                dec
+            )] + [i.strip('\\') for i in findall(
+                r'\"(https?://snapxcdn.*?)\"',
+                dec
+            )])
+        ]
+
+    async def __aiter__(self):
+        return await self.get_media()
+
+
+def snaptik(url: str):
+    return Snaptik(url).get_media()
 
 
-def Ssstik(url: str, delay=10):
-    return ssstik(delay).get_media(url)
+async def snaptik_async(url: str):
+    return await SnaptikAsync(url).get_media()
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/static/loading.svg` & `tiktok_downloader-0.3.5/tiktok_downloader/static/loading.svg`

 * *Files identical despite different names*

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/static/script.js` & `tiktok_downloader-0.3.5/tiktok_downloader/static/script.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -33,30 +33,58 @@
               const data = await response.json();
               data.msg && Swal.fire({
                   icon: 'error',
                   title: 'Oops...',
                   text: data.msg,
                   showConfirmButton: false
               })
-              $(".emptydiv").empty().append(`
+              if (data.legacy) {
+                  $(".emptydiv").empty().append(`
+                <div class="row justify-content-center" id="downgrup" style="padding-bottom: 100px;">
+                  <div class="card" style="width: 20 rem;background-color:${localStorage.mode === 'black'?'black; border-color: #0D6EFD':'white'}">
+                    <video class="card-img-top" alt="..." poster="${data.aweme_detail.video.origin_cover.url_list[0]}" style="padding-top:7px;" controls>
+                      <source src="${data.aweme_detail.video.play_addr.url_list[0]}" type="video/mp4">
+                    </video>
+                    
+                    <div class="card-body">
+                      <h5 class="card-title"><a href="https://www.tiktok.com/@${data.aweme_detail.author.unique_id}">${data.aweme_detail.author.unique_id}</a></h5>
+                      <p class="card-text ${localStorage.mode === 'black'?'text-white':'text-black'}">${data.aweme_detail.desc}</p>
+                    </div>
+                    ${data.aweme_detail.video.play_addr.url_list.map(function(x){
+                      return '<a href="'+x+'" target="_blank" class="btn btn-primary"> Video </a>&nbsp;';
+                    }).join('')}
+                    <a href="${data.aweme_detail.music.play_url.uri}" target="_blank" class="btn btn-primary mb-3"> Music </a>
+                  </div>
+              </div>
+            `)
+                  $("body").removeClass("loading");
+              } else {
+                  fetch('mdown?' + (new URLSearchParams({
+                      url: document.getElementById('tiktokurl').value
+                  })), {
+                      method: 'GET'
+                  }).then(async (resp) => {
+                      const dj = await resp.json()
+                      $(".emptydiv").empty().append(`
               <div class="row justify-content-center" id="downgrup" style="padding-bottom: 100px;">
                 <div class="card" style="width: 20 rem;background-color:${localStorage.mode === 'black'?'black; border-color: #0D6EFD':'white'}">
-                  <video class="card-img-top" alt="..." poster="${data.aweme_detail.video.origin_cover.url_list[0]}" style="padding-top:7px;" controls>
-                    <source src="${data.aweme_detail.video.play_addr.url_list[0]}" type="video/mp4">
+                  <video class="card-img-top" alt="..." poster="${data.cover}" style="padding-top:7px;" controls>
+                    <source src="${dj[0].url}" type="video/mp4">
                   </video>
                   
                   <div class="card-body">
-                    <h5 class="card-title"><a href="https://www.tiktok.com/@${data.aweme_detail.author.unique_id}">${data.aweme_detail.author.unique_id}</a></h5>
-                    <p class="card-text ${localStorage.mode === 'black'?'text-white':'text-black'}">${data.aweme_detail.desc}</p>
+                    <h5 class="card-title"><a href="https://www.tiktok.com/@${data.author}">${data.author}</a></h5>
+                    <p class="card-text ${localStorage.mode === 'black'?'text-white':'text-black'}">${data.caption}</p>
                   </div>
-                  ${data.aweme_detail.video.play_addr.url_list.map(function(x){
+                  ${dj.slice(1).map(function(x){
                     return '<a href="'+x+'" target="_blank" class="btn btn-primary"> Video </a>&nbsp;';
                   }).join('')}
-                  <a href="${data.aweme_detail.music.play_url.uri}" target="_blank" class="btn btn-primary mb-3"> Music </a>
                 </div>
             </div>
           `)
-              $("body").removeClass("loading");
+                      $("body").removeClass("loading");
+                  })
+              }
           }).catch(function(err) {
               $("body").removeClass("loading");
           })
       }
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/static/tiktok.svg` & `tiktok_downloader-0.3.5/tiktok_downloader/static/tiktok.svg`

 * *Files identical despite different names*

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/templates/index.html` & `tiktok_downloader-0.3.5/tiktok_downloader/templates/index.html`

 * *Files identical despite different names*

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/test.py` & `tiktok_downloader-0.3.5/tiktok_downloader/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import unittest
-from .scrapper import info_post
+from .scrapper import VideoInfo
 from .snaptik import snaptik
 from .tikmate import tikmate
 from .mdown import mdown
 
 
 class TikTok(unittest.TestCase):
     base_url = ('https://www.tiktok.com/' +
                 '@tribunsumselcom/' +
                 'video/7020708969563917595')
 
     def test_snaptk(self):
-        self.assertTrue(snaptik(self.base_url).get_media())
+        self.assertTrue(bool(snaptik(self.base_url)))
 
     def test_info(self):
-        self.assertTrue(bool(info_post(self.base_url)))
+        self.assertTrue(bool(VideoInfo.get_info(self.base_url)))
 
     def tikmat(self):
-        self.assertTrue(tikmate().get_media(self.base_url))
+        self.assertTrue(bool(tikmate(self.base_url)))
 
-    def mdown(self):
-        self.assertTrue(mdown().get_media(self.base_url))
+    def mdown_(self):
+        self.assertTrue(bool(mdown(self.base_url)))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader/tikdown.py` & `tiktok_downloader-0.3.5/tiktok_downloader/tikdown.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from httpx import AsyncClient
 from requests import Session
 import re
-from .utils import info_videotiktok
+from .utils import DownloadAsync, Download
 
 
-class TKDown(Session):
+class Tikdown(Session):
     BASE_URL = 'https://tikdown.org/'
-    headers = {
+    headers: dict[str, str] = {
         "origin": 'https://tikdown.org',
         "referer": 'https://tikdown.org/',
         "sec-ch-ua": '"Chromium";v="94", '
         '"Google Chrome";v="94", ";Not A Brand";v="99"',
         "sec-ch-ua-mobile": '?0',
         "sec-ch-ua-platform": '"Linux"',
         "sec-fetch-dest": 'empty',
@@ -21,15 +22,15 @@
         "x-requested-with": 'XMLHttpRequest'
     }
 
     def __init__(self, url: str) -> None:
         super().__init__()
         self.url = url
 
-    def get_media(self) -> list[info_videotiktok]:
+    def get_media(self) -> list[Download]:
         res = self.get(self.BASE_URL)
         _token = re.findall(
             r'type\="hidden".*?value\="([0-9a-zA-Z]+)"',
             res.text
         )[0]
         self.headers.update({'x-csrf-token': _token})
         js = self.post(self.BASE_URL+'getAjax', data={
@@ -37,13 +38,59 @@
             '_token': _token
         }).json()
         if js.get('status'):
             video = re.findall(
                 r'\"(https?://.*?\.mp4)\"',
                 js['html']
             )[0]
-            return [info_videotiktok(video, self)]
+            return [Download(video, self)]
         return []
 
 
-def TikDown(url: str):
-    return TKDown(url).get_media()
+class TikdownAsync(AsyncClient):
+    BASE_URL = 'https://tikdown.org/'
+    headers: dict[str, str] = {
+        "origin": 'https://tikdown.org',
+        "referer": 'https://tikdown.org/',
+        "sec-ch-ua": '"Chromium";v="94", '
+        '"Google Chrome";v="94", ";Not A Brand";v="99"',
+        "sec-ch-ua-mobile": '?0',
+        "sec-ch-ua-platform": '"Linux"',
+        "sec-fetch-dest": 'empty',
+        "sec-fetch-mode": 'cors',
+        "sec-fetch-site": 'same-origin',
+        "user-agent": 'Mozilla/5.0 (X11; Linux x86_64) '
+        'AppleWebKit/537.36 (KHTML, like Gecko) '
+        'Chrome/94.0.4606.81 Safari/537.36',
+        "x-requested-with": 'XMLHttpRequest'
+    }
+
+    def __init__(self, url: str) -> None:
+        super().__init__()
+        self.url = url
+
+    async def get_media(self) -> list[DownloadAsync]:
+        res = await self.get(self.BASE_URL)
+        _token = re.findall(
+            r'type\="hidden".*?value\="([0-9a-zA-Z]+)"',
+            res.text
+        )[0]
+        self.headers.update({'x-csrf-token': _token})
+        js = (await self.post(self.BASE_URL+'getAjax', data={
+            'url': self.url,
+            '_token': _token
+        })).json()
+        if js.get('status'):
+            video = re.findall(
+                r'\"(https?://.*?\.mp4)\"',
+                js['html']
+            )[0]
+            return [DownloadAsync(video, self)]
+        return []
+
+
+def tikdown(url: str):
+    return Tikdown(url).get_media()
+
+
+async def tikdown_async(url: str):
+    return await TikdownAsync(url).get_media()
```

### Comparing `tiktok_downloader-0.3.4/tiktok_downloader.egg-info/SOURCES.txt` & `tiktok_downloader-0.3.5/tiktok_downloader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 setup.py
 tiktok_downloader/Except.py
 tiktok_downloader/__init__.py
 tiktok_downloader/__main__.py
 tiktok_downloader/decoder.py
 tiktok_downloader/mdown.py
 tiktok_downloader/scrapper.py
+tiktok_downloader/scrapper_v2.py
 tiktok_downloader/server.py
 tiktok_downloader/snaptik.py
 tiktok_downloader/ssstik.py
 tiktok_downloader/test.py
 tiktok_downloader/tikdown.py
 tiktok_downloader/tikmate.py
+tiktok_downloader/tiktok_async.py
+tiktok_downloader/tikwm.py
 tiktok_downloader/ttdownloader.py
 tiktok_downloader/utils.py
 tiktok_downloader.egg-info/PKG-INFO
 tiktok_downloader.egg-info/SOURCES.txt
 tiktok_downloader.egg-info/dependency_links.txt
 tiktok_downloader.egg-info/requires.txt
 tiktok_downloader.egg-info/top_level.txt
```

