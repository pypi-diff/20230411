# Comparing `tmp/Trapalyzer-0.0.6.tar.gz` & `tmp/Trapalyzer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/czaki/Projekty/neutrofile/dist/.tmp-zmkhsf7i/Trapalyzer-0.0.6.tar", last modified: Tue Apr 11 10:29:25 2023, max compression
+gzip compressed data, was "/home/czaki/Projekty/neutrofile/dist/.tmp-y2wn7opa/Trapalyzer-0.0.7.tar", last modified: Tue Apr 11 10:37:52 2023, max compression
```

## Comparing `Trapalyzer-0.0.6.tar` & `Trapalyzer-0.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/
--rw-rw-r--   0 czaki     (1000) grzegorz  (1000)     4481 2022-11-08 10:29:53.000000 Trapalyzer-0.0.6/.gitignore
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1203 2023-04-11 10:23:38.000000 Trapalyzer-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1111 2021-09-14 08:55:56.000000 Trapalyzer-0.0.6/License.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1984 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/PKG-INFO
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1170 2023-04-11 10:28:23.000000 Trapalyzer-0.0.6/Readme.md
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.134333 Trapalyzer-0.0.6/Tutorial/
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/Tutorial/Figs/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   449991 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/0.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   161340 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/1.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   204547 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/2.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   354022 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/3.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    12518 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/4.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   365588 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/5.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    33826 2021-11-30 23:18:29.000000 Trapalyzer-0.0.6/Tutorial/Figs/download.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    89369 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig 6_2.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   418704 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig 6_3.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   484998 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig10.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   322530 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig6.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   419852 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig6_1.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   206264 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig7.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   381829 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig8.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)   247383 2022-03-23 10:37:03.000000 Trapalyzer-0.0.6/Tutorial/Figs/fig9.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    26355 2023-04-11 10:28:02.000000 Trapalyzer-0.0.6/Tutorial/Figs/release_img.png
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    12227 2023-04-11 10:23:38.000000 Trapalyzer-0.0.6/Tutorial/Readme.md
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3478 2022-03-23 10:42:01.000000 Trapalyzer-0.0.6/Tutorial/example_profile.json
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      877 2021-08-05 12:21:15.000000 Trapalyzer-0.0.6/pyproject.toml
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1163 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/setup.cfg
--rw-rw-r--   0 czaki     (1000) grzegorz  (1000)       38 2021-03-09 14:56:49.000000 Trapalyzer-0.0.6/setup.py
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.134333 Trapalyzer-0.0.6/src/
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/src/Trapalyzer/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     2099 2022-11-28 10:16:04.000000 Trapalyzer-0.0.6/src/Trapalyzer/__init__.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      160 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer/_version.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     6829 2022-11-08 10:29:52.000000 Trapalyzer-0.0.6/src/Trapalyzer/measurement.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1445 2021-09-02 16:39:02.000000 Trapalyzer-0.0.6/src/Trapalyzer/napari_functions.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)    28769 2023-02-06 17:30:42.000000 Trapalyzer-0.0.6/src/Trapalyzer/segmentation.py
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     4426 2022-04-14 19:34:30.000000 Trapalyzer-0.0.6/src/Trapalyzer/widgets.py
-drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:29:25.146333 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1984 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/PKG-INFO
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      915 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)        1 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)      103 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/entry_points.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       75 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/requires.txt
--rw-r--r--   0 czaki     (1000) grzegorz  (1000)       11 2023-04-11 10:29:25.000000 Trapalyzer-0.0.6/src/Trapalyzer.egg-info/top_level.txt
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:37:52.681590 Trapalyzer-0.0.7/
+-rw-rw-r--   0 czaki     (1000) grzegorz  (1000)     4481 2022-11-08 10:29:53.000000 Trapalyzer-0.0.7/.gitignore
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1203 2023-04-11 10:23:38.000000 Trapalyzer-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1111 2021-09-14 08:55:56.000000 Trapalyzer-0.0.7/License.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1984 2023-04-11 10:37:52.681590 Trapalyzer-0.0.7/PKG-INFO
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1170 2023-04-11 10:36:25.000000 Trapalyzer-0.0.7/Readme.md
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:37:52.673590 Trapalyzer-0.0.7/Tutorial/
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:37:52.677590 Trapalyzer-0.0.7/Tutorial/Figs/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   449991 2021-11-30 23:18:29.000000 Trapalyzer-0.0.7/Tutorial/Figs/0.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   161340 2021-11-30 23:18:29.000000 Trapalyzer-0.0.7/Tutorial/Figs/1.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   204547 2021-11-30 23:18:29.000000 Trapalyzer-0.0.7/Tutorial/Figs/2.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   354022 2021-11-30 23:18:29.000000 Trapalyzer-0.0.7/Tutorial/Figs/3.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    12518 2021-11-30 23:18:29.000000 Trapalyzer-0.0.7/Tutorial/Figs/4.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   365588 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/5.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    33826 2021-11-30 23:18:29.000000 Trapalyzer-0.0.7/Tutorial/Figs/download.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    89369 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/fig 6_2.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   418704 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/fig 6_3.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   484998 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/fig10.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   322530 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/fig6.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   419852 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/fig6_1.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   206264 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/fig7.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   381829 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/fig8.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)   247383 2022-03-23 10:37:03.000000 Trapalyzer-0.0.7/Tutorial/Figs/fig9.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    36397 2023-04-11 10:32:34.000000 Trapalyzer-0.0.7/Tutorial/Figs/release_img.png
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    12227 2023-04-11 10:23:38.000000 Trapalyzer-0.0.7/Tutorial/Readme.md
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3478 2022-03-23 10:42:01.000000 Trapalyzer-0.0.7/Tutorial/example_profile.json
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      877 2021-08-05 12:21:15.000000 Trapalyzer-0.0.7/pyproject.toml
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1163 2023-04-11 10:37:52.681590 Trapalyzer-0.0.7/setup.cfg
+-rw-rw-r--   0 czaki     (1000) grzegorz  (1000)       38 2021-03-09 14:56:49.000000 Trapalyzer-0.0.7/setup.py
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:37:52.673590 Trapalyzer-0.0.7/src/
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:37:52.681590 Trapalyzer-0.0.7/src/Trapalyzer/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     2099 2022-11-28 10:16:04.000000 Trapalyzer-0.0.7/src/Trapalyzer/__init__.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      160 2023-04-11 10:37:52.000000 Trapalyzer-0.0.7/src/Trapalyzer/_version.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     6829 2022-11-08 10:29:52.000000 Trapalyzer-0.0.7/src/Trapalyzer/measurement.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1445 2021-09-02 16:39:02.000000 Trapalyzer-0.0.7/src/Trapalyzer/napari_functions.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)    28769 2023-02-06 17:30:42.000000 Trapalyzer-0.0.7/src/Trapalyzer/segmentation.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     4426 2022-04-14 19:34:30.000000 Trapalyzer-0.0.7/src/Trapalyzer/widgets.py
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-04-11 10:37:52.681590 Trapalyzer-0.0.7/src/Trapalyzer.egg-info/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1984 2023-04-11 10:37:52.000000 Trapalyzer-0.0.7/src/Trapalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      915 2023-04-11 10:37:52.000000 Trapalyzer-0.0.7/src/Trapalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)        1 2023-04-11 10:37:52.000000 Trapalyzer-0.0.7/src/Trapalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      103 2023-04-11 10:37:52.000000 Trapalyzer-0.0.7/src/Trapalyzer.egg-info/entry_points.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       75 2023-04-11 10:37:52.000000 Trapalyzer-0.0.7/src/Trapalyzer.egg-info/requires.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       11 2023-04-11 10:37:52.000000 Trapalyzer-0.0.7/src/Trapalyzer.egg-info/top_level.txt
```

### Comparing `Trapalyzer-0.0.6/.gitignore` & `Trapalyzer-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/.pre-commit-config.yaml` & `Trapalyzer-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/License.txt` & `Trapalyzer-0.0.7/License.txt`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/PKG-INFO` & `Trapalyzer-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Trapalyzer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatic feature detection and quantification for in-vitro NETosis experiments plugin for PartSeg
 Home-page: https://github.com/Czaki/Trapalyzer
 Author: Grzegorz Bokota, Michał Ciach
 Author-email: g.bokota@uw.edu.pl, m_ciach@student.uw.edu.pl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 If you use Windows, you can simply download and unpack the `PartSeg.zip` file -
 no further installation needed. If you use Linux with a working Python
 distribution, we recommend installing PartSeg by running
 `pip install PartSeg[all]` in the command line.
 
 After you have installed PartSeg, you can install Trapalyzer:
 
-- If you install PArtSeg from prebuild binaries (from zip) then you need to download 
+- If you install PartSeg from prebuild binaries (from zip) then you need to download 
   this plugin from [release page](https://github.com/Czaki/Trapalyzer/releases) and unpack it to `plugins` directory in PartSeg folder.
 - If you install PartSeg using pip or conda then you can install this plugin using pip
   `pip install Trapalyzer`
 
 
 
 ![](Tutorial/Figs/release_img.png)
```

