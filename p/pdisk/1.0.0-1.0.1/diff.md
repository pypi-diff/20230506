# Comparing `tmp/pdisk-1.0.0.tar.gz` & `tmp/pdisk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdisk-1.0.0.tar", last modified: Sat May  6 18:59:07 2023, max compression
+gzip compressed data, was "pdisk-1.0.1.tar", last modified: Sat May  6 20:17:17 2023, max compression
```

## Comparing `pdisk-1.0.0.tar` & `pdisk-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:59:07.222379 pdisk-1.0.0/
--rw-rw-rw-   0        0        0     2591 2023-05-06 18:59:07.172238 pdisk-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1911 2023-05-06 18:40:29.000000 pdisk-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 18:59:07.093927 pdisk-1.0.0/pdisk/
--rw-rw-rw-   0        0        0       26 2023-05-06 15:56:36.000000 pdisk-1.0.0/pdisk/__init__.py
--rw-rw-rw-   0        0        0    11386 2023-05-06 18:19:45.000000 pdisk-1.0.0/pdisk/pdisk.py
--rw-rw-rw-   0        0        0     2540 2023-05-06 18:03:15.000000 pdisk-1.0.0/pdisk/type.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:59:07.156744 pdisk-1.0.0/pdisk.egg-info/
--rw-rw-rw-   0        0        0     2591 2023-05-06 18:59:06.000000 pdisk-1.0.0/pdisk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-06 18:59:06.000000 pdisk-1.0.0/pdisk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:59:06.000000 pdisk-1.0.0/pdisk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 18:59:06.000000 pdisk-1.0.0/pdisk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 18:59:06.000000 pdisk-1.0.0/pdisk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 18:59:07.222379 pdisk-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1097 2023-05-06 18:56:51.000000 pdisk-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 20:17:17.221432 pdisk-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-06 19:48:25.000000 pdisk-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2614 2023-05-06 20:17:17.217911 pdisk-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4295 2023-05-06 19:48:25.000000 pdisk-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 20:17:17.079201 pdisk-1.0.1/pdisk/
+-rw-rw-rw-   0        0        0       26 2023-05-06 15:56:36.000000 pdisk-1.0.1/pdisk/__init__.py
+-rw-rw-rw-   0        0        0    11319 2023-05-06 19:57:54.000000 pdisk-1.0.1/pdisk/pdisk.py
+-rw-rw-rw-   0        0        0     2540 2023-05-06 18:03:15.000000 pdisk-1.0.1/pdisk/type.py
+drwxrwxrwx   0        0        0        0 2023-05-06 20:17:17.213192 pdisk-1.0.1/pdisk.egg-info/
+-rw-rw-rw-   0        0        0     2614 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 20:17:16.000000 pdisk-1.0.1/pdisk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 20:17:17.223085 pdisk-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2023-05-06 20:16:55.000000 pdisk-1.0.1/setup.py
```

### Comparing `pdisk-1.0.0/PKG-INFO` & `pdisk-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pdisk
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Unofficial Asynchronous Python version of pdisk API wrapper
 Home-page: https://github.com/kalanakt/pdisk
 Author: kalanakt
 Author-email: kalanakt@uvew.xyz
 License: MIT
 Keywords: python,pdisk,earn money 
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # PDisk.pro API Wrapper
 >A Python package to interact with the unofficial API of PDisk.pro.
 
 
 ## Installation
```

### Comparing `pdisk-1.0.0/pdisk/pdisk.py` & `pdisk-1.0.1/pdisk/pdisk.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,28 +121,28 @@
         if response.status_code != 200:
             raise Exception(f"Failed to retrieve file list: {response.text}")
 
         data = response.json()
         if data["msg"] != "OK":
             raise Exception(f"Failed to retrieve file list: {data['msg']}")
 
-        files = []
-        for file_data in data["result"]["files"]:
-            files.append(File(
+        return [
+            File(
                 file_data["name"],
                 file_data["file_code"],
                 file_data["downloads"],
                 file_data["thumbnail"],
                 file_data["public"],
                 file_data["size"],
                 file_data["link"],
                 file_data["fld_id"],
-                file_data["uploaded"]
-            ))
-        return files
+                file_data["uploaded"],
+            )
+            for file_data in data["result"]["files"]
+        ]
     
     async def rename_file(self, file_code: str, new_name: str) -> bool:
         isLink = await self.is_pdisk_link(file_code)
         if isLink:
             file_code = await self.extract_file_code(file_code)
 
         url = f"{self.__base_url}/file/rename?key={self.__api_key}&file_code={file_code}&name={new_name}"
@@ -224,14 +224,12 @@
         if data["status"] != 200:
             raise Exception(f"Failed to rename folder: {data['msg']}")
         return data["result"] == "true"
 
     @staticmethod
     async def is_pdisk_link(link:str) -> bool:
         domain = urlparse(link).netloc
-        if 'pdisk.pro' in domain:
-            return True
-        return False
+        return 'pdisk.pro' in domain
     
     @staticmethod
     async def extract_file_code(link:str) -> bool:
         return link.replace('https://pdisk.pro/', '')
```

### Comparing `pdisk-1.0.0/pdisk/type.py` & `pdisk-1.0.1/pdisk/type.py`

 * *Files identical despite different names*

### Comparing `pdisk-1.0.0/pdisk.egg-info/PKG-INFO` & `pdisk-1.0.1/pdisk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pdisk
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Unofficial Asynchronous Python version of pdisk API wrapper
 Home-page: https://github.com/kalanakt/pdisk
 Author: kalanakt
 Author-email: kalanakt@uvew.xyz
 License: MIT
 Keywords: python,pdisk,earn money 
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # PDisk.pro API Wrapper
 >A Python package to interact with the unofficial API of PDisk.pro.
 
 
 ## Installation
```

### Comparing `pdisk-1.0.0/setup.py` & `pdisk-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "package.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'An Unofficial Asynchronous Python version of pdisk API wrapper'
 
 # Setting up
 setup(
     name="pdisk",
     version=VERSION,
     author="kalanakt",
     license="MIT",
     author_email="kalanakt@uvew.xyz",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['requests', 'urllib'],
+    install_requires=['requests'],
     url="https://github.com/kalanakt/pdisk",
     keywords=['python', 'pdisk', 'earn money '],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

