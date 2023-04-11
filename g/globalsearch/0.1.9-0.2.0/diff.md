# Comparing `tmp/globalsearch-0.1.9.tar.gz` & `tmp/globalsearch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalsearch-0.1.9.tar", last modified: Fri Apr  7 20:19:25 2023, max compression
+gzip compressed data, was "globalsearch-0.2.0.tar", last modified: Tue Apr 11 15:49:44 2023, max compression
```

## Comparing `globalsearch-0.1.9.tar` & `globalsearch-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.220249 globalsearch-0.1.9/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-07 20:19:25.220319 globalsearch-0.1.9/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.1.9/README.md
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.215184 globalsearch-0.1.9/bin/
--rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.1.9/bin/gs_prepare
--rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.1.9/bin/gs_submit
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.214271 globalsearch-0.1.9/globalsearch/
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.216359 globalsearch-0.1.9/globalsearch/control/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.1.9/globalsearch/control/__init__.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.1.9/globalsearch/control/gs_prepare.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.219965 globalsearch-0.1.9/globalsearch/rnaseq/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.1.9/globalsearch/rnaseq/__init__.py
--rw-r--r--   0 weiju      (501) staff       (20)     7034 2023-03-21 18:06:55.000000 globalsearch-0.1.9/globalsearch/rnaseq/find_files.py
--rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.1.9/globalsearch/rnaseq/index_star.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.1.9/globalsearch/rnaseq/make_kallisto_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.1.9/globalsearch/rnaseq/make_star_idx_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6154 2023-04-07 20:18:38.000000 globalsearch-0.1.9/globalsearch/rnaseq/make_star_salmon_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     1634 2023-02-09 22:31:19.000000 globalsearch-0.1.9/globalsearch/rnaseq/post_star_salmon.py
--rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.1.9/globalsearch/rnaseq/run_kallisto.py
--rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.1.9/globalsearch/rnaseq/run_spladder.py
--rwxr-xr-x   0 weiju      (501) staff       (20)    12988 2023-04-07 20:18:38.000000 globalsearch-0.1.9/globalsearch/rnaseq/run_star_salmon.py
--rw-r--r--   0 weiju      (501) staff       (20)     3664 2023-03-21 18:06:55.000000 globalsearch-0.1.9/globalsearch/rnaseq/trim_galore.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.216136 globalsearch-0.1.9/globalsearch.egg-info/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/SOURCES.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/dependency_links.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.1.9/globalsearch.egg-info/not-zip-safe
--rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/requires.txt
--rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/top_level.txt
--rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-07 20:19:25.220536 globalsearch-0.1.9/setup.cfg
--rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-07 20:18:38.000000 globalsearch-0.1.9/setup.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.032609 globalsearch-0.2.0/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-11 15:49:44.032669 globalsearch-0.2.0/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.0/README.md
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.027840 globalsearch-0.2.0/bin/
+-rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.0/bin/gs_prepare
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.0/bin/gs_submit
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.027004 globalsearch-0.2.0/globalsearch/
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.029011 globalsearch-0.2.0/globalsearch/control/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.0/globalsearch/control/__init__.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.0/globalsearch/control/gs_prepare.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.032395 globalsearch-0.2.0/globalsearch/rnaseq/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.0/globalsearch/rnaseq/__init__.py
+-rw-r--r--   0 weiju      (501) staff       (20)     7034 2023-03-21 18:06:55.000000 globalsearch-0.2.0/globalsearch/rnaseq/find_files.py
+-rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.0/globalsearch/rnaseq/index_star.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.0/globalsearch/rnaseq/make_kallisto_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.0/globalsearch/rnaseq/make_star_idx_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6154 2023-04-07 20:18:38.000000 globalsearch-0.2.0/globalsearch/rnaseq/make_star_salmon_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1634 2023-02-09 22:31:19.000000 globalsearch-0.2.0/globalsearch/rnaseq/post_star_salmon.py
+-rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.0/globalsearch/rnaseq/run_kallisto.py
+-rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.2.0/globalsearch/rnaseq/run_spladder.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)    13266 2023-04-11 15:47:13.000000 globalsearch-0.2.0/globalsearch/rnaseq/run_star_salmon.py
+-rw-r--r--   0 weiju      (501) staff       (20)     3664 2023-03-21 18:06:55.000000 globalsearch-0.2.0/globalsearch/rnaseq/trim_galore.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.028762 globalsearch-0.2.0/globalsearch.egg-info/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.0/globalsearch.egg-info/not-zip-safe
+-rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/requires.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/top_level.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-11 15:49:44.032864 globalsearch-0.2.0/setup.cfg
+-rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-11 15:48:05.000000 globalsearch-0.2.0/setup.py
```

### Comparing `globalsearch-0.1.9/PKG-INFO` & `globalsearch-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.1.9
+Version: 0.2.0
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.1.9/bin/gs_prepare` & `globalsearch-0.2.0/bin/gs_prepare`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/bin/gs_submit` & `globalsearch-0.2.0/bin/gs_submit`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/control/gs_prepare.py` & `globalsearch-0.2.0/globalsearch/control/gs_prepare.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/find_files.py` & `globalsearch-0.2.0/globalsearch/rnaseq/find_files.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/index_star.py` & `globalsearch-0.2.0/globalsearch/rnaseq/index_star.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/make_kallisto_job.py` & `globalsearch-0.2.0/globalsearch/rnaseq/make_kallisto_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/make_star_idx_job.py` & `globalsearch-0.2.0/globalsearch/rnaseq/make_star_idx_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/make_star_salmon_job.py` & `globalsearch-0.2.0/globalsearch/rnaseq/make_star_salmon_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/post_star_salmon.py` & `globalsearch-0.2.0/globalsearch/rnaseq/post_star_salmon.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/run_kallisto.py` & `globalsearch-0.2.0/globalsearch/rnaseq/run_kallisto.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/run_spladder.py` & `globalsearch-0.2.0/globalsearch/rnaseq/run_spladder.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/run_star_salmon.py` & `globalsearch-0.2.0/globalsearch/rnaseq/run_star_salmon.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,19 @@
     print('\033[33mRunning salmon-quant! \033[0m', flush=True)
     # check if we are performing deduplication
     if args.dedup:
         salmon_input = '%sNoSingletonCollated.out.bam' % (outfile_prefix)
     else:
         salmon_input = '%sAligned.out.bam' % (outfile_prefix)
 
