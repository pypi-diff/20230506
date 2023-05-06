# Comparing `tmp/callingcardstools-0.1.1.tar.gz` & `tmp/callingcardstools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callingcardstools-0.1.1.tar", max compression
+gzip compressed data, was "callingcardstools-0.1.2.tar", max compression
```

## Comparing `callingcardstools-0.1.1.tar` & `callingcardstools-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.1/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.1/README.md
--rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.1/callingcardstools/Alignment/AlignmentTagger.py
--rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.1/callingcardstools/Alignment/SummaryParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.1/callingcardstools/Alignment/__init__.py
--rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/Alignment/mammals/ReadRecords.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/Alignment/mammals/__init__.py
--rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.1/callingcardstools/Alignment/mammals/process_alignments.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/Alignment/yeast/__init__.py
--rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/Alignment/yeast/legacy_makeccf.py
--rw-r--r--   0        0        0    10645 2023-05-06 03:12:16.663723 callingcardstools-0.1.1/callingcardstools/Alignment/yeast/process_alignments.py
--rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.1/callingcardstools/BarcodeParser/BarcodeParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/BarcodeParser/__init__.py
--rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/BarcodeParser/barcode_table_to_json.py
--rw-r--r--   0        0        0    16874 2023-05-02 18:36:19.660388 callingcardstools-0.1.1/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
--rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.1/callingcardstools/BarcodeParser/yeast/__init__.py
--rw-r--r--   0        0        0     1120 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/QC/StatusFlags.py
--rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/QC/__init__.py
--rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.1/callingcardstools/QC/create_status_coder.py
--rw-r--r--   0        0        0     7337 2023-04-30 11:31:28.623544 callingcardstools-0.1.1/callingcardstools/QC/parse_id_to_barcode.py
--rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/Reads/ReadParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/Reads/__init__.py
--rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/Reads/legacy_split_fastq.py
--rw-r--r--   0        0        0    11222 2023-05-03 02:30:53.474496 callingcardstools-0.1.1/callingcardstools/Reads/split_fastq.py
--rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/Resources/PackageResources.py
--rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/human/__init__.py
--rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/human/barcode_details.json
--rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/human/chr_map.csv
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/mouse/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/mouse/barcode_details.json
--rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/yeast/README.md
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/yeast/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.1/callingcardstools/Resources/yeast/barcode_details.json
--rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.1/callingcardstools/Resources/yeast/yeast.db
--rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.1/callingcardstools/__init__.py
--rw-r--r--   0        0        0     5674 2023-05-02 19:43:08.730006 callingcardstools-0.1.1/callingcardstools/__main__.py
--rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.1/callingcardstools/utils.py
--rw-r--r--   0        0        0     2016 2023-05-06 04:21:26.651606 callingcardstools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.1/setup.py
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.2/README.md
+-rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.2/callingcardstools/Alignment/AlignmentTagger.py
+-rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.2/callingcardstools/Alignment/SummaryParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.2/callingcardstools/Alignment/__init__.py
+-rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.2/callingcardstools/Alignment/mammals/ReadRecords.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.2/callingcardstools/Alignment/mammals/__init__.py
+-rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.2/callingcardstools/Alignment/mammals/process_alignments.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.2/callingcardstools/Alignment/yeast/__init__.py
+-rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.2/callingcardstools/Alignment/yeast/legacy_makeccf.py
+-rw-r--r--   0        0        0    11373 2023-05-06 12:27:56.051093 callingcardstools-0.1.2/callingcardstools/Alignment/yeast/process_alignments.py
+-rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.2/callingcardstools/BarcodeParser/BarcodeParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.2/callingcardstools/BarcodeParser/__init__.py
+-rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.2/callingcardstools/BarcodeParser/barcode_table_to_json.py
+-rw-r--r--   0        0        0    16874 2023-05-02 18:36:19.660388 callingcardstools-0.1.2/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
+-rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.2/callingcardstools/BarcodeParser/yeast/__init__.py
+-rw-r--r--   0        0        0     4084 2023-05-06 12:15:15.710439 callingcardstools-0.1.2/callingcardstools/QC/StatusFlags.py
+-rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.2/callingcardstools/QC/__init__.py
+-rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.2/callingcardstools/QC/create_status_coder.py
+-rw-r--r--   0        0        0     7357 2023-05-06 11:17:03.212706 callingcardstools-0.1.2/callingcardstools/QC/parse_id_to_barcode.py
+-rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.2/callingcardstools/Reads/ReadParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.2/callingcardstools/Reads/__init__.py
+-rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.2/callingcardstools/Reads/legacy_split_fastq.py
+-rw-r--r--   0        0        0    11222 2023-05-03 02:30:53.474496 callingcardstools-0.1.2/callingcardstools/Reads/split_fastq.py
+-rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.2/callingcardstools/Resources/PackageResources.py
+-rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.2/callingcardstools/Resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.2/callingcardstools/Resources/human/__init__.py
+-rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.2/callingcardstools/Resources/human/barcode_details.json
+-rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.2/callingcardstools/Resources/human/chr_map.csv
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.2/callingcardstools/Resources/mouse/__init__.py
+-rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.2/callingcardstools/Resources/mouse/barcode_details.json
+-rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.2/callingcardstools/Resources/yeast/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.2/callingcardstools/Resources/yeast/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.2/callingcardstools/Resources/yeast/barcode_details.json
+-rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.2/callingcardstools/Resources/yeast/yeast.db
+-rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.2/callingcardstools/__init__.py
+-rw-r--r--   0        0        0     5674 2023-05-02 19:43:08.730006 callingcardstools-0.1.2/callingcardstools/__main__.py
+-rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.2/callingcardstools/utils.py
+-rw-r--r--   0        0        0     2016 2023-05-06 12:51:22.591132 callingcardstools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.2/setup.py
+-rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.2/PKG-INFO
```

### Comparing `callingcardstools-0.1.1/LICENSE` & `callingcardstools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/README.md` & `callingcardstools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Alignment/AlignmentTagger.py` & `callingcardstools-0.1.2/callingcardstools/Alignment/AlignmentTagger.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Alignment/SummaryParser.py` & `callingcardstools-0.1.2/callingcardstools/Alignment/SummaryParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Alignment/mammals/ReadRecords.py` & `callingcardstools-0.1.2/callingcardstools/Alignment/mammals/ReadRecords.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Alignment/mammals/process_alignments.py` & `callingcardstools-0.1.2/callingcardstools/Alignment/mammals/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Alignment/yeast/legacy_makeccf.py` & `callingcardstools-0.1.2/callingcardstools/Alignment/yeast/legacy_makeccf.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Alignment/yeast/process_alignments.py` & `callingcardstools-0.1.2/callingcardstools/Alignment/yeast/process_alignments.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pandas as pd
 
 # from memory_profiler import profile
 # local dependencies
 from callingcardstools.Alignment.AlignmentTagger import AlignmentTagger
 from callingcardstools.QC.create_status_coder import create_status_coder  # noqa
 from callingcardstools.Alignment.SummaryParser import SummaryParser
