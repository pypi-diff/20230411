# Comparing `tmp/Trapalyzer-0.0.5.tar.gz` & `tmp/Trapalyzer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/czaki/Projekty/neutrofile/dist/tmp240e51ca/Trapalyzer-0.0.5.tar", last modified: Tue Nov  8 11:09:03 2022, max compression
+gzip compressed data, was "/home/czaki/Projekty/neutrofile/dist/.tmp-zmkhsf7i/Trapalyzer-0.0.6.tar", last modified: Tue Apr 11 10:29:25 2023, max compression
```

## Comparing `Trapalyzer-0.0.5.tar` & `Trapalyzer-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2022-11-08 11:09:03.329834 Trapalyzer-0.0.5/
--rw-rw-r--   0 czaki     (1000) grzegorz  (1000)     4481 2022-11-08 10:29:53.000000 Trapalyzer-0.0.5/.gitignore
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1128 2022-03-23 10:58:30.000000 Trapalyzer-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1111 2021-09-14 08:55:56.000000 Trapalyzer-0.0.5/License.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1978 2022-11-08 11:09:03.329834 Trapalyzer-0.0.5/PKG-INFO
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1155 2022-11-08 09:47:36.000000 Trapalyzer-0.0.5/Readme.md
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2022-11-08 11:09:03.317834 Trapalyzer-0.0.5/Tutorial/
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2022-11-08 11:09:03.325834 Trapalyzer-0.0.5/Tutorial/Figs/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   449991 2021-11-30 23:18:29.000000 Trapalyzer-0.0.5/Tutorial/Figs/0.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   161340 2021-11-30 23:18:29.000000 Trapalyzer-0.0.5/Tutorial/Figs/1.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   204547 2021-11-30 23:18:29.000000 Trapalyzer-0.0.5/Tutorial/Figs/2.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   354022 2021-11-30 23:18:29.000000 Trapalyzer-0.0.5/Tutorial/Figs/3.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    12518 2021-11-30 23:18:29.000000 Trapalyzer-0.0.5/Tutorial/Figs/4.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   365588 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/5.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    33826 2021-11-30 23:18:29.000000 Trapalyzer-0.0.5/Tutorial/Figs/download.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    89369 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/fig 6_2.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   418704 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/fig 6_3.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   484998 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/fig10.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   322530 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/fig6.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   419852 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/fig6_1.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   206264 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/fig7.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   381829 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/fig8.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   247383 2022-03-23 10:37:03.000000 Trapalyzer-0.0.5/Tutorial/Figs/fig9.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    12220 2022-03-23 10:51:57.000000 Trapalyzer-0.0.5/Tutorial/Readme.md
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3478 2022-03-23 10:42:01.000000 Trapalyzer-0.0.5/Tutorial/example_profile.json
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      877 2021-08-05 12:21:15.000000 Trapalyzer-0.0.5/pyproject.toml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1172 2022-11-08 11:09:03.329834 Trapalyzer-0.0.5/setup.cfg
--rw-rw-r--   0 czaki     (1000) grzegorz  (1000)       38 2021-03-09 14:56:49.000000 Trapalyzer-0.0.5/setup.py
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2022-11-08 11:09:03.313834 Trapalyzer-0.0.5/src/
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2022-11-08 11:09:03.325834 Trapalyzer-0.0.5/src/Trapalyzer/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     2018 2022-11-08 09:47:36.000000 Trapalyzer-0.0.5/src/Trapalyzer/__init__.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      176 2022-11-08 11:09:03.000000 Trapalyzer-0.0.5/src/Trapalyzer/_version.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     6829 2022-11-08 10:29:52.000000 Trapalyzer-0.0.5/src/Trapalyzer/measurement.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1445 2021-09-02 16:39:02.000000 Trapalyzer-0.0.5/src/Trapalyzer/napari_functions.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    28808 2022-04-14 19:33:49.000000 Trapalyzer-0.0.5/src/Trapalyzer/segmentation.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     4426 2022-04-14 19:34:30.000000 Trapalyzer-0.0.5/src/Trapalyzer/widgets.py
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2022-11-08 11:09:03.325834 Trapalyzer-0.0.5/src/Trapalyzer.egg-info/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1978 2022-11-08 11:09:03.000000 Trapalyzer-0.0.5/src/Trapalyzer.egg-info/PKG-INFO
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      885 2022-11-08 11:09:03.000000 Trapalyzer-0.0.5/src/Trapalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)        1 2022-11-08 11:09:03.000000 Trapalyzer-0.0.5/src/Trapalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      103 2022-11-08 11:09:03.000000 Trapalyzer-0.0.5/src/Trapalyzer.egg-info/entry_points.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       75 2022-11-08 11:09:03.000000 Trapalyzer-0.0.5/src/Trapalyzer.egg-info/requires.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       11 2022-11-08 11:09:03.000000 Trapalyzer-0.0.5/src/Trapalyzer.egg-info/top_level.txt
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/
+-rw-rw-r--   0 czaki     (1000) grzegorz  (1000)     4481 2022-11-08 10:29:53.000000 Trapalyzer-0.0.6/.gitignore
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1203 2023-04-11 10:23:38.000000 Trapalyzer-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1111 2021-09-14 08:55:56.000000 Trapalyzer-0.0.6/License.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1984 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/PKG-INFO
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1170 2023-04-11 10:28:23.000000 Trapalyzer-0.0.6/Readme.md
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.134333 Trapalyzer-0.0.6/Tutorial/
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/Tutorial/Figs/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   449991 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/0.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   161340 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/1.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   204547 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/2.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   354022 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/3.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    12518 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/4.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   365588 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/5.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    33826 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/download.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    89369 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig 6_2.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   418704 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig 6_3.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   484998 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig10.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   322530 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig6.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   419852 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig6_1.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   206264 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig7.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   381829 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig8.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   247383 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig9.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    26355 2023-04-11 10:28:02.000000 Trapalyzer-0.0.6/Tutorial/Figs/release_img.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    12227 2023-04-11 10:23:38.000000 Trapalyzer-0.0.6/Tutorial/Readme.md
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3478 2022-03-23 10:42:01.000000 Trapalyzer-0.0.6/Tutorial/example_profile.json
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      877 2021-08-05 12:21:15.000000 Trapalyzer-0.0.6/pyproject.toml
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1163 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/setup.cfg
+-rw-rw-r--   0 czaki     (1000) grzegorz  (1000)       38 2021-03-09 14:56:49.000000 Trapalyzer-0.0.6/setup.py
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.134333 Trapalyzer-0.0.6/src/
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/src/Trapalyzer/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     2099 2022-11-28 10:16:04.000000 Trapalyzer-0.0.6/src/Trapalyzer/__init__.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      160 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer/_version.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     6829 2022-11-08 10:29:52.000000 Trapalyzer-0.0.6/src/Trapalyzer/measurement.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1445 2021-09-02 16:39:02.000000 Trapalyzer-0.0.6/src/Trapalyzer/napari_functions.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    28769 2023-02-06 17:30:42.000000 Trapalyzer-0.0.6/src/Trapalyzer/segmentation.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     4426 2022-04-14 19:34:30.000000 Trapalyzer-0.0.6/src/Trapalyzer/widgets.py
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1984 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      915 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)        1 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      103 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/entry_points.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       75 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/requires.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       11 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/top_level.txt
```

### Comparing `Trapalyzer-0.0.5/.gitignore` & `Trapalyzer-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/.pre-commit-config.yaml` & `Trapalyzer-0.0.6/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 default_language_version:
-    python: python3.7
+    python: python3.8
 
 repos:
 -   repo: https://github.com/psf/black
