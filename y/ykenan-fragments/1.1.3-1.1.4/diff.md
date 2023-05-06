# Comparing `tmp/ykenan_fragments-1.1.3.tar.gz` & `tmp/ykenan_fragments-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.1.3.tar", last modified: Sat May  6 12:04:18 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.1.4.tar", last modified: Sat May  6 12:18:38 2023, max compression
```

## Comparing `ykenan_fragments-1.1.3.tar` & `ykenan_fragments-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 12:04:18.153938 ykenan_fragments-1.1.3/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      964 2023-05-06 12:04:18.153938 ykenan_fragments-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.3/README.md
--rw-rw-rw-   0        0        0      773 2023-05-06 12:02:03.000000 ykenan_fragments-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 12:04:18.154938 ykenan_fragments-1.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 12:04:18.123938 ykenan_fragments-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 12:04:18.139937 ykenan_fragments-1.1.3/src/ykenan_fragments/
--rw-rw-rw-   0        0        0    33745 2023-05-06 12:02:47.000000 ykenan_fragments-1.1.3/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     3185 2023-05-06 09:16:51.000000 ykenan_fragments-1.1.3/src/ykenan_fragments/genome_transformation.py
-drwxrwxrwx   0        0        0        0 2023-05-06 12:04:18.152938 ykenan_fragments-1.1.3/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      964 2023-05-06 12:04:18.000000 ykenan_fragments-1.1.3/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-05-06 12:04:18.000000 ykenan_fragments-1.1.3/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 12:04:18.000000 ykenan_fragments-1.1.3/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-06 12:04:18.000000 ykenan_fragments-1.1.3/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-06 12:04:18.000000 ykenan_fragments-1.1.3/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 12:18:38.368108 ykenan_fragments-1.1.4/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      964 2023-05-06 12:18:38.368108 ykenan_fragments-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.4/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-06 12:17:34.000000 ykenan_fragments-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 12:18:38.368108 ykenan_fragments-1.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 12:18:38.323107 ykenan_fragments-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 12:18:38.353109 ykenan_fragments-1.1.4/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0    32828 2023-05-06 12:16:37.000000 ykenan_fragments-1.1.4/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     3185 2023-05-06 09:16:51.000000 ykenan_fragments-1.1.4/src/ykenan_fragments/genome_transformation.py
+drwxrwxrwx   0        0        0        0 2023-05-06 12:18:38.366107 ykenan_fragments-1.1.4/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      964 2023-05-06 12:18:38.000000 ykenan_fragments-1.1.4/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-05-06 12:18:38.000000 ykenan_fragments-1.1.4/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 12:18:38.000000 ykenan_fragments-1.1.4/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-06 12:18:38.000000 ykenan_fragments-1.1.4/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 12:18:38.000000 ykenan_fragments-1.1.4/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.1.3/LICENSE` & `ykenan_fragments-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.1.3/PKG-INFO` & `ykenan_fragments-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.1.3
+Version: 1.1.4
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.1.3/pyproject.toml` & `ykenan_fragments-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.1.3/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.1.4/src/ykenan_fragments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import TextIO
 
 import pandas as pd
 from pandas import DataFrame
 from ykenan_log import Logger
 import ykenan_file as yf
 import gzip
-import threading
 from multiprocessing.dummy import Pool
 
 from ykenan_fragments.genome_transformation import Hg19ToHg38
 
 
 class GetFragments:
 
@@ -37,21 +36,14 @@
         self.barcodes_key: str = "barcodes"
         self.mtx_key: str = "mtx"
         self.peaks_key: str = "peaks"
         # Extract files and remove suffix information
         self.endswith_list: list = [".cell_barcodes.txt.gz", ".mtx.gz", ".peaks.txt.gz"]
         self.suffix_fragments: str = ".tsv"
         self.suffix_information: str = ".txt"