+from callingcardstools.QC.StatusFlags import StatusFlags
 
 __all__ = ['parse_args', 'process_alignments']
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 def parse_args(
@@ -76,17 +77,17 @@
                         type=int)
 
     parser.add_argument("-o",
                         "--output_dir",
                         help="path to the output directory"
                         " (default: current directory)",
                         default='.')
-    
+
     parser.add_argument("-v",
-                        "--verbose",
+                        "--verbose_qc",
                         help="save complete alignment summary",
                         action="store_true")
 
     return subparser
 
 
 def process_alignments(args: argparse.Namespace) -> dict:
@@ -148,15 +149,15 @@
     except AttributeError:
         nthreads = 1
 
     try:
         output_dir = args.output_dir
     except AttributeError:
         output_dir = os.getcwd()
-    
+
     output_basename = os.path.splitext(os.path.basename(args.bampath))[0]
 
     logging.info("tagging reads...")
     # temp_dir is automatically cleaned when context ends
     with tempfile.TemporaryDirectory() as temp_dir:
         # create temp file in temp dir -- note that temp dir is destroyed
         # when this context ends
@@ -257,18 +258,38 @@
     pysam.index(bampath_out)  # pylint:disable=E1101
 
     logging.info(f'summarizing {bampath_out} to summary_df and qbed...')
     aln_summary_df = pd.DataFrame(read_summary)
     sp = SummaryParser(aln_summary_df)
     qbed_df = sp.to_qbed()
 
