# Comparing `tmp/callingcardstools-0.1.0.tar.gz` & `tmp/callingcardstools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callingcardstools-0.1.0.tar", max compression
+gzip compressed data, was "callingcardstools-0.1.1.tar", max compression
```

## Comparing `callingcardstools-0.1.0.tar` & `callingcardstools-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.0/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.0/README.md
--rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.0/callingcardstools/Alignment/AlignmentTagger.py
--rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.0/callingcardstools/Alignment/SummaryParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.0/callingcardstools/Alignment/__init__.py
--rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.0/callingcardstools/Alignment/mammals/ReadRecords.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.0/callingcardstools/Alignment/mammals/__init__.py
--rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.0/callingcardstools/Alignment/mammals/process_alignments.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.0/callingcardstools/Alignment/yeast/__init__.py
--rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.0/callingcardstools/Alignment/yeast/legacy_makeccf.py
--rw-r--r--   0        0        0    10718 2023-04-30 11:27:21.769662 callingcardstools-0.1.0/callingcardstools/Alignment/yeast/process_alignments.py
--rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.0/callingcardstools/BarcodeParser/BarcodeParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.0/callingcardstools/BarcodeParser/__init__.py
--rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.0/callingcardstools/BarcodeParser/barcode_table_to_json.py
--rw-r--r--   0        0        0    16874 2023-05-02 18:36:19.660388 callingcardstools-0.1.0/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
--rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.0/callingcardstools/BarcodeParser/yeast/__init__.py
--rw-r--r--   0        0        0     1120 2023-04-30 11:24:56.130406 callingcardstools-0.1.0/callingcardstools/QC/StatusFlags.py
--rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.0/callingcardstools/QC/__init__.py
--rw-r--r--   0        0        0     4321 2023-04-30 11:27:31.528600 callingcardstools-0.1.0/callingcardstools/QC/create_status_coder.py
--rw-r--r--   0        0        0     7337 2023-04-30 11:31:28.623544 callingcardstools-0.1.0/callingcardstools/QC/parse_id_to_barcode.py
--rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.0/callingcardstools/Reads/ReadParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.0/callingcardstools/Reads/__init__.py
--rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.0/callingcardstools/Reads/legacy_split_fastq.py
--rw-r--r--   0        0        0    11073 2023-05-02 14:46:36.323618 callingcardstools-0.1.0/callingcardstools/Reads/split_fastq.py
--rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.0/callingcardstools/Resources/PackageResources.py
--rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.0/callingcardstools/Resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.0/callingcardstools/Resources/human/__init__.py
--rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.0/callingcardstools/Resources/human/barcode_details.json
--rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.0/callingcardstools/Resources/human/chr_map.csv
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.0/callingcardstools/Resources/mouse/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.0/callingcardstools/Resources/mouse/barcode_details.json
--rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.0/callingcardstools/Resources/yeast/README.md
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.0/callingcardstools/Resources/yeast/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.0/callingcardstools/Resources/yeast/barcode_details.json
--rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.0/callingcardstools/Resources/yeast/yeast.db
--rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.0/callingcardstools/__init__.py
--rw-r--r--   0        0        0     5674 2023-05-02 19:43:08.730006 callingcardstools-0.1.0/callingcardstools/__main__.py
--rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.0/callingcardstools/utils.py
--rw-r--r--   0        0        0     1991 2023-05-02 19:56:43.412622 callingcardstools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.0/setup.py
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.1/README.md
+-rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.1/callingcardstools/Alignment/AlignmentTagger.py
+-rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.1/callingcardstools/Alignment/SummaryParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.1/callingcardstools/Alignment/__init__.py
+-rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/Alignment/mammals/ReadRecords.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/Alignment/mammals/__init__.py
+-rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.1/callingcardstools/Alignment/mammals/process_alignments.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/Alignment/yeast/__init__.py
+-rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/Alignment/yeast/legacy_makeccf.py
+-rw-r--r--   0        0        0    10645 2023-05-06 03:12:16.663723 callingcardstools-0.1.1/callingcardstools/Alignment/yeast/process_alignments.py
+-rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.1/callingcardstools/BarcodeParser/BarcodeParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/BarcodeParser/__init__.py
+-rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.1/callingcardstools/BarcodeParser/barcode_table_to_json.py
+-rw-r--r--   0        0        0    16874 2023-05-02 18:36:19.660388 callingcardstools-0.1.1/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
+-rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.1/callingcardstools/BarcodeParser/yeast/__init__.py
+-rw-r--r--   0        0        0     1120 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/QC/StatusFlags.py
+-rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/QC/__init__.py
+-rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.1/callingcardstools/QC/create_status_coder.py
+-rw-r--r--   0        0        0     7337 2023-04-30 11:31:28.623544 callingcardstools-0.1.1/callingcardstools/QC/parse_id_to_barcode.py
+-rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/Reads/ReadParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/Reads/__init__.py
+-rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/Reads/legacy_split_fastq.py
+-rw-r--r--   0        0        0    11222 2023-05-03 02:30:53.474496 callingcardstools-0.1.1/callingcardstools/Reads/split_fastq.py
+-rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.1/callingcardstools/Resources/PackageResources.py
+-rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/human/__init__.py
+-rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/human/barcode_details.json
+-rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/human/chr_map.csv
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/mouse/__init__.py
+-rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/mouse/barcode_details.json
+-rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/yeast/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.1/callingcardstools/Resources/yeast/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.1/callingcardstools/Resources/yeast/barcode_details.json
+-rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.1/callingcardstools/Resources/yeast/yeast.db
+-rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.1/callingcardstools/__init__.py
+-rw-r--r--   0        0        0     5674 2023-05-02 19:43:08.730006 callingcardstools-0.1.1/callingcardstools/__main__.py
+-rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.1/callingcardstools/utils.py
+-rw-r--r--   0        0        0     2016 2023-05-06 04:21:26.651606 callingcardstools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.1/setup.py
+-rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.1/PKG-INFO
```

### Comparing `callingcardstools-0.1.0/LICENSE` & `callingcardstools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/README.md` & `callingcardstools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Alignment/AlignmentTagger.py` & `callingcardstools-0.1.1/callingcardstools/Alignment/AlignmentTagger.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Alignment/SummaryParser.py` & `callingcardstools-0.1.1/callingcardstools/Alignment/SummaryParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Alignment/mammals/ReadRecords.py` & `callingcardstools-0.1.1/callingcardstools/Alignment/mammals/ReadRecords.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Alignment/mammals/process_alignments.py` & `callingcardstools-0.1.1/callingcardstools/Alignment/mammals/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Alignment/yeast/legacy_makeccf.py` & `callingcardstools-0.1.1/callingcardstools/Alignment/yeast/legacy_makeccf.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Alignment/yeast/process_alignments.py` & `callingcardstools-0.1.1/callingcardstools/Alignment/yeast/process_alignments.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,56 +54,42 @@
     parser.set_defaults(func=process_alignments)
 
     parser.add_argument("-i",
                         "--bampath",
                         help="path to the input bam file",
                         required=True)
 
