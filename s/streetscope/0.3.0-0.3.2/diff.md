# Comparing `tmp/streetscope-0.3.0.tar.gz` & `tmp/streetscope-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetscope-0.3.0.tar", max compression
+gzip compressed data, was "streetscope-0.3.2.tar", max compression
```

## Comparing `streetscope-0.3.0.tar` & `streetscope-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.0/LICENSE
--rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.0/README.md
--rw-r--r--   0        0        0      655 2023-05-05 09:07:24.973706 streetscope-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.0/src/streetscope/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.0/src/streetscope/cv/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.0/src/streetscope/cv/segmentation/__init__.py
--rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.0/src/streetscope/cv/segmentation/segmentation.py
--rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.0/src/streetscope/download/__init__.py
--rw-r--r--   0        0        0    11032 2023-05-04 13:54:48.068866 streetscope-0.3.0/src/streetscope/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.0/src/streetscope/download/utils/UserAgent.csv
--rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.0/src/streetscope/download/utils/__init__.py
--rw-r--r--   0        0        0     5049 2023-05-02 14:00:58.512937 streetscope-0.3.0/src/streetscope/download/utils/geoprocess.py
--rw-r--r--   0        0        0     3553 2023-04-12 01:50:02.108635 streetscope-0.3.0/src/streetscope/download/utils/get_pids.py
--rw-r--r--   0        0        0     6788 2023-04-12 02:06:17.157691 streetscope-0.3.0/src/streetscope/download/utils/imtool.py
--rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.0/src/streetscope/streetscope.py
--rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.0/src/streetscope/transform/__init__.py
--rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.0/src/streetscope/transform/transform_image.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.2/LICENSE
+-rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.2/README.md
+-rw-r--r--   0        0        0      655 2023-05-06 01:02:17.921343 streetscope-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.2/src/streetscope/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.2/src/streetscope/cv/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.2/src/streetscope/cv/segmentation/__init__.py
+-rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.2/src/streetscope/cv/segmentation/segmentation.py
+-rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.2/src/streetscope/download/__init__.py
+-rw-r--r--   0        0        0    10738 2023-05-05 22:57:18.657057 streetscope-0.3.2/src/streetscope/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.2/src/streetscope/download/utils/UserAgent.csv
+-rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.2/src/streetscope/download/utils/__init__.py
+-rw-r--r--   0        0        0     5048 2023-05-05 13:59:33.549883 streetscope-0.3.2/src/streetscope/download/utils/geoprocess.py
+-rw-r--r--   0        0        0     3553 2023-04-12 01:50:02.108635 streetscope-0.3.2/src/streetscope/download/utils/get_pids.py
+-rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.2/src/streetscope/download/utils/imtool.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.2/src/streetscope/streetscope.py
+-rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.2/src/streetscope/transform/__init__.py
+-rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.2/src/streetscope/transform/transform_image.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.2/PKG-INFO
```

### Comparing `streetscope-0.3.0/LICENSE` & `streetscope-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.0/README.md` & `streetscope-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.0/pyproject.toml` & `streetscope-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "streetscope"
-version = "0.3.0"
+version = "0.3.2"
 description = "This package handles downloading, cleaning, analyzing street view imagery"
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Pillow = ">=8.3.2,<9.6"
 geopandas = "^0.9.0"
 geopy = "^2.2.0"
 numpy = "^1.21.2"
 opencv_python = "^4.5.3"
 osmnx = "^1.1.1"
 pandas = "^1.3.3"
-requests = "^2.26.0"
+requests = "^2.30.0"
 setuptools = "^58.0.4"
 Shapely = "^1.7.1"
 torch = "^2.0.0"
 tqdm = "^4.62.2"
 transformers = "^4.10.2"
 scipy = "^1.7.1"
