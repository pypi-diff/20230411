# Comparing `tmp/plhtools-1.1.8.tar.gz` & `tmp/plhtools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plhtools-1.1.8.tar", last modified: Thu Aug 11 11:35:51 2022, max compression
+gzip compressed data, was "dist/plhtools-1.1.9.tar", last modified: Thu Aug 11 12:26:39 2022, max compression
```

## Comparing `plhtools-1.1.8.tar` & `plhtools-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 penglinhan   (501) staff       (20)        0 2022-08-11 11:35:51.000000 plhtools-1.1.8/
--rw-r--r--   0 penglinhan   (501) staff       (20)     1068 2022-06-16 03:06:48.000000 plhtools-1.1.8/LICENSE.txt
--rw-r--r--   0 penglinhan   (501) staff       (20)      976 2022-08-11 11:35:51.000000 plhtools-1.1.8/PKG-INFO
--rw-r--r--   0 penglinhan   (501) staff       (20)      131 2022-08-01 08:09:34.000000 plhtools-1.1.8/README.rst
-drwxr-xr-x   0 penglinhan   (501) staff       (20)        0 2022-08-11 11:35:51.000000 plhtools-1.1.8/plhtools/
--rw-r--r--   0 penglinhan   (501) staff       (20)      655 2022-08-03 11:02:40.000000 plhtools-1.1.8/plhtools/__init__.py
--rw-r--r--   0 penglinhan   (501) staff       (20)     1413 2022-08-04 03:15:38.000000 plhtools-1.1.8/plhtools/configuration.py
--rw-r--r--   0 penglinhan   (501) staff       (20)     7713 2022-08-03 09:34:18.000000 plhtools-1.1.8/plhtools/encryption_and_decryption.py
--rw-r--r--   0 penglinhan   (501) staff       (20)     6632 2022-08-11 11:24:03.000000 plhtools-1.1.8/plhtools/es.py
--rw-r--r--   0 penglinhan   (501) staff       (20)     8548 2022-08-03 10:40:37.000000 plhtools-1.1.8/plhtools/mysql.py
-drwxr-xr-x   0 penglinhan   (501) staff       (20)        0 2022-08-11 11:35:51.000000 plhtools-1.1.8/plhtools.egg-info/
--rw-r--r--   0 penglinhan   (501) staff       (20)      976 2022-08-11 11:35:50.000000 plhtools-1.1.8/plhtools.egg-info/PKG-INFO
--rw-r--r--   0 penglinhan   (501) staff       (20)      308 2022-08-11 11:35:51.000000 plhtools-1.1.8/plhtools.egg-info/SOURCES.txt
--rw-r--r--   0 penglinhan   (501) staff       (20)        1 2022-08-11 11:35:50.000000 plhtools-1.1.8/plhtools.egg-info/dependency_links.txt
--rw-r--r--   0 penglinhan   (501) staff       (20)      126 2022-08-11 11:35:50.000000 plhtools-1.1.8/plhtools.egg-info/requires.txt
--rw-r--r--   0 penglinhan   (501) staff       (20)        9 2022-08-11 11:35:51.000000 plhtools-1.1.8/plhtools.egg-info/top_level.txt
--rw-r--r--   0 penglinhan   (501) staff       (20)       38 2022-08-11 11:35:51.000000 plhtools-1.1.8/setup.cfg
--rw-r--r--   0 penglinhan   (501) staff       (20)     1787 2022-08-11 11:24:03.000000 plhtools-1.1.8/setup.py
+drwxr-xr-x   0 penglinhan   (501) staff       (20)        0 2022-08-11 12:26:39.000000 plhtools-1.1.9/
+-rw-r--r--   0 penglinhan   (501) staff       (20)     1068 2022-06-16 03:06:48.000000 plhtools-1.1.9/LICENSE.txt
+-rw-r--r--   0 penglinhan   (501) staff       (20)      976 2022-08-11 12:26:39.000000 plhtools-1.1.9/PKG-INFO
+-rw-r--r--   0 penglinhan   (501) staff       (20)      131 2022-08-01 08:09:34.000000 plhtools-1.1.9/README.rst
+drwxr-xr-x   0 penglinhan   (501) staff       (20)        0 2022-08-11 12:26:39.000000 plhtools-1.1.9/plhtools/
+-rw-r--r--   0 penglinhan   (501) staff       (20)      655 2022-08-03 11:02:40.000000 plhtools-1.1.9/plhtools/__init__.py
+-rw-r--r--   0 penglinhan   (501) staff       (20)     1413 2022-08-04 03:15:38.000000 plhtools-1.1.9/plhtools/configuration.py
+-rw-r--r--   0 penglinhan   (501) staff       (20)     7713 2022-08-03 09:34:18.000000 plhtools-1.1.9/plhtools/encryption_and_decryption.py
+-rw-r--r--   0 penglinhan   (501) staff       (20)     6730 2022-08-11 12:26:34.000000 plhtools-1.1.9/plhtools/es.py
+-rw-r--r--   0 penglinhan   (501) staff       (20)     8548 2022-08-03 10:40:37.000000 plhtools-1.1.9/plhtools/mysql.py
+drwxr-xr-x   0 penglinhan   (501) staff       (20)        0 2022-08-11 12:26:39.000000 plhtools-1.1.9/plhtools.egg-info/
+-rw-r--r--   0 penglinhan   (501) staff       (20)      976 2022-08-11 12:26:38.000000 plhtools-1.1.9/plhtools.egg-info/PKG-INFO
+-rw-r--r--   0 penglinhan   (501) staff       (20)      308 2022-08-11 12:26:39.000000 plhtools-1.1.9/plhtools.egg-info/SOURCES.txt
+-rw-r--r--   0 penglinhan   (501) staff       (20)        1 2022-08-11 12:26:38.000000 plhtools-1.1.9/plhtools.egg-info/dependency_links.txt
+-rw-r--r--   0 penglinhan   (501) staff       (20)      126 2022-08-11 12:26:39.000000 plhtools-1.1.9/plhtools.egg-info/requires.txt
+-rw-r--r--   0 penglinhan   (501) staff       (20)        9 2022-08-11 12:26:39.000000 plhtools-1.1.9/plhtools.egg-info/top_level.txt
+-rw-r--r--   0 penglinhan   (501) staff       (20)       38 2022-08-11 12:26:39.000000 plhtools-1.1.9/setup.cfg
+-rw-r--r--   0 penglinhan   (501) staff       (20)     1787 2022-08-11 12:26:34.000000 plhtools-1.1.9/setup.py
```

### Comparing `plhtools-1.1.8/LICENSE.txt` & `plhtools-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plhtools-1.1.8/PKG-INFO` & `plhtools-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plhtools
-Version: 1.1.8
+Version: 1.1.9
 Summary: 彭麟汉的工具包
 Home-page: https://mp.weixin.qq.com/s/9FQ-Tun5FbpBepBAsdY62w
 Author: penglinhan
 Author-email: 2453995079@qq.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `plhtools-1.1.8/plhtools/__init__.py` & `plhtools-1.1.9/plhtools/__init__.py`

 * *Files identical despite different names*