-    parser.add_argument("-o",
-                        "--output_dir",
-                        help="path to the output directory"
-                        " (default: current directory)")
-
     parser.add_argument("-g",
                         "--genome",
                         help=" ".join(["Path to a genome .fasta file.",
                                        "Note that an index .fai file must exist in the same path"]),
                         required=True)
 
     parser.add_argument("-j",
                         "--barcode_details",
                         help="Path to the barcode details json file",
                         required=True)
 
-    parser.add_argument('-d',
-                        '--database',
-                        help='path to the cc database',
-                        required=True)
-
-    parser.add_argument('-t',
-                        '--tf',
-                        help='Name of the tf for this alignment',
-                        required=True)
-
-    parser.add_argument('-r',
-                        '--regions_tblname',
-                        help='Name of the regions table in the db',
-                        required=True)
-
-    parser.add_argument('-b',
-                        '--background_tblname',
-                        help='Name of the background table in the db',
-                        required=True)
-
     parser.add_argument("-q",
                         "--mapq_threshold",
                         help="",
                         default=10,
                         type=int)
 
+    parser.add_argument("-o",
+                        "--output_dir",
+                        help="path to the output directory"
+                        " (default: current directory)",
+                        default='.')
+    
+    parser.add_argument("-v",
+                        "--verbose",
+                        help="save complete alignment summary",
+                        action="store_true")
+
     return subparser
 
 
 def process_alignments(args: argparse.Namespace) -> dict:
     """Iterate over a bam file, set tags and output updated bam with
      read groups added to the header, tags added to the reads.
      Also output a summary of the reads
@@ -162,25 +148,26 @@
     except AttributeError:
         nthreads = 1
 
     try:
         output_dir = args.output_dir
     except AttributeError:
         output_dir = os.getcwd()
+    
+    output_basename = os.path.splitext(os.path.basename(args.bampath))[0]
 
     logging.info("tagging reads...")
     # temp_dir is automatically cleaned when context ends
     with tempfile.TemporaryDirectory() as temp_dir:
         # create temp file in temp dir -- note that temp dir is destroyed
         # when this context ends
         bampath_tmp = os.path.join(temp_dir, "tmp_tagged.bam")
         # create the path to store the (permanent) output bam
         bampath_out = os.path.join(
-            output_dir,
-            os.path.splitext(os.path.basename(args.bampath))[0] + out_suffix)  # noqa
+            output_dir, output_basename + out_suffix)
 
         # open files
         # open the input bam
         input_bamfile = pysam.AlignmentFile(  # pylint:disable=E1101
             args.bampath, "rb",
             require_index=True,
             threads=nthreads)
@@ -190,21 +177,22 @@
             "wb",
             header=input_bamfile.header)
 
         at = AlignmentTagger(args.barcode_details, args.genome)
 
         status_coder = create_status_coder(
             mapq_threshold=mapq_threshold,
-            check_5_prime_clip=True)
+            check_5_prime_clip=True,
+            check_passing=False)
 
         read_group_set = set()
         read_summary = []
         # until_eof will include unmapped reads, also
         for read in input_bamfile.fetch(until_eof=True):
-            tagged_read = at.tag_read(read)
+            tagged_read = at.tag_read(read, decompose_barcode=False)
 
             status_code = status_coder(tagged_read)
 
             summary_record = {"id": tagged_read.get('read').query_name,
                               "status": status_code,
                               "mapq": tagged_read.get('read').mapping_quality,
                               "flag": tagged_read.get('read').flag,
@@ -269,9 +257,18 @@
     pysam.index(bampath_out)  # pylint:disable=E1101
 
     logging.info(f'summarizing {bampath_out} to summary_df and qbed...')
     aln_summary_df = pd.DataFrame(read_summary)
     sp = SummaryParser(aln_summary_df)
     qbed_df = sp.to_qbed()
 
+    qbed_df.to_csv(os.path.join(output_dir, output_basename + '.qbed'), 
+                   sep='\t',
+                   index=False)
+    
+    if args.verbose:
+        aln_summary_df.to_csv(os.path.join(output_dir, output_basename + '.summary'), 
+                              sep='\t',
+                              index=False)
+
     logging.info(f'{bampath_out} complete!')
-    return {'summary': aln_summary_df, 'qbed': qbed_df}
+    #return {'summary': aln_summary_df, 'qbed': qbed_df}
```

### Comparing `callingcardstools-0.1.0/callingcardstools/BarcodeParser/BarcodeParser.py` & `callingcardstools-0.1.1/callingcardstools/BarcodeParser/BarcodeParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/BarcodeParser/barcode_table_to_json.py` & `callingcardstools-0.1.1/callingcardstools/BarcodeParser/barcode_table_to_json.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py` & `callingcardstools-0.1.1/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/QC/StatusFlags.py` & `callingcardstools-0.1.1/callingcardstools/QC/StatusFlags.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/QC/create_status_coder.py` & `callingcardstools-0.1.1/callingcardstools/QC/create_status_coder.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 def create_status_coder(
         insert_seqs: list = ['*'],
         mapq_threshold: int = 10,
-        check_5_prime_clip: bool = False) -> Callable[[AlignedSegment], int]:
+        check_5_prime_clip: bool = False,
+        check_passing: bool = True) -> Callable[[AlignedSegment], int]:
     """A factory function which returns a function capable of determining
      the status code of a read tagged by an AlignmentTagger object
 
     Args:
         insert_seqs (list): a list of acceptable insert sequences. Defaults to
          ['*'], which will skip the insert seq check altogether.
         mapq_threshold (int): a mapq_threshold. Less than this value will be
         marked as failing the mapq threshold test. Default is 10.
