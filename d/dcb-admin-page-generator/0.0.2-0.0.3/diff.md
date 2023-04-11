# Comparing `tmp/dcb_admin_page_generator-0.0.2.tar.gz` & `tmp/dcb_admin_page_generator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcb_admin_page_generator-0.0.2.tar", last modified: Tue Apr 11 07:21:05 2023, max compression
+gzip compressed data, was "dcb_admin_page_generator-0.0.3.tar", last modified: Tue Apr 11 07:44:45 2023, max compression
```

## Comparing `dcb_admin_page_generator-0.0.2.tar` & `dcb_admin_page_generator-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:21:05.044559 dcb_admin_page_generator-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-03-29 08:48:00.000000 dcb_admin_page_generator-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      595 2023-04-11 07:21:05.043561 dcb_admin_page_generator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-03-29 08:47:11.000000 dcb_admin_page_generator-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:21:05.039586 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/
--rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/__init__.py
--rw-rw-rw-   0        0        0     2780 2023-04-11 07:21:01.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/main.py
--rw-rw-rw-   0        0        0    10002 2023-04-11 07:16:02.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/page_class.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:21:05.042564 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/
--rw-rw-rw-   0        0        0      595 2023-04-11 07:21:04.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-04-11 07:21:05.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:21:04.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-11 07:21:04.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:21:05.044559 dcb_admin_page_generator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      633 2023-04-11 07:18:53.000000 dcb_admin_page_generator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:44:45.899589 dcb_admin_page_generator-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-03-29 08:48:00.000000 dcb_admin_page_generator-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      664 2023-04-11 07:44:45.898621 dcb_admin_page_generator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-11 07:24:11.000000 dcb_admin_page_generator-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:44:45.892635 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator/
+-rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator/__init__.py
+-rw-rw-rw-   0        0        0     2781 2023-04-11 07:36:42.000000 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator/main.py
+-rw-rw-rw-   0        0        0    10002 2023-04-11 07:16:02.000000 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator/page_class.py
+-rw-rw-rw-   0        0        0     4213 2023-04-11 07:16:42.000000 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator/res_text.vue
+drwxrwxrwx   0        0        0        0 2023-04-11 07:44:45.897618 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-04-11 07:44:45.000000 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-11 07:44:45.000000 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:44:45.000000 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-11 07:44:45.000000 dcb_admin_page_generator-0.0.3/dcb_admin_page_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:44:45.899589 dcb_admin_page_generator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-04-11 07:44:26.000000 dcb_admin_page_generator-0.0.3/setup.py
```

### Comparing `dcb_admin_page_generator-0.0.2/LICENSE` & `dcb_admin_page_generator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.2/PKG-INFO` & `dcb_admin_page_generator-0.0.3/dcb_admin_page_generator.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dcb_admin_page_generator
-Version: 0.0.2
+Name: dcb-admin-page-generator
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: wyz
 Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,9 @@
 # Example Package
 
 This is a simple example package. You can use
 
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 
 to write your content.
+1銆乸ython3 setup.py sdist bdist_wheel
+2銆乼wine upload dist/*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/main.py` & `dcb_admin_page_generator-0.0.3/dcb_admin_page_generator/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from page_class import *
+from .page_class import *
 
 
 def deal_yapi(configuration, file_path):
     print('file_path', file_path)
     yapi_url = input('请输入获取数据链接的YapiURL')
     id_dict = get_id(yapi_url, configuration)
     resp = requests.get(f'{configuration["serverUrl"]}{configuration["getInfoPath"]}', params=id_dict)
```

### Comparing `dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/page_class.py` & `dcb_admin_page_generator-0.0.3/dcb_admin_page_generator/page_class.py`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.2/setup.py` & `dcb_admin_page_generator-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dcb_admin_page_generator",
-    version="0.0.2",
+    version="0.0.3",
     author="wyz",
     author_email="846630116@qq.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
+    package_data={'': ['*.vue']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

