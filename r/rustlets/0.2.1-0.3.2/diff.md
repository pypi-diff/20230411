# Comparing `tmp/rustlets-0.2.1.tar.gz` & `tmp/rustlets-0.3.2.tar.gz`

## Comparing `rustlets-0.2.1.tar` & `rustlets-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 rustlets-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123     4087 2023-04-11 05:54:03.000000 rustlets-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      123      739 2023-04-11 05:54:03.000000 rustlets-0.2.1/.gitignore
--rw-r--r--   0     1001      123    11934 2023-04-11 05:55:12.000000 rustlets-0.2.1/Cargo.lock
--rw-r--r--   0     1001      123      572 2023-04-11 05:54:03.000000 rustlets-0.2.1/README.md
--rw-r--r--   0     1001      123     1077 2023-04-11 05:54:03.000000 rustlets-0.2.1/cwtfuncs.py
--rw-r--r--   0     1001      123       10 2023-04-11 05:55:13.000000 rustlets-0.2.1/dist/rustlets-0.2.1.tar.gz
--rw-r--r--   0     1001      123      734 2023-04-11 05:54:03.000000 rustlets-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123     2341 2023-04-11 05:54:03.000000 rustlets-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123      370 2023-04-11 05:54:03.000000 rustlets-0.2.1/src/main.rs
--rw-r--r--   0     1001      123     7782 2023-04-11 05:54:03.000000 rustlets-0.2.1/src/waveletanalysis.rs
--rw-r--r--   0     1001      123     4289 2023-04-11 05:54:03.000000 rustlets-0.2.1/test/queenofthenight/freqshift.py
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 rustlets-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 rustlets-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      123     4087 2023-04-11 07:33:00.000000 rustlets-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123      739 2023-04-11 07:33:00.000000 rustlets-0.3.2/.gitignore
+-rw-r--r--   0     1001      123    11934 2023-04-11 07:34:14.000000 rustlets-0.3.2/Cargo.lock
+-rw-r--r--   0     1001      123      572 2023-04-11 07:33:00.000000 rustlets-0.3.2/README.md
+-rw-r--r--   0     1001      123     1121 2023-04-11 07:33:00.000000 rustlets-0.3.2/cwtfuncs.py
+-rw-r--r--   0     1001      123       10 2023-04-11 07:34:14.000000 rustlets-0.3.2/dist/rustlets-0.3.2.tar.gz
+-rw-r--r--   0     1001      123      748 2023-04-11 07:33:00.000000 rustlets-0.3.2/pyproject.toml
+-rw-r--r--   0     1001      123     2207 2023-04-11 07:33:00.000000 rustlets-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      123      370 2023-04-11 07:33:00.000000 rustlets-0.3.2/src/main.rs
+-rw-r--r--   0     1001      123     7642 2023-04-11 07:33:00.000000 rustlets-0.3.2/src/waveletanalysis.rs
+-rw-r--r--   0     1001      123     4289 2023-04-11 07:33:00.000000 rustlets-0.3.2/test/queenofthenight/freqshift.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 rustlets-0.3.2/PKG-INFO
```

### Comparing `rustlets-0.2.1/.github/workflows/ci.yml` & `rustlets-0.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rustlets-0.2.1/.gitignore` & `rustlets-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rustlets-0.2.1/Cargo.lock` & `rustlets-0.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
  "strength_reduce",
  "transpose",
  "version_check",
 ]
 
 [[package]]
 name = "rustlets"
