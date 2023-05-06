# Comparing `tmp/IMDbTraktSyncer-1.0.7.tar.gz` & `tmp/IMDbTraktSyncer-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.0.7.tar", last modified: Sat May  6 04:34:15 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.0.8.tar", last modified: Sat May  6 04:57:14 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.0.7.tar` & `IMDbTraktSyncer-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 04:34:15.637039 IMDbTraktSyncer-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-05-06 04:34:15.606579 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0     7736 2023-05-06 03:40:14.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 01:55:31.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      642 2023-05-05 01:55:31.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     2038 2023-05-06 03:24:18.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1408 2023-05-06 03:16:22.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2516 2023-05-06 04:33:00.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-06 04:34:15.634553 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     5945 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     5945 2023-05-06 04:34:15.636041 IMDbTraktSyncer-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5335 2023-05-06 04:29:30.000000 IMDbTraktSyncer-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 04:34:15.637539 IMDbTraktSyncer-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-05-06 03:46:33.000000 IMDbTraktSyncer-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:57:14.858586 IMDbTraktSyncer-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-06 04:57:14.838585 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0     7796 2023-05-06 04:53:07.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 01:55:31.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      642 2023-05-05 01:55:31.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     2038 2023-05-06 03:24:18.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1408 2023-05-06 03:16:22.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2516 2023-05-06 04:33:00.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:57:14.856089 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     5945 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5945 2023-05-06 04:57:14.858087 IMDbTraktSyncer-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5335 2023-05-06 04:29:30.000000 IMDbTraktSyncer-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 04:57:14.859085 IMDbTraktSyncer-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-05-06 04:56:52.000000 IMDbTraktSyncer-1.0.8/setup.py
```

### Comparing `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     
     #Start web driver
     print('Starting webdriver')
     options = Options()
     options.add_argument("--headless=new")
     options.add_argument('--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3')
     options.add_experimental_option("prefs", {"download.default_directory": directory, "download.directory_upgrade": True, "download.prompt_for_download": False})
+    options.add_argument("--disable-save-password-bubble")
     options.add_argument('--disable-notifications')
     options.add_argument("--disable-third-party-cookies")
     options.add_argument("--disable-dev-shm-usage")
     options.add_argument("--no-sandbox")
     options.add_argument("--disable-extensions")
     options.add_experimental_option("excludeSwitches", ["enable-automation"])
     options.add_experimental_option("useAutomationExtension", False)
```

### Comparing `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/imdbRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.7
+Version: 1.0.8
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.0.7/LICENSE` & `IMDbTraktSyncer-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.7/PKG-INFO` & `IMDbTraktSyncer-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.7
+Version: 1.0.8
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.0.7/README.md` & `IMDbTraktSyncer-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.7/setup.py` & `IMDbTraktSyncer-1.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 DESCRIPTION = 'This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

