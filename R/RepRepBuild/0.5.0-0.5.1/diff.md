# Comparing `tmp/RepRepBuild-0.5.0.tar.gz` & `tmp/RepRepBuild-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.5.0.tar", last modified: Thu Mar 30 21:54:15 2023, max compression
+gzip compressed data, was "RepRepBuild-0.5.1.tar", last modified: Tue Apr 11 13:57:27 2023, max compression
```

## Comparing `RepRepBuild-0.5.0.tar` & `RepRepBuild-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-03-30 21:54:15.613976 RepRepBuild-0.5.0/
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.5.0/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-03-30 21:54:15.613976 RepRepBuild-0.5.0/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.5.0/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1597 2023-03-30 21:53:33.000000 RepRepBuild-0.5.0/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-03-30 21:54:15.613976 RepRepBuild-0.5.0/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-03-30 21:54:15.610976 RepRepBuild-0.5.0/src/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-03-30 21:54:15.611976 RepRepBuild-0.5.0/src/RepRepBuild.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-03-30 21:54:15.000000 RepRepBuild-0.5.0/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-03-30 21:54:15.000000 RepRepBuild-0.5.0/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-03-30 21:54:15.000000 RepRepBuild-0.5.0/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-03-30 21:54:15.000000 RepRepBuild-0.5.0/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       28 2023-03-30 21:54:15.000000 RepRepBuild-0.5.0/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-03-30 21:54:15.000000 RepRepBuild-0.5.0/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-03-30 21:54:15.612976 RepRepBuild-0.5.0/src/reprepbuild/
--rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.5.0/src/reprepbuild/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     9284 2023-03-30 21:46:55.000000 RepRepBuild-0.5.0/src/reprepbuild/__main__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.5.0/src/reprepbuild/articlezip.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3109 2023-03-25 10:49:48.000000 RepRepBuild-0.5.0/src/reprepbuild/bibtex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.5.0/src/reprepbuild/latex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4434 2023-03-25 09:51:45.000000 RepRepBuild-0.5.0/src/reprepbuild/latexdep.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.5.0/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4087 2023-03-25 09:44:04.000000 RepRepBuild-0.5.0/src/reprepbuild/pythonscript.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.5.0/src/reprepbuild/repeat.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.5.0/src/reprepbuild/utils.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.5.0/src/reprepbuild/zip.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-11 13:57:27.689089 RepRepBuild-0.5.1/
+-rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.5.1/COPYING
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-11 13:57:27.688089 RepRepBuild-0.5.1/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.5.1/README.md
+-rw-r--r--   0 toon      (1000) toon      (1000)     1597 2023-04-11 13:56:44.000000 RepRepBuild-0.5.1/pyproject.toml
+-rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-11 13:57:27.689089 RepRepBuild-0.5.1/setup.cfg
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-11 13:57:27.673089 RepRepBuild-0.5.1/src/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-11 13:57:27.674089 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       28 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-11 13:57:27.000000 RepRepBuild-0.5.1/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-11 13:57:27.688089 RepRepBuild-0.5.1/src/reprepbuild/
+-rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.5.1/src/reprepbuild/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     9811 2023-04-11 13:17:07.000000 RepRepBuild-0.5.1/src/reprepbuild/__main__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.5.1/src/reprepbuild/articlezip.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3109 2023-03-25 10:49:48.000000 RepRepBuild-0.5.1/src/reprepbuild/bibtex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.5.1/src/reprepbuild/latex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4434 2023-03-25 09:51:45.000000 RepRepBuild-0.5.1/src/reprepbuild/latexdep.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.5.1/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4087 2023-03-25 09:44:04.000000 RepRepBuild-0.5.1/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.5.1/src/reprepbuild/repeat.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.5.1/src/reprepbuild/utils.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.5.1/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.5.0/COPYING` & `RepRepBuild-0.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/PKG-INFO` & `RepRepBuild-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.5.0
+Version: 0.5.1
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.5.0/README.md` & `RepRepBuild-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/pyproject.toml` & `RepRepBuild-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepRepBuild"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Toon Verstraelen", email="toon.verstraelen@ugent.be" },
 ]
 description = "Build tool for Reproducible Reporting"
 readme = "README.md"
 license = {file = "COPYING"}
 requires-python = ">=3.6"
```

### Comparing `RepRepBuild-0.5.0/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.5.1/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.5.0
+Version: 0.5.1
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.5.0/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.5.1/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/__init__.py` & `RepRepBuild-0.5.1/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/__main__.py` & `RepRepBuild-0.5.1/src/reprepbuild/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,29 +110,42 @@
 def latexdiff_pattern(path):
     """Make ninja build commands to generate a latex diff."""
     result = re.match(r"latex-(?P<prefix>[a-z0-9-]+)/(?P=prefix)-old.(?P<ext>.*)$", path)
     if not result:
         return
     prefix = result.group("prefix")
     ext = result.group("ext")
-    workdir = f"latex_{prefix}"
+    workdir = f"latex-{prefix}"
 
     def fixpath(fn_local):
         return os.path.normpath(os.path.join(workdir, fn_local))
 
     yield {
         "outputs": fixpath(f"{prefix}-diff.{ext}"),
         "rule": "latexdiff",
         "inputs": [fixpath(f"{prefix}-old.{ext}"), fixpath(f"{prefix}.{ext}")],
     }
     if ext == "tex":
         yield {
+            "outputs": fixpath(f"{prefix}-diff.tex.dd"),
+            "implicit_outputs": [
+                fixpath(f"{prefix}-diff.aux"),
+                fixpath(f"{prefix}-diff.first.aux"),
+                fixpath(f"{prefix}-diff.fls"),
+                fixpath(f"{prefix}-diff.log"),
+            ],
+            "rule": "latexdep",
+            "inputs": fixpath(f"{prefix}-diff.tex"),
+        }
+        yield {
             "outputs": fixpath(f"{prefix}-diff.pdf"),
             "rule": "latex",
             "inputs": fixpath(f"{prefix}-diff.tex"),
+            "order_only": fixpath(f"{prefix}-diff.tex.dd"),
+            "dyndep": fixpath(f"{prefix}-diff.tex.dd"),
         }
         yield {
             "outputs": os.path.join("uploads", f"{prefix}-diff.pdf"),
             "rule": "copy",
             "inputs": fixpath(f"{prefix}-diff.pdf"),
             "default": True,
         }
```

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/articlezip.py` & `RepRepBuild-0.5.1/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/bibtex.py` & `RepRepBuild-0.5.1/src/reprepbuild/bibtex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/latex.py` & `RepRepBuild-0.5.1/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/latexdep.py` & `RepRepBuild-0.5.1/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.5.1/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.5.1/src/reprepbuild/pythonscript.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/repeat.py` & `RepRepBuild-0.5.1/src/reprepbuild/repeat.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/utils.py` & `RepRepBuild-0.5.1/src/reprepbuild/utils.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.5.0/src/reprepbuild/zip.py` & `RepRepBuild-0.5.1/src/reprepbuild/zip.py`

 * *Files identical despite different names*

