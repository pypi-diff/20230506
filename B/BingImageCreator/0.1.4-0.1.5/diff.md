# Comparing `tmp/BingImageCreator-0.1.4.tar.gz` & `tmp/BingImageCreator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.1.4.tar", last modified: Sun Apr 30 03:29:37 2023, max compression
+gzip compressed data, was "BingImageCreator-0.1.5.tar", last modified: Sat May  6 04:28:38 2023, max compression
```

## Comparing `BingImageCreator-0.1.4.tar` & `BingImageCreator-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:29:37.427073 BingImageCreator-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-30 03:29:14.000000 BingImageCreator-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-30 03:29:37.427073 BingImageCreator-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-30 03:29:14.000000 BingImageCreator-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 03:29:37.427073 BingImageCreator-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-30 03:29:14.000000 BingImageCreator-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:29:37.423073 BingImageCreator-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 03:29:37.427073 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-30 03:29:37.000000 BingImageCreator-0.1.4/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-04-30 03:29:14.000000 BingImageCreator-0.1.4/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:28:38.788215 BingImageCreator-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/test/test_example.py
```

### Comparing `BingImageCreator-0.1.4/LICENSE` & `BingImageCreator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.1.4/PKG-INFO` & `BingImageCreator-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.1.4
+Version: 0.1.5
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.1.4/README.md` & `BingImageCreator-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.1.4/setup.py` & `BingImageCreator-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.1.4",
+    version="0.1.5",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.1.4/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.1.5/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.1.4
+Version: 0.1.5
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.1.4/src/BingImageCreator.py` & `BingImageCreator-0.1.5/src/BingImageCreator.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 sending_message = "Sending request..."
 wait_message = "Waiting for results..."
 download_message = "\nDownloading images..."
 
 
 def debug(debug_file, text_var):
     """helper function for debug"""
-    with open(f"{debug_file}", "a") as f:
+    with open(f"{debug_file}", "a", encoding="utf-8") as f:
         f.write(str(text_var))
 
 
 class ImageGen:
     """
     Image generation by Microsoft Bing
     Parameters:3
@@ -155,34 +155,35 @@
             if img in bad_images:
                 raise Exception("Bad images")
         # No images
         if not normal_image_links:
             raise Exception(error_no_images)
         return normal_image_links
 
-    def save_images(self, links: list, output_dir: str) -> None:
+    def save_images(self, links: list, output_dir: str,file_name:str=None) -> None:
         """
         Saves images to output directory
         """
         if self.debug_file:
             self.debug(download_message)
         if not self.quiet:
             print(download_message)
         with contextlib.suppress(FileExistsError):
             os.mkdir(output_dir)
         try:
+            fn=f'{file_name}_' if file_name else ''
             jpeg_index = 0
             for link in links:
-                while os.path.exists(os.path.join(output_dir, f"{jpeg_index}.jpeg")):
+                while os.path.exists(os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")):
                     jpeg_index += 1
                 with self.session.get(link, stream=True) as response:
                     # save response to file
                     response.raise_for_status()
                     with open(
-                        os.path.join(output_dir, f"{jpeg_index}.jpeg"), "wb"
+                        os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"), "wb"
                     ) as output_file:
                         for chunk in response.iter_content(chunk_size=8192):
                             output_file.write(chunk)
         except requests.exceptions.MissingSchema as url_exception:
             raise Exception(
                 "Inappropriate contents found in the generated images. Please try again or try another prompt.",
             ) from url_exception
```

