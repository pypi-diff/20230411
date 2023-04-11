# Comparing `tmp/dcb_admin_page_generator-0.0.1.tar.gz` & `tmp/dcb_admin_page_generator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcb_admin_page_generator-0.0.1.tar", last modified: Thu Mar 30 02:08:41 2023, max compression
+gzip compressed data, was "dcb_admin_page_generator-0.0.2.tar", last modified: Tue Apr 11 07:21:05 2023, max compression
```

## Comparing `dcb_admin_page_generator-0.0.1.tar` & `dcb_admin_page_generator-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 02:08:41.559078 dcb_admin_page_generator-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-03-29 08:48:00.000000 dcb_admin_page_generator-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      608 2023-03-30 02:08:41.558081 dcb_admin_page_generator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-03-29 08:47:11.000000 dcb_admin_page_generator-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 02:08:41.552126 dcb_admin_page_generator-0.0.1/dcb_admin_page_generator/
--rw-rw-rw-   0        0        0       20 2023-03-29 08:48:00.000000 dcb_admin_page_generator-0.0.1/dcb_admin_page_generator/__init__.py
--rw-rw-rw-   0        0        0      901 2023-03-29 07:16:19.000000 dcb_admin_page_generator-0.0.1/dcb_admin_page_generator/main.py
-drwxrwxrwx   0        0        0        0 2023-03-30 02:08:41.557084 dcb_admin_page_generator-0.0.1/dcb_admin_page_generator.egg-info/
--rw-rw-rw-   0        0        0      608 2023-03-30 02:08:41.000000 dcb_admin_page_generator-0.0.1/dcb_admin_page_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-03-30 02:08:41.000000 dcb_admin_page_generator-0.0.1/dcb_admin_page_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 02:08:41.000000 dcb_admin_page_generator-0.0.1/dcb_admin_page_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-30 02:08:41.000000 dcb_admin_page_generator-0.0.1/dcb_admin_page_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 02:08:41.559078 dcb_admin_page_generator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-03-30 02:08:30.000000 dcb_admin_page_generator-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:21:05.044559 dcb_admin_page_generator-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-03-29 08:48:00.000000 dcb_admin_page_generator-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      595 2023-04-11 07:21:05.043561 dcb_admin_page_generator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-03-29 08:47:11.000000 dcb_admin_page_generator-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:21:05.039586 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/
+-rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/__init__.py
+-rw-rw-rw-   0        0        0     2780 2023-04-11 07:21:01.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/main.py
+-rw-rw-rw-   0        0        0    10002 2023-04-11 07:16:02.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator/page_class.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:21:05.042564 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/
+-rw-rw-rw-   0        0        0      595 2023-04-11 07:21:04.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-04-11 07:21:05.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:21:04.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-11 07:21:04.000000 dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:21:05.044559 dcb_admin_page_generator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      633 2023-04-11 07:18:53.000000 dcb_admin_page_generator-0.0.2/setup.py
```

### Comparing `dcb_admin_page_generator-0.0.1/LICENSE` & `dcb_admin_page_generator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.1/PKG-INFO` & `dcb_admin_page_generator-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dcb_admin_page_generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
-Author: Example Author
-Author-email: author@example.com
+Author: wyz
+Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example Package
```

### Comparing `dcb_admin_page_generator-0.0.1/dcb_admin_page_generator.egg-info/PKG-INFO` & `dcb_admin_page_generator-0.0.2/dcb_admin_page_generator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dcb-admin-page-generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
-Author: Example Author
-Author-email: author@example.com
+Author: wyz
+Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example Package
```

