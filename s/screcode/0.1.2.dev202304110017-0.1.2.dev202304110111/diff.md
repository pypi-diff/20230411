# Comparing `tmp/screcode-0.1.2.dev202304110017-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202304110111-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 118811 bytes, number of entries: 6
+Zip file size: 119179 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    56897 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304110017.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304110017.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304110017.dist-info/RECORD
-6 files, 207683 bytes uncompressed, 117907 bytes compressed:  43.2%
+-rw-r--r--  2.0 unx    58817 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304110111.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304110111.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304110111.dist-info/RECORD
+6 files, 209603 bytes uncompressed, 118275 bytes compressed:  43.6%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304110017.dist-info/METADATA
+Filename: screcode-0.1.2.dev202304110111.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304110017.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202304110111.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304110017.dist-info/RECORD
+Filename: screcode-0.1.2.dev202304110111.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -35,15 +35,15 @@
 		----------
 		fast_algorithm : boolean, default=True
 			If True, the fast algorithm is conducted. The upper bound of parameter :math:`\ell` is set in ``fast_algorithm_ell_ub``.
 		
 		fast_algorithm_ell_ub : int, default=1000
 			Upper bound of parameter :math:`\ell` for the fast algorithm. Must be of range [1,:math:`\infity`).
 		
-		seq_target : {'RNA','ATAC','Hi-C'}, default='RNA'
+		seq_target : {'RNA','ATAC','Hi-C','Multiome'}, default='RNA'
 			Sequencing target. If 'ATAC', the preprocessing (odd-even stabilization) will be performed before the regular algorithm. 
 
 		version : int default='1'
 			Version of RECODE. 
 		
 		verbose : boolean, default=True
 			If False, all running messages are not displayed.
@@ -80,14 +80,16 @@
 		self.anndata_key = anndata_key
 		self.verbose = verbose
 		self.unit,self.Unit = 'gene','Gene'
 		if seq_target == 'ATAC':
 			self.unit,self.Unit = 'peak','Peak'
 		if seq_target == 'Hi-C':
 			self.unit,self.Unit = 'bin','Bin'
+		if seq_target == 'Multiome':
+			self.unit,self.Unit = 'feature','Feature'
 		self.log_ = {}
 		self.log_['seq_target'] = self.seq_target
 		self.fit_idx = False
 		self.logger = logging.getLogger("argument checking")
 		if verbose:
 			self.logger.setLevel(logging.WARNING)
 		else:
@@ -100,14 +102,23 @@
 		if type(X) == anndata._core.anndata.AnnData:
 			if scipy.sparse.issparse(X.X):
 				return X.X.toarray()
 			elif type(X.X) == np.ndarray:
 				return X.X
 			else:
 				raise TypeError("Data type error: ndarray or anndata is available.")
+			if 'feature_types' in adata.var.keys():
+				if (set(adata.var['feature_types']) == {'Gene Expression'}) & (self.seq_target != 'RNA'):
+					self.logger.warning('Warning: Input data may be scRNA-seq data. Please add option seq_target=\'RNA\' like screcode.RECODE(seq_target=\'RNA\'). ')
+				elif (set(adata.var['feature_types']) == {'Peaks'}) & (self.seq_target != 'ATAC'):
+					self.logger.warning('Warning: Input data may be scATAC-seq data. Please add option seq_target=\'ATAC\' like screcode.RECODE(seq_target=\'ATAC\'). ')
+				elif (set(adata.var['feature_types']) == {'Gene Expression', 'Peaks'}) & (self.seq_target != 'Multiome'):
+					self.logger.warning('Warning: Input data may be multiome (scRNA-seq + scATAC-seq) data. Please add option seq_target=\'Multiome\' like screcode.RECODE(seq_target=\'Multiome\'). ')
+		elif self.seq_target == 'Multiome':
+			raise TypeError("Data type error: only anndata type is acceptable for multiome (scRNA-seq + scATAC-seq) data.")
 		elif scipy.sparse.issparse(X):
 			self.logger.warning('RECODE does not support sparse input. The input and output are transformed as regular matricies. ')
 			return X.toarray()
 		elif type(X) == np.ndarray:
 			return X
 		else:
 			raise TypeError("Data type error: ndarray or anndata is available.")
