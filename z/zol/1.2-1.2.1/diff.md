# Comparing `tmp/zol-1.2.tar.gz` & `tmp/zol-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zol-1.2.tar", last modified: Fri May  5 05:53:35 2023, max compression
+gzip compressed data, was "zol-1.2.1.tar", last modified: Sat May  6 00:21:12 2023, max compression
```

## Comparing `zol-1.2.tar` & `zol-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-05-05 05:53:35.563969 zol-1.2/
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     1517 2023-05-04 23:57:25.000000 zol-1.2/LICENSE
--rw-rw-r--   0 rauf      (1000) rauf      (1000)      184 2023-05-05 05:53:35.563969 zol-1.2/PKG-INFO
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     9725 2023-05-05 05:32:59.000000 zol-1.2/README.md
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-05-05 05:53:35.563969 zol-1.2/bin/
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    31264 2023-05-04 23:57:25.000000 zol-1.2/bin/fai
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    12075 2023-05-04 23:57:25.000000 zol-1.2/bin/prepTG
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    35208 2023-05-04 23:57:25.000000 zol-1.2/bin/zol
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-05-05 05:53:35.563969 zol-1.2/scripts/
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    10375 2023-05-04 23:57:25.000000 zol-1.2/scripts/convertMiniprotGffToGbkAndProt.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     5692 2023-05-04 23:57:25.000000 zol-1.2/scripts/expandDereplicatedAlignment.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     6274 2023-05-04 23:57:25.000000 zol-1.2/scripts/extractBiG-SCAPEclusters.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     4479 2023-05-04 23:57:25.000000 zol-1.2/scripts/generateSyntenicVisual.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     9582 2023-05-04 23:57:25.000000 zol-1.2/scripts/listAllGenomesInDirectory.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     8377 2023-05-04 23:57:25.000000 zol-1.2/scripts/processNCBIGenBank.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     7726 2023-05-04 23:57:25.000000 zol-1.2/scripts/runProdigalAndMakeProperGenbank.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    18176 2023-05-05 04:59:00.000000 zol-1.2/scripts/setup_annotation_dbs.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)       38 2023-05-05 05:53:35.567969 zol-1.2/setup.cfg
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)     1189 2023-05-05 04:05:25.000000 zol-1.2/setup.py
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-05-05 05:53:35.563969 zol-1.2/zol/
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-05-04 23:57:25.000000 zol-1.2/zol/__init__.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    49500 2023-05-04 23:57:25.000000 zol-1.2/zol/fai.py
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-05-05 05:53:35.563969 zol-1.2/zol/orthologs/
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    18309 2023-05-04 23:57:25.000000 zol-1.2/zol/orthologs/findOrthologs.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)    41840 2023-05-04 23:57:25.000000 zol-1.2/zol/util.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    89963 2023-05-04 23:57:25.000000 zol-1.2/zol/zol.py
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-05-05 05:53:35.563969 zol-1.2/zol.egg-info/
--rw-rw-r--   0 rauf      (1000) rauf      (1000)      184 2023-05-05 05:53:35.000000 zol-1.2/zol.egg-info/PKG-INFO
--rw-rw-r--   0 rauf      (1000) rauf      (1000)      561 2023-05-05 05:53:35.000000 zol-1.2/zol.egg-info/SOURCES.txt
--rw-rw-r--   0 rauf      (1000) rauf      (1000)        1 2023-05-05 05:53:35.000000 zol-1.2/zol.egg-info/dependency_links.txt
--rw-rw-r--   0 rauf      (1000) rauf      (1000)        1 2023-05-05 05:53:35.000000 zol-1.2/zol.egg-info/not-zip-safe
--rw-rw-r--   0 rauf      (1000) rauf      (1000)        4 2023-05-05 05:53:35.000000 zol-1.2/zol.egg-info/top_level.txt
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-06 00:21:12.399253 zol-1.2.1/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     1517 2023-05-05 19:44:18.000000 zol-1.2.1/LICENSE
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      186 2023-05-06 00:21:12.399253 zol-1.2.1/PKG-INFO
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     9943 2023-05-06 00:12:43.000000 zol-1.2.1/README.md
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-06 00:21:12.395253 zol-1.2.1/bin/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    31293 2023-05-05 23:56:11.000000 zol-1.2.1/bin/fai
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    12075 2023-05-05 19:44:18.000000 zol-1.2.1/bin/prepTG
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    35208 2023-05-05 19:44:18.000000 zol-1.2.1/bin/zol
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-06 00:21:12.395253 zol-1.2.1/scripts/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    10375 2023-05-05 19:44:18.000000 zol-1.2.1/scripts/convertMiniprotGffToGbkAndProt.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     5692 2023-05-05 19:44:18.000000 zol-1.2.1/scripts/expandDereplicatedAlignment.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     6274 2023-05-05 19:44:18.000000 zol-1.2.1/scripts/extractBiG-SCAPEclusters.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     4479 2023-05-05 19:44:18.000000 zol-1.2.1/scripts/generateSyntenicVisual.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     9582 2023-05-05 19:44:18.000000 zol-1.2.1/scripts/listAllGenomesInDirectory.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     8377 2023-05-05 19:44:18.000000 zol-1.2.1/scripts/processNCBIGenBank.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7726 2023-05-05 19:44:18.000000 zol-1.2.1/scripts/runProdigalAndMakeProperGenbank.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    18176 2023-05-05 19:44:18.000000 zol-1.2.1/scripts/setup_annotation_dbs.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)       38 2023-05-06 00:21:12.399253 zol-1.2.1/setup.cfg
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1191 2023-05-05 19:53:42.000000 zol-1.2.1/setup.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-06 00:21:12.399253 zol-1.2.1/zol/
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-05 19:44:18.000000 zol-1.2.1/zol/__init__.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    49389 2023-05-05 23:55:09.000000 zol-1.2.1/zol/fai.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-06 00:21:12.399253 zol-1.2.1/zol/orthologs/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    18309 2023-05-05 19:44:18.000000 zol-1.2.1/zol/orthologs/findOrthologs.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    39571 2023-05-05 19:57:02.000000 zol-1.2.1/zol/util.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    83835 2023-05-06 00:14:40.000000 zol-1.2.1/zol/zol.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-06 00:21:12.399253 zol-1.2.1/zol.egg-info/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      186 2023-05-06 00:21:12.000000 zol-1.2.1/zol.egg-info/PKG-INFO
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      561 2023-05-06 00:21:12.000000 zol-1.2.1/zol.egg-info/SOURCES.txt
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-05-06 00:21:12.000000 zol-1.2.1/zol.egg-info/dependency_links.txt
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-05-06 00:21:12.000000 zol-1.2.1/zol.egg-info/not-zip-safe
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        4 2023-05-06 00:21:12.000000 zol-1.2.1/zol.egg-info/top_level.txt
```

### Comparing `zol-1.2/LICENSE` & `zol-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zol-1.2/README.md` & `zol-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,19 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
 ## Updates  
 
