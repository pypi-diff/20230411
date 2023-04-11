# Comparing `tmp/goes2go-2023.4.1.tar.gz` & `tmp/goes2go-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goes2go-2023.4.1.tar", last modified: Mon Apr 10 19:04:41 2023, max compression
+gzip compressed data, was "goes2go-2023.4.2.tar", last modified: Tue Apr 11 15:29:45 2023, max compression
```

## Comparing `goes2go-2023.4.1.tar` & `goes2go-2023.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 19:04:41.000000 goes2go-2023.4.1/
--rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-03-07 22:50:31.000000 goes2go-2023.4.1/.gitattributes
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     2027 2023-02-02 16:15:19.000000 goes2go-2023.4.1/.gitignore
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1079 2023-02-02 16:12:51.000000 goes2go-2023.4.1/.readthedocs.yml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      977 2023-04-10 16:44:33.000000 goes2go-2023.4.1/CITATION.cff
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1076 2022-03-07 22:50:31.000000 goes2go-2023.4.1/LICENSE
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      102 2022-10-20 19:50:16.000000 goes2go-2023.4.1/MANIFEST.in
--rw-------   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-10 19:04:41.000000 goes2go-2023.4.1/PKG-INFO
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     8722 2023-02-02 16:12:51.000000 goes2go-2023.4.1/README.md
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     2393 2022-11-15 17:49:05.000000 goes2go-2023.4.1/environment-dev.yml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      747 2022-11-15 17:45:56.000000 goes2go-2023.4.1/environment-test-conda.yml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1038 2022-10-20 20:22:08.000000 goes2go-2023.4.1/environment-test.yml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1352 2023-02-02 16:28:56.000000 goes2go-2023.4.1/environment.yml
-drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 19:04:41.000000 goes2go-2023.4.1/goes2go/
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     7797 2022-10-20 15:16:21.000000 goes2go-2023.4.1/goes2go/NEW.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     3105 2023-03-20 15:41:44.000000 goes2go-2023.4.1/goes2go/__init__.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      166 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go/_version.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)    41018 2023-04-10 18:53:52.000000 goes2go-2023.4.1/goes2go/accessors.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)    21281 2023-03-20 15:46:12.000000 goes2go-2023.4.1/goes2go/data.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     6710 2022-05-12 15:43:43.000000 goes2go-2023.4.1/goes2go/product_table.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)    35082 2023-04-10 18:44:07.000000 goes2go-2023.4.1/goes2go/rgb.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     6947 2023-04-10 18:59:52.000000 goes2go-2023.4.1/goes2go/tools.py
-drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 19:04:41.000000 goes2go-2023.4.1/goes2go.egg-info/
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go.egg-info/PKG-INFO
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      656 2023-04-10 19:04:41.000000 goes2go-2023.4.1/goes2go.egg-info/SOURCES.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go.egg-info/dependency_links.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2021-02-22 16:48:38.000000 goes2go-2023.4.1/goes2go.egg-info/not-zip-safe
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      237 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go.egg-info/requires.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)       14 2023-04-10 19:04:34.000000 goes2go-2023.4.1/goes2go.egg-info/top_level.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      277 2022-10-20 19:33:08.000000 goes2go-2023.4.1/pyproject.toml
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      107 2022-10-20 18:27:34.000000 goes2go-2023.4.1/requirements.txt
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     1541 2023-04-10 19:04:41.000000 goes2go-2023.4.1/setup.cfg
--rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-10-20 19:32:14.000000 goes2go-2023.4.1/setup.py
-drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 19:04:41.000000 goes2go-2023.4.1/tests/
--rw-r-----   0 blaylock (922916) 0381G056  (8708)        0 2022-10-20 15:16:21.000000 goes2go-2023.4.1/tests/__init__.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      532 2022-11-15 17:49:05.000000 goes2go-2023.4.1/tests/test_GOES.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      302 2022-03-21 20:48:21.000000 goes2go-2023.4.1/tests/test_abi.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)     2756 2023-03-20 15:41:44.000000 goes2go-2023.4.1/tests/test_data.py
--rw-r-----   0 blaylock (922916) 0381G056  (8708)      332 2022-03-21 20:48:21.000000 goes2go-2023.4.1/tests/test_glm.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-11 15:29:45.000000 goes2go-2023.4.2/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-03-07 22:50:31.000000 goes2go-2023.4.2/.gitattributes
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2027 2023-02-02 16:15:19.000000 goes2go-2023.4.2/.gitignore
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1079 2023-02-02 16:12:51.000000 goes2go-2023.4.2/.readthedocs.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      977 2023-04-10 16:44:33.000000 goes2go-2023.4.2/CITATION.cff
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1076 2022-03-07 22:50:31.000000 goes2go-2023.4.2/LICENSE
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      102 2022-10-20 19:50:16.000000 goes2go-2023.4.2/MANIFEST.in
+-rw-------   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-11 15:29:45.000000 goes2go-2023.4.2/PKG-INFO
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     8722 2023-02-02 16:12:51.000000 goes2go-2023.4.2/README.md
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2393 2022-11-15 17:49:05.000000 goes2go-2023.4.2/environment-dev.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      747 2022-11-15 17:45:56.000000 goes2go-2023.4.2/environment-test-conda.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1038 2022-10-20 20:22:08.000000 goes2go-2023.4.2/environment-test.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1352 2023-02-02 16:28:56.000000 goes2go-2023.4.2/environment.yml
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-11 15:29:45.000000 goes2go-2023.4.2/goes2go/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     8426 2023-04-11 15:23:23.000000 goes2go-2023.4.2/goes2go/NEW.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     3105 2023-03-20 15:41:44.000000 goes2go-2023.4.2/goes2go/__init__.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      166 2023-04-11 15:29:40.000000 goes2go-2023.4.2/goes2go/_version.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    41018 2023-04-10 18:53:52.000000 goes2go-2023.4.2/goes2go/accessors.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    21281 2023-03-20 15:46:12.000000 goes2go-2023.4.2/goes2go/data.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     6710 2022-05-12 15:43:43.000000 goes2go-2023.4.2/goes2go/product_table.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    35082 2023-04-10 18:44:07.000000 goes2go-2023.4.2/goes2go/rgb.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     6947 2023-04-10 18:59:52.000000 goes2go-2023.4.2/goes2go/tools.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-11 15:29:45.000000 goes2go-2023.4.2/goes2go.egg-info/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-11 15:29:40.000000 goes2go-2023.4.2/goes2go.egg-info/PKG-INFO
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      656 2023-04-11 15:29:45.000000 goes2go-2023.4.2/goes2go.egg-info/SOURCES.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2023-04-11 15:29:40.000000 goes2go-2023.4.2/goes2go.egg-info/dependency_links.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2021-02-22 16:48:38.000000 goes2go-2023.4.2/goes2go.egg-info/not-zip-safe
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      237 2023-04-11 15:29:40.000000 goes2go-2023.4.2/goes2go.egg-info/requires.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       14 2023-04-11 15:29:40.000000 goes2go-2023.4.2/goes2go.egg-info/top_level.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      277 2022-10-20 19:33:08.000000 goes2go-2023.4.2/pyproject.toml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      107 2022-10-20 18:27:34.000000 goes2go-2023.4.2/requirements.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1541 2023-04-11 15:29:45.000000 goes2go-2023.4.2/setup.cfg
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-10-20 19:32:14.000000 goes2go-2023.4.2/setup.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-11 15:29:45.000000 goes2go-2023.4.2/tests/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        0 2022-10-20 15:16:21.000000 goes2go-2023.4.2/tests/__init__.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      532 2022-11-15 17:49:05.000000 goes2go-2023.4.2/tests/test_GOES.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      302 2022-03-21 20:48:21.000000 goes2go-2023.4.2/tests/test_abi.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2756 2023-03-20 15:41:44.000000 goes2go-2023.4.2/tests/test_data.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      332 2022-03-21 20:48:21.000000 goes2go-2023.4.2/tests/test_glm.py
```

### Comparing `goes2go-2023.4.1/.gitignore` & `goes2go-2023.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/.readthedocs.yml` & `goes2go-2023.4.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/CITATION.cff` & `goes2go-2023.4.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/LICENSE` & `goes2go-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/PKG-INFO` & `goes2go-2023.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goes2go
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Retrieve GOES-16/17 data from AWS. Also proves some RGB recipes.
 Home-page: https://github.com/blaylockbk/goes2go
 Author: Brian K. Blaylock
 Author-email: blaylockbk@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/blaylockbk/goes2go
 Project-URL: Documentation, https://goes2go.readthedocs.io/