+        check_passing (bool, optional): Whether to check the passing key
+            in the barcode_details dict. Defaults to True.
 
     Returns:
         Callable[[pysam.AlignedSegment], int]: A function which given a tagged
          pysam AlignedSegment will return the status code for a the read
     """
 
-    def coder(read_details: AlignedSegment, status_code: int = 0) -> int:
+    def coder(read_details: AlignedSegment,
+              status_code: int = 0) -> int:
         """_summary_
 
         Args:
             read_details.get('read') (AlignedSegment): a pysam.AlignedSegment
              object
             status_code (int, optional): Initial status code.
              Defaults to 0.
@@ -51,21 +55,24 @@
                            'read_details')
         if not isinstance(read_details.get('read'), AlignedSegment):
             raise ValueError('read_details["read"] must be a '
                              'pysam.AlignedSegment object')
         if not isinstance(read_details.get('barcode_details'), dict):
             raise ValueError('read_details["barcode_details"] must be a '
                              'dict')
-        if not isinstance(
-                read_details.get('barcode_details').get('passing', None),
-                bool):
-            raise KeyError('passing must be a key in '
-                           'read_details["barcode_details"]')
-
-        if not read_details.get('barcode_details').get('passing'):
+        if check_passing:
+            if not isinstance(
+                    read_details.get('barcode_details').get('passing', None),
+                    bool):
+                raise KeyError('passing must be a key in '
+                               'read_details["barcode_details"]')
+
+        # if check passing is set to false, then the passing key may not
+        # exist. In this event, assume the read is passing
+        if not read_details.get('barcode_details').get('passing', True):
             status_code += StatusFlags.BARCODE.flag()
         # if the read is unmapped, add the flag, but don't check
         # other alignment metrics
         if read_details.get('read').is_unmapped:
             status_code += StatusFlags.UNMAPPED.flag()
         else:
             if read_details.get('read').is_qcfail:
