# Comparing `tmp/ykenan_fragments-1.0.1.tar.gz` & `tmp/ykenan_fragments-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.0.1.tar", last modified: Fri Apr 28 00:59:02 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.1.0.tar", last modified: Sat May  6 07:01:54 2023, max compression
```

## Comparing `ykenan_fragments-1.0.1.tar` & `ykenan_fragments-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 00:59:02.050022 ykenan_fragments-1.0.1/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      964 2023-04-28 00:59:02.050022 ykenan_fragments-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.0.1/README.md
--rw-rw-rw-   0        0        0      773 2023-04-28 00:53:12.000000 ykenan_fragments-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 00:59:02.051025 ykenan_fragments-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 00:59:02.027023 ykenan_fragments-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 00:59:02.038024 ykenan_fragments-1.0.1/src/ykenan_fragments/
--rw-rw-rw-   0        0        0    26955 2023-04-28 00:53:12.000000 ykenan_fragments-1.0.1/src/ykenan_fragments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:59:02.048023 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      964 2023-04-28 00:59:01.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-04-28 00:59:02.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 00:59:01.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-28 00:59:01.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-28 00:59:02.000000 ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 07:01:54.444533 ykenan_fragments-1.1.0/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      964 2023-05-06 07:01:54.444533 ykenan_fragments-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-21 11:53:38.000000 ykenan_fragments-1.1.0/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-06 06:57:01.000000 ykenan_fragments-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-04-21 09:37:07.000000 ykenan_fragments-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:01:54.444533 ykenan_fragments-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 07:01:54.427533 ykenan_fragments-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 07:01:54.431534 ykenan_fragments-1.1.0/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0    32202 2023-05-06 06:53:55.000000 ykenan_fragments-1.1.0/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     2597 2023-05-06 04:53:34.000000 ykenan_fragments-1.1.0/src/ykenan_fragments/genome_transformation.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:01:54.442533 ykenan_fragments-1.1.0/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      964 2023-05-06 07:01:54.000000 ykenan_fragments-1.1.0/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-05-06 07:01:54.000000 ykenan_fragments-1.1.0/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:01:54.000000 ykenan_fragments-1.1.0/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-06 07:01:54.000000 ykenan_fragments-1.1.0/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-06 07:01:54.000000 ykenan_fragments-1.1.0/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.0.1/LICENSE` & `ykenan_fragments-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.0.1/PKG-INFO` & `ykenan_fragments-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.0.1
+Version: 1.1.0
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.0.1/pyproject.toml` & `ykenan_fragments-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.0.1/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.1.0/src/ykenan_fragments/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,31 +8,33 @@
 
 import pandas as pd
 from pandas import DataFrame
 from ykenan_log import Logger
 import ykenan_file as yf
 import gzip
 
+from ykenan_fragments.genome_transformation import Hg19ToHg38
+
 
 class GetFragments:
 
-    def __init__(self, base_path: str, cp_path: str, GSE: str):
+    def __init__(self, base_path: str, cp_path: str, gsm: str):
         """
         Form an unordered fragments
         :param base_path: Path to store three files
         :param cp_path: Path to generate unordered fragments files
-        :param GSE: GSE number (here is a folder name)
+        :param gsm: GSE number (here is a folder name)
         """
         self.log = Logger("Three files form fragments file", "log/fragments.log")
         self.file = yf.staticMethod(log_file="log")
         # Folder path containing three files
-        self.GSE: str = GSE
-        self.base_path: str = os.path.join(base_path, GSE)
+        self.GSE: str = gsm
+        self.base_path: str = os.path.join(base_path, gsm)
         # The path to copy the fragments file to
-        self.cp_path: str = os.path.join(cp_path, GSE)
+        self.cp_path: str = os.path.join(cp_path, gsm)
         # keyword
         self.barcodes_key: str = "barcodes"
         self.mtx_key: str = "mtx"
         self.peaks_key: str = "peaks"
         # Extract files and remove suffix information
         self.endswith_list: list = [".cell_barcodes.txt.gz", ".mtx.gz", ".peaks.txt.gz"]
         self.suffix_fragments: str = ".tsv"
