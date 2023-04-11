# Comparing `tmp/pyskani-0.1.0.tar.gz` & `tmp/pyskani-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyskani-0.1.0.tar", last modified: Thu Feb  9 17:42:46 2023, max compression
+gzip compressed data, was "pyskani-0.1.1.tar", last modified: Tue Apr 11 11:01:17 2023, max compression
```

## Comparing `pyskani-0.1.0.tar` & `pyskani-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 17:42:46.111319 pyskani-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-02-09 17:42:42.000000 pyskani-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-09 17:42:42.000000 pyskani-0.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    50594 2023-02-09 17:42:42.000000 pyskani-0.1.0/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-09 17:42:42.000000 pyskani-0.1.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-09 17:42:42.000000 pyskani-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-02-09 17:42:46.111319 pyskani-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-02-09 17:42:42.000000 pyskani-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-09 17:42:46.000000 pyskani-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 17:42:46.107319 pyskani-0.1.0/pyskani/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 17:42:46.107319 pyskani-0.1.0/pyskani/_skani/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/_skani/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/_skani/hit.rs
--rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/_skani/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/_skani/sketch.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/_skani/utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/_skani.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 17:42:46.111319 pyskani-0.1.0/pyskani/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1414238 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/tests/e.coli-EC590.fasta.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1424962 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/tests/e.coli-K12.fasta.gz
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/tests/fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/tests/test_ani.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-02-09 17:42:42.000000 pyskani-0.1.0/pyskani/tests/unittest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 17:42:46.107319 pyskani-0.1.0/pyskani.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-02-09 17:42:46.000000 pyskani-0.1.0/pyskani.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-09 17:42:46.000000 pyskani-0.1.0/pyskani.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 17:42:46.000000 pyskani-0.1.0/pyskani.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-09 17:42:46.000000 pyskani-0.1.0/pyskani.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 17:42:46.000000 pyskani-0.1.0/pyskani.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-02-09 17:42:46.111319 pyskani-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-02-09 17:42:42.000000 pyskani-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:01:17.186598 pyskani-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 11:01:08.000000 pyskani-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-11 11:01:08.000000 pyskani-0.1.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    49004 2023-04-11 11:01:08.000000 pyskani-0.1.1/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-11 11:01:08.000000 pyskani-0.1.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-11 11:01:08.000000 pyskani-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-11 11:01:17.186598 pyskani-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-11 11:01:08.000000 pyskani-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 11:01:17.000000 pyskani-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:01:17.178597 pyskani-0.1.1/pyskani/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:01:17.182597 pyskani-0.1.1/pyskani/_skani/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/_skani/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/_skani/hit.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/_skani/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/_skani/sketch.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/_skani/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/_skani.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:01:17.186598 pyskani-0.1.1/pyskani/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1414238 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/tests/e.coli-EC590.fasta.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1424962 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/tests/e.coli-K12.fasta.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/tests/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/tests/test_ani.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-11 11:01:08.000000 pyskani-0.1.1/pyskani/tests/unittest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:01:17.182597 pyskani-0.1.1/pyskani.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-11 11:01:17.000000 pyskani-0.1.1/pyskani.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-11 11:01:17.000000 pyskani-0.1.1/pyskani.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:01:17.000000 pyskani-0.1.1/pyskani.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 11:01:17.000000 pyskani-0.1.1/pyskani.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:01:17.000000 pyskani-0.1.1/pyskani.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-11 11:01:17.186598 pyskani-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-11 11:01:08.000000 pyskani-0.1.1/setup.py
```

### Comparing `pyskani-0.1.0/COPYING` & `pyskani-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/Cargo.lock` & `pyskani-0.1.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -38,25 +38,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
-]
-
-[[package]]
 name = "autocfg"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0dde43e75fd43e8a1bf86103336bc699aa8d17ad1be60c76c0bdfd4828e19b78"
 dependencies = [
  "autocfg 1.1.0",
 ]
@@ -284,38 +273,14 @@
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
-name = "clap"
-version = "3.2.23"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
-dependencies = [
- "atty",
- "bitflags",
- "clap_lex",
- "indexmap",
- "strsim",
- "termcolor",
- "textwrap",
-]
-
-[[package]]
-name = "clap_lex"
-version = "0.2.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
-dependencies = [
- "os_str_bytes",
-]
-
-[[package]]
 name = "cloudabi"
 version = "0.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ddfc5b9aa5d4507acaf872de71051dfd0e309860e88966e1051e462a077aac4f"
 dependencies = [
  "bitflags",
 ]
