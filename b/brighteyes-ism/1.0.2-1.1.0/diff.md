# Comparing `tmp/brighteyes-ism-1.0.2.tar.gz` & `tmp/brighteyes-ism-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brighteyes-ism-1.0.2.tar", last modified: Tue Feb 14 14:21:23 2023, max compression
+gzip compressed data, was "brighteyes-ism-1.1.0.tar", last modified: Tue Apr 11 12:56:02 2023, max compression
```

## Comparing `brighteyes-ism-1.0.2.tar` & `brighteyes-ism-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 14:21:23.877053 brighteyes-ism-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3928 2023-02-14 14:21:23.878051 brighteyes-ism-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3065 2023-02-06 17:38:53.000000 brighteyes-ism-1.0.2/README.md
--rw-rw-rw-   0        0        0      983 2023-02-14 14:07:16.000000 brighteyes-ism-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1656 2023-02-14 14:21:23.887026 brighteyes-ism-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 brighteyes-ism-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-14 14:21:23.740416 brighteyes-ism-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-02-14 14:21:23.767343 brighteyes-ism-1.0.2/src/brighteyes_ism/
--rw-rw-rw-   0        0        0      123 2023-02-06 17:07:56.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-14 14:21:23.853117 brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/
--rw-rw-rw-   0        0        0     7411 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/APR_lib.py
--rw-rw-rw-   0        0        0    15153 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/Deconv_lib.py
--rw-rw-rw-   0        0        0     7678 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/FRC_lib.py
--rw-rw-rw-   0        0        0    10935 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/FocusISM_lib.py
--rw-rw-rw-   0        0        0     6130 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/Tools_lib.py
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-14 14:21:23.866082 brighteyes-ism-1.0.2/src/brighteyes_ism/dataio/
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/dataio/__init__.py
--rw-rw-rw-   0        0        0     5786 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/dataio/mcs.py
-drwxrwxrwx   0        0        0        0 2023-02-14 14:21:23.877053 brighteyes-ism-1.0.2/src/brighteyes_ism/simulation/
--rw-rw-rw-   0        0        0    17901 2023-02-14 14:01:14.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/simulation/PSF_sim.py
--rw-rw-rw-   0        0        0     5701 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/simulation/Tubulin_sim.py
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.0.2/src/brighteyes_ism/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-14 14:21:23.800256 brighteyes-ism-1.0.2/src/brighteyes_ism.egg-info/
--rw-rw-rw-   0        0        0     3928 2023-02-14 14:21:23.000000 brighteyes-ism-1.0.2/src/brighteyes_ism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-02-14 14:21:23.000000 brighteyes-ism-1.0.2/src/brighteyes_ism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 14:21:23.000000 brighteyes-ism-1.0.2/src/brighteyes_ism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2023-02-14 14:21:23.000000 brighteyes-ism-1.0.2/src/brighteyes_ism.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-02-14 14:21:23.000000 brighteyes-ism-1.0.2/src/brighteyes_ism.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 12:56:02.651396 brighteyes-ism-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3928 2023-04-11 12:56:02.651396 brighteyes-ism-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3065 2023-02-06 17:38:53.000000 brighteyes-ism-1.1.0/README.md
+-rw-rw-rw-   0        0        0      983 2023-04-11 12:52:23.000000 brighteyes-ism-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1656 2023-04-11 12:56:02.658376 brighteyes-ism-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 brighteyes-ism-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:56:02.549666 brighteyes-ism-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 12:56:02.566650 brighteyes-ism-1.1.0/src/brighteyes_ism/
+-rw-rw-rw-   0        0        0      123 2023-02-06 17:07:56.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:56:02.625463 brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/
+-rw-rw-rw-   0        0        0     7411 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/APR_lib.py
+-rw-rw-rw-   0        0        0    15991 2023-04-07 08:56:11.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/Deconv_lib.py
+-rw-rw-rw-   0        0        0     9410 2023-04-07 12:04:30.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/FRC_lib.py
+-rw-rw-rw-   0        0        0    10935 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/FocusISM_lib.py
+-rw-rw-rw-   0        0        0     9866 2023-04-07 10:06:43.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/Tools_lib.py
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:56:02.631448 brighteyes-ism-1.1.0/src/brighteyes_ism/dataio/
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/dataio/__init__.py
+-rw-rw-rw-   0        0        0     5852 2023-04-06 15:11:23.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/dataio/mcs.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:56:02.650441 brighteyes-ism-1.1.0/src/brighteyes_ism/simulation/
+-rw-rw-rw-   0        0        0    17901 2023-02-14 14:01:14.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/simulation/PSF_sim.py
+-rw-rw-rw-   0        0        0     5701 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/simulation/Tubulin_sim.py
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.0/src/brighteyes_ism/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:56:02.588563 brighteyes-ism-1.1.0/src/brighteyes_ism.egg-info/
+-rw-rw-rw-   0        0        0     3928 2023-04-11 12:56:02.000000 brighteyes-ism-1.1.0/src/brighteyes_ism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-04-11 12:56:02.000000 brighteyes-ism-1.1.0/src/brighteyes_ism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 12:56:02.000000 brighteyes-ism-1.1.0/src/brighteyes_ism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-04-11 12:56:02.000000 brighteyes-ism-1.1.0/src/brighteyes_ism.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 12:56:02.000000 brighteyes-ism-1.1.0/src/brighteyes_ism.egg-info/top_level.txt
```

### Comparing `brighteyes-ism-1.0.2/LICENSE` & `brighteyes-ism-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.0.2/PKG-INFO` & `brighteyes-ism-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighteyes-ism
-Version: 1.0.2
+Version: 1.1.0
 Summary: A toolbox for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/brighteyes-ism
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/brighteyes-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `brighteyes-ism-1.0.2/README.md` & `brighteyes-ism-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.0.2/pyproject.toml` & `brighteyes-ism-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "scikit-image>=0.19.2", "scikit-learn", "numpy", "scipy", "matplotlib", "joblib", "poppy", 	"PyCustomFocus", "h5py", "statsmodels", "tqdm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brighteyes-ism"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="Alessandro Zunino", email="alessandro.zunino@iit.it" },
 ]
 description = "A toolbox for analysing and simulating ISM images"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
```

