# Comparing `tmp/kmergenetyper-1.0.6.tar.gz` & `tmp/kmergenetyper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmergenetyper-1.0.6.tar", last modified: Tue Apr 11 08:51:48 2023, max compression
+gzip compressed data, was "kmergenetyper-1.0.7.tar", last modified: Tue Apr 11 12:08:10 2023, max compression
```

## Comparing `kmergenetyper-1.0.6.tar` & `kmergenetyper-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 08:51:48.710136 kmergenetyper-1.0.6/
--rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.6/LICENSE
--rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-11 08:51:48.710023 kmergenetyper-1.0.6/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      195 2023-04-04 09:02:07.000000 kmergenetyper-1.0.6/README.md
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 08:51:48.708302 kmergenetyper-1.0.6/bin/
--rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.6/bin/kmergenetyper
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 08:51:48.709367 kmergenetyper-1.0.6/kmergenetyper/
--rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.6/kmergenetyper/__init__.py
--rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.6/kmergenetyper/kma.py
--rw-r--r--   0 malhal     (502) staff       (20)     3609 2023-04-11 08:50:40.000000 kmergenetyper-1.0.6/kmergenetyper/realignConsensus.py
--rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.6/kmergenetyper/typeGenes.py
--rw-r--r--   0 malhal     (502) staff       (20)       21 2023-04-11 08:51:21.000000 kmergenetyper-1.0.6/kmergenetyper/version.py
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 08:51:48.709849 kmergenetyper-1.0.6/kmergenetyper.egg-info/
--rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-11 08:51:48.000000 kmergenetyper-1.0.6/kmergenetyper.egg-info/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      325 2023-04-11 08:51:48.000000 kmergenetyper-1.0.6/kmergenetyper.egg-info/SOURCES.txt
--rw-r--r--   0 malhal     (502) staff       (20)        1 2023-04-11 08:51:48.000000 kmergenetyper-1.0.6/kmergenetyper.egg-info/dependency_links.txt
--rw-r--r--   0 malhal     (502) staff       (20)       14 2023-04-11 08:51:48.000000 kmergenetyper-1.0.6/kmergenetyper.egg-info/top_level.txt
--rw-r--r--   0 malhal     (502) staff       (20)       38 2023-04-11 08:51:48.710186 kmergenetyper-1.0.6/setup.cfg
--rw-r--r--   0 malhal     (502) staff       (20)      442 2023-04-11 08:51:21.000000 kmergenetyper-1.0.6/setup.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 12:08:10.554905 kmergenetyper-1.0.7/
+-rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.7/LICENSE
+-rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-11 12:08:10.554787 kmergenetyper-1.0.7/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      195 2023-04-04 09:02:07.000000 kmergenetyper-1.0.7/README.md
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 12:08:10.553209 kmergenetyper-1.0.7/bin/
+-rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.7/bin/kmergenetyper
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 12:08:10.554163 kmergenetyper-1.0.7/kmergenetyper/
+-rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.7/kmergenetyper/__init__.py
+-rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.7/kmergenetyper/kma.py
+-rw-r--r--   0 malhal     (502) staff       (20)     4010 2023-04-11 12:06:05.000000 kmergenetyper-1.0.7/kmergenetyper/realignConsensus.py
+-rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.7/kmergenetyper/typeGenes.py
+-rw-r--r--   0 malhal     (502) staff       (20)       21 2023-04-11 12:08:05.000000 kmergenetyper-1.0.7/kmergenetyper/version.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 12:08:10.554620 kmergenetyper-1.0.7/kmergenetyper.egg-info/
+-rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-11 12:08:10.000000 kmergenetyper-1.0.7/kmergenetyper.egg-info/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      325 2023-04-11 12:08:10.000000 kmergenetyper-1.0.7/kmergenetyper.egg-info/SOURCES.txt
+-rw-r--r--   0 malhal     (502) staff       (20)        1 2023-04-11 12:08:10.000000 kmergenetyper-1.0.7/kmergenetyper.egg-info/dependency_links.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       14 2023-04-11 12:08:10.000000 kmergenetyper-1.0.7/kmergenetyper.egg-info/top_level.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       38 2023-04-11 12:08:10.554957 kmergenetyper-1.0.7/setup.cfg
+-rw-r--r--   0 malhal     (502) staff       (20)      442 2023-04-11 12:08:05.000000 kmergenetyper-1.0.7/setup.py
```

### Comparing `kmergenetyper-1.0.6/LICENSE` & `kmergenetyper-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.6/bin/kmergenetyper` & `kmergenetyper-1.0.7/bin/kmergenetyper`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.6/kmergenetyper/kma.py` & `kmergenetyper-1.0.7/kmergenetyper/kma.py`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.6/kmergenetyper/realignConsensus.py` & `kmergenetyper-1.0.7/kmergenetyper/realignConsensus.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,20 +5,25 @@
     non_perfect_hits = []
     alignment_dict = {}
     headers = ''
     with open('{}/{}.res'.format(output, prefix), 'r') as f:
         for line in f:
             line = line.strip()
             if not line.startswith('#'):
