# Comparing `tmp/cross_cal_resourcesat-0.1.0.tar.gz` & `tmp/cross_cal_resourcesat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cross_cal_resourcesat-0.1.0.tar", last modified: Mon Apr 10 21:11:06 2023, max compression
+gzip compressed data, was "cross_cal_resourcesat-0.1.1.tar", last modified: Tue Apr 11 17:24:09 2023, max compression
```

## Comparing `cross_cal_resourcesat-0.1.0.tar` & `cross_cal_resourcesat-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:11:06.670409 cross_cal_resourcesat-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-10 21:11:06.670409 cross_cal_resourcesat-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:11:06.666409 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat/cross_cal_resourcesat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:11:06.670409 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 21:11:06.000000 cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-10 21:11:06.670409 cross_cal_resourcesat-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-10 21:10:55.000000 cross_cal_resourcesat-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat/cross_cal_resourcesat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/setup.py
```

### Comparing `cross_cal_resourcesat-0.1.0/LICENSE` & `cross_cal_resourcesat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cross_cal_resourcesat-0.1.0/PKG-INFO` & `cross_cal_resourcesat-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cross_cal_resourcesat
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.
 Home-page: https://github.com/akhi9661/cross_cal_resourcesat
 Author: Akhilesh Kumar
 Author-email: akhiraj9661@gmail.com
 License: MIT license
 Keywords: cross_cal_resourcesat
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -29,27 +29,25 @@
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![image](https://github.com/opengeos/leafmap/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
 
 ---
 
 ## Introduction
 
-This code module applies a simple cross calibration on LISS III and AWiFS to calibrate them with the help
-of a reference image like Landsat 8 and Sentinel 2.
+This package applies a cross calibrates LISS III and AWiFS with the help of a reference image like Landsat 8 and Sentinel 2.
 
 Takes two inputs:
 - `inpf_liss` = path to folder LISS III or AWiFS bands
-- `inpf_ref` = path to folder containing reference image bands
+- `inpf_ref` = path to folder containing reference image bands. Could be `Landsat 8` or `Sentinel 2`.
 
 Final output folder: 
 - `inpf_liss\Reflectance\Calibration`
 
 Four temporary images are also generated which are automatically deleted after the execution. These are two composite images,
 one resampled image, and one clipped image
-Note: Please make sure that both input and reference image have the same projection system. If not, please reproject the input.
 
 ---
 
 
 ## Package information
 A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.
 
@@ -57,13 +55,12 @@
 -   Github repo: https://github.com/akhi9661/cross_cal_resourcesat
 -   PypI: https://pypi.org/project/cross-cal-resourcesat/
 -   Free software: MIT license
 -   Documentation: https://akhi9661.github.io/cross_cal_resourcesat
 
 
 Note: At the moment, if `reference_sensor  = 'Landsat 8'`, path to reflectance images will have to provided in `inpf_ref`. 
-      The reprojection too is bit sketchy at the moment (defaults to `EPSG: 32643`). Will be fixed shortly.
 
 ---
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `cross_cal_resourcesat-0.1.0/README.md` & `cross_cal_resourcesat-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,27 +7,25 @@
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![image](https://github.com/opengeos/leafmap/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
 
 ---
 
 ## Introduction
 
-This code module applies a simple cross calibration on LISS III and AWiFS to calibrate them with the help
-of a reference image like Landsat 8 and Sentinel 2.
+This package applies a cross calibrates LISS III and AWiFS with the help of a reference image like Landsat 8 and Sentinel 2.
 
 Takes two inputs:
 - `inpf_liss` = path to folder LISS III or AWiFS bands
-- `inpf_ref` = path to folder containing reference image bands
+- `inpf_ref` = path to folder containing reference image bands. Could be `Landsat 8` or `Sentinel 2`.
 
 Final output folder: 
 - `inpf_liss\Reflectance\Calibration`
 
 Four temporary images are also generated which are automatically deleted after the execution. These are two composite images,
 one resampled image, and one clipped image
-Note: Please make sure that both input and reference image have the same projection system. If not, please reproject the input.
 
 ---
 
 
 ## Package information
 A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.
 
@@ -35,13 +33,12 @@
 -   Github repo: https://github.com/akhi9661/cross_cal_resourcesat
 -   PypI: https://pypi.org/project/cross-cal-resourcesat/
 -   Free software: MIT license
 -   Documentation: https://akhi9661.github.io/cross_cal_resourcesat
 
 
 Note: At the moment, if `reference_sensor  = 'Landsat 8'`, path to reflectance images will have to provided in `inpf_ref`. 
-      The reprojection too is bit sketchy at the moment (defaults to `EPSG: 32643`). Will be fixed shortly.
 
 ---
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `cross_cal_resourcesat-0.1.0/cross_cal_resourcesat/cross_cal_resourcesat.py` & `cross_cal_resourcesat-0.1.1/cross_cal_resourcesat/cross_cal_resourcesat.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,22 +183,23 @@
     Returns:
             opf_resample (str): path to the resampled LISS III image
     """
     
     print('Resampling: LISS III to reference image')
     
     reference = gdal.Open(file_ref, 0)
+    projection = reference.GetProjectionRef()
     referenceTrans = reference.GetGeoTransform()
     x_res = referenceTrans[1]
     y_res = -referenceTrans[5]
 
     opf_resample = os.path.join(os.path.dirname(file_liss), os.path.basename(file_liss).split('.')[0] + '_resample.TIF')
 
     kwargs = {"format": "GTiff", "xRes": x_res, "yRes": y_res}
-    ds = gdal.Warp(opf_resample, file_liss, dstSRS = 'EPSG:32643', **kwargs)
+    ds = gdal.Warp(opf_resample, file_liss, dstSRS = projection, **kwargs)
     ds = None
     
     return opf_resample
     
 
 def calc_calibration(file_liss, file_ref):
```

### Comparing `cross_cal_resourcesat-0.1.0/cross_cal_resourcesat.egg-info/PKG-INFO` & `cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cross-cal-resourcesat
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.
 Home-page: https://github.com/akhi9661/cross_cal_resourcesat
 Author: Akhilesh Kumar
 Author-email: akhiraj9661@gmail.com
 License: MIT license
 Keywords: cross_cal_resourcesat
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -29,27 +29,25 @@
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![image](https://github.com/opengeos/leafmap/workflows/docs/badge.svg)](https://github.com/akhi9661/cross_cal_resourcesat)
 
 ---
 
 ## Introduction
 
-This code module applies a simple cross calibration on LISS III and AWiFS to calibrate them with the help
-of a reference image like Landsat 8 and Sentinel 2.
+This package applies a cross calibrates LISS III and AWiFS with the help of a reference image like Landsat 8 and Sentinel 2.
 
 Takes two inputs:
 - `inpf_liss` = path to folder LISS III or AWiFS bands
-- `inpf_ref` = path to folder containing reference image bands
+- `inpf_ref` = path to folder containing reference image bands. Could be `Landsat 8` or `Sentinel 2`.
 
 Final output folder: 
 - `inpf_liss\Reflectance\Calibration`
 
 Four temporary images are also generated which are automatically deleted after the execution. These are two composite images,
 one resampled image, and one clipped image
-Note: Please make sure that both input and reference image have the same projection system. If not, please reproject the input.
 
 ---
 
 
 ## Package information
 A python package to cross calibrate ResourceSat 2 sensors like LISS III, AWiFS or LISS IV.
 
@@ -57,13 +55,12 @@
 -   Github repo: https://github.com/akhi9661/cross_cal_resourcesat
 -   PypI: https://pypi.org/project/cross-cal-resourcesat/
 -   Free software: MIT license
 -   Documentation: https://akhi9661.github.io/cross_cal_resourcesat
 
 
 Note: At the moment, if `reference_sensor  = 'Landsat 8'`, path to reflectance images will have to provided in `inpf_ref`. 
-      The reprojection too is bit sketchy at the moment (defaults to `EPSG: 32643`). Will be fixed shortly.
 
 ---
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `cross_cal_resourcesat-0.1.0/setup.py` & `cross_cal_resourcesat-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='cross_cal_resourcesat',
     name='cross_cal_resourcesat',
     packages=find_packages(include=['cross_cal_resourcesat', 'cross_cal_resourcesat.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/akhi9661/cross_cal_resourcesat',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