+### Version 1.2.1
+
+- add line in beginning of fai to request "fork" method for multiprocessing to work on macOS with python >=v3.8.
+- clean up unused functions and simplify yaml file for specifying conda environment.
+
 ### Minor Update - 05/05/2023
 
 - update parsing of PGAP HMMs directory after extracting with tar.
 
 ### Version 1.2/1.02
 
 - prepTG sample to GenBank relations now specified locally so creation of database is not locked into one location.
```

### Comparing `zol-1.2/bin/fai` & `zol-1.2.1/bin/fai`

 * *Files 0% similar despite different names*

```diff
@@ -37,22 +37,20 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import sys
 import argparse
-from Bio import SeqIO
 from time import sleep
 from zol import util, fai
 import subprocess
 import pickle
 import shutil
-import math
-
+import multiprocessing
 zol_main_directory = '/'.join(os.path.realpath(__file__).split('/')[:-2]) + '/'
 
 def create_parser():
 	""" Parse arguments """
 	parser = argparse.ArgumentParser(description="""
 	Program: zol
 	Author: Rauf Salamzade
@@ -520,8 +518,9 @@
 		os.system('touch %s' % step5_check_file)
 
 	# Close logging object and exit
 	util.closeLoggerObject(logObject)
 	sys.exit(0)
 
 if __name__ == '__main__':
-	faiMain()
+	multiprocessing.set_start_method('fork')
+	faiMain()
```

### Comparing `zol-1.2/bin/prepTG` & `zol-1.2.1/bin/prepTG`

 * *Files identical despite different names*

### Comparing `zol-1.2/bin/zol` & `zol-1.2.1/bin/zol`

 * *Files identical despite different names*

### Comparing `zol-1.2/scripts/convertMiniprotGffToGbkAndProt.py` & `zol-1.2.1/scripts/convertMiniprotGffToGbkAndProt.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/scripts/expandDereplicatedAlignment.py` & `zol-1.2.1/scripts/expandDereplicatedAlignment.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/scripts/extractBiG-SCAPEclusters.py` & `zol-1.2.1/scripts/extractBiG-SCAPEclusters.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/scripts/generateSyntenicVisual.py` & `zol-1.2.1/scripts/generateSyntenicVisual.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/scripts/listAllGenomesInDirectory.py` & `zol-1.2.1/scripts/listAllGenomesInDirectory.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/scripts/processNCBIGenBank.py` & `zol-1.2.1/scripts/processNCBIGenBank.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/scripts/runProdigalAndMakeProperGenbank.py` & `zol-1.2.1/scripts/runProdigalAndMakeProperGenbank.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/scripts/setup_annotation_dbs.py` & `zol-1.2.1/scripts/setup_annotation_dbs.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/setup.py` & `zol-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 import os
 
 setup(name='zol',
-      version='1.2',
+      version='1.2.1',
       description='',
       url='http://github.com/Kalan-Lab/zol/',
       author='Rauf Salamzade',
       author_email='salamzader@gmail.com',
       license='BSD-3',
       packages=['zol'],
       scripts=['bin/zol',
```

### Comparing `zol-1.2/zol/fai.py` & `zol-1.2.1/zol/fai.py`

 * *Files 1% similar despite different names*

```diff
@@ -618,15 +618,14 @@
 						if lt in sample_lt_to_hg[sample]:
 							hgs_ordered.append(sample_lt_to_hg[sample][lt])
 						else:
 							hgs_ordered.append('background')
 					hgs_ordered_dict[sample][scaffold] = hgs_ordered
 					lts_ordered_dict[sample][scaffold] = lts_ordered
 
-				# TODO switch to using global variables for large dictionaries to reference in parallelized task directly
 				identify_gc_segments_input.append([sample, min_hits, min_key_hits, key_hgs, kq_evalue_threshold,
 												   syntenic_correlation_threshold, max_int_genes_for_merge,
 												   flanking_context, draft_mode, gc_delineation_mode])
 
 			p = multiprocessing.Pool(cpus)
 			p.map(identify_gc_instances, identify_gc_segments_input)
 			p.close()
@@ -1153,8 +1152,8 @@
 			sys.exit(1)
 
 	except Exception as e:
 		logObject.error('Issues with plotting overviews of homologous gene-cluster segments identified.')
 		sys.stderr.write('Issues with plotting overviews of homologous gene-cluster segments identified.\n')
 		sys.stderr.write(str(e) + '\n')
 		raise RuntimeError(traceback.format_exc())
-		sys.exit(1)
+		sys.exit(1)
```

### Comparing `zol-1.2/zol/orthologs/findOrthologs.py` & `zol-1.2.1/zol/orthologs/findOrthologs.py`

 * *Files identical despite different names*

### Comparing `zol-1.2/zol/util.py` & `zol-1.2.1/zol/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from Bio.Seq import Seq
 import logging
 import subprocess
 from operator import itemgetter
 from collections import defaultdict
 import traceback
 from scipy import stats
-from ete3 import Tree
 import numpy as np
 import gzip
 import pathlib
 import copy
 import itertools
 import multiprocessing
 import pickle
@@ -223,26 +222,14 @@
 	p = np.asfarray(p)
 	by_descend = p.argsort()[::-1]
 	by_orig = by_descend.argsort()
 	steps = float(len(p)) / np.arange(len(p), 0, -1)
 	q = np.minimum(1, np.minimum.accumulate(steps * p[by_descend]))
 	return q[by_orig]
 
-
-def is_newick(newick):
-	"""
-	Function to validate if Newick phylogeny file is correctly formatted.
-	"""
-	try:
-		t = Tree(newick)
-		return True
-	except:
-		return False
-
-
 def is_fastq(fastq):
 	"""
 	Function to validate if FASTA file is correctly formatted.
 	"""
 	try:
 		with open(fastq) as of:
 			SeqIO.parse(of, 'fastq')
@@ -617,77 +604,18 @@
 			panda_dict[key] = vals
 		panda_df = pd.DataFrame(panda_dict)
 
 	except Exception as e:
 		raise RuntimeError(traceback.format_exc())
 	return panda_df
 
-def calculateSelectDistances(newick_file, selected_pairs):
-	try:
-		t = Tree(newick_file)
-		leafs = set([])
-		for node in t.traverse('postorder'):
-			if node.is_leaf():
-				leafs.add(node.name)
-		pw_info = defaultdict(lambda: "nan")
-		for i, n1 in enumerate(sorted(leafs)):
-			for j, n2 in enumerate(sorted(leafs)):
-				if i >= j: continue
-				if n1 == n2: continue
-				gn1 = n1.split('|')[0]
-				gn2 = n2.split('|')[0]
-				pw_key = tuple([gn1, gn2])
-				pw_dist = t.get_distance(n1, n2)
-				if pw_key in selected_pairs:
-					if pw_key in pw_info and pw_dist < pw_info[pw_key]:
-						pw_info[pw_key] = pw_dist
-					else:
-						pw_info[pw_key] = pw_dist
-		return (pw_info)
-	except Exception as e:
-		sys.stderr.write('Issues with calculating pairwise distances for tree: %s.\n' % newick_file)
-		sys.stderr.write(str(e) + '\n')
-		raise RuntimeError(traceback.format_exc())
-		sys.exit(1)
-
-def computeCongruence(hg, gene_tree, gc_pw_info, selected_pairs, outf, logObject):
-	try:
-		hg_pw_info = calculateSelectDistances(gene_tree, selected_pairs)
-		hg_pw_dists_filt = []
-		gc_pw_dists_filt = []
-		for pair in selected_pairs:
-			if hg_pw_info[pair] != 'nan' and gc_pw_info[pair] != 'nan':
-				hg_pw_dists_filt.append(hg_pw_info[pair])
-				gc_pw_dists_filt.append(gc_pw_info[pair])
-
-		congruence_slope = 'NA'
-		congruence_rvalue = 'NA'
-		if hg_pw_dists_filt == gc_pw_dists_filt:
-			congruence_slope = '1.0'
-			congruence_rvalue = '1.0'
-		elif len(hg_pw_dists_filt) >= 3:
-			try:
-				slope, _, rvalue, pvalue, _ = stats.linregress(gc_pw_dists_filt, hg_pw_dists_filt)
-			except:
-				slope = 'nan'
-				rvalue = 'nan'
-			if slope != 'nan' and rvalue != 'nan':
-				congruence_slope = float(slope)
-				congruence_rvalue = float(rvalue)
-		out_handle = open(outf, 'w')
-		out_handle.write(str(congruence_slope) + '\t' + str(congruence_rvalue) + '\n')
-		out_handle.close()
-
-	except Exception as e:
-		sys.stderr.write('Issues with computing congruence of gene tree for homolog group %s to gene-cluster consensus tree.\n' % hg)
-		logObject.error('Issues with computing congruence of gene tree for homolog group %s to gene-cluster consensus tree.' % hg)
-		sys.stderr.write(str(e) + '\n')
-		sys.exit(1)
-
 def checkCoreHomologGroupsExist(ortho_matrix_file):
+	"""
+	Function to check that a core ortholog/homolog group exists across homologous gene-clusters.
+	"""
 	try:
 		core_hgs = set([])
 		with open(ortho_matrix_file) as omf:
 			for i, line in enumerate(omf):
 				if i == 0: continue
 				line = line.rstrip('\n')
 				ls = line.split('\t')
```

### Comparing `zol-1.2/zol/zol.py` & `zol-1.2.1/zol/zol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1807,15 +1807,15 @@
 
 		# Generate Excel spreadsheet
 		writer = pd.ExcelWriter(final_report_xlsx, engine='xlsxwriter')
 		workbook = writer.book
 		dd_sheet = workbook.add_worksheet('Data Dictionary')
 		dd_sheet.write(0, 0, 'WARNING: some evolutionary statistics are experimental - evaluate with caution!!!')
 		dd_sheet.write(1, 0, 'Data Dictionary describing columns of "Overview" spreadsheets can be found on zol\'s Wiki at:')
-		dd_sheet.write(2, 0, 'https://github.com/Kalan-Lab/zol/wiki/2.-more-info-on-zol#explanation-of-report')
+		dd_sheet.write(2, 0, 'https://github.com/Kalan-Lab/zol/wiki/3.-more-info-on-zol#explanation-of-report')
 
 		numeric_columns = {'Proportion of Total Gene Clusters with HG', 'Proportion of Focal Gene Clusters with HG',
 						   'Proportion of Comparator Gene Clusters with HG', 'Fixation Index',
 						   'Upstream Region Fixation Index', 'HG Median Length (bp)', 'HG Consensus Order',
 						   'Tajima\'s D', 'Entropy', 'Upstream Region Entropy',
 						   'GARD Partitions Based on Recombination Breakpoints',
 						   'Number of Sites Identified as Under Positive or Negative Selection by FUBAR',
@@ -2028,154 +2028,16 @@
 		plot_cmd = ['Rscript', plot_prog, ml_track_file, hm_track_file, plot_result_pdf, str(height), str(width)]
 		try:
 			subprocess.call(' '.join(plot_cmd), shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL,
 							executable='/bin/bash')
 			assert (os.path.isfile(plot_result_pdf))
 			logObject.info('Successfully ran: %s' % ' '.join(plot_cmd))
 		except Exception as e:
-			logObject.error('Had an issue running R based plotting: %s' % ' '.join(plot_cmd))
-			sys.stderr.write('Had an issue running R based plotting: %s\n' % ' '.join(plot_cmd))
+			logObject.error('Had an issue running R based plotting - potentially because of R setup issues in conda: %s' % ' '.join(plot_cmd))
+			sys.stderr.write('Had an issue running R based plotting - potentially because of R setup issues in conda: %s\n' % ' '.join(plot_cmd))
 			logObject.error(e)
 			sys.exit(1)
 	except Exception as e:
 		sys.stderr.write('Issues creating visualizations.\n')
 		logObject.error('Issues creating visualizations.')
 		sys.stderr.write(str(e) + '\n')
-		sys.exit(1)
-
-"""
-def runTreemmer(genbanks, gene_cluster_tree, max_for_visualization, logObject):
-	representative_genbanks = set([])
-	try:
-		if len(genbanks) <= max_for_visualization:
-			for gbk in genbanks:
-				representative_genbanks.add('.'.join(gbk.split('/')[-1].split('.')[:-1]))
-		else:
-			retain_listing_file = gene_cluster_tree + '_trimmed_list_X_' + str(max_for_visualization)
-			treemmer_cmd = ['python', treemmer_prog, '-X=' + str(max_for_visualization), gene_cluster_tree]
-			try:
-				subprocess.call(' '.join(treemmer_cmd), shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL,
-								executable='/bin/bash')
-				assert (os.path.isfile(retain_listing_file))
-				logObject.info('Successfully ran: %s' % ' '.join(treemmer_cmd))
-			except Exception as e:
-				logObject.error('Had an issue running Treemmer: %s' % ' '.join(treemmer_cmd))
-				sys.stderr.write('Had an issue running Treemmer: %s\n' % ' '.join(treemmer_cmd))
-				logObject.error(e)
-				sys.exit(1)
-			with open(retain_listing_file) as orlf:
-				for line in orlf:
-					line = line.strip()
-					representative_genbanks.add(line)
-	except Exception as e:
-		sys.stderr.write('Issues running Treemmer to reduce the set of input GenBanks to a representative set for easier visualization with clinker.\n')
-		logObject.error('Issues running Treemmer to reduce the set of input GenBanks to a representative set for easier visualization with clinker.')
-		sys.stderr.write(str(e) + '\n')
-		sys.exit(1)
-	return(representative_genbanks)
-
-def runGeneTreeCongruenceAnalysis(genbanks, tree_dir, gtc_results_dir, logObject, subsample_max=1000):
-	try:
-		# Run STAG by David Emms and Steve Kelley
-		stag_map_file = gtc_results_dir + 'Species_Mapping.txt'
-		smf_handle = open(stag_map_file, 'w')
-		prefices = []
-		for gbk in genbanks:
-			prefix = '.'.join(gbk.split('/')[-1].split('.')[:-1])
-			prefices.append(prefix)
-			smf_handle.write(prefix + '|*\t' + prefix + '\n')
-		smf_handle.close()
-
-		stag_cmd = [stag_prog, stag_map_file, tree_dir]
-		result_gc_tree = None
-		try:
-			subprocess.call(' '.join(stag_cmd), shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL,
-							executable='/bin/bash')
-			par_dir_with_species_tree = '/'.join(os.path.abspath(tree_dir).split('/')[:-1]) + '/'
-			for sd in os.listdir(par_dir_with_species_tree):
-				if sd.startswith("STAG"):
-					result_gc_tree = par_dir_with_species_tree + sd + '/SpeciesTree.tre'
-			assert(os.path.isfile(result_gc_tree))
-			logObject.info('Successfully ran: %s' % ' '.join(stag_cmd))
-		except Exception as e:
-			logObject.error('Had an issue running STAG: %s' % ' '.join(stag_cmd))
-			sys.stderr.write('Had an issue running STAG: %s\n' % ' '.join(stag_cmd))
-			logObject.error(e)
-			sys.exit(1)
-
-		all_pairwise_combinations = itertools.combinations(sorted(prefices), 2)
-		all_pairwise_combinations = sorted(list(all_pairwise_combinations))
-		num_total_pairwise = len(all_pairwise_combinations)
-		subsample_size = min(subsample_max, num_total_pairwise)
-		selected_pairs = random.sample(all_pairwise_combinations, k=subsample_size)
-
-		gc_pw_info = util.calculateSelectDistances(result_gc_tree, selected_pairs)
-		hg_to_gc_congruence_slope = {}
-		hg_to_gc_congruence_rvalue = {}
-		for hgt in os.listdir(tree_dir):
-			hg = hgt.split('.tre')[0]
-			outf = gtc_results_dir + hg + '.txt'
-			util.computeCongruence(hg, tree_dir + hgt, gc_pw_info, selected_pairs, outf, logObject)
-
-		for f in os.listdir(gtc_results_dir):
-			if f == 'Species_Mapping.txt': continue
-			hg = f.split('.txt')[0]
-			with open(gtc_results_dir + f) as ogf:
-				for line in ogf:
-					line = line.strip()
-					slope, rvalue = line.split('\t')
-					hg_to_gc_congruence_slope[hg] = slope
-					hg_to_gc_congruence_rvalue[hg] = rvalue
-		return([result_gc_tree, hg_to_gc_congruence_slope, hg_to_gc_congruence_rvalue])
-	except Exception as e:
-		sys.stderr.write('Issues with running gene tree to gene-cluster tree congruence analysis.\n')
-		logObject.error('Issues with running gene tree to gene-cluster tree congruence analysis.')
-		sys.stderr.write(str(e) + '\n')
-		sys.exit(1)
-
-# clinker is great but I was having trouble with mapping proteins to homolog groups so it will be akin 
-# running the tool itself on the raw data. If you are reading this check out clinker!
-def runClinker(genbanks, hg_lts, representative_genbanks, fin_dir, work_dir, logObject):
-	try:
-		renamed_lts_dir = work_dir + 'GenBanks_LTs_Renamed/'
-		util.setupReadyDirectory([renamed_lts_dir])
-		input_gbks = []
-		for gbk in genbanks:
-			gbk_name = '.'.join(gbk.split('/')[-1].split('.')[:-1])
-			if not gbk_name in representative_genbanks: continue
-			updated_gbk = renamed_lts_dir + gbk.split('/')[-1]
-			ug_handle = open(updated_gbk, 'w')
-			with open(gbk) as ogbk:
-				for rec in SeqIO.parse(ogbk, 'genbank'):
-					for feature in rec.features:
-						if not feature.type == 'CDS': continue
-						lt = feature.qualifiers.get('locus_tag')[0]
-						feature.qualifiers['locus_tag'] = gbk_name + '|' + lt
-					SeqIO.write(rec, ug_handle, 'genbank')
-			ug_handle.close()
-			input_gbks.append(updated_gbk)
-		hg_mapping_file = work_dir + 'Locus_Tag_to_Homolog_Group_Mapping.csv'
-		hmf_handle = open(hg_mapping_file, 'w')
-		for hg in hg_lts:
-			for lt in hg_lts[hg]:
-				if lt.split('|')[0] in representative_genbanks:
-					hmf_handle.write(lt.split('|')[-1] + ',' + hg + '\n')
-		hmf_handle.close()
-
-		result_html = fin_dir + 'clinker_Visual_of_Representative_Gene_Clusters.html'
-		clinker_cmd = ['clinker', '-gf', hg_mapping_file, '-p', result_html] + input_gbks
-		try:
-			subprocess.call(' '.join(clinker_cmd), shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL,
-							executable='/bin/bash')
-			assert (os.path.isfile(result_html))
-			logObject.info('Successfully ran: %s' % ' '.join(clinker_cmd))
-		except Exception as e:
-			logObject.error('Had an issue running clinker: %s' % ' '.join(clinker_cmd))
-			sys.stderr.write('Had an issue running clinker: %s\n' % ' '.join(clinker_cmd))
-			logObject.error(e)
-			sys.exit(1)
-	except Exception as e:
-		sys.stderr.write('Issues running clinker or creating inputs for clinker.\n')
-		logObject.error('Issues running clinker or creating inputs for clinker.')
-		sys.stderr.write(str(e) + '\n')
-		sys.exit(1)
-"""
+		sys.exit(1)
```

### Comparing `zol-1.2/zol.egg-info/SOURCES.txt` & `zol-1.2.1/zol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

