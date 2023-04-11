# Comparing `tmp/gwas_sumstats_tools-1.0.0a2.tar.gz` & `tmp/gwas_sumstats_tools-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwas_sumstats_tools-1.0.0a2.tar", max compression
+gzip compressed data, was "gwas_sumstats_tools-1.0.0a3.tar", max compression
```

## Comparing `gwas_sumstats_tools-1.0.0a2.tar` & `gwas_sumstats_tools-1.0.0a3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-02-10 17:38:30.835988 gwas_sumstats_tools-1.0.0a2/LICENSE
--rw-r--r--   0        0        0     4610 2023-03-09 10:23:17.020053 gwas_sumstats_tools-1.0.0a2/README.md
--rw-r--r--   0        0        0    10971 2023-03-14 16:18:20.060683 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/cli.py
--rw-r--r--   0        0        0     1387 2023-03-14 16:01:27.150283 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/config.py
--rw-r--r--   0        0        0     5671 2023-03-14 16:01:27.150847 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/format.py
--rw-r--r--   0        0        0     8560 2023-03-14 16:01:27.151771 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/interfaces/data_table.py
--rw-r--r--   0        0        0     7260 2023-03-14 16:01:27.152429 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/interfaces/metadata.py
--rw-r--r--   0        0        0     3913 2023-03-09 09:56:43.902434 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/read.py
--rw-r--r--   0        0        0     5754 2023-03-14 16:01:27.154602 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/schema/data_table.py
--rw-r--r--   0        0        0     1785 2023-03-09 09:56:43.903952 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/schema/metadata.py
--rw-r--r--   0        0        0     4603 2023-03-14 16:08:45.228413 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/utils.py
--rw-r--r--   0        0        0     7452 2023-03-14 16:01:27.155876 gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/validate.py
--rw-r--r--   0        0        0      679 2023-03-20 10:53:36.643146 gwas_sumstats_tools-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     5674 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.0a2/setup.py
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/LICENSE
+-rw-r--r--   0        0        0     4610 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/README.md
+-rw-r--r--   0        0        0    10971 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/cli.py
+-rw-r--r--   0        0        0     1387 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/config.py
+-rw-r--r--   0        0        0     5671 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/format.py
+-rw-r--r--   0        0        0     8560 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/interfaces/data_table.py
+-rw-r--r--   0        0        0     7260 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/interfaces/metadata.py
+-rw-r--r--   0        0        0     3913 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/read.py
+-rw-r--r--   0        0        0     5754 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/schema/data_table.py
+-rw-r--r--   0        0        0     1785 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/schema/metadata.py
+-rw-r--r--   0        0        0     4603 2023-03-20 10:58:07.449067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/utils.py
+-rw-r--r--   0        0        0     7452 2023-03-20 10:58:07.449067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/validate.py
+-rw-r--r--   0        0        0      679 2023-03-20 11:15:13.339784 gwas_sumstats_tools-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.0a3/PKG-INFO
```

### Comparing `gwas_sumstats_tools-1.0.0a2/LICENSE` & `gwas_sumstats_tools-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/README.md` & `gwas_sumstats_tools-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/cli.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/cli.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/config.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/config.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/format.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/format.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/interfaces/data_table.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/interfaces/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/interfaces/metadata.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/interfaces/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/read.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/read.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/schema/data_table.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/schema/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/schema/metadata.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/utils.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/utils.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/gwas_sumstats_tools/validate.py` & `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/validate.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a2/pyproject.toml` & `gwas_sumstats_tools-1.0.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwas-sumstats-tools"
-version = "1.0.0a2"
+version = "1.0.0a3"
 description = ""
 authors = ["jdhayhurst <jhayhurst@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "gwas_sumstats_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gwas_sumstats_tools-1.0.0a2/PKG-INFO` & `gwas_sumstats_tools-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwas-sumstats-tools
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: 
 Author: jdhayhurst
 Author-email: jhayhurst@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

