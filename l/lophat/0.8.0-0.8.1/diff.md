# Comparing `tmp/lophat-0.8.0.tar.gz` & `tmp/lophat-0.8.1.tar.gz`

## Comparing `lophat-0.8.0.tar` & `lophat-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 lophat-0.8.0/Cargo.toml
--rw-r--r--   0     1000     1001      691 2023-03-09 14:38:58.000000 lophat-0.8.0/.gitignore
--rw-r--r--   0     1000     1001     1071 2023-03-07 14:26:14.000000 lophat-0.8.0/LICENSE
--rw-r--r--   0     1000     1001     4016 2023-03-23 12:01:20.000000 lophat-0.8.0/README.md
--rw-r--r--   0     1000     1001     1102 2023-03-24 12:16:44.000000 lophat-0.8.0/example.py
--rw-r--r--   0     1000     1001     2249 2023-03-24 12:16:44.000000 lophat-0.8.0/lophat.pyi
--rw-r--r--   0     1000     1001      316 2023-03-09 07:17:41.000000 lophat-0.8.0/pyproject.toml
--rw-r--r--   0     1000     1001     4104 2023-03-24 12:16:44.000000 lophat-0.8.0/src/anti_transpose.rs
--rw-r--r--   0     1000     1001     3745 2023-03-24 12:16:44.000000 lophat-0.8.0/src/column.rs
--rw-r--r--   0     1000     1001     5905 2023-03-24 12:16:44.000000 lophat-0.8.0/src/decomposition.rs
--rw-r--r--   0     1000     1001     1272 2023-03-22 10:55:15.000000 lophat-0.8.0/src/diagram.rs
--rw-r--r--   0     1000     1001     1360 2023-03-24 12:16:44.000000 lophat-0.8.0/src/indexing.rs
--rw-r--r--   0     1000     1001     4736 2023-03-24 12:16:44.000000 lophat-0.8.0/src/lib.rs
--rw-r--r--   0     1000     1001    10674 2023-03-24 12:16:44.000000 lophat-0.8.0/src/lock_free.rs
--rw-r--r--   0     1000     1001     2105 2023-03-24 12:16:44.000000 lophat-0.8.0/src/options.rs
--rw-r--r--   0     1000     1001     2450 2023-03-24 12:16:44.000000 lophat-0.8.0/timing_test.py
--rw-r--r--   0     1000     1001    19340 2023-03-24 12:16:44.000000 lophat-0.8.0/Cargo.lock
--rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 lophat-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 lophat-0.8.1/Cargo.toml
+-rw-r--r--   0     1000     1001      691 2023-03-09 14:38:58.000000 lophat-0.8.1/.gitignore
+-rw-r--r--   0     1000     1001     1071 2023-03-07 14:26:14.000000 lophat-0.8.1/LICENSE
+-rw-r--r--   0     1000     1001     4203 2023-03-27 15:27:02.000000 lophat-0.8.1/README.md
+-rw-r--r--   0     1000     1001     1154 2023-03-27 07:14:32.000000 lophat-0.8.1/example.py
+-rw-r--r--   0     1000     1001     2249 2023-03-24 12:16:44.000000 lophat-0.8.1/lophat.pyi
+-rw-r--r--   0     1000     1001      316 2023-03-09 07:17:41.000000 lophat-0.8.1/pyproject.toml
+-rw-r--r--   0     1000     1001     4028 2023-03-27 14:48:35.000000 lophat-0.8.1/src/anti_transpose.rs
+-rw-r--r--   0     1000     1001     3745 2023-03-27 14:52:52.000000 lophat-0.8.1/src/column.rs
+-rw-r--r--   0     1000     1001     5905 2023-03-31 10:49:18.000000 lophat-0.8.1/src/decomposition.rs
+-rw-r--r--   0     1000     1001     1658 2023-04-11 08:28:55.000000 lophat-0.8.1/src/diagram.rs
+-rw-r--r--   0     1000     1001     1360 2023-03-24 12:16:44.000000 lophat-0.8.1/src/indexing.rs
+-rw-r--r--   0     1000     1001     4925 2023-04-11 08:28:55.000000 lophat-0.8.1/src/lib.rs
+-rw-r--r--   0     1000     1001    11702 2023-04-11 08:28:55.000000 lophat-0.8.1/src/lock_free.rs
+-rw-r--r--   0     1000     1001     3438 2023-04-11 08:28:55.000000 lophat-0.8.1/src/options.rs
+-rw-r--r--   0     1000     1001     2416 2023-03-27 07:19:20.000000 lophat-0.8.1/timing_test.py
+-rw-r--r--   0     1000     1001    19340 2023-04-11 08:28:55.000000 lophat-0.8.1/Cargo.lock
+-rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 lophat-0.8.1/PKG-INFO
```

### Comparing `lophat-0.8.0/Cargo.toml` & `lophat-0.8.1/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lophat"
-version = "0.8.0"
+version = "0.8.1"
 edition = "2021"
 license = "MIT"
 description = "Lockfree Persistent Homology Algorithm Toolbox"
 homepage = "https://github.com/tomchaplin/lophat"
 repository = "https://github.com/tomchaplin/lophat"
 readme = "README.md"
 exclude = ["scripts/**/*", "docs/**/*"]