@@ -101,28 +103,28 @@
         # Determine if the folder contains three files
         self.log.info(f"Filter folder information under {self.base_path} path")
         for dir_name in dirs_name:
             get_files = self.file.get_files(dirs_dict[dir_name])
             if len(get_files) < 3:
                 continue
             count: int = 0
-            isAdd: bool = True
+            is_add: bool = True
             for file in get_files:
                 # Determine if there are folders that have already formed fragments
                 if dir_name + self.suffix_fragments == file or dir_name + self.suffix_information == file:
                     self.log.info(f"{dir_name} The fragments file has been generated")
                     self.log.warn(f"Skip generation of {dir_name} type fragments file")
-                    isAdd = False
+                    is_add = False
                     break
                 # Does it contain three
                 for endswith in self.endswith_list:
                     if dir_name + endswith == file:
                         count += 1
                         break
-            if count == 3 and isAdd:
+            if count == 3 and is_add:
                 dirs_key.append(dir_name)
                 dirs_key_dict = dict(itertools.chain(dirs_key_dict.items(), {
                     dir_name: dirs_dict[dir_name]
                 }.items()))
         return {
             "all": {
                 "key": dirs_name,
@@ -340,35 +342,40 @@
             self.log.info(f"Start copying files to the specified path for {key}")
             self.cp_files(all_infor_paths[key], key)
             self.log.info(f"Copy file to specified path for {key} completed")
 
 
 class GetChrSortFragments:
 
-    def __init__(self, path: str, cp_path: str, GSE: str, get_fragments_path: str, is_exec: bool = True):
+    def __init__(self, path: str, cp_path: str, gsm: str, get_fragments_path: str, lift_over_path: str, is_hg19_to_hg38: bool = True, is_exec: bool = True):
         """
         Form an fragments
         :param path: Path to store unordered fragments files
         :param cp_path: Path to generate fragments files
-        :param GSE: GSE number (here is a folder name)
+        :param gsm: GSE number (here is a folder name)
         :param get_fragments_path: base_path parameter in GetFragments class
+        :param is_hg19_to_hg38: 是否为 hg19 文件
         :param is_exec: Do you want to execute the GetFragments class
         """
         self.log = Logger("Three files form fragments file", "log/fragments.log")
         self.file = yf.staticMethod(log_file="log")
-        self.base_path: str = os.path.join(path, GSE)
+        self.base_path: str = os.path.join(path, gsm)
         self.fragments_path: str = os.path.join(self.base_path, "fragments")
         self.cp_input_path: str = cp_path
+        self.lift_over_path: str = lift_over_path
+        self.is_hg19_to_hg38: bool = is_hg19_to_hg38
+        self.genome_source: str = "hg19" if self.is_hg19_to_hg38 else "hg38"
+        self.genome_generate: str = "hg38" if self.is_hg19_to_hg38 else "hg19"
         self.chr_list: dict = {
             "chr1": 1, "chr2": 2, "chr3": 3, "chr4": 4, "chr5": 5, "chr6": 6, "chr7": 7, "chr8": 8, "chr9": 9, "chr10": 10,
             "chr11": 11, "chr12": 12, "chr13": 13, "chr14": 14, "chr15": 15, "chr16": 16, "chr17": 17, "chr18": 18, "chr19": 19, "chr20": 20,
             "chr21": 21, "chr22": 22, "chrX": 23, "chrY": 24
         }
         if is_exec:
-            GetFragments(get_fragments_path, path, GSE)
+            GetFragments(base_path=get_fragments_path, cp_path=path, gsm=gsm)
         self.exec_sort_fragments()
 
     @staticmethod
     def classification_name(chromosome: str, path: str, name: str):
         # Do not use any methods under os.path for path operations here, as looping will slow down several times
         # splitext_name = os.path.splitext(name)[0]
         # splitext_name_suffix = os.path.splitext(name)[1]
@@ -387,17 +394,17 @@
         need_handler_fragments_path: dict = {}
         if not os.path.exists(self.cp_input_path):
             self.log.info(f"create folder {self.cp_input_path}")
             os.makedirs(self.cp_input_path)
         # Add processing files
         for file in files_dict_name:
             # 排序后的文件
-            ArchR_fragments_file: str = os.path.join(self.cp_input_path, file)
-            if os.path.exists(ArchR_fragments_file):
-                self.log.warn(f"The fragments file {ArchR_fragments_file} sorted by chromatin already exists")
+            archr_fragments_file: str = os.path.join(self.cp_input_path, file)
+            if os.path.exists(archr_fragments_file):
+                self.log.warn(f"The fragments file {archr_fragments_file} sorted by chromatin already exists")
                 continue
             # 添加信息
             need_handler_fragments.append(file)
             need_handler_fragments_path = dict(itertools.chain(need_handler_fragments_path.items(), {
                 file: files_dict[file]
             }.items()))
         return {
@@ -409,20 +416,20 @@
         # 读取数量
         fragments_count: int = 0
         # error_count: int = 0
         chr_f_list: list = []
         chr_f_dict: dict = {}
         chr_f_path: dict = {}
         # Determine whether to merge directly
-        isMerge: bool = True
+        is_merge: bool = True
         # Create a folder to store chromatin
-        chromosome_path: str = os.path.join(self.fragments_path, f"{file}_chromosome")
+        chromosome_path: str = os.path.join(self.fragments_path, f"{file}_chromosome", self.genome_source)
         if not os.path.exists(chromosome_path):
             self.log.info(f"create folder {chromosome_path}")
-            isMerge = False
+            is_merge = False
             os.makedirs(chromosome_path)
         with open(path, "r", encoding="utf-8") as r:
             while True:
                 line: str = r.readline().strip()
                 if not line:
                     break
                 if fragments_count >= 500000 and fragments_count % 500000 == 0:
@@ -431,15 +438,15 @@
                 # To determine if an error stop occurs when the length is not 5
                 # if len(split) != 5:
                 #     fragments_count += 1
                 #     error_count += 1
                 #     log.error(f"fragments file error line ===> content: {split}, line number: {fragments_count}")
                 #     raise ValueError(f"fragments file error line ===> content: {split}, line number: {fragments_count}")
                 chromosome: str = split[0]
-                if not isMerge:
+                if not is_merge:
                     chromosome_path_file: str = self.classification_name(chromosome, chromosome_path, file)
                     # Do not judge os. path. exists in this area, as the speed will decrease by 50 times when the number of cycles exceeds 500000
                     # if chromosome not in chr_f_list and not os.path.exists(chromosome_path_file):
                     if chromosome not in chr_f_list:
                         chr_f_list.append(chromosome)
                         chr_f = open(chromosome_path_file, "w", encoding="utf-8", newline="\n", buffering=1)
                         chr_f_dict = dict(itertools.chain(chr_f_dict.items(), {
@@ -456,39 +463,40 @@
                     if chromosome not in chr_f_list:
                         chr_f_list.append(chromosome)
                         chr_f_path = dict(itertools.chain(chr_f_path.items(), {
                             chromosome: chromosome_path_file
                         }.items()))
                 fragments_count += 1
         # 关闭文件
-        if not isMerge:
+        if not is_merge:
             for chromosome in chr_f_list:
                 chromosome_file: TextIO = chr_f_dict[chromosome]
                 chromosome_file.close()
         return {
             "name": chr_f_list,
-            "path": chr_f_path
+            "path": chr_f_path,
+            "base_path": os.path.join(self.fragments_path, f"{file}_chromosome")
         }
 
     def sort_position_files(self, chr_file_dict: dict, file: str):
         chr_name: list = chr_file_dict["name"]
         file_dict_path: dict = chr_file_dict["path"]
         position_f_path: dict = {}
         # sort
         chr_name.sort(key=lambda elem: self.chr_list[elem])
         # Determine whether to merge directly
-        isMerge: bool = True
+        is_merge: bool = True
         # output file
         position: str = os.path.join(self.fragments_path, f"{file}_position")
         if not os.path.exists(position):
             self.log.info(f"create folder {position}")
-            isMerge = False
+            is_merge = False
             os.makedirs(position)
 
-        if not isMerge:
+        if not is_merge:
             for chr_ in chr_name:
                 self.log.info(f"Start sorting file {file_dict_path[chr_]} Sort")
                 chr_file_content: DataFrame = pd.read_table(file_dict_path[chr_], encoding="utf-8", header=None)
                 # 进行排序
                 chr_file_content.sort_values(1, inplace=True)
                 position_file: str = os.path.join(position, f"{file}_{chr_}.tsv")
                 chr_file_content.to_csv(position_file, sep="\t", encoding="utf-8", header=False, index=False)
@@ -503,14 +511,45 @@
                     chr_: position_file
                 }.items()))
         return {
             "name": chr_name,
             "path": position_f_path
         }
 
+    def genome_transformation(self, chr_file_dict: dict, file: str):
+        chr_name: list = chr_file_dict["name"]
+        chr_name.sort(key=lambda elem: self.chr_list[elem])
+        base_path: str = chr_file_dict["base_path"]
+        genome_f_path: dict = {}
+        # Determine whether to merge directly
+        is_merge: bool = True
+        # output file
+        genome_output: str = os.path.join(self.base_path, self.genome_generate)
+        if not os.path.exists(genome_output):
+            self.log.info(f"create folder {genome_output}")
+            is_merge = False
+            os.makedirs(genome_output)
+
+        if not is_merge:
+            # 执行信息
+            Hg19ToHg38(path=base_path, lift_over_path=self.lift_over_path, is_hg19_to_hg38=self.is_hg19_to_hg38)
+
+        for chr_ in chr_name:
+            genome_file: str = os.path.join(genome_output, f"{file}_{chr_}.tsv")
+            genome_f_path = dict(itertools.chain(genome_f_path.items(), {
+                chr_: genome_file
+            }.items()))
+        return {
+            self.genome_source: chr_file_dict,
+            self.genome_generate: {
+                "name": chr_name,
+                "path": genome_f_path
+            }
+        }
+
     def merge_chr_files(self, chr_file_dict: dict, output_file: str) -> None:
         chr_name: list = chr_file_dict["name"]
         file_dict_path: dict = chr_file_dict["path"]
         # 排序
         chr_name.sort(key=lambda elem: self.chr_list[elem])
         self.log.info(f"Start merging file {chr_name}")
         # 生成文件
@@ -521,28 +560,103 @@
                     while True:
                         line: str = r.readline().strip()
                         if not line:
                             break
                         w.write(f"{line}\n")
                 self.log.info(f"Completed adding {chr_} file")
 
+    def after_two_step(self, file: str, chr_file_dict: dict, fragments_file: str):
+        # 多染色质进行排序
+        self.log.info(f"Start sorting {file} grouped files")
+        position_file_dict: dict = self.sort_position_files(chr_file_dict, file)
+        self.log.info(f"Sorted file information {position_file_dict}")
+        self.log.info(f"Sorting {file} group files completed")
+        # 对位点进行排序
+        self.log.info(f"Start merging {file} grouped files")
+        self.merge_chr_files(position_file_dict, fragments_file)
+        self.log.info(f"Merge {file} group files completed")
+
     def exec_sort_fragments(self) -> None:
         files_dict: dict = self.get_files()
         files_name: list = files_dict["name"]
         files_path: dict = files_dict["path"]
+
+        # 创建文件夹
+        cp_input_path_genome_source = os.path.join(self.cp_input_path, self.genome_source)
+        cp_input_path_genome_generate = os.path.join(self.cp_input_path, self.genome_generate)
+        if not cp_input_path_genome_source:
+            self.log.info(f"创建 {cp_input_path_genome_source} 文件夹")
+            os.makedirs(cp_input_path_genome_source)
+        if not cp_input_path_genome_generate:
+            self.log.info("")
+            self.log.info(f"创建 {cp_input_path_genome_generate} 文件夹")
+
         for file in files_name:
             # output file
-            chr_sort_fragments_file: str = os.path.join(self.cp_input_path, file)
-            if os.path.exists(chr_sort_fragments_file):
-                self.log.warn(f"{chr_sort_fragments_file} The file already exists, it has been processed by default")
-                continue
+            chr_sort_fragments_file_source: str = os.path.join(cp_input_path_genome_source, file)
+            chr_sort_fragments_file_generate: str = os.path.join(cp_input_path_genome_source, file)
+            chr_sort_fragments_file: dict = {
+                self.genome_source: cp_input_path_genome_source,
+                self.genome_generate: chr_sort_fragments_file_generate
+            }
+
+            if self.lift_over_path:
+                if os.path.exists(chr_sort_fragments_file_source) and os.path.exists(chr_sort_fragments_file_generate):
+                    self.log.warn(f"{chr_sort_fragments_file_source} and {chr_sort_fragments_file_generate}. The files already exists, it has been processed by default")
+                    continue
+            else:
+                if os.path.exists(chr_sort_fragments_file_source):
+                    self.log.warn(f"{chr_sort_fragments_file_source}. The file already exists, it has been processed by default")
+                    continue
+
             self.log.info(f"Start to group {file} files according to chromatin information")
             chr_file_dict: dict = self.write_chr_file(files_path[file], file)
             self.log.info(f"File information after grouping {chr_file_dict}")
             self.log.info(f"Complete file grouping of {file} according to chromatin information")
-            self.log.info(f"Start sorting {file} grouped files")
-            position_file_dict: dict = self.sort_position_files(chr_file_dict, file)
-            self.log.info(f"Sorted file information {position_file_dict}")
-            self.log.info(f"Sorting {file} group files completed")
-            self.log.info(f"Start merging {file} grouped files")
-            self.merge_chr_files(position_file_dict, chr_sort_fragments_file)
-            self.log.info(f"Merge {file} group files completed")
+
+            # 判断是否需要进行 liftOver
+            if self.lift_over_path:
+                # 进行转化为 hg19 或 hg38
+                genome_transformation_dict: dict = self.genome_transformation(chr_file_dict, file)
+                genome_list: list = list(genome_transformation_dict.keys())
+                for genome in genome_list:
+                    self.after_two_step(file, genome_transformation_dict[genome], chr_sort_fragments_file[genome])
+            else:
+                self.after_two_step(file, chr_file_dict, chr_sort_fragments_file_source)
+
+
+class Run:
+
+    def __init__(self, path: str, lift_over_path: str = None, is_hg19_to_hg38: bool = True):
+        self.base_path: str = os.path.join(path, "handler")
+        self.source_path: str = os.path.join(path, "source")
+        self.log = Logger("Run", "log/fragments.log")
+        self.file = yf.staticMethod(log_file="log")
+        self.lift_over_path: str = lift_over_path
+        self.is_hg19_to_hg38: bool = is_hg19_to_hg38
+        self.exec()
+
+    def exec(self):
+        # 尽量保证该路径下只有 GSE 号的文件
+        dirs_dict: dict = self.file.entry_dirs_dict(self.base_path)
+        dirs_name: list = dirs_dict["name"]
+
+        if not os.path.exists(self.source_path):
+            self.log.error(f"输入文件夹 {self.source_path} 不存在")
+
+        # 执行
+        for gsm in dirs_name:
+
+            archr_path = os.path.join(self.base_path, gsm, "ArchR")
+            if not os.path.exists(archr_path):
+                self.log.info(f"创建 {archr_path} 文件夹")
+                os.makedirs(archr_path)
+
+            self.log.info(f"开始执行 {gsm} 内容信息")
+            GetChrSortFragments(
+                path=self.base_path,
+                cp_path=archr_path,
+                gsm=gsm,
+                get_fragments_path=self.source_path,
+                lift_over_path=self.lift_over_path,
+                is_hg19_to_hg38=self.is_hg19_to_hg38
+            )
```

### Comparing `ykenan_fragments-1.0.1/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.1.0/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.0.1
+Version: 1.1.0
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

