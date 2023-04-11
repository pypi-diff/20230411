# Comparing `tmp/vbjax-0.0.9rc2.tar.gz` & `tmp/vbjax-0.0.9rc3.tar.gz`

## Comparing `vbjax-0.0.9rc2.tar` & `vbjax-0.0.9rc3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/_version.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/connectome.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/coupling.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/diagnostics.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/embed.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/layers.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/loops.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/neural_mass.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/regmap.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/shtlc.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/__main__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_connectome.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_coupling.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_embed.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_field_inference.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_jaxisms.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_layers.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_loops.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_regmap.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_shtlc.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/vbjax/tests/test_sparse.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/.gitignore
--rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/LICENSE
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/README.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/pyproject.toml
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 vbjax-0.0.9rc2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/_version.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/connectome.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/coupling.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/diagnostics.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/embed.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/layers.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/loops.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/neural_mass.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/regmap.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/shtlc.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/__main__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_connectome.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_coupling.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_embed.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_field_inference.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_jaxisms.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_layers.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_loops.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_regmap.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_shtlc.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/vbjax/tests/test_sparse.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/.gitignore
+-rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/LICENSE
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/pyproject.toml
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 vbjax-0.0.9rc3/PKG-INFO
```

### Comparing `vbjax-0.0.9rc2/vbjax/connectome.py` & `vbjax-0.0.9rc3/vbjax/connectome.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/coupling.py` & `vbjax-0.0.9rc3/vbjax/coupling.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/diagnostics.py` & `vbjax-0.0.9rc3/vbjax/diagnostics.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/embed.py` & `vbjax-0.0.9rc3/vbjax/embed.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/layers.py` & `vbjax-0.0.9rc3/vbjax/layers.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/loops.py` & `vbjax-0.0.9rc3/vbjax/loops.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/neural_mass.py` & `vbjax-0.0.9rc3/vbjax/neural_mass.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/regmap.py` & `vbjax-0.0.9rc3/vbjax/regmap.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/shtlc.py` & `vbjax-0.0.9rc3/vbjax/shtlc.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/sparse.py` & `vbjax-0.0.9rc3/vbjax/sparse.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/tests/test_connectome.py` & `vbjax-0.0.9rc3/vbjax/tests/test_connectome.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/tests/test_coupling.py` & `vbjax-0.0.9rc3/vbjax/tests/test_coupling.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/tests/test_field_inference.py` & `vbjax-0.0.9rc3/vbjax/tests/test_field_inference.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/tests/test_jaxisms.py` & `vbjax-0.0.9rc3/vbjax/tests/test_jaxisms.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/tests/test_loops.py` & `vbjax-0.0.9rc3/vbjax/tests/test_loops.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/vbjax/tests/test_sparse.py` & `vbjax-0.0.9rc3/vbjax/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/LICENSE` & `vbjax-0.0.9rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `vbjax-0.0.9rc2/pyproject.toml` & `vbjax-0.0.9rc3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,16 @@
   "pytest-xdist",
   "pytest-benchmark",
   "twine",
   "build",
   "tqdm",
   "jupyter",
   "matplotlib",
+  "joblib",
+  "grip",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ins-amu/vbjax"
 "Bug Tracker" = "https://github.com/ins-amu/vbjax/issues"
 
 [tool.hatch.build]
```

