# Comparing `tmp/ojtool-0.1.0.tar.gz` & `tmp/ojtool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ojtool-0.1.0.tar", last modified: Mon Apr 10 02:22:14 2023, max compression
+gzip compressed data, was "ojtool-0.1.1.tar", last modified: Tue Apr 11 07:20:01 2023, max compression
```

## Comparing `ojtool-0.1.0.tar` & `ojtool-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-10 02:22:14.565809 ojtool-0.1.0/
--rw-r--r--   0 jihongwang   (501) staff       (20)     1073 2023-04-10 02:07:11.000000 ojtool-0.1.0/LICENSE
--rw-r--r--   0 jihongwang   (501) staff       (20)      573 2023-04-10 02:22:14.565670 ojtool-0.1.0/PKG-INFO
--rw-r--r--   0 jihongwang   (501) staff       (20)       59 2023-04-10 02:07:11.000000 ojtool-0.1.0/README.md
--rw-r--r--   0 jihongwang   (501) staff       (20)       84 2023-04-10 02:07:11.000000 ojtool-0.1.0/pyproject.toml
--rw-r--r--   0 jihongwang   (501) staff       (20)       38 2023-04-10 02:22:14.565855 ojtool-0.1.0/setup.cfg
--rw-r--r--   0 jihongwang   (501) staff       (20)      812 2023-04-10 02:21:53.000000 ojtool-0.1.0/setup.py
-drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-10 02:22:14.562737 ojtool-0.1.0/src/
-drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-10 02:22:14.564532 ojtool-0.1.0/src/ojtool/
--rw-r--r--   0 jihongwang   (501) staff       (20)       41 2023-04-10 02:07:11.000000 ojtool-0.1.0/src/ojtool/__init__.py
--rw-r--r--   0 jihongwang   (501) staff       (20)     5048 2023-04-10 02:10:51.000000 ojtool-0.1.0/src/ojtool/ojtool.py
--rw-r--r--   0 jihongwang   (501) staff       (20)      395 2023-04-10 02:14:36.000000 ojtool-0.1.0/src/ojtool/utils.py
-drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-10 02:22:14.565484 ojtool-0.1.0/src/ojtool.egg-info/
--rw-r--r--   0 jihongwang   (501) staff       (20)      573 2023-04-10 02:22:14.000000 ojtool-0.1.0/src/ojtool.egg-info/PKG-INFO
--rw-r--r--   0 jihongwang   (501) staff       (20)      241 2023-04-10 02:22:14.000000 ojtool-0.1.0/src/ojtool.egg-info/SOURCES.txt
--rw-r--r--   0 jihongwang   (501) staff       (20)        1 2023-04-10 02:22:14.000000 ojtool-0.1.0/src/ojtool.egg-info/dependency_links.txt
--rw-r--r--   0 jihongwang   (501) staff       (20)        7 2023-04-10 02:22:14.000000 ojtool-0.1.0/src/ojtool.egg-info/top_level.txt
+drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-11 07:20:01.418419 ojtool-0.1.1/
+-rw-r--r--   0 jihongwang   (501) staff       (20)     1073 2023-04-10 02:07:11.000000 ojtool-0.1.1/LICENSE
+-rw-r--r--   0 jihongwang   (501) staff       (20)      573 2023-04-11 07:20:01.418279 ojtool-0.1.1/PKG-INFO
+-rw-r--r--   0 jihongwang   (501) staff       (20)       59 2023-04-10 02:07:11.000000 ojtool-0.1.1/README.md
+-rw-r--r--   0 jihongwang   (501) staff       (20)       84 2023-04-10 02:07:11.000000 ojtool-0.1.1/pyproject.toml
+-rw-r--r--   0 jihongwang   (501) staff       (20)       38 2023-04-11 07:20:01.418456 ojtool-0.1.1/setup.cfg
+-rw-r--r--   0 jihongwang   (501) staff       (20)      812 2023-04-11 07:19:27.000000 ojtool-0.1.1/setup.py
+drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-11 07:20:01.411584 ojtool-0.1.1/src/
+drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-11 07:20:01.417138 ojtool-0.1.1/src/ojtool/
+-rw-r--r--   0 jihongwang   (501) staff       (20)       41 2023-04-10 02:07:11.000000 ojtool-0.1.1/src/ojtool/__init__.py
+-rw-r--r--   0 jihongwang   (501) staff       (20)     5060 2023-04-11 07:19:10.000000 ojtool-0.1.1/src/ojtool/ojtool.py
+-rw-r--r--   0 jihongwang   (501) staff       (20)      425 2023-04-11 07:19:04.000000 ojtool-0.1.1/src/ojtool/utils.py
+drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-11 07:20:01.418065 ojtool-0.1.1/src/ojtool.egg-info/
+-rw-r--r--   0 jihongwang   (501) staff       (20)      573 2023-04-11 07:20:01.000000 ojtool-0.1.1/src/ojtool.egg-info/PKG-INFO
+-rw-r--r--   0 jihongwang   (501) staff       (20)      241 2023-04-11 07:20:01.000000 ojtool-0.1.1/src/ojtool.egg-info/SOURCES.txt
+-rw-r--r--   0 jihongwang   (501) staff       (20)        1 2023-04-11 07:20:01.000000 ojtool-0.1.1/src/ojtool.egg-info/dependency_links.txt
+-rw-r--r--   0 jihongwang   (501) staff       (20)        7 2023-04-11 07:20:01.000000 ojtool-0.1.1/src/ojtool.egg-info/top_level.txt
```

### Comparing `ojtool-0.1.0/LICENSE` & `ojtool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ojtool-0.1.0/PKG-INFO` & `ojtool-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ojtool
-Version: 0.1.0
+Version: 0.1.1
 Summary: Online Judge Test Data Generator.
 Home-page: https://github.com/ElementCraft/python-ojtool
 Author: elecraft
 Author-email: elecraft@outlook.com
 Project-URL: Bug Tracker, https://github.com/ElementCraft/python-ojtool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ojtool-0.1.0/setup.py` & `ojtool-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ojtool",
-    version="0.1.0",
+    version="0.1.1",
     author="elecraft",
     author_email="elecraft@outlook.com",
     description="Online Judge Test Data Generator.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ElementCraft/python-ojtool",
     project_urls={
```

### Comparing `ojtool-0.1.0/src/ojtool/ojtool.py` & `ojtool-0.1.1/src/ojtool/ojtool.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         foutpath = os.path.join(self.save_path,foutname)
 
         if platform.system() == "Windows":
             ret = subprocess.run([self.std, "<", finpath, ">", foutpath], shell=True)
             if ret.returncode != 0:
                 if self.debug: print(ret)
         else:
-            os.system(f"{self.std} < {finpath} > {foutpath}")
+            os.system(f"\"{self.std}\" < \"{finpath}\" > \"{foutpath}\"")
         self.FILES.append(finpath)
         self.FILES.append(foutpath)
         
     def done(self, o, zip=False):
         '''
         开始根据配置生成数据，需传入一个对象实例。
         '''
```

### Comparing `ojtool-0.1.0/src/ojtool.egg-info/PKG-INFO` & `ojtool-0.1.1/src/ojtool.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ojtool
-Version: 0.1.0
+Version: 0.1.1
 Summary: Online Judge Test Data Generator.
 Home-page: https://github.com/ElementCraft/python-ojtool
 Author: elecraft
 Author-email: elecraft@outlook.com
 Project-URL: Bug Tracker, https://github.com/ElementCraft/python-ojtool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

