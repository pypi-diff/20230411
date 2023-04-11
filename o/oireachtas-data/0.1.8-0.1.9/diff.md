# Comparing `tmp/oireachtas-data-0.1.8.tar.gz` & `tmp/oireachtas-data-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oireachtas-data-0.1.8.tar", last modified: Sun Jul 17 12:37:54 2022, max compression
+gzip compressed data, was "oireachtas-data-0.1.9.tar", last modified: Mon Jul 18 16:07:40 2022, max compression
```

## Comparing `oireachtas-data-0.1.8.tar` & `oireachtas-data-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 12:37:54.913762 oireachtas-data-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-17 12:37:54.913762 oireachtas-data-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-17 12:37:54.913762 oireachtas-data-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 12:37:54.909762 oireachtas-data-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 12:37:54.913762 oireachtas-data-0.1.8/src/oireachtas_data/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 12:37:54.913762 oireachtas-data-0.1.8/src/oireachtas_data/bin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/bin/load_debates.py
--rw-r--r--   0 runner    (1001) docker     (121)     3548 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/bin/pull_debates.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/bin/pull_members.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 12:37:54.913762 oireachtas-data-0.1.8/src/oireachtas_data/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/debate.py
--rw-r--r--   0 runner    (1001) docker     (121)     6367 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/debate_section.py
--rw-r--r--   0 runner    (1001) docker     (121)    10465 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/member.py
--rw-r--r--   0 runner    (1001) docker     (121)    11483 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/new_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/old_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/para.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/models/speech.py
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/src/oireachtas_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 12:37:54.913762 oireachtas-data-0.1.8/src/oireachtas_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-17 12:37:54.000000 oireachtas-data-0.1.8/src/oireachtas_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-07-17 12:37:54.000000 oireachtas-data-0.1.8/src/oireachtas_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-17 12:37:54.000000 oireachtas-data-0.1.8/src/oireachtas_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-07-17 12:37:54.000000 oireachtas-data-0.1.8/src/oireachtas_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-07-17 12:37:54.000000 oireachtas-data-0.1.8/src/oireachtas_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-17 12:37:54.000000 oireachtas-data-0.1.8/src/oireachtas_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 12:37:54.913762 oireachtas-data-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-07-17 12:36:58.000000 oireachtas-data-0.1.8/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/src/oireachtas_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/src/oireachtas_data/bin/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/bin/load_debates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3548 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/bin/pull_debates.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/bin/pull_members.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/src/oireachtas_data/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/debate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6367 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/debate_section.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10508 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11483 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/new_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/old_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/para.py
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/models/speech.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/src/oireachtas_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/src/oireachtas_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-18 16:07:39.000000 oireachtas-data-0.1.9/src/oireachtas_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-07-18 16:07:40.000000 oireachtas-data-0.1.9/src/oireachtas_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 16:07:39.000000 oireachtas-data-0.1.9/src/oireachtas_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-07-18 16:07:40.000000 oireachtas-data-0.1.9/src/oireachtas_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-07-18 16:07:40.000000 oireachtas-data-0.1.9/src/oireachtas_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-18 16:07:40.000000 oireachtas-data-0.1.9/src/oireachtas_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 16:07:40.464725 oireachtas-data-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2022-07-18 16:06:28.000000 oireachtas-data-0.1.9/test/test_utils.py
```

### Comparing `oireachtas-data-0.1.8/LICENSE` & `oireachtas-data-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/README.md` & `oireachtas-data-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/setup.py` & `oireachtas-data-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'transformers',
     'unidecode',
     'edlib'
 )
 
 setup(
     name='oireachtas-data',
-    version='0.1.8',
+    version='0.1.9',
     python_requires='>=3.6',
     description='Oireachtas debate data',
     long_description='Oireachtas debate data',
     author='Robert Lucey',
     url='https://github.com/RobertLucey/oireachtas-data',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/bin/pull_debates.py` & `oireachtas-data-0.1.9/src/oireachtas_data/bin/pull_debates.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/bin/pull_members.py` & `oireachtas-data-0.1.9/src/oireachtas_data/bin/pull_members.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/models/debate.py` & `oireachtas-data-0.1.9/src/oireachtas_data/models/debate.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/models/debate_section.py` & `oireachtas-data-0.1.9/src/oireachtas_data/models/debate_section.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/models/member.py` & `oireachtas-data-0.1.9/src/oireachtas_data/models/member.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,17 @@
 
         # Some issues with michael collins since there are two
         # FIXME: Any near duplicate names should be noted.
         # if there's a number at the end we need to be very careful
 
         name = self.clean_name(name)
 
+        if name == '':
+            return
+
         for member in self.data:
             if member.pid is None:
                 continue
             if member.pid == name:
                 self.found_member_pids.add(member.pid)
                 return member
             if member.pid == f'{name}FF':
```

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/models/new_pdf.py` & `oireachtas-data-0.1.9/src/oireachtas_data/models/new_pdf.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/models/old_pdf.py` & `oireachtas-data-0.1.9/src/oireachtas_data/models/old_pdf.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/models/para.py` & `oireachtas-data-0.1.9/src/oireachtas_data/models/para.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/models/pdf.py` & `oireachtas-data-0.1.9/src/oireachtas_data/models/pdf.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/models/speech.py` & `oireachtas-data-0.1.9/src/oireachtas_data/models/speech.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data/utils.py` & `oireachtas-data-0.1.9/src/oireachtas_data/utils.py`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/src/oireachtas_data.egg-info/SOURCES.txt` & `oireachtas-data-0.1.9/src/oireachtas_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oireachtas-data-0.1.8/test/test_utils.py` & `oireachtas-data-0.1.9/test/test_utils.py`

 * *Files identical despite different names*

