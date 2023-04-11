# Comparing `tmp/adviz-0.0.8.tar.gz` & `tmp/adviz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adviz-0.0.8.tar", last modified: Mon Apr 10 19:21:08 2023, max compression
+gzip compressed data, was "adviz-0.0.9.tar", last modified: Mon Apr 10 19:54:55 2023, max compression
```

## Comparing `adviz-0.0.8.tar` & `adviz-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:21:08.534019 adviz-0.0.8/
--rw-rw-r--   0 me         (501) staff       (20)    11337 2023-01-20 02:50:04.000000 adviz-0.0.8/LICENSE
--rw-rw-r--   0 me         (501) staff       (20)      111 2023-01-20 02:50:04.000000 adviz-0.0.8/MANIFEST.in
--rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 19:21:08.533073 adviz-0.0.8/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)  3584472 2023-04-03 19:59:35.000000 adviz-0.0.8/README.md
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:21:08.515397 adviz-0.0.8/adviz/
--rw-r--r--   0 me         (501) staff       (20)      111 2023-04-10 19:17:02.000000 adviz-0.0.8/adviz/__init__.py
--rw-r--r--   0 me         (501) staff       (20)      738 2023-04-10 19:17:02.000000 adviz-0.0.8/adviz/_modidx.py
--rw-r--r--   0 me         (501) staff       (20)      142 2023-03-20 19:27:57.000000 adviz-0.0.8/adviz/core.py
--rw-r--r--   0 me         (501) staff       (20)     2478 2023-04-10 19:17:02.000000 adviz-0.0.8/adviz/status_codes.py
--rw-r--r--   0 me         (501) staff       (20)     3921 2023-04-10 19:17:02.000000 adviz-0.0.8/adviz/value_counts_plus.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:21:08.521638 adviz-0.0.8/adviz.egg-info/
--rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)      353 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/SOURCES.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/dependency_links.txt
--rw-r--r--   0 me         (501) staff       (20)       32 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/entry_points.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2023-03-19 21:23:32.000000 adviz-0.0.8/adviz.egg-info/not-zip-safe
--rw-r--r--   0 me         (501) staff       (20)       50 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/requires.txt
--rw-r--r--   0 me         (501) staff       (20)        6 2023-04-10 19:21:08.000000 adviz-0.0.8/adviz.egg-info/top_level.txt
--rw-r--r--   0 me         (501) staff       (20)      832 2023-04-10 19:17:02.000000 adviz-0.0.8/settings.ini
--rw-r--r--   0 me         (501) staff       (20)       38 2023-04-10 19:21:08.534142 adviz-0.0.8/setup.cfg
--rw-rw-r--   0 me         (501) staff       (20)     2560 2023-01-20 02:50:04.000000 adviz-0.0.8/setup.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:54:55.280104 adviz-0.0.9/
+-rw-rw-r--   0 me         (501) staff       (20)    11337 2023-01-20 02:50:04.000000 adviz-0.0.9/LICENSE
+-rw-rw-r--   0 me         (501) staff       (20)      111 2023-01-20 02:50:04.000000 adviz-0.0.9/MANIFEST.in
+-rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 19:54:55.279139 adviz-0.0.9/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)  3584472 2023-04-03 19:59:35.000000 adviz-0.0.9/README.md
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:54:55.262947 adviz-0.0.9/adviz/
+-rw-r--r--   0 me         (501) staff       (20)      111 2023-04-10 19:52:09.000000 adviz-0.0.9/adviz/__init__.py
+-rw-r--r--   0 me         (501) staff       (20)      738 2023-04-10 19:52:10.000000 adviz-0.0.9/adviz/_modidx.py
+-rw-r--r--   0 me         (501) staff       (20)      142 2023-03-20 19:27:57.000000 adviz-0.0.9/adviz/core.py
+-rw-r--r--   0 me         (501) staff       (20)     2478 2023-04-10 19:52:09.000000 adviz-0.0.9/adviz/status_codes.py
+-rw-r--r--   0 me         (501) staff       (20)     3917 2023-04-10 19:52:09.000000 adviz-0.0.9/adviz/value_counts_plus.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2023-04-10 19:54:55.269455 adviz-0.0.9/adviz.egg-info/
+-rw-r--r--   0 me         (501) staff       (20)  3585235 2023-04-10 19:54:55.000000 adviz-0.0.9/adviz.egg-info/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)      353 2023-04-10 19:54:55.000000 adviz-0.0.9/adviz.egg-info/SOURCES.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2023-04-10 19:54:55.000000 adviz-0.0.9/adviz.egg-info/dependency_links.txt
+-rw-r--r--   0 me         (501) staff       (20)       32 2023-04-10 19:54:55.000000 adviz-0.0.9/adviz.egg-info/entry_points.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2023-03-19 21:23:32.000000 adviz-0.0.9/adviz.egg-info/not-zip-safe
+-rw-r--r--   0 me         (501) staff       (20)       50 2023-04-10 19:54:55.000000 adviz-0.0.9/adviz.egg-info/requires.txt
+-rw-r--r--   0 me         (501) staff       (20)        6 2023-04-10 19:54:55.000000 adviz-0.0.9/adviz.egg-info/top_level.txt
+-rw-r--r--   0 me         (501) staff       (20)      832 2023-04-10 19:49:18.000000 adviz-0.0.9/settings.ini
+-rw-r--r--   0 me         (501) staff       (20)       38 2023-04-10 19:54:55.280246 adviz-0.0.9/setup.cfg
+-rw-rw-r--   0 me         (501) staff       (20)     2560 2023-01-20 02:50:04.000000 adviz-0.0.9/setup.py
```

### Comparing `adviz-0.0.8/LICENSE` & `adviz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adviz-0.0.8/PKG-INFO` & `adviz-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adviz
-Version: 0.0.8
+Version: 0.0.9
 Summary: advertools visualizations
 Home-page: https://github.com/eliasdabbas/adviz
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adviz-0.0.8/README.md` & `adviz-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `adviz-0.0.8/adviz/_modidx.py` & `adviz-0.0.9/adviz/_modidx.py`

 * *Files identical despite different names*