```

### Comparing `streetscope-0.3.0/src/streetscope/cv/segmentation/segmentation.py` & `streetscope-0.3.2/src/streetscope/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.0/src/streetscope/download/streetview_downloader.py` & `streetscope-0.3.2/src/streetscope/download/streetview_downloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 from tqdm import tqdm
 
 from streetscope.download.utils.imtool import ImageTool
 from streetscope.download.utils.get_pids import panoids
 from streetscope.download.utils.geoprocess import GeoProcessor
 
 class StreetViewDownloader:
-    def __init__(self, gsv_api_key = None, log_path = None, nthreads = 5):
+    def __init__(self, gsv_api_key = None, log_path = None, nthreads = 5, distance = 1):
         if gsv_api_key == None:
             warnings.warn("Please provide your Google Street View API key to augment metadata.")
         self._gsv_api_key = gsv_api_key
         self._log_path = log_path
         self._nthreads = nthreads
+        self._distance = distance
         self._user_agent = self._get_ua()
 
     @property
     def gsv_api_key(self):
         return self._gsv_api_key    
     @gsv_api_key.setter
     def gsv_api_key(self,gsv_api_key):
@@ -43,14 +44,21 @@
     def nthreads(self):
         return self._nthreads    
     @nthreads.setter
     def nthreads(self,nthreads):
         self._nthreads = nthreads
     
     @property
+    def distance(self):
+        return self._distance    
+    @distance.setter
+    def distance(self,distance):
+        self._distance = distance
+    
+    @property
     def user_agent(self):
         return self._user_agent  
     
     def _get_ua(self):
         user_agent_file = pkg_resources.resource_filename('streetscope.download.utils', 'UserAgent.csv')
         UA = []
         with open(user_agent_file, 'r') as f:
@@ -167,15 +175,15 @@
         def worker(row):
             input_longitude = row['longitude']
             input_latitude = row['latitude']
             return (input_longitude, input_latitude), get_street_view_info(input_longitude, input_latitude)
 
         # read shapefile
         gdf = gpd.read_file(input_shp_file)
-        gp = GeoProcessor(gdf)
+        gp = GeoProcessor(gdf, distance=self.distance)
         df = gp.get_lat_lon()
         results = []
 
         with ThreadPoolExecutor() as executor:
             futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in df.iterrows()}
             for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids", ncols=100):
                 (input_longitude, input_latitude), row_results = future.result()
@@ -215,48 +223,32 @@
         # If path_pid is None, call get_pids function first
         if path_pid is None:
             print("Getting pids...")
             path_pid = os.path.join(self.dir_output, "pids.csv")
             self.get_pids(path_pid, lat=lat, lng=lng,
                         input_csv_file=input_csv_file, input_shp_file = input_shp_file, closest=closest, disp=disp, augment_metadata=augment_metadata)
 
-        # Import tool
-        tool = ImageTool()
         # Horizontal Google Street View tiles
         # zoom 3: (8, 4); zoom 5: (26, 13) zoom 2: (4, 2) zoom 1: (2, 1);4:(8,16)
         # zoom = 2
         # h_tiles = 4  # 26
         # v_tiles = 2  # 13
         # cropped = False
         # full = True
         # create a folder within self.dir_output
         panorama_output = os.path.join(self.dir_output, "panorama")
         os.makedirs(panorama_output, exist_ok=True)
         
         panoids = self._read_pids(path_pid)
         panoids_rest = self._check_already(panoids)
 
-        # random.shuffle(panoids_rest)
-        task_pids, errors, img_num = [], 0, 0
+        panoids = self._read_pids(path_pid)
+        panoids_rest = self._check_already(panoids)
 
