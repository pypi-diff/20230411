# Comparing `tmp/coso-1.0.0.tar.gz` & `tmp/coso-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coso-1.0.0.tar", last modified: Tue Apr 11 09:32:58 2023, max compression
+gzip compressed data, was "coso-1.0.1.tar", last modified: Tue Apr 11 09:35:16 2023, max compression
```

## Comparing `coso-1.0.0.tar` & `coso-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:32:58.569233 coso-1.0.0/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.0.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-11 09:32:58.568148 coso-1.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.0.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:32:58.532222 coso-1.0.0/coso.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-11 09:32:58.000000 coso-1.0.0/coso.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      446 2023-04-11 09:32:58.000000 coso-1.0.0/coso.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-11 09:32:58.000000 coso-1.0.0/coso.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-11 09:32:58.000000 coso-1.0.0/coso.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        4 2023-04-11 09:32:58.000000 coso-1.0.0/coso.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.0.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-11 09:32:58.569801 coso-1.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      956 2023-04-11 09:32:30.000000 coso-1.0.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:32:58.565878 coso-1.0.0/src/
--rwxrwxrwx   0 root         (0) root         (0)    20083 2023-02-03 09:38:17.000000 coso-1.0.0/src/VisCoSo.py
--rwxrwxrwx   0 root         (0) root         (0)     3477 2023-02-03 09:38:26.000000 coso-1.0.0/src/VisCoSo_widget.py
--rwxrwxrwx   0 root         (0) root         (0)      163 2023-02-06 14:36:36.000000 coso-1.0.0/src/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11429 2023-02-03 09:39:45.000000 coso-1.0.0/src/cola_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.0.0/src/configuration.py
--rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.0.0/src/count.py
--rwxrwxrwx   0 root         (0) root         (0)    15928 2023-02-03 09:36:18.000000 coso-1.0.0/src/gen_plots.py
--rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.0.0/src/level_1.py
--rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.0.0/src/level_2.py
--rwxrwxrwx   0 root         (0) root         (0)     8708 2023-02-03 09:36:51.000000 coso-1.0.0/src/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     9606 2023-02-02 16:57:05.000000 coso-1.0.0/src/parsetab.py
--rwxrwxrwx   0 root         (0) root         (0)     9515 2023-02-03 09:37:05.000000 coso-1.0.0/src/problem.py
--rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.0.0/src/sharpCSP.py
--rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.0.0/src/solver.py
--rwxrwxrwx   0 root         (0) root         (0)    43623 2023-02-03 09:37:43.000000 coso-1.0.0/src/tester.py
--rwxrwxrwx   0 root         (0) root         (0)    14266 2023-01-13 13:24:30.000000 coso-1.0.0/src/util.py
--rwxrwxrwx   0 root         (0) root         (0)     9131 2023-02-03 09:38:05.000000 coso-1.0.0/src/venn.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:35:16.878400 coso-1.0.1/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.0.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-11 09:35:16.877026 coso-1.0.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.0.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:35:16.828971 coso-1.0.1/coso.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      446 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        4 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.0.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-11 09:35:16.878944 coso-1.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      956 2023-04-11 09:34:52.000000 coso-1.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:35:16.874585 coso-1.0.1/src/
+-rwxrwxrwx   0 root         (0) root         (0)    20083 2023-02-03 09:38:17.000000 coso-1.0.1/src/VisCoSo.py
+-rwxrwxrwx   0 root         (0) root         (0)     3477 2023-02-03 09:38:26.000000 coso-1.0.1/src/VisCoSo_widget.py
+-rwxrwxrwx   0 root         (0) root         (0)      163 2023-02-06 14:36:36.000000 coso-1.0.1/src/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11429 2023-02-03 09:39:45.000000 coso-1.0.1/src/cola_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.0.1/src/configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.0.1/src/count.py
+-rwxrwxrwx   0 root         (0) root         (0)    15928 2023-02-03 09:36:18.000000 coso-1.0.1/src/gen_plots.py
+-rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.0.1/src/level_1.py
+-rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.0.1/src/level_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8708 2023-02-03 09:36:51.000000 coso-1.0.1/src/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     9606 2023-02-02 16:57:05.000000 coso-1.0.1/src/parsetab.py
+-rwxrwxrwx   0 root         (0) root         (0)     9515 2023-02-03 09:37:05.000000 coso-1.0.1/src/problem.py
+-rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.0.1/src/sharpCSP.py
+-rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.0.1/src/solver.py
+-rwxrwxrwx   0 root         (0) root         (0)    43623 2023-02-03 09:37:43.000000 coso-1.0.1/src/tester.py
+-rwxrwxrwx   0 root         (0) root         (0)    14266 2023-01-13 13:24:30.000000 coso-1.0.1/src/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     9131 2023-02-03 09:38:05.000000 coso-1.0.1/src/venn.py
```

### Comparing `coso-1.0.0/LICENSE` & `coso-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/PKG-INFO` & `coso-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.0.0
+Version: 1.0.1
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.0.0/README.md` & `coso-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/coso.egg-info/PKG-INFO` & `coso-1.0.1/coso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.0.0
+Version: 1.0.1
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.0.0/setup.py` & `coso-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='coso',
-    version='1.0.0',    
+    version='1.0.1',    
     url='https://github.com/PietroTotis/CoSo',
     author='Pietro Totis',
     author_email='pietro.totis@kuleuven.be',
     license='GNU General Public License (GPL)',
     packages=['src'],
     install_requires=["portion",
                       "clingo==5.5.1",
```

### Comparing `coso-1.0.0/src/VisCoSo.py` & `coso-1.0.1/src/VisCoSo.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/VisCoSo_widget.py` & `coso-1.0.1/src/VisCoSo_widget.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/cola_parser.py` & `coso-1.0.1/src/cola_parser.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/configuration.py` & `coso-1.0.1/src/configuration.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/count.py` & `coso-1.0.1/src/count.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/gen_plots.py` & `coso-1.0.1/src/gen_plots.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/level_1.py` & `coso-1.0.1/src/level_1.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/level_2.py` & `coso-1.0.1/src/level_2.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/logger.py` & `coso-1.0.1/src/logger.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/parsetab.py` & `coso-1.0.1/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/problem.py` & `coso-1.0.1/src/problem.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/sharpCSP.py` & `coso-1.0.1/src/sharpCSP.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/solver.py` & `coso-1.0.1/src/solver.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/tester.py` & `coso-1.0.1/src/tester.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/util.py` & `coso-1.0.1/src/util.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.0/src/venn.py` & `coso-1.0.1/src/venn.py`

 * *Files identical despite different names*

