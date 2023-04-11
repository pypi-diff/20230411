# Comparing `tmp/rustlets-0.2.0.tar.gz` & `tmp/rustlets-0.2.1.tar.gz`

## Comparing `rustlets-0.2.0.tar` & `rustlets-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 rustlets-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     4087 2023-04-03 07:13:51.000000 rustlets-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0     1001      123      739 2023-04-03 07:13:51.000000 rustlets-0.2.0/.gitignore
--rw-r--r--   0     1001      123    10699 2023-04-03 07:15:34.000000 rustlets-0.2.0/Cargo.lock
--rw-r--r--   0     1001      123      485 2023-04-03 07:13:51.000000 rustlets-0.2.0/README.md
--rw-r--r--   0     1001      123     1226 2023-04-03 07:13:51.000000 rustlets-0.2.0/cwtfuncs.py
--rw-r--r--   0     1001      123       10 2023-04-03 07:15:35.000000 rustlets-0.2.0/dist/rustlets-0.2.0.tar.gz
--rw-r--r--   0     1001      123      734 2023-04-03 07:13:51.000000 rustlets-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123     1209 2023-04-03 07:13:51.000000 rustlets-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123      415 2023-04-03 07:13:51.000000 rustlets-0.2.0/src/main.rs
--rw-r--r--   0     1001      123     7605 2023-04-03 07:13:51.000000 rustlets-0.2.0/src/waveletanalysis.rs
--rw-r--r--   0     1001      123     4289 2023-04-03 07:13:51.000000 rustlets-0.2.0/test/queenofthenight/freqshift.py
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 rustlets-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 rustlets-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123     4087 2023-04-11 05:54:03.000000 rustlets-0.2.1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123      739 2023-04-11 05:54:03.000000 rustlets-0.2.1/.gitignore
+-rw-r--r--   0     1001      123    11934 2023-04-11 05:55:12.000000 rustlets-0.2.1/Cargo.lock
+-rw-r--r--   0     1001      123      572 2023-04-11 05:54:03.000000 rustlets-0.2.1/README.md
+-rw-r--r--   0     1001      123     1077 2023-04-11 05:54:03.000000 rustlets-0.2.1/cwtfuncs.py
+-rw-r--r--   0     1001      123       10 2023-04-11 05:55:13.000000 rustlets-0.2.1/dist/rustlets-0.2.1.tar.gz
+-rw-r--r--   0     1001      123      734 2023-04-11 05:54:03.000000 rustlets-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123     2341 2023-04-11 05:54:03.000000 rustlets-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123      370 2023-04-11 05:54:03.000000 rustlets-0.2.1/src/main.rs
+-rw-r--r--   0     1001      123     7782 2023-04-11 05:54:03.000000 rustlets-0.2.1/src/waveletanalysis.rs
+-rw-r--r--   0     1001      123     4289 2023-04-11 05:54:03.000000 rustlets-0.2.1/test/queenofthenight/freqshift.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 rustlets-0.2.1/PKG-INFO
```

### Comparing `rustlets-0.2.0/.github/workflows/ci.yml` & `rustlets-0.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rustlets-0.2.0/.gitignore` & `rustlets-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rustlets-0.2.0/Cargo.lock` & `rustlets-0.2.1/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -24,38 +24,60 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "matrixmultiply"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+dependencies = [
+ "rawpointer",
+]
+
+[[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "ndarray"
+version = "0.15.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
+dependencies = [
+ "matrixmultiply",
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "rawpointer",
+]
+
+[[package]]
 name = "num"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
 dependencies = [
  "num-bigint",
  "num-complex",
@@ -124,14 +146,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "numpy"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
+dependencies = [
+ "libc",
+ "ndarray",
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "pyo3",
+ "rustc-hash",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
@@ -241,23 +278,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rawpointer"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "rustfft"
 version = "6.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e17d4f6cbdb180c9f4b2a26bbf01c4e647f1e1dea22fe8eb9db54198b32f9434"
 dependencies = [
  "num-complex",
  "num-integer",
@@ -266,19 +315,21 @@
  "strength_reduce",
  "transpose",
  "version_check",
 ]
 
 [[package]]
 name = "rustlets"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
+ "ndarray",
  "num",
  "num-complex",
  "num-traits",
+ "numpy",
  "pyo3",
  "rustfft",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
```

### Comparing `rustlets-0.2.0/cwtfuncs.py` & `rustlets-0.2.1/cwtfuncs.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,28 +10,25 @@
     length = 1.0
     times = np.arange(0,length,1/hz)
     samples = signal.chirp(times, f0=2200, f1=1500, t1=1, method='linear')
     samples = samples + signal.chirp(times, f0=600, f1=1100, t1=1, method='linear') + signal.gausspulse(times,fc=700)
     #samples = samples + signal.chirp(times, f0=20000, f1=8000, t1=1, method='linear')
 
 
-    cwt_list,scales_list = rustlets.cwt_morlet(samples,hz,10)
+    cwtmat,scales = rustlets.cwt_morlet(samples,hz,10)
 
-    scales = np.array(scales_list)
     freqs = 1 / (scales * rustlets.morlet_wavelength(2 * np.pi))
-    cwtmat = np.array(cwt_list,dtype=np.complex64).reshape((len(scales),-1))[:,:len(times)]
 
     plt.plot(times,samples,label="original")
     plt.show()
 
-    #plt.pcolormesh(times,freqs, np.abs(cwtmat), cmap='viridis', shading='gouraud')
-    #plt.show()
-
+    plt.pcolormesh(times,freqs, np.abs(cwtmat), cmap='viridis', shading='gouraud')
+    plt.show()
 
-    f_rec = np.array(rustlets.icwt_morlet(cwt_list,scales,times))
+    f_rec = rustlets.icwt_morlet(cwtmat,scales,times)
 
     plt.plot(times,samples,label="original")
     plt.plot(times,f_rec,label="recovered")
     plt.legend()
     plt.show()
 
     plt.plot(times,f_rec/samples,label="ratio")
```

### Comparing `rustlets-0.2.0/pyproject.toml` & `rustlets-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rustlets-0.2.0/src/waveletanalysis.rs` & `rustlets-0.2.1/src/waveletanalysis.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use std::{f64::consts::PI, sync::{mpsc, Arc}, thread};
 use num_complex::{Complex64, ComplexFloat};
 use rustfft::{self, FftPlanner};
+use ndarray::prelude::*;
 
 pub fn chirp(t_0: f64, t_1: f64, f_0: f64, f_1: f64) -> f64 {
     f64::sin(f_0 + (f_1 - f_0) * t_0 / t_1) 
 }
 
 
 pub fn morlet_fourier(s: f64,omega: f64,omega_0: f64) -> Complex64{
@@ -17,26 +18,26 @@
     }
 }
 
 pub fn morlet_wavelength(omega_0: f64) -> f64 {
     4.0 * PI / (omega_0 + f64::sqrt(2.0 + omega_0.powi(2)))
 }
 
-fn gen_scales(t: f64, hz: f64, steps: f64) -> Vec<f64> {
+fn gen_scales(t: f64, hz: f64, steps: f64) -> Array1<f64> {
     let min_scale: f64 = 2.0 / hz; // smallest scale is twice the timestep
     let num_scales: usize = (f64::log2(t / min_scale) * steps) as usize; // log2 spacing of scales
     
-    let mut scales: Vec<f64> = Vec::with_capacity(num_scales+1);
+    let mut scales: Array1<f64> = Array::zeros(num_scales+1);
     for j in 0..(num_scales+1){
-        scales.push(min_scale * f64::powf(2.0, j as f64 / steps)) // compute the scale
+        scales[j] = min_scale * f64::powf(2.0, j as f64 / steps);// compute the scale
     }
     return scales;
 }
 
-pub fn cwt(timeseries: &Vec<f64>, wavelet: fn(f64, f64, f64) -> Complex64, hz: f64, steps: f64, normalize: bool) -> (Vec<Vec<Complex64>>, Vec<f64>){
+pub fn cwt(timeseries: &ArrayView1<f64>, wavelet: fn(f64, f64, f64) -> Complex64, hz: f64, steps: f64, normalize: bool) -> (Array2<Complex64>, Arc<Array1<f64>>){
     let steps = steps as f64;
 
     let mut nrm = 0;
     if normalize { // should we normalize wavelets for equal energy?
         nrm = 1; // set normalization exponent to 1, nfac^1 = nfac
     }
 
@@ -53,94 +54,95 @@
     fft.process(&mut data); // do the fft
     for i in 0..data.len() {
         data[i] = data[i] / (n as f64); // normalize by 1/len, we will transform back to time later
                                         // rustfft documentation states output is not normalized
     }
 
     let t = n0 as f64 / hz;
-    let data = Arc::new(data);
+    let data = Arc::new(Array::from_vec(data));
     let scales = Arc::new(gen_scales(t, hz, steps));
 
     //let newscales: Vec<f64> = scales.iter().map(|s| s * rescale).collect();
 
     // generate angular frequencies for wavelet
-    let mut angs: Vec<f64> = Vec::with_capacity(n); 
+    let mut angs: Array1<f64> = Array::zeros(n); 
     let c: f64 = 2.0 * PI / (n as f64) * hz;
     for i in 0..n {
         if i <= n/2 {
-            angs.push(c * i as f64) // pos to n/2
+            angs[i] = c * i as f64; // pos to n/2
         } else {
-            angs.push(c * (i as f64 - n as f64)) // wrap to [-n/2, -1]
+            angs[i] = c * (i as f64 - n as f64); // wrap to [-n/2, -1]
         }
     }
     let angs = Arc::new(angs);
 
     let ifft = planner.plan_fft_inverse(n);
     
 
-    let mut cwtm = vec![vec![Complex64{ re: 0.0f64, im: 0.0f64 }; n0]; scales.len()]; //output
+    let mut cwtm = Array::zeros((scales.len(),n0));
     let (tx,rx) = mpsc::channel();
 
     let num_scales = scales.len();
     
     for i in 0..num_scales {
         // clone ownerships
         let scale = scales[i];
         let txi = tx.clone();
         let angs = Arc::clone(&angs);
         let data = Arc::clone(&data);
         let ifft = Arc::clone(&ifft);
         
+        
         // spawn one thread per scale
         thread::spawn(move || {
-            let norm = f64::sqrt(2.0 * PI * scale * hz).powi(nrm); // 1 if normalize = false
-            
-            let mut eval = Vec::with_capacity(num_scales);
-            eval = angs.iter()
-                .zip::<Vec<Complex64>>(data.to_vec())
-                .map(|(&w, f)| f * norm * wavelet(scale,w,2.0*PI))
-                .collect();
-
+            let norm = Complex64::from(f64::sqrt(2.0 * PI * scale * hz).powi(nrm)); // 1 if normalize = false
+            let daught_waves = angs.mapv(|w| wavelet(scale,w,2.0*PI));
+            let mut eval: Array1<Complex64> = norm * daught_waves * data.view();
             //let mut scratch = Vec::with_capacity(ifft.get_outofplace_scratch_len());
 
             //ifft.process_outofplace_with_scratch(&mut eval,&mut cwtm[i],&mut scratch);
-            ifft.process(&mut eval);
-            eval.truncate(n0); // return to original unpadded length
-            txi.send((i,eval)).unwrap();
+            if let Some(eval_slice) = eval.as_slice_mut(){
+                ifft.process(eval_slice);
+            } else {
+                println!("IFFT ERROR"); //TODO handle
+            }
+            txi.send((i,eval.slice_move(s![..n0]))).unwrap();
         });
     }
 
     drop(tx); // stop listening
 
-    for (i,cwtrow) in rx {
-        cwtm[i] = cwtrow;
+    for (i, mut cwtrow) in rx {
+        let mut cwtrowi = cwtm.row_mut(i);
+        cwtrowi.assign(&mut cwtrow);
     }
-    return (cwtm, scales.to_vec())
-}
 
+    return (cwtm, scales)
+}
 
-pub fn icwt_morlet(cwtm: &Vec<Vec<Complex64>>, scales: &Vec<f64>,times: &Vec<f64>) -> Vec<f64> {
-    let mut diffs = vec![vec![Complex64{ re: 0.0f64, im: 0.0f64 }; times.len()]; scales.len()];
+pub fn icwt_morlet(cwtm: &ArrayView2<Complex64>, scales: &ArrayView1<f64>, times: &ArrayView1<f64>) -> Array1<f64> {
+    let mut diffs: Array2<Complex64> = Array::zeros((scales.len(),times.len()));
     for i in 0..scales.len() {
-        calctools::diff(&cwtm[i], times, &mut diffs[i]); //differentiate each row
+        calctools::diff(&cwtm.row(i), times, &mut diffs.row_mut(i)); //differentiate each row
     }
     
     //recovered signal
-    let mut rec: Vec<f64> = Vec::with_capacity(times.len());
+    let mut rec: Array1<f64> = Array::zeros(times.len());
 
     for j in 0..times.len() { //integrate over each column and push the scaled result
-        let integral: Complex64 = calctools::trapz_col(&mut diffs, scales, j);
-        rec.push(PI * integral.im() / (2.0 * PI).sqrt());
+        let integral: Complex64 = calctools::trapz_col(&diffs.view(), scales, j);
+        rec[j] = PI * integral.im() / (2.0 * PI).sqrt();
     }
     return rec;
 
 
 }
 
 mod calctools {
+    use ndarray::prelude::*;
     use num_complex::{Complex64};
     use std::f64::consts::PI;
 
     fn centraldiff3(f_prev: &Complex64, f_next: &Complex64, x_prev: &f64, x_next: &f64) -> Complex64 {
         (*f_next - *f_prev)/(*x_next - *x_prev)
     }
 
@@ -148,15 +150,15 @@
         (*f_next - *f)/(*x_next - *x)
     }
 
     fn backwarddiff(f_prev: &Complex64, f: &Complex64, x_prev: &f64, x: &f64) -> Complex64 {
         (*f - *f_prev)/(*x - *x_prev)
     }
 
-    pub fn diff(f: &[Complex64], x: &Vec<f64>, target: &mut[Complex64]){ //Complex64ODO handle mismatch lengths
+    pub fn diff(f: &ArrayView1<Complex64>, x: &ArrayView1<f64>, target: &mut ArrayViewMut1<Complex64>){ //Complex64ODO handle mismatch lengths
         for i in 0..f.len() {
             if i == 0 {
                 target[i] = forwarddiff(&f[0], &f[1], &x[0], &x[1]);
             } 
             else if i == f.len() - 1 {
                 target[i] = backwarddiff(&f[i-1], &f[i], &x[i-1], &x[i]);
             }
@@ -190,19 +192,19 @@
             sum += h * (f[i] + f[i_next]) / 2.0;
         }
         return sum;
         
     }
 
     // compute the integral over the column of a 2d array
-    pub fn trapz_col(f: &Vec<Vec<Complex64>>, x: &Vec<f64>, col: usize) -> Complex64 { //Complex64ODO handle mismatch lengths
+    pub fn trapz_col(f: &ArrayView2<Complex64>, x: &ArrayView1<f64>, col: usize) -> Complex64 { //Complex64ODO handle mismatch lengths
         let mut sum = Complex64{re: 0.0f64, im: 0.0f64}; 
-        for i in 0..f.len()-1 {
+        for i in 0..x.len()-1 {
             let h = x[i + 1] - x[i];
-            sum += h * (f[i][col] + f[i+1][col]) / 2.0;
+            sum += h * (f[[i, col]] + f[[i+1, col]]) / 2.0;
         }
         return sum;
         
     }
 
     fn phase_unwrap(phases: &mut[f64]) { // T(N^2/2 - N/2), bad
         let op = phases.to_vec();// old phases
```

### Comparing `rustlets-0.2.0/test/queenofthenight/freqshift.py` & `rustlets-0.2.1/test/queenofthenight/freqshift.py`

 * *Files identical despite different names*

### Comparing `rustlets-0.2.0/PKG-INFO` & `rustlets-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustlets
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # rustlets
@@ -19,12 +19,18 @@
 
 Install maturin python package into virtual environment. Install numpy as well
 
 For example, with pip, do 
 pip install maturin
 
 
-You will also need matplotlib, scipy to run demos
+You will also need matplotlib, scipy, numpy to run demos
 
 
 To build, run maturin develop --release
 
+## usage
+see cwtfuncs.py
+
+## TODO
+Move Array types to ArcArray for cleanliness
+
```