+        # Use BAM file aligned to transcriptome for salmon input if it exists
+        salmon_transcriptome_input = "%sAligned.toTranscriptome.out.bam" % outfile_prefix
+        if os.path.exists(salmon_transcriptome_input):
+            salmon_input = salmon_transcriptome_input
+
     command = ['salmon', 'quant', '-t', genome_fasta,
         '-l', 'A',  '-a',  salmon_input, '-o', '%s/%s_salmon_quant' % (results_dir, args.salmonPrefix)]
     cmd = ' '.join(command)
     print("Salmon quant command: '%s'" % cmd, flush=True)
     # run as a joined string
     compl_proc = subprocess.run(cmd, check=True, capture_output=False, cwd=results_dir, shell=True)
```

### Comparing `globalsearch-0.1.9/globalsearch/rnaseq/trim_galore.py` & `globalsearch-0.2.0/globalsearch/rnaseq/trim_galore.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/globalsearch.egg-info/PKG-INFO` & `globalsearch-0.2.0/globalsearch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.1.9
+Version: 0.2.0
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.1.9/globalsearch.egg-info/SOURCES.txt` & `globalsearch-0.2.0/globalsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.9/setup.py` & `globalsearch-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'globalsearch'
 PACKAGES = ['globalsearch.rnaseq', 'globalsearch.control']
 DESCRIPTION = 'globalsearch is a collection of Python modules and command tools for the Global Search pipeline.'
 LICENSE = 'LGPL V3'
 URI = 'https://github.com/baliga-lab/Global_Search'
 AUTHOR = 'Wei-ju Wu'
-VERSION = '0.1.9'
+VERSION = '0.2.0'
 
 KEYWORDS = ['global search', 'coral reef']
 
 # See trove classifiers
 # https://testpypi.python.org/pypi?%3Aaction=list_classifiers
 
 CLASSIFIERS = [
```