### Comparing `brighteyes-ism-1.0.2/setup.cfg` & `brighteyes-ism-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7269 6768 7465 7965 732d 6973   = brighteyes-is
-00000020: 6d0d 0a76 6572 7369 6f6e 203d 2031 2e30  m..version = 1.0
-00000030: 2e32 0d0a 6175 7468 6f72 203d 2041 6c65  .2..author = Ale
+00000020: 6d0d 0a76 6572 7369 6f6e 203d 2031 2e31  m..version = 1.1
+00000030: 2e30 0d0a 6175 7468 6f72 203d 2041 6c65  .0..author = Ale
 00000040: 7373 616e 6472 6f20 5a75 6e69 6e6f 0d0a  ssandro Zunino..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 2061  author_email = a
 00000060: 6c65 7373 616e 6472 6f2e 7a75 6e69 6e6f  lessandro.zunino
 00000070: 4069 6974 2e69 740d 0a75 726c 203d 2068  @iit.it..url = h
 00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000090: 6d2f 5669 6369 646f 6d69 6e69 4c61 622f  m/VicidominiLab/
 000000a0: 6272 6967 6874 6579 6573 2d69 736d 0d0a  brighteyes-ism..
```

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/APR_lib.py` & `brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/APR_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/Deconv_lib.py` & `brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/Deconv_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     B = np.conj(H)*I
     OUT =  np.real( np.fft.ifft2(B/A) )
     out = np.fft.fftshift(OUT)
     
     return out
 
 
-def deconv_RL_FFT(h, i, max_iter = 50, epsilon = None, reg = 0):
+def deconv_RL_FFT(h, i, max_iter = 50, epsilon = None, reg = 0, out = 'last'):
     """
     Richardson-Lucy deconvolution, performed using FFT
 
     Parameters
     ----------
     h : np.array (Nx x Ny)
         PSF of the system
@@ -233,14 +233,17 @@
     
     Returns
     -------
     img_deconv : np.array(Mx x My)
         Deconvolved image
     
     """
+    if out == 'all':
+        sz = [max_iter, i.shape[0], i.shape[1]]
+        obj_all = np.empty(sz)
     
     if epsilon is None:
        epsilon = np.finfo(float).eps    
 
     h = h/np.sum(h) #PSF normalization
     hT = np.flip(h)
     obj = np.ones(i.shape) #Initialization
@@ -250,20 +253,26 @@
 
         conv = convolve( obj, h, mode = 'same' )
         A = np.where(conv < epsilon, 0, i / conv)
         B = convolve( hT, A, mode = 'same' )
         C = obj / ( 1 + reg * obj )
         obj = B * C
         
+        if out == 'all':
+            obj_all[k] = obj.copy()
+        
         k += 1
     
-    return obj
+    if out == 'last':
+        return obj
+    elif out == 'all':
+        return obj_all
 
 
-def MultiImg_RL_FFT(h, i, bkg = None, max_iter = 50, pad = None, epsilon = None, reg = 0):
+def MultiImg_RL_FFT(h, i, bkg = None, max_iter = 50, pad = None, epsilon = None, reg = 0, out = 'last', verbose = False):
     """
     Multi-image Richardson-Lucy deconvolution, performed using FFT.
     It deconvolves the entire dataset, returning a single deconvoluted image.
 
     Parameters
     ----------
     h : np.array(Nx x Ny x Nch)
@@ -283,14 +292,18 @@
     Returns
     -------
     img_deconv : np.array(Nx x Ny)
         Deconvolved image
     
     """
     
+    if out == 'all':
+        sz = [max_iter, i.shape[0], i.shape[1]]
+        obj_all = np.empty(sz)
+    
     if bkg is None:
         bkg = np.zeros(i.shape)
     
     if pad is not None:
         h = PadDataset(h, pad)
         i = PadDataset(i, pad)
         
@@ -301,32 +314,46 @@
     
     h = h/np.sum(h) #PSF normalization
     hT = np.flip(h, axis=(0,1))
     obj = np.ones( i.shape[0:-1] ) #Initialization
     
     k = 0
     while k < max_iter:
-    
+        
+        if verbose == True:
+            print(k)
+        
         tmp = 0        
         
         for n in range(N):
             with np.errstate(invalid='ignore', divide='ignore'):
                 
                 conv = convolve( obj, h[:, :, n], mode = 'same' ) + bkg[:,:,n]
                 A = np.where(conv < epsilon, 0, i[:, :, n] / conv)
                 B = convolve( hT[:, :, n], A, mode = 'same' )
                 tmp += B
             
         obj = ( obj * tmp / ( 1 + reg * obj ) ) # * s[n]
+
+        if out == 'all':
+            obj_all[k] = obj.copy()
+            
         k += 1
 
     if pad is not None:
-        obj = UnpadDataset(obj, pad)
-
-    return obj
+        if out == 'last':
+            obj = UnpadDataset(obj, pad)
+        elif out == 'all':
+            for n in range(max_iter):
+                obj_all[n] = UnpadDataset(obj_all[n], pad)
+            
+    if out == 'last':
+        return obj
+    elif out == 'all':
+        return obj_all
 
 def PSF_FRC(i_1, i_2):
     """
     PSFs estimation with Fourier Ring Correlation
     from two replicas of the same image.
 
     Parameters
@@ -349,74 +376,76 @@
     
     frc_result = FRC.FRC_resolution(i_1[:,:,ref], i_2[:,:,ref], px = 1, method = 'fixed')
 
     sigma_frc = frc_result[0] / (2*np.sqrt(2*np.log(2)))
     
     usf = 100
     
-    shift_frc, _ = APR.APR(i_1, usf, ref, 1, degree=None)
+    shift_frc, _ = APR.APR(i_1, usf, ref, 1)
 
     shift_frc_x, shift_frc_y = -shift_frc[:,1], -shift_frc[:,0]
     
     psf_frc = np.empty(i_1.shape)
 
     x = np.arange(sz[0]) - sz[0]//2
     y = np.arange(sz[1]) - sz[1]//2
     X, Y = np.meshgrid(x, y)
 
-    Fingerprint = np.sum(i_1 + i_2, axis = (0,1) )
+    Fingerprint = np.sum(i_1 + i_2, axis = (0,1) ).astype('float64')
     Fingerprint /= np.sum(Fingerprint)
 
     for i in range( sz[-1] ):
         psf_frc[:, :, i] = gauss2d(X, Y, shift_frc_x[i], shift_frc_y[i], sigma_frc)
         psf_frc[:, :, i] = psf_frc[:, :, i] * Fingerprint[i] / np.sum( psf_frc[:, :, i])
         
     return psf_frc
 
 
-def FRC_MultiImg_RL_FFT(i_1, i_2, max_iter = 50, pad = None, epsilon = None, reg = 0, sum_data = True):
+def FRC_MultiImg_RL_FFT(dset, max_iter = 50, pad = None, epsilon = None, reg = 0):
     """
     Multi-image Richardson-Lucy deconvolution, performed using FFT.
     It deconvolves the entire dataset, returning a single deconvoluted image.
     The PSF is automatically estimated with Fourier Ring Correlation from two
     replicas of the same image.
 
     Parameters
     ----------
-    i_1 : np.array(Nx x Ny x Nch)
-        ISM dataset
-    i_2 : np.array(Nx x Ny x Nch)
-        ISM dataset
+    i_1 : np.ndarray
+        ISM dataset (Nx x Ny x Nt x Nch)
     max_iter : int
         Number of iteration
     pad : np.array(Nx x Ny x Nch)
         Number of pixels used for zer-padding the image on each side
     epsilon : float
         Minimum value of the denominator.
         Used to avoid division by zero (default = float.eps)
     reg : float
         Regularization parameter (Tikhonov)
-    sum_data : bool
-        Sum both images
-    
+        
     Returns
     -------
     img_deconv : np.array(Nx x Ny)
         Deconvolved image
     
     """
     
-    psf_frc = PSF_FRC(i_1, i_2)
-    
-    if sum_data == True:
-        img = i_1 + i_2
-        obj = MultiImg_RL_FFT(psf_frc, img, max_iter = max_iter, pad = pad, epsilon = epsilon, reg = reg)
+    Nt = dset.shape[-2]
+   
+    if Nt % 2 == 0:
+        img_even = dset[:, :, 0::2, :].sum(axis = -2)
+        img_odd  = dset[:, :, 1::2, :].sum(axis = -2)
     else:
-        obj = MultiImg_RL_FFT(psf_frc, i_1, max_iter = max_iter, pad = pad, epsilon = epsilon, reg = reg)
-        
+        img_even = dset[:, :, 0:-1:2, :].sum(axis = -2)
+        img_odd  = dset[:, :, 1::2, :].sum(axis = -2)
+    
+    psf_frc = PSF_FRC(img_even, img_odd)
+    
+    img = dset.sum(axis = -2)
+    obj = MultiImg_RL_FFT(psf_frc, img, max_iter = max_iter, pad = pad, epsilon = epsilon, reg = reg)
+ 
     return obj, psf_frc
 
 
 def MultiImg_RL_FFT_2(h, i, max_iter = 50, pad = None, epsilon = None, reg = 0):
     """
     Multi-image Richardson-Lucy deconvolution, performed using FFT.
     It deconvolves each image of the dataset, returning Nch  deconvoluted images.
```

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/FRC_lib.py` & `brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/FRC_lib.py`

 * *Files 11% similar despite different names*

```diff
@@ -253,15 +253,58 @@
     elif method == '5sigma':
         th, idx = nsigma_threshold(k, frc_smooth, I1, 5)
 
     res_um = (1/k_interp[idx])
     
     return res_um, k, frc, k_interp, frc_smooth, th
 
