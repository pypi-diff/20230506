# Comparing `tmp/cellmap-1.0.1.dev202305031402-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202305060213-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 19848 bytes, number of entries: 5
+Zip file size: 19898 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   113410 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305031402.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305031402.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305031402.dist-info/RECORD
-5 files, 115824 bytes uncompressed, 19094 bytes compressed:  83.5%
+-rw-r--r--  2.0 unx   113621 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060213.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060213.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305060213.dist-info/RECORD
+5 files, 116035 bytes uncompressed, 19144 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305031402.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202305060213.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305031402.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202305060213.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305031402.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202305060213.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -356,16 +356,16 @@
     pot_flow_2_ = np.hstack((pot_flow_,-pot_flow_))
     rot_flow_2_ = np.hstack((rot_flow_,-rot_flow_))
     edge_vel_norm = np.linalg.norm(edge_velocity(exp_LD,vel_LD,source,target,normalization=False))
     if graph_method == 'Delauney':
         for i in range(adata.shape[0]):
             idx_ = src_trg_ == i
             ex_s = -(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]])/np.linalg.norm(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]],ord=2)
-            vel_potential[i] = edge_vel_norm*edge_vel_norm*np.sum(pot_flow_2_[idx_]*ex_s.T,axis=1)
-            vel_rotation[i]  = edge_vel_norm*edge_vel_norm*np.sum(rot_flow_2_[idx_]*ex_s.T,axis=1)
+            vel_potential[i] = edge_vel_norm*np.sum(pot_flow_2_[idx_]*ex_s.T,axis=1)
+            vel_rotation[i]  = edge_vel_norm*np.sum(rot_flow_2_[idx_]*ex_s.T,axis=1)
             # idx_s = source == i
             # idx_t = target == i
             # if sum(idx_s) > 0:
             #     ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
             #     vel_potential[i] += 2*edge_vel_norm*np.sum(pot_flow_[idx_s]*ex_s.T,axis=1)
             #     vel_rotation[i]  += 2*edge_vel_norm*np.sum(rot_flow_[idx_s]*ex_s.T,axis=1)
             # if sum(idx_t) > 0:
@@ -378,15 +378,16 @@
     elif graph_method == 'knn':
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_LD)
         distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         for i in range(adata.shape[0]):
             ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
-            vel_potential[i] = -edge_vel_norm*np.sum((adata.obs[potential_key].values[indices[i]]-adata.obs[potential_key].values[i])*ex_s.T,axis=1)
+            vel_potential[i] = -np.sum((pot_flow_[indices[i]]-pot_flow_[i])*ex_s.T,axis=1)
+            vel_rotation[i] = -np.sum((rot_flow_[indices[i]]-rot_flow_[i])*ex_s.T,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
         # adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
         adata.obsm[rot_vkey_] = vel_rotation
     
     # for i in idx_bd_:
     #     lap[i,:] = 0
     #     lap[i,i] = 1
@@ -657,34 +658,40 @@
 def view_stream(
     adata,
     basis = 'umap',
     vkey = 'velocity',
     potential_vkey = 'potential_velocity',
     rotation_vkey = 'rotation_velocity',
     cluster_key = 'clusters',
+    additional_key = '',
     figsize=(24,6),
     density = 2,
     alpha = 0.3,
     fontsize = 18,
     legend_fontsize = 18,
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata, basis = basis)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     data_pos = adata.obsm[basis_key]
     cluster = adata.obs[cluster_key]
+
+    vkey_ = vkey
+    pot_vkey_ = potential_vkey+additional_key
+    rot_vkey_ = rotation_vkey+additional_key
+    
     
     fig,ax = plt.subplots(1,3,figsize=figsize,tight_layout=True)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey, title='RNA velocity',ax=ax[0],color=cluster_key,
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey_, title='RNA velocity',ax=ax[0],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=potential_vkey, title='Potential flow',ax=ax[1],color=cluster_key,
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=pot_vkey_, title='Potential flow',ax=ax[1],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],color=cluster_key,
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rot_vkey_, title='Rotational flow',ax=ax[2],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
     for i in range(3):
         texts = []
         for c in np.unique(cluster):
             txt = ax[i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=legend_fontsize,ha='center', va='center',fontweight='bold',zorder=20)
             txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
             texts.append(txt)
@@ -693,14 +700,15 @@
 def view_stream_line(
     adata,
     basis = 'umap',
     contour_key = 'streamfunc',
     cluster_key = 'clusters',
     potential_key = 'potential',
     rotation_key = 'rotation',
+    additional_key = '',
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
     save_dir = None,
     save_filename = 'CellMap_stream_line',
     figsize = (24,6),
@@ -709,17 +717,17 @@
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata,basis = basis)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
-    key_ = '%s_%s' % (contour_key,basis)
-    pot_key_ = '%s_%s_%s' % (potential_key,contour_key,basis)
-    rot_key_ = '%s_%s_%s' % (rotation_key,contour_key,basis)
+    key_ = ('%s_%s' % (contour_key,basis))+additional_key
+    pot_key_ = ('%s_%s_%s' % (potential_key,contour_key,basis))+additional_key
+    rot_key_ = ('%s_%s_%s' % (rotation_key,contour_key,basis))+additional_key
     
     
     data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
     
     contour_keys = [key_, pot_key_, rot_key_]
     camps = [cmap_earth(adata.obs[key_]),'rainbow','coolwarm']
```

## Comparing `cellmap-1.0.1.dev202305031402.dist-info/METADATA` & `cellmap-1.0.1.dev202305060213.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202305031402
+Version: 1.0.1.dev202305060213
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

