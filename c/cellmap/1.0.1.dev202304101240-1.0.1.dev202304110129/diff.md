# Comparing `tmp/cellmap-1.0.1.dev202304101240-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304110129-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8550 bytes, number of entries: 5
+Zip file size: 8546 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    40811 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101240.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304101240.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304101240.dist-info/RECORD
-5 files, 42942 bytes uncompressed, 7796 bytes compressed:  81.8%
+-rw-r--r--  2.0 unx    40660 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304110129.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304110129.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304110129.dist-info/RECORD
+5 files, 42791 bytes uncompressed, 7792 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101240.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304110129.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101240.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304110129.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304101240.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304110129.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -303,25 +303,25 @@
             idx_s = source == i
             idx_t = target == i
             ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
             ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
             vel_potential[i] = 2*(np.sum((adata.obs[potential_key][source[idx_s]].values-adata.obs[potential_key][target[idx_s]].values)*ex_s.T,axis=1) + \
                                 np.sum((adata.obs[potential_key][target[idx_t]].values-adata.obs[potential_key][source[idx_t]].values)*ex_t.T,axis=1))
         adata.obsm[pot_vkey_] = vel_potential
-        adata.obsm[rot_vkey_]  = adata.obsm['velocity_umap']-vel_potential
+        adata.obsm[rot_vkey_]  = adata.obsm[pot_vkey_]-vel_potential
     elif graph_method == 'knn':
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_LD)
         distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         for i in range(adata.shape[0]):
             ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
             vel_potential[i] = -2*np.sum((adata.obs[potential_key].values[indices[i]]-adata.obs[potential_key].values[i])*ex_s.T,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
-        adata.obsm[rot_vkey_]  = adata.obsm['velocity_umap']-vel_potential
+        adata.obsm[rot_vkey_]  = adata.obsm[pot_vkey_]-vel_potential
 
     ## Contribution ratio
     log_ = {}
     log_["Contribution_ratio"] = {}
     norm_grad = np.linalg.norm(pot_flow)
     norm_curl = np.linalg.norm(rot_flow)
     log_["Contribution_ratio"]['Potential'] = '{:.2%}'.format(norm_grad/(norm_grad+norm_curl))
@@ -376,15 +376,14 @@
     else:
         exp_HD = adata.layers[exp_key]
     
     vel_HD = adata.obsm[vel_key] if vel_key in adata.obsm.keys() else adata.layers[vel_key]
     if logscale_vel:
         vel_HD = (1e+4*vel_HD.T/adata.obs['n_counts'].values).T/np.power(2,exp_HD)
     exp_LD = adata.obsm[exp_2d_key][:,:2] if exp_2d_key in adata.obsm.keys() else adata.layers[exp_2d_key][:,:2]
-    vel_LD = adata.obsm[vel_2d_key][:,:2] if vel_2d_key in adata.obsm.keys() else adata.layers[vel_2d_key][:,:2]
     
     n_node_ = exp_HD.shape[0]
     if graph_method == 'Delauney':
         tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
         source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
@@ -405,15 +404,14 @@
     lap = -np.dot(div_mat,grad_mat)
     lap_inv = np.linalg.pinv(lap)
     
     for gene in genes:
         X1,X2 = exp_HD[:,adata.var.index == gene][source],exp_HD[:,adata.var.index == gene][target]
         V1,V2 = vel_HD[:,adata.var.index == gene][source],vel_HD[:,adata.var.index == gene][target]
         Dis = np.linalg.norm(exp_HD[target]-exp_HD[source],axis=1)
-        # Dis[Dis==0] = 1
         edge_vel = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
         source_term = np.dot(div_mat,edge_vel)
         potential = np.dot(lap_inv,source_term)
         adata.obs[potential_key+'_Gene_%s' % gene] = potential - np.min(potential)
 
 def view(
     adata,
```

## Comparing `cellmap-1.0.1.dev202304101240.dist-info/METADATA` & `cellmap-1.0.1.dev202304110129.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304101240
+Version: 1.0.1.dev202304110129
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