```

### Comparing `goes2go-2023.4.1/README.md` & `goes2go-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/environment-dev.yml` & `goes2go-2023.4.2/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/environment-test-conda.yml` & `goes2go-2023.4.2/environment-test-conda.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/environment-test.yml` & `goes2go-2023.4.2/environment-test.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/environment.yml` & `goes2go-2023.4.2/environment.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/goes2go/NEW.py` & `goes2go-2023.4.2/goes2go/NEW.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 class GOES:
     def __init__(
         self,
         satellite=config["timerange"].get("satellite"),
         product=config["timerange"].get("product"),
         domain=config["timerange"].get("domain"),
         bands=None,
+        channel=None,
     ):
         """Initialize a GOES object for a desired satellite and product.
 
         Parameters
         ----------
         satellite : {16, 17, 18}
             The satellite number. May also use the following aliases
@@ -72,22 +73,35 @@
         domain : {None, 'F', 'C', "M", "M1", "M2"}
             Only needed for ABI products.
             - F = Full Disk
             - C = CONUS
             - M = Mesoscale sector (both)
             - M1 = Mesoscale sector 1
             - M2 = Mesoscale sector 2
-        band : None, int, or list
+        bands : None, int, or list
             Specify the ABI channels to retrieve. *Only used if the
             product requested has unique bands.*
+            For example, ``bands=2`` for channel 2 or ``bands=[1,2,3]``
+            for channels 1, 2 and 3.
+        channel : None, int, or list
+            Alias for "bands" argument. If channel is not None, then
+            "bands" is not use.
+
+            Note: I don't like the name of "bands", but the NetCDF file
+            uses the term "band" instead of "channel" in reference to
+            the ABI products, so I'll stick with "band" for now.
         """
         self.satellite = satellite
         self.product = product
         self.domain = domain
