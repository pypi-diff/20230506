# Comparing `tmp/cellmap-1.0.1.dev202305060213-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202305060457-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 19898 bytes, number of entries: 5
+Zip file size: 19774 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   113621 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060213.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060213.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305060213.dist-info/RECORD
-5 files, 116035 bytes uncompressed, 19144 bytes compressed:  83.5%
+-rw-r--r--  2.0 unx   112591 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060457.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060457.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305060457.dist-info/RECORD
+5 files, 115005 bytes uncompressed, 19020 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060213.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202305060457.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060213.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202305060457.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060213.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202305060457.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -304,20 +304,23 @@
     
     ## Compute graph and edge velocities
     n_node_ = exp_HD.shape[0]
     idx_bd_  = []
     if graph_method == 'Delauney':
         source, target, idx_bd_ = create_graph(exp_LD,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,cut_std=cut_std,return_type='edges_bd')
     elif graph_method == 'knn':
-        pca = sklearn.decomposition.PCA()
-        exp_HD_pca = pca.fit_transform(exp_HD)
-        n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
+        # pca = sklearn.decomposition.PCA()
+        # exp_HD_pca = pca.fit_transform(exp_HD)
+        # n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
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
     
     if HD_rate > 0:
         edge_vel_HD = edge_velocity(exp_HD,vel_HD,source,target)
     else:
@@ -333,18 +336,14 @@
     grad_mat = np.zeros([n_edge_,n_node_],dtype=float)
     grad_mat[tuple(np.vstack((np.arange(n_edge_),source)))] = -1
     grad_mat[tuple(np.vstack((np.arange(n_edge_),target)))] = 1
     div_mat = -grad_mat.T
     lap = -np.dot(div_mat,grad_mat)
     edge_vel = (1-HD_rate)*edge_vel_LD+HD_rate*edge_vel_HD
     source_term = np.dot(div_mat,edge_vel)
-    # for i in idx_bd_:
-    #     lap[i,:] = 0
-    #     lap[i,i] = 1
-    #     source_term[i] = 0
     lap_inv_ = np.linalg.pinv(lap)
     potential = np.dot(lap_inv_,source_term)
     pot_flow_ = -np.dot(grad_mat,potential)
     rot_flow_ = edge_vel - pot_flow_
     adata.obs[potential_key] = potential - np.min(potential)
 
 
@@ -352,72 +351,54 @@
     vel_potential = np.zeros([adata.shape[0],2],dtype=float)
     vel_rotation = np.zeros([adata.shape[0],2],dtype=float)
     src_trg_ = np.hstack((source,target))
     trg_src_ = np.hstack((target,source))
     pot_flow_2_ = np.hstack((pot_flow_,-pot_flow_))
     rot_flow_2_ = np.hstack((rot_flow_,-rot_flow_))
     edge_vel_norm = np.linalg.norm(edge_velocity(exp_LD,vel_LD,source,target,normalization=False))
-    if graph_method == 'Delauney':
-        for i in range(adata.shape[0]):
-            idx_ = src_trg_ == i
-            ex_s = -(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]])/np.linalg.norm(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]],ord=2)
-            vel_potential[i] = edge_vel_norm*np.sum(pot_flow_2_[idx_]*ex_s.T,axis=1)
-            vel_rotation[i]  = edge_vel_norm*np.sum(rot_flow_2_[idx_]*ex_s.T,axis=1)
-            # idx_s = source == i
-            # idx_t = target == i
-            # if sum(idx_s) > 0:
-            #     ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
-            #     vel_potential[i] += 2*edge_vel_norm*np.sum(pot_flow_[idx_s]*ex_s.T,axis=1)
-            #     vel_rotation[i]  += 2*edge_vel_norm*np.sum(rot_flow_[idx_s]*ex_s.T,axis=1)
-            # if sum(idx_t) > 0:
-            #     ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
-            #     vel_potential[i] += -2*edge_vel_norm*np.sum(pot_flow_[idx_t]*ex_t.T,axis=1)
-            #     vel_rotation[i]  += -2*edge_vel_norm*np.sum(rot_flow_[idx_t]*ex_t.T,axis=1)
-        adata.obsm[pot_vkey_] = vel_potential
-        # adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
-        adata.obsm[rot_vkey_] = vel_rotation
-    elif graph_method == 'knn':
-        knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
-        knn.fit(exp_LD)
-        distances, indices = knn.kneighbors(exp_LD)
-        distances, indices = distances[:,1:], indices[:,1:]
-        for i in range(adata.shape[0]):
-            ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
-            vel_potential[i] = -np.sum((pot_flow_[indices[i]]-pot_flow_[i])*ex_s.T,axis=1)
-            vel_rotation[i] = -np.sum((rot_flow_[indices[i]]-rot_flow_[i])*ex_s.T,axis=1)
-        adata.obsm[pot_vkey_] = vel_potential
-        # adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
-        adata.obsm[rot_vkey_] = vel_rotation
-    
-    # for i in idx_bd_:
-    #     lap[i,:] = 0
-    #     lap[i,i] = 1
-    # lap_inv_ = np.linalg.pinv(lap)
-    ## Solve vorticity & stream line
+    # if graph_method == 'Delauney':
+    for i in range(adata.shape[0]):
+        idx_ = src_trg_ == i
+        # ex_s = -(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]])/np.linalg.norm(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]],ord=2)
+        # vel_potential[i] = 2.*edge_vel_norm*np.mean(pot_flow_2_[idx_]*ex_s.T,axis=1)
+        # vel_rotation[i]  = 2.*edge_vel_norm*np.mean(rot_flow_2_[idx_]*ex_s.T,axis=1)
+        dis_ = np.linalg.norm(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]],axis=1,ord=2)
+        dis_[dis_==0] = 1
+        ex_ = -(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]]).T/dis_
+        vel_potential[i] = 4.*edge_vel_norm*np.mean(pot_flow_2_[idx_]*ex_,axis=1)
+        vel_rotation[i]  = 4.*edge_vel_norm*np.mean(rot_flow_2_[idx_]*ex_,axis=1)
+    adata.obsm[pot_vkey_] = vel_potential
+    adata.obsm[rot_vkey_] = vel_rotation
+    # elif graph_method == 'knn':
+    #     knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
+    #     knn.fit(exp_LD)
+    #     distances, indices = knn.kneighbors(exp_LD)
+    #     distances, indices = distances[:,1:], indices[:,1:]
+    #     for i in range(adata.shape[0]):
+    #         ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
+    #         vel_potential[i] = -4.*edge_vel_norm*np.mean((pot_flow_[indices[i]]-pot_flow_[i])*ex_s.T,axis=1)
+    #         vel_rotation[i]  = -4.*edge_vel_norm*np.mean((rot_flow_[indices[i]]-rot_flow_[i])*ex_s.T,axis=1)
+    #     adata.obsm[pot_vkey_] = vel_potential
+    #     adata.obsm[rot_vkey_] = vel_rotation
+    
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target,normalization=False))
     source_term_ = vorticity_
