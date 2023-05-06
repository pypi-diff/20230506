# Comparing `tmp/Slpapy-0.2.8.tar.gz` & `tmp/Slpapy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.2.8.tar", last modified: Fri May  5 07:59:05 2023, max compression
+gzip compressed data, was "Slpapy-0.2.9.tar", last modified: Sat May  6 04:53:46 2023, max compression
```

## Comparing `Slpapy-0.2.8.tar` & `Slpapy-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 07:59:05.082957 Slpapy-0.2.8/
--rw-rw-rw-   0        0        0      159 2023-05-05 07:59:05.081956 Slpapy-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 07:59:05.046957 Slpapy-0.2.8/Slpapy/
--rw-rw-rw-   0        0        0     3120 2023-05-05 07:57:07.000000 Slpapy-0.2.8/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.2.8/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:59:05.079957 Slpapy-0.2.8/Slpapy/Spatial_map/
--rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.2.8/Slpapy/Spatial_map/Spatial_map.py
--rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.2.8/Slpapy/Spatial_map/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.2.8/Slpapy/Spatial_map/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.2.8/Slpapy/Spatial_map/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.2.8/Slpapy/Spatial_map/readwrite.py
--rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.2.8/Slpapy/Spatial_map/scatterplots.py
--rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.2.8/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5262 2023-05-03 07:08:38.000000 Slpapy-0.2.8/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:59:05.055987 Slpapy-0.2.8/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 07:59:05.082957 Slpapy-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-05-05 07:58:15.000000 Slpapy-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:53:46.434014 Slpapy-0.2.9/
+-rw-rw-rw-   0        0        0      159 2023-05-06 04:53:46.433018 Slpapy-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 04:53:46.397114 Slpapy-0.2.9/Slpapy/
+-rw-rw-rw-   0        0        0     3145 2023-05-06 04:53:05.000000 Slpapy-0.2.9/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.2.9/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:53:46.431023 Slpapy-0.2.9/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.2.9/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.2.9/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.2.9/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.2.9/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.2.9/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.2.9/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.2.9/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.2.9/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.2.9/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.2.9/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.2.9/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.2.9/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.2.9/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.2.9/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5266 2023-05-06 04:33:53.000000 Slpapy-0.2.9/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:53:46.406090 Slpapy-0.2.9/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-06 04:53:45.000000 Slpapy-0.2.9/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-05-06 04:53:46.000000 Slpapy-0.2.9/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 04:53:45.000000 Slpapy-0.2.9/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-05-06 04:53:45.000000 Slpapy-0.2.9/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 04:53:45.000000 Slpapy-0.2.9/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 04:53:46.434014 Slpapy-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-05-06 04:53:30.000000 Slpapy-0.2.9/setup.py
```

### Comparing `Slpapy-0.2.8/Slpapy/Data_reconstruction.py` & `Slpapy-0.2.9/Slpapy/Data_reconstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         mask = str(mask)
         resave(mask, 10)
         df2 = pd.read_csv(f'{mask}' + "-1.csv", usecols=['m/z'], low_memory=False)
         os.remove(f'{mask}' + "-1.csv")
         for i in df2['m/z']:
             t = round(i, 2)
             for j in adata.var_names:
-                if round(adata.var.loc[j, 'm/z'], 2) == t:
+                tt = adata.var.loc[j, 'm/z']
+                if round(tt, 2) == t:
                     adata.var.loc[j, 'mask'] = True
                     break
 
     adata = adata[:, adata.var['mask'] != True]
     # 保存adata
     adata.write(f'{XY}' + ".h5ad")
     return adata
```

### Comparing `Slpapy-0.2.8/Slpapy/MZ_ppm_match.py` & `Slpapy-0.2.9/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/_compat.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/_docs.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/_rcmod.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/_settings.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/_utils.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/beats.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/is_constant.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/logging.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/palettes.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/readwrite.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/Spatial_map/scatterplots.py` & `Slpapy-0.2.9/Slpapy/Spatial_map/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.8/Slpapy/processing_analyze.py` & `Slpapy-0.2.9/Slpapy/processing_analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
         sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
         adata = adata[:, adata.var.highly_variable]
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     # 回归每个细胞的总计数和表达的线粒体基因的百分比的影响。
     sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
     #保存mz值
-    mz=adata.var
-    mz.to_csv('mz.csv')
+    mz = adata.var
+    mz.to_csv('./mz.csv')
     adata.write('./pp_done.h5ad')
     return adata
 
 
 def se_analyze(adata, n_neighbors, n_pcs,resolution):
     # 将每个脂质缩放到单位方差。阈值超过标准偏差 10。，如非高斯分布，则不建议使用
     #sc.pp.scale(adata, max_value=10)
```

### Comparing `Slpapy-0.2.8/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.2.9/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