-def plotFRC(res_um, k, frc, k_interp, frc_smooth, th):
+def timeFRC(dset, px = 1, method = 'fixed'):
+    """
+    Fourier Ring Correlation analysis. It requires a single dataset with a
+    temporal dimension to generate two images using the even and odd indices
+    of the time axis. Then, it estimates the resolution using the FRC analysis.
+
+    Parameters
+    ----------
+    dset : np.ndarray
+        dataset (Nx x Ny x Nt)
+    px : float
+        Pixel size of the images
+    Method : str
+        Threshold criterium. If 'fixed', it uses the 1/7 threshold.
+        Other possibilities are '3sigma' and '5sigma'
+
+    Returns
+    -------
+    res_um : float
+        Estimated resolution, in real units
+    k : np.array( np.sqrt(N**2 + M**2) )
+        Array of spatial frequencies
+    frc : np.array( np.sqrt(N**2 + M**2) )
+        Array of raw FRC
+    k_interp : np.array( 100 x np.sqrt(N**2 + M**2) )
+        Interpolated array of spatial frequencies
+    frc_smooth : np.array( 100 x np.sqrt(N**2 + M**2) )
+        Interpolated and smoothed FRC curve
+    th : np.array( 100 x np.sqrt(N**2 + M**2) )
+        Threshold curve
+    """
+    
+    if dset.shape[-1] % 2 == 0:
+        img_even = dset[:, :, 0::2].sum(axis = -1)
+        img_odd  = dset[:, :, 1::2].sum(axis = -1)
+    else:
+        img_even = dset[:, :, 0:-1:2].sum(axis = -1)
+        img_odd  = dset[:, :, 1::2].sum(axis = -1)
+    
+    res_um, k, frc, k_interp, frc_smooth, th = FRC_resolution(img_even, img_odd, px = px, method = method)
+    
+    return res_um, k, frc, k_interp, frc_smooth, th
+
+def plotFRC(res_um, k, frc, k_interp, frc_smooth, th, fig = None, ax = None):
     """
     Visualization of the results of the FRC curve. The inputs are exactly the
     outputs of FRC_resolution function.
 
     Parameters
     ----------
     res_um : float
@@ -278,26 +321,30 @@
         Threshold curve
 
     Returns
     -------
     None.
     """
     