-    rev: 22.1.0
+    rev: 23.1.0
     hooks:
     - id: black
       pass_filenames: true
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
     - id: check-json
     - id: check-yaml
     - id: check-merge-conflict
     - id: end-of-file-fixer
     - id: trailing-whitespace
       exclude: .*\.md
     - id: debug-statements
     - id: mixed-line-ending
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.20.0
+    rev: v2.2.0
     hooks:
     - id: setup-cfg-fmt
+      args: ["--include-version-classifiers", "--max-py-version", "3.10"]
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.1
+    rev: v3.3.1
     hooks:
     - id: pyupgrade
-      args: ["--py37-plus"]
+      args: ["--py38-plus"]
 -   repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
     -   id: rst-backticks
 -   repo: https://github.com/PyCQA/isort
-    rev: '5.10.1'  # Use the revision sha / tag you want to point at
+    rev: '5.12.0'  # Use the revision sha / tag you want to point at
     hooks:
     -   id: isort
 
 -   repo: https://github.com/myint/autoflake
-    rev: 'v1.4'  # Use the revision sha / tag you want to point at
+    rev: 'v2.0.1'  # Use the revision sha / tag you want to point at
     hooks:
     -   id: autoflake
         args: ["--remove-all-unused-imports", "-i"]
```

### Comparing `Trapalyzer-0.0.5/License.txt` & `Trapalyzer-0.0.6/License.txt`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/PKG-INFO` & `Trapalyzer-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Trapalyzer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automatic feature detection and quantification for in-vitro NETosis experiments plugin for PartSeg
-Home-page: https://github.com/Czaki/Neutrofile_analysis
+Home-page: https://github.com/Czaki/Trapalyzer
 Author: Grzegorz Bokota, Michał Ciach
 Author-email: g.bokota@uw.edu.pl, m_ciach@student.uw.edu.pl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -30,19 +30,20 @@
 If you use Windows, you can simply download and unpack the `PartSeg.zip` file -
 no further installation needed. If you use Linux with a working Python
 distribution, we recommend installing PartSeg by running
 `pip install PartSeg[all]` in the command line.
 
 After you have installed PartSeg, you can install Trapalyzer:
 
-- On Windows, download the ZIP file with the plug-in (see the screenshot
-   below). Unpack the .zip archive and move the `Trapalyzer` directory
-   (located in `Trapalyzer-master/src` in the unpacked archive) to the
-  `plugins` directory in the PartSeg folder.
-- On Linux, we recommend installing via `pip install Trapalyzer`.
+- If you install PArtSeg from prebuild binaries (from zip) then you need to download 
+  this plugin from [release page](https://github.com/Czaki/Trapalyzer/releases) and unpack it to `plugins` directory in PartSeg folder.
+- If you install PartSeg using pip or conda then you can install this plugin using pip
+  `pip install Trapalyzer`
 
-![](Tutorial/Figs/download.png)
+
+
+![](Tutorial/Figs/release_img.png)
 
 ## Usage examples
 
 In the Tutorial directory you will find instructions on how to use
 Trapalyzer to analyze an example data set of fluorescence microscopy images.
```

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/0.png` & `Trapalyzer-0.0.6/Tutorial/Figs/0.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/1.png` & `Trapalyzer-0.0.6/Tutorial/Figs/1.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/2.png` & `Trapalyzer-0.0.6/Tutorial/Figs/2.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/3.png` & `Trapalyzer-0.0.6/Tutorial/Figs/3.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/4.png` & `Trapalyzer-0.0.6/Tutorial/Figs/4.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/5.png` & `Trapalyzer-0.0.6/Tutorial/Figs/5.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/download.png` & `Trapalyzer-0.0.6/Tutorial/Figs/download.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/fig 6_2.png` & `Trapalyzer-0.0.6/Tutorial/Figs/fig 6_2.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/fig 6_3.png` & `Trapalyzer-0.0.6/Tutorial/Figs/fig 6_3.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/fig10.png` & `Trapalyzer-0.0.6/Tutorial/Figs/fig10.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/fig6.png` & `Trapalyzer-0.0.6/Tutorial/Figs/fig6.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/fig6_1.png` & `Trapalyzer-0.0.6/Tutorial/Figs/fig6_1.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/fig7.png` & `Trapalyzer-0.0.6/Tutorial/Figs/fig7.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/fig8.png` & `Trapalyzer-0.0.6/Tutorial/Figs/fig8.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Figs/fig9.png` & `Trapalyzer-0.0.6/Tutorial/Figs/fig9.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/Tutorial/Readme.md` & `Trapalyzer-0.0.6/Tutorial/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,19 +64,21 @@
 ![](Figs/5.png)
 
 If you set the acceptable intervals for all three features of NETs and click "Execute", Trapalyzer will update its annotation. The update should be reflected in changed colors of the annotations of NETs and increased quality score. Hover the mouse cursor over one of them to verify that the "Unknown extra" category has changed into the "NET" category.
 
 Now, select the second image (by clicking *raw image* under the second filename in the *Multiple files* window on the left-hand side), click *Execute* again, and check if you need to update the parameters of NETs.
 Trapalyzer should already classify most NETs properly. In this case, move on to the next image. Do not update the parameters if only one small NET is misclassified to avoid overfitting the software to a single image.
 
