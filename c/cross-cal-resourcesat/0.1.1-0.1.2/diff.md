# Comparing `tmp/cross_cal_resourcesat-0.1.1.tar.gz` & `tmp/cross_cal_resourcesat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cross_cal_resourcesat-0.1.1.tar", last modified: Tue Apr 11 17:24:09 2023, max compression
+gzip compressed data, was "cross_cal_resourcesat-0.1.2.tar", last modified: Tue Apr 11 18:52:08 2023, max compression
```

## Comparing `cross_cal_resourcesat-0.1.1.tar` & `cross_cal_resourcesat-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat/cross_cal_resourcesat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 17:24:09.000000 cross_cal_resourcesat-0.1.1/cross_cal_resourcesat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 17:24:09.045430 cross_cal_resourcesat-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-11 17:23:59.000000 cross_cal_resourcesat-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:52:08.055851 cross_cal_resourcesat-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-11 18:52:08.055851 cross_cal_resourcesat-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:52:08.051851 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat/cross_cal_resourcesat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:52:08.055851 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 18:52:08.000000 cross_cal_resourcesat-0.1.2/cross_cal_resourcesat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 18:52:08.055851 cross_cal_resourcesat-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-11 18:51:59.000000 cross_cal_resourcesat-0.1.2/setup.py
```

### Comparing `cross_cal_resourcesat-0.1.1/LICENSE` & `cross_cal_resourcesat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cross_cal_resourcesat-0.1.1/cross_cal_resourcesat/cross_cal_resourcesat.py` & `cross_cal_resourcesat-0.1.2/cross_cal_resourcesat/cross_cal_resourcesat.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -279,8 +279,8 @@
     os.makedirs(opf)
 
     do_ref(inpf_liss, opf)
     
     op_liss, op_ref = do_multiband(opf, inpf_ref, reference_sensor)
     sbaf, cal_liss, ref_liss, ref_band = calc_calibration(op_liss, op_ref)
     
-    return None
+    return None
```

### Comparing `cross_cal_resourcesat-0.1.1/setup.py` & `cross_cal_resourcesat-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='cross_cal_resourcesat',
     name='cross_cal_resourcesat',
     packages=find_packages(include=['cross_cal_resourcesat', 'cross_cal_resourcesat.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/akhi9661/cross_cal_resourcesat',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