-        # 写入文件中的信息
-        # Judge comment information
-        self.mtx_start: int = 0
-        # Read quantity
-        self.mtx_count: int = 0
-        self.error_count: int = 0
-        self.mtx_all_number: int = 0
         # start processing
         self.exec_fragments()
 
     def handler_source_files(self) -> dict:
         # Obtain gz file information
         files: list = self.file.get_files(self.base_path)
         gz_files: list = []
@@ -214,107 +206,87 @@
 
     def fragments_file_name(self, key: str) -> str:
         return f"{key}{self.suffix_fragments}"
 
     def information_file_name(self, key: str) -> str:
         return f"{key}{self.suffix_information}"
 
-    def write_fragments_file(self, write: TextIO, line: str, peaks_len: int, barcodes_len: int, peaks_dict: dict, barcodes_dict: dict) -> None:
-        if self.mtx_count >= 500000 and self.mtx_count % 500000 == 0:
-            if self.mtx_all_number != 0:
-                self.log.info(f"Processed {self.mtx_count} lines, completed {round(self.mtx_count / self.mtx_all_number, 4) * 100} %")
-            else:
-                self.log.info(f"Processed {self.mtx_count} lines")
-        split: list = line.split(" ")
-        # To determine the removal of a length of not 3
-        if len(split) != 3:
-            self.mtx_count += 1
-            self.error_count += 1
-            self.log.error(f"mtx information ===> content: {split}, line number: {self.mtx_count}")
-            return
-        if int(split[0]) > peaks_len or int(split[1]) > barcodes_len:
-            self.mtx_count += 1
-            self.error_count += 1
-            return
-        # peak, barcode, There is a header+1, but the index starts from 0 and the record starts from 1
-        peak: str = peaks_dict[int(split[0])]
-        barcode: str = barcodes_dict[int(split[1])]
-        peak_split = peak.split("_")
-        barcode_split = barcode.split("\t")
-        # Adding information, it was found that some files in mtx contain two columns, less than three columns. This line was ignored and recorded in the log
-        try:
-            write.write(f"{peak_split[0]}\t{peak_split[1]}\t{peak_split[2]}\t{barcode_split[6]}\t{split[2]}\n")
-        except Exception as e:
-            self.error_count += 1
-            self.log.error(f"peak information: {peak_split}")
-            self.log.error(f"barcodes file information: {barcode}")
-            self.log.error(f"barcodes information: {barcode_split}")
-            self.log.error(f"mtx information ===> content: {split}, line number: {self.mtx_count}")
-            self.log.error(f"Write error: {e}")
-        self.mtx_count += 1
-
-    def write_fragments(self, param: tuple) -> None:
+    def write_fragments(self, path: str, key: str) -> None:
         """
         Form fragments file
         :return:
         """
-        path: str = param[0]
-        key: str = param[1]
-        self.log.info(f"Process {key} related files (folders)")
         # Obtain file information
         files: dict = self.get_files(path)
         # Get Barcodes
         self.log.info(f"Getting {self.barcodes_key} file information")
         barcodes: list = self.get_file_content(path, files[self.barcodes_key])
         self.log.info(f"Getting {self.mtx_key} file path")
         mtx_path: str = self.get_file_content(path, files[self.mtx_key])
         self.log.info(f"Getting {self.peaks_key} file information")
         peaks: list = self.get_file_content(path, files[self.peaks_key])
-        # 形成字典
-        barcodes_dict: dict = {}
-        barcodes_i: int = 0
-        for barcode_elem in barcodes:
-            barcodes_dict.update({barcodes_i: barcode_elem})
-            barcodes_i += 1
-        peaks_dict: dict = {}
-        peaks_i: int = 0
-        for peak_elem in peaks:
-            peaks_dict.update({peaks_i: peak_elem})
-            peaks_i += 1
         # length
         barcodes_len: int = len(barcodes)
         peaks_len: int = len(peaks)
         if barcodes_len < 2 or peaks_len < 2:
             self.log.error(f"Insufficient file read length {self.barcodes_key}: {barcodes_len}, {self.peaks_key}: {peaks_len}")
             raise ValueError("Insufficient file read length")
         self.log.info(f"Quantity or Path {self.barcodes_key}: {barcodes_len}, {self.mtx_key}: {mtx_path}, {self.peaks_key}: {peaks_len}")
