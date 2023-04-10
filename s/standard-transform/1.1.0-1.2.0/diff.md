# Comparing `tmp/standard-transform-1.1.0.tar.gz` & `tmp/standard-transform-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard-transform-1.1.0.tar", last modified: Sat Feb 25 05:42:14 2023, max compression
+gzip compressed data, was "standard-transform-1.2.0.tar", last modified: Mon Apr 10 23:43:14 2023, max compression
```

## Comparing `standard-transform-1.1.0.tar` & `standard-transform-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-02-25 05:42:14.251331 standard-transform-1.1.0/
--rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:20:55.000000 standard-transform-1.1.0/LICENSE
--rw-r--r--   0 caseysm    (501) staff       (20)       24 2022-11-16 18:20:55.000000 standard-transform-1.1.0/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)     4464 2023-02-25 05:42:14.251144 standard-transform-1.1.0/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     4138 2023-02-16 06:33:59.000000 standard-transform-1.1.0/README.md
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-02-16 06:59:35.000000 standard-transform-1.1.0/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-02-25 05:42:14.251380 standard-transform-1.1.0/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1520 2022-11-16 18:20:55.000000 standard-transform-1.1.0/setup.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-02-25 05:42:14.249614 standard-transform-1.1.0/standard_transform/
--rw-r--r--   0 caseysm    (501) staff       (20)      143 2023-02-25 05:41:54.000000 standard-transform-1.1.0/standard_transform/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5490 2023-02-16 06:22:00.000000 standard-transform-1.1.0/standard_transform/base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2163 2023-02-16 06:48:04.000000 standard-transform-1.1.0/standard_transform/datasets.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1973 2023-02-25 05:35:09.000000 standard-transform-1.1.0/standard_transform/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-02-25 05:42:14.250521 standard-transform-1.1.0/standard_transform.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)     4464 2023-02-25 05:42:14.000000 standard-transform-1.1.0/standard_transform.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      400 2023-02-25 05:42:14.000000 standard-transform-1.1.0/standard_transform.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-02-25 05:42:14.000000 standard-transform-1.1.0/standard_transform.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-02-25 05:42:14.000000 standard-transform-1.1.0/standard_transform.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-02-25 05:42:14.000000 standard-transform-1.1.0/standard_transform.egg-info/top_level.txt
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-02-25 05:42:14.250676 standard-transform-1.1.0/test/
--rw-r--r--   0 caseysm    (501) staff       (20)     3762 2023-02-25 05:39:09.000000 standard-transform-1.1.0/test/test_tform.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.214937 standard-transform-1.2.0/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:20:55.000000 standard-transform-1.2.0/LICENSE
+-rw-r--r--   0 caseysm    (501) staff       (20)       63 2023-04-10 23:37:06.000000 standard-transform-1.2.0/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)     7737 2023-04-10 23:43:14.214778 standard-transform-1.2.0/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     7411 2023-04-10 23:37:06.000000 standard-transform-1.2.0/README.md
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-03-28 05:17:19.000000 standard-transform-1.2.0/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-10 23:43:14.214983 standard-transform-1.2.0/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1597 2023-04-10 23:43:10.000000 standard-transform-1.2.0/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.212911 standard-transform-1.2.0/standard_transform/
+-rw-r--r--   0 caseysm    (501) staff       (20)      270 2023-04-10 23:40:16.000000 standard-transform-1.2.0/standard_transform/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     7066 2023-04-10 23:37:06.000000 standard-transform-1.2.0/standard_transform/base.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.214117 standard-transform-1.2.0/standard_transform/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)     5384 2023-04-10 23:37:06.000000 standard-transform-1.2.0/standard_transform/data/v1dd_um_streamline.json
+-rw-r--r--   0 caseysm    (501) staff       (20)     4892 2023-04-10 23:37:06.000000 standard-transform-1.2.0/standard_transform/datasets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9256 2023-04-10 23:37:06.000000 standard-transform-1.2.0/standard_transform/streamlines.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1973 2023-02-25 05:35:09.000000 standard-transform-1.2.0/standard_transform/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.213966 standard-transform-1.2.0/standard_transform.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)     7737 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      506 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-10 23:43:14.000000 standard-transform-1.2.0/standard_transform.egg-info/top_level.txt
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-10 23:43:14.214435 standard-transform-1.2.0/test/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1394 2023-04-10 23:37:06.000000 standard-transform-1.2.0/test/test_streamline.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3762 2023-02-25 05:39:09.000000 standard-transform-1.2.0/test/test_tform.py
```

### Comparing `standard-transform-1.1.0/LICENSE` & `standard-transform-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `standard-transform-1.1.0/setup.py` & `standard-transform-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,11 +39,12 @@
     author="Casey Schneider-Mizell",
     author_email="caseys@alleninstitute.org",
     description="Define and repeat basic affine transformation tasks for datasets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=required,
     include_package_data=True,
+    package_data={"standard_transform": ['standard_transform/data/*.json']},
     dependency_links=dependency_links,
     url="https://github.com/ceesem/standard_transform",
     packages=["standard_transform"],
 )
```

### Comparing `standard-transform-1.1.0/standard_transform/utils.py` & `standard-transform-1.2.0/standard_transform/utils.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.1.0/test/test_tform.py` & `standard-transform-1.2.0/test/test_tform.py`

 * *Files identical despite different names*

