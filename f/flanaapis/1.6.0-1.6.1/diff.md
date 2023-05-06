# Comparing `tmp/flanaapis-1.6.0.tar.gz` & `tmp/flanaapis-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flanaapis-1.6.0.tar", last modified: Tue Jan 10 23:08:39 2023, max compression
+gzip compressed data, was "flanaapis-1.6.1.tar", last modified: Sat May  6 18:44:24 2023, max compression
```

## Comparing `flanaapis-1.6.0.tar` & `flanaapis-1.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:08:39.805810 flanaapis-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-10 23:08:23.000000 flanaapis-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-01-10 23:08:39.805810 flanaapis-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-01-10 23:08:23.000000 flanaapis-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:08:39.797810 flanaapis-1.6.0/flanaapis/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:08:39.797810 flanaapis-1.6.0/flanaapis/geolocation/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/geolocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/geolocation/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/geolocation/google_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/geolocation/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/geolocation/open_street_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/geolocation/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:08:39.801810 flanaapis-1.6.0/flanaapis/scraping/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/google_weather_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/instagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/tiktok.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/scraping/yt_dlp_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:08:39.805810 flanaapis-1.6.0/flanaapis/weather/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/weather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/weather/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/weather/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/weather/google.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/weather/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/weather/open_weather_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/weather/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-01-10 23:08:23.000000 flanaapis-1.6.0/flanaapis/weather/visual_crossing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 23:08:39.797810 flanaapis-1.6.0/flanaapis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-01-10 23:08:39.000000 flanaapis-1.6.0/flanaapis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-01-10 23:08:39.000000 flanaapis-1.6.0/flanaapis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 23:08:39.000000 flanaapis-1.6.0/flanaapis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-10 23:08:39.000000 flanaapis-1.6.0/flanaapis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-10 23:08:39.000000 flanaapis-1.6.0/flanaapis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-10 23:08:23.000000 flanaapis-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-01-10 23:08:39.805810 flanaapis-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 18:44:08.000000 flanaapis-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-06 18:44:24.158690 flanaapis-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-06 18:44:08.000000 flanaapis-1.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis/geolocation/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/google_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/open_street_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis/scraping/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/google_weather_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/tiktok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/yt_dlp_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/open_weather_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/visual_crossing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 18:44:08.000000 flanaapis-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-06 18:44:24.162690 flanaapis-1.6.1/setup.cfg
```

### Comparing `flanaapis-1.6.0/LICENSE` & `flanaapis-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/PKG-INFO` & `flanaapis-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: flanaapis
-Version: 1.6.0
+Version: 1.6.1
 Summary: Set of functions that can be used as an imported library or as an api rest running the main.py. There is currently an instance of the api running at https://flanaserver.ddns.net/flanaapis.
 Home-page: https://github.com/AlberLC/flanaapis
 Author: AlberLC