### Comparing `adviz-0.0.8/adviz/status_codes.py` & `adviz-0.0.9/adviz/status_codes.py`

 * *Files identical despite different names*

### Comparing `adviz-0.0.8/adviz/value_counts_plus.py` & `adviz-0.0.9/adviz/value_counts_plus.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,17 @@
     if not style:
         return count_df
     count_df.index = range(1, len(count_df)+1)
     count_df.columns = [name, 'count', 'cum. count', '%', 'cum. %']
     return (count_df
             .style
             .format({'count': '{:,}', 'cumsum': '{:,}', 
-                     'perc': '{:.1%}',
-                     'cum_count': '{:,}',
-                     'cum_perc': '{:.1%}'},
+                     '%': '{:.1%}',
+                     'cum. count': '{:,}',
+                     'cum. %': '{:.1%}'},
                     thousands=thousands,
                     decimal=decimal)
             .background_gradient(background_gradient)
             .highlight_null()
             .set_caption(f'<h2>Counts of <b>{name}</b></h2>')
             .set_table_attributes(f'style=font-size:{size}pt;'))
```

### Comparing `adviz-0.0.8/adviz.egg-info/PKG-INFO` & `adviz-0.0.9/adviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adviz
-Version: 0.0.8
+Version: 0.0.9
 Summary: advertools visualizations
 Home-page: https://github.com/eliasdabbas/adviz
 Author: Elias Dabbas
 Author-email: eliasdabbas@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adviz-0.0.8/settings.ini` & `adviz-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = adviz
 lib_name = adviz
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = adviz
 nbs_path = nbs
 recursive = True
```

### Comparing `adviz-0.0.8/setup.py` & `adviz-0.0.9/setup.py`

 * *Files identical despite different names*

