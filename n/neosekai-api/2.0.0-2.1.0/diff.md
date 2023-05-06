# Comparing `tmp/neosekai_api-2.0.0-py3-none-any.whl.zip` & `tmp/neosekai_api-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6667 bytes, number of entries: 10
+Zip file size: 6877 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      221 b- defN 23-May-05 14:54 neosekai_api/__init__.py
--rw-rw-rw-  2.0 fat     2257 b- defN 23-May-05 16:49 neosekai_api/chapter.py
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-05 16:31 neosekai_api/constants.py
+-rw-rw-rw-  2.0 fat     2891 b- defN 23-May-06 02:41 neosekai_api/chapter.py
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-06 02:45 neosekai_api/constants.py
 -rw-rw-rw-  2.0 fat      332 b- defN 23-Apr-20 09:21 neosekai_api/helper.py
 -rw-rw-rw-  2.0 fat     5571 b- defN 23-May-05 16:31 neosekai_api/novel.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3165 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      807 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/RECORD
-10 files, 13568 bytes uncompressed, 5287 bytes compressed:  61.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-06 02:51 neosekai_api-2.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3165 b- defN 23-May-06 02:51 neosekai_api-2.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 02:51 neosekai_api-2.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-May-06 02:51 neosekai_api-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      807 b- defN 23-May-06 02:51 neosekai_api-2.1.0.dist-info/RECORD
+10 files, 14202 bytes uncompressed, 5497 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: neosekai_api/helper.py
 Comment: 
 
 Filename: neosekai_api/novel.py
 Comment: 
 
-Filename: neosekai_api-2.0.0.dist-info/LICENSE
+Filename: neosekai_api-2.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: neosekai_api-2.0.0.dist-info/METADATA
+Filename: neosekai_api-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: neosekai_api-2.0.0.dist-info/WHEEL
+Filename: neosekai_api-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: neosekai_api-2.0.0.dist-info/top_level.txt
+Filename: neosekai_api-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: neosekai_api-2.0.0.dist-info/RECORD
+Filename: neosekai_api-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neosekai_api/chapter.py

```diff
@@ -11,33 +11,40 @@
     :params _url : The Mangadex Chapter URL
     '''
 
     def __init__(self, _url: str) -> None:
         self.url = _url
         self.__response_object = requests.get(self.url, timeout=10)
 
-    def chapter_details(self):
+    def chapter_details(self, name_only=False):
         """
         returns chapter details : 
 
         - chapter volume
         - chapter name
         - url
         - chapter release date
 
         In the given order in JSON format
+        - If option name_only is set to True, the function will only return the name of the chapter
+        - This makes the program much faster as it has to go through a bunch of processes in order to get the other details 
         """
-        novel_url_ = self.url.split('neosekaitranslations.com/novel/')[-1]
-        novel_name = novel_url_[:novel_url_.index('/')]
-        novel_url = f"https://www.neosekaitranslations.com/novel/{novel_name}/"
-        novel = Novel(novel_url)
-        index_page = novel.get_index_page()
-        for i in index_page:
-            if index_page[i]['url'] == self.url:
-                return index_page[i]
+        if not name_only:
+            novel_url_ = self.url.split('neosekaitranslations.com/novel/')[-1]
+            novel_name = novel_url_[:novel_url_.index('/')]
+            novel_url = f"https://www.neosekaitranslations.com/novel/{novel_name}/"
+            novel = Novel(novel_url)
+            index_page = novel.get_index_page()
+            for i in index_page:
+                if index_page[i]['url'] == self.url:
+                    return index_page[i]
+        else:
+            soup = BeautifulSoup(self.__response_object.content, 'lxml')
+            heading = soup.find('li', attrs={'class': ['active']})
+            return heading.text.strip()
 
     def get_chapter_content(self, fancy=True):
         """
         returns main chapter content in JSON format
 
         JSON format:
         ```json
@@ -64,7 +71,10 @@
                 n += 1
             elif i.img != None:
                 content[str(n)] = {'type': 'img', 'content': i.img['src']}
                 n += 1
             else:
                 continue
         return content
+
+
+print(NovelChapter('https://www.neosekaitranslations.com/novel/transfer-student/chapter-114/').chapter_details(name_only=True))
```

## neosekai_api/constants.py

```diff
@@ -1 +1 @@
-VERSION = '2.0.0'
+VERSION = '2.1.0'
```

## Comparing `neosekai_api-2.0.0.dist-info/LICENSE` & `neosekai_api-2.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `neosekai_api-2.0.0.dist-info/METADATA` & `neosekai_api-2.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosekai-api
-Version: 2.0.0
+Version: 2.1.0
 Summary: An Unoffical Python API for neosekaitranslations.com
 Home-page: https://github.com/john-erinjery/neosekai-api/
 Author: John Erinjery
 Author-email: jancyvinod415@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
```

