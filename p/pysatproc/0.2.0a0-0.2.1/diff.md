# Comparing `tmp/pysatproc-0.2.0a0.tar.gz` & `tmp/pysatproc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysatproc-0.2.0a0.tar", max compression
+gzip compressed data, was "pysatproc-0.2.1.tar", max compression
```

## Comparing `pysatproc-0.2.0a0.tar` & `pysatproc-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0    11357 2021-11-14 23:49:22.590082 pysatproc-0.2.0a0/LICENSE.txt
--rw-r--r--   0        0        0     1557 2022-08-16 16:02:34.743915 pysatproc-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0      366 2022-06-03 12:49:37.210682 pysatproc-0.2.0a0/satproc/__init__.py
--rw-r--r--   0        0        0    10445 2022-07-12 12:48:59.183174 pysatproc-0.2.0a0/satproc/chips.py
--rw-r--r--   0        0        0     9453 2022-07-12 12:48:59.183174 pysatproc-0.2.0a0/satproc/console/extract_chips.py
--rw-r--r--   0        0        0     2896 2022-06-03 12:49:37.214682 pysatproc-0.2.0a0/satproc/console/filter.py
--rw-r--r--   0        0        0     3674 2022-06-03 12:49:37.214682 pysatproc-0.2.0a0/satproc/console/generalize.py
--rw-r--r--   0        0        0     3595 2022-07-12 12:48:59.183174 pysatproc-0.2.0a0/satproc/console/make_masks.py
--rw-r--r--   0        0        0     2442 2022-06-03 12:49:37.214682 pysatproc-0.2.0a0/satproc/console/match_histograms.py
--rw-r--r--   0        0        0     3448 2022-06-03 12:49:37.214682 pysatproc-0.2.0a0/satproc/console/polygonize.py
--rw-r--r--   0        0        0     2661 2022-06-03 12:49:37.214682 pysatproc-0.2.0a0/satproc/console/scale.py
--rw-r--r--   0        0        0     2301 2022-06-03 16:49:44.143185 pysatproc-0.2.0a0/satproc/console/smooth_stitch.py
--rw-r--r--   0        0        0     3490 2022-06-03 16:49:44.143185 pysatproc-0.2.0a0/satproc/console/spatial_filter.py
--rw-r--r--   0        0        0      923 2022-06-03 12:49:37.214682 pysatproc-0.2.0a0/satproc/filter.py
--rw-r--r--   0        0        0     2641 2022-06-03 12:49:37.218682 pysatproc-0.2.0a0/satproc/histogram.py
--rw-r--r--   0        0        0     8480 2022-07-12 12:48:59.187174 pysatproc-0.2.0a0/satproc/masks.py
--rw-r--r--   0        0        0     3470 2022-06-03 12:49:37.218682 pysatproc-0.2.0a0/satproc/postprocess/generalize.py
--rwxr-xr-x   0        0        0     6401 2022-06-03 12:49:37.218682 pysatproc-0.2.0a0/satproc/postprocess/polygonize.py
--rw-r--r--   0        0        0     7258 2022-06-03 16:49:44.143185 pysatproc-0.2.0a0/satproc/postprocess/smooth.py
--rw-r--r--   0        0        0     1483 2022-06-03 16:49:44.143185 pysatproc-0.2.0a0/satproc/postprocess/spatial_filter.py
--rw-r--r--   0        0        0     3244 2022-06-03 12:49:37.218682 pysatproc-0.2.0a0/satproc/scale.py
--rw-r--r--   0        0        0     9173 2022-06-03 16:49:44.143185 pysatproc-0.2.0a0/satproc/utils.py
--rw-r--r--   0        0        0     1807 2022-08-16 16:16:51.638270 pysatproc-0.2.0a0/setup.py
--rw-r--r--   0        0        0      940 2022-08-16 16:16:51.638726 pysatproc-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-03 18:35:28.571169 pysatproc-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     1550 2023-04-11 14:48:42.349115 pysatproc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-03-03 18:35:28.572716 pysatproc-0.2.1/satproc/__init__.py
+-rw-r--r--   0        0        0    10445 2023-04-11 14:43:47.691013 pysatproc-0.2.1/satproc/chips.py
+-rw-r--r--   0        0        0     9453 2023-04-11 14:43:47.691129 pysatproc-0.2.1/satproc/console/extract_chips.py
+-rw-r--r--   0        0        0     2896 2023-03-03 18:35:28.573015 pysatproc-0.2.1/satproc/console/filter.py
+-rw-r--r--   0        0        0     3674 2023-03-03 18:35:28.573084 pysatproc-0.2.1/satproc/console/generalize.py
+-rw-r--r--   0        0        0     3595 2023-04-11 14:43:47.691374 pysatproc-0.2.1/satproc/console/make_masks.py
+-rw-r--r--   0        0        0     2442 2023-03-03 18:35:28.573190 pysatproc-0.2.1/satproc/console/match_histograms.py
+-rw-r--r--   0        0        0     3448 2023-03-03 18:35:28.573240 pysatproc-0.2.1/satproc/console/polygonize.py
+-rw-r--r--   0        0        0     2661 2023-03-03 18:35:28.573289 pysatproc-0.2.1/satproc/console/scale.py
+-rw-r--r--   0        0        0     2301 2023-03-03 18:35:28.573372 pysatproc-0.2.1/satproc/console/smooth_stitch.py
+-rw-r--r--   0        0        0     3490 2023-03-03 18:35:28.573445 pysatproc-0.2.1/satproc/console/spatial_filter.py
+-rw-r--r--   0        0        0      923 2023-03-03 18:35:28.573504 pysatproc-0.2.1/satproc/filter.py
+-rw-r--r--   0        0        0     2641 2023-03-03 18:35:28.573561 pysatproc-0.2.1/satproc/histogram.py
+-rw-r--r--   0        0        0     8480 2023-04-11 14:43:47.691474 pysatproc-0.2.1/satproc/masks.py
+-rw-r--r--   0        0        0     4334 2023-03-03 18:35:28.573735 pysatproc-0.2.1/satproc/postprocess/generalize.py
+-rwxr-xr-x   0        0        0     6401 2023-03-03 18:35:28.573806 pysatproc-0.2.1/satproc/postprocess/polygonize.py
+-rw-r--r--   0        0        0     7258 2023-03-03 18:35:28.573882 pysatproc-0.2.1/satproc/postprocess/smooth.py
+-rw-r--r--   0        0        0     1483 2023-03-03 18:35:28.573937 pysatproc-0.2.1/satproc/postprocess/spatial_filter.py
+-rw-r--r--   0        0        0     3244 2023-03-03 18:35:28.574010 pysatproc-0.2.1/satproc/scale.py
+-rw-r--r--   0        0        0     9173 2023-03-03 18:35:28.574089 pysatproc-0.2.1/satproc/utils.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 pysatproc-0.2.1/PKG-INFO
```

### Comparing `pysatproc-0.2.0a0/LICENSE.txt` & `pysatproc-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/pyproject.toml` & `pysatproc-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pysatproc"
-version = "0.2.0-alpha.0"
+version = "0.2.1"
 description = "Python library and CLI tools for processing geospatial imagery for ML"
 authors = ["Damián Silvani <munshkr@gmail.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "satproc"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 Fiona = "^1.8.21"
 numpy = "^1.22.2"
 opencv-python = "^4.5.5"
 pyproj = "^3.3.0"
-rasterio = "1.3b1"
+rasterio = "^1.3.6"
 Rtree = "^0.9.7"
 scikit-image = "^0.19.2"
 scipy = "^1.8.0"
 Shapely = "^1.8.1"
 tqdm = "^4.62.3"
 packaging = "^21.3"
```

### Comparing `pysatproc-0.2.0a0/satproc/chips.py` & `pysatproc-0.2.1/satproc/chips.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/extract_chips.py` & `pysatproc-0.2.1/satproc/console/extract_chips.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/filter.py` & `pysatproc-0.2.1/satproc/console/filter.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/generalize.py` & `pysatproc-0.2.1/satproc/console/generalize.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/make_masks.py` & `pysatproc-0.2.1/satproc/console/make_masks.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/match_histograms.py` & `pysatproc-0.2.1/satproc/console/match_histograms.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/polygonize.py` & `pysatproc-0.2.1/satproc/console/polygonize.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/scale.py` & `pysatproc-0.2.1/satproc/console/scale.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/smooth_stitch.py` & `pysatproc-0.2.1/satproc/console/smooth_stitch.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/console/spatial_filter.py` & `pysatproc-0.2.1/satproc/console/spatial_filter.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/filter.py` & `pysatproc-0.2.1/satproc/filter.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/histogram.py` & `pysatproc-0.2.1/satproc/histogram.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/masks.py` & `pysatproc-0.2.1/satproc/masks.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/postprocess/generalize.py` & `pysatproc-0.2.1/satproc/postprocess/generalize.py`

 * *Files 25% similar despite different names*

```diff
@@ -56,23 +56,40 @@
                             "coordinate system for accurate results."
                         ),
                         input_file,
                         proj_crs.to_string(),
                     )
 
                 dst_meta = src.meta.copy()