-Now, select the sixth image. This image contains mostly unstimulated neutrophils (PMN neu). If needed, disable the green channel (if the channel is almost empty, PartSeg may overinflate its brightness).
-Click Execute. All cells will initially be classified as Unknown intra.
-Hover the mouse cursor over some of the detected cells to get the appropriate intervals for the brightness, size, extracellular brightness and brightness gradient for the PMN neu class.
-Try to achieve the annotation quality between 80% and 95%. The partial scores for features (highlighted on the right-hand side of the image below) will tell, on a scale from 0 to 1, how well this feature matches the appropriate interval of the given type of cells.
-Select the fifth image and validate your parameters for the PMN neutrophils.
+Now, select the sixth image. This image contains mostly unstimulated neutrophils (PMN neu). 
+If needed, disable the green channel (if the channel is almost empty, PartSeg may overinflate its brightness). 
+Click Execute. All cells will initially be classified as Unknown intra. 
+Hover the mouse cursor over some of the detected cells to get the appropriate intervals for the brightness, size, extracellular brightness and brightness gradient for the PMN neu class. 
+Try to achieve the annotation quality between 80% and 95%. The partial scores for features (highlighted on the right-hand side of the image below) will tell, on a scale from 0 to 1, how well this feature matches the appropriate interval of the given type of cells. 
+Select the fifth image and validate your parameters for the PMN neutrophils. 
+
 
 ![](Figs/fig6.png)
 
 Repeat this process for the other images and classes of cells that you want to detect.
 Trapalyzer allows to define up to four classes of cells, which are assumed to be:
 
 - Polymorphonuclear, unstimulated neutrophils (PMN neu),
