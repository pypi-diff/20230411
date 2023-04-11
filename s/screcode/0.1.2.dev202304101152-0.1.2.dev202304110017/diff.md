# Comparing `tmp/screcode-0.1.2.dev202304101152-py3-none-any.whl.zip` & `tmp/screcode-0.1.2.dev202304110017-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 118728 bytes, number of entries: 6
+Zip file size: 118811 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 screcode/__init__.py
 -rw-r--r--  2.0 unx   148900 b- defN 80-Jan-01 00:00 screcode/integrecode_test.ipynb
--rw-r--r--  2.0 unx    56674 b- defN 80-Jan-01 00:00 screcode/screcode.py
--rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304101152.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304101152.dist-info/WHEEL
-?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304101152.dist-info/RECORD
-6 files, 207460 bytes uncompressed, 117824 bytes compressed:  43.2%
+-rw-r--r--  2.0 unx    56897 b- defN 80-Jan-01 00:00 screcode/screcode.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304110017.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 screcode-0.1.2.dev202304110017.dist-info/WHEEL
+?rw-r--r--  2.0 unx      500 b- defN 16-Jan-01 00:00 screcode-0.1.2.dev202304110017.dist-info/RECORD
+6 files, 207683 bytes uncompressed, 117907 bytes compressed:  43.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: screcode/integrecode_test.ipynb
 Comment: 
 
 Filename: screcode/screcode.py
 Comment: 
 
-Filename: screcode-0.1.2.dev202304101152.dist-info/METADATA
+Filename: screcode-0.1.2.dev202304110017.dist-info/METADATA
 Comment: 
 
-Filename: screcode-0.1.2.dev202304101152.dist-info/WHEEL
+Filename: screcode-0.1.2.dev202304110017.dist-info/WHEEL
 Comment: 
 
-Filename: screcode-0.1.2.dev202304101152.dist-info/RECORD
+Filename: screcode-0.1.2.dev202304110017.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## screcode/screcode.py

```diff
@@ -201,15 +201,15 @@
 		X_nUMI = np.sum(self.X_temp,axis=1)
 		X_scaled = (self.X_temp.T/X_nUMI).T
 		X_scaled_mean = np.mean(X_scaled,axis=0)
 		noise_var = np.mean(self.X_temp.T/np.sum(self.X_temp,axis=1)/np.sum(self.X_temp,axis=1),axis=1)
 		noise_var[noise_var==0] = 1
 		X_norm = (X_scaled-X_scaled_mean)/np.sqrt(noise_var)
 		X_norm_var = np.var(X_norm,axis=0)
-		recode_ = RECODE_core(variance_estimate=False,fast_algorithm=self.fast_algorithm,fast_algorithm_ell_ub=self.fast_algorithm_ell_ub,version=self.version)
+		recode_ = RECODE_core(variance_estimate=False,fast_algorithm=self.fast_algorithm,fast_algorithm_ell_ub=self.fast_algorithm_ell_ub,version=self.version,verbose=self.verbose)
 		recode_.fit(X_norm)
 
 		# self.X_fit = X_mat
 		self.n_all = X_mat.shape[0]
 		self.d_all = X_mat.shape[1]
 		self.d_nonsilent = sum(self.idx_nonsilent)
 		self.noise_var = noise_var
@@ -1387,15 +1387,16 @@
 		self,
 		solver = 'variance',
 		variance_estimate = True,
 		fast_algorithm = True,
 		fast_algorithm_ell_ub = 1000,
 		ell_manual = 10,
 		ell_min = 3,
-		version = 1
+		version = 1,
+		verbose = True,
 	):
 		"""
 		The core part of RECODE (for non-randam sampling data). 
 
 		Parameters
 		----------
 		solver : {'variance','manual'}
@@ -1426,14 +1427,21 @@
 		self.fast_algorithm = fast_algorithm
 		self.fast_algorithm_ell_ub = fast_algorithm_ell_ub
 		self.ell_manual = ell_manual
 		self.ell_min = ell_min
 		self.fit_idx = False
 		self.version = version 
 		self.RECODE_done = False
+		self.verbose = verbose
+		self.logger = logging.getLogger("argument checking")
+		if verbose:
+			self.logger.setLevel(logging.WARNING)
+		else:
+			self.logger.setLevel(logging.ERROR)
+
 	
 	def _noise_reductor(
 		self,
 		X,
 		L,
 		U,
 		Xmean,
```

## Comparing `screcode-0.1.2.dev202304101152.dist-info/METADATA` & `screcode-0.1.2.dev202304110017.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screcode
-Version: 0.1.2.dev202304101152
+Version: 0.1.2.dev202304110017
 Summary: RECODE - resolution of the curse of dimensionality in single-cell data analysis
 Home-page: https://github.com/yusuke-imoto-lab/RECODE
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