-    # source_term_[idx_bd_] = 100
     streamfunc_ = -np.dot(lap_inv_,source_term_)
-    # vorticity_ = -np.dot(lap,streamfunc_)
     adata.obs[vor_key_] = vorticity_
     adata.obs[sl_key_]  = streamfunc_-np.min(streamfunc_)
 
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target,normalization=False))
     source_term_ = vorticity_
-    # source_term_[idx_bd_] = 100
     streamfunc_ = -np.dot(lap_inv_,source_term_)
-    # vorticity_ = -np.dot(lap,streamfunc_)
     adata.obs[pot_vor_key_] = vorticity_
     adata.obs[pot_sl_key_] = streamfunc_-np.min(streamfunc_)
 
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target,normalization=False))
     source_term_ = vorticity_
-    # source_term_[idx_bd_] = 100
     streamfunc_ = -np.dot(lap_inv_,source_term_)
-    # vorticity_ = -np.dot(lap,streamfunc_)
     adata.obs[rot_vor_key_] = vorticity_
     adata.obs[rot_sl_key_] = streamfunc_-np.min(streamfunc_)
 
     adata.obs[rotation_key] = np.array([np.mean(np.hstack((rot_flow_[source==i],-rot_flow_[target==i]))) for i in range(adata.shape[0])])
 
     ## Contribution ratio
     log_ = {}
@@ -658,40 +639,34 @@
 def view_stream(
     adata,
     basis = 'umap',
     vkey = 'velocity',
     potential_vkey = 'potential_velocity',
     rotation_vkey = 'rotation_velocity',
     cluster_key = 'clusters',
-    additional_key = '',
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
-
-    vkey_ = vkey
-    pot_vkey_ = potential_vkey+additional_key
-    rot_vkey_ = rotation_vkey+additional_key
-    
     
     fig,ax = plt.subplots(1,3,figsize=figsize,tight_layout=True)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey_, title='RNA velocity',ax=ax[0],color=cluster_key,
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey, title='RNA velocity',ax=ax[0],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=pot_vkey_, title='Potential flow',ax=ax[1],color=cluster_key,
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=potential_vkey, title='Potential flow',ax=ax[1],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
-    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rot_vkey_, title='Rotational flow',ax=ax[2],color=cluster_key,
+    scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
     for i in range(3):
         texts = []
         for c in np.unique(cluster):
             txt = ax[i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=legend_fontsize,ha='center', va='center',fontweight='bold',zorder=20)
             txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
             texts.append(txt)
@@ -700,15 +675,14 @@
 def view_stream_line(
     adata,
     basis = 'umap',
     contour_key = 'streamfunc',
     cluster_key = 'clusters',
     potential_key = 'potential',
     rotation_key = 'rotation',
-    additional_key = '',
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
     save_dir = None,
     save_filename = 'CellMap_stream_line',
     figsize = (24,6),
@@ -717,17 +691,17 @@
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata,basis = basis)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
-    key_ = ('%s_%s' % (contour_key,basis))+additional_key
-    pot_key_ = ('%s_%s_%s' % (potential_key,contour_key,basis))+additional_key
-    rot_key_ = ('%s_%s_%s' % (rotation_key,contour_key,basis))+additional_key
+    key_ = '%s_%s' % (contour_key,basis)
+    pot_key_ = '%s_%s_%s' % (potential_key,contour_key,basis)
+    rot_key_ = '%s_%s_%s' % (rotation_key,contour_key,basis)
     
     
     data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
     
     contour_keys = [key_, pot_key_, rot_key_]
     camps = [cmap_earth(adata.obs[key_]),'rainbow','coolwarm']
```

## Comparing `cellmap-1.0.1.dev202305060213.dist-info/METADATA` & `cellmap-1.0.1.dev202305060457.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202305060213
+Version: 1.0.1.dev202305060457
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