```

### Comparing `Trapalyzer-0.0.5/Tutorial/example_profile.json` & `Trapalyzer-0.0.6/Tutorial/example_profile.json`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/pyproject.toml` & `Trapalyzer-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/setup.cfg` & `Trapalyzer-0.0.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = Trapalyzer
 description = Automatic feature detection and quantification for in-vitro NETosis experiments plugin for PartSeg
 long_description = file: Readme.md
 long_description_content_type = text/markdown
-url = https://github.com/Czaki/Neutrofile_analysis
+url = https://github.com/Czaki/Trapalyzer
 author = Grzegorz Bokota, Michał Ciach
 author_email = g.bokota@uw.edu.pl, m_ciach@student.uw.edu.pl
 license = MIT
 license_file = License.txt
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

### Comparing `Trapalyzer-0.0.5/src/Trapalyzer/__init__.py` & `Trapalyzer-0.0.6/src/Trapalyzer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         import importlib
 
         importlib.reload(segmentation)
         importlib.reload(measurement)
         importlib.reload(widgets)
     # register_fun(segmentation.NeutrofileSegmentation, RegisterEnum.analysis_algorithm)
     register_fun(segmentation.Trapalyzer, RegisterEnum.analysis_algorithm)
+    register_fun(segmentation.TrapalyzerSimple, RegisterEnum.analysis_algorithm)
     register_fun(measurement.ComponentArea, RegisterEnum.analysis_measurement)
     register_fun(measurement.NetPercent, RegisterEnum.analysis_measurement)
     register_fun(measurement.ComponentCount, RegisterEnum.analysis_measurement)
     register_fun(measurement.ClassifyNeutrofile, RegisterEnum.analysis_measurement)
     register_fun(measurement.NeutrofileScore, RegisterEnum.analysis_measurement)
     register_fun(measurement.NeutrofileParameter, RegisterEnum.analysis_measurement)
     register_fun(measurement.ComponentMid, RegisterEnum.analysis_measurement)
