# Comparing `tmp/kmergenetyper-1.0.4.tar.gz` & `tmp/kmergenetyper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmergenetyper-1.0.4.tar", last modified: Wed Apr  5 08:41:19 2023, max compression
+gzip compressed data, was "kmergenetyper-1.0.5.tar", last modified: Tue Apr 11 07:54:22 2023, max compression
```

## Comparing `kmergenetyper-1.0.4.tar` & `kmergenetyper-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-05 08:41:19.485760 kmergenetyper-1.0.4/
--rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.4/LICENSE
--rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-05 08:41:19.485647 kmergenetyper-1.0.4/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      195 2023-04-04 09:02:07.000000 kmergenetyper-1.0.4/README.md
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-05 08:41:19.483861 kmergenetyper-1.0.4/bin/
--rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.4/bin/kmergenetyper
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-05 08:41:19.484928 kmergenetyper-1.0.4/kmergenetyper/
--rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.4/kmergenetyper/__init__.py
--rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.4/kmergenetyper/kma.py
--rw-r--r--   0 malhal     (502) staff       (20)     3579 2023-04-05 08:41:01.000000 kmergenetyper-1.0.4/kmergenetyper/realignConsensus.py
--rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.4/kmergenetyper/typeGenes.py
--rw-r--r--   0 malhal     (502) staff       (20)       21 2023-03-22 08:23:42.000000 kmergenetyper-1.0.4/kmergenetyper/version.py
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-05 08:41:19.485481 kmergenetyper-1.0.4/kmergenetyper.egg-info/
--rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-05 08:41:19.000000 kmergenetyper-1.0.4/kmergenetyper.egg-info/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      325 2023-04-05 08:41:19.000000 kmergenetyper-1.0.4/kmergenetyper.egg-info/SOURCES.txt
--rw-r--r--   0 malhal     (502) staff       (20)        1 2023-04-05 08:41:19.000000 kmergenetyper-1.0.4/kmergenetyper.egg-info/dependency_links.txt
--rw-r--r--   0 malhal     (502) staff       (20)       14 2023-04-05 08:41:19.000000 kmergenetyper-1.0.4/kmergenetyper.egg-info/top_level.txt
--rw-r--r--   0 malhal     (502) staff       (20)       38 2023-04-05 08:41:19.485808 kmergenetyper-1.0.4/setup.cfg
--rw-r--r--   0 malhal     (502) staff       (20)      442 2023-04-05 08:41:01.000000 kmergenetyper-1.0.4/setup.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 07:54:22.836493 kmergenetyper-1.0.5/
+-rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.5/LICENSE
+-rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-11 07:54:22.836392 kmergenetyper-1.0.5/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      195 2023-04-04 09:02:07.000000 kmergenetyper-1.0.5/README.md
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 07:54:22.834651 kmergenetyper-1.0.5/bin/
+-rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.5/bin/kmergenetyper
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 07:54:22.835760 kmergenetyper-1.0.5/kmergenetyper/
+-rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.5/kmergenetyper/__init__.py
+-rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.5/kmergenetyper/kma.py
+-rw-r--r--   0 malhal     (502) staff       (20)     3599 2023-04-11 07:53:32.000000 kmergenetyper-1.0.5/kmergenetyper/realignConsensus.py
+-rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.5/kmergenetyper/typeGenes.py
+-rw-r--r--   0 malhal     (502) staff       (20)       21 2023-04-11 07:53:49.000000 kmergenetyper-1.0.5/kmergenetyper/version.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 07:54:22.836265 kmergenetyper-1.0.5/kmergenetyper.egg-info/
+-rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-11 07:54:22.000000 kmergenetyper-1.0.5/kmergenetyper.egg-info/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      325 2023-04-11 07:54:22.000000 kmergenetyper-1.0.5/kmergenetyper.egg-info/SOURCES.txt
+-rw-r--r--   0 malhal     (502) staff       (20)        1 2023-04-11 07:54:22.000000 kmergenetyper-1.0.5/kmergenetyper.egg-info/dependency_links.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       14 2023-04-11 07:54:22.000000 kmergenetyper-1.0.5/kmergenetyper.egg-info/top_level.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       38 2023-04-11 07:54:22.836561 kmergenetyper-1.0.5/setup.cfg
+-rw-r--r--   0 malhal     (502) staff       (20)      442 2023-04-11 07:53:49.000000 kmergenetyper-1.0.5/setup.py
```

### Comparing `kmergenetyper-1.0.4/LICENSE` & `kmergenetyper-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.4/bin/kmergenetyper` & `kmergenetyper-1.0.5/bin/kmergenetyper`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.4/kmergenetyper/kma.py` & `kmergenetyper-1.0.5/kmergenetyper/kma.py`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.4/kmergenetyper/realignConsensus.py` & `kmergenetyper-1.0.5/kmergenetyper/realignConsensus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
+import sys
 
 def realign_consensus(output, prefix, database, keep):
     non_perfect_hits = []
     alignment_dict = {}
     headers = ''
     with open('{}/{}.res'.format(output, prefix), 'r') as f:
         for line in f:
             line = line.rstrip()
             if not line.startswith('#'):
                 if float(line.split('\t')[4]) < 100.00:
-                    non_perfect_hits.append('>' + line.split('\t')[0])
+                    non_perfect_hits.append('>' + line.split('\t')[0].rstrip())
                 alignment_dict[line.split('\t')[0]] = line.split('\t')[1:]
             else:
                 headers = line
 
     with open('{}/{}.fsa'.format(output, prefix), 'r') as f:
         flag = False
         for line in f:
```

### Comparing `kmergenetyper-1.0.4/kmergenetyper/typeGenes.py` & `kmergenetyper-1.0.5/kmergenetyper/typeGenes.py`

 * *Files identical despite different names*

