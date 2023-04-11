# Comparing `tmp/dcb_admin_page_generator-0.0.4.tar.gz` & `tmp/dcb_admin_page_generator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcb_admin_page_generator-0.0.4.tar", last modified: Tue Apr 11 07:49:20 2023, max compression
+gzip compressed data, was "dcb_admin_page_generator-0.0.5.tar", last modified: Tue Apr 11 09:12:32 2023, max compression
```

## Comparing `dcb_admin_page_generator-0.0.4.tar` & `dcb_admin_page_generator-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:49:20.448842 dcb_admin_page_generator-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-03-29 08:48:00.000000 dcb_admin_page_generator-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      664 2023-04-11 07:49:20.448842 dcb_admin_page_generator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-11 07:24:11.000000 dcb_admin_page_generator-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:49:20.436895 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/
--rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/__init__.py
--rw-rw-rw-   0        0        0     2781 2023-04-11 07:36:42.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/main.py
--rw-rw-rw-   0        0        0    10002 2023-04-11 07:16:02.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/page_class.py
--rw-rw-rw-   0        0        0     4213 2023-04-11 07:16:42.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/res_text.vue
-drwxrwxrwx   0        0        0        0 2023-04-11 07:49:20.447845 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:48:27.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-11 07:12:32.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/add_or_edit.vue
--rw-rw-rw-   0        0        0     2258 2023-04-11 07:11:16.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/dialog_add_or_edit.vue
--rw-rw-rw-   0        0        0     2762 2023-04-11 07:10:16.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/dialog_list.vue
--rw-rw-rw-   0        0        0     5529 2023-04-06 07:21:58.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/index.vue
-drwxrwxrwx   0        0        0        0 2023-04-11 07:49:20.441861 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator.egg-info/
--rw-rw-rw-   0        0        0      664 2023-04-11 07:49:20.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-04-11 07:49:20.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:49:20.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-11 07:49:20.000000 dcb_admin_page_generator-0.0.4/dcb_admin_page_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 07:49:20.449858 dcb_admin_page_generator-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      668 2023-04-11 07:49:19.000000 dcb_admin_page_generator-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:12:32.056390 dcb_admin_page_generator-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-03-29 08:48:00.000000 dcb_admin_page_generator-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      664 2023-04-11 09:12:32.055393 dcb_admin_page_generator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-11 07:24:11.000000 dcb_admin_page_generator-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 09:12:32.036443 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/
+-rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/__init__.py
+-rw-rw-rw-   0        0        0     2781 2023-04-11 08:44:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/main.py
+-rw-rw-rw-   0        0        0    10139 2023-04-11 08:45:36.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/page_class.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:12:32.054394 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:48:27.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-11 07:12:32.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/add_or_edit.vue
+-rw-rw-rw-   0        0        0     2258 2023-04-11 07:11:16.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/dialog_add_or_edit.vue
+-rw-rw-rw-   0        0        0     2762 2023-04-11 07:10:16.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/dialog_list.vue
+-rw-rw-rw-   0        0        0     5529 2023-04-06 07:21:58.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/index.vue
+drwxrwxrwx   0        0        0        0 2023-04-11 09:12:32.041429 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-04-11 09:12:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2023-04-11 09:12:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:12:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-11 09:12:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:12:32.056390 dcb_admin_page_generator-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-04-11 09:12:19.000000 dcb_admin_page_generator-0.0.5/setup.py
```

### Comparing `dcb_admin_page_generator-0.0.4/LICENSE` & `dcb_admin_page_generator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.4/PKG-INFO` & `dcb_admin_page_generator-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcb_admin_page_generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: wyz
 Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/main.py` & `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/main.py`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/page_class.py` & `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/page_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import time
 import requests
 import re
+import os
+import sys
+here = os.path.dirname(os.path.abspath(__file__))
 
 
 def deal_p(data, p_type, need_req=False):
     resp = []
     for ele in data:
         if data[ele]['type'] != 'object' and data[ele]['type'] != 'array' and ele != 'pageIndex' and ele != 'pageSize':
             temp_dict = []
@@ -150,28 +153,30 @@
             return {"id": api_id, "token": token}
     else:
         return False
 
 
 def read_template(file_type):
     # print(os.listdir())
+    print(sys.path)
+
     if file_type == 'list':
-        with open('template/index.vue', encoding='utf8') as f:
+        with open(f'{here}\\template\\index.vue', encoding='utf8') as f:
             text = f.read()
         return text
     elif file_type == 'add':
-        with open('template/add_or_edit.vue', encoding='utf8') as f:
+        with open(f'{here}\\template\\add_or_edit.vue', encoding='utf8') as f:
             text = f.read()
         return text
     elif file_type == 'dialog_add':
-        with open('template/dialog_add_or_edit.vue', encoding='utf8') as f:
+        with open(f'{here}\\template\\dialog_add_or_edit.vue', encoding='utf8') as f:
             text = f.read()
         return text
     elif file_type == 'dialog_list':
-        with open('template/dialog_list.vue', encoding='utf8') as f:
+        with open(f'{here}\\template\\dialog_list.vue', encoding='utf8') as f:
             text = f.read()
         return text
     else:
         return ''
 
 
 class GenerateList(object):
```

### Comparing `dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/add_or_edit.vue` & `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/add_or_edit.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/dialog_add_or_edit.vue` & `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/dialog_add_or_edit.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/dialog_list.vue` & `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/dialog_list.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.4/dcb_admin_page_generator/template/index.vue` & `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/index.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.4/dcb_admin_page_generator.egg-info/PKG-INFO` & `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcb-admin-page-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: wyz
 Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcb_admin_page_generator-0.0.4/dcb_admin_page_generator.egg-info/SOURCES.txt` & `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.py
 dcb_admin_page_generator/__init__.py
 dcb_admin_page_generator/main.py
 dcb_admin_page_generator/page_class.py
-dcb_admin_page_generator/res_text.vue
 dcb_admin_page_generator.egg-info/PKG-INFO
 dcb_admin_page_generator.egg-info/SOURCES.txt
 dcb_admin_page_generator.egg-info/dependency_links.txt
 dcb_admin_page_generator.egg-info/top_level.txt
 dcb_admin_page_generator/template/__init__.py
 dcb_admin_page_generator/template/add_or_edit.vue
 dcb_admin_page_generator/template/dialog_add_or_edit.vue
```

### Comparing `dcb_admin_page_generator-0.0.4/setup.py` & `dcb_admin_page_generator-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dcb_admin_page_generator",
-    version="0.0.4",
+    version="0.0.5",
     author="wyz",
     author_email="846630116@qq.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=['ceshi']),
     package_data={'': ['*.vue']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