-                if float(line.split('\t')[4].strip()) < 100.00:
-                    non_perfect_hits.append('>' + line.split('\t')[0].strip())
-                alignment_dict[line.split('\t')[0].strip()] = line.split()[1:]
+                line = line.split('\t')
+                for item in line:
+                    item = item.strip()
+                if float(line[4]) < 100.00:
+                    non_perfect_hits.append('>' + line[0].strip())
+                alignment_dict[line[0]] = line[1:]
             else:
                 headers = line
 
+    alignment_dict = reformat_dict(alignment_dict)
+
     with open('{}/{}.fsa'.format(output, prefix), 'r') as f:
         flag = False
         for line in f:
             line = line.rstrip()
             if line.startswith('>'):
                 header = line
                 if line in non_perfect_hits:
@@ -34,14 +39,22 @@
 
     eval_realignments(output, prefix, headers, alignment_dict, non_perfect_hits)
 
     if not keep:
         for item in non_perfect_hits:
             os.system('rm {}/{}*'.format(output, item[1:]))
         os.system('rm {}/old_*'.format(output, prefix))
+
+def reformat_dict(input_dict):
+    output_dict = {}
+    for item in input_dict:
+        output_dict[item.strip()] = []
+        for value in input_dict[item]:
+            output_dict[item.strip()].append(value.strip())
+    return output_dict
 def eval_realignments(output, prefix, headers, alignment_dict, non_perfect_hits):
     realignment_dict = {}
 
     for item in alignment_dict:
         if float(alignment_dict[item][3]) == 100.00:
             realignment_dict[item] = alignment_dict[item]
 
@@ -53,25 +66,25 @@
                 if not line.startswith('#'):
                     gene = line.split('\t')[0]
                     if gene not in realignment_dict:
                         realignment_dict[gene] = alignment_dict[original_gene]
                         t_id_1 = realignment_dict[gene][3]
                         t_id_2 = line.split('\t')[4]
                         if float(t_id_1) < float(t_id_2):
-                            realignment_dict[gene][3] = t_id_2  # Replace template identity
+                            realignment_dict[gene][3] = t_id_2 # Replace template identity
                             realignment_dict[gene][4] = line.split('\t')[5]  # Replace template coverage
                             realignment_dict[gene][5] = line.split('\t')[6]  # Replace template coverage
                     else:
                         t_id_1 = realignment_dict[gene][3]
                         t_id_2 = line.split('\t')[4]
                         if float(t_id_1) < float(t_id_2):
                             realignment_dict[gene][3] = t_id_2 #Replace template identity
                             realignment_dict[gene][4] = line.split('\t')[5] #Replace template coverage
                             realignment_dict[gene][5] = line.split('\t')[6]  # Replace template coverage
-
+    realignment_dict = reformat_dict(realignment_dict)
 
     keys = list(realignment_dict.keys())
     keys.sort()
 
     with open('{}/final_{}.res'.format(output, prefix), 'w') as f:
         print (headers, file=f)
         for item in keys:
```

### Comparing `kmergenetyper-1.0.6/kmergenetyper/typeGenes.py` & `kmergenetyper-1.0.7/kmergenetyper/typeGenes.py`

 * *Files identical despite different names*