### Comparing `plhtools-1.1.8/plhtools/configuration.py` & `plhtools-1.1.9/plhtools/configuration.py`

 * *Files identical despite different names*

### Comparing `plhtools-1.1.8/plhtools/encryption_and_decryption.py` & `plhtools-1.1.9/plhtools/encryption_and_decryption.py`

 * *Files identical despite different names*

### Comparing `plhtools-1.1.8/plhtools/es.py` & `plhtools-1.1.9/plhtools/es.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,17 @@
                 temp_dict = i['_source']
                 temp_dict['_id'] = i['_id']
                 temp_dict['_score'] = i['_score']
                 result_list.append(temp_dict)
             return result_list
         else:
             return '未查到'
+
+    def index_search(self,index_name,body):
+        self.conn.search(index=index_name,body=body)
     def index_search_all(self,index_name,pn=1,size=10000,doc_type=''):
         body = {
             "query": {
                 "match_all": {}
             },
             "from": (pn - 1) * size,
             "size": size,
```

### Comparing `plhtools-1.1.8/plhtools/mysql.py` & `plhtools-1.1.9/plhtools/mysql.py`

 * *Files identical despite different names*

### Comparing `plhtools-1.1.8/plhtools.egg-info/PKG-INFO` & `plhtools-1.1.9/plhtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plhtools
-Version: 1.1.8
+Version: 1.1.9
 Summary: 彭麟汉的工具包
 Home-page: https://mp.weixin.qq.com/s/9FQ-Tun5FbpBepBAsdY62w
 Author: penglinhan
 Author-email: 2453995079@qq.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `plhtools-1.1.8/setup.py` & `plhtools-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 setup(name='plhtools',  # 包名
-      version='1.1.8',  # 版本号
+      version='1.1.9',  # 版本号
       description='彭麟汉的工具包',
       long_description=long_description,
       author='penglinhan',
       author_email='2453995079@qq.com',
       url='https://mp.weixin.qq.com/s/9FQ-Tun5FbpBepBAsdY62w',
       install_requires=[
           'pycryptodome',
```