@@ -617,23 +582,14 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.1.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
@@ -963,15 +919,15 @@
 
 [[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -983,20 +939,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d84eb1409416d254e4a9c8fa56cc24701755025b458f0fcd8e59e1f5f40c23bf"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
-name = "os_str_bytes"
-version = "6.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -1156,15 +1106,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyskani"
-version = "0.0.1"
+version = "0.1.1"
 dependencies = [
  "bincode",
  "built",
  "pyo3",
  "pyo3-built",
  "skani",
 ]
@@ -1531,21 +1481,20 @@
  "lazy_static",
  "log",
  "thread-id",
 ]
 
 [[package]]
 name = "skani"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3e40cf4ff4ab2724b3e7cb674966df43924b93c9ca54a7996d2b9a9999797ff"
+checksum = "b5c3a5362b16be2c22766be0c0a1ecbe5ee8f557cadfbf7d7a7883f77e99303e"
 dependencies = [
  "bincode",
  "bio",
- "clap",
  "fastrand",
  "fxhash",
  "gbdt",
  "gcollections",
  "intervallum",
  "log",
  "needletail",
@@ -1582,20 +1531,14 @@
  "lazy_static",
  "nalgebra",
  "num-traits",
  "rand 0.8.5",
 ]
 
 [[package]]
-name = "strsim"
-version = "0.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
-
-[[package]]
 name = "strum"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "063e6045c0e62079840579a7e47a355ae92f60eb74daaf156fb1e84ba164e63f"
 
 [[package]]
 name = "strum_macros"
@@ -1633,20 +1576,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "textwrap"
-version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
-
-[[package]]
 name = "thiserror"
 version = "1.0.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
 dependencies = [
  "thiserror-impl",
 ]
```

### Comparing `pyskani-0.1.0/Cargo.toml` & `pyskani-0.1.1/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyskani"
-version = "0.1.0"
+version = "0.1.1"
 authors = ["Martin Larralde <martin.larralde@embl.de>"]
 license = "MIT"
 publish = false
 edition = "2021"
 build = "pyskani/_skani/build.rs"
 
 [lib]
@@ -13,18 +13,21 @@
 
 [build-dependencies.built]
 version = "0.4"
 features = ["chrono"]
 
 [dependencies]
 bincode = "1.3.3"
-skani = "0.1.0"
 pyo3 = "0.18.1"
 pyo3-built = "0.4.7"
 
+[dependencies.skani]
+version = "0.1.1"
+default-features = false
+
 [features]
 default = []
 extension-module = ["pyo3/extension-module"]
 nightly = ["pyo3/nightly"]
 
 [[test]]
 name = "unittest"
```

### Comparing `pyskani-0.1.0/PKG-INFO` & `pyskani-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyskani
-Version: 0.1.0
+Version: 0.1.1
 Summary: PyO3 bindings and Python interface to skani, a method for fast fast genomic identity calculation using sparse chaining.
 Home-page: https://github.com/althonos/pyskani
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/pyskani/issues
 Project-URL: Changelog, https://github.com/althonos/pyskani/blob/master/CHANGELOG.md
```

### Comparing `pyskani-0.1.0/README.md` & `pyskani-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/pyskani/__init__.py` & `pyskani-0.1.1/pyskani/__init__.py`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/pyskani/_skani/hit.rs` & `pyskani-0.1.1/pyskani/_skani/hit.rs`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 use pyo3::prelude::*;
 use pyo3::types::PyString;
 use skani::types::AniEstResult;
 
 /// A single hit found when querying a `~pyskani.Database` with a genome.
 ///
 /// Attributes:
-///     identity (`float`):
+///     identity (`float`): The estimated Average Nucleotide Identity
+///         between the query and reference genomes.
 ///     query_name (`str`): The name of the query genome.
 ///     reference_name (`str`): The name of the reference genome.
 ///     query_fraction (`float`): The fraction of the query sequence
 ///         covered by the alignment.
 ///     reference_fraction (`float`): The fraction of the reference
 ///         sequence covered by the alignment.
 ///
```

### Comparing `pyskani-0.1.0/pyskani/_skani/lib.rs` & `pyskani-0.1.1/pyskani/_skani/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 mod utils;
 
 #[allow(dead_code)]
 mod build {
     include!(concat!(env!("OUT_DIR"), "/built.rs"));
 }
 
-use std::sync::RwLock;
 use std::borrow::Cow;
 use std::collections::HashMap;
 use std::collections::HashSet;
 use std::fs::File;
 use std::io::BufReader;
 use std::path::Path;
 use std::path::PathBuf;
+use std::sync::RwLock;
 
 use pyo3::exceptions::PyFileExistsError;
 use pyo3::exceptions::PyKeyError;
 use pyo3::exceptions::PyOSError;
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
@@ -94,14 +94,21 @@
                     Ok((_, raw_sketch)) => Ok(Cow::Owned(Sketch::from(raw_sketch))),
                 }
             }
         }
     }
 }
 