-
+        # Read quantity
+        mtx_count: int = 0
+        error_count: int = 0
+        mtx_all_number: int = 0
         # create a file
         fragments_file: str = os.path.join(path, self.fragments_file_name(key))
         self.log.info(f"Starting to form {mtx_path} fragments file")
         with open(fragments_file, "w", encoding="utf-8", buffering=1, newline="\n") as w:
             with open(mtx_path, "r", encoding="utf-8") as r:
                 line: str = r.readline().strip()
                 if line.startswith("%"):
                     self.log.info(f"Annotation Information: {line}")
                 line: str = r.readline().strip()
                 split: list = line.split(" ")
                 if len(split) == 3 and line:
                     self.log.info(f"Remove Statistical Rows: {line}")
-                    self.mtx_all_number = int(split[2])
+                    mtx_all_number = int(split[2])
                     if int(split[0]) + 1 != peaks_len and int(split[1]) + 1 != barcodes_len:
                         raise ValueError(f"File mismatch {self.peaks_key}: {int(split[0])} {peaks_len}, {self.barcodes_key}: {int(split[1])} {barcodes_len}")
                 while True:
                     line: str = r.readline().strip()
                     if not line:
                         break
-                    # 此处用多线程作用不大
-                    threading.Thread(target=self.write_fragments_file, args=(w, line, peaks_len, barcodes_len, peaks_dict, barcodes_dict)).start()
-
-        self.log.info(f"The number of rows ignored is {self.error_count}, {round(self.error_count / self.mtx_all_number, 4) * 100} % of total")
+                    if mtx_count >= 500000 and mtx_count % 500000 == 0:
+                        self.log.info(f"Processed {mtx_count} lines, completed {round(mtx_count / mtx_all_number, 4) * 100} %")
+                    split: list = line.split(" ")
+                    # To determine the removal of a length of not 3
+                    if len(split) != 3:
+                        mtx_count += 1
+                        error_count += 1
+                        self.log.error(f"mtx information ===> content: {split}, line number: {mtx_count}")
+                        continue
+                    if int(split[0]) > peaks_len or int(split[1]) > barcodes_len:
+                        mtx_count += 1
+                        continue
+                    # peak, barcode, There is a header+1, but the index starts from 0 and the record starts from 1
+                    peak: str = peaks[int(split[0])]
+                    barcode: str = barcodes[int(split[1])]
+                    peak_split = peak.split("_")
+                    barcode_split = barcode.split("\t")
+                    # Adding information, it was found that some files in mtx contain two columns, less than three columns. This line was ignored and recorded in the log
+                    try:
+                        w.write(f"{peak_split[0]}\t{peak_split[1]}\t{peak_split[2]}\t{barcode_split[6]}\t{split[2]}\n")
+                    except Exception as e:
+                        error_count += 1
+                        self.log.error(f"peak information: {peak_split}")
+                        self.log.error(f"barcodes file information: {barcode}")
+                        self.log.error(f"barcodes information: {barcode_split}")
+                        self.log.error(f"mtx information ===> content: {split}, line number: {mtx_count}")
+                        self.log.error(f"Write error: {e}")
+                    mtx_count += 1
+        self.log.info(f"The number of rows ignored is {error_count}, {round(error_count / mtx_all_number, 4) * 100} % of total")
         self.log.info(f"Complete the formation of {mtx_path} fragments file")
         self.log.info(f"Complete processing of {key} related files (folders)")
 
     def copy_file(self, source_file: str, target_file: str) -> None:
         if os.path.exists(target_file):
             self.log.warn(f"{target_file} The file already exists, it has been copied by default")
         else:
```

### Comparing `ykenan_fragments-1.1.3/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.1.4/src/ykenan_fragments/genome_transformation.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.1.3/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.1.4/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.1.3
+Version: 1.1.4
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

