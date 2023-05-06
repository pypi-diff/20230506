# Comparing `tmp/cellmap-1.0.1.dev202305060457-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202305060747-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 19774 bytes, number of entries: 5
+Zip file size: 19769 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   112591 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060457.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060457.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305060457.dist-info/RECORD
-5 files, 115005 bytes uncompressed, 19020 bytes compressed:  83.5%
+-rw-r--r--  2.0 unx   112785 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060747.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060747.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305060747.dist-info/RECORD
+5 files, 115199 bytes uncompressed, 19015 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060457.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202305060747.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060457.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202305060747.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060457.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202305060747.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -248,15 +248,15 @@
     exp_key = None,
     potential_key = 'potential',
     rotation_key = 'rotation',
     vorticity_key = 'vorticity',
     streamfunc_key = 'streamfunc',
     graph_key = 'CellMap_graph',
     edge_vel_key = 'edge_velocity',
-    graph_method = 'Delauney',
+    graph_method = 'knn',#'Delauney',
     HD_rate = 0.0,
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
     cut_std = None,
     verbose = True,
@@ -419,15 +419,15 @@
     basis = 'umap',
     vkey  = 'velocity',
     exp_key = None,
     potential_key = 'potential',
     potential_vkey = 'potential_velocity',
     rotation_key = 'rotation',
     rotation_vkey = 'rotation_velocity',
-    graph_method = 'Delauney',
+    graph_method = 'knn',#'Delauney',
     n_neighbors = 10,
     cutedge_vol  = None,
     cutedge_length = None,
     verbose = True,
     logscale_vel = True,
     ):
     """
@@ -444,15 +444,14 @@
     exp_key,vkey,basis = kwargs_arg['exp_key'],kwargs_arg['vkey'],kwargs_arg['basis']
     
     exp_2d_key_ = 'X_%s' % basis
     vel_2d_key_ = '%s_%s' % (vkey,basis)
     pot_vkey_ = '%s_%s' % (potential_vkey,basis)
     rot_vkey_ = '%s_%s' % (rotation_vkey,basis)
     
-    
     if exp_key == None:
         if scipy.sparse.issparse(adata.X):
             exp_HD = adata.X.toarray()
         else:
             exp_HD = adata.X
     elif exp_key in adata.obsm.keys():
         exp_HD = adata.obsm[exp_key]
@@ -465,20 +464,23 @@
     exp_LD = adata.obsm[exp_2d_key_][:,:2] if exp_2d_key_ in adata.obsm.keys() else adata.layers[exp_2d_key_][:,:2]
     
     n_node_ = exp_HD.shape[0]
     if graph_method == 'Delauney':
         source, target = create_graph(exp_LD,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='edges')
         # source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
     elif graph_method == 'knn':
-        pca = sklearn.decomposition.PCA()
-        exp_HD_pca = pca.fit_transform(exp_HD)
-        n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate])
+        # pca = sklearn.decomposition.PCA()
+        # exp_HD_pca = pca.fit_transform(exp_HD)
+        # n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate])
+        # knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
+        # knn.fit(exp_HD_pca[:,:n_pca])
+        # distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
-        knn.fit(exp_HD_pca[:,:n_pca])
-        distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
+        knn.fit(exp_LD)
+        distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         source = np.ravel(np.repeat(np.arange(exp_HD.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
         target = np.ravel(indices)
     
     n_edge_ = len(source)
     grad_mat = np.zeros([n_edge_,n_node_],dtype=float)
     grad_mat[tuple(np.vstack((np.arange(n_edge_),source)))] = -1
```

## Comparing `cellmap-1.0.1.dev202305060457.dist-info/METADATA` & `cellmap-1.0.1.dev202305060747.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202305060457
+Version: 1.0.1.dev202305060747
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