-Author-email: alberlc@outlook.com
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanaapis/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `flanaapis-1.6.0/README.rst` & `flanaapis-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/exceptions.py` & `flanaapis-1.6.1/flanaapis/exceptions.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/geolocation/functions.py` & `flanaapis-1.6.1/flanaapis/geolocation/functions.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/geolocation/google_maps.py` & `flanaapis-1.6.1/flanaapis/geolocation/google_maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import re
 import urllib.parse
 from typing import AsyncIterable
 
 import playwright
-from flanaapis.geolocation.models import Place
 from playwright.async_api import async_playwright
 
+from flanaapis.geolocation.models import Place
+
 
 async def find_place(place_query: str) -> Place | None:
     async with async_playwright() as p:
         async with await p.chromium.launch() as browser:
             try:
                 page: playwright.async_api.Page = await browser.new_page()
                 await page.goto(f"https://www.google.es/maps/search/{'+'.join(place_query.split())}")
-                button = page.locator("'Acepto'")
-                if await button.count():
-                    await button.click()
+                if await (button := page.locator("'Acepto'")).count() or await (button := page.locator("'Aceptar todo'")).count():
+                    await button.first.click()
                 while '@' not in page.url:
                     await page.wait_for_event('framenavigated')
 
                 await page.wait_for_load_state('domcontentloaded')
                 if await page.query_selector("'Google Maps no encuentra'"):
                     return
             except playwright.async_api.TimeoutError:
                 return
 
             try:
-                place_name, latitude, longitude = re.findall(r'(?:place|search)/\d*(.+)/@([\d.-]+),([\d.-]+)', page.url)[0]
+                place_name, latitude, longitude = re.findall('(?:place|search)/\d*(.+)/@([\d.-]+),([\d.-]+)', page.url)[0]
             except IndexError:
                 return
 
             place_name = urllib.parse.unquote(place_name.replace('+', ' ').strip())
 
             return Place(place_name, latitude, longitude)
 
@@ -40,15 +40,15 @@
     async with async_playwright() as p:
         async with await p.chromium.launch() as browser:
             try:
                 page: playwright.async_api.Page = await browser.new_page()
                 yield 'Dirigiéndome a google.es/maps...'
                 await page.goto(f"https://www.google.es/maps/search/{'+'.join(place_query.split())}")
 
-                if await (button := page.locator("button:has-text('Acepto')")).count() or await (button := page.locator("button:has-text('Aceptar todo')")).count():
+                if await (button := page.locator("'Acepto'")).count() or await (button := page.locator("'Aceptar todo'")).count():
                     yield 'Aceptando consentimiento de privacidad...'
                     await button.first.click()
 
                 yield 'Rebuscando coordenadas en la página...'
                 while '@' not in page.url:
                     await page.wait_for_event('framenavigated')
 
@@ -57,15 +57,15 @@
                     yield
                     return
             except playwright.async_api.TimeoutError:
                 yield
                 return
 
             try:
-                place_name, latitude, longitude = re.findall(r'(?:place|search)/\d*(.+)/@([\d.-]+),([\d.-]+)', page.url)[0]
+                place_name, latitude, longitude = re.findall('(?:place|search)/\d*(.+)/@([\d.-]+),([\d.-]+)', page.url)[0]
             except IndexError:
                 yield
                 return
 
             place_name = urllib.parse.unquote(place_name.replace('+', ' ').strip())
 
             yield Place(place_name, latitude, longitude)
```

### Comparing `flanaapis-1.6.0/flanaapis/geolocation/models.py` & `flanaapis-1.6.1/flanaapis/geolocation/models.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/geolocation/open_street_map.py` & `flanaapis-1.6.1/flanaapis/geolocation/open_street_map.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/geolocation/routes.py` & `flanaapis-1.6.1/flanaapis/geolocation/routes.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/main.py` & `flanaapis-1.6.1/flanaapis/main.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/scraping/constants.py` & `flanaapis-1.6.1/flanaapis/scraping/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)",
     "Googlebot/2.1 (+http://www.googlebot.com/bot.html)",
     "Googlebot/2.1 (+http://www.google.com/bot.html)"
 ]
 INSTAGRAM_BASE_URL = 'https://www.instagram.com/'
 INSTAGRAM_CONTENT_PATH = 'p/'
 INSTAGRAM_LOGIN_URL = INSTAGRAM_BASE_URL + 'accounts/login/ajax/'
+INSTAGRAM_USER_AGENT = 'Instagram 123.0.0.21.114 (iPhone; CPU iPhone OS 11_4 like Mac OS X; en_US; en-US; scale=2.00; 750x1334) AppleWebKit/605.1.15'
 REDDIT_BASE_URL = 'https://www.reddit.com/'
 REDDIT_CONTENT_PATH = 'comments/'
 TIKTOK_BASE_URL = 'https://www.tiktok.com/'
 TWITTER_ENDPOINT_V1 = 'https://api.twitter.com/1.1/statuses/lookup.json'
 TWITTER_ENDPOINT_V2 = 'https://api.twitter.com/2/tweets'
-USER_AGENT = 'Instagram 123.0.0.21.114 (iPhone; CPU iPhone OS 11_4 like Mac OS X; en_US; en-US; scale=2.00; 750x1334) AppleWebKit/605.1.15'
-USER_AGENT_2 = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36'
+USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36'
 YT_DLP_WRAPPER_TITLE_MAX_LENGTH = 20
```

### Comparing `flanaapis-1.6.0/flanaapis/scraping/functions.py` & `flanaapis-1.6.1/flanaapis/scraping/functions.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/scraping/google_weather_scraper.py` & `flanaapis-1.6.1/flanaapis/scraping/google_weather_scraper.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/scraping/reddit.py` & `flanaapis-1.6.1/flanaapis/scraping/reddit.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     async with aiohttp.ClientSession() as session:
         for url in urls:
             try:
                 data = await flanautils.get_request(url, session=session)
             except ResponseError:
                 continue
 
