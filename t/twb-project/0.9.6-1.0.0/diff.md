# Comparing `tmp/twb_project-0.9.6.tar.gz` & `tmp/twb_project-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.9.6.tar", max compression
+gzip compressed data, was "twb_project-1.0.0.tar", max compression
```

## Comparing `twb_project-0.9.6.tar` & `twb_project-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.6/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.6/README.md
--rw-r--r--   0        0        0      760 2023-05-05 14:20:12.789097 twb_project-0.9.6/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.6/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.6/twb/bip.py
--rw-r--r--   0        0        0    20020 2023-05-05 03:07:36.078433 twb_project-0.9.6/twb/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.6/twb/builder_helpers.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.6/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.6/twb/downloader.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.6/twb/logger.py
--rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-0.9.6/twb/logger_init.py
--rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.6/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.6/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.6/twb/reader.py
--rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.6/twb/utils.py
--rw-r--r--   0        0        0     5877 2023-05-05 14:17:57.836997 twb_project-0.9.6/twb/warehouse.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.6/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-1.0.0/README.md
+-rw-r--r--   0        0        0      760 2023-05-06 15:59:06.172123 twb_project-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-1.0.0/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-1.0.0/twb/bip.py
+-rw-r--r--   0        0        0    20033 2023-05-06 15:57:13.965716 twb_project-1.0.0/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-1.0.0/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-1.0.0/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-1.0.0/twb/downloader.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-1.0.0/twb/logger.py
+-rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-1.0.0/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-1.0.0/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-1.0.0/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-1.0.0/twb/reader.py
+-rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-1.0.0/twb/utils.py
+-rw-r--r--   0        0        0     5878 2023-05-05 14:46:34.743706 twb_project-1.0.0/twb/warehouse.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-1.0.0/setup.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-1.0.0/PKG-INFO
```

### Comparing `twb_project-0.9.6/LICENSE` & `twb_project-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/README.md` & `twb_project-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/pyproject.toml` & `twb_project-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.9.6"
+version = "1.0.0"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.9.6/twb/bip.py` & `twb_project-1.0.0/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/builder.py` & `twb_project-1.0.0/twb/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,16 +86,16 @@
 
         logging.debug(f'Decompressing [{archive_filename}]...')
 
         with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
             start_time = time.time()
             z.extractall(path=decompressed_dir_path)
             end_time = time.time()
-            execution_duration = end_time - start_time
-            logging.debug(f'Decompression took {execution_duration:.2f} seconds. ({archive_filename})')
+            execution_duration = (end_time - start_time) / 60
+            logging.debug(f'Decompression took {execution_duration:.2f} min. ({archive_filename})')
         decompressed_files = get_file_list(decompressed_dir_path)
 
         return decompressed_files
 
     def _process_executor(self, xml_path: str) -> List[str]:
         """
         Process the file.
@@ -482,11 +482,11 @@
 
         logging.info(f'Cleanup loop finished.')
 
         # Clean up the global temporary directory.
         cleanup_dir(global_temp_dir)
 
         end_time = time.time()
-        execution_duration = end_time - start_time
+        execution_duration = (end_time - start_time) / 60
 
         # Log the end of the task.
-        logging.info(f'All done! Finished all files. (took {execution_duration:.2f}s in total)')
+        logging.info(f'All done! Finished all files. (took {execution_duration:.2f} min in total)')
```

### Comparing `twb_project-0.9.6/twb/decompressor.py` & `twb_project-1.0.0/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/downloader.py` & `twb_project-1.0.0/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/logger.py` & `twb_project-1.0.0/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/logger_init.py` & `twb_project-1.0.0/twb/logger_init.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/modifier.py` & `twb_project-1.0.0/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/parallelization.py` & `twb_project-1.0.0/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/reader.py` & `twb_project-1.0.0/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/utils.py` & `twb_project-1.0.0/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.6/twb/warehouse.py` & `twb_project-1.0.0/twb/warehouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class Warehouse:
     def __init__(self,
                  output_dir: str,
                  prefix: str = 'warehouse_',
                  suffix: str = '',
-                 max_size: int = 8,
+                 max_size: int = 12,
                  compress: bool = True):
         self.output_dir = output_dir
         self.prefix = prefix
         self.suffix = suffix
         self.max_size = max_size
         self.compress = compress
```

### Comparing `twb_project-0.9.6/setup.py` & `twb_project-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.9.6',
+    'version': '1.0.0',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.9.6/PKG-INFO` & `twb_project-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.9.6
+Version: 1.0.0
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