+                dst_meta["schema"]["geometry"] = "Polygon"
                 if target_crs:
                     del dst_meta["crs"]
                     dst_meta["crs_wkt"] = fiona_crs_from_proj_crs(target_crs)
 
                 with fiona.open(output_file, "w", **dst_meta) as dst:
                     for feat in tqdm(
                         src, ascii=True, desc=os.path.basename(input_file)
                     ):
+                        if not feat["geometry"]:
+                            _logger.warn(
+                                "Skipped feature %s with empty geometry", feat["id"]
+                            )
+                            continue
                         shp = shape(feat["geometry"])
+                        if shp.is_empty:
+                            _logger.warn(
+                                "Skipped feature %s with empty geometry", feat["id"]
+                            )
+                            continue
+                        if shp.type == "MultiPolygon" and len(shp.geoms) > 1:
+                            _logger.warn(
+                                "Skipped feature %s with a multi-part geometry (MultiPolygon)",
+                                feat["id"],
+                            )
+                            continue
                         if target_crs:
                             shp = reproject_shape(shp, proj_crs, target_crs)
                         if simplify == "douglas":
                             shp = shp.simplify(
                                 tolerance=douglas_tolerance, preserve_topology=True
                             )
                         if smooth == "chaikin":
```

### Comparing `pysatproc-0.2.0a0/satproc/postprocess/polygonize.py` & `pysatproc-0.2.1/satproc/postprocess/polygonize.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/postprocess/smooth.py` & `pysatproc-0.2.1/satproc/postprocess/smooth.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/postprocess/spatial_filter.py` & `pysatproc-0.2.1/satproc/postprocess/spatial_filter.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/scale.py` & `pysatproc-0.2.1/satproc/scale.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/satproc/utils.py` & `pysatproc-0.2.1/satproc/utils.py`

 * *Files identical despite different names*

### Comparing `pysatproc-0.2.0a0/PKG-INFO` & `pysatproc-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pysatproc
-Version: 0.2.0a0
+Version: 0.2.1
 Summary: Python library and CLI tools for processing geospatial imagery for ML
 License: Apache-2.0
 Author: Damián Silvani
 Author-email: munshkr@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Fiona (>=1.8.21,<2.0.0)
 Requires-Dist: Rtree (>=0.9.7,<0.10.0)
 Requires-Dist: Shapely (>=1.8.1,<2.0.0)
 Requires-Dist: numpy (>=1.22.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.5.5,<5.0.0)
 Requires-Dist: packaging (>=21.3,<22.0)
 Requires-Dist: pyproj (>=3.3.0,<4.0.0)
-Requires-Dist: rasterio (==1.3b1)
+Requires-Dist: rasterio (>=1.3.6,<2.0.0)
 Requires-Dist: scikit-image (>=0.19.2,<0.20.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
```