-    plt.figure()
-    plt.plot(k, frc, '.', label = 'FRC - raw')
-    plt.plot(k_interp, frc_smooth, '.', label = 'FRC - smoothed')
-    plt.plot(k_interp, th, label = 'Threshold')
+    if fig == None or ax == None:
+        fig, ax = plt.subplots()
+        
+    ax.plot(k, frc, '.', label = 'FRC - raw')
+    ax.plot(k_interp, frc_smooth, '-', linewidth = 3, label = 'FRC - smoothed')
+    ax.plot(k_interp, th, linewidth = 3, label = 'Threshold')
     
-    plt.legend()
+    ax.legend()
     
     idx = (np.abs(k_interp - 1/res_um)).argmin()
     
-    plt.plot(k_interp[idx], frc_smooth[idx], 'o', markersize = 10)
+    ax.plot(k_interp[idx], frc_smooth[idx], 'o', markersize = 6)
     
     k_max = k[-1]*np.sqrt( 2 )/2
-    plt.xlim( ( 0, k_max ) )
-    plt.ylim( ( 0, 1 ) )
+    ax.set_xlim( ( 0, k_max ) )
+    ax.set_ylim( ( -0.05, 1.05 ) )
+    
+    ax.set_xlabel(r'k ($\mu m ^{-1}$)')
+    ax.set_ylabel('FRC')
     