@@ -14,12 +14,17 @@
 name = "lophat"
 crate-type = ["lib", "cdylib"]
 
 [dependencies]
 crossbeam = "0.8.2"
 hashbrown = { version = "0.13.2", features = ["rayon"] }
 pinboard = "2.1.0"
-pyo3 = { version = "0.18.1", features = ["hashbrown", "extension-module"] }
+pyo3 = { version = "0.18.1", features = ["hashbrown", "extension-module"], optional=true }
 rayon = "1.7.0"
 
+[features]
+default = ["python", "local_thread_pool"]
+python = ["dep:pyo3"]
+local_thread_pool = []
+
 [dev-dependencies]
 proptest = "1.1.0"
```

### Comparing `lophat-0.8.0/.gitignore` & `lophat-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lophat-0.8.0/LICENSE` & `lophat-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lophat-0.8.0/README.md` & `lophat-0.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,21 +53,24 @@
 To use serial algorithm or limit number of threads, additionally provide a `LoPhatOptions` object.
 
 For more details, please consult [the Python docs](https://lophat.readthedocs.io/en/latest/).
 For example usage, see the file `example.py` or [this Google colab notebook](https://colab.research.google.com/drive/1y0_wZfvuUZfRreYPO50mo4rBlflkMcfj?usp=sharing).
 
 ## TODO
 
-- [ ] Implement clearing optimisation when V not required
 - [ ] Increase property testing
 - [ ] Write unit tests
+- [ ] Write integration tests (testing V) 
 - [ ] Benchmark
 - [ ] Add alternative column representations
 - [ ] Implement a `LoPhatOptionsBuilder` in Rust and Python
 - [ ] Abstract out matrix trait
+- [ ] Reduce memory usage when V not maintained
+- [ ] Add example Rust usage
+- [ ] Add support for returning generators (needs different logic depending on whether homology or cohomology was computed).
 
 ## References
 
 <a id="1">[1]</a> Morozov, Dmitriy, and Arnur Nigmetov.
 "Towards lockfree persistent homology."
 Proceedings of the 32nd ACM Symposium on Parallelism in Algorithms and Architectures. 2020.
```

### Comparing `lophat-0.8.0/lophat.pyi` & `lophat-0.8.1/lophat.pyi`

 * *Files identical despite different names*

### Comparing `lophat-0.8.0/src/anti_transpose.rs` & `lophat-0.8.1/src/anti_transpose.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-use hashbrown::HashSet;
-
 use crate::{Column, PersistenceDiagram};
 
 /// Re-indexes a persistence diagram, assuming that it was produced from an anti-transposed matrix.
 /// * `diagram` - the diagram to reindex.
 /// * `matrix_size` - the size of the decomposed matrix, assumed to be square.
 pub fn anti_transpose_diagram(
     mut diagram: PersistenceDiagram,
     matrix_size: usize,
 ) -> PersistenceDiagram {
     let new_paired = diagram
         .paired
         .into_iter()
         .map(|(b, d)| (matrix_size - 1 - d, matrix_size - 1 - b))
         .collect();
+    let new_unpaired = diagram
+        .unpaired
+        .into_iter()
+        .map(|idx| matrix_size - 1 - idx)
+        .collect();
     diagram.paired = new_paired;
-    let mut unpaired: HashSet<usize> = (0..matrix_size).collect();
-    for (birth, death) in diagram.paired.iter() {
-        unpaired.remove(birth);
-        unpaired.remove(death);
-    }
-    diagram.unpaired = unpaired;
+    diagram.unpaired = new_unpaired;
     diagram
 }
 
 /// Anti-transposes the input matrix (e.g. to compute cohomology).
 /// * `matrix` - a reference to a collected matrix (vector of columns).
 /// Assumes that input matrix is square.
 pub fn anti_transpose<C: Column>(matrix: &Vec<C>) -> Vec<C> {
```

### Comparing `lophat-0.8.0/src/column.rs` & `lophat-0.8.1/src/column.rs`

 * *Files identical despite different names*

### Comparing `lophat-0.8.0/src/decomposition.rs` & `lophat-0.8.1/src/decomposition.rs`

 * *Files identical despite different names*

### Comparing `lophat-0.8.0/src/diagram.rs` & `lophat-0.8.1/src/diagram.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 use hashbrown::HashSet;
+
+#[cfg(feature = "python")]
 use pyo3::prelude::*;
+
+#[cfg(feature = "python")]
 /// Stores the pairings from a matrix decomposition,
 /// as well as those columns which did not appear in a pairing.
 #[pyclass]
 #[derive(Default, Debug, Clone, PartialEq)]
 pub struct PersistenceDiagram {
     #[pyo3(get)]
     pub unpaired: HashSet<usize>,
     #[pyo3(get)]
     pub paired: HashSet<(usize, usize)>,
 }
 
+#[cfg(not(feature = "python"))]
+/// Stores the pairings from a matrix decomposition,
+/// as well as those columns which did not appear in a pairing.
+#[derive(Default, Debug, Clone, PartialEq)]
+pub struct PersistenceDiagram {
+    pub unpaired: HashSet<usize>,
+    pub paired: HashSet<(usize, usize)>,
+}
+
 impl std::fmt::Display for PersistenceDiagram {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "Paired: {:?}\nUnpaired: {:?}",
             self.paired, self.unpaired
         )
     }
 }
 
+#[cfg(feature = "python")]
 #[pymethods]
 impl PersistenceDiagram {
     fn __richcmp__(&self, other: &PyAny, cmp_op: pyo3::basic::CompareOp) -> bool {
         if let Ok(other) = other.extract::<PersistenceDiagram>() {
             match cmp_op {
                 pyo3::pyclass::CompareOp::Eq => *self == other,
                 _ => panic!("Only able to check equality between PersistenceDiagram"),
```

### Comparing `lophat-0.8.0/src/indexing.rs` & `lophat-0.8.1/src/indexing.rs`

 * *Files identical despite different names*

### Comparing `lophat-0.8.0/src/lib.rs` & `lophat-0.8.1/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 //! For many applications, [`VecColumn`] is a good choice for your columns.
 //! The function returns a [`RVDecomposition`], from which you can read off the persistence diagram.
 //! Additional options can be set by providing a [`LoPhatOptions`] struct.
 //!
 //! If you would like to force the use of the serial or parallel algorithm,
 //! use [`rv_decompose_serial`] or [`rv_decompose_lock_free`] respectively.
 
-use pyo3::prelude::*;
-use pyo3::types::PyIterator;
-
 mod anti_transpose;
 mod column;
 mod decomposition;
 mod diagram;
 mod indexing;
 mod lock_free;
 mod options;
@@ -41,25 +38,32 @@
     if options.num_threads == 1 {
         rv_decompose_serial(matrix, &options)
     } else {
         rv_decompose_lock_free(matrix, &options).into()
     }
 }
 
+#[cfg(feature = "python")]
+use pyo3::prelude::*;
+#[cfg(feature = "python")]
+use pyo3::types::PyIterator;
+
+#[cfg(feature = "python")]
 fn compute_pairings_rs<C: Column + 'static>(
     matrix: impl Iterator<Item = C>,
     options: &LoPhatOptions,
 ) -> PersistenceDiagram {
     if options.num_threads == 1 {
         rv_decompose_serial(matrix, &options).diagram()
     } else {
         rv_decompose_lock_free(matrix, &options).diagram()
     }
 }
 
+#[cfg(feature = "python")]
 fn compute_pairings_anti_transpose(
     py: Python<'_>,
     matrix: &PyAny,
     options: Option<LoPhatOptions>,
 ) -> PersistenceDiagram {
     let options = options.unwrap_or(LoPhatOptions::default());
     let matrix_as_vec: Vec<_> =
@@ -78,14 +82,15 @@
         };
     let width = matrix_as_vec.len();
     let at: Vec<_> = anti_transpose(&matrix_as_vec);
     let dgm = compute_pairings_rs(at.into_iter(), &options);
     anti_transpose_diagram(dgm, width)
 }
 
+#[cfg(feature = "python")]
 fn compute_pairings_non_transpose(
     py: Python<'_>,
     matrix: &PyAny,
     options: Option<LoPhatOptions>,
 ) -> PersistenceDiagram {
     let options = options.unwrap_or(LoPhatOptions::default());
     if let Ok(matrix_as_vec) = matrix.extract::<Vec<(usize, Vec<usize>)>>() {
@@ -99,14 +104,15 @@
         });
         compute_pairings_rs(matrix_as_rs_iter, &options)
     } else {
         panic!("Could not coerce input matrix into List[List[int]] | Iterator[List[int]]");
     }
 }
 