-    qbed_df.to_csv(os.path.join(output_dir, output_basename + '.qbed'), 
+    qbed_df.to_csv(os.path.join(output_dir, output_basename + '.qbed'),
                    sep='\t',
                    index=False)
-    
-    if args.verbose:
-        aln_summary_df.to_csv(os.path.join(output_dir, output_basename + '.summary'), 
-                              sep='\t',
-                              index=False)
+
+    aln_summary_df = aln_summary_df\
+        .assign(status_decomp=StatusFlags.decompose(aln_summary_df['status'],
+                                                    as_str=True))
+    # Convert the lists in the status_decomp column to strings
+    # by joining the elements with a comma
+    aln_summary_df['status_decomp'] = aln_summary_df['status_decomp']\
+        .apply(lambda x: ', '.join(x))
+
+    qc_summary = aln_summary_df\
+        .groupby(['status_decomp'])\
+        .agg({'id': 'count'})\
+        .reset_index()\
+        .rename(columns={'id': 'count'})
+
+    qc_summary.to_csv(
+        os.path.join(output_dir, output_basename + '_summary.tsv'),
+        sep='\t',
+        index=False)
+
+    if args.verbose_qc:
+        aln_summary_df.to_csv(
+            os.path.join(output_dir, output_basename + '_aln_info.tsv'),
+            sep='\t',
+            index=False)
 
     logging.info(f'{bampath_out} complete!')
-    #return {'summary': aln_summary_df, 'qbed': qbed_df}
+    # return {'summary': aln_summary_df, 'qbed': qbed_df}
```

### Comparing `callingcardstools-0.1.1/callingcardstools/BarcodeParser/BarcodeParser.py` & `callingcardstools-0.1.2/callingcardstools/BarcodeParser/BarcodeParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/BarcodeParser/barcode_table_to_json.py` & `callingcardstools-0.1.2/callingcardstools/BarcodeParser/barcode_table_to_json.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py` & `callingcardstools-0.1.2/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/QC/create_status_coder.py` & `callingcardstools-0.1.2/callingcardstools/QC/create_status_coder.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/QC/parse_id_to_barcode.py` & `callingcardstools-0.1.2/callingcardstools/QC/parse_id_to_barcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from callingcardstools.BarcodeParser import BarcodeParser
+import pandas as pd
 
 
 class QcParser(BarcodeParser):
 
     def __init__(self, id_to_barcode_tsv: str,
                  barcode_details_json: str,
                  **kwargs):
```

### Comparing `callingcardstools-0.1.1/callingcardstools/Reads/ReadParser.py` & `callingcardstools-0.1.2/callingcardstools/Reads/ReadParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Reads/legacy_split_fastq.py` & `callingcardstools-0.1.2/callingcardstools/Reads/legacy_split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Reads/split_fastq.py` & `callingcardstools-0.1.2/callingcardstools/Reads/split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Resources/PackageResources.py` & `callingcardstools-0.1.2/callingcardstools/Resources/PackageResources.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Resources/human/barcode_details.json` & `callingcardstools-0.1.2/callingcardstools/Resources/human/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Resources/human/chr_map.csv` & `callingcardstools-0.1.2/callingcardstools/Resources/human/chr_map.csv`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Resources/mouse/barcode_details.json` & `callingcardstools-0.1.2/callingcardstools/Resources/mouse/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Resources/yeast/README.md` & `callingcardstools-0.1.2/callingcardstools/Resources/yeast/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Resources/yeast/barcode_details.json` & `callingcardstools-0.1.2/callingcardstools/Resources/yeast/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/Resources/yeast/yeast.db` & `callingcardstools-0.1.2/callingcardstools/Resources/yeast/yeast.db`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/__main__.py` & `callingcardstools-0.1.2/callingcardstools/__main__.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/callingcardstools/utils.py` & `callingcardstools-0.1.2/callingcardstools/utils.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.1/pyproject.toml` & `callingcardstools-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "callingCardsTools"
-version = "0.1.1"
+version = "0.1.2"
 description = "A collection of objects and functions to work with calling cards sequencing tools"
 authors = ["chase mateusiak <chase.mateusiak@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cmatkhan.github.io/callingCardsTools/"
 repository = "https://github.com/cmatKhan/callingCardsTools"
 documentation = "https://cmatkhan.github.io/callingCardsTools/"
```

### Comparing `callingcardstools-0.1.1/setup.py` & `callingcardstools-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'scipy>=1.8.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['callingcardstools = callingcardstools:__main__.main']}
 
 setup_kwargs = {
     'name': 'callingcardstools',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A collection of objects and functions to work with calling cards sequencing tools',
     'long_description': "# Installation \n\n```\npip install callingcardstools\n```\n\nTo start using the command line tools, see the help message with:\n\n```\ncallingcardstools --help\n```\n\n# Development Installation\n\n1. install [poetry](https://python-poetry.org/)\n  - I prefer to set the default location of the virtual environment to the \n  project directory. You can set that as a global configuration for your \n  poetry installation like so: `poetry config virtualenvs.in-project true`\n\n2. git clone the repo\n\n3. cd into the repo and issue the command `poetry install`\n\n4. shell into the virtual environment with `poetry shell`\n\n5. build the package with `poetry build`\n\n6. install the callingcardstools packge into your virtual environment \n  `pip install dist/callingcardstools-...`\n  - Note: you could figure out how to use the pip install `-e` flag to \n  have an interactive development environment. I don't think that is compatible \n  with only the `pyproject.toml` file, but if you look it up, you'll find good \n  stackoverflow instructions on how to put a dummy `setup.py` file in to make \n  this possible\n\n7. Building the Dockerimage:\n\nCurrently the Dockerimage is built from a stable version on github\n\nNote that unless I set it up, you won't be able to push to my dockerhub repo. \nI think that is possible to do, though. If you wish to push to your own dockerhub, \nreplace the cmatkhan to your username.\n\n```bash\ndocker build -t cmatkhan/callingcardstools - < Dockerfile\n```\n\nwhere cmatkhan/callingcardstools is the tag. This will default to the version \n`latest`\n\nTo push:\n\n```bash\ndocker push cmatkhan/callingcardstools\n```",
     'author': 'chase mateusiak',
     'author_email': 'chase.mateusiak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://cmatkhan.github.io/callingCardsTools/',
```

### Comparing `callingcardstools-0.1.1/PKG-INFO` & `callingcardstools-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callingcardstools
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of objects and functions to work with calling cards sequencing tools
 Home-page: https://cmatkhan.github.io/callingCardsTools/
 License: MIT
 Author: chase mateusiak
 Author-email: chase.mateusiak@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

