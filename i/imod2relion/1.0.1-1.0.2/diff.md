# Comparing `tmp/imod2relion-1.0.1.tar.gz` & `tmp/imod2relion-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imod2relion-1.0.1.tar", last modified: Tue Apr 11 03:57:28 2023, max compression
+gzip compressed data, was "imod2relion-1.0.2.tar", last modified: Tue Apr 11 04:01:16 2023, max compression
```

## Comparing `imod2relion-1.0.1.tar` & `imod2relion-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 03:57:28.823452 imod2relion-1.0.1/
--rw-r--r--   0 hzvictor   (501) staff       (20)      544 2023-04-11 03:57:28.823331 imod2relion-1.0.1/PKG-INFO
--rw-r--r--   0 hzvictor   (501) staff       (20)      179 2023-04-11 03:42:54.000000 imod2relion-1.0.1/README.md
-drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 03:57:28.822305 imod2relion-1.0.1/imod2relion/
--rw-r--r--   0 hzvictor   (501) staff       (20)       81 2023-04-11 03:57:24.000000 imod2relion-1.0.1/imod2relion/__init__.py
--rw-r--r--   0 hzvictor   (501) staff       (20)     2790 2023-04-11 03:18:38.000000 imod2relion-1.0.1/imod2relion/_utils.py
--rw-r--r--   0 hzvictor   (501) staff       (20)     3201 2023-04-11 03:30:08.000000 imod2relion-1.0.1/imod2relion/main.py
--rw-r--r--   0 hzvictor   (501) staff       (20)     1630 2023-04-10 15:42:42.000000 imod2relion-1.0.1/imod2relion/test.py
-drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 03:57:28.823165 imod2relion-1.0.1/imod2relion.egg-info/
--rw-r--r--   0 hzvictor   (501) staff       (20)      544 2023-04-11 03:57:28.000000 imod2relion-1.0.1/imod2relion.egg-info/PKG-INFO
--rw-r--r--   0 hzvictor   (501) staff       (20)      316 2023-04-11 03:57:28.000000 imod2relion-1.0.1/imod2relion.egg-info/SOURCES.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)        1 2023-04-11 03:57:28.000000 imod2relion-1.0.1/imod2relion.egg-info/dependency_links.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)       54 2023-04-11 03:57:28.000000 imod2relion-1.0.1/imod2relion.egg-info/entry_points.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)       45 2023-04-11 03:57:28.000000 imod2relion-1.0.1/imod2relion.egg-info/requires.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)       12 2023-04-11 03:57:28.000000 imod2relion-1.0.1/imod2relion.egg-info/top_level.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)       38 2023-04-11 03:57:28.823495 imod2relion-1.0.1/setup.cfg
--rw-r--r--   0 hzvictor   (501) staff       (20)      891 2023-04-11 03:46:36.000000 imod2relion-1.0.1/setup.py
+drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 04:01:16.370798 imod2relion-1.0.2/
+-rw-r--r--   0 hzvictor   (501) staff       (20)      584 2023-04-11 04:01:16.370679 imod2relion-1.0.2/PKG-INFO
+-rw-r--r--   0 hzvictor   (501) staff       (20)      179 2023-04-11 03:42:54.000000 imod2relion-1.0.2/README.md
+drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 04:01:16.369729 imod2relion-1.0.2/imod2relion/
+-rw-r--r--   0 hzvictor   (501) staff       (20)       81 2023-04-11 04:01:04.000000 imod2relion-1.0.2/imod2relion/__init__.py
+-rw-r--r--   0 hzvictor   (501) staff       (20)     2790 2023-04-11 03:18:38.000000 imod2relion-1.0.2/imod2relion/_utils.py
+-rw-r--r--   0 hzvictor   (501) staff       (20)     3201 2023-04-11 03:30:08.000000 imod2relion-1.0.2/imod2relion/main.py
+-rw-r--r--   0 hzvictor   (501) staff       (20)     1630 2023-04-10 15:42:42.000000 imod2relion-1.0.2/imod2relion/test.py
+drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 04:01:16.370515 imod2relion-1.0.2/imod2relion.egg-info/
+-rw-r--r--   0 hzvictor   (501) staff       (20)      584 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/PKG-INFO
+-rw-r--r--   0 hzvictor   (501) staff       (20)      316 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/SOURCES.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)        1 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/dependency_links.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)       54 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/entry_points.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)       45 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/requires.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)       12 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/top_level.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)       38 2023-04-11 04:01:16.370840 imod2relion-1.0.2/setup.cfg
+-rw-r--r--   0 hzvictor   (501) staff       (20)      960 2023-04-11 04:00:34.000000 imod2relion-1.0.2/setup.py
```

### Comparing `imod2relion-1.0.1/PKG-INFO` & `imod2relion-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: imod2relion
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool reading IMOD points, obtaining particles' info and generating .star file for RELION
 Home-page: https://github.com/ZhenHuangLab/imod2relion
 Author: Zhen Huang
 Author-email: hzvictor@zju.edu.cn
 License: BSD 3-Clause License
 Keywords: cryo-em,cryo-et,imod,relion,starfile
 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 
 # imod2relion
 
 
 
 A tool reading IMOD points, obtaining particles' info and generating .star file for RELION.
```

### Comparing `imod2relion-1.0.1/imod2relion/_utils.py` & `imod2relion-1.0.2/imod2relion/_utils.py`

 * *Files identical despite different names*

### Comparing `imod2relion-1.0.1/imod2relion/main.py` & `imod2relion-1.0.2/imod2relion/main.py`

 * *Files identical despite different names*

### Comparing `imod2relion-1.0.1/imod2relion/test.py` & `imod2relion-1.0.2/imod2relion/test.py`

 * *Files identical despite different names*

### Comparing `imod2relion-1.0.1/imod2relion.egg-info/PKG-INFO` & `imod2relion-1.0.2/imod2relion.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: imod2relion
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool reading IMOD points, obtaining particles' info and generating .star file for RELION
 Home-page: https://github.com/ZhenHuangLab/imod2relion
 Author: Zhen Huang
 Author-email: hzvictor@zju.edu.cn
 License: BSD 3-Clause License
 Keywords: cryo-em,cryo-et,imod,relion,starfile
 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 
 # imod2relion
 
 
 
 A tool reading IMOD points, obtaining particles' info and generating .star file for RELION.
```

### Comparing `imod2relion-1.0.1/setup.py` & `imod2relion-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 setup(
     name = 'imod2relion',
     packages = find_packages(),
     version=f'{__version__}',
     license='BSD 3-Clause License',
     description='''A tool reading IMOD points, obtaining particles' info and generating .star file for RELION''',
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding='utf-8').read(),
+    long_description_content_type='text/markdown',
     author=f'{__author__}',
     author_email=f'{__email__}',
     url='https://github.com/ZhenHuangLab/imod2relion',
     keywords=['cryo-em', 'cryo-et', 'imod', 'relion', 'starfile'],
     python_requires='>=3.9',
     install_requires=[
         'starfile>=0.4.11',
```

