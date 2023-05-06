# Comparing `tmp/ntscraper-0.1.2.tar.gz` & `tmp/ntscraper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntscraper-0.1.2.tar", last modified: Wed Feb  1 20:52:01 2023, max compression
+gzip compressed data, was "ntscraper-0.1.3.tar", last modified: Sat May  6 07:28:01 2023, max compression
```

## Comparing `ntscraper-0.1.2.tar` & `ntscraper-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 20:52:01.275220 ntscraper-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3225 2023-02-01 20:52:01.275220 ntscraper-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2299 2023-02-01 20:47:38.000000 ntscraper-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-01 20:52:01.216499 ntscraper-0.1.2/ntscraper/
--rw-rw-rw-   0        0        0       26 2023-01-31 13:55:18.000000 ntscraper-0.1.2/ntscraper/__init__.py
--rw-rw-rw-   0        0        0    27015 2023-02-01 20:46:45.000000 ntscraper-0.1.2/ntscraper/nitter.py
-drwxrwxrwx   0        0        0        0 2023-02-01 20:52:01.267213 ntscraper-0.1.2/ntscraper.egg-info/
--rw-rw-rw-   0        0        0     3225 2023-02-01 20:52:00.000000 ntscraper-0.1.2/ntscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-02-01 20:52:00.000000 ntscraper-0.1.2/ntscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 20:52:00.000000 ntscraper-0.1.2/ntscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-02-01 20:52:00.000000 ntscraper-0.1.2/ntscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-01 20:52:00.000000 ntscraper-0.1.2/ntscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-01 20:52:01.275220 ntscraper-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-02-01 20:51:23.000000 ntscraper-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:28:01.262889 ntscraper-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3485 2023-05-06 07:28:01.262889 ntscraper-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2559 2023-05-06 07:24:10.000000 ntscraper-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 07:28:01.230866 ntscraper-0.1.3/ntscraper/
+-rw-rw-rw-   0        0        0       26 2023-01-31 13:55:18.000000 ntscraper-0.1.3/ntscraper/__init__.py
+-rw-rw-rw-   0        0        0    27229 2023-05-06 07:24:10.000000 ntscraper-0.1.3/ntscraper/nitter.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:28:01.258874 ntscraper-0.1.3/ntscraper.egg-info/
+-rw-rw-rw-   0        0        0     3485 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 07:28:01.000000 ntscraper-0.1.3/ntscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:28:01.262889 ntscraper-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-05-06 07:24:10.000000 ntscraper-0.1.3/setup.py
```

### Comparing `ntscraper-0.1.2/LICENSE.txt` & `ntscraper-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ntscraper-0.1.2/PKG-INFO` & `ntscraper-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
@@ -45,20 +45,20 @@
 ## How to use
 
 First, initialize the library:
 
 ```
 from ntscraper import Nitter
 
-scraper = Nitter(log_level=None)
+scraper = Nitter(log_level=1)
 ```
 The valid logging levels are:
 - None = no logs
-- 1 = informational logs (default)
-- 2 = informational, warning and error logs
+- 0 = only warning and error logs
+- 1 = previous + informational logs (default)
 
 Then, choose the proper function for what you want to do from the following.
 
 ### Scrape tweets
 
 ```
 github_hash_tweets = scraper.get_tweets("github", mode='hashtag')
@@ -94,10 +94,14 @@
 
 ```
 random_instance = scraper.get_random_instance()
 ```
 
 Returns a random Nitter instance.
 
+## Note
+
+Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
+
 ## To do list
 
 - [ ] Add scraping of posts and comments
```

### Comparing `ntscraper-0.1.2/README.md` & `ntscraper-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 ## How to use
 
 First, initialize the library:
 
 ```
 from ntscraper import Nitter
 
-scraper = Nitter(log_level=None)
+scraper = Nitter(log_level=1)
 ```
 The valid logging levels are:
 - None = no logs
-- 1 = informational logs (default)
-- 2 = informational, warning and error logs
+- 0 = only warning and error logs
+- 1 = previous + informational logs (default)
 
 Then, choose the proper function for what you want to do from the following.
 
 ### Scrape tweets
 
 ```
 github_hash_tweets = scraper.get_tweets("github", mode='hashtag')
@@ -72,10 +72,14 @@
 
 ```
 random_instance = scraper.get_random_instance()
 ```
 
 Returns a random Nitter instance.
 
+## Note
+
+Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
+
 ## To do list
 
 - [ ] Add scraping of posts and comments
```

### Comparing `ntscraper-0.1.2/ntscraper/nitter.py` & `ntscraper-0.1.3/ntscraper/nitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
         self.instances = self.__get_instances()
         self.r = requests.Session()
         self.r.headers.update(
             {
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:108.0) Gecko/20100101 Firefox/108.0"
             }
         )
-        if log_level == 1:
-            log_level = logging.INFO
-        elif log_level == 2:
+        if log_level == 0:
             log_level = logging.WARNING