```

### Comparing `Trapalyzer-0.0.5/src/Trapalyzer/measurement.py` & `Trapalyzer-0.0.6/src/Trapalyzer/measurement.py`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/src/Trapalyzer/napari_functions.py` & `Trapalyzer-0.0.6/src/Trapalyzer/napari_functions.py`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/src/Trapalyzer/segmentation.py` & `Trapalyzer-0.0.6/src/Trapalyzer/segmentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import operator
 import typing
 from abc import ABC
 from collections import Counter
 from enum import Enum
 from itertools import product
+from typing import Callable
 
 import numpy as np
 import SimpleITK as sitk
 from napari.layers import Image
 from napari.types import LayerDataTuple
 from nme import REGISTER, class_to_str, register_class
 from pydantic import Field
 
 from PartSegCore.algorithm_describe_base import ROIExtractionProfile
 from PartSegCore.analysis.measurement_calculation import Diameter, get_border
 from PartSegCore.autofit import density_mass_center
-from PartSegCore.channel_class import Channel
-from PartSegCore.class_generator import enum_register
 from PartSegCore.roi_info import ROIInfo
 from PartSegCore.segmentation import RestartableAlgorithm
-from PartSegCore.segmentation.algorithm_base import AdditionalLayerDescription, SegmentationResult
+from PartSegCore.segmentation.algorithm_base import AdditionalLayerDescription, ROIExtractionResult
 from PartSegCore.segmentation.noise_filtering import NoiseFilterSelection
-from PartSegCore.segmentation.threshold import BaseThreshold, ThresholdSelection, threshold_dict
+from PartSegCore.segmentation.threshold import BaseThreshold, ThresholdSelection
 from PartSegCore.utils import BaseModel
+from PartSegImage.channel_class import Channel
 
 from .widgets import TrapezoidRange
 
 
+@register_class
 class NeuType(Enum):
     PMN_neu = 1
     RND_neu = 2
     NER_neu = 3
     PMP_neu = 4
     Bacteria = 5
     NET = 8
@@ -57,15 +58,15 @@
 
 
 try:
     # noinspection PyUnresolvedReferences,PyUnboundLocalVariable
     reloading
 except NameError:
     reloading = False  # means the module is being imported