+#[cfg(feature = "python")]
 #[pyfunction]
 #[pyo3(signature = (matrix,anti_transpose= true, options=None))]
 fn compute_pairings(
     py: Python<'_>,
     matrix: &PyAny,
     anti_transpose: bool,
     options: Option<LoPhatOptions>,
@@ -116,12 +122,13 @@
     } else {
         compute_pairings_non_transpose(py, matrix, options)
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
+#[cfg(feature = "python")]
 fn lophat(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(compute_pairings, m)?)?;
     m.add_class::<LoPhatOptions>()?;
     Ok(())
 }
```

### Comparing `lophat-0.8.0/src/lock_free.rs` & `lophat-0.8.1/src/lock_free.rs`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,46 @@
 use crate::PersistenceDiagram;
 use crate::RVDecomposition;
 
 use crossbeam::atomic::AtomicCell;
 use hashbrown::HashSet;
 use pinboard::NonEmptyPinboard;
 use rayon::prelude::*;
-use rayon::ThreadPool;
+#[cfg(feature = "local_thread_pool")]
 use rayon::ThreadPoolBuilder;
 
+enum LoPhatThreadPool {
+    #[cfg(not(feature = "local_thread_pool"))]
+    Global(),
+    #[cfg(feature = "local_thread_pool")]
+    Local(rayon::ThreadPool),
+}
+
+impl LoPhatThreadPool {
+    fn install<OP, R>(&self, op: OP) -> R
+    where
+        OP: FnOnce() -> R + Send,
+        R: Send,
+    {
+        match self {
+            #[cfg(not(feature = "local_thread_pool"))]
+            LoPhatThreadPool::Global() => op(),
+            #[cfg(feature = "local_thread_pool")]
+            LoPhatThreadPool::Local(pool) => pool.install(op),
+        }
+    }
+}
+
 /// Stores the matrix and pivot vector behind appropriate atomic data types, as well as the algorithm options.
 /// Provides methods for reducing the matrix in parallel.
 pub struct LockFreeAlgorithm<'a, C: Column + 'static> {
     matrix: Vec<NonEmptyPinboard<(C, Option<C>)>>,
     pivots: Vec<AtomicCell<Option<usize>>>,
     options: &'a LoPhatOptions,
-    thread_pool: ThreadPool,
+    thread_pool: LoPhatThreadPool,
     max_dim: usize,
 }
 
 impl<'a, C: Column + 'static> LockFreeAlgorithm<'a, C> {
     /// Initialise atomic data structure with provided `matrix`, store algorithm options and init thread pool.
     pub fn new(matrix: impl Iterator<Item = C>, options: &'a LoPhatOptions) -> Self {
         let mut max_dim = 0;
@@ -37,18 +59,31 @@
                     NonEmptyPinboard::new((r_col, None))
                 }
             })
             .collect();
         let column_height = options.column_height.unwrap_or(matrix.len());
         let pivots: Vec<_> = (0..column_height).map(|_| AtomicCell::new(None)).collect();
         // Setup thread pool
-        let thread_pool = ThreadPoolBuilder::new()
-            .num_threads(options.num_threads)
-            .build()
-            .expect("Failed to build thread pool");
+        #[cfg(feature = "local_thread_pool")]
+        let thread_pool = LoPhatThreadPool::Local(
+            ThreadPoolBuilder::new()
+                .num_threads(options.num_threads)
+                .build()
+                .expect("Failed to build thread pool"),
+        );
+        #[cfg(not(feature = "local_thread_pool"))]
+        let thread_pool = {
+            if options.num_threads != 0 {
+                panic!(
+                    "To specify a number of threads, please enable the local_thread_pool feature"
+                );
+            }
+            LoPhatThreadPool::Global()
+        };
+        // Return options
         Self {
             matrix,
             pivots,
             options,
             thread_pool,
             max_dim,
         }
```