-        self.bands = bands
+
+        if channel is not None:
+            self.bands = channel
+        else:
+            self.bands = bands
 
         if self.product.startswith("ABI") and self.product in _product:
             # Sometimes the user might inavertantly give the domain
             # in the product name.
             self.domain = self.product[-1]
             self.product = self.product[:-1]
 
@@ -157,15 +171,19 @@
             f"╰───────────────────────────────╌┄┈",
         ]
         return "\n".join(msg)
 
     def latest(self, **kwargs):
         """Get the latest available GOES data."""
         return goes_latest(
-            satellite=self.satellite, product=self.product, domain=self.domain, **kwargs
+            satellite=self.satellite,
+            product=self.product,
+            domain=self.domain,
+            bands=self.bands,
+            **kwargs,
         )
 
     def nearesttime(
         self,
         attime,
         within=pd.to_timedelta(config["nearesttime"].get("within", "1H")),
         **kwargs,
```

### Comparing `goes2go-2023.4.1/goes2go/__init__.py` & `goes2go-2023.4.2/goes2go/__init__.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/goes2go/accessors.py` & `goes2go-2023.4.2/goes2go/accessors.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/goes2go/data.py` & `goes2go-2023.4.2/goes2go/data.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/goes2go/product_table.txt` & `goes2go-2023.4.2/goes2go/product_table.txt`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/goes2go/rgb.py` & `goes2go-2023.4.2/goes2go/rgb.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/goes2go/tools.py` & `goes2go-2023.4.2/goes2go/tools.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/goes2go.egg-info/PKG-INFO` & `goes2go-2023.4.2/goes2go.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goes2go
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Retrieve GOES-16/17 data from AWS. Also proves some RGB recipes.
 Home-page: https://github.com/blaylockbk/goes2go
 Author: Brian K. Blaylock
 Author-email: blaylockbk@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/blaylockbk/goes2go
 Project-URL: Documentation, https://goes2go.readthedocs.io/
```

### Comparing `goes2go-2023.4.1/goes2go.egg-info/SOURCES.txt` & `goes2go-2023.4.2/goes2go.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/setup.cfg` & `goes2go-2023.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/tests/test_GOES.py` & `goes2go-2023.4.2/tests/test_GOES.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.4.1/tests/test_data.py` & `goes2go-2023.4.2/tests/test_data.py`

 * *Files identical despite different names*