-    enum_register.register_class(NeuType)
+
 
 LABELING_NAME = "Labeling"
 SCORE_SUFFIX = "_score"
 CATEGORY_STR = "category"
 PARAMETER_TYPE_LIST = [
     "pixel count",
     "brightness",
@@ -90,15 +91,15 @@
         return False
 
     @classmethod
     def support_z(cls):
         return False
 
     def _calculate_mask(self, channel, threshold_info):
-        thr: BaseThreshold = threshold_dict[threshold_info.name]
+        thr: BaseThreshold = ThresholdSelection[threshold_info.name]
         mask, thr_val = thr.calculate_mask(channel, self.mask, threshold_info.values, operator.gt)
         return mask, thr_val
 
     @staticmethod
     def _calc_components(arr, min_size, close_holes=0):
         components = sitk.RelabelComponent(
             sitk.ConnectedComponent(sitk.GetImageFromArray(arr)),
@@ -254,15 +255,15 @@
                 "ext. brightness SD": brightness_std,
             }
             annotation[i] = data_dict
             nets[component] = i
             i += 1
         return nets, annotation
 
-    def calculation_run(self, report_fun: typing.Callable[[str, int], None]) -> SegmentationResult:
+    def calculation_run(self, report_fun: typing.Callable[[str, int], None]) -> ROIExtractionResult:
         self.count_dict = Counter()
         self.area_dict = Counter()
         self.nets = 0
         self.other = 0
         self.net_size = 0
         inner_dna_channel = self.get_channel(self.new_parameters.inner_dna)
         self.image_size = inner_dna_channel.shape[0] * inner_dna_channel.shape[1] * inner_dna_channel.shape[2]
@@ -321,17 +322,17 @@
             alternative_representation[str(val)] = (result_labeling == val.value).astype(np.uint8) * val.value
         self.net_size = np.count_nonzero(alternative_representation[str(NeuType.NET)])
         self.area_dict[NeuType.NET] = self.net_size
 
         from .measurement import QualityMeasure
 
         self.quality = QualityMeasure.calculate_property(inner_dna_components, roi_annotation)
-        return SegmentationResult(
-            inner_dna_components,
-            self.get_segmentation_profile(),
+        return ROIExtractionResult(
+            roi=inner_dna_components,
+            parameters=self.get_segmentation_profile(),
             alternative_representation=alternative_representation,
             roi_annotation=roi_annotation,
             additional_layers={
                 "inner_mask": AdditionalLayerDescription(inner_dna_mask.astype(np.uint8), "labels", "inner_mask"),
                 "cleaned outer brightness gradient": AdditionalLayerDescription(
                     _laplacian_estimate(cleaned_outer, 1.3), "image", "cleaned outer brightness gradient"
                 ),
@@ -440,104 +441,86 @@
     def get_segmentation_profile(self) -> ROIExtractionProfile:
         return ROIExtractionProfile(name="", algorithm=self.get_name(), values=self.new_parameters.copy())
 
     @classmethod
     def get_name(cls) -> str:
         return "Trapalyzer"
 
-    # @classmethod
-    # def get_fields(cls) -> typing.List[typing.Union[AlgorithmProperty, str]]:
-    #     initial = list(
-    #         chain(
-    #             *(
-    #                 [
-    #                     AlgorithmProperty(
-    #                         f"{prefix.name.lower()}_{suffix}",
-    #                         f"{prefix} {suffix}",
-    #                         {"lower_bound": 0, "upper_bound": 1},
-    #                         property_type=TrapezoidWidget,
-    #                         help_text=f"{DESCRIPTION_DICT[prefix]} {suffix}",
-    #                     )
-    #                     for suffix in PARAMETER_TYPE_LIST
-    #                 ]
-    #                 + ["-------------------"]
-    #                 for prefix in NeuType.neutrofile_components()
-    #             )
-    #         )
-    #     ) + [
-    #         AlgorithmProperty("minimum_score", "Minimum score", 0.8),
-    #         AlgorithmProperty("maximum_other", "Maximum competing score", 0.4),
-    #         AlgorithmProperty(
-    #             "minimum_size", "Minimum comp. pixel count", 40, (1, 9999), help_text="Minimum component pixel count"
-    #         ),
-    #         AlgorithmProperty("softness", "Error margin coeficient", 0.1, (0, 1)),
-    #     ]
-    #
-    #     thresholds = [
-    #         AlgorithmProperty("inner_dna", "All DNA channel", 1, property_type=Channel),
-    #         AlgorithmProperty(
-    #             "inner_dna_noise_filtering",
-    #             "Filter type",
-    #             next(iter(noise_filtering_dict.keys())),
-    #             possible_values=noise_filtering_dict,
-    #             value_type=AlgorithmDescribeBase,
-    #         ),
-    #         AlgorithmProperty(
-    #             "inner_threshold",
-    #             "Threshold type",
-    #             next(iter(threshold_dict.keys())),
-    #             possible_values=threshold_dict,
-    #             property_type=AlgorithmDescribeBase,
-    #         ),
-    #         AlgorithmProperty("outer_dna", "Extracellural DNA channel", 1, property_type=Channel),
-    #         AlgorithmProperty(
-    #             "outer_dna_noise_filtering",
-    #             "Filter type",
-    #             next(iter(noise_filtering_dict.keys())),
-    #             possible_values=noise_filtering_dict,
-    #             value_type=AlgorithmDescribeBase,
-    #         ),
-    #         AlgorithmProperty(
-    #             "outer_threshold",
-    #             "Threshold type",
-    #             next(iter(threshold_dict.keys())),
-    #             possible_values=threshold_dict,
-    #             property_type=AlgorithmDescribeBase,
-    #         ),
-    #         AlgorithmProperty(
-    #             "net_size",
-    #             "NET pixel count",
-    #             {"lower_bound": 850, "upper_bound": 999999},
-    #             property_type=TrapezoidWidget,
-    #         ),
-    #         AlgorithmProperty(
-    #             "net_ext_brightness",
-    #             "NET extracellular brightness",
-    #             {"lower_bound": 21, "upper_bound": 100},
-    #             property_type=TrapezoidWidget,
-    #         ),
-    #         # AlgorithmProperty(
-    #         #     "net_brightness_gradient",
-    #         #     "NET ext. brightness gradient",
-    #         #     {"lower_bound": -1.0, "upper_bound": 1.0},
-    #         #     property_type=TrapezoidWidget,
-    #         # ),
-    #         AlgorithmProperty(
-    #             "net_ext_brightness_std",
-    #             "NET ext. brightness SD",
-    #             {"lower_bound": 0.0, "upper_bound": 1.0},
-    #             property_type=TrapezoidWidget,
-    #         ),
-    #         AlgorithmProperty(
-    #             "unknown_net", "detect extracellular artifacts", True, help_text="If mark unknown net components"
-    #         ),
-    #         "-----------------------",
-    #     ]
-    #
-    #     return thresholds + initial
+
+class TrapalyzerSimpleParameters(BaseModel):
+    inner_dna: Channel = Field(1, title="All DNA channel")
+    inner_dna_noise_filtering: NoiseFilterSelection = Field(NoiseFilterSelection.get_default(), title="Filter type")
+    inner_threshold: ThresholdSelection = Field(ThresholdSelection.get_default(), title="Threshold type")
+    outer_dna: Channel = Field(1, title="Extracellural DNA channel")
+    outer_dna_noise_filtering: NoiseFilterSelection = Field(NoiseFilterSelection.get_default(), title="Filter type")
+    dead_threshold: ThresholdSelection = Field(ThresholdSelection.get_default(), title="Thr. dead neu")
+    net_threshold: ThresholdSelection = Field(ThresholdSelection.get_default(), title="Threshold NET")
+    minimum_size: int = Field(
+        40, title="Minimum comp. pixel count", description="Minimum component pixel count", ge=1, le=9999
+    )
+
+
+class TrapalyzerSimple(NeutrofileSegmentationBase):
+    __argument_class__ = TrapalyzerSimpleParameters
+    new_parameters: TrapalyzerSimpleParameters
+
+    def calculation_run(self, report_fun: Callable[[str, int], None]) -> ROIExtractionResult:
+        inner_dna_channel = self.get_channel(self.new_parameters.inner_dna)
+        inner_noise_filtering_parameters = self.new_parameters.inner_dna_noise_filtering
+        cleaned_inner = NoiseFilterSelection[inner_noise_filtering_parameters.name].noise_filter(
+            inner_dna_channel, self.image.spacing, inner_noise_filtering_parameters.values
+        )
+        inner_dna_mask, thr_val = self._calculate_mask(cleaned_inner, self.new_parameters.inner_threshold)
+
+        outer_dna_channel = self.get_channel(self.new_parameters.outer_dna)
+        outer_noise_filtering_parameters = self.new_parameters.outer_dna_noise_filtering
+        cleaned_outer = NoiseFilterSelection[outer_noise_filtering_parameters.name].noise_filter(
+            outer_dna_channel, self.image.spacing, outer_noise_filtering_parameters.values
+        )
+        dead_dna_mask, dead_thr_val = self._calculate_mask(cleaned_outer, self.new_parameters.dead_threshold)
+        net_dna_mask, net_thr_val = self._calculate_mask(cleaned_outer, self.new_parameters.net_threshold)
+
+        inner_dna_components = self._calc_components(inner_dna_mask, self.new_parameters.minimum_size, close_holes=100)
+
+        labeled_neu, roi_annotation = self._classify_neutrofile(inner_dna_components, dead_dna_mask)
+
+        net_dna_mask[inner_dna_components > 0] = 0
+        net_components = self._calc_components(net_dna_mask, self.new_parameters.minimum_size, close_holes=100)
+
+        cmp_max = inner_dna_components.max()
+        for i in range(cmp_max + 1, cmp_max + net_components.max() + 1):
+            roi_annotation[i] = {CATEGORY_STR: 3}
+
+        labeled_neu[net_components > 0] = 3
+        inner_dna_components[net_components > 0] = net_components[net_components > 0] + cmp_max
+
+        return ROIExtractionResult(
+            roi=inner_dna_components,
+            parameters=self.get_segmentation_profile(),
+            alternative_representation={LABELING_NAME: labeled_neu},
+            roi_annotation=roi_annotation,
+        )
+
+    def _classify_neutrofile(self, inner_dna_components, dead_dna_mask):
+        bounds = ROIInfo.calc_bounds(inner_dna_components)
+        mapping = np.arange(0, np.max(inner_dna_components) + 1, dtype=np.uint16)
+        annotation = {}
+        for val in np.unique(inner_dna_components):
+            if val == 0:
+                continue
+            slices = tuple(bounds[val].get_slices(margin=5))
+            component_mask = inner_dna_components[slices] == val
+            dead_mask = dead_dna_mask[slices]
+            mapping[val] = 2 if np.any(component_mask * dead_mask) else 1
+            annotation[val] = {CATEGORY_STR: mapping[val]}
+        return mapping[inner_dna_components], annotation
+
+    @classmethod
+    def get_name(cls) -> str:
+        return "Trapalyzer simple"
 
 
 def trapezoid_score_function(x, lower_bound, upper_bound, softness=0.5):
     """
     Compute a score on a scale from 0 to 1 that indicate whether values from x belong
     to the interval (lbound, ubound) with a softened boundary.
     If a point lies inside the interval, its score is equal to 1.
```

### Comparing `Trapalyzer-0.0.5/src/Trapalyzer/widgets.py` & `Trapalyzer-0.0.6/src/Trapalyzer/widgets.py`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.5/src/Trapalyzer.egg-info/PKG-INFO` & `Trapalyzer-0.0.6/src/Trapalyzer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Trapalyzer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automatic feature detection and quantification for in-vitro NETosis experiments plugin for PartSeg
-Home-page: https://github.com/Czaki/Neutrofile_analysis
+Home-page: https://github.com/Czaki/Trapalyzer
 Author: Grzegorz Bokota, Michał Ciach
 Author-email: g.bokota@uw.edu.pl, m_ciach@student.uw.edu.pl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -30,19 +30,20 @@
 If you use Windows, you can simply download and unpack the `PartSeg.zip` file -
 no further installation needed. If you use Linux with a working Python
 distribution, we recommend installing PartSeg by running
 `pip install PartSeg[all]` in the command line.
 
 After you have installed PartSeg, you can install Trapalyzer:
 
-- On Windows, download the ZIP file with the plug-in (see the screenshot
-   below). Unpack the .zip archive and move the `Trapalyzer` directory
-   (located in `Trapalyzer-master/src` in the unpacked archive) to the
-  `plugins` directory in the PartSeg folder.
-- On Linux, we recommend installing via `pip install Trapalyzer`.
+- If you install PArtSeg from prebuild binaries (from zip) then you need to download 
+  this plugin from [release page](https://github.com/Czaki/Trapalyzer/releases) and unpack it to `plugins` directory in PartSeg folder.
+- If you install PartSeg using pip or conda then you can install this plugin using pip
+  `pip install Trapalyzer`
 
-![](Tutorial/Figs/download.png)
+
+
+![](Tutorial/Figs/release_img.png)
 
 ## Usage examples
 
 In the Tutorial directory you will find instructions on how to use
 Trapalyzer to analyze an example data set of fluorescence microscopy images.
```

### Comparing `Trapalyzer-0.0.5/src/Trapalyzer.egg-info/SOURCES.txt` & `Trapalyzer-0.0.6/src/Trapalyzer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 Tutorial/Figs/fig 6_3.png
 Tutorial/Figs/fig10.png
 Tutorial/Figs/fig6.png
 Tutorial/Figs/fig6_1.png
 Tutorial/Figs/fig7.png
 Tutorial/Figs/fig8.png
 Tutorial/Figs/fig9.png
+Tutorial/Figs/release_img.png
 src/Trapalyzer/__init__.py
 src/Trapalyzer/_version.py
 src/Trapalyzer/measurement.py
 src/Trapalyzer/napari_functions.py
 src/Trapalyzer/segmentation.py
 src/Trapalyzer/widgets.py
 src/Trapalyzer.egg-info/PKG-INFO
```

