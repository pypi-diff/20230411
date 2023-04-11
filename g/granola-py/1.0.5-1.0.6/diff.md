# Comparing `tmp/granola_py-1.0.5.tar.gz` & `tmp/granola_py-1.0.6.tar.gz`

## Comparing `granola_py-1.0.5.tar` & `granola_py-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 granola_py-1.0.5/Cargo.toml
--rw-r--r--   0      501       20     6148 2023-04-07 17:31:37.000000 granola_py-1.0.5/.DS_Store
--rw-r--r--   0      501       20       24 2023-04-07 17:31:37.000000 granola_py-1.0.5/.gitignore
--rw-r--r--   0      501       20  1029970 2023-04-07 17:31:37.000000 granola_py-1.0.5/Granola_Logo.png
--rw-r--r--   0      501       20     1063 2023-04-07 17:31:37.000000 granola_py-1.0.5/LICENSE.md
--rw-r--r--   0      501       20     1061 2023-04-07 17:31:37.000000 granola_py-1.0.5/README.md
--rw-r--r--   0      501       20   132240 2023-04-07 17:31:37.000000 granola_py-1.0.5/code_snippet.png
--rw-r--r--   0      501       20      114 2023-04-07 17:31:37.000000 granola_py-1.0.5/examples/hello_world.py
--rw-r--r--   0      501       20      235 2023-04-07 17:31:37.000000 granola_py-1.0.5/main.py
--rw-r--r--   0      501       20      320 2023-04-07 17:31:37.000000 granola_py-1.0.5/pyproject.toml
--rw-r--r--   0      501       20     2122 2023-04-09 00:35:32.000000 granola_py-1.0.5/src/http.rs
--rw-r--r--   0      501       20     4617 2023-04-09 16:45:32.000000 granola_py-1.0.5/src/lib.rs
--rw-r--r--   0      501       20      942 2023-04-07 17:31:37.000000 granola_py-1.0.5/src/net/mod.rs
--rw-r--r--   0      501       20       26 2023-04-07 17:31:37.000000 granola_py-1.0.5/tests/__main__.py
--rw-r--r--   0      501       20      885 2023-04-07 17:31:37.000000 granola_py-1.0.5/user-guide.md
--rw-r--r--   0      501       20     8755 2023-04-09 16:52:08.000000 granola_py-1.0.5/Cargo.lock
--rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 granola_py-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 granola_py-1.0.6/Cargo.toml
+-rw-r--r--   0      501       20     6148 2023-04-07 17:31:37.000000 granola_py-1.0.6/.DS_Store
+-rw-r--r--   0      501       20       24 2023-04-07 17:31:37.000000 granola_py-1.0.6/.gitignore
+-rw-r--r--   0      501       20  1029970 2023-04-07 17:31:37.000000 granola_py-1.0.6/Granola_Logo.png
+-rw-r--r--   0      501       20     1063 2023-04-07 17:31:37.000000 granola_py-1.0.6/LICENSE.md
+-rw-r--r--   0      501       20     1061 2023-04-07 17:31:37.000000 granola_py-1.0.6/README.md
+-rw-r--r--   0      501       20   132240 2023-04-07 17:31:37.000000 granola_py-1.0.6/code_snippet.png
+-rw-r--r--   0      501       20      114 2023-04-07 17:31:37.000000 granola_py-1.0.6/examples/hello_world.py
+-rw-r--r--   0      501       20      235 2023-04-07 17:31:37.000000 granola_py-1.0.6/main.py
+-rw-r--r--   0      501       20      320 2023-04-07 17:31:37.000000 granola_py-1.0.6/pyproject.toml
+-rw-r--r--   0      501       20     2122 2023-04-09 00:35:32.000000 granola_py-1.0.6/src/http.rs
+-rw-r--r--   0      501       20     4917 2023-04-11 16:50:59.000000 granola_py-1.0.6/src/lib.rs
+-rw-r--r--   0      501       20      942 2023-04-07 17:31:37.000000 granola_py-1.0.6/src/net/mod.rs
+-rw-r--r--   0      501       20       26 2023-04-07 17:31:37.000000 granola_py-1.0.6/tests/__main__.py
+-rw-r--r--   0      501       20      885 2023-04-07 17:31:37.000000 granola_py-1.0.6/user-guide.md
+-rw-r--r--   0      501       20     8755 2023-04-11 16:51:37.000000 granola_py-1.0.6/Cargo.lock
+-rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 granola_py-1.0.6/PKG-INFO
```

### Comparing `granola_py-1.0.5/.DS_Store` & `granola_py-1.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.5/Granola_Logo.png` & `granola_py-1.0.6/Granola_Logo.png`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.5/LICENSE.md` & `granola_py-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.5/README.md` & `granola_py-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.5/code_snippet.png` & `granola_py-1.0.6/code_snippet.png`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.5/src/http.rs` & `granola_py-1.0.6/src/http.rs`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.5/src/lib.rs` & `granola_py-1.0.6/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-use pyo3::prelude::*; use std::{
-    io::{ErrorKind},
+use pyo3::prelude::*; 
+use std::{
+    io::{Error, ErrorKind},
     sync::{
         atomic::{AtomicBool, Ordering},
         Arc,
     },
     time::Duration,
     thread::sleep
 }; 
@@ -57,21 +58,26 @@
     }
 }
 
 fn process_response(call: String, request: Request, app: &PyAny) -> (RouteResult<&PyAny>, Request) {
     (
         match app.call_method1(call.as_str(), request.clone()) {
             Ok (e) => RouteResult::SubRoute(e),
-            Err(_) => {
-                match app.call_method0(call.as_str()) {
-                    Ok (e) => RouteResult::SubRoute(e),
-                    Err(e) => {
-                        println!("{}", e);
-                        RouteResult::Failed
+            Err(e) => {
+                println!("{}", e);
+                if Error::from(e).to_string() == format!("TypeError: {}.{} missing 1 required argument", app.get_type().name().unwrap(), call) { 
+                    match app.call_method0(call.as_str()) {
+                        Ok (e) => RouteResult::SubRoute(e),
+                        Err(e) => {
+                            println!("{}", e);
+                            RouteResult::Failed
+                        }
                     }
+                } else {
+                    RouteResult::Failed
                 }
             }
         },
         request
     )
 }
```

### Comparing `granola_py-1.0.5/src/net/mod.rs` & `granola_py-1.0.6/src/net/mod.rs`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.5/user-guide.md` & `granola_py-1.0.6/user-guide.md`

 * *Files identical despite different names*

### Comparing `granola_py-1.0.5/Cargo.lock` & `granola_py-1.0.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 dependencies = [
  "nix",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "granola"
-version = "1.0.5"
+version = "1.0.6"
 dependencies = [
  "ctrlc",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
```

### Comparing `granola_py-1.0.5/PKG-INFO` & `granola_py-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granola-py
-Version: 1.0.5
+Version: 1.0.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