-version = "0.2.1"
+version = "0.3.2"
 dependencies = [
  "ndarray",
  "num",
  "num-complex",
  "num-traits",
  "numpy",
  "pyo3",
```

### Comparing `rustlets-0.2.1/README.md` & `rustlets-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `rustlets-0.2.1/cwtfuncs.py` & `rustlets-0.3.2/cwtfuncs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     hz=10180
     length = 1.0
     times = np.arange(0,length,1/hz)
     samples = signal.chirp(times, f0=2200, f1=1500, t1=1, method='linear')
     samples = samples + signal.chirp(times, f0=600, f1=1100, t1=1, method='linear') + signal.gausspulse(times,fc=700)
     #samples = samples + signal.chirp(times, f0=20000, f1=8000, t1=1, method='linear')
 
-
-    cwtmat,scales = rustlets.cwt_morlet(samples,hz,10)
+    scales = rustlets.gen_scales(length, hz, 8)
+    cwtmat = rustlets.cwt_morlet(samples,hz,scales)
 
     freqs = 1 / (scales * rustlets.morlet_wavelength(2 * np.pi))
 
     plt.plot(times,samples,label="original")
     plt.show()
 
     plt.pcolormesh(times,freqs, np.abs(cwtmat), cmap='viridis', shading='gouraud')
```

### Comparing `rustlets-0.2.1/pyproject.toml` & `rustlets-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [tool.poetry]
 name = "rustlets"
-version = "0.2.0"
-description = "A wavelet library written in Rust, with bindings to python."
+version = "0.3.2"
+description = "A multithreaded wavelet library written in Rust, with bindings to python."
 authors = ["Jack Ruder <jackruder14@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jackruder/rustlets"
 keywords = ["multithreaded", "transform", "wavelet", "continuous"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `rustlets-0.2.1/src/waveletanalysis.rs` & `rustlets-0.3.2/src/waveletanalysis.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,26 @@
     }
 }
 
 pub fn morlet_wavelength(omega_0: f64) -> f64 {
     4.0 * PI / (omega_0 + f64::sqrt(2.0 + omega_0.powi(2)))
 }
 
-fn gen_scales(t: f64, hz: f64, steps: f64) -> Array1<f64> {
+pub fn gen_scales(t: f64, hz: f64, steps: f64) -> Array1<f64> {
     let min_scale: f64 = 2.0 / hz; // smallest scale is twice the timestep
     let num_scales: usize = (f64::log2(t / min_scale) * steps) as usize; // log2 spacing of scales
     
     let mut scales: Array1<f64> = Array::zeros(num_scales+1);
     for j in 0..(num_scales+1){
         scales[j] = min_scale * f64::powf(2.0, j as f64 / steps);// compute the scale
     }
     return scales;
 }
 
-pub fn cwt(timeseries: &ArrayView1<f64>, wavelet: fn(f64, f64, f64) -> Complex64, hz: f64, steps: f64, normalize: bool) -> (Array2<Complex64>, Arc<Array1<f64>>){
-    let steps = steps as f64;
-
+pub fn cwt(timeseries: &ArrayView1<f64>, wavelet: fn(f64, f64, f64) -> Complex64, hz: f64, scales: &ArrayView1<f64>, normalize: bool) -> Array2<Complex64>{
     let mut nrm = 0;
     if normalize { // should we normalize wavelets for equal energy?
         nrm = 1; // set normalization exponent to 1, nfac^1 = nfac
     }
 
     // cast real timeseries to complex
     let mut data: Vec<Complex64> = timeseries.iter().map(|x| Complex64{re: *x, im: 0.0}).collect();
@@ -55,17 +53,15 @@
     for i in 0..data.len() {
         data[i] = data[i] / (n as f64); // normalize by 1/len, we will transform back to time later
                                         // rustfft documentation states output is not normalized
     }
 
     let t = n0 as f64 / hz;
     let data = Arc::new(Array::from_vec(data));
-    let scales = Arc::new(gen_scales(t, hz, steps));
-
-    //let newscales: Vec<f64> = scales.iter().map(|s| s * rescale).collect();
+    let scales = Arc::new(scales);
 
     // generate angular frequencies for wavelet
     let mut angs: Array1<f64> = Array::zeros(n); 
     let c: f64 = 2.0 * PI / (n as f64) * hz;
     for i in 0..n {
         if i <= n/2 {
             angs[i] = c * i as f64; // pos to n/2
@@ -112,15 +108,15 @@
     drop(tx); // stop listening
 
     for (i, mut cwtrow) in rx {
         let mut cwtrowi = cwtm.row_mut(i);
         cwtrowi.assign(&mut cwtrow);
     }
 
-    return (cwtm, scales)
+    return cwtm
 }
 
 pub fn icwt_morlet(cwtm: &ArrayView2<Complex64>, scales: &ArrayView1<f64>, times: &ArrayView1<f64>) -> Array1<f64> {
     let mut diffs: Array2<Complex64> = Array::zeros((scales.len(),times.len()));
     for i in 0..scales.len() {
         calctools::diff(&cwtm.row(i), times, &mut diffs.row_mut(i)); //differentiate each row
     }
```

### Comparing `rustlets-0.2.1/test/queenofthenight/freqshift.py` & `rustlets-0.3.2/test/queenofthenight/freqshift.py`

 * *Files identical despite different names*

### Comparing `rustlets-0.2.1/PKG-INFO` & `rustlets-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustlets
-Version: 0.2.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # rustlets
```

