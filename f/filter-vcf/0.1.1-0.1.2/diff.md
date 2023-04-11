# Comparing `tmp/filter-vcf-0.1.1.tar.gz` & `tmp/filter-vcf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter-vcf-0.1.1.tar", last modified: Tue Nov 29 20:12:00 2022, max compression
+gzip compressed data, was "filter-vcf-0.1.2.tar", last modified: Tue Apr 11 12:39:57 2023, max compression
```

## Comparing `filter-vcf-0.1.1.tar` & `filter-vcf-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,24 @@
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-11-29 20:11:33.861663 filter-vcf-0.1.1/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-11-29 20:11:33.865663 filter-vcf-0.1.1/filter_vcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-11-29 20:11:33.865663 filter-vcf-0.1.1/filter_vcf/filter_vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2022-11-29 20:11:33.865663 filter-vcf-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    63873 2022-11-29 20:11:33.865663 filter-vcf-0.1.1/tests/sample.nrm.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-11-29 20:11:33.865663 filter-vcf-0.1.1/tests/test_filter_vcf.py
--rw-------   0 runner    (1001) docker     (123)      239 2022-11-29 20:12:00.950070 filter-vcf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/PYPI.md
+-rw-r--r--   0        0        0        0 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/__init__.py
+-rw-r--r--   0        0        0     1217 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/process.py
+-rw-r--r--   0        0        0        0 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/util/__init__.py
+-rw-r--r--   0        0        0     1791 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/util/addDepth.py
+-rw-r--r--   0        0        0     2015 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/util/cleanAD.py
+-rw-r--r--   0        0        0     4179 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/util/cleanGT.py
+-rw-r--r--   0        0        0     1753 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/convertChrName.py
+-rw-r--r--   0        0        0      631 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/detectVcf.py
+-rw-r--r--   0        0        0     1744 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/passFilter.py
+-rw-r--r--   0        0        0      814 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/readVcf.py
+-rw-r--r--   0        0        0      720 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/removeNonRef.py
+-rw-r--r--   0        0        0      685 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/sortVcf.py
+-rw-r--r--   0        0        0      781 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/unique.py
+-rw-r--r--   0        0        0      899 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3490 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/tests/decomp.vcf
+-rw-r--r--   0        0        0   270284 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/tests/full.vcf
+-rw-r--r--   0        0        0     1682 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/tests/presorted.vcf
+-rw-r--r--   0        0        0    62601 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/sample.nrm.vcf.gz
+-rw-r--r--   0        0        0    38219 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/test_process.py
+-rw-r--r--   0        0        0     1682 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/unsorted.vcf
+-rw-r--r--   0        0        0      514 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/unsorted.vcf.gz
+-rw-r--r--   0        0        0       40 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/vcf.txt
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 filter-vcf-0.1.2/PKG-INFO
```

### Comparing `filter-vcf-0.1.1/filter_vcf/filter_vcf.py` & `filter-vcf-0.1.2/filter_vcf/process.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import vcfpy
 import logging
 from pathlib import Path
+from filter_vcf.util.readVcf import read_vcf
+from filter_vcf.util.sortVcf import sort_vcf
+from filter_vcf.util.addDepth import add_depth
 
 
-def filter_vcf(vcf_in: str, filters: str):
+def process_vcf(vcf_in: str, filters: str):
     allowed_filters = filters.split(":")
     vcf_out = vcf_in.replace("nrm.vcf.gz", "nrm.filtered.vcf.gz")
     print(f"saving file {vcf_out}")
 
     logging.info("Filtering VCF using filters: {}".format(allowed_filters))
     reader = vcfpy.Reader.from_path(vcf_in)
     writer = vcfpy.Writer.from_path(vcf_out, reader.header)
```

### Comparing `filter-vcf-0.1.1/pyproject.toml` & `filter-vcf-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "filter-vcf"
-version = "0.1.1"
+version = "0.1.2"
 description = "LifeOmic VCF filtering"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging==0.3.2",
     "vcfpy>=0.13.4",
     "pysam==0.19.1",
+    "pytest>=7.1.2",
+    "fuc>=0.36.0",
+    "setuptools>=67.6.1",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.9,<3.11"
 readme = "PYPI.md"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
```