+            data = data[0]['data']['children'][0]['data']
             medias |= await get_medias_from_data(
                 data,
                 preferred_video_codec,
                 preferred_extension,
                 force,
                 audio_only,
                 timeout_for_media
@@ -51,36 +52,30 @@
     if audio_only:
         medias = await functions.filter_audios(medias)
 
     return medias
 
 
 async def get_medias_from_data(
-    data: list[dict],
+    data: dict,
     preferred_video_codec: str = None,
     preferred_extension: str = None,
     force=False,
     audio_only=False,
     timeout: int | float = None
 ) -> OrderedSet[Media]:
     medias = OrderedSet()
 
-    data = data[0]['data']['children'][0]['data']
+    for crosspost_data in data.get('crosspost_parent_list', ()):
+        medias |= await get_medias_from_data(crosspost_data)
+
     data['url'] = html.unescape(data['url'])
 
     # image
-    if (
-            data.get('post_hint') == 'image'
-            or
-            data.get('is_reddit_media_domain')
-            and
-            not data.get('is_video')
-            and
-            data['url']
-    ):
+    if data.get('post_hint') == 'image':
         extension = pathlib.Path(data['url']).suffix.strip('.')
         medias.add(Media(data['url'], MediaType.IMAGE, extension, Source.REDDIT))
 
     # images / gifs
     if data.get('media_metadata'):
         if data.get('gallery_data'):
             media_ids = (media_data['media_id'] for media_data in data['gallery_data']['items'])
```

### Comparing `flanaapis-1.6.0/flanaapis/scraping/routes.py` & `flanaapis-1.6.1/flanaapis/scraping/routes.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import base64
 from enum import Enum
 
 from fastapi import APIRouter
 from flanautils import Media
 from pydantic import BaseModel
 
-from flanaapis.scraping import instagram, tiktok, twitter, youtube
+from flanaapis.scraping import instagram, tiktok, twitter, yt_dlp_wrapper
 
 router = APIRouter(prefix='/medias')
 
 
 def media_to_dict(media: Media) -> dict:
     response_media_vars = {}
 
@@ -49,9 +49,9 @@
 
 @router.post('/', response_model=list[MediaOutput], response_model_exclude_defaults=True, response_model_exclude_unset=True)
 async def get_medias(input_: Input):
     return [media_to_dict(media) for media in (
         *await twitter.get_medias(twitter.find_ids(input_.text)),
         *await instagram.get_medias(instagram.find_ids(input_.text)),
         *await tiktok.get_medias(await tiktok.find_ids(input_.text), tiktok.find_download_urls(input_.text)),
-        *await youtube.get_medias(youtube.find_youtube_ids(input_.text))
+        *await yt_dlp_wrapper.get_medias(input_.text)
     )]
```

### Comparing `flanaapis-1.6.0/flanaapis/scraping/tiktok.py` & `flanaapis-1.6.1/flanaapis/scraping/tiktok.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,41 @@
+import random
 import re
 from typing import Iterable
 
 import flanautils
 from flanautils import Media, MediaType, OrderedSet, Source
 
 from flanaapis.exceptions import TikTokMediaNotFoundError
 from flanaapis.scraping import constants, functions, yt_dlp_wrapper
 
 
 async def _find_ids(text: str, pattern: str) -> OrderedSet[str]:
-    return OrderedSet(re.findall(pattern, text), re.findall(pattern, ''.join(await get_desktop_urls(text))))
+    return OrderedSet(re.findall(pattern, '\n'.join((text, *await get_desktop_urls(text)))))
 
 
 def find_download_urls(text: str) -> OrderedSet[str]:
-    partial_download_urls = re.findall(r'web\.tiktok\.com.+=&vr=', text)
+    partial_download_urls = re.findall('web\.tiktok\.com.+=&vr=', text)
     return OrderedSet(f'https://v16-{partial_download_url}' for partial_download_url in partial_download_urls)
 
 
 async def find_ids(text: str) -> OrderedSet[str]:
     return await _find_ids(text, 'tok.*[tv](?:ideo)?/(\d+)')
 
 
 async def find_users_and_ids(text: str) -> OrderedSet[str]:
     return await _find_ids(text, 'tok\.com/(.*/\d+)')
 
 
 async def get_desktop_urls(text: str) -> OrderedSet[str]:
-    mobile_ids = re.findall(r'vm\.tiktok\.com/(\w+)', text)
+    mobile_ids = re.findall('vm\.tiktok\.com/(\w+)', text)
     mobile_urls = [f'https://vm.tiktok.com/{mobile_id}/' for mobile_id in mobile_ids]
-    t_ids = re.findall(r'tok.*t/(\w+)', text)
+    t_ids = re.findall('tok.*t/(\w+)', text)
     t_urls = [f'{constants.TIKTOK_BASE_URL}t/{t_id}' for t_id in t_ids]
-    return OrderedSet([str((await flanautils.get_request(mobile_url, headers={'User-Agent': constants.USER_AGENT}, return_response=True)).url) for mobile_url in mobile_urls + t_urls])
+    return OrderedSet([str((await flanautils.get_request(mobile_url, headers={'User-Agent': random.choice(constants.GOOGLE_BOT_USER_AGENTS)}, return_response=True)).url) for mobile_url in mobile_urls + t_urls])
 
 
 async def get_medias(
     users_and_ids: Iterable[str] = (),
     download_urls: Iterable[str] = (),
     preferred_video_codec: str = None,
     preferred_extension: str = None,
```

### Comparing `flanaapis-1.6.0/flanaapis/scraping/twitter.py` & `flanaapis-1.6.1/flanaapis/scraping/twitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 from flanaapis.scraping import constants, functions
 
 
 @return_if_first_empty(OrderedSet)
 def find_ids(text: str | list[str]) -> OrderedSet[str]:
     if isinstance(text, list):
         text = ''.join(text)
-    return OrderedSet(re.findall(r'atus/(\d+)', text))
+    return OrderedSet(re.findall('atus/(\d+)', text))
 
 
 async def get_medias(ids: Iterable[str], audio_only=False) -> OrderedSet[Media]:
     ids = OrderedSet(ids)
 
     medias: OrderedSet[Media] = OrderedSet()
 
-    while referenced_ids := find_ids(await get_referenced_tweet_urls(ids)) - ids:
-        ids |= referenced_ids
+    # Paid Twitter API v2
+    # while referenced_ids := find_ids(await get_referenced_tweet_urls(ids)) - ids:
+    #     ids |= referenced_ids
     if not ids:
         return medias
 
     try:
         tweets_data = await get_tweet_data(constants.TWITTER_ENDPOINT_V1, params={'id': ','.join(ids), 'tweet_mode': 'extended'})
     except aiohttp.ClientError:
         tweets_data = []
```

### Comparing `flanaapis-1.6.0/flanaapis/scraping/yt_dlp_wrapper.py` & `flanaapis-1.6.1/flanaapis/scraping/yt_dlp_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     url: str,
     preferred_video_codec: str = None,
     preferred_extension: str = None,
     force=False,
     audio_only=False,
     timeout: int | float = None
 ) -> Media | None:
+    url = await flanautils.resolve_real_url(url)
+
     output_file_stem = str(uuid.uuid1())
 
     options = {
         "outtmpl": f'{output_file_stem}.%(ext)s',
         'logtostderr': True,
         'noplaylist': True,
         'extract_flat': 'in_playlist'
@@ -63,55 +65,63 @@
                     path.unlink()
                 except PermissionError:
                     await asyncio.sleep(1)
                 else:
                     break
         return
 
-    output_file_path = next(flanautils.find_paths_by_stem(output_file_stem, lazy=True))
+    try:
+        output_file_path = next(flanautils.find_paths_by_stem(output_file_stem, lazy=True))
+    except StopIteration:
+        return
+
     bytes_ = output_file_path.read_bytes()
 
     if (
             not (extension := output_file_path.suffix.strip('.'))
             and
             not (extension := media_info.get('final_extension'))
             and
             (output_file_name := media_info.get('output_file_name'))
     ):
         extension = pathlib.Path(output_file_name).suffix.strip('.')
 
-    type_ = None
-    source = None
     extractor_key = media_info.get('extractor_key', '')
-    try:
-        source = Source[extractor_key.upper()]
-    except (AttributeError, KeyError):
-        if 'generic' == extractor_key.lower():
-            bytes_format = await flanautils.get_format(bytes_)
-            if any(format_ in bytes_format for format_ in ('jfif', 'jpeg', 'jpg', 'png', 'tiff')):
-                type_ = MediaType.IMAGE
-            elif 'gif' in bytes_format:
-                type_ = MediaType.GIF
-            elif any(format_ in bytes_format for format_ in ('avchd', 'avi', 'flv', 'mkv', 'mov', 'mp4', 'webm', 'wmv')):
-                type_ = MediaType.VIDEO
-            elif any(format_ in bytes_format for format_ in ('aac', 'flac', 'm4a', 'mp3', 'wav')):
-                type_ = MediaType.AUDIO
+    if 'generic' == extractor_key.lower():
+        bytes_format = await flanautils.get_format(bytes_)
+        if any(format_ in bytes_format for format_ in ('jfif', 'jpeg', 'jpg', 'png', 'tiff')):
+            type_ = MediaType.IMAGE
+        elif 'gif' in bytes_format:
+            type_ = MediaType.GIF
+        elif any(format_ in bytes_format for format_ in ('avchd', 'avi', 'flv', 'mkv', 'mov', 'mp4', 'webm', 'wmv')):
+            type_ = MediaType.VIDEO
+        elif any(format_ in bytes_format for format_ in ('aac', 'flac', 'm4a', 'mp3', 'wav')):
+            type_ = MediaType.AUDIO
+        else:
+            type_ = None
 
-            if domains := flanautils.find_url_domains(url):
-                source = domains[0]
+        if domains := flanautils.find_url_domains(url):
+            source = domains[0]
+        else:
+            source = None
     else:
         if audio_only:
             type_ = MediaType.AUDIO
         elif extension == 'gif':
             type_ = MediaType.GIF
         else:
             type_ = MediaType.VIDEO
 
+        try:
+            source = Source[extractor_key.upper()]
+        except (AttributeError, KeyError):
+            source = extractor_key
+
     if title := media_info.get('title'):
-        title = title[:constants.YT_DLP_WRAPPER_TITLE_MAX_LENGTH]
+        title = title[:constants.YT_DLP_WRAPPER_TITLE_MAX_LENGTH].strip()
         try:
             bytes_ = await flanautils.edit_metadata(output_file_path, {'title': title}, overwrite=False)
         except FileNotFoundError:
             pass
 
     output_file_path.unlink(missing_ok=True)
```

### Comparing `flanaapis-1.6.0/flanaapis/weather/functions.py` & `flanaapis-1.6.1/flanaapis/weather/functions.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/weather/google.py` & `flanaapis-1.6.1/flanaapis/weather/google.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/weather/models.py` & `flanaapis-1.6.1/flanaapis/weather/models.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/weather/open_weather_map.py` & `flanaapis-1.6.1/flanaapis/weather/open_weather_map.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/weather/routes.py` & `flanaapis-1.6.1/flanaapis/weather/routes.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis/weather/visual_crossing.py` & `flanaapis-1.6.1/flanaapis/weather/visual_crossing.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/flanaapis.egg-info/PKG-INFO` & `flanaapis-1.6.1/flanaapis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: flanaapis
-Version: 1.6.0
+Version: 1.6.1
 Summary: Set of functions that can be used as an imported library or as an api rest running the main.py. There is currently an instance of the api running at https://flanaserver.ddns.net/flanaapis.
 Home-page: https://github.com/AlberLC/flanaapis
 Author: AlberLC
-Author-email: alberlc@outlook.com
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanaapis/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `flanaapis-1.6.0/flanaapis.egg-info/SOURCES.txt` & `flanaapis-1.6.1/flanaapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.0/setup.cfg` & `flanaapis-1.6.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [metadata]
 name = flanaapis
-version = v1.6.0
+version = v1.6.1
 author = AlberLC
-author_email = alberlc@outlook.com
 description = Set of functions that can be used as an imported library or as an api rest running the main.py. There is currently an instance of the api running at https://flanaserver.ddns.net/flanaapis.
 long_description = file: README.rst
 url = https://github.com/AlberLC/flanaapis
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/flanaapis/issues
 classifiers = 
 	Programming Language :: Python :: 3.10
```

