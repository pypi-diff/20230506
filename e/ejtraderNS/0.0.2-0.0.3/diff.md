# Comparing `tmp/ejtraderNS-0.0.2.tar.gz` & `tmp/ejtraderNS-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderNS-0.0.2.tar", last modified: Fri May  5 21:45:56 2023, max compression
+gzip compressed data, was "ejtraderNS-0.0.3.tar", last modified: Sat May  6 16:01:03 2023, max compression
```

## Comparing `ejtraderNS-0.0.2.tar` & `ejtraderNS-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:45:56.801326 ejtraderNS-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 21:45:43.000000 ejtraderNS-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 21:45:43.000000 ejtraderNS-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-05-05 21:45:56.801326 ejtraderNS-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-05-05 21:45:43.000000 ejtraderNS-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:45:56.801326 ejtraderNS-0.0.2/ejtraderNS/
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-05-05 21:45:43.000000 ejtraderNS-0.0.2/ejtraderNS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:45:56.801326 ejtraderNS-0.0.2/ejtraderNS/data/
--rw-r--r--   0 runner    (1001) docker     (123)   536576 2023-05-05 21:45:43.000000 ejtraderNS-0.0.2/ejtraderNS/data/rss.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:45:56.801326 ejtraderNS-0.0.2/ejtraderNS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-05-05 21:45:56.000000 ejtraderNS-0.0.2/ejtraderNS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-05 21:45:56.000000 ejtraderNS-0.0.2/ejtraderNS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:45:56.000000 ejtraderNS-0.0.2/ejtraderNS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-05 21:45:56.000000 ejtraderNS-0.0.2/ejtraderNS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 21:45:56.000000 ejtraderNS-0.0.2/ejtraderNS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 21:45:43.000000 ejtraderNS-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 21:45:56.801326 ejtraderNS-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-05 21:45:43.000000 ejtraderNS-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:01:03.457442 ejtraderNS-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-06 16:00:46.000000 ejtraderNS-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-06 16:00:46.000000 ejtraderNS-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-06 16:01:03.457442 ejtraderNS-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-06 16:00:46.000000 ejtraderNS-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:01:03.453442 ejtraderNS-0.0.3/ejtraderNS/
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-05-06 16:00:46.000000 ejtraderNS-0.0.3/ejtraderNS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:01:03.457442 ejtraderNS-0.0.3/ejtraderNS/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   536576 2023-05-06 16:00:46.000000 ejtraderNS-0.0.3/ejtraderNS/data/rss.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:01:03.457442 ejtraderNS-0.0.3/ejtraderNS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-05-06 16:01:03.000000 ejtraderNS-0.0.3/ejtraderNS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-06 16:01:03.000000 ejtraderNS-0.0.3/ejtraderNS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:01:03.000000 ejtraderNS-0.0.3/ejtraderNS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-06 16:01:03.000000 ejtraderNS-0.0.3/ejtraderNS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 16:01:03.000000 ejtraderNS-0.0.3/ejtraderNS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-06 16:00:46.000000 ejtraderNS-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 16:01:03.457442 ejtraderNS-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-06 16:00:46.000000 ejtraderNS-0.0.3/setup.py
```

### Comparing `ejtraderNS-0.0.2/LICENSE` & `ejtraderNS-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderNS-0.0.2/PKG-INFO` & `ejtraderNS-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderNS
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a News Library.
 Home-page: https://ejtraderNS.readthedocs.io/
 Download-URL: https://github.com/ejtraderlabs/ejtraderNS
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/ejtraderLabs/ejtraderNS/issues
@@ -67,102 +67,86 @@
 ```python
 api = ejtraderNS(website = 'nytimes.com', topic = 'politics')
 
 results = api.get_news()
 articles = results['articles']
 ```
 
