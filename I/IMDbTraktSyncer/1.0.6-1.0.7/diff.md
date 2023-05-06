# Comparing `tmp/IMDbTraktSyncer-1.0.6.tar.gz` & `tmp/IMDbTraktSyncer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.0.6.tar", last modified: Fri May  5 01:46:54 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.0.7.tar", last modified: Sat May  6 04:34:15 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.0.6.tar` & `IMDbTraktSyncer-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 01:46:54.870618 IMDbTraktSyncer-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-05 01:46:54.835159 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0     6906 2023-05-05 01:45:00.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 01:37:55.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      642 2023-04-30 07:12:26.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3596 2023-05-05 01:45:38.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1401 2023-05-05 01:41:48.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2094 2023-05-05 01:34:29.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-05 01:46:54.868115 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     5945 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     5945 2023-05-05 01:46:54.870114 IMDbTraktSyncer-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5335 2023-05-05 01:46:16.000000 IMDbTraktSyncer-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 01:46:54.871111 IMDbTraktSyncer-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-05-05 01:40:55.000000 IMDbTraktSyncer-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:34:15.637039 IMDbTraktSyncer-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-06 04:34:15.606579 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0     7736 2023-05-06 03:40:14.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 01:55:31.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      642 2023-05-05 01:55:31.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     2038 2023-05-06 03:24:18.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1408 2023-05-06 03:16:22.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2516 2023-05-06 04:33:00.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:34:15.634553 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     5945 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 04:34:15.000000 IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5945 2023-05-06 04:34:15.636041 IMDbTraktSyncer-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5335 2023-05-06 04:29:30.000000 IMDbTraktSyncer-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 04:34:15.637539 IMDbTraktSyncer-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-05-06 03:46:33.000000 IMDbTraktSyncer-1.0.7/setup.py
```

### Comparing `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,31 @@
 
     #Get credentials
     trakt_client_id = verifyCredentials.trakt_client_id
     trakt_client_secret = verifyCredentials.trakt_client_secret
     trakt_access_token = verifyCredentials.trakt_access_token
     imdb_username = verifyCredentials.imdb_username
     imdb_password = verifyCredentials.imdb_password
-
+    
+    directory = os.path.dirname(os.path.realpath(__file__))
+    
     #Start web driver
+    print('Starting webdriver')
     options = Options()
     options.add_argument("--headless=new")
-    options.add_argument('--disable-notifications')
     options.add_argument('--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3')
+    options.add_experimental_option("prefs", {"download.default_directory": directory, "download.directory_upgrade": True, "download.prompt_for_download": False})
+    options.add_argument('--disable-notifications')
+    options.add_argument("--disable-third-party-cookies")
+    options.add_argument("--disable-dev-shm-usage")
+    options.add_argument("--no-sandbox")
+    options.add_argument("--disable-extensions")
+    options.add_experimental_option("excludeSwitches", ["enable-automation"])
+    options.add_experimental_option("useAutomationExtension", False)
+    options.add_argument('--log-level=3')
 
     service = Service(executable_path=binary_path)
     driver = webdriver.Chrome(service=service, options=options)
 
     wait = WebDriverWait(driver, 20)
 
     driver.get('https://www.imdb.com/registration/signin')
@@ -67,20 +78,23 @@
 
     # Check if signed in
     element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".nav__userMenu.navbar__user")))
     if "Sign In" in element.text:
         print("Not signed in")
     else:
         print("Signed in")
-        
+    
+    trakt_ratings = traktRatings.getTraktRatings(trakt_client_id, trakt_access_token)
+    imdb_ratings = imdbRatings.getImdbRatings(imdb_username, imdb_password, driver, directory, wait)
+    
     print('Setting IMDB Ratings')
         
     #Get trakt and imdb ratings and filter out trakt ratings wish missing imbd id
-    trakt_ratings = [rating for rating in traktRatings.trakt_ratings if rating['ID'] is not None]
-    imdb_ratings = [rating for rating in imdbRatings.imdb_ratings if rating['ID'] is not None]
+    trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None]
+    imdb_ratings = [rating for rating in imdb_ratings if rating['ID'] is not None]
     #Filter out ratings already set
     imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [imdb_rating['ID'] for imdb_rating in imdb_ratings]]
     trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
 
     # loop through each movie and TV show rating and submit rating on IMDb website
     for i, item in enumerate(imdb_ratings_to_set, 1):
         print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]} ({item["Year"]}): {item["Rating"]}/10 on IMDb')
```

### Comparing `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.0.7/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.6
+Version: 1.0.7
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.0.6/LICENSE` & `IMDbTraktSyncer-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.6/PKG-INFO` & `IMDbTraktSyncer-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.6
+Version: 1.0.7
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.0.6/README.md` & `IMDbTraktSyncer-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.6/setup.py` & `IMDbTraktSyncer-1.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 DESCRIPTION = 'This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