-        for i in range(len(panoids_rest)):
-            if i%self.nthreads != 0 or i == 0:
-                task_pids.append(panoids_rest[i])
-            else:
-                UAs = random.sample(self.user_agent, self.nthreads)
-                try:
-                    tool.dwl_multiple(task_pids, task_pids, self.nthreads, zoom, v_tiles, h_tiles, panorama_output, UAs, cropped, full)
-                    img_num += self.nthreads
-                    print(datetime.datetime.now(), "Task:", i, "/ ", len(panoids_rest),"got:",img_num, "errors:", errors, self.dir_output)
-
-                except Exception as e:
-                    print(e)
-                    time.sleep(random.randint(1, 5)*0.1)
-                    errors += self.nthreads
-                    if self.log_path != None:
-                        self._log_write(task_pids)
-                task_pids = []
+        UAs = random.choices(self.user_agent, k = len(panoids_rest))
+        ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, panorama_output, UAs, cropped, full, log_path=self.log_path)
                 
 if __name__ == "__main__":
     sv_downloader = StreetViewDownloader(gsv_api_key="AIzaSyDjIBLaZ-nAWq0RIoOUQUOzCLYzMYAN2aQ", log_path = "/Users/koichiito/Downloads/Delft/log.txt")
-    # sv_downloader.download_gsv(input_shp_file = "/Users/koichiito/Downloads/Delft/Delft.shp", augment_metadata=True)
-    sv_downloader.download_gsv("/Users/koichiito/Downloads/Delft", lat = 52.004400, lng = 4.342597, augment_metadata=True)
+    sv_downloader.download_gsv("/Volumes/exfat_archi/streetscope_test/delft/images", path_pid = "/Volumes/exfat_archi/streetscope_test/delft/images/pids.csv",
+                            input_shp_file = "/Volumes/exfat_archi/streetscope_test/delft/Delft/Delft.shp", augment_metadata=True)
+    # sv_downloader.download_gsv("/Users/koichiito/Downloads/Delft", lat = 52.004400, lng = 4.342597, augment_metadata=True)
```

### Comparing `streetscope-0.3.0/src/streetscope/download/utils/UserAgent.csv` & `streetscope-0.3.2/src/streetscope/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.0/src/streetscope/download/utils/geoprocess.py` & `streetscope-0.3.2/src/streetscope/download/utils/geoprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 from shapely.geometry import LineString
 from tqdm.auto import tqdm
 import math
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed
 
 class GeoProcessor:
-    def __init__(self, gdf, distance=20):
+    def __init__(self, gdf, distance=1):
         self.gdf = gdf
         self.distance = distance
         self.processing_functions = {
             'Point': self.process_point,
             'MultiPoint': self.process_multipoint,
             'LineString': self.process_linestring,
             'MultiLineString': self.process_multilinestring,
```

### Comparing `streetscope-0.3.0/src/streetscope/download/utils/get_pids.py` & `streetscope-0.3.2/src/streetscope/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.0/src/streetscope/download/utils/imtool.py` & `streetscope-0.3.2/src/streetscope/download/utils/imtool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 import requests
 from PIL import Image
-from concurrent import futures
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import ThreadPoolExecutor, as_completed
 import numpy as np
+from tqdm import tqdm
 
 class ImageTool():
 
     @staticmethod
     def concat_horizontally(im1, im2):
         """
         Description of concat_horizontally
@@ -127,57 +127,89 @@
         # if cropped:
         #     first_slice.crop((0, 0, size[1], size[1])).save(f'{name}_p1.jpg')
         #     first_slice.crop((size[1], 0, size[0], size[1])).save(f'{name}_p2.jpg')
         
         return identif
 
     @staticmethod
-    def dwl_multiple(panoids, identifiers, nthreads, zoom, v_tiles, h_tiles, out_path, uas, cropped=True, full=False):
+    def dwl_multiple(panoids, zoom, v_tiles, h_tiles, out_path, uas, cropped=True, full=False):
         """
-        Description of get_and_save_image
+
+        """
+
+        if not os.path.exists(out_path):
+            os.makedirs(out_path)
+
+        with ThreadPoolExecutor(max_workers=len(uas)) as executor:
+            jobs = []
+            for pano, ua in zip(panoids, uas):
+                kw = {
+                    "pano_id": pano,
+                    "identif": pano,
+                    "ua": ua,
+                    "zoom": zoom,
+                    "vertical_tiles": v_tiles,
+                    "horizontal_tiles": h_tiles,
+                    "out_path": out_path,
+                    "cropped": cropped,
+                    "full": full
+                }
+                jobs.append(executor.submit(ImageTool.get_and_save_image, **kw))
+
+            for job in tqdm(as_completed(jobs), total=len(jobs), desc="Downloading images"):
+                job.result()
+
+    @staticmethod
+    def dwl_multiple(panoids, zoom, v_tiles, h_tiles, out_path, uas, cropped=True, full=False, log_path=None):
+        """
+        Description of dwl_multiple
         
         Calls the get_and_save_image function using multiple threads.
         
         Args:
             panoids (undefined): GSV anorama id
-            identifiers (undefined): custom identifier
-            nthreads (undefined): number of threads
             zoom (undefined):    image resolution
             v_tiles (undefined): number of vertical tiles
             h_tiles (undefined): number of horizontal tiles
             out_path (undefined): output path
             cropped=False (undefined): set True if the image split horizontally in half is needed
             full=True (undefined): set to True if the full image is needed
-
+            log_path=None (undefined): path to a log file
         """
-        
+
         if not os.path.exists(out_path):
             os.makedirs(out_path)
-            
-        workers_range = nthreads
 
-        with ThreadPoolExecutor(max_workers = workers_range) as executor:
+        errors = 0
 
-            jobs = []
-            results_done = []
-            for pano, identif, ua in zip(panoids, identifiers, uas):
+        def log_error(panoid):
+            nonlocal log_path
+            if log_path is not None:
+                with open(log_path, 'a') as log_file:
+                    log_file.write(f"{panoid}\n")
 
+        with ThreadPoolExecutor(max_workers=len(uas)) as executor:
+            jobs = []
+            for pano, ua in tqdm(zip(panoids, uas), total=len(panoids), desc="Preparing & downloading images"):
                 kw = {
-                    "pano_id" : pano, 
-                    "identif" : identif,
+                    "pano_id": pano,
+                    "identif": pano,
                     "ua": ua,
-                    "zoom" : zoom,
-                    "vertical_tiles" : v_tiles, 
-                    "horizontal_tiles" : h_tiles,
-                    "out_path" : out_path,
-                    "cropped" : cropped,
-                    "full" : full
+                    "zoom": zoom,
+                    "vertical_tiles": v_tiles,
+                    "horizontal_tiles": h_tiles,
+                    "out_path": out_path,
+                    "cropped": cropped,
+                    "full": full
                 }
-                
                 jobs.append(executor.submit(ImageTool.get_and_save_image, **kw))
 
+            for job in tqdm(as_completed(jobs), total=len(jobs), desc="Downloading images"):
+                try:
+                    job.result()
+                except Exception as e:
+                    print(e)
+                    errors += 1
+                    failed_panoid = panoids[jobs.index(job)]
+                    log_error(failed_panoid)
 
-            for job in futures.as_completed(jobs):
-                result_done = job.result()
-                results_done.append(result_done)
-
-
+        print("Total images downloaded:", len(jobs) - errors, "Errors:", errors)
```

### Comparing `streetscope-0.3.0/src/streetscope/transform/transform_image.py` & `streetscope-0.3.2/src/streetscope/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.0/PKG-INFO` & `streetscope-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetscope
-Version: 0.3.0
+Version: 0.3.2
 Summary: This package handles downloading, cleaning, analyzing street view imagery
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,15 +14,15 @@
 Requires-Dist: Shapely (>=1.7.1,<2.0.0)
 Requires-Dist: geopandas (>=0.9.0,<0.10.0)
 Requires-Dist: geopy (>=2.2.0,<3.0.0)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: opencv_python (>=4.5.3,<5.0.0)
 Requires-Dist: osmnx (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
 Requires-Dist: setuptools (>=58.0.4,<59.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.62.2,<5.0.0)
 Requires-Dist: transformers (>=4.10.2,<5.0.0)
 Description-Content-Type: text/markdown
```