-There is a limited set of topic that you might find:
+Some websites support multiple countries, such as  [investing.com](https://www.investing.com) or [tradingeconomics.com](https://www.tradingeconomics.com)
 
-``` 'tech', 'news', 'business', 'science', 'finance', 'food', 'politics', 'economics', 'travel', 'entertainment', 'music', 'sport', 'world' ```
+
+In this example, I will demonstrate a website that supports multiple countries,
+ retrieve multiple topics, and convert the data into a pandas dataframe.
 
 
-### some url supports multiple languages
 ```python
 import pandas as pd
-from ejtraderNS import Client, describe_url
+from ejtraderNS import Client
 from datetime import datetime
 
-country_topic = describe_url('investing.com')
-
-# Criando uma lista vazia para armazenar os DataFrames
+url = 'investing.com' # or tradingeconomics.com
+country = 'GB'
+country_topic = ["finance","news","economics"]
 dfs = []
 
-# Iterando pelos países, idiomas e tópicos
-
-    
-for topic in country_topic['topics']:
-    try:
-        api = Client(website="investing.com", topic=topic, country="BR")
-    except:
-        pass
+for topic in country_topic:
+    api = Client(website=url, topic=topic, country=country)
+    getdata = api.get_news()
     print(f"topic: {topic}")
-    
-    try:
-        getdata = api.get_news()
-    except:
-        pass
-    # Coletando os dados
-    
 
-    # Se getdata for None, pule para o próximo tópico
     if getdata is None:
         continue
 
-    # Criando uma lista vazia para armazenar as informações
     data = []
 
-    # Iterando pelos artigos e extraindo as informações relevantes
     for article in getdata['articles']:
-        article_data = {}
-        article_data['topic'] = getdata['topic']
-        article_data['author'] = article['author']
-        article_data['date'] = article['published_parsed'] if article['published_parsed'] else article['published']
-
-        article_data['country'] = getdata['country']
-        article_data['language'] = getdata['language']
-
-        article_data['title'] = article['title']
-        
-        try:
-            article_data['summary'] = article['summary']
-            article_data['url'] = article['link']
-        except:
-            article_data['url'] = None
-            article_data['summary'] = article['title']
-            pass
-        
+        article_data = {
+            'topic': getdata['topic'],
+            'author': article['author'],
+            'date': article['published_parsed'] if article['published_parsed'] else article['published'],
+            'country': getdata['country'],
+            'language': getdata['language'],
+            'title': article['title'],
+            'summary': article.get('summary', article['title'])
+        }
         data.append(article_data)
 
-    # Converter objetos time.struct_time para objetos datetime
-    for item in data:
-        try:
-            item['date'] = datetime(*item['date'][:6])
-        except:
-            pass
-    # Criando o dataframe com as informações extraídas
     df = pd.DataFrame(data)
-    df['date'] = pd.to_datetime(df['date'], utc=True)
-    df.set_index('date', inplace=True)
 
-    # Adicionando o DataFrame atual à lista de DataFrames
+    df['date'] = pd.to_datetime(df['date'].apply(lambda x: datetime(*x[:6]) if isinstance(x, tuple) else x), utc=True, errors='coerce')
+    df.set_index('date', inplace=True)
     dfs.append(df)
 
-# Concatenando todos os DataFrames na lista dfs
 df = pd.concat(dfs)
-
-# Reordenando o índice
 df.sort_index(inplace=True)
 print(df)
 
 ```
+output example:
+
+| topic     | author        | country   | language   | title                                                                            | summary                                                                          |
+|:----------|:--------------|:----------|:-----------|:---------------------------------------------------------------------------------|:---------------------------------------------------------------------------------|
+| finance   | Reuters       | GB        | en         | Italy pushes to limit executive pay in listed state-run firms                    | Italy pushes to limit executive pay in listed state-run firms                    |
+| economics | Reuters       | GB        | en         | UK's Cleverly raises Xinjiang and Taiwan with Chinese vice president             | UK's Cleverly raises Xinjiang and Taiwan with Chinese vice president             |
+| news      | Reuters       | GB        | en         | Ukraine hails return of 45 Azov fighters, Russia says 3 pilots released          | Ukraine hails return of 45 Azov fighters, Russia says 3 pilots released          |
+
+
+
+
+
+There is a limited set of topic that you might find:
+``` 'tech', 'news', 'business', 'science', 'finance', 'food', 'politics', 'economics', 'travel', 'entertainment', 'music', 'sport', 'world' ```
+
+extras topics only for [investing.com](https://www.investing.com)
+
+``` 'crypto', 'forex', 'stock', 'commodities', 'central_bank', 'forex_analysis', 'forex_technical', 'forex_fundamental', 'forex_opinion', 'forex_signal', 'bonds_analysis', 'bonds_technical', 'bonds_fundamental', 'bonds_opinion', 'bonds_strategy', 'bonds_government', 'bonds_corporate', 'stock_analysis', 'stock_technical', 'stock_fundamental', 'stock_opinion', 'stock_picks', 'indices_analysis', 'futures_analysis', 'options_analysis', 'commodities_analysis', 'commodities_technical', 'commodities_Fundamental', 'commodities_opinion', 'commodities_strategy', 'commodities_metals', 'commodities_energy', 'commodities_agriculture', 'overview_analysis', 'overview_technical', 'overview_fundamental', 'overview_opinion', 'overview_investing', 'crypto_opinion'```
+  
+
 
-for investing.com  is a limited set of topic base on country 
 
-``` 'news', 'crypto_news', 'forex_news', 'popular_news', 'commodities_news', 'stock_news', 'economic_indicators_news', 'economy_news', 'central_bank', 'crypto_opinion', 'forex_analysis', 'forex_technical', 'forex_fundamental', 'forex_opinion', 'forex_signal', 'overview_analysis', 'overview_technical', 'overview_fundamental', 'overview_opinion', 'overview_investing', 'commodities_analysis', 'commodities_technical', 'commodities_Fundamental', 'commodities_opinion', 'commodities_strategy', 'commodities_metals', 'commodities_energy', 'commodities_agriculture', 'bonds_analysis', 'bonds_technical', 'bonds_fundamental', 'bonds_opinion', 'bonds_trategy', 'bonds_government', 'bonds_corporate', 'stock_analysis', 'stock_technical', 'stock_fundamental', 'stock_opinion', 'stock_picks', 'stock', 'indices', 'futures', 'options', 'politics_news', 'world_news' ```
 
 However, not all topics are supported by every newspaper.
 
 How to check which topics are supported by which newspaper:
 ```python
 from ejtraderNS import describe_url
 
@@ -274,31 +258,17 @@
 `US`, `GB`, `DE`, `FR`, `IN`, `RU`, `ES`, `BR`, `IT`, `CA`, `AU`, `NL`, `PL`, `NZ`, `PT`, `RO`, `UA`, `JP`, `AR`, `IR`, `IE`, `PH`, `IS`, `ZA`, `AT`, `CL`, `HR`, `BG`, `HU`, `KR`, `SZ`, `AE`, `EG`, `VE`, `CO`, `SE`, `CZ`, `ZH`, `MT`, `AZ`, `GR`, `BE`, `LU`, `IL`, `LT`, `NI`, `MY`, `TR`, `BM`, `NO`, `ME`, `SA`, `RS`, `BA`
 
 Supported languages:
 `EL`, `IT`, `ZH`, `EN`, `RU`, `CS`, `RO`, `FR`, `JA`, `DE`, `PT`, `ES`, `AR`, `HE`, `UK`, `PL`, `NL`, `TR`, `VI`, `KO`, `TH`, `ID`, `HR`, `DA`, `BG`, `NO`, `SK`, `FA`, `ET`, `SV`, `BN`, `GU`, `MK`, `PA`, `HU`, `SL`, `FI`, `LT`, `MR`, `HI`
 
 
 
-
-
 ## Tech/framework used
 The package itself is nothing more than a SQLite database with 
 RSS feed endpoints for each website and some basic wrapper of
 [feedparser](https://pythonhosted.org/feedparser/index.html).
 
 
-## About Us
-We are ejtraderNS API team. We are glad that you liked our package.
-
-If you want to search for any news data, consider using [our API](https://ejtraderNSapi.com/)
-
-![](ejtraderNS_oneliner.png)
-
-
-[Artem Bugara]() - co-founder of ejtraderNS, made v.0.1.0
-
-[Maksym Sugonyaka](https://www.linkedin.com/mwlite/in/msugonyaka) - co-founder of ejtraderNS, made v.0.1.0
+## Acknowledgements
 
-[Becket Trotter](https://www.linkedin.com/in/beckettrotter/) - Python Developer, made v.0.2.0
+I would like to express my gratitude to [@kotartemiy](https://github.com/kotartemiy) for creating the initial project. Their work has been an invaluable starting point for my modifications and improvements.
 
-## Licence
-MIT
```

### Comparing `ejtraderNS-0.0.2/README.md` & `ejtraderNS-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -40,102 +40,86 @@
 ```python
 api = ejtraderNS(website = 'nytimes.com', topic = 'politics')
 
 results = api.get_news()
 articles = results['articles']
 ```
 
-There is a limited set of topic that you might find:
+Some websites support multiple countries, such as  [investing.com](https://www.investing.com) or [tradingeconomics.com](https://www.tradingeconomics.com)
 
-``` 'tech', 'news', 'business', 'science', 'finance', 'food', 'politics', 'economics', 'travel', 'entertainment', 'music', 'sport', 'world' ```
+
+In this example, I will demonstrate a website that supports multiple countries,
+ retrieve multiple topics, and convert the data into a pandas dataframe.
 
 
-### some url supports multiple languages
 ```python
 import pandas as pd
-from ejtraderNS import Client, describe_url
+from ejtraderNS import Client
 from datetime import datetime
 
-country_topic = describe_url('investing.com')
-
-# Criando uma lista vazia para armazenar os DataFrames
+url = 'investing.com' # or tradingeconomics.com
+country = 'GB'
+country_topic = ["finance","news","economics"]
 dfs = []
 
-# Iterando pelos países, idiomas e tópicos
-
-    
-for topic in country_topic['topics']:
-    try:
-        api = Client(website="investing.com", topic=topic, country="BR")
-    except:
-        pass
+for topic in country_topic:
+    api = Client(website=url, topic=topic, country=country)
+    getdata = api.get_news()
     print(f"topic: {topic}")
-    
-    try:
-        getdata = api.get_news()
-    except:
-        pass
-    # Coletando os dados
-    
 
-    # Se getdata for None, pule para o próximo tópico
     if getdata is None:
         continue
 
-    # Criando uma lista vazia para armazenar as informações
     data = []
 
-    # Iterando pelos artigos e extraindo as informações relevantes
     for article in getdata['articles']:
-        article_data = {}
-        article_data['topic'] = getdata['topic']
-        article_data['author'] = article['author']
-        article_data['date'] = article['published_parsed'] if article['published_parsed'] else article['published']
-
-        article_data['country'] = getdata['country']
-        article_data['language'] = getdata['language']
-
-        article_data['title'] = article['title']
-        
-        try:
-            article_data['summary'] = article['summary']
-            article_data['url'] = article['link']
-        except:
-            article_data['url'] = None
-            article_data['summary'] = article['title']
-            pass
-        
+        article_data = {
+            'topic': getdata['topic'],
+            'author': article['author'],
+            'date': article['published_parsed'] if article['published_parsed'] else article['published'],
+            'country': getdata['country'],
+            'language': getdata['language'],
+            'title': article['title'],
+            'summary': article.get('summary', article['title'])
+        }
         data.append(article_data)
 
-    # Converter objetos time.struct_time para objetos datetime
-    for item in data:
-        try:
-            item['date'] = datetime(*item['date'][:6])
-        except:
-            pass
-    # Criando o dataframe com as informações extraídas
     df = pd.DataFrame(data)
-    df['date'] = pd.to_datetime(df['date'], utc=True)
-    df.set_index('date', inplace=True)
 
-    # Adicionando o DataFrame atual à lista de DataFrames
+    df['date'] = pd.to_datetime(df['date'].apply(lambda x: datetime(*x[:6]) if isinstance(x, tuple) else x), utc=True, errors='coerce')
+    df.set_index('date', inplace=True)
     dfs.append(df)
 
-# Concatenando todos os DataFrames na lista dfs
 df = pd.concat(dfs)
-
-# Reordenando o índice
 df.sort_index(inplace=True)
 print(df)
 
 ```
+output example:
+
+| topic     | author        | country   | language   | title                                                                            | summary                                                                          |
+|:----------|:--------------|:----------|:-----------|:---------------------------------------------------------------------------------|:---------------------------------------------------------------------------------|
+| finance   | Reuters       | GB        | en         | Italy pushes to limit executive pay in listed state-run firms                    | Italy pushes to limit executive pay in listed state-run firms                    |
+| economics | Reuters       | GB        | en         | UK's Cleverly raises Xinjiang and Taiwan with Chinese vice president             | UK's Cleverly raises Xinjiang and Taiwan with Chinese vice president             |
+| news      | Reuters       | GB        | en         | Ukraine hails return of 45 Azov fighters, Russia says 3 pilots released          | Ukraine hails return of 45 Azov fighters, Russia says 3 pilots released          |
+
+
+
+
+
+There is a limited set of topic that you might find:
+``` 'tech', 'news', 'business', 'science', 'finance', 'food', 'politics', 'economics', 'travel', 'entertainment', 'music', 'sport', 'world' ```
+
+extras topics only for [investing.com](https://www.investing.com)
+
+``` 'crypto', 'forex', 'stock', 'commodities', 'central_bank', 'forex_analysis', 'forex_technical', 'forex_fundamental', 'forex_opinion', 'forex_signal', 'bonds_analysis', 'bonds_technical', 'bonds_fundamental', 'bonds_opinion', 'bonds_strategy', 'bonds_government', 'bonds_corporate', 'stock_analysis', 'stock_technical', 'stock_fundamental', 'stock_opinion', 'stock_picks', 'indices_analysis', 'futures_analysis', 'options_analysis', 'commodities_analysis', 'commodities_technical', 'commodities_Fundamental', 'commodities_opinion', 'commodities_strategy', 'commodities_metals', 'commodities_energy', 'commodities_agriculture', 'overview_analysis', 'overview_technical', 'overview_fundamental', 'overview_opinion', 'overview_investing', 'crypto_opinion'```
+  
+
 
-for investing.com  is a limited set of topic base on country 
 
-``` 'news', 'crypto_news', 'forex_news', 'popular_news', 'commodities_news', 'stock_news', 'economic_indicators_news', 'economy_news', 'central_bank', 'crypto_opinion', 'forex_analysis', 'forex_technical', 'forex_fundamental', 'forex_opinion', 'forex_signal', 'overview_analysis', 'overview_technical', 'overview_fundamental', 'overview_opinion', 'overview_investing', 'commodities_analysis', 'commodities_technical', 'commodities_Fundamental', 'commodities_opinion', 'commodities_strategy', 'commodities_metals', 'commodities_energy', 'commodities_agriculture', 'bonds_analysis', 'bonds_technical', 'bonds_fundamental', 'bonds_opinion', 'bonds_trategy', 'bonds_government', 'bonds_corporate', 'stock_analysis', 'stock_technical', 'stock_fundamental', 'stock_opinion', 'stock_picks', 'stock', 'indices', 'futures', 'options', 'politics_news', 'world_news' ```
 
 However, not all topics are supported by every newspaper.
 
 How to check which topics are supported by which newspaper:
 ```python
 from ejtraderNS import describe_url
 
@@ -247,31 +231,17 @@
 `US`, `GB`, `DE`, `FR`, `IN`, `RU`, `ES`, `BR`, `IT`, `CA`, `AU`, `NL`, `PL`, `NZ`, `PT`, `RO`, `UA`, `JP`, `AR`, `IR`, `IE`, `PH`, `IS`, `ZA`, `AT`, `CL`, `HR`, `BG`, `HU`, `KR`, `SZ`, `AE`, `EG`, `VE`, `CO`, `SE`, `CZ`, `ZH`, `MT`, `AZ`, `GR`, `BE`, `LU`, `IL`, `LT`, `NI`, `MY`, `TR`, `BM`, `NO`, `ME`, `SA`, `RS`, `BA`
 
 Supported languages:
 `EL`, `IT`, `ZH`, `EN`, `RU`, `CS`, `RO`, `FR`, `JA`, `DE`, `PT`, `ES`, `AR`, `HE`, `UK`, `PL`, `NL`, `TR`, `VI`, `KO`, `TH`, `ID`, `HR`, `DA`, `BG`, `NO`, `SK`, `FA`, `ET`, `SV`, `BN`, `GU`, `MK`, `PA`, `HU`, `SL`, `FI`, `LT`, `MR`, `HI`
 
 
 
-
-
 ## Tech/framework used
 The package itself is nothing more than a SQLite database with 
 RSS feed endpoints for each website and some basic wrapper of
 [feedparser](https://pythonhosted.org/feedparser/index.html).
 
 
-## About Us
-We are ejtraderNS API team. We are glad that you liked our package.
-
-If you want to search for any news data, consider using [our API](https://ejtraderNSapi.com/)
-
-![](ejtraderNS_oneliner.png)
-
-
-[Artem Bugara]() - co-founder of ejtraderNS, made v.0.1.0
-
-[Maksym Sugonyaka](https://www.linkedin.com/mwlite/in/msugonyaka) - co-founder of ejtraderNS, made v.0.1.0
+## Acknowledgements
 
-[Becket Trotter](https://www.linkedin.com/in/beckettrotter/) - Python Developer, made v.0.2.0
+I would like to express my gratitude to [@kotartemiy](https://github.com/kotartemiy) for creating the initial project. Their work has been an invaluable starting point for my modifications and improvements.
 
-## Licence
-MIT
```

### Comparing `ejtraderNS-0.0.2/ejtraderNS/__init__.py` & `ejtraderNS-0.0.3/ejtraderNS/__init__.py`

 * *Files identical despite different names*

### Comparing `ejtraderNS-0.0.2/ejtraderNS/data/rss.db` & `ejtraderNS-0.0.3/ejtraderNS/data/rss.db`

 * *Files 3% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -4500,1298 +4500,1544 @@
 INSERT INTO rss_main VALUES('dailyprogress.com','en','news',1,'None','http://www.dailyprogress.com/search/?q=&t=article&l=25&d=&d1=&d2=&s=start_time&sd=desc&c[]=news*&f=rss',11347);
 INSERT INTO rss_main VALUES('dailypress.com','en','politics',1,'None','http://www.dailypress.com/rss2.0.xml',999999);
 INSERT INTO rss_main VALUES('cwtv.com','en','entertainment',1,'None','http://www.cwtv.com/feed/episodes/xml',8519);
 INSERT INTO rss_main VALUES('uol.com.br','pt','tech','None','BR','http://rss.tecnologia.uol.com.br/ultnot/index.xml',667);
 INSERT INTO rss_main VALUES('uol.com.br','pt','politics','None','BR','http://congressoemfoco.uol.com.br/feed/',667);
 INSERT INTO rss_main VALUES('uol.com.br','pt','news',1,'BR','http://rss.noticias.uol.com.br/ultnot/index.xml',667);
 INSERT INTO rss_main VALUES('uol.com.br','pt','economics','None','BR','http://rss.noticias.uol.com.br/economia/ultnot/index.xml',667);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AF','https://tradingeconomics.com/afghanistan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AL','https://tradingeconomics.com/albania/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'DZ','https://tradingeconomics.com/algeria/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AD','https://tradingeconomics.com/andorra/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AO','https://tradingeconomics.com/angola/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AG','https://tradingeconomics.com/antigua-and-barbuda/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AR','https://tradingeconomics.com/argentina/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AM','https://tradingeconomics.com/armenia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AW','https://tradingeconomics.com/aruba/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AU','https://tradingeconomics.com/australia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AT','https://tradingeconomics.com/austria/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AZ','https://tradingeconomics.com/azerbaijan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BS','https://tradingeconomics.com/bahamas/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BH','https://tradingeconomics.com/bahrain/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BD','https://tradingeconomics.com/bangladesh/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BB','https://tradingeconomics.com/barbados/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BY','https://tradingeconomics.com/belarus/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BE','https://tradingeconomics.com/belgium/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BZ','https://tradingeconomics.com/belize/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BJ','https://tradingeconomics.com/benin/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BT','https://tradingeconomics.com/bhutan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BO','https://tradingeconomics.com/bolivia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BA','https://tradingeconomics.com/bosnia-and-herzegovina/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BW','https://tradingeconomics.com/botswana/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BR','https://tradingeconomics.com/brazil/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BN','https://tradingeconomics.com/brunei/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BG','https://tradingeconomics.com/bulgaria/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BF','https://tradingeconomics.com/burkina-faso/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'BI','https://tradingeconomics.com/burundi/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KH','https://tradingeconomics.com/cambodia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CM','https://tradingeconomics.com/cameroon/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CA','https://tradingeconomics.com/canada/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CV','https://tradingeconomics.com/cape-verde/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CF','https://tradingeconomics.com/central-african-republic/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TD','https://tradingeconomics.com/chad/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CL','https://tradingeconomics.com/chile/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CN','https://tradingeconomics.com/china/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CO','https://tradingeconomics.com/colombia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KM','https://tradingeconomics.com/comoros/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CG','https://tradingeconomics.com/congo/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CR','https://tradingeconomics.com/costa-rica/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'HR','https://tradingeconomics.com/croatia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CU','https://tradingeconomics.com/cuba/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CY','https://tradingeconomics.com/cyprus/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CZ','https://tradingeconomics.com/czech-republic/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'DK','https://tradingeconomics.com/denmark/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'DJ','https://tradingeconomics.com/djibouti/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'DM','https://tradingeconomics.com/dominica/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'DO','https://tradingeconomics.com/dominican-republic/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'EC','https://tradingeconomics.com/ecuador/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'EG','https://tradingeconomics.com/egypt/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SV','https://tradingeconomics.com/el-salvador/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GQ','https://tradingeconomics.com/equatorial-guinea/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'EE','https://tradingeconomics.com/estonia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ET','https://tradingeconomics.com/ethiopia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'FJ','https://tradingeconomics.com/fiji/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'FI','https://tradingeconomics.com/finland/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'FR','https://tradingeconomics.com/france/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GA','https://tradingeconomics.com/gabon/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GM','https://tradingeconomics.com/gambia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GE','https://tradingeconomics.com/georgia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'DE','https://tradingeconomics.com/germany/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GH','https://tradingeconomics.com/ghana/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GR','https://tradingeconomics.com/greece/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GL','https://tradingeconomics.com/greenland/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GD','https://tradingeconomics.com/grenada/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GT','https://tradingeconomics.com/guatemala/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GN','https://tradingeconomics.com/guinea/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GW','https://tradingeconomics.com/guinea-bissau/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GY','https://tradingeconomics.com/guyana/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'HT','https://tradingeconomics.com/haiti/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'HN','https://tradingeconomics.com/honduras/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'HK','https://tradingeconomics.com/hong-kong/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'HU','https://tradingeconomics.com/hungary/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'IS','https://tradingeconomics.com/iceland/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'IN','https://tradingeconomics.com/india/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ID','https://tradingeconomics.com/indonesia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'IR','https://tradingeconomics.com/iran/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'IQ','https://tradingeconomics.com/iraq/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'IE','https://tradingeconomics.com/ireland/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'IL','https://tradingeconomics.com/israel/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'IT','https://tradingeconomics.com/italy/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CI','https://tradingeconomics.com/ivory-coast/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'JM','https://tradingeconomics.com/jamaica/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'JP','https://tradingeconomics.com/japan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'JO','https://tradingeconomics.com/jordan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KZ','https://tradingeconomics.com/kazakhstan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KE','https://tradingeconomics.com/kenya/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KI','https://tradingeconomics.com/kiribati/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'XK','https://tradingeconomics.com/kosovo/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KW','https://tradingeconomics.com/kuwait/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KG','https://tradingeconomics.com/kyrgyzstan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LA','https://tradingeconomics.com/laos/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LV','https://tradingeconomics.com/latvia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LB','https://tradingeconomics.com/lebanon/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LS','https://tradingeconomics.com/lesotho/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LR','https://tradingeconomics.com/liberia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LY','https://tradingeconomics.com/libya/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LI','https://tradingeconomics.com/liechtenstein/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LT','https://tradingeconomics.com/lithuania/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LU','https://tradingeconomics.com/luxembourg/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MO','https://tradingeconomics.com/macau/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MK','https://tradingeconomics.com/macedonia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MG','https://tradingeconomics.com/madagascar/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MW','https://tradingeconomics.com/malawi/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MY','https://tradingeconomics.com/malaysia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MV','https://tradingeconomics.com/maldives/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ML','https://tradingeconomics.com/mali/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MT','https://tradingeconomics.com/malta/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MH','https://tradingeconomics.com/marshall-islands/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MR','https://tradingeconomics.com/mauritania/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MU','https://tradingeconomics.com/mauritius/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MX','https://tradingeconomics.com/mexico/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'FM','https://tradingeconomics.com/micronesia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MD','https://tradingeconomics.com/moldova/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MC','https://tradingeconomics.com/monaco/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MN','https://tradingeconomics.com/mongolia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ME','https://tradingeconomics.com/montenegro/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MA','https://tradingeconomics.com/morocco/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MZ','https://tradingeconomics.com/mozambique/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'MM','https://tradingeconomics.com/myanmar/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NA','https://tradingeconomics.com/namibia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NR','https://tradingeconomics.com/nauru/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NP','https://tradingeconomics.com/nepal/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NL','https://tradingeconomics.com/netherlands/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NC','https://tradingeconomics.com/new-caledonia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NZ','https://tradingeconomics.com/new-zealand/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NI','https://tradingeconomics.com/nicaragua/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NE','https://tradingeconomics.com/niger/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NG','https://tradingeconomics.com/nigeria/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KP','https://tradingeconomics.com/north-korea/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'NO','https://tradingeconomics.com/norway/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'OM','https://tradingeconomics.com/oman/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PK','https://tradingeconomics.com/pakistan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PW','https://tradingeconomics.com/palau/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PS','https://tradingeconomics.com/palestine/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PA','https://tradingeconomics.com/panama/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PG','https://tradingeconomics.com/papua-new-guinea/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PY','https://tradingeconomics.com/paraguay/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PE','https://tradingeconomics.com/peru/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PH','https://tradingeconomics.com/philippines/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PL','https://tradingeconomics.com/poland/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PT','https://tradingeconomics.com/portugal/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'PR','https://tradingeconomics.com/puerto-rico/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'QA','https://tradingeconomics.com/qatar/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CD','https://tradingeconomics.com/republic-of-the-congo/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'RO','https://tradingeconomics.com/romania/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'RU','https://tradingeconomics.com/russia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'RW','https://tradingeconomics.com/rwanda/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KN','https://tradingeconomics.com/st-kitts-and-nevis/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LC','https://tradingeconomics.com/st-lucia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'VC','https://tradingeconomics.com/st-vincent-and-the-grenadines/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'WS','https://tradingeconomics.com/samoa/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SM','https://tradingeconomics.com/san-marino/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ST','https://tradingeconomics.com/sao-tome-and-principe/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SA','https://tradingeconomics.com/saudi-arabia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SN','https://tradingeconomics.com/senegal/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'RS','https://tradingeconomics.com/serbia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SC','https://tradingeconomics.com/seychelles/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SL','https://tradingeconomics.com/sierra-leone/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SG','https://tradingeconomics.com/singapore/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SK','https://tradingeconomics.com/slovakia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SI','https://tradingeconomics.com/slovenia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SB','https://tradingeconomics.com/solomon-islands/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SO','https://tradingeconomics.com/somalia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ZA','https://tradingeconomics.com/south-africa/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'KR','https://tradingeconomics.com/south-korea/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SS','https://tradingeconomics.com/south-sudan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ES','https://tradingeconomics.com/spain/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'LK','https://tradingeconomics.com/sri-lanka/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SD','https://tradingeconomics.com/sudan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SR','https://tradingeconomics.com/suriname/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SZ','https://tradingeconomics.com/swaziland/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SE','https://tradingeconomics.com/sweden/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'CH','https://tradingeconomics.com/switzerland/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'SY','https://tradingeconomics.com/syria/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TW','https://tradingeconomics.com/taiwan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TJ','https://tradingeconomics.com/tajikistan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TZ','https://tradingeconomics.com/tanzania/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TH','https://tradingeconomics.com/thailand/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TL','https://tradingeconomics.com/timor-leste/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TG','https://tradingeconomics.com/togo/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TO','https://tradingeconomics.com/tonga/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TT','https://tradingeconomics.com/trinidad-and-tobago/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TN','https://tradingeconomics.com/tunisia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TR','https://tradingeconomics.com/turkey/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TM','https://tradingeconomics.com/turkmenistan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'TV','https://tradingeconomics.com/tuvalu/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'UG','https://tradingeconomics.com/uganda/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'UA','https://tradingeconomics.com/ukraine/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'AE','https://tradingeconomics.com/united-arab-emirates/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'GB','https://tradingeconomics.com/united-kingdom/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'US','https://tradingeconomics.com/united-states/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'UY','https://tradingeconomics.com/uruguay/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'UZ','https://tradingeconomics.com/uzbekistan/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'VU','https://tradingeconomics.com/vanuatu/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'VA','https://tradingeconomics.com/vatican-city/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'VE','https://tradingeconomics.com/venezuela/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'VN','https://tradingeconomics.com/vietnam/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'YE','https://tradingeconomics.com/yemen/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ZM','https://tradingeconomics.com/zambia/rss',2289);
+INSERT INTO rss_main VALUES('tradingeconomics.com','en','news',1,'ZW','https://tradingeconomics.com/zimbabwe/rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','news',1,'RU','https://ru.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','crypto_news',0,'RU','https://ru.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','forex_news',0,'RU','https://ru.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','popular_news',0,'RU','https://ru.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_news',0,'RU','https://ru.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','stock_news',0,'RU','https://ru.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','economic_indicators_news',0,'RU','https://ru.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','economy_news',0,'RU','https://ru.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','world',0,'RU','https://ru.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','finance',0,'RU','https://ru.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','economics',0,'RU','https://ru.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','politics',0,'RU','https://ru.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','popular',0,'RU','https://ru.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','crypto',0,'RU','https://ru.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','forex',0,'RU','https://ru.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','stock',0,'RU','https://ru.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities',0,'RU','https://ru.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','central_bank',0,'RU','https://ru.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','crypto_opinion ',0,'RU','https://ru.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','forex_analysis',0,'RU','https://ru.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','forex_technical',0,'RU','https://ru.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','forex_fundamental',0,'RU','https://ru.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','forex_opinion',0,'RU','https://ru.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','forex_signal',0,'RU','https://ru.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','overview_analysis',0,'RU','https://ru.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','overview_technical',0,'RU','https://ru.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','overview_fundamental',0,'RU','https://ru.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','overview_opinion',0,'RU','https://ru.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','overview_investing',0,'RU','https://ru.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_analysis',0,'RU','https://ru.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_technical',0,'RU','https://ru.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_Fundamental',0,'RU','https://ru.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_opinion',0,'RU','https://ru.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_strategy',0,'RU','https://ru.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_metals',0,'RU','https://ru.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_energy',0,'RU','https://ru.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','commodities_agriculture',0,'RU','https://ru.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','bonds_analysis',0,'RU','https://ru.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','bonds_technical',0,'RU','https://ru.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','bonds_fundamental',0,'RU','https://ru.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','bonds_opinion',0,'RU','https://ru.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','bonds_trategy',0,'RU','https://ru.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','bonds_government',0,'RU','https://ru.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','bonds_corporate',0,'RU','https://ru.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','stock_analysis',0,'RU','https://ru.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','stock_technical',0,'RU','https://ru.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','stock_fundamental',0,'RU','https://ru.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','stock_opinion',0,'RU','https://ru.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ru','stock_picks',0,'RU','https://ru.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','stock',0,'RU','https://ru.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','indices',0,'RU','https://ru.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','futures',0,'RU','https://ru.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ru','options',0,'RU','https://ru.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','stock_analysis',0,'RU','https://ru.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','indices_analysis',0,'RU','https://ru.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','futures_analysis',0,'RU','https://ru.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','options_analysis',0,'RU','https://ru.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities_analysis',0,'RU','https://ru.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities_technical',0,'RU','https://ru.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities_Fundamental',0,'RU','https://ru.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities_opinion',0,'RU','https://ru.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities_strategy',0,'RU','https://ru.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities_metals',0,'RU','https://ru.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities_energy',0,'RU','https://ru.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','commodities_agriculture',0,'RU','https://ru.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','overview_analysis',0,'RU','https://ru.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','overview_technical',0,'RU','https://ru.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','overview_fundamental',0,'RU','https://ru.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','overview_opinion',0,'RU','https://ru.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','overview_investing',0,'RU','https://ru.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ru','crypto_opinion',0,'RU','https://ru.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','news',1,'BR','https://br.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','crypto_news',0,'BR','https://br.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','forex_news',0,'BR','https://br.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','popular_news',0,'BR','https://br.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_news',0,'BR','https://br.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','stock_news',0,'BR','https://br.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','economic_indicators_news',0,'BR','https://br.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','politics_news',0,'BR','https://br.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','economy_news',0,'BR','https://br.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','world_news',0,'BR','https://br.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','world',0,'BR','https://br.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','finance',0,'BR','https://br.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','economics',0,'BR','https://br.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','politics',0,'BR','https://br.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','popular',0,'BR','https://br.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','crypto',0,'BR','https://br.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','forex',0,'BR','https://br.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','stock',0,'BR','https://br.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities',0,'BR','https://br.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','central_bank',0,'BR','https://br.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','crypto_opinion ',0,'BR','https://br.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_analysis',0,'BR','https://br.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_technical',0,'BR','https://br.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_fundamental',0,'BR','https://br.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_opinion',0,'BR','https://br.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_signal',0,'BR','https://br.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_analysis',0,'BR','https://br.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_technical',0,'BR','https://br.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_fundamental',0,'BR','https://br.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_opinion',0,'BR','https://br.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_investing',0,'BR','https://br.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_analysis',0,'BR','https://br.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_technical',0,'BR','https://br.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_Fundamental',0,'BR','https://br.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_opinion',0,'BR','https://br.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_strategy',0,'BR','https://br.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_metals',0,'BR','https://br.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_energy',0,'BR','https://br.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_agriculture',0,'BR','https://br.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_analysis',0,'BR','https://br.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_technical',0,'BR','https://br.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_fundamental',0,'BR','https://br.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_opinion',0,'BR','https://br.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_trategy',0,'BR','https://br.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_government',0,'BR','https://br.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_corporate',0,'BR','https://br.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_analysis',0,'BR','https://br.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_technical',0,'BR','https://br.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_fundamental',0,'BR','https://br.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_opinion',0,'BR','https://br.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_picks',0,'BR','https://br.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','stock',0,'BR','https://br.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','indices',0,'BR','https://br.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','futures',0,'BR','https://br.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','options',0,'BR','https://br.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','stock_analysis',0,'BR','https://br.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','indices_analysis',0,'BR','https://br.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','futures_analysis',0,'BR','https://br.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','options_analysis',0,'BR','https://br.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_analysis',0,'BR','https://br.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_technical',0,'BR','https://br.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_Fundamental',0,'BR','https://br.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_opinion',0,'BR','https://br.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_strategy',0,'BR','https://br.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_metals',0,'BR','https://br.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_energy',0,'BR','https://br.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_agriculture',0,'BR','https://br.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_analysis',0,'BR','https://br.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_technical',0,'BR','https://br.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_fundamental',0,'BR','https://br.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_opinion',0,'BR','https://br.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_investing',0,'BR','https://br.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','crypto_opinion',0,'BR','https://br.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','news',1,'PT','https://pt.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','crypto_news',0,'PT','https://pt.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','forex_news',0,'PT','https://pt.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','popular_news',0,'PT','https://pt.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_news',0,'PT','https://pt.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','stock_news',0,'PT','https://pt.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','economic_indicators_news',0,'PT','https://pt.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','politics_news',0,'PT','https://pt.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','economy_news',0,'PT','https://pt.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','world_news',0,'PT','https://pt.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','world',0,'PT','https://pt.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','finance',0,'PT','https://pt.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','economics',0,'PT','https://pt.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','politics',0,'PT','https://pt.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','popular',0,'PT','https://pt.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','crypto',0,'PT','https://pt.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','forex',0,'PT','https://pt.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','stock',0,'PT','https://pt.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities',0,'PT','https://pt.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','central_bank',0,'PT','https://pt.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','crypto_opinion ',0,'PT','https://pt.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_analysis',0,'PT','https://pt.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_technical',0,'PT','https://pt.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_fundamental',0,'PT','https://pt.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_opinion',0,'PT','https://pt.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','forex_signal',0,'PT','https://pt.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_analysis',0,'PT','https://pt.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_technical',0,'PT','https://pt.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_fundamental',0,'PT','https://pt.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_opinion',0,'PT','https://pt.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','overview_investing',0,'PT','https://pt.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_analysis',0,'PT','https://pt.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_technical',0,'PT','https://pt.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_Fundamental',0,'PT','https://pt.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_opinion',0,'PT','https://pt.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_strategy',0,'PT','https://pt.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_metals',0,'PT','https://pt.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_energy',0,'PT','https://pt.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','commodities_agriculture',0,'PT','https://pt.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_analysis',0,'PT','https://pt.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_technical',0,'PT','https://pt.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_fundamental',0,'PT','https://pt.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_opinion',0,'PT','https://pt.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_trategy',0,'PT','https://pt.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_government',0,'PT','https://pt.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','bonds_corporate',0,'PT','https://pt.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_analysis',0,'PT','https://pt.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_technical',0,'PT','https://pt.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_fundamental',0,'PT','https://pt.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_opinion',0,'PT','https://pt.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pt','stock_picks',0,'PT','https://pt.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','stock',0,'PT','https://pt.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','indices',0,'PT','https://pt.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','futures',0,'PT','https://pt.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pt','options',0,'PT','https://pt.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','stock_analysis',0,'PT','https://pt.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','indices_analysis',0,'PT','https://pt.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','futures_analysis',0,'PT','https://pt.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','options_analysis',0,'PT','https://pt.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_analysis',0,'PT','https://pt.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_technical',0,'PT','https://pt.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_Fundamental',0,'PT','https://pt.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_opinion',0,'PT','https://pt.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_strategy',0,'PT','https://pt.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_metals',0,'PT','https://pt.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_energy',0,'PT','https://pt.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','commodities_agriculture',0,'PT','https://pt.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_analysis',0,'PT','https://pt.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_technical',0,'PT','https://pt.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_fundamental',0,'PT','https://pt.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_opinion',0,'PT','https://pt.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','overview_investing',0,'PT','https://pt.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pt','crypto_opinion',0,'PT','https://pt.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','news',1,'TR','https://tr.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','crypto_news',0,'TR','https://tr.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','forex_news',0,'TR','https://tr.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','popular_news',0,'TR','https://tr.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_news',0,'TR','https://tr.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','stock_news',0,'TR','https://tr.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','economic_indicators_news',0,'TR','https://tr.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','politics_news',0,'TR','https://tr.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','economy_news',0,'TR','https://tr.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','world_news',0,'TR','https://tr.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','world',0,'TR','https://tr.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','finance',0,'TR','https://tr.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','economics',0,'TR','https://tr.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','politics',0,'TR','https://tr.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','popular',0,'TR','https://tr.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','crypto',0,'TR','https://tr.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','forex',0,'TR','https://tr.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','stock',0,'TR','https://tr.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities',0,'TR','https://tr.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','central_bank',0,'TR','https://tr.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','crypto_opinion ',0,'TR','https://tr.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','forex_analysis',0,'TR','https://tr.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','forex_technical',0,'TR','https://tr.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','forex_fundamental',0,'TR','https://tr.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','forex_opinion',0,'TR','https://tr.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','forex_signal',0,'TR','https://tr.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','overview_analysis',0,'TR','https://tr.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','overview_technical',0,'TR','https://tr.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','overview_fundamental',0,'TR','https://tr.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','overview_opinion',0,'TR','https://tr.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','overview_investing',0,'TR','https://tr.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_analysis',0,'TR','https://tr.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_technical',0,'TR','https://tr.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_Fundamental',0,'TR','https://tr.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_opinion',0,'TR','https://tr.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_strategy',0,'TR','https://tr.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_metals',0,'TR','https://tr.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_energy',0,'TR','https://tr.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','commodities_agriculture',0,'TR','https://tr.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','bonds_analysis',0,'TR','https://tr.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','bonds_technical',0,'TR','https://tr.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','bonds_fundamental',0,'TR','https://tr.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','bonds_opinion',0,'TR','https://tr.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','bonds_trategy',0,'TR','https://tr.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','bonds_government',0,'TR','https://tr.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','bonds_corporate',0,'TR','https://tr.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','stock_analysis',0,'TR','https://tr.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','stock_technical',0,'TR','https://tr.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','stock_fundamental',0,'TR','https://tr.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','stock_opinion',0,'TR','https://tr.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','tr','stock_picks',0,'TR','https://tr.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','stock',0,'TR','https://tr.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','indices',0,'TR','https://tr.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','futures',0,'TR','https://tr.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','tr','options',0,'TR','https://tr.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','stock_analysis',0,'TR','https://tr.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','indices_analysis',0,'TR','https://tr.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','futures_analysis',0,'TR','https://tr.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','options_analysis',0,'TR','https://tr.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities_analysis',0,'TR','https://tr.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities_technical',0,'TR','https://tr.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities_Fundamental',0,'TR','https://tr.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities_opinion',0,'TR','https://tr.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities_strategy',0,'TR','https://tr.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities_metals',0,'TR','https://tr.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities_energy',0,'TR','https://tr.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','commodities_agriculture',0,'TR','https://tr.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','overview_analysis',0,'TR','https://tr.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','overview_technical',0,'TR','https://tr.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','overview_fundamental',0,'TR','https://tr.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','overview_opinion',0,'TR','https://tr.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','overview_investing',0,'TR','https://tr.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','tr','crypto_opinion',0,'TR','https://tr.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','news',1,'IN','https://in.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_news',0,'IN','https://in.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_news',0,'IN','https://in.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','popular_news',0,'IN','https://in.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_news',0,'IN','https://in.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_news',0,'IN','https://in.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economic_indicators_news',0,'IN','https://in.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','politics_news',0,'IN','https://in.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economy_news',0,'IN','https://in.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','world_news',0,'IN','https://in.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','world',0,'IN','https://in.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','finance',0,'IN','https://in.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','economics',0,'IN','https://in.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','politics',0,'IN','https://in.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','popular',0,'IN','https://in.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto',0,'IN','https://in.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex',0,'IN','https://in.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock',0,'IN','https://in.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities',0,'IN','https://in.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'IN','https://in.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion ',0,'IN','https://in.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'IN','https://in.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'IN','https://in.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'IN','https://in.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'IN','https://in.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'IN','https://in.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'IN','https://in.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'IN','https://in.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'IN','https://in.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'IN','https://in.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'IN','https://in.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'IN','https://in.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'IN','https://in.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'IN','https://in.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'IN','https://in.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'IN','https://in.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'IN','https://in.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'IN','https://in.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'IN','https://in.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'IN','https://in.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'IN','https://in.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'IN','https://in.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'IN','https://in.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'IN','https://in.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'IN','https://in.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'IN','https://in.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'IN','https://in.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'IN','https://in.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'IN','https://in.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'IN','https://in.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'IN','https://in.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock',0,'IN','https://in.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','indices',0,'IN','https://in.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','futures',0,'IN','https://in.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','options',0,'IN','https://in.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'IN','https://in.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','indices_analysis',0,'IN','https://in.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','futures_analysis',0,'IN','https://in.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','options_analysis',0,'IN','https://in.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'IN','https://in.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'IN','https://in.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'IN','https://in.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'IN','https://in.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'IN','https://in.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'IN','https://in.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'IN','https://in.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'IN','https://in.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'IN','https://in.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'IN','https://in.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'IN','https://in.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'IN','https://in.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'IN','https://in.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion',0,'IN','https://in.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','news',1,'AU','https://au.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_news',0,'AU','https://au.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_news',0,'AU','https://au.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','popular_news',0,'AU','https://au.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_news',0,'AU','https://au.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_news',0,'AU','https://au.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economic_indicators_news',0,'AU','https://au.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','politics_news',0,'AU','https://au.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economy_news',0,'AU','https://au.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','world_news',0,'AU','https://au.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','world',0,'AU','https://au.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','finance',0,'AU','https://au.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','economics',0,'AU','https://au.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','politics',0,'AU','https://au.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','popular',0,'AU','https://au.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto',0,'AU','https://au.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex',0,'AU','https://au.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock',0,'AU','https://au.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities',0,'AU','https://au.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'AU','https://au.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion ',0,'AU','https://au.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'AU','https://au.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'AU','https://au.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'AU','https://au.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'AU','https://au.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'AU','https://au.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'AU','https://au.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'AU','https://au.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'AU','https://au.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'AU','https://au.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'AU','https://au.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'AU','https://au.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'AU','https://au.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'AU','https://au.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'AU','https://au.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'AU','https://au.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'AU','https://au.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'AU','https://au.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'AU','https://au.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'AU','https://au.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'AU','https://au.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'AU','https://au.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'AU','https://au.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'AU','https://au.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'AU','https://au.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'AU','https://au.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'AU','https://au.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'AU','https://au.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'AU','https://au.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'AU','https://au.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'AU','https://au.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock',0,'AU','https://au.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','indices',0,'AU','https://au.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','futures',0,'AU','https://au.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','options',0,'AU','https://au.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'AU','https://au.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','indices_analysis',0,'AU','https://au.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','futures_analysis',0,'AU','https://au.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','options_analysis',0,'AU','https://au.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'AU','https://au.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'AU','https://au.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'AU','https://au.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'AU','https://au.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'AU','https://au.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'AU','https://au.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'AU','https://au.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'AU','https://au.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'AU','https://au.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'AU','https://au.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'AU','https://au.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'AU','https://au.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'AU','https://au.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion',0,'AU','https://au.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','news',1,'PH','https://ph.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_news',0,'PH','https://ph.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_news',0,'PH','https://ph.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','popular_news',0,'PH','https://ph.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_news',0,'PH','https://ph.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_news',0,'PH','https://ph.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economic_indicators_news',0,'PH','https://ph.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','politics_news',0,'PH','https://ph.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economy_news',0,'PH','https://ph.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','world_news',0,'PH','https://ph.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','world',0,'PH','https://ph.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','finance',0,'PH','https://ph.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','economics',0,'PH','https://ph.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','politics',0,'PH','https://ph.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','popular',0,'PH','https://ph.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto',0,'PH','https://ph.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex',0,'PH','https://ph.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock',0,'PH','https://ph.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities',0,'PH','https://ph.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'PH','https://ph.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion ',0,'PH','https://ph.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'PH','https://ph.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'PH','https://ph.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'PH','https://ph.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'PH','https://ph.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'PH','https://ph.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'PH','https://ph.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'PH','https://ph.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'PH','https://ph.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'PH','https://ph.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'PH','https://ph.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'PH','https://ph.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'PH','https://ph.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'PH','https://ph.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'PH','https://ph.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'PH','https://ph.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'PH','https://ph.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'PH','https://ph.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'PH','https://ph.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'PH','https://ph.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'PH','https://ph.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'PH','https://ph.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'PH','https://ph.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'PH','https://ph.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'PH','https://ph.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'PH','https://ph.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'PH','https://ph.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'PH','https://ph.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'PH','https://ph.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'PH','https://ph.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'PH','https://ph.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock',0,'PH','https://ph.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','indices',0,'PH','https://ph.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','futures',0,'PH','https://ph.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','options',0,'PH','https://ph.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'PH','https://ph.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','indices_analysis',0,'PH','https://ph.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','futures_analysis',0,'PH','https://ph.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','options_analysis',0,'PH','https://ph.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'PH','https://ph.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'PH','https://ph.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'PH','https://ph.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'PH','https://ph.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'PH','https://ph.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'PH','https://ph.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'PH','https://ph.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'PH','https://ph.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'PH','https://ph.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'PH','https://ph.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'PH','https://ph.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'PH','https://ph.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'PH','https://ph.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion',0,'PH','https://ph.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','news',1,'ZA','https://za.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_news',0,'ZA','https://za.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_news',0,'ZA','https://za.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','popular_news',0,'ZA','https://za.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_news',0,'ZA','https://za.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_news',0,'ZA','https://za.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economic_indicators_news',0,'ZA','https://za.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','politics_news',0,'ZA','https://za.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economy_news',0,'ZA','https://za.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','world_news',0,'ZA','https://za.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','world',0,'ZA','https://za.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','finance',0,'ZA','https://za.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','economics',0,'ZA','https://za.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','politics',0,'ZA','https://za.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','popular',0,'ZA','https://za.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto',0,'ZA','https://za.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex',0,'ZA','https://za.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock',0,'ZA','https://za.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities',0,'ZA','https://za.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'ZA','https://za.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion ',0,'ZA','https://za.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'ZA','https://za.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'ZA','https://za.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'ZA','https://za.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'ZA','https://za.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'ZA','https://za.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'ZA','https://za.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'ZA','https://za.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'ZA','https://za.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'ZA','https://za.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'ZA','https://za.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'ZA','https://za.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'ZA','https://za.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'ZA','https://za.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'ZA','https://za.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'ZA','https://za.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'ZA','https://za.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'ZA','https://za.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'ZA','https://za.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'ZA','https://za.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'ZA','https://za.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'ZA','https://za.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'ZA','https://za.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'ZA','https://za.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'ZA','https://za.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'ZA','https://za.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'ZA','https://za.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'ZA','https://za.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'ZA','https://za.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'ZA','https://za.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'ZA','https://za.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock',0,'ZA','https://za.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','indices',0,'ZA','https://za.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','futures',0,'ZA','https://za.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','options',0,'ZA','https://za.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'ZA','https://za.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','indices_analysis',0,'ZA','https://za.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','futures_analysis',0,'ZA','https://za.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','options_analysis',0,'ZA','https://za.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'ZA','https://za.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'ZA','https://za.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'ZA','https://za.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'ZA','https://za.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'ZA','https://za.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'ZA','https://za.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'ZA','https://za.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'ZA','https://za.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'ZA','https://za.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'ZA','https://za.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'ZA','https://za.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'ZA','https://za.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'ZA','https://za.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion',0,'ZA','https://za.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','news',1,'CA','https://ca.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_news',0,'CA','https://ca.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_news',0,'CA','https://ca.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','popular_news',0,'CA','https://ca.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_news',0,'CA','https://ca.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_news',0,'CA','https://ca.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economic_indicators_news',0,'CA','https://ca.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','politics_news',0,'CA','https://ca.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economy_news',0,'CA','https://ca.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','world_news',0,'CA','https://ca.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','world',0,'CA','https://ca.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','finance',0,'CA','https://ca.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','economics',0,'CA','https://ca.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','politics',0,'CA','https://ca.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','popular',0,'CA','https://ca.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto',0,'CA','https://ca.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex',0,'CA','https://ca.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock',0,'CA','https://ca.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities',0,'CA','https://ca.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'CA','https://ca.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion ',0,'CA','https://ca.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'CA','https://ca.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'CA','https://ca.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'CA','https://ca.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'CA','https://ca.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'CA','https://ca.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'CA','https://ca.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'CA','https://ca.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'CA','https://ca.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'CA','https://ca.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'CA','https://ca.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'CA','https://ca.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'CA','https://ca.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'CA','https://ca.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'CA','https://ca.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'CA','https://ca.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'CA','https://ca.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'CA','https://ca.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'CA','https://ca.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'CA','https://ca.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'CA','https://ca.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'CA','https://ca.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'CA','https://ca.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'CA','https://ca.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'CA','https://ca.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'CA','https://ca.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'CA','https://ca.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'CA','https://ca.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'CA','https://ca.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'CA','https://ca.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'CA','https://ca.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock',0,'CA','https://ca.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','indices',0,'CA','https://ca.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','futures',0,'CA','https://ca.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','options',0,'CA','https://ca.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'CA','https://ca.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','indices_analysis',0,'CA','https://ca.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','futures_analysis',0,'CA','https://ca.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','options_analysis',0,'CA','https://ca.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'CA','https://ca.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'CA','https://ca.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'CA','https://ca.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'CA','https://ca.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'CA','https://ca.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'CA','https://ca.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'CA','https://ca.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'CA','https://ca.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'CA','https://ca.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'CA','https://ca.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'CA','https://ca.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'CA','https://ca.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'CA','https://ca.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion',0,'CA','https://ca.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','news',1,'GB','https://uk.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_news',0,'GB','https://uk.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_news',0,'GB','https://uk.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','popular_news',0,'GB','https://uk.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_news',0,'GB','https://uk.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_news',0,'GB','https://uk.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economic_indicators_news',0,'GB','https://uk.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','politics_news',0,'GB','https://uk.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economy_news',0,'GB','https://uk.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','world_news',0,'GB','https://uk.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','world',0,'GB','https://uk.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','finance',0,'GB','https://uk.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','economics',0,'GB','https://uk.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','politics',0,'GB','https://uk.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','popular',0,'GB','https://uk.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto',0,'GB','https://uk.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex',0,'GB','https://uk.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock',0,'GB','https://uk.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities',0,'GB','https://uk.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'GB','https://uk.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion ',0,'GB','https://uk.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'GB','https://uk.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'GB','https://uk.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'GB','https://uk.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'GB','https://uk.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'GB','https://uk.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'GB','https://uk.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'GB','https://uk.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'GB','https://uk.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'GB','https://uk.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'GB','https://uk.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'GB','https://uk.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'GB','https://uk.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'GB','https://uk.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'GB','https://uk.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'GB','https://uk.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'GB','https://uk.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'GB','https://uk.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'GB','https://uk.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'GB','https://uk.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'GB','https://uk.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'GB','https://uk.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'GB','https://uk.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'GB','https://uk.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'GB','https://uk.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'GB','https://uk.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'GB','https://uk.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'GB','https://uk.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'GB','https://uk.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'GB','https://uk.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'GB','https://uk.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock',0,'GB','https://uk.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','indices',0,'GB','https://uk.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','futures',0,'GB','https://uk.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','options',0,'GB','https://uk.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'GB','https://uk.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','indices_analysis',0,'GB','https://uk.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','futures_analysis',0,'GB','https://uk.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','options_analysis',0,'GB','https://uk.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'GB','https://uk.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'GB','https://uk.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'GB','https://uk.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'GB','https://uk.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'GB','https://uk.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'GB','https://uk.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'GB','https://uk.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'GB','https://uk.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'GB','https://uk.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'GB','https://uk.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'GB','https://uk.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'GB','https://uk.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'GB','https://uk.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion',0,'GB','https://uk.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','news',1,'NG','https://ng.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_news',0,'NG','https://ng.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_news',0,'NG','https://ng.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','popular_news',0,'NG','https://ng.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_news',0,'NG','https://ng.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_news',0,'NG','https://ng.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economic_indicators_news',0,'NG','https://ng.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','politics_news',0,'NG','https://ng.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economy_news',0,'NG','https://ng.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','world_news',0,'NG','https://ng.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','world',0,'NG','https://ng.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','finance',0,'NG','https://ng.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','economics',0,'NG','https://ng.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','politics',0,'NG','https://ng.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','popular',0,'NG','https://ng.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto',0,'NG','https://ng.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex',0,'NG','https://ng.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock',0,'NG','https://ng.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities',0,'NG','https://ng.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'NG','https://ng.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion ',0,'NG','https://ng.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'NG','https://ng.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'NG','https://ng.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'NG','https://ng.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'NG','https://ng.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'NG','https://ng.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'NG','https://ng.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'NG','https://ng.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'NG','https://ng.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'NG','https://ng.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'NG','https://ng.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'NG','https://ng.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'NG','https://ng.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'NG','https://ng.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'NG','https://ng.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'NG','https://ng.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'NG','https://ng.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'NG','https://ng.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'NG','https://ng.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'NG','https://ng.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'NG','https://ng.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'NG','https://ng.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'NG','https://ng.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'NG','https://ng.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'NG','https://ng.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'NG','https://ng.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'NG','https://ng.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'NG','https://ng.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'NG','https://ng.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'NG','https://ng.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'NG','https://ng.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock',0,'NG','https://ng.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','indices',0,'NG','https://ng.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','futures',0,'NG','https://ng.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','options',0,'NG','https://ng.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'NG','https://ng.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','indices_analysis',0,'NG','https://ng.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','futures_analysis',0,'NG','https://ng.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','options_analysis',0,'NG','https://ng.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'NG','https://ng.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'NG','https://ng.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'NG','https://ng.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'NG','https://ng.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'NG','https://ng.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'NG','https://ng.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'NG','https://ng.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'NG','https://ng.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'NG','https://ng.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'NG','https://ng.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'NG','https://ng.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'NG','https://ng.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'NG','https://ng.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion',0,'NG','https://ng.investing.com/rss/302.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','news',1,'US','https://www.investing.com/rss/news.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','world',0,'US','https://www.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','finance',0,'US','https://www.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','economics',0,'US','https://www.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','politics',0,'US','https://www.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','popular',0,'US','https://www.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto',0,'US','https://www.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex',0,'US','https://www.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock',0,'US','https://www.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities',0,'US','https://www.investing.com/rss/news_11.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'US','https://www.investing.com/rss/central_banks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'US','https://www.investing.com/rss/forex.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'US','https://www.investing.com/rss/forex_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'US','https://www.investing.com/rss/forex_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'US','https://www.investing.com/rss/forex_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'US','https://www.investing.com/rss/forex_Signals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'US','https://www.investing.com/rss/bonds.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'US','https://www.investing.com/rss/bonds_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'US','https://www.investing.com/rss/bonds_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'US','https://www.investing.com/rss/bonds_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'US','https://www.investing.com/rss/bonds_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'US','https://www.investing.com/rss/bonds_Government.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'US','https://www.investing.com/rss/bonds_Corporate.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'US','https://www.investing.com/rss/stock.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'US','https://www.investing.com/rss/stock_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'US','https://www.investing.com/rss/stock_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'US','https://www.investing.com/rss/stock_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'US','https://www.investing.com/rss/stock_stock_picks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'US','https://www.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','indices_analysis',0,'US','https://www.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','futures_analysis',0,'US','https://www.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','options_analysis',0,'US','https://www.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'US','https://www.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'US','https://www.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'US','https://www.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'US','https://www.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'US','https://www.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'US','https://www.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'US','https://www.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'US','https://www.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'US','https://www.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'US','https://www.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'US','https://www.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'US','https://www.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'US','https://www.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion',0,'US','https://www.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','news',1,'SA','https://sa.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','crypto_news',0,'SA','https://sa.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','forex_news',0,'SA','https://sa.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','popular_news',0,'SA','https://sa.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_news',0,'SA','https://sa.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','stock_news',0,'SA','https://sa.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','economic_indicators_news',0,'SA','https://sa.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','politics_news',0,'SA','https://sa.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','economy_news',0,'SA','https://sa.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','world_news',0,'SA','https://sa.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','world',0,'SA','https://sa.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','finance',0,'SA','https://sa.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','economics',0,'SA','https://sa.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','politics',0,'SA','https://sa.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','popular',0,'SA','https://sa.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','crypto',0,'SA','https://sa.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','forex',0,'SA','https://sa.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','stock',0,'SA','https://sa.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities',0,'SA','https://sa.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','central_bank',0,'SA','https://sa.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','crypto_opinion ',0,'SA','https://sa.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','forex_analysis',0,'SA','https://sa.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','forex_technical',0,'SA','https://sa.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','forex_fundamental',0,'SA','https://sa.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','forex_opinion',0,'SA','https://sa.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','forex_signal',0,'SA','https://sa.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','overview_analysis',0,'SA','https://sa.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','overview_technical',0,'SA','https://sa.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','overview_fundamental',0,'SA','https://sa.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','overview_opinion',0,'SA','https://sa.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','overview_investing',0,'SA','https://sa.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_analysis',0,'SA','https://sa.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_technical',0,'SA','https://sa.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_Fundamental',0,'SA','https://sa.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_opinion',0,'SA','https://sa.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_strategy',0,'SA','https://sa.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_metals',0,'SA','https://sa.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_energy',0,'SA','https://sa.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','commodities_agriculture',0,'SA','https://sa.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','bonds_analysis',0,'SA','https://sa.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','bonds_technical',0,'SA','https://sa.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','bonds_fundamental',0,'SA','https://sa.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','bonds_opinion',0,'SA','https://sa.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','bonds_trategy',0,'SA','https://sa.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','bonds_government',0,'SA','https://sa.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','bonds_corporate',0,'SA','https://sa.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','stock_analysis',0,'SA','https://sa.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','stock_technical',0,'SA','https://sa.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','stock_fundamental',0,'SA','https://sa.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','stock_opinion',0,'SA','https://sa.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ar','stock_picks',0,'SA','https://sa.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','stock',0,'SA','https://sa.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','indices',0,'SA','https://sa.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','futures',0,'SA','https://sa.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ar','options',0,'SA','https://sa.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','stock_analysis',0,'SA','https://sa.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','indices_analysis',0,'SA','https://sa.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','futures_analysis',0,'SA','https://sa.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','options_analysis',0,'SA','https://sa.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities_analysis',0,'SA','https://sa.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities_technical',0,'SA','https://sa.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities_Fundamental',0,'SA','https://sa.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities_opinion',0,'SA','https://sa.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities_strategy',0,'SA','https://sa.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities_metals',0,'SA','https://sa.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities_energy',0,'SA','https://sa.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','commodities_agriculture',0,'SA','https://sa.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','overview_analysis',0,'SA','https://sa.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','overview_technical',0,'SA','https://sa.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','overview_fundamental',0,'SA','https://sa.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','overview_opinion',0,'SA','https://sa.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','overview_investing',0,'SA','https://sa.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ar','crypto_opinion',0,'SA','https://sa.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','el','news',1,'GR','https://gr.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','el','economy_news',0,'GR','https://gr.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','el','world_news',0,'GR','https://gr.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','world',0,'GR','https://gr.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','finance',0,'GR','https://gr.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','economics',0,'GR','https://gr.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','politics',0,'GR','https://gr.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','popular',0,'GR','https://gr.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','crypto',0,'GR','https://gr.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','forex',0,'GR','https://gr.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','stock',0,'GR','https://gr.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities',0,'GR','https://gr.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','el','central_bank',0,'GR','https://gr.investing.com/rss/central_banks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','forex_analysis',0,'GR','https://gr.investing.com/rss/forex.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','forex_technical',0,'GR','https://gr.investing.com/rss/forex_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','forex_fundamental',0,'GR','https://gr.investing.com/rss/forex_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','forex_opinion',0,'GR','https://gr.investing.com/rss/forex_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','forex_signal',0,'GR','https://gr.investing.com/rss/forex_Signals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','bonds_analysis',0,'GR','https://gr.investing.com/rss/bonds.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','bonds_technical',0,'GR','https://gr.investing.com/rss/bonds_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','bonds_fundamental',0,'GR','https://gr.investing.com/rss/bonds_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','bonds_opinion',0,'GR','https://gr.investing.com/rss/bonds_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','bonds_trategy',0,'GR','https://gr.investing.com/rss/bonds_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','bonds_government',0,'GR','https://gr.investing.com/rss/bonds_Government.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','bonds_corporate',0,'GR','https://gr.investing.com/rss/bonds_Corporate.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','stock_analysis',0,'GR','https://gr.investing.com/rss/stock.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','stock_technical',0,'GR','https://gr.investing.com/rss/stock_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','stock_fundamental',0,'GR','https://gr.investing.com/rss/stock_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','stock_opinion',0,'GR','https://gr.investing.com/rss/stock_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','stock_picks',0,'GR','https://gr.investing.com/rss/stock_stock_picks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','stock_analysis',0,'GR','https://gr.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','indices_analysis',0,'GR','https://gr.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','futures_analysis',0,'GR','https://gr.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','options_analysis',0,'GR','https://gr.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities_analysis',0,'GR','https://gr.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities_technical',0,'GR','https://gr.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities_Fundamental',0,'GR','https://gr.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities_opinion',0,'GR','https://gr.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities_strategy',0,'GR','https://gr.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities_metals',0,'GR','https://gr.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities_energy',0,'GR','https://gr.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','commodities_agriculture',0,'GR','https://gr.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','overview_analysis',0,'GR','https://gr.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','overview_technical',0,'GR','https://gr.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','overview_fundamental',0,'GR','https://gr.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','overview_opinion',0,'GR','https://gr.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','overview_investing',0,'GR','https://gr.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','el','crypto_opinion',0,'GR','https://gr.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','news',1,'SE','https://se.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','crypto_news',0,'SE','https://se.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','forex_news',0,'SE','https://se.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','popular_news',0,'SE','https://se.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_news',0,'SE','https://se.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','stock_news',0,'SE','https://se.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','economic_indicators_news',0,'SE','https://se.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','politics_news',0,'SE','https://se.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','economy_news',0,'SE','https://se.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','world_news',0,'SE','https://se.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','world',0,'SE','https://se.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','finance',0,'SE','https://se.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','economics',0,'SE','https://se.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','politics',0,'SE','https://se.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','popular',0,'SE','https://se.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','crypto',0,'SE','https://se.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','forex',0,'SE','https://se.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','stock',0,'SE','https://se.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities',0,'SE','https://se.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','central_bank',0,'SE','https://se.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','crypto_opinion ',0,'SE','https://se.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','forex_analysis',0,'SE','https://se.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','forex_technical',0,'SE','https://se.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','forex_fundamental',0,'SE','https://se.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','forex_opinion',0,'SE','https://se.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','forex_signal',0,'SE','https://se.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','overview_analysis',0,'SE','https://se.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','overview_technical',0,'SE','https://se.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','overview_fundamental',0,'SE','https://se.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','overview_opinion',0,'SE','https://se.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','overview_investing',0,'SE','https://se.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_analysis',0,'SE','https://se.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_technical',0,'SE','https://se.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_Fundamental',0,'SE','https://se.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_opinion',0,'SE','https://se.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_strategy',0,'SE','https://se.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_metals',0,'SE','https://se.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_energy',0,'SE','https://se.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','commodities_agriculture',0,'SE','https://se.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','bonds_analysis',0,'SE','https://se.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','bonds_technical',0,'SE','https://se.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','bonds_fundamental',0,'SE','https://se.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','bonds_opinion',0,'SE','https://se.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','bonds_trategy',0,'SE','https://se.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','bonds_government',0,'SE','https://se.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','bonds_corporate',0,'SE','https://se.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','stock_analysis',0,'SE','https://se.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','stock_technical',0,'SE','https://se.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','stock_fundamental',0,'SE','https://se.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','stock_opinion',0,'SE','https://se.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','sv','stock_picks',0,'SE','https://se.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','stock',0,'SE','https://se.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','indices',0,'SE','https://se.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','futures',0,'SE','https://se.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','sv','options',0,'SE','https://se.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','stock_analysis',0,'SE','https://se.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','indices_analysis',0,'SE','https://se.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','futures_analysis',0,'SE','https://se.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','options_analysis',0,'SE','https://se.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities_analysis',0,'SE','https://se.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities_technical',0,'SE','https://se.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities_Fundamental',0,'SE','https://se.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities_opinion',0,'SE','https://se.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities_strategy',0,'SE','https://se.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities_metals',0,'SE','https://se.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities_energy',0,'SE','https://se.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','commodities_agriculture',0,'SE','https://se.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','overview_analysis',0,'SE','https://se.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','overview_technical',0,'SE','https://se.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','overview_fundamental',0,'SE','https://se.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','overview_opinion',0,'SE','https://se.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','overview_investing',0,'SE','https://se.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','sv','crypto_opinion',0,'SE','https://se.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','news',1,'FI','https://fi.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','crypto_news',0,'FI','https://fi.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','forex_news',0,'FI','https://fi.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','popular_news',0,'FI','https://fi.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_news',0,'FI','https://fi.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','stock_news',0,'FI','https://fi.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','economic_indicators_news',0,'FI','https://fi.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','politics_news',0,'FI','https://fi.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','economy_news',0,'FI','https://fi.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','world_news',0,'FI','https://fi.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','world',0,'FI','https://fi.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','finance',0,'FI','https://fi.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','economics',0,'FI','https://fi.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','politics',0,'FI','https://fi.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','popular',0,'FI','https://fi.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','crypto',0,'FI','https://fi.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','forex',0,'FI','https://fi.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','stock',0,'FI','https://fi.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities',0,'FI','https://fi.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','central_bank',0,'FI','https://fi.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','crypto_opinion ',0,'FI','https://fi.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','forex_analysis',0,'FI','https://fi.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','forex_technical',0,'FI','https://fi.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','forex_fundamental',0,'FI','https://fi.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','forex_opinion',0,'FI','https://fi.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','forex_signal',0,'FI','https://fi.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','overview_analysis',0,'FI','https://fi.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','overview_technical',0,'FI','https://fi.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','overview_fundamental',0,'FI','https://fi.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','overview_opinion',0,'FI','https://fi.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','overview_investing',0,'FI','https://fi.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_analysis',0,'FI','https://fi.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_technical',0,'FI','https://fi.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_Fundamental',0,'FI','https://fi.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_opinion',0,'FI','https://fi.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_strategy',0,'FI','https://fi.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_metals',0,'FI','https://fi.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_energy',0,'FI','https://fi.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','commodities_agriculture',0,'FI','https://fi.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','bonds_analysis',0,'FI','https://fi.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','bonds_technical',0,'FI','https://fi.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','bonds_fundamental',0,'FI','https://fi.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','bonds_opinion',0,'FI','https://fi.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','bonds_trategy',0,'FI','https://fi.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','bonds_government',0,'FI','https://fi.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','bonds_corporate',0,'FI','https://fi.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','stock_analysis',0,'FI','https://fi.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','stock_technical',0,'FI','https://fi.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','stock_fundamental',0,'FI','https://fi.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','stock_opinion',0,'FI','https://fi.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fi','stock_picks',0,'FI','https://fi.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','stock',0,'FI','https://fi.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','indices',0,'FI','https://fi.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','futures',0,'FI','https://fi.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fi','options',0,'FI','https://fi.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','stock_analysis',0,'FI','https://fi.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','indices_analysis',0,'FI','https://fi.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','futures_analysis',0,'FI','https://fi.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','options_analysis',0,'FI','https://fi.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities_analysis',0,'FI','https://fi.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities_technical',0,'FI','https://fi.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities_Fundamental',0,'FI','https://fi.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities_opinion',0,'FI','https://fi.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities_strategy',0,'FI','https://fi.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities_metals',0,'FI','https://fi.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities_energy',0,'FI','https://fi.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','commodities_agriculture',0,'FI','https://fi.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','overview_analysis',0,'FI','https://fi.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','overview_technical',0,'FI','https://fi.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','overview_fundamental',0,'FI','https://fi.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','overview_opinion',0,'FI','https://fi.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','overview_investing',0,'FI','https://fi.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fi','crypto_opinion',0,'FI','https://fi.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','news',1,'IL','https://il.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','crypto_news',0,'IL','https://il.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','forex_news',0,'IL','https://il.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','popular_news',0,'IL','https://il.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_news',0,'IL','https://il.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','stock_news',0,'IL','https://il.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','economic_indicators_news',0,'IL','https://il.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','politics_news',0,'IL','https://il.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','economy_news',0,'IL','https://il.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','world_news',0,'IL','https://il.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','world',0,'IL','https://il.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','finance',0,'IL','https://il.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','economics',0,'IL','https://il.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','politics',0,'IL','https://il.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','popular',0,'IL','https://il.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','crypto',0,'IL','https://il.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','forex',0,'IL','https://il.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','stock',0,'IL','https://il.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities',0,'IL','https://il.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','central_bank',0,'IL','https://il.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','crypto_opinion ',0,'IL','https://il.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','forex_analysis',0,'IL','https://il.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','forex_technical',0,'IL','https://il.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','forex_fundamental',0,'IL','https://il.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','forex_opinion',0,'IL','https://il.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','forex_signal',0,'IL','https://il.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','overview_analysis',0,'IL','https://il.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','overview_technical',0,'IL','https://il.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','overview_fundamental',0,'IL','https://il.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','overview_opinion',0,'IL','https://il.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','overview_investing',0,'IL','https://il.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_analysis',0,'IL','https://il.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_technical',0,'IL','https://il.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_Fundamental',0,'IL','https://il.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_opinion',0,'IL','https://il.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_strategy',0,'IL','https://il.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_metals',0,'IL','https://il.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_energy',0,'IL','https://il.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','commodities_agriculture',0,'IL','https://il.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','bonds_analysis',0,'IL','https://il.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','bonds_technical',0,'IL','https://il.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','bonds_fundamental',0,'IL','https://il.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','bonds_opinion',0,'IL','https://il.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','bonds_trategy',0,'IL','https://il.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','bonds_government',0,'IL','https://il.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','bonds_corporate',0,'IL','https://il.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','stock_analysis',0,'IL','https://il.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','stock_technical',0,'IL','https://il.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','stock_fundamental',0,'IL','https://il.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','stock_opinion',0,'IL','https://il.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','he','stock_picks',0,'IL','https://il.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','stock',0,'IL','https://il.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','indices',0,'IL','https://il.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','futures',0,'IL','https://il.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','he','options',0,'IL','https://il.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','stock_analysis',0,'IL','https://il.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','indices_analysis',0,'IL','https://il.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','futures_analysis',0,'IL','https://il.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','options_analysis',0,'IL','https://il.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities_analysis',0,'IL','https://il.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities_technical',0,'IL','https://il.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities_Fundamental',0,'IL','https://il.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities_opinion',0,'IL','https://il.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities_strategy',0,'IL','https://il.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities_metals',0,'IL','https://il.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities_energy',0,'IL','https://il.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','commodities_agriculture',0,'IL','https://il.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','overview_analysis',0,'IL','https://il.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','overview_technical',0,'IL','https://il.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','overview_fundamental',0,'IL','https://il.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','overview_opinion',0,'IL','https://il.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','overview_investing',0,'IL','https://il.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','he','crypto_opinion',0,'IL','https://il.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','news',1,'DE','https://de.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','crypto_news',0,'DE','https://de.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','forex_news',0,'DE','https://de.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','popular_news',0,'DE','https://de.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_news',0,'DE','https://de.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','stock_news',0,'DE','https://de.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','economic_indicators_news',0,'DE','https://de.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','politics_news',0,'DE','https://de.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','economy_news',0,'DE','https://de.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','world_news',0,'DE','https://de.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','world',0,'DE','https://de.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','finance',0,'DE','https://de.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','economics',0,'DE','https://de.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','politics',0,'DE','https://de.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','popular',0,'DE','https://de.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','crypto',0,'DE','https://de.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','forex',0,'DE','https://de.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','stock',0,'DE','https://de.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities',0,'DE','https://de.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','central_bank',0,'DE','https://de.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','crypto_opinion ',0,'DE','https://de.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','forex_analysis',0,'DE','https://de.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','forex_technical',0,'DE','https://de.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','forex_fundamental',0,'DE','https://de.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','forex_opinion',0,'DE','https://de.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','forex_signal',0,'DE','https://de.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','overview_analysis',0,'DE','https://de.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','overview_technical',0,'DE','https://de.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','overview_fundamental',0,'DE','https://de.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','overview_opinion',0,'DE','https://de.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','overview_investing',0,'DE','https://de.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_analysis',0,'DE','https://de.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_technical',0,'DE','https://de.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_Fundamental',0,'DE','https://de.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_opinion',0,'DE','https://de.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_strategy',0,'DE','https://de.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_metals',0,'DE','https://de.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_energy',0,'DE','https://de.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','commodities_agriculture',0,'DE','https://de.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','bonds_analysis',0,'DE','https://de.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','bonds_technical',0,'DE','https://de.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','bonds_fundamental',0,'DE','https://de.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','bonds_opinion',0,'DE','https://de.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','bonds_trategy',0,'DE','https://de.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','bonds_government',0,'DE','https://de.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','bonds_corporate',0,'DE','https://de.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','stock_analysis',0,'DE','https://de.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','stock_technical',0,'DE','https://de.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','stock_fundamental',0,'DE','https://de.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','stock_opinion',0,'DE','https://de.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','de','stock_picks',0,'DE','https://de.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','stock',0,'DE','https://de.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','indices',0,'DE','https://de.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','futures',0,'DE','https://de.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','de','options',0,'DE','https://de.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','stock_analysis',0,'DE','https://de.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','indices_analysis',0,'DE','https://de.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','futures_analysis',0,'DE','https://de.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','options_analysis',0,'DE','https://de.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities_analysis',0,'DE','https://de.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities_technical',0,'DE','https://de.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities_Fundamental',0,'DE','https://de.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities_opinion',0,'DE','https://de.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities_strategy',0,'DE','https://de.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities_metals',0,'DE','https://de.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities_energy',0,'DE','https://de.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','commodities_agriculture',0,'DE','https://de.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','overview_analysis',0,'DE','https://de.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','overview_technical',0,'DE','https://de.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','overview_fundamental',0,'DE','https://de.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','overview_opinion',0,'DE','https://de.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','overview_investing',0,'DE','https://de.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','de','crypto_opinion',0,'DE','https://de.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','news',1,'JP','https://jp.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','crypto_news',0,'JP','https://jp.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','forex_news',0,'JP','https://jp.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','popular_news',0,'JP','https://jp.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_news',0,'JP','https://jp.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','stock_news',0,'JP','https://jp.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','economic_indicators_news',0,'JP','https://jp.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','politics_news',0,'JP','https://jp.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','economy_news',0,'JP','https://jp.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','world_news',0,'JP','https://jp.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','world',0,'JP','https://jp.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','finance',0,'JP','https://jp.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','economics',0,'JP','https://jp.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','politics',0,'JP','https://jp.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','popular',0,'JP','https://jp.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','crypto',0,'JP','https://jp.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','forex',0,'JP','https://jp.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','stock',0,'JP','https://jp.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities',0,'JP','https://jp.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','central_bank',0,'JP','https://jp.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','crypto_opinion ',0,'JP','https://jp.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','forex_analysis',0,'JP','https://jp.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','forex_technical',0,'JP','https://jp.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','forex_fundamental',0,'JP','https://jp.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','forex_opinion',0,'JP','https://jp.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','forex_signal',0,'JP','https://jp.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','overview_analysis',0,'JP','https://jp.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','overview_technical',0,'JP','https://jp.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','overview_fundamental',0,'JP','https://jp.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','overview_opinion',0,'JP','https://jp.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','overview_investing',0,'JP','https://jp.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_analysis',0,'JP','https://jp.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_technical',0,'JP','https://jp.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_Fundamental',0,'JP','https://jp.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_opinion',0,'JP','https://jp.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_strategy',0,'JP','https://jp.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_metals',0,'JP','https://jp.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_energy',0,'JP','https://jp.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','commodities_agriculture',0,'JP','https://jp.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','bonds_analysis',0,'JP','https://jp.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','bonds_technical',0,'JP','https://jp.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','bonds_fundamental',0,'JP','https://jp.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','bonds_opinion',0,'JP','https://jp.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','bonds_trategy',0,'JP','https://jp.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','bonds_government',0,'JP','https://jp.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','bonds_corporate',0,'JP','https://jp.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','stock_analysis',0,'JP','https://jp.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','stock_technical',0,'JP','https://jp.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','stock_fundamental',0,'JP','https://jp.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','stock_opinion',0,'JP','https://jp.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ja','stock_picks',0,'JP','https://jp.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','stock',0,'JP','https://jp.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','indices',0,'JP','https://jp.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','futures',0,'JP','https://jp.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ja','options',0,'JP','https://jp.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','stock_analysis',0,'JP','https://jp.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','indices_analysis',0,'JP','https://jp.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','futures_analysis',0,'JP','https://jp.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','options_analysis',0,'JP','https://jp.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities_analysis',0,'JP','https://jp.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities_technical',0,'JP','https://jp.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities_Fundamental',0,'JP','https://jp.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities_opinion',0,'JP','https://jp.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities_strategy',0,'JP','https://jp.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities_metals',0,'JP','https://jp.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities_energy',0,'JP','https://jp.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','commodities_agriculture',0,'JP','https://jp.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','overview_analysis',0,'JP','https://jp.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','overview_technical',0,'JP','https://jp.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','overview_fundamental',0,'JP','https://jp.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','overview_opinion',0,'JP','https://jp.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','overview_investing',0,'JP','https://jp.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ja','crypto_opinion',0,'JP','https://jp.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','news',1,'FR','https://fr.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','crypto_news',0,'FR','https://fr.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','forex_news',0,'FR','https://fr.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','popular_news',0,'FR','https://fr.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_news',0,'FR','https://fr.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','stock_news',0,'FR','https://fr.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','economic_indicators_news',0,'FR','https://fr.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','politics_news',0,'FR','https://fr.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','economy_news',0,'FR','https://fr.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','world_news',0,'FR','https://fr.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','world',0,'FR','https://fr.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','finance',0,'FR','https://fr.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','economics',0,'FR','https://fr.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','politics',0,'FR','https://fr.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','popular',0,'FR','https://fr.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','crypto',0,'FR','https://fr.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','forex',0,'FR','https://fr.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','stock',0,'FR','https://fr.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities',0,'FR','https://fr.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','central_bank',0,'FR','https://fr.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','crypto_opinion ',0,'FR','https://fr.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','forex_analysis',0,'FR','https://fr.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','forex_technical',0,'FR','https://fr.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','forex_fundamental',0,'FR','https://fr.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','forex_opinion',0,'FR','https://fr.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','forex_signal',0,'FR','https://fr.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','overview_analysis',0,'FR','https://fr.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','overview_technical',0,'FR','https://fr.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','overview_fundamental',0,'FR','https://fr.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','overview_opinion',0,'FR','https://fr.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','overview_investing',0,'FR','https://fr.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_analysis',0,'FR','https://fr.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_technical',0,'FR','https://fr.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_Fundamental',0,'FR','https://fr.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_opinion',0,'FR','https://fr.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_strategy',0,'FR','https://fr.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_metals',0,'FR','https://fr.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_energy',0,'FR','https://fr.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','commodities_agriculture',0,'FR','https://fr.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','bonds_analysis',0,'FR','https://fr.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','bonds_technical',0,'FR','https://fr.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','bonds_fundamental',0,'FR','https://fr.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','bonds_opinion',0,'FR','https://fr.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','bonds_trategy',0,'FR','https://fr.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','bonds_government',0,'FR','https://fr.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','bonds_corporate',0,'FR','https://fr.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','stock_analysis',0,'FR','https://fr.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','stock_technical',0,'FR','https://fr.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','stock_fundamental',0,'FR','https://fr.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','stock_opinion',0,'FR','https://fr.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','fr','stock_picks',0,'FR','https://fr.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','stock',0,'FR','https://fr.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','indices',0,'FR','https://fr.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','futures',0,'FR','https://fr.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','fr','options',0,'FR','https://fr.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','stock_analysis',0,'FR','https://fr.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','indices_analysis',0,'FR','https://fr.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','futures_analysis',0,'FR','https://fr.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','options_analysis',0,'FR','https://fr.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities_analysis',0,'FR','https://fr.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities_technical',0,'FR','https://fr.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities_Fundamental',0,'FR','https://fr.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities_opinion',0,'FR','https://fr.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities_strategy',0,'FR','https://fr.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities_metals',0,'FR','https://fr.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities_energy',0,'FR','https://fr.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','commodities_agriculture',0,'FR','https://fr.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','overview_analysis',0,'FR','https://fr.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','overview_technical',0,'FR','https://fr.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','overview_fundamental',0,'FR','https://fr.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','overview_opinion',0,'FR','https://fr.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','overview_investing',0,'FR','https://fr.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','fr','crypto_opinion',0,'FR','https://fr.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','news',1,'IT','https://it.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','crypto_news',0,'IT','https://it.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','forex_news',0,'IT','https://it.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','popular_news',0,'IT','https://it.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_news',0,'IT','https://it.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','stock_news',0,'IT','https://it.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','economic_indicators_news',0,'IT','https://it.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','politics_news',0,'IT','https://it.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','economy_news',0,'IT','https://it.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','world_news',0,'IT','https://it.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','world',0,'IT','https://it.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','finance',0,'IT','https://it.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','economics',0,'IT','https://it.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','politics',0,'IT','https://it.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','popular',0,'IT','https://it.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','crypto',0,'IT','https://it.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','forex',0,'IT','https://it.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','stock',0,'IT','https://it.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities',0,'IT','https://it.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','central_bank',0,'IT','https://it.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','crypto_opinion ',0,'IT','https://it.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','forex_analysis',0,'IT','https://it.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','forex_technical',0,'IT','https://it.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','forex_fundamental',0,'IT','https://it.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','forex_opinion',0,'IT','https://it.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','forex_signal',0,'IT','https://it.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','overview_analysis',0,'IT','https://it.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','overview_technical',0,'IT','https://it.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','overview_fundamental',0,'IT','https://it.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','overview_opinion',0,'IT','https://it.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','overview_investing',0,'IT','https://it.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_analysis',0,'IT','https://it.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_technical',0,'IT','https://it.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_Fundamental',0,'IT','https://it.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_opinion',0,'IT','https://it.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_strategy',0,'IT','https://it.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_metals',0,'IT','https://it.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_energy',0,'IT','https://it.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','commodities_agriculture',0,'IT','https://it.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','bonds_analysis',0,'IT','https://it.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','bonds_technical',0,'IT','https://it.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','bonds_fundamental',0,'IT','https://it.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','bonds_opinion',0,'IT','https://it.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','bonds_trategy',0,'IT','https://it.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','bonds_government',0,'IT','https://it.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','bonds_corporate',0,'IT','https://it.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','stock_analysis',0,'IT','https://it.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','stock_technical',0,'IT','https://it.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','stock_fundamental',0,'IT','https://it.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','stock_opinion',0,'IT','https://it.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','it','stock_picks',0,'IT','https://it.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','stock',0,'IT','https://it.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','indices',0,'IT','https://it.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','futures',0,'IT','https://it.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','it','options',0,'IT','https://it.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','stock_analysis',0,'IT','https://it.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','indices_analysis',0,'IT','https://it.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','futures_analysis',0,'IT','https://it.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','options_analysis',0,'IT','https://it.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities_analysis',0,'IT','https://it.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities_technical',0,'IT','https://it.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities_Fundamental',0,'IT','https://it.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities_opinion',0,'IT','https://it.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities_strategy',0,'IT','https://it.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities_metals',0,'IT','https://it.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities_energy',0,'IT','https://it.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','commodities_agriculture',0,'IT','https://it.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','overview_analysis',0,'IT','https://it.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','overview_technical',0,'IT','https://it.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','overview_fundamental',0,'IT','https://it.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','overview_opinion',0,'IT','https://it.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','overview_investing',0,'IT','https://it.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','it','crypto_opinion',0,'IT','https://it.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','news',1,'ID','https://id.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','crypto_news',0,'ID','https://id.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','forex_news',0,'ID','https://id.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','popular_news',0,'ID','https://id.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_news',0,'ID','https://id.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','stock_news',0,'ID','https://id.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','economic_indicators_news',0,'ID','https://id.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','politics_news',0,'ID','https://id.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','economy_news',0,'ID','https://id.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','world_news',0,'ID','https://id.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','world',0,'ID','https://id.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','finance',0,'ID','https://id.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','economics',0,'ID','https://id.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','politics',0,'ID','https://id.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','popular',0,'ID','https://id.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','crypto',0,'ID','https://id.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','forex',0,'ID','https://id.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','stock',0,'ID','https://id.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities',0,'ID','https://id.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','central_bank',0,'ID','https://id.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','crypto_opinion ',0,'ID','https://id.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','forex_analysis',0,'ID','https://id.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','forex_technical',0,'ID','https://id.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','forex_fundamental',0,'ID','https://id.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','forex_opinion',0,'ID','https://id.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','forex_signal',0,'ID','https://id.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','overview_analysis',0,'ID','https://id.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','overview_technical',0,'ID','https://id.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','overview_fundamental',0,'ID','https://id.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','overview_opinion',0,'ID','https://id.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','overview_investing',0,'ID','https://id.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_analysis',0,'ID','https://id.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_technical',0,'ID','https://id.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_Fundamental',0,'ID','https://id.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_opinion',0,'ID','https://id.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_strategy',0,'ID','https://id.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_metals',0,'ID','https://id.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_energy',0,'ID','https://id.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','commodities_agriculture',0,'ID','https://id.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','bonds_analysis',0,'ID','https://id.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','bonds_technical',0,'ID','https://id.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','bonds_fundamental',0,'ID','https://id.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','bonds_opinion',0,'ID','https://id.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','bonds_trategy',0,'ID','https://id.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','bonds_government',0,'ID','https://id.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','bonds_corporate',0,'ID','https://id.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','stock_analysis',0,'ID','https://id.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','stock_technical',0,'ID','https://id.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','stock_fundamental',0,'ID','https://id.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','stock_opinion',0,'ID','https://id.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','id','stock_picks',0,'ID','https://id.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','stock',0,'ID','https://id.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','indices',0,'ID','https://id.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','futures',0,'ID','https://id.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','id','options',0,'ID','https://id.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','stock_analysis',0,'ID','https://id.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','indices_analysis',0,'ID','https://id.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','futures_analysis',0,'ID','https://id.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','options_analysis',0,'ID','https://id.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities_analysis',0,'ID','https://id.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities_technical',0,'ID','https://id.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities_Fundamental',0,'ID','https://id.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities_opinion',0,'ID','https://id.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities_strategy',0,'ID','https://id.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities_metals',0,'ID','https://id.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities_energy',0,'ID','https://id.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','commodities_agriculture',0,'ID','https://id.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','overview_analysis',0,'ID','https://id.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','overview_technical',0,'ID','https://id.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','overview_fundamental',0,'ID','https://id.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','overview_opinion',0,'ID','https://id.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','overview_investing',0,'ID','https://id.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','id','crypto_opinion',0,'ID','https://id.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','news',1,'MX','https://mx.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','crypto_news',0,'MX','https://mx.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','forex_news',0,'MX','https://mx.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','popular_news',0,'MX','https://mx.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_news',0,'MX','https://mx.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','stock_news',0,'MX','https://mx.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','economic_indicators_news',0,'MX','https://mx.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','politics_news',0,'MX','https://mx.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','economy_news',0,'MX','https://mx.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','world_news',0,'MX','https://mx.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','world',0,'MX','https://mx.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','finance',0,'MX','https://mx.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','economics',0,'MX','https://mx.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','politics',0,'MX','https://mx.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','popular',0,'MX','https://mx.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','crypto',0,'MX','https://mx.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','forex',0,'MX','https://mx.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','stock',0,'MX','https://mx.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities',0,'MX','https://mx.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','central_bank',0,'MX','https://mx.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','crypto_opinion ',0,'MX','https://mx.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_analysis',0,'MX','https://mx.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_technical',0,'MX','https://mx.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_fundamental',0,'MX','https://mx.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_opinion',0,'MX','https://mx.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_signal',0,'MX','https://mx.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_analysis',0,'MX','https://mx.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_technical',0,'MX','https://mx.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_fundamental',0,'MX','https://mx.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_opinion',0,'MX','https://mx.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_investing',0,'MX','https://mx.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_analysis',0,'MX','https://mx.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_technical',0,'MX','https://mx.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_Fundamental',0,'MX','https://mx.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_opinion',0,'MX','https://mx.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_strategy',0,'MX','https://mx.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_metals',0,'MX','https://mx.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_energy',0,'MX','https://mx.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_agriculture',0,'MX','https://mx.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_analysis',0,'MX','https://mx.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_technical',0,'MX','https://mx.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_fundamental',0,'MX','https://mx.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_opinion',0,'MX','https://mx.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_trategy',0,'MX','https://mx.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_government',0,'MX','https://mx.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_corporate',0,'MX','https://mx.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_analysis',0,'MX','https://mx.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_technical',0,'MX','https://mx.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_fundamental',0,'MX','https://mx.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_opinion',0,'MX','https://mx.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_picks',0,'MX','https://mx.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','stock',0,'MX','https://mx.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','indices',0,'MX','https://mx.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','futures',0,'MX','https://mx.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','options',0,'MX','https://mx.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','stock_analysis',0,'MX','https://mx.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','indices_analysis',0,'MX','https://mx.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','futures_analysis',0,'MX','https://mx.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','options_analysis',0,'MX','https://mx.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_analysis',0,'MX','https://mx.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_technical',0,'MX','https://mx.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_Fundamental',0,'MX','https://mx.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_opinion',0,'MX','https://mx.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_strategy',0,'MX','https://mx.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_metals',0,'MX','https://mx.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_energy',0,'MX','https://mx.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_agriculture',0,'MX','https://mx.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_analysis',0,'MX','https://mx.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_technical',0,'MX','https://mx.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_fundamental',0,'MX','https://mx.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_opinion',0,'MX','https://mx.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_investing',0,'MX','https://mx.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','crypto_opinion',0,'MX','https://mx.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','news',1,'ES','https://es.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','crypto_news',0,'ES','https://es.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','forex_news',0,'ES','https://es.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','popular_news',0,'ES','https://es.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_news',0,'ES','https://es.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','stock_news',0,'ES','https://es.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','economic_indicators_news',0,'ES','https://es.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','politics_news',0,'ES','https://es.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','economy_news',0,'ES','https://es.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','world_news',0,'ES','https://es.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','world',0,'ES','https://es.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','finance',0,'ES','https://es.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','economics',0,'ES','https://es.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','politics',0,'ES','https://es.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','popular',0,'ES','https://es.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','crypto',0,'ES','https://es.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','forex',0,'ES','https://es.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','stock',0,'ES','https://es.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities',0,'ES','https://es.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','central_bank',0,'ES','https://es.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','crypto_opinion ',0,'ES','https://es.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_analysis',0,'ES','https://es.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_technical',0,'ES','https://es.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_fundamental',0,'ES','https://es.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_opinion',0,'ES','https://es.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','forex_signal',0,'ES','https://es.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_analysis',0,'ES','https://es.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_technical',0,'ES','https://es.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_fundamental',0,'ES','https://es.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_opinion',0,'ES','https://es.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','overview_investing',0,'ES','https://es.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_analysis',0,'ES','https://es.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_technical',0,'ES','https://es.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_Fundamental',0,'ES','https://es.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_opinion',0,'ES','https://es.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_strategy',0,'ES','https://es.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_metals',0,'ES','https://es.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_energy',0,'ES','https://es.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','commodities_agriculture',0,'ES','https://es.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_analysis',0,'ES','https://es.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_technical',0,'ES','https://es.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_fundamental',0,'ES','https://es.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_opinion',0,'ES','https://es.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_trategy',0,'ES','https://es.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_government',0,'ES','https://es.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','bonds_corporate',0,'ES','https://es.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_analysis',0,'ES','https://es.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_technical',0,'ES','https://es.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_fundamental',0,'ES','https://es.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_opinion',0,'ES','https://es.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','es','stock_picks',0,'ES','https://es.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','stock',0,'ES','https://es.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','indices',0,'ES','https://es.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','futures',0,'ES','https://es.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','es','options',0,'ES','https://es.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','stock_analysis',0,'ES','https://es.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','indices_analysis',0,'ES','https://es.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','futures_analysis',0,'ES','https://es.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','options_analysis',0,'ES','https://es.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_analysis',0,'ES','https://es.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_technical',0,'ES','https://es.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_Fundamental',0,'ES','https://es.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_opinion',0,'ES','https://es.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_strategy',0,'ES','https://es.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_metals',0,'ES','https://es.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_energy',0,'ES','https://es.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','commodities_agriculture',0,'ES','https://es.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_analysis',0,'ES','https://es.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_technical',0,'ES','https://es.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_fundamental',0,'ES','https://es.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_opinion',0,'ES','https://es.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','overview_investing',0,'ES','https://es.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','es','crypto_opinion',0,'ES','https://es.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','news',1,'MY','https://my.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','crypto_news',0,'MY','https://my.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','forex_news',0,'MY','https://my.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','popular_news',0,'MY','https://my.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_news',0,'MY','https://my.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','stock_news',0,'MY','https://my.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','economic_indicators_news',0,'MY','https://my.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','politics_news',0,'MY','https://my.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','economy_news',0,'MY','https://my.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','world_news',0,'MY','https://my.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','world',0,'MY','https://my.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','finance',0,'MY','https://my.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','economics',0,'MY','https://my.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','politics',0,'MY','https://my.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','popular',0,'MY','https://my.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','crypto',0,'MY','https://my.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','forex',0,'MY','https://my.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','stock',0,'MY','https://my.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities',0,'MY','https://my.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','central_bank',0,'MY','https://my.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','crypto_opinion ',0,'MY','https://my.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','forex_analysis',0,'MY','https://my.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','forex_technical',0,'MY','https://my.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','forex_fundamental',0,'MY','https://my.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','forex_opinion',0,'MY','https://my.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','forex_signal',0,'MY','https://my.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','overview_analysis',0,'MY','https://my.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','overview_technical',0,'MY','https://my.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','overview_fundamental',0,'MY','https://my.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','overview_opinion',0,'MY','https://my.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','overview_investing',0,'MY','https://my.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_analysis',0,'MY','https://my.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_technical',0,'MY','https://my.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_Fundamental',0,'MY','https://my.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_opinion',0,'MY','https://my.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_strategy',0,'MY','https://my.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_metals',0,'MY','https://my.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_energy',0,'MY','https://my.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','commodities_agriculture',0,'MY','https://my.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','bonds_analysis',0,'MY','https://my.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','bonds_technical',0,'MY','https://my.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','bonds_fundamental',0,'MY','https://my.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','bonds_opinion',0,'MY','https://my.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','bonds_trategy',0,'MY','https://my.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','bonds_government',0,'MY','https://my.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','bonds_corporate',0,'MY','https://my.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','stock_analysis',0,'MY','https://my.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','stock_technical',0,'MY','https://my.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','stock_fundamental',0,'MY','https://my.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','stock_opinion',0,'MY','https://my.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','ms','stock_picks',0,'MY','https://my.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','stock',0,'MY','https://my.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','indices',0,'MY','https://my.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','futures',0,'MY','https://my.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','ms','options',0,'MY','https://my.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','stock_analysis',0,'MY','https://my.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','indices_analysis',0,'MY','https://my.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','futures_analysis',0,'MY','https://my.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','options_analysis',0,'MY','https://my.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities_analysis',0,'MY','https://my.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities_technical',0,'MY','https://my.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities_Fundamental',0,'MY','https://my.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities_opinion',0,'MY','https://my.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities_strategy',0,'MY','https://my.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities_metals',0,'MY','https://my.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities_energy',0,'MY','https://my.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','commodities_agriculture',0,'MY','https://my.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','overview_analysis',0,'MY','https://my.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','overview_technical',0,'MY','https://my.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','overview_fundamental',0,'MY','https://my.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','overview_opinion',0,'MY','https://my.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','overview_investing',0,'MY','https://my.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','ms','crypto_opinion',0,'MY','https://my.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','news',1,'CN','https://cn.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','crypto_news',0,'CN','https://cn.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','forex_news',0,'CN','https://cn.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','popular_news',0,'CN','https://cn.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_news',0,'CN','https://cn.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','stock_news',0,'CN','https://cn.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','economic_indicators_news',0,'CN','https://cn.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','politics_news',0,'CN','https://cn.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','economy_news',0,'CN','https://cn.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','world_news',0,'CN','https://cn.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','world',0,'CN','https://cn.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','finance',0,'CN','https://cn.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','economics',0,'CN','https://cn.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','politics',0,'CN','https://cn.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','popular',0,'CN','https://cn.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','crypto',0,'CN','https://cn.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','forex',0,'CN','https://cn.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','stock',0,'CN','https://cn.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities',0,'CN','https://cn.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','central_bank',0,'CN','https://cn.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','crypto_opinion ',0,'CN','https://cn.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','forex_analysis',0,'CN','https://cn.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','forex_technical',0,'CN','https://cn.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','forex_fundamental',0,'CN','https://cn.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','forex_opinion',0,'CN','https://cn.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','forex_signal',0,'CN','https://cn.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','overview_analysis',0,'CN','https://cn.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','overview_technical',0,'CN','https://cn.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','overview_fundamental',0,'CN','https://cn.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','overview_opinion',0,'CN','https://cn.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','overview_investing',0,'CN','https://cn.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_analysis',0,'CN','https://cn.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_technical',0,'CN','https://cn.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_Fundamental',0,'CN','https://cn.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_opinion',0,'CN','https://cn.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_strategy',0,'CN','https://cn.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_metals',0,'CN','https://cn.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_energy',0,'CN','https://cn.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','commodities_agriculture',0,'CN','https://cn.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','bonds_analysis',0,'CN','https://cn.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','bonds_technical',0,'CN','https://cn.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','bonds_fundamental',0,'CN','https://cn.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','bonds_opinion',0,'CN','https://cn.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','bonds_trategy',0,'CN','https://cn.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','bonds_government',0,'CN','https://cn.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','bonds_corporate',0,'CN','https://cn.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','stock_analysis',0,'CN','https://cn.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','stock_technical',0,'CN','https://cn.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','stock_fundamental',0,'CN','https://cn.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','stock_opinion',0,'CN','https://cn.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','zh','stock_picks',0,'CN','https://cn.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','stock',0,'CN','https://cn.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','indices',0,'CN','https://cn.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','futures',0,'CN','https://cn.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','zh','options',0,'CN','https://cn.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','stock_analysis',0,'CN','https://cn.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','indices_analysis',0,'CN','https://cn.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','futures_analysis',0,'CN','https://cn.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','options_analysis',0,'CN','https://cn.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities_analysis',0,'CN','https://cn.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities_technical',0,'CN','https://cn.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities_Fundamental',0,'CN','https://cn.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities_opinion',0,'CN','https://cn.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities_strategy',0,'CN','https://cn.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities_metals',0,'CN','https://cn.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities_energy',0,'CN','https://cn.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','commodities_agriculture',0,'CN','https://cn.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','overview_analysis',0,'CN','https://cn.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','overview_technical',0,'CN','https://cn.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','overview_fundamental',0,'CN','https://cn.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','overview_opinion',0,'CN','https://cn.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','overview_investing',0,'CN','https://cn.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','zh','crypto_opinion',0,'CN','https://cn.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','news',1,'TH','https://th.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','crypto_news',0,'TH','https://th.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','forex_news',0,'TH','https://th.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','popular_news',0,'TH','https://th.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_news',0,'TH','https://th.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','stock_news',0,'TH','https://th.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','economic_indicators_news',0,'TH','https://th.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','politics_news',0,'TH','https://th.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','economy_news',0,'TH','https://th.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','world_news',0,'TH','https://th.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','world',0,'TH','https://th.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','finance',0,'TH','https://th.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','economics',0,'TH','https://th.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','politics',0,'TH','https://th.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','popular',0,'TH','https://th.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','crypto',0,'TH','https://th.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','forex',0,'TH','https://th.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','stock',0,'TH','https://th.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities',0,'TH','https://th.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','central_bank',0,'TH','https://th.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','crypto_opinion ',0,'TH','https://th.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','forex_analysis',0,'TH','https://th.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','forex_technical',0,'TH','https://th.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','forex_fundamental',0,'TH','https://th.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','forex_opinion',0,'TH','https://th.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','forex_signal',0,'TH','https://th.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','overview_analysis',0,'TH','https://th.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','overview_technical',0,'TH','https://th.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','overview_fundamental',0,'TH','https://th.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','overview_opinion',0,'TH','https://th.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','overview_investing',0,'TH','https://th.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_analysis',0,'TH','https://th.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_technical',0,'TH','https://th.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_Fundamental',0,'TH','https://th.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_opinion',0,'TH','https://th.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_strategy',0,'TH','https://th.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_metals',0,'TH','https://th.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_energy',0,'TH','https://th.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','commodities_agriculture',0,'TH','https://th.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','bonds_analysis',0,'TH','https://th.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','bonds_technical',0,'TH','https://th.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','bonds_fundamental',0,'TH','https://th.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','bonds_opinion',0,'TH','https://th.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','bonds_trategy',0,'TH','https://th.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','bonds_government',0,'TH','https://th.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','bonds_corporate',0,'TH','https://th.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','stock_analysis',0,'TH','https://th.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','stock_technical',0,'TH','https://th.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','stock_fundamental',0,'TH','https://th.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','stock_opinion',0,'TH','https://th.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','th','stock_picks',0,'TH','https://th.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','stock',0,'TH','https://th.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','indices',0,'TH','https://th.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','futures',0,'TH','https://th.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','th','options',0,'TH','https://th.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','stock_analysis',0,'TH','https://th.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','indices_analysis',0,'TH','https://th.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','futures_analysis',0,'TH','https://th.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','options_analysis',0,'TH','https://th.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities_analysis',0,'TH','https://th.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities_technical',0,'TH','https://th.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities_Fundamental',0,'TH','https://th.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities_opinion',0,'TH','https://th.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities_strategy',0,'TH','https://th.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities_metals',0,'TH','https://th.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities_energy',0,'TH','https://th.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','commodities_agriculture',0,'TH','https://th.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','overview_analysis',0,'TH','https://th.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','overview_technical',0,'TH','https://th.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','overview_fundamental',0,'TH','https://th.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','overview_opinion',0,'TH','https://th.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','overview_investing',0,'TH','https://th.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','th','crypto_opinion',0,'TH','https://th.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','news',1,'PL','https://pl.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','crypto_news',0,'PL','https://pl.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','forex_news',0,'PL','https://pl.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','popular_news',0,'PL','https://pl.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_news',0,'PL','https://pl.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','stock_news',0,'PL','https://pl.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','economic_indicators_news',0,'PL','https://pl.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','politics_news',0,'PL','https://pl.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','economy_news',0,'PL','https://pl.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','world_news',0,'PL','https://pl.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','world',0,'PL','https://pl.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','finance',0,'PL','https://pl.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','economics',0,'PL','https://pl.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','politics',0,'PL','https://pl.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','popular',0,'PL','https://pl.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','crypto',0,'PL','https://pl.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','forex',0,'PL','https://pl.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','stock',0,'PL','https://pl.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities',0,'PL','https://pl.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','central_bank',0,'PL','https://pl.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','crypto_opinion ',0,'PL','https://pl.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','forex_analysis',0,'PL','https://pl.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','forex_technical',0,'PL','https://pl.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','forex_fundamental',0,'PL','https://pl.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','forex_opinion',0,'PL','https://pl.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','forex_signal',0,'PL','https://pl.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','overview_analysis',0,'PL','https://pl.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','overview_technical',0,'PL','https://pl.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','overview_fundamental',0,'PL','https://pl.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','overview_opinion',0,'PL','https://pl.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','overview_investing',0,'PL','https://pl.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_analysis',0,'PL','https://pl.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_technical',0,'PL','https://pl.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_Fundamental',0,'PL','https://pl.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_opinion',0,'PL','https://pl.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_strategy',0,'PL','https://pl.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_metals',0,'PL','https://pl.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_energy',0,'PL','https://pl.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','commodities_agriculture',0,'PL','https://pl.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','bonds_analysis',0,'PL','https://pl.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','bonds_technical',0,'PL','https://pl.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','bonds_fundamental',0,'PL','https://pl.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','bonds_opinion',0,'PL','https://pl.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','bonds_trategy',0,'PL','https://pl.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','bonds_government',0,'PL','https://pl.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','bonds_corporate',0,'PL','https://pl.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','stock_analysis',0,'PL','https://pl.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','stock_technical',0,'PL','https://pl.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','stock_fundamental',0,'PL','https://pl.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','stock_opinion',0,'PL','https://pl.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','pl','stock_picks',0,'PL','https://pl.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','stock',0,'PL','https://pl.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','indices',0,'PL','https://pl.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','futures',0,'PL','https://pl.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','pl','options',0,'PL','https://pl.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','stock_analysis',0,'PL','https://pl.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','indices_analysis',0,'PL','https://pl.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','futures_analysis',0,'PL','https://pl.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','options_analysis',0,'PL','https://pl.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities_analysis',0,'PL','https://pl.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities_technical',0,'PL','https://pl.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities_Fundamental',0,'PL','https://pl.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities_opinion',0,'PL','https://pl.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities_strategy',0,'PL','https://pl.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities_metals',0,'PL','https://pl.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities_energy',0,'PL','https://pl.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','commodities_agriculture',0,'PL','https://pl.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','overview_analysis',0,'PL','https://pl.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','overview_technical',0,'PL','https://pl.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','overview_fundamental',0,'PL','https://pl.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','overview_opinion',0,'PL','https://pl.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','overview_investing',0,'PL','https://pl.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','pl','crypto_opinion',0,'PL','https://pl.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','news',1,'VN','https://vn.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','crypto_news',0,'VN','https://vn.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','forex_news',0,'VN','https://vn.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','popular_news',0,'VN','https://vn.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_news',0,'VN','https://vn.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','stock_news',0,'VN','https://vn.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','economic_indicators_news',0,'VN','https://vn.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','politics_news',0,'VN','https://vn.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','economy_news',0,'VN','https://vn.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','world_news',0,'VN','https://vn.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','world',0,'VN','https://vn.investing.com/rss/news_287.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','finance',0,'VN','https://vn.investing.com/rss/news_95.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','economics',0,'VN','https://vn.investing.com/rss/news_14.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','politics',0,'VN','https://vn.investing.com/rss/news_289.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','popular',0,'VN','https://vn.investing.com/rss/news_285.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','crypto',0,'VN','https://vn.investing.com/rss/news_301.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','forex',0,'VN','https://vn.investing.com/rss/news_1.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','stock',0,'VN','https://vn.investing.com/rss/news_25.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities',0,'VN','https://vn.investing.com/rss/news_11.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','central_bank',0,'VN','https://vn.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','crypto_opinion ',0,'VN','https://vn.investing.com/rss/302.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','forex_analysis',0,'VN','https://vn.investing.com/rss/forex.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','forex_technical',0,'VN','https://vn.investing.com/rss/forex_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','forex_fundamental',0,'VN','https://vn.investing.com/rss/forex_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','forex_opinion',0,'VN','https://vn.investing.com/rss/forex_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','forex_signal',0,'VN','https://vn.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','overview_analysis',0,'VN','https://vn.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','overview_technical',0,'VN','https://vn.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','overview_fundamental',0,'VN','https://vn.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','overview_opinion',0,'VN','https://vn.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','overview_investing',0,'VN','https://vn.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_analysis',0,'VN','https://vn.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_technical',0,'VN','https://vn.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_Fundamental',0,'VN','https://vn.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_opinion',0,'VN','https://vn.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_strategy',0,'VN','https://vn.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_metals',0,'VN','https://vn.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_energy',0,'VN','https://vn.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','commodities_agriculture',0,'VN','https://vn.investing.com/rss/commodities_Agriculture.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','bonds_analysis',0,'VN','https://vn.investing.com/rss/bonds.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','bonds_technical',0,'VN','https://vn.investing.com/rss/bonds_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','bonds_fundamental',0,'VN','https://vn.investing.com/rss/bonds_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','bonds_opinion',0,'VN','https://vn.investing.com/rss/bonds_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','bonds_trategy',0,'VN','https://vn.investing.com/rss/bonds_Strategy.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','bonds_government',0,'VN','https://vn.investing.com/rss/bonds_Government.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','bonds_corporate',0,'VN','https://vn.investing.com/rss/bonds_Corporate.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','stock_analysis',0,'VN','https://vn.investing.com/rss/stock.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','stock_technical',0,'VN','https://vn.investing.com/rss/stock_Technical.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','stock_fundamental',0,'VN','https://vn.investing.com/rss/stock_Fundamental.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','stock_opinion',0,'VN','https://vn.investing.com/rss/stock_Opinion.rss',2289);
 INSERT INTO rss_main VALUES('investing.com','vi','stock_picks',0,'VN','https://vn.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','stock',0,'VN','https://vn.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','indices',0,'VN','https://vn.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','futures',0,'VN','https://vn.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','vi','options',0,'VN','https://vn.investing.com/rss/stock_Options.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','news',1,'US','https://www.investing.com/rss/news.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_news',0,'US','https://www.investing.com/rss/news_301.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_news',0,'US','https://www.investing.com/rss/news_1.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','popular_news',0,'US','https://www.investing.com/rss/news_285.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_news',0,'US','https://www.investing.com/rss/news_11.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_news',0,'US','https://www.investing.com/rss/news_25.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economic_indicators_news',0,'US','https://www.investing.com/rss/news_95.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','politics_news',0,'US','https://www.investing.com/rss/news_289.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','economy_news',0,'US','https://www.investing.com/rss/news_14.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','world_news',0,'US','https://www.investing.com/rss/news_287.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','central_bank',0,'US','https://www.investing.com/rss/central_banks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','crypto_opinion ',0,'US','https://www.investing.com/rss/302.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_analysis',0,'US','https://www.investing.com/rss/forex.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_technical',0,'US','https://www.investing.com/rss/forex_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_fundamental',0,'US','https://www.investing.com/rss/forex_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_opinion',0,'US','https://www.investing.com/rss/forex_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','forex_signal',0,'US','https://www.investing.com/rss/forex_Signals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_analysis',0,'US','https://www.investing.com/rss/market_overview.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_technical',0,'US','https://www.investing.com/rss/market_overview_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_fundamental',0,'US','https://www.investing.com/rss/market_overview_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_opinion',0,'US','https://www.investing.com/rss/market_overview_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','overview_investing',0,'US','https://www.investing.com/rss/market_overview_investing_ideas.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_analysis',0,'US','https://www.investing.com/rss/commodities.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_technical',0,'US','https://www.investing.com/rss/commodities_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_Fundamental',0,'US','https://www.investing.com/rss/commodities_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_opinion',0,'US','https://www.investing.com/rss/commodities_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_strategy',0,'US','https://www.investing.com/rss/commodities_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_metals',0,'US','https://www.investing.com/rss/commodities_Metals.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_energy',0,'US','https://www.investing.com/rss/commodities_Energy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','commodities_agriculture',0,'US','https://www.investing.com/rss/commodities_Agriculture.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','bonds_analysis',0,'US','https://www.investing.com/rss/bonds.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','bonds_technical',0,'US','https://www.investing.com/rss/bonds_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','bonds_fundamental',0,'US','https://www.investing.com/rss/bonds_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','bonds_opinion',0,'US','https://www.investing.com/rss/bonds_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','bonds_trategy',0,'US','https://www.investing.com/rss/bonds_Strategy.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','bonds_government',0,'US','https://www.investing.com/rss/bonds_Government.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','bonds_corporate',0,'US','https://www.investing.com/rss/bonds_Corporate.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_analysis',0,'US','https://www.investing.com/rss/stock.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_technical',0,'US','https://www.investing.com/rss/stock_Technical.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_fundamental',0,'US','https://www.investing.com/rss/stock_Fundamental.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_opinion',0,'US','https://www.investing.com/rss/stock_Opinion.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock_picks',0,'US','https://www.investing.com/rss/stock_stock_picks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','stock',0,'US','https://www.investing.com/rss/stock_Stocks.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','indices',0,'US','https://www.investing.com/rss/stock_Indices.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','futures',0,'US','https://www.investing.com/rss/stock_Futures.rss',2289);
-INSERT INTO rss_main VALUES('investing.com','en','options',0,'US','https://www.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','stock_analysis',0,'VN','https://vn.investing.com/rss/stock_Stocks.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','indices_analysis',0,'VN','https://vn.investing.com/rss/stock_Indices.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','futures_analysis',0,'VN','https://vn.investing.com/rss/stock_Futures.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','options_analysis',0,'VN','https://vn.investing.com/rss/stock_Options.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities_analysis',0,'VN','https://vn.investing.com/rss/commodities.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities_technical',0,'VN','https://vn.investing.com/rss/commodities_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities_Fundamental',0,'VN','https://vn.investing.com/rss/commodities_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities_opinion',0,'VN','https://vn.investing.com/rss/commodities_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities_strategy',0,'VN','https://vn.investing.com/rss/commodities_Strategy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities_metals',0,'VN','https://vn.investing.com/rss/commodities_Metals.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities_energy',0,'VN','https://vn.investing.com/rss/commodities_Energy.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','commodities_agriculture',0,'VN','https://vn.investing.com/rss/commodities_Agriculture.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','overview_analysis',0,'VN','https://vn.investing.com/rss/market_overview.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','overview_technical',0,'VN','https://vn.investing.com/rss/market_overview_Technical.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','overview_fundamental',0,'VN','https://vn.investing.com/rss/market_overview_Fundamental.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','overview_opinion',0,'VN','https://vn.investing.com/rss/market_overview_Opinion.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','overview_investing',0,'VN','https://vn.investing.com/rss/market_overview_investing_ideas.rss',2289);
+INSERT INTO rss_main VALUES('investing.com','vi','crypto_opinion',0,'VN','https://vn.investing.com/rss/302.rss',2289);
 COMMIT;
```

### Comparing `ejtraderNS-0.0.2/ejtraderNS.egg-info/PKG-INFO` & `ejtraderNS-0.0.3/ejtraderNS.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderNS
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a News Library.
 Home-page: https://ejtraderNS.readthedocs.io/
 Download-URL: https://github.com/ejtraderlabs/ejtraderNS
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/ejtraderLabs/ejtraderNS/issues
@@ -67,102 +67,86 @@
 ```python
 api = ejtraderNS(website = 'nytimes.com', topic = 'politics')
 
 results = api.get_news()
 articles = results['articles']
 ```
 
-There is a limited set of topic that you might find:
+Some websites support multiple countries, such as  [investing.com](https://www.investing.com) or [tradingeconomics.com](https://www.tradingeconomics.com)
 
-``` 'tech', 'news', 'business', 'science', 'finance', 'food', 'politics', 'economics', 'travel', 'entertainment', 'music', 'sport', 'world' ```
+
+In this example, I will demonstrate a website that supports multiple countries,
+ retrieve multiple topics, and convert the data into a pandas dataframe.
 
 
-### some url supports multiple languages
 ```python
 import pandas as pd
-from ejtraderNS import Client, describe_url
+from ejtraderNS import Client
 from datetime import datetime
 
-country_topic = describe_url('investing.com')
-
-# Criando uma lista vazia para armazenar os DataFrames
+url = 'investing.com' # or tradingeconomics.com
+country = 'GB'
+country_topic = ["finance","news","economics"]
 dfs = []
 
-# Iterando pelos países, idiomas e tópicos
-
-    
-for topic in country_topic['topics']:
-    try:
-        api = Client(website="investing.com", topic=topic, country="BR")
-    except:
-        pass
+for topic in country_topic:
+    api = Client(website=url, topic=topic, country=country)
+    getdata = api.get_news()
     print(f"topic: {topic}")
-    
-    try:
-        getdata = api.get_news()
-    except:
-        pass
-    # Coletando os dados
-    
 
-    # Se getdata for None, pule para o próximo tópico
     if getdata is None:
         continue
 
-    # Criando uma lista vazia para armazenar as informações
     data = []
 
-    # Iterando pelos artigos e extraindo as informações relevantes
     for article in getdata['articles']:
-        article_data = {}
-        article_data['topic'] = getdata['topic']
-        article_data['author'] = article['author']
-        article_data['date'] = article['published_parsed'] if article['published_parsed'] else article['published']
-
-        article_data['country'] = getdata['country']
-        article_data['language'] = getdata['language']
-
-        article_data['title'] = article['title']
-        
-        try:
-            article_data['summary'] = article['summary']
-            article_data['url'] = article['link']
-        except:
-            article_data['url'] = None
-            article_data['summary'] = article['title']
-            pass
-        
+        article_data = {
+            'topic': getdata['topic'],
+            'author': article['author'],
+            'date': article['published_parsed'] if article['published_parsed'] else article['published'],
+            'country': getdata['country'],
+            'language': getdata['language'],
+            'title': article['title'],
+            'summary': article.get('summary', article['title'])
+        }
         data.append(article_data)
 
-    # Converter objetos time.struct_time para objetos datetime
-    for item in data:
-        try:
-            item['date'] = datetime(*item['date'][:6])
-        except:
-            pass
-    # Criando o dataframe com as informações extraídas
     df = pd.DataFrame(data)
-    df['date'] = pd.to_datetime(df['date'], utc=True)
-    df.set_index('date', inplace=True)
 
-    # Adicionando o DataFrame atual à lista de DataFrames
+    df['date'] = pd.to_datetime(df['date'].apply(lambda x: datetime(*x[:6]) if isinstance(x, tuple) else x), utc=True, errors='coerce')
+    df.set_index('date', inplace=True)
     dfs.append(df)
 
-# Concatenando todos os DataFrames na lista dfs
 df = pd.concat(dfs)
-
-# Reordenando o índice
 df.sort_index(inplace=True)
 print(df)
 
 ```
+output example:
+
+| topic     | author        | country   | language   | title                                                                            | summary                                                                          |
+|:----------|:--------------|:----------|:-----------|:---------------------------------------------------------------------------------|:---------------------------------------------------------------------------------|
+| finance   | Reuters       | GB        | en         | Italy pushes to limit executive pay in listed state-run firms                    | Italy pushes to limit executive pay in listed state-run firms                    |
+| economics | Reuters       | GB        | en         | UK's Cleverly raises Xinjiang and Taiwan with Chinese vice president             | UK's Cleverly raises Xinjiang and Taiwan with Chinese vice president             |
+| news      | Reuters       | GB        | en         | Ukraine hails return of 45 Azov fighters, Russia says 3 pilots released          | Ukraine hails return of 45 Azov fighters, Russia says 3 pilots released          |
+
+
+
+
+
+There is a limited set of topic that you might find:
+``` 'tech', 'news', 'business', 'science', 'finance', 'food', 'politics', 'economics', 'travel', 'entertainment', 'music', 'sport', 'world' ```
+
+extras topics only for [investing.com](https://www.investing.com)
+
+``` 'crypto', 'forex', 'stock', 'commodities', 'central_bank', 'forex_analysis', 'forex_technical', 'forex_fundamental', 'forex_opinion', 'forex_signal', 'bonds_analysis', 'bonds_technical', 'bonds_fundamental', 'bonds_opinion', 'bonds_strategy', 'bonds_government', 'bonds_corporate', 'stock_analysis', 'stock_technical', 'stock_fundamental', 'stock_opinion', 'stock_picks', 'indices_analysis', 'futures_analysis', 'options_analysis', 'commodities_analysis', 'commodities_technical', 'commodities_Fundamental', 'commodities_opinion', 'commodities_strategy', 'commodities_metals', 'commodities_energy', 'commodities_agriculture', 'overview_analysis', 'overview_technical', 'overview_fundamental', 'overview_opinion', 'overview_investing', 'crypto_opinion'```
+  
+
 
-for investing.com  is a limited set of topic base on country 
 
-``` 'news', 'crypto_news', 'forex_news', 'popular_news', 'commodities_news', 'stock_news', 'economic_indicators_news', 'economy_news', 'central_bank', 'crypto_opinion', 'forex_analysis', 'forex_technical', 'forex_fundamental', 'forex_opinion', 'forex_signal', 'overview_analysis', 'overview_technical', 'overview_fundamental', 'overview_opinion', 'overview_investing', 'commodities_analysis', 'commodities_technical', 'commodities_Fundamental', 'commodities_opinion', 'commodities_strategy', 'commodities_metals', 'commodities_energy', 'commodities_agriculture', 'bonds_analysis', 'bonds_technical', 'bonds_fundamental', 'bonds_opinion', 'bonds_trategy', 'bonds_government', 'bonds_corporate', 'stock_analysis', 'stock_technical', 'stock_fundamental', 'stock_opinion', 'stock_picks', 'stock', 'indices', 'futures', 'options', 'politics_news', 'world_news' ```
 
 However, not all topics are supported by every newspaper.
 
 How to check which topics are supported by which newspaper:
 ```python
 from ejtraderNS import describe_url
 
@@ -274,31 +258,17 @@
 `US`, `GB`, `DE`, `FR`, `IN`, `RU`, `ES`, `BR`, `IT`, `CA`, `AU`, `NL`, `PL`, `NZ`, `PT`, `RO`, `UA`, `JP`, `AR`, `IR`, `IE`, `PH`, `IS`, `ZA`, `AT`, `CL`, `HR`, `BG`, `HU`, `KR`, `SZ`, `AE`, `EG`, `VE`, `CO`, `SE`, `CZ`, `ZH`, `MT`, `AZ`, `GR`, `BE`, `LU`, `IL`, `LT`, `NI`, `MY`, `TR`, `BM`, `NO`, `ME`, `SA`, `RS`, `BA`
 
 Supported languages:
 `EL`, `IT`, `ZH`, `EN`, `RU`, `CS`, `RO`, `FR`, `JA`, `DE`, `PT`, `ES`, `AR`, `HE`, `UK`, `PL`, `NL`, `TR`, `VI`, `KO`, `TH`, `ID`, `HR`, `DA`, `BG`, `NO`, `SK`, `FA`, `ET`, `SV`, `BN`, `GU`, `MK`, `PA`, `HU`, `SL`, `FI`, `LT`, `MR`, `HI`
 
 
 
-
-
 ## Tech/framework used
 The package itself is nothing more than a SQLite database with 
 RSS feed endpoints for each website and some basic wrapper of
 [feedparser](https://pythonhosted.org/feedparser/index.html).
 
 
-## About Us
-We are ejtraderNS API team. We are glad that you liked our package.
-
-If you want to search for any news data, consider using [our API](https://ejtraderNSapi.com/)
-
-![](ejtraderNS_oneliner.png)
-
-
-[Artem Bugara]() - co-founder of ejtraderNS, made v.0.1.0
-
-[Maksym Sugonyaka](https://www.linkedin.com/mwlite/in/msugonyaka) - co-founder of ejtraderNS, made v.0.1.0
+## Acknowledgements
 
-[Becket Trotter](https://www.linkedin.com/in/beckettrotter/) - Python Developer, made v.0.2.0
+I would like to express my gratitude to [@kotartemiy](https://github.com/kotartemiy) for creating the initial project. Their work has been an invaluable starting point for my modifications and improvements.
 
-## Licence
-MIT
```

### Comparing `ejtraderNS-0.0.2/setup.py` & `ejtraderNS-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name='ejtraderNS',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     url='https://ejtraderNS.readthedocs.io/',
     download_url='https://github.com/ejtraderlabs/ejtraderNS',
     license='MIT License',
     author='Emerson Pedroso',
     author_email='support@ejtrader.com',
     description='This is a News Library.',
```

