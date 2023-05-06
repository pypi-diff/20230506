# Comparing `tmp/panfeed-1.1.1.tar.gz` & `tmp/panfeed-1.2.1.tar.gz`

## Comparing `panfeed-1.1.1.tar` & `panfeed-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.1.1/environment.yml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 panfeed-1.1.1/make_release.txt
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed-get-clusters-runner.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed-get-kmers-runner.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed-plot-runner.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed-runner.py
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/.plot.py.swp
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/__init__.py
--rw-r--r--   0        0        0    12672 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/__main__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/classes.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/colorlog.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/get_clusters.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/get_kmers.py
--rw-r--r--   0        0        0    13281 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/input.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/panfeed.py
--rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 panfeed-1.1.1/panfeed/plot.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.1.1/LICENSE
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.1.1/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.2.1/environment.yml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 panfeed-1.2.1/make_release.txt
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed-get-clusters-runner.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed-get-kmers-runner.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed-plot-runner.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed-runner.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/__init__.py
+-rw-r--r--   0        0        0    12672 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/__main__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/classes.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/colorlog.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/get_clusters.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/get_kmers.py
+-rw-r--r--   0        0        0    13821 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/input.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/panfeed.py
+-rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/plot.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.2.1/LICENSE
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.2.1/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.2.1/PKG-INFO
```

### Comparing `panfeed-1.1.1/panfeed/__main__.py` & `panfeed-1.2.1/panfeed/__main__.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/panfeed/classes.py` & `panfeed-1.2.1/panfeed/classes.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/panfeed/colorlog.py` & `panfeed-1.2.1/panfeed/colorlog.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/panfeed/get_clusters.py` & `panfeed-1.2.1/panfeed/get_clusters.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/panfeed/get_kmers.py` & `panfeed-1.2.1/panfeed/get_kmers.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/panfeed/input.py` & `panfeed-1.2.1/panfeed/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,25 @@
                 continue
     
     return features
 
 
 def iter_gene_clusters(panaroo, genome_data, up, down, down_start_codon, patfilt,
                        gene_list=None):
-    
+    # check if we have genome data for all
+    # strains in the pangenome
+    # if not give a warning
+    all_strains = set(panaroo.columns)
+    missing_strains = all_strains.difference(genome_data.keys())
+    if len(missing_strains) > 0:
+        logger.warning(f'There are {len(missing_strains)} strains present '
+                       'in the pangenome table but not in the GFF directory')
+        for strain in missing_strains:
+            logger.debug(f'Missing GFF file: {strain}')
+
     # go through each gene cluster
     all_ogs = panaroo.shape[0]
     for i, (idx, row) in enumerate(panaroo.iterrows()):
         if gene_list is not None and idx not in gene_list:
             logger.debug(f"Skipping {idx} ({i+1}/{all_ogs})")
             continue
 
@@ -295,15 +305,18 @@
             clusterpresab[sortstrain[strain]] = 1 
 
         # print(clusterpresab)
         # cycle through all the strains that have the gene
         for strain, genes in row.dropna().items():
             
             strain = str(strain)
-            
+
+            if strain not in genome_data:
+                continue
+
             gene_sequences[strain] = []
             # access the GFF/fasta data
             sequences, features = genome_data[strain]
             # be aware of paralogs
             for gene in genes.split(';'):
                 # access a particular gene
                 try:
```

### Comparing `panfeed-1.1.1/panfeed/panfeed.py` & `panfeed-1.2.1/panfeed/panfeed.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/panfeed/plot.py` & `panfeed-1.2.1/panfeed/plot.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/LICENSE` & `panfeed-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/README.md` & `panfeed-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/pyproject.toml` & `panfeed-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panfeed-1.1.1/PKG-INFO` & `panfeed-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panfeed
-Version: 1.1.1
+Version: 1.2.1
 Summary: Compute gene-cluster specific k-mers over a pangenome
 Project-URL: Homepage, https://github.com/microbial-pangenomes-lab/panfeed
 Project-URL: Bug Tracker, https://github.com/microbial-pangenomes-lab/panfeed/issues
 Author-email: Hannes Neubauer <neubauer.hannes@mh-hannover.de>, Marco Galardini <galardini.marco@mh-hannover.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