+/// A database storing sketched genomes.
+///
+/// The database contains two different sketch collections with different
+/// compression levels: marker sketches, which are heavily compressed, and
+/// always kept in memory; and genome sketches, which take more memory, but
+/// may be stored inside an external file.
+///
 #[pyclass(module = "pyskani._skani")]
 pub struct Database {
     params: SketchParams,
     markers: RwLock<Vec<Sketch>>,
     sketches: RwLock<DatabaseStorage>,
 }
 
@@ -424,37 +431,35 @@
     /// Add a reference genome to the database.
     ///
     /// This method is a shortcut for `Database.add_draft` when a genome is
     /// complete (i.e. only contains a single contig).
     ///
     /// Arguments:
     ///     name (`object`): The name of the reference genome to add.
-    ///     contigs (`str`, `bytes`, `bytearray` or `memoryview`): The contigs 
+    ///     contigs (`str`, `bytes`, `bytearray` or `memoryview`): The contigs
     ///         of the reference genome.
     ///
     #[pyo3(signature = (name, *contigs, seed=true))]
     pub fn sketch(&mut self, name: String, contigs: &PyTuple, seed: bool) -> PyResult<()> {
         // Get a view on the contigs
         let contents = contigs
             .into_iter()
             .map(|item| self::utils::as_bytes(item))
             .collect::<PyResult<Vec<_>>>()?;
-        let views = contents.iter()
-            .map(|cow| cow.as_ref());
+        let views = contents.iter().map(|cow| cow.as_ref());
 
         // Release the GIL while sketching
         let py = contigs.py();
         let (sketch, marker) = py.allow_threads(|| {
-            self._sketch(name, views, seed)
-                .map(|sketch| {
-                    let marker = skani::types::Sketch::get_markers_only(sketch.as_ref()).into();
-                    (sketch, marker)
-                })
+            self._sketch(name, views, seed).map(|sketch| {
+                let marker = skani::types::Sketch::get_markers_only(sketch.as_ref()).into();
+                (sketch, marker)
+            })
         })?;
-          
+
         // Record sketches
         self.markers
             .write()
             .map_err(|_| self::utils::poisoned_lock_error())?
             .push(marker);
         self.sketches
             .write()
@@ -463,15 +468,15 @@
         Ok(())
     }
 
     /// Query the database with a genome.
     ///      
     /// Arguments:
     ///     name (`str`): The name of the query genome.
-    ///     contigs (`str`, `bytes`, `bytearray` or `memoryview`): The contigs 
+    ///     contigs (`str`, `bytes`, `bytearray` or `memoryview`): The contigs
     ///         of the query genome.
     ///
     /// Keyword Arguments:
     ///     seed (`bool`): Use a seeded random number generator to ensure
     ///         reproducibility of results.
     ///     learned_ani (`bool` or `None`): Use a regression model to
     ///         compute ANI, using a model trained on MAGs. Pass `True`
