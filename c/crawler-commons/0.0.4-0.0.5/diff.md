# Comparing `tmp/crawler_commons-0.0.4.tar.gz` & `tmp/crawler_commons-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawler_commons-0.0.4.tar", last modified: Sat May  6 07:43:01 2023, max compression
+gzip compressed data, was "crawler_commons-0.0.5.tar", last modified: Sat May  6 07:54:50 2023, max compression
```

## Comparing `crawler_commons-0.0.4.tar` & `crawler_commons-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:43:01.564264 crawler_commons-0.0.4/
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.4/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:43:01.564069 crawler_commons-0.0.4/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.4/README.md
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:43:01.562845 crawler_commons-0.0.4/crawapi/
--rw-r--r--   0 nezah      (501) staff       (20)     2541 2023-05-06 07:42:57.000000 crawler_commons-0.0.4/crawapi/__init__.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:43:01.563509 crawler_commons-0.0.4/crawler_commons.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:43:01.000000 crawler_commons-0.0.4/crawler_commons.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      250 2023-05-06 07:43:01.000000 crawler_commons-0.0.4/crawler_commons.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-06 07:43:01.000000 crawler_commons-0.0.4/crawler_commons.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-06 07:43:01.000000 crawler_commons-0.0.4/crawler_commons.egg-info/top_level.txt
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:43:01.563846 crawler_commons-0.0.4/crawlutils/
--rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.4/crawlutils/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.4/crawlutils/text_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-06 07:43:01.564319 crawler_commons-0.0.4/setup.cfg
--rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-06 07:42:57.000000 crawler_commons-0.0.4/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:54:50.939345 crawler_commons-0.0.5/
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.5/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:54:50.939059 crawler_commons-0.0.5/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.5/README.md
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:54:50.937340 crawler_commons-0.0.5/crawapi/
+-rw-r--r--   0 nezah      (501) staff       (20)     2634 2023-05-06 07:54:17.000000 crawler_commons-0.0.5/crawapi/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:54:50.938221 crawler_commons-0.0.5/crawler_commons.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/crawler_commons.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      250 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/crawler_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/crawler_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/crawler_commons.egg-info/top_level.txt
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:54:50.938590 crawler_commons-0.0.5/crawlutils/
+-rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.5/crawlutils/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.5/crawlutils/text_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-06 07:54:50.939414 crawler_commons-0.0.5/setup.cfg
+-rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-06 07:54:50.000000 crawler_commons-0.0.5/setup.py
```

### Comparing `crawler_commons-0.0.4/LICENSE` & `crawler_commons-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.4/crawapi/__init__.py` & `crawler_commons-0.0.5/crawapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         cp_soup = BeautifulSoup(cp_r.text, 'html.parser')
 
         price, mc, total_stock_count = -1, 0, 0
 
         try:
             price = int(cp_soup.findAll('dd')[3].text.split(' ')[1].replace(',', ''))
             mc = make_num_include_zo(cp_soup.findAll('em', id='_market_sum')[0].text)
-            total_stock_count = int(make_num(cp_soup.find("th", text="상장주식수").parent.find("td").text))
+            total_stock_count = int(make_num(cp_soup.find("th", string="상장주식수").parent.find("td").text))
             logger.debug(f"total_stock_count : {total_stock_count}")
         except Exception as ex:
             logger.exception(ex)
 
         data = {
             "market_cap": mc,
             "current_price": price,
@@ -56,28 +56,28 @@
 
         if mc != 0:
             self.cache.hset(f"marketcap_{code}", data )
             logger.debug(f"set cache for code {code} - {data}")
 
         return data
 
-    def get_cur_price(self, code):
-        mc, price = self.get_stock_info(code=code)
-        return price
-
-    def get_market_cap(self, code):
-        mc, price = self.get_stock_info(code=code)
-        return mc
+    def get_cur_price(self, code) -> int:
+        d = self.get_stock_info(code=code)
+        return d.get("current_price")
+
+    def get_market_cap(self, code) -> int:
+        d = self.get_stock_info(code=code)
+        return d.get("market_cap")
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.DEBUG, format='[%(levelname)s] > %(message)s')
     naver = NaverWeb(cache=None)
 
     mc = naver.get_market_cap(code="000660")
     logger.info(mc)
 
     price = naver.get_cur_price(code="000660")
     logger.info(price)
 
-    mc, price = naver.get_stock_info(code="000660")
-    logger.info(f"market cap : {mc}, price : {price}")
+    d = naver.get_stock_info(code="000660")
+    logger.info(f"market cap : {mc}, price : {d.get('current_price')}, total_stock_count : {d.get('total_stock_count')}")
```

### Comparing `crawler_commons-0.0.4/crawlutils/__init__.py` & `crawler_commons-0.0.5/crawlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.4/crawlutils/text_utils.py` & `crawler_commons-0.0.5/crawlutils/text_utils.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.4/setup.py` & `crawler_commons-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="crawler_commons",
-    version="0.0.4",
+    version="0.0.5",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="crawler commons",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/crawler_commons",
     packages=setuptools.find_packages(exclude=("test",)),
```