### Comparing `Trapalyzer-0.0.6/Readme.md` & `Trapalyzer-0.0.7/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 If you use Windows, you can simply download and unpack the `PartSeg.zip` file -
 no further installation needed. If you use Linux with a working Python
 distribution, we recommend installing PartSeg by running
 `pip install PartSeg[all]` in the command line.
 
 After you have installed PartSeg, you can install Trapalyzer:
 
-- If you install PArtSeg from prebuild binaries (from zip) then you need to download 
+- If you install PartSeg from prebuild binaries (from zip) then you need to download 
   this plugin from [release page](https://github.com/Czaki/Trapalyzer/releases) and unpack it to `plugins` directory in PartSeg folder.
 - If you install PartSeg using pip or conda then you can install this plugin using pip
   `pip install Trapalyzer`
 
 
 
 ![](Tutorial/Figs/release_img.png)
```

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/0.png` & `Trapalyzer-0.0.7/Tutorial/Figs/0.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/1.png` & `Trapalyzer-0.0.7/Tutorial/Figs/1.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/2.png` & `Trapalyzer-0.0.7/Tutorial/Figs/2.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/3.png` & `Trapalyzer-0.0.7/Tutorial/Figs/3.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/4.png` & `Trapalyzer-0.0.7/Tutorial/Figs/4.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/5.png` & `Trapalyzer-0.0.7/Tutorial/Figs/5.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/download.png` & `Trapalyzer-0.0.7/Tutorial/Figs/download.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/fig 6_2.png` & `Trapalyzer-0.0.7/Tutorial/Figs/fig 6_2.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/fig 6_3.png` & `Trapalyzer-0.0.7/Tutorial/Figs/fig 6_3.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/fig10.png` & `Trapalyzer-0.0.7/Tutorial/Figs/fig10.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/fig6.png` & `Trapalyzer-0.0.7/Tutorial/Figs/fig6.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/fig6_1.png` & `Trapalyzer-0.0.7/Tutorial/Figs/fig6_1.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/fig7.png` & `Trapalyzer-0.0.7/Tutorial/Figs/fig7.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/fig8.png` & `Trapalyzer-0.0.7/Tutorial/Figs/fig8.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Figs/fig9.png` & `Trapalyzer-0.0.7/Tutorial/Figs/fig9.png`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/Readme.md` & `Trapalyzer-0.0.7/Tutorial/Readme.md`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/Tutorial/example_profile.json` & `Trapalyzer-0.0.7/Tutorial/example_profile.json`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/pyproject.toml` & `Trapalyzer-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/setup.cfg` & `Trapalyzer-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/src/Trapalyzer/__init__.py` & `Trapalyzer-0.0.7/src/Trapalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/src/Trapalyzer/measurement.py` & `Trapalyzer-0.0.7/src/Trapalyzer/measurement.py`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/src/Trapalyzer/napari_functions.py` & `Trapalyzer-0.0.7/src/Trapalyzer/napari_functions.py`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/src/Trapalyzer/segmentation.py` & `Trapalyzer-0.0.7/src/Trapalyzer/segmentation.py`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/src/Trapalyzer/widgets.py` & `Trapalyzer-0.0.7/src/Trapalyzer/widgets.py`

 * *Files identical despite different names*

### Comparing `Trapalyzer-0.0.6/src/Trapalyzer.egg-info/PKG-INFO` & `Trapalyzer-0.0.7/src/Trapalyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Trapalyzer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatic feature detection and quantification for in-vitro NETosis experiments plugin for PartSeg
 Home-page: https://github.com/Czaki/Trapalyzer
 Author: Grzegorz Bokota, Michał Ciach
 Author-email: g.bokota@uw.edu.pl, m_ciach@student.uw.edu.pl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 If you use Windows, you can simply download and unpack the `PartSeg.zip` file -
 no further installation needed. If you use Linux with a working Python
 distribution, we recommend installing PartSeg by running
 `pip install PartSeg[all]` in the command line.
 
 After you have installed PartSeg, you can install Trapalyzer:
 
-- If you install PArtSeg from prebuild binaries (from zip) then you need to download 
+- If you install PartSeg from prebuild binaries (from zip) then you need to download 
   this plugin from [release page](https://github.com/Czaki/Trapalyzer/releases) and unpack it to `plugins` directory in PartSeg folder.
 - If you install PartSeg using pip or conda then you can install this plugin using pip
   `pip install Trapalyzer`
 
 
 
 ![](Tutorial/Figs/release_img.png)
```

### Comparing `Trapalyzer-0.0.6/src/Trapalyzer.egg-info/SOURCES.txt` & `Trapalyzer-0.0.7/src/Trapalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