```

### Comparing `callingcardstools-0.1.0/callingcardstools/QC/parse_id_to_barcode.py` & `callingcardstools-0.1.1/callingcardstools/QC/parse_id_to_barcode.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Reads/ReadParser.py` & `callingcardstools-0.1.1/callingcardstools/Reads/ReadParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Reads/legacy_split_fastq.py` & `callingcardstools-0.1.1/callingcardstools/Reads/legacy_split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Reads/split_fastq.py` & `callingcardstools-0.1.1/callingcardstools/Reads/split_fastq.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                         required=True)
     parser.add_argument('-s',
                         '--split_key',
                         help="Either a name of a key in " +
                         "barcode_details['components'], or just a string. "
                         "This will be used to create the passing "
                         "output fastq filenames",
-                        required=True)
+                        default="tf")
     parser.add_argument('-n',
                         '--split_suffix',
                         help='append this after the tf name and before _R1.fq '
                         'in the output fastq files',
                         default="split")
     parser.add_argument('-v',
                         '--verbose_qc',
@@ -237,16 +237,19 @@
         for write_handle in determined_out[read_end].values():
             write_handle.close()
 
     # construct the input to the BarcodeQcCounter summarize method
     component_dict = {k: [] for k in ['tf', 'r1_primer', 'r2_transposon']}
     r1_primer_start = rp.barcode_dict['r1']['primer']['index'][0]
     r1_primer_end = rp.barcode_dict['r1']['primer']['index'][1]
-    r2_transposon_start = rp.barcode_dict['r2']['transposon']['index'][0]
-    r2_transposon_end = rp.barcode_dict['r2']['transposon']['index'][1]
+    r2_transposon_start = r1_primer_end + \
+        rp.barcode_dict['r2']['transposon']['index'][0]
+    r2_transposon_end = (r2_transposon_start +
+                         rp.barcode_dict['r2']['transposon']['index'][1] -
+                         rp.barcode_dict['r2']['transposon']['index'][0])
     for k, v in rp.barcode_dict['components']['tf']['map'].items():
         r1_primer_seq = k[r1_primer_start:r1_primer_end]
         r2_transposon_seq = k[r2_transposon_start:r2_transposon_end]
         component_dict['tf'].append(v)
         component_dict['r1_primer'].append(r1_primer_seq)
         component_dict['r2_transposon'].append(r2_transposon_seq)
     # summarize the barcode metrics
```

### Comparing `callingcardstools-0.1.0/callingcardstools/Resources/PackageResources.py` & `callingcardstools-0.1.1/callingcardstools/Resources/PackageResources.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Resources/human/barcode_details.json` & `callingcardstools-0.1.1/callingcardstools/Resources/human/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Resources/human/chr_map.csv` & `callingcardstools-0.1.1/callingcardstools/Resources/human/chr_map.csv`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Resources/mouse/barcode_details.json` & `callingcardstools-0.1.1/callingcardstools/Resources/mouse/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Resources/yeast/README.md` & `callingcardstools-0.1.1/callingcardstools/Resources/yeast/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Resources/yeast/barcode_details.json` & `callingcardstools-0.1.1/callingcardstools/Resources/yeast/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/Resources/yeast/yeast.db` & `callingcardstools-0.1.1/callingcardstools/Resources/yeast/yeast.db`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/__main__.py` & `callingcardstools-0.1.1/callingcardstools/__main__.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/callingcardstools/utils.py` & `callingcardstools-0.1.1/callingcardstools/utils.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.0/pyproject.toml` & `callingcardstools-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "callingCardsTools"
-version = "0.1.0"
+version = "0.1.1"
 description = "A collection of objects and functions to work with calling cards sequencing tools"
 authors = ["chase mateusiak <chase.mateusiak@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cmatkhan.github.io/callingCardsTools/"
 repository = "https://github.com/cmatKhan/callingCardsTools"
 documentation = "https://cmatkhan.github.io/callingCardsTools/"
@@ -38,15 +38,17 @@
 autopep8 = "^2.0.2"
 
 [tool.pyright]
 include = ["callingcardstools"]
 exclude = ["**/node_modules",
     "**/__pycache__",
     "src/experimental",
-    "src/typestubs"
+    "src/typestubs",
+    "tests",
+    "temp"
 ]
 defineConstant = { DEBUG = true }
 stubPath = "src/stubs"
 venvPath = "."
 venv = ".venv"
 
 reportMissingImports = true
```

### Comparing `callingcardstools-0.1.0/setup.py` & `callingcardstools-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'scipy>=1.8.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['callingcardstools = callingcardstools:__main__.main']}
 
 setup_kwargs = {
     'name': 'callingcardstools',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A collection of objects and functions to work with calling cards sequencing tools',
     'long_description': "# Installation \n\n```\npip install callingcardstools\n```\n\nTo start using the command line tools, see the help message with:\n\n```\ncallingcardstools --help\n```\n\n# Development Installation\n\n1. install [poetry](https://python-poetry.org/)\n  - I prefer to set the default location of the virtual environment to the \n  project directory. You can set that as a global configuration for your \n  poetry installation like so: `poetry config virtualenvs.in-project true`\n\n2. git clone the repo\n\n3. cd into the repo and issue the command `poetry install`\n\n4. shell into the virtual environment with `poetry shell`\n\n5. build the package with `poetry build`\n\n6. install the callingcardstools packge into your virtual environment \n  `pip install dist/callingcardstools-...`\n  - Note: you could figure out how to use the pip install `-e` flag to \n  have an interactive development environment. I don't think that is compatible \n  with only the `pyproject.toml` file, but if you look it up, you'll find good \n  stackoverflow instructions on how to put a dummy `setup.py` file in to make \n  this possible\n\n7. Building the Dockerimage:\n\nCurrently the Dockerimage is built from a stable version on github\n\nNote that unless I set it up, you won't be able to push to my dockerhub repo. \nI think that is possible to do, though. If you wish to push to your own dockerhub, \nreplace the cmatkhan to your username.\n\n```bash\ndocker build -t cmatkhan/callingcardstools - < Dockerfile\n```\n\nwhere cmatkhan/callingcardstools is the tag. This will default to the version \n`latest`\n\nTo push:\n\n```bash\ndocker push cmatkhan/callingcardstools\n```",
     'author': 'chase mateusiak',
     'author_email': 'chase.mateusiak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://cmatkhan.github.io/callingCardsTools/',
```

### Comparing `callingcardstools-0.1.0/PKG-INFO` & `callingcardstools-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callingcardstools
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of objects and functions to work with calling cards sequencing tools
 Home-page: https://cmatkhan.github.io/callingCardsTools/
 License: MIT
 Author: chase mateusiak
 Author-email: chase.mateusiak@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