@@ -494,19 +499,18 @@
         seed: bool,
         learned_ani: Option<bool>,
         median: bool,
         robust: bool,
     ) -> PyResult<Vec<Hit>> {
         // Get a view on the contigs
         let contents = contigs
-        .into_iter()
-        .map(|item| self::utils::as_bytes(item))
-        .collect::<PyResult<Vec<_>>>()?;
-        let views = contents.iter()
-        .map(|cow| cow.as_ref());
+            .into_iter()
+            .map(|item| self::utils::as_bytes(item))
+            .collect::<PyResult<Vec<_>>>()?;
+        let views = contents.iter().map(|cow| cow.as_ref());
         // Release the GIL while querying
         let py = contigs.py();
         py.allow_threads(move || {
             // Sketch query
             let query = self._sketch(name, views, seed)?;
             // Build command parameters
             let command_params = CommandParams {
@@ -521,58 +525,67 @@
                 robust,
                 median,
                 sparse: false,
                 full_matrix: false,
                 max_results: 1_000_000_000,
                 individual_contig_q: false,
                 individual_contig_r: false,
-                min_aligned_frac: skani::params::D_FRAC_COVER_CUTOFF.parse::<f64>().unwrap() / 100.0,
+                min_aligned_frac: skani::params::D_FRAC_COVER_CUTOFF.parse::<f64>().unwrap()
+                    / 100.0,
                 keep_refs: true,
                 est_ci: Default::default(),
                 learned_ani_cmd: learned_ani.is_some(),
                 learned_ani: learned_ani.unwrap_or(false),
                 detailed_out: false,
             };
             // Search marker sketches first
             let mut shortlist = HashSet::new();
-            for marker in self.markers.read().map_err(|_| self::utils::poisoned_lock_error())?.iter() {
+            for marker in self
+                .markers
+                .read()
+                .map_err(|_| self::utils::poisoned_lock_error())?
+                .iter()
+            {
                 if skani::chain::check_markers_quickly(
                     query.as_ref(),
                     marker.as_ref(),
                     command_params.screen_val,
                 ) {
                     let name = Path::new(&marker.as_ref().file_name)
-                    .file_name()
-                    .unwrap()
-                    .to_os_string()
+                        .file_name()
+                        .unwrap()
+                        .to_os_string()
                         .into_string()
                         .unwrap();
                     shortlist.insert(name);
                 }
             }
             // Search full sketches
             let mut hits = Vec::new();
             for name in shortlist.iter() {
-                let guard = self.sketches.read()
+                let guard = self
+                    .sketches
+                    .read()
                     .map_err(|_| self::utils::poisoned_lock_error())?;
                 let reference = &*guard.load(&name)?;
                 let map_params = skani::chain::map_params_from_sketch(
                     reference.as_ref(),
                     self.params.use_aa,
                     &command_params,
                 );
-                let ani_res = skani::chain::chain_seeds(reference.as_ref(), query.as_ref(), map_params);
+                let ani_res =
+                    skani::chain::chain_seeds(reference.as_ref(), query.as_ref(), map_params);
                 if ani_res.ani > 0.5 {
                     hits.push(Hit::from(ani_res));
                 }
             }
             // Apply regression model for ANI correction
             // FIXME: maybe pre-load model, to avoid having to deserialize on every query?
             let learned = learned_ani.unwrap_or_else(|| {
-                skani::parse::use_learned_ani(self.params.c, false, false, robust, median)
+                skani::regression::use_learned_ani(self.params.c, false, false, robust, median)
             });
             if let Some(ref model) = skani::regression::get_model(self.params.c, learned) {
                 for hit in hits.iter_mut() {
                     skani::regression::predict_from_ani_res(&mut hit.as_mut(), model);
                 }
             }
             Ok(hits)
@@ -623,15 +636,22 @@
                 .unwrap(); // FIXME
             let sketch_path = folder.join(format!("{}.sketch", name));
             if !overwrite && sketch_path.exists() {
                 return Err(PyFileExistsError::new_err(
                     sketch_path.display().to_string(),
                 ));
             }
-            self._save_sketch(sketch_path, &*self.sketches.read().map_err(|_| self::utils::poisoned_lock_error())?.load(&name)?)?;
+            self._save_sketch(
+                sketch_path,
+                &*self
+                    .sketches
+                    .read()
+                    .map_err(|_| self::utils::poisoned_lock_error())?
+                    .load(&name)?,
+            )?;
         }
         Ok(())
     }
 
     /// Flush the database.
     ///
     /// This does nothing for a database loaded in memory. For a database
```

### Comparing `pyskani-0.1.0/pyskani/_skani/sketch.rs` & `pyskani-0.1.1/pyskani/_skani/sketch.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use pyo3::prelude::*;
 
+/// A sketched genome.
 #[pyclass(module = "pyskani._skani")]
 #[derive(Clone)]
 pub struct Sketch {
     sketch: skani::types::Sketch,
 }
 
 impl AsRef<skani::types::Sketch> for Sketch {
```

### Comparing `pyskani-0.1.0/pyskani/_skani/utils.rs` & `pyskani-0.1.1/pyskani/_skani/utils.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::borrow::Cow;
 
-use pyo3::prelude::*;
 use pyo3::buffer::PyBuffer;
 use pyo3::exceptions::PyRuntimeError;
-use pyo3::types::PyString;
+use pyo3::prelude::*;
 use pyo3::types::PyBytes;
+use pyo3::types::PyString;
 
 /// Try to obtain a path from a Python object using `os.fsdecode`.
 pub fn fsdecode<'py>(object: &'py PyAny) -> PyResult<&PyString> {
     let py = object.py();
     py.import(pyo3::intern!(py, "os"))?
         .call_method1(pyo3::intern!(py, "fsdecode"), (object,))?
         .downcast::<PyString>()
@@ -27,11 +27,11 @@
     } else {
         let buffer = PyBuffer::get(object)?;
         let contents = buffer.to_vec(py)?;
         Ok(Cow::Owned(contents))
     }
 }
 
-/// Create a new error 
+/// Create a new error
 pub fn poisoned_lock_error() -> PyErr {
     PyRuntimeError::new_err("Poisoned lock")
-}
+}
```

### Comparing `pyskani-0.1.0/pyskani/_skani.pyi` & `pyskani-0.1.1/pyskani/_skani.pyi`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/pyskani/tests/e.coli-EC590.fasta.gz` & `pyskani-0.1.1/pyskani/tests/e.coli-EC590.fasta.gz`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/pyskani/tests/e.coli-K12.fasta.gz` & `pyskani-0.1.1/pyskani/tests/e.coli-K12.fasta.gz`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/pyskani/tests/fasta.py` & `pyskani-0.1.1/pyskani/tests/fasta.py`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/pyskani/tests/test_ani.py` & `pyskani-0.1.1/pyskani/tests/test_ani.py`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/pyskani/tests/test_database.py` & `pyskani-0.1.1/pyskani/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/pyskani/tests/unittest.rs` & `pyskani-0.1.1/pyskani/tests/unittest.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 
 use pyo3::prelude::PyResult;
 use pyo3::types::PyDict;
 use pyo3::types::PyList;
 use pyo3::types::PyModule;
 use pyo3::Python;
 
-
 pub fn main() -> PyResult<()> {
     // get the relative path to the project folder
     let folder = Path::new(file!())
         .parent()
         .unwrap()
         .parent()
         .unwrap()
         .parent()
         .unwrap();
 
     // spawn a Python interpreter
     pyo3::prepare_freethreaded_python();
     Python::with_gil(|py| {
-        // insert the project folder in `sys.modules` so that 
+        // insert the project folder in `sys.modules` so that
         // the main module can be imported by Python
         let sys = py.import("sys").unwrap();
         sys.getattr("path")
             .unwrap()
             .downcast::<PyList>()
             .unwrap()
             .insert(0, folder)
@@ -44,14 +43,13 @@
             .set_item("pyskani._skani", module)
             .unwrap();
 
         // run unittest on the tests
         let mut kwargs = PyDict::new(py);
         kwargs.set_item("exit", false).unwrap();
         kwargs.set_item("verbosity", 2u8).unwrap();
-        py.import("unittest").unwrap().call_method(
-            "TestProgram",
-            ("pyskani.tests",),
-            Some(kwargs),
-        ).map(|_| ())
+        py.import("unittest")
+            .unwrap()
+            .call_method("TestProgram", ("pyskani.tests",), Some(kwargs))
+            .map(|_| ())
     })
 }
```

### Comparing `pyskani-0.1.0/pyskani.egg-info/PKG-INFO` & `pyskani-0.1.1/pyskani.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyskani
-Version: 0.1.0
+Version: 0.1.1
 Summary: PyO3 bindings and Python interface to skani, a method for fast fast genomic identity calculation using sparse chaining.
 Home-page: https://github.com/althonos/pyskani
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/pyskani/issues
 Project-URL: Changelog, https://github.com/althonos/pyskani/blob/master/CHANGELOG.md
```

### Comparing `pyskani-0.1.0/pyskani.egg-info/SOURCES.txt` & `pyskani-0.1.1/pyskani.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/setup.cfg` & `pyskani-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyskani-0.1.0/setup.py` & `pyskani-0.1.1/setup.py`

 * *Files identical despite different names*