+        elif log_level == 1:
+            log_level = logging.INFO
         elif log_level:
             raise ValueError("Invalid log level")
         
         logging.basicConfig(level=log_level, format='%(asctime)s - %(message)s', datefmt='%d-%b-%y %H:%M:%S')
 
     def __is_instance_encrypted(self, instance):
         """
@@ -117,15 +117,15 @@
             else:
                 logging.warning(f"Error fetching {instance}, trying another random instance")
                 instance = self.get_random_instance()
                 count += 1
             sleep(1)
 
         if count >= max_retries:
-            logging.info("Max retries reached. Check your request and try again.")
+            logging.warning("Max retries reached. Check your request and try again.")
             return None, None
 
         return instance, soup
 
     def __get_quoted_media(self, quoted_tweet, is_encrypted):
         """
         Extract media from a quoted tweet
@@ -311,15 +311,15 @@
         Extract date from a tweet
 
         :param tweet: tweet to extract date from
         :return: date of tweet
         """
         return (
             tweet.find("span", class_="tweet-date")
-            .find("a")["href"]
+            .find("a")["title"]
             .split("/")[-1]
             .split("#")[0]
         )
 
     def __get_tweet_text(self, tweet):
         """
         Extract text from a tweet
@@ -376,14 +376,17 @@
             tweet.find("div", class_="quote")
             if tweet.find("div", class_="quote")
             else None
         )
 
         # Extract media from the quoted tweet
         if quoted_tweet:
+            deleted = False
+            if quoted_tweet["class"] == ["quote", "unavailable"]:
+                deleted = True
             (
                 quoted_pictures,
                 quoted_videos,
                 quoted_gifs,
             ) = self.__get_quoted_media(quoted_tweet, is_encrypted)
 
         # Extract media from the tweet
@@ -394,18 +397,18 @@
             "text": self.__get_tweet_text(tweet),
             "user": self.__get_user(tweet, is_encrypted),
             "date": self.__get_tweet_date(tweet),
             "is-retweet": tweet.find("div", class_="retweet-header")
             is not None,
             "external-link": self.__get_external_link(tweet),
             "quoted-post": {
-                "link": self.__get_tweet_link(quoted_tweet),
-                "text": self.__get_tweet_text(quoted_tweet),
-                "user": self.__get_user(quoted_tweet, is_encrypted),
-                "date": self.__get_tweet_date(quoted_tweet),
+                "link": self.__get_tweet_link(quoted_tweet) if not deleted else "",
+                "text": self.__get_tweet_text(quoted_tweet) if not deleted else "",
+                "user": self.__get_user(quoted_tweet, is_encrypted) if not deleted else {},
+                "date": self.__get_tweet_date(quoted_tweet) if not deleted else "",
                 "pictures": quoted_pictures,
                 "videos": quoted_videos,
                 "gifs": quoted_gifs,
             }
             if quoted_tweet
             else {},
             "stats": self.__get_tweet_stats(tweet),
@@ -505,14 +508,15 @@
                             thread.append(to_append)
                             already_scraped.add(self.__get_tweet_link(tweet))
 
                         if len(tweet["class"]) == 3:
                             tweets["threads"].append(thread)
                             thread = []
 
+            logging.info(f"Current stats: {len(tweets['tweets'])} tweets, {len(tweets['threads'])} threads...")
             if not(since and until) and not(since) and len(tweets["tweets"]) + len(tweets["threads"]) >= number:
                 keep_scraping = False
             else:
                 sleep(uniform(1, 2))
 
                 # Go to the next page
                 show_more_buttons = soup.find_all("div", class_="show-more")
@@ -540,16 +544,14 @@
                             ]
                         )
                     instance, soup = self.__get_page(next_page, instance, max_retries)
                     if instance is None or soup is None:
                         keep_scraping = False
                 else:
                     keep_scraping = False
-            
-            logging.info(f"Total tweets: {len(tweets['tweets'])}; Total threads: {len(tweets['threads'])}")
         return tweets
 
     def get_random_instance(self):
         """
         Get a random Nitter instance
 
         :return: URL of random Nitter instance
```

### Comparing `ntscraper-0.1.2/ntscraper.egg-info/PKG-INFO` & `ntscraper-0.1.3/ntscraper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
@@ -45,20 +45,20 @@
 ## How to use
 
 First, initialize the library:
 
 ```
 from ntscraper import Nitter
 
-scraper = Nitter(log_level=None)
+scraper = Nitter(log_level=1)
 ```
 The valid logging levels are:
 - None = no logs
-- 1 = informational logs (default)
-- 2 = informational, warning and error logs
+- 0 = only warning and error logs
+- 1 = previous + informational logs (default)
 
 Then, choose the proper function for what you want to do from the following.
 
 ### Scrape tweets
 
 ```
 github_hash_tweets = scraper.get_tweets("github", mode='hashtag')
@@ -94,10 +94,14 @@
 
 ```
 random_instance = scraper.get_random_instance()
 ```
 
 Returns a random Nitter instance.
 
+## Note
+
+Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
+
 ## To do list
 
 - [ ] Add scraping of posts and comments
```

### Comparing `ntscraper-0.1.2/setup.py` & `ntscraper-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ntscraper",
-    version="0.1.2",
+    version="0.1.3",
     description="Unofficial library to scrape Twitter profiles and posts from Nitter instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Homepage': 'https://github.com/bocchilorenzo/ntscraper',
         'Source': 'https://github.com/bocchilorenzo/ntscraper',
         'Documentation': 'https://github.com/bocchilorenzo/ntscraper'
```