@@ -193,15 +204,17 @@
 		X_mat = self._check_datatype(X)
 		if np.linalg.norm(X_mat-np.array(X_mat,dtype=int)) > 0:
 			self.logger.warning("Warning: RECODE is applicable for count data (integer matrix). Plese make sure the data type.")
 		self.idx_nonsilent = np.sum(X_mat,axis=0) > 0
 		self.X_temp = X_mat[:,self.idx_nonsilent]
 		if self.seq_target == 'ATAC':
 			self.X_temp = self._ATAC_preprocessing(self.X_temp)
-		
+		if self.seq_target == 'Multiome':
+			self.idx_atac = X.var['feature_types'][self.idx_nonsilent] == 'Peaks'
+			self.X_temp[:,self.idx_atac] = self._ATAC_preprocessing(self.X_temp[:,self.idx_atac])
 		X_nUMI = np.sum(self.X_temp,axis=1)
 		X_scaled = (self.X_temp.T/X_nUMI).T
 		X_scaled_mean = np.mean(X_scaled,axis=0)
 		noise_var = np.mean(self.X_temp.T/np.sum(self.X_temp,axis=1)/np.sum(self.X_temp,axis=1),axis=1)
 		noise_var[noise_var==0] = 1
 		X_norm = (X_scaled-X_scaled_mean)/np.sqrt(noise_var)
 		X_norm_var = np.var(X_norm,axis=0)
@@ -476,16 +489,22 @@
 		x,y = np.mean(X_scaled,axis=0),norm_var
 		idx_nonsig, idx_sig = y <= 1, y > 1
 		fig = plt.figure(figsize=figsize)
 		plt.rcParams['xtick.direction'] = 'in'
 		plt.rcParams['ytick.direction'] = 'in'
 		spec = matplotlib.gridspec.GridSpec(ncols=2, nrows=1,width_ratios=[4, 1],wspace=0.)
 		ax0 = fig.add_subplot(spec[0])
-		ax0.scatter(x[idx_sig],y[idx_sig],color='b',s=ps,label='significant %s' % self.unit,zorder=2)
-		ax0.scatter(x[idx_nonsig],y[idx_nonsig],color='r',s=ps,label='non-significant %s' % self.unit,zorder=3)
+		if self.seq_target == 'Multiome':
+			ax0.scatter(x[idx_sig & (self.idx_atac==False)],y[idx_sig & (self.idx_atac==False)],color='b',s=ps,label='significant genes' ,zorder=2,marker='x')
+			ax0.scatter(x[idx_sig & self.idx_atac],y[idx_sig & self.idx_atac],color='b',s=ps,label='significant peaks',zorder=2,marker='o',facecolor='None')
+			ax0.scatter(x[idx_nonsig & (self.idx_atac==False)],y[idx_nonsig & (self.idx_atac==False)],color='r',s=ps,label='non-significant genes',zorder=3,marker='x')
+			ax0.scatter(x[idx_nonsig & self.idx_atac],y[idx_nonsig & self.idx_atac],color='r',s=ps,label='non-significant peaks',zorder=3,marker='o',facecolor='None')
+		else:
+			ax0.scatter(x[idx_sig],y[idx_sig],color='b',s=ps,label='significant %s' % self.unit,zorder=2)
+			ax0.scatter(x[idx_nonsig],y[idx_nonsig],color='r',s=ps,label='non-significant %s' % self.unit,zorder=3)
 		ax0.axhline(1,color='gray',ls='--',lw=2,zorder=1)
 		ax0.set_xscale('log')
 		ax0.set_yscale('log')
 		ax0.set_title(title,fontsize=14)
 		ax0.set_xlabel('Mean of scaled data',fontsize=14)
 		ax0.set_ylabel('NVSN variance',fontsize=14)
 		ax0.legend(loc='upper left',borderaxespad=0,fontsize=14,markerscale=2).get_frame().set_alpha(0)
```

## Comparing `screcode-0.1.2.dev202304110017.dist-info/METADATA` & `screcode-0.1.2.dev202304110111.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304110017
+Version: 0.1.2.dev202304110111
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

