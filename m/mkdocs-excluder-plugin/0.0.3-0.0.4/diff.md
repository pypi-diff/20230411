# Comparing `tmp/mkdocs-excluder-plugin-0.0.3.tar.gz` & `tmp/mkdocs-excluder-plugin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-excluder-plugin-0.0.3.tar", last modified: Tue Apr  4 12:47:52 2023, max compression
+gzip compressed data, was "mkdocs-excluder-plugin-0.0.4.tar", last modified: Tue Apr 11 13:15:50 2023, max compression
```

## Comparing `mkdocs-excluder-plugin-0.0.3.tar` & `mkdocs-excluder-plugin-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 12:47:52.780291 mkdocs-excluder-plugin-0.0.3/
--rw-rw-rw-   0        0        0    11562 2023-04-04 11:40:10.000000 mkdocs-excluder-plugin-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       31 2023-04-04 11:33:42.000000 mkdocs-excluder-plugin-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1802 2023-04-04 12:47:52.779289 mkdocs-excluder-plugin-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1479 2023-04-04 12:13:27.000000 mkdocs-excluder-plugin-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 12:47:52.770775 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder/
--rw-rw-rw-   0        0        0       75 2023-04-04 11:43:42.000000 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder/__init__.py
--rw-rw-rw-   0        0        0     4008 2023-04-04 11:43:42.000000 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder/plugin.py
-drwxrwxrwx   0        0        0        0 2023-04-04 12:47:52.778289 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder_plugin.egg-info/
--rw-rw-rw-   0        0        0     1802 2023-04-04 12:47:52.000000 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-04-04 12:47:52.000000 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 12:47:52.000000 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-04 12:47:52.000000 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-04 12:47:52.000000 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-04 12:47:52.000000 mkdocs-excluder-plugin-0.0.3/mkdocs_excluder_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 12:47:52.780291 mkdocs-excluder-plugin-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-04-04 12:44:43.000000 mkdocs-excluder-plugin-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:15:50.930137 mkdocs-excluder-plugin-0.0.4/
+-rw-rw-rw-   0        0        0    11560 2023-04-11 13:08:59.000000 mkdocs-excluder-plugin-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-04-11 13:08:59.000000 mkdocs-excluder-plugin-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1802 2023-04-11 13:15:50.930137 mkdocs-excluder-plugin-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1479 2023-04-11 13:08:59.000000 mkdocs-excluder-plugin-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 13:15:50.920368 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder/
+-rw-rw-rw-   0        0        0      116 2023-04-11 13:08:59.000000 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder/__init__.py
+-rw-rw-rw-   0        0        0     4049 2023-04-11 13:08:59.000000 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder/plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:15:50.929130 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder_plugin.egg-info/
+-rw-rw-rw-   0        0        0     1802 2023-04-11 13:15:50.000000 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-04-11 13:15:50.000000 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:15:50.000000 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-11 13:15:50.000000 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 13:15:50.000000 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 13:15:50.000000 mkdocs-excluder-plugin-0.0.4/mkdocs_excluder_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 13:15:50.930137 mkdocs-excluder-plugin-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-04-11 13:13:44.000000 mkdocs-excluder-plugin-0.0.4/setup.py
```

### Comparing `mkdocs-excluder-plugin-0.0.3/LICENSE` & `mkdocs-excluder-plugin-0.0.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [2023] [Avery Pennarun, polygoniq]
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `mkdocs-excluder-plugin-0.0.3/PKG-INFO` & `mkdocs-excluder-plugin-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-excluder-plugin
-Version: 0.0.3
+Version: 0.0.4
 Summary: A mkdocs plugin that lets you exclude files or trees and removes navigation entries.
 Author: polygoniq
 Author-email: zdeno@polygoniq.com
 License: Apache
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs-excluder-plugin-0.0.3/README.md` & `mkdocs-excluder-plugin-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-excluder-plugin-0.0.3/mkdocs_excluder/plugin.py` & `mkdocs-excluder-plugin-0.0.4/mkdocs_excluder/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # copyright (c) 2018- polygoniq xyz s.r.o.
+# copyright (c) 2019-2023 Avery Pennaru
 
 import fnmatch
 import re
 import os
 import mkdocs
 import mkdocs.plugins
 import mkdocs.structure.files
```

### Comparing `mkdocs-excluder-plugin-0.0.3/mkdocs_excluder_plugin.egg-info/PKG-INFO` & `mkdocs-excluder-plugin-0.0.4/mkdocs_excluder_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-excluder-plugin
-Version: 0.0.3
+Version: 0.0.4
 Summary: A mkdocs plugin that lets you exclude files or trees and removes navigation entries.
 Author: polygoniq
 Author-email: zdeno@polygoniq.com
 License: Apache
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs-excluder-plugin-0.0.3/setup.py` & `mkdocs-excluder-plugin-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # copyright (c) 2018- polygoniq xyz s.r.o.
+# copyright (c) 2019-2023 Avery Pennaru
 
 import os.path
 import setuptools
 
 
 def read(name: str):
     mydir = os.path.abspath(os.path.dirname(__file__))
     return open(os.path.join(mydir, name)).read()
 
 
 setuptools.setup(
     name='mkdocs-excluder-plugin',
-    version='0.0.3',
+    version='0.0.4',
     packages=['mkdocs_excluder'],
     license='Apache',
     author='polygoniq',
     author_email='zdeno@polygoniq.com',
     description='A mkdocs plugin that lets you exclude files or trees and removes navigation entries.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
```