-    plt.xlabel(r'k ($\mu m ^{-1}$)')
-    plt.ylabel('FRC')
+    ax.set_title(f'Resolution = {res_um:.3f} $\mu m$')
     
-    return None
+    return fig, ax
```

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism/analysis/FocusISM_lib.py` & `brighteyes-ism-1.1.0/src/brighteyes_ism/analysis/FocusISM_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism/dataio/mcs.py` & `brighteyes-ism-1.1.0/src/brighteyes_ism/dataio/mcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,18 @@
     
     __slots__ = ['version', 'comment', 'rangex', 'rangey', 'rangez', 'nbin', 'dt', 'nx', 'ny', 'nz', 'nrep', 'calib_x', 'calib_y', 'calib_z']
     
     def __init__(self, f):
             
         # MCS version
         self.version = f.attrs['data_format_version']
-        self.comment = f.attrs['comment']
+        try:
+            self.comment = f.attrs['comment']
+        except:
+            self.comment = ''
         
         # range in um
         self.rangex = f['configurationGUI'].attrs['range_x']
         self.rangey = f['configurationGUI'].attrs['range_y']
         self.rangez = f['configurationGUI'].attrs['range_z']
         
         # number of time bins per pixel
```

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism/simulation/PSF_sim.py` & `brighteyes-ism-1.1.0/src/brighteyes_ism/simulation/PSF_sim.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism/simulation/Tubulin_sim.py` & `brighteyes-ism-1.1.0/src/brighteyes_ism/simulation/Tubulin_sim.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism.egg-info/PKG-INFO` & `brighteyes-ism-1.1.0/src/brighteyes_ism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighteyes-ism
-Version: 1.0.2
+Version: 1.1.0
 Summary: A toolbox for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/brighteyes-ism
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/brighteyes-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `brighteyes-ism-1.0.2/src/brighteyes_ism.egg-info/SOURCES.txt` & `brighteyes-ism-1.1.0/src/brighteyes_ism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