### Comparing `lophat-0.8.0/timing_test.py` & `lophat-0.8.1/timing_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,16 +58,16 @@
     )
 
 
 opts = LoPhatOptions(num_threads=1)
 
 
 print("Starting runs")
-clearing_opts = LoPhatOptions(min_chunk_len=1, clearing=True)
-no_clearing_opts = LoPhatOptions(min_chunk_len=1, clearing=False)
+clearing_opts = LoPhatOptions(clearing=True)
+no_clearing_opts = LoPhatOptions(clearing=False)
 
 # print("Normal clearing")
 # matrix = [get_sparse_boundary(f_val[0]) for f_val in s_tree2.get_filtration()]
 # tic1 = time.time()
 # diagram1 = compute_pairings(matrix, clearing_opts)
 # tic2 = time.time()
 # print(tic2 - tic1)
```

### Comparing `lophat-0.8.0/Cargo.lock` & `lophat-0.8.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "lophat"
-version = "0.8.0"
+version = "0.8.1"
 dependencies = [
  "crossbeam",
  "hashbrown",
  "pinboard",
  "proptest",
  "pyo3",
  "rayon",
@@ -339,17 +339,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proptest"
 version = "1.1.0"
@@ -369,17 +369,17 @@
  "rusty-fork",
  "tempfile",
  "unarray",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
  "hashbrown",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
@@ -387,49 +387,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -442,17 +442,17 @@
 name = "quick-error"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a993555f31e5a609f617c12db6250dedcac1b0a85076912c436e6fc9b2c8e6a3"
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
```

### Comparing `lophat-0.8.0/PKG-INFO` & `lophat-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lophat
-Version: 0.8.0
+Version: 0.8.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Lockfree Persistent Homology Algorithm Toolbox
 Home-Page: https://github.com/tomchaplin/lophat
 License: MIT
@@ -67,21 +67,24 @@
 To use serial algorithm or limit number of threads, additionally provide a `LoPhatOptions` object.
 
 For more details, please consult [the Python docs](https://lophat.readthedocs.io/en/latest/).
 For example usage, see the file `example.py` or [this Google colab notebook](https://colab.research.google.com/drive/1y0_wZfvuUZfRreYPO50mo4rBlflkMcfj?usp=sharing).
 
 ## TODO
 
-- [ ] Implement clearing optimisation when V not required
 - [ ] Increase property testing
 - [ ] Write unit tests
+- [ ] Write integration tests (testing V) 
 - [ ] Benchmark
 - [ ] Add alternative column representations
 - [ ] Implement a `LoPhatOptionsBuilder` in Rust and Python
 - [ ] Abstract out matrix trait
+- [ ] Reduce memory usage when V not maintained
+- [ ] Add example Rust usage
+- [ ] Add support for returning generators (needs different logic depending on whether homology or cohomology was computed).
 
 ## References
 
 <a id="1">[1]</a> Morozov, Dmitriy, and Arnur Nigmetov.
 "Towards lockfree persistent homology."
 Proceedings of the 32nd ACM Symposium on Parallelism in Algorithms and Architectures. 2020.
```

