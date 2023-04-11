# Comparing `tmp/JablotronPy-0.4.2.tar.gz` & `tmp/JablotronPy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JablotronPy-0.4.2.tar", last modified: Mon Apr  3 21:50:41 2023, max compression
+gzip compressed data, was "JablotronPy-0.5.0.tar", last modified: Tue Apr 11 07:30:22 2023, max compression
```

## Comparing `JablotronPy-0.4.2.tar` & `JablotronPy-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:50:41.649718 JablotronPy-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:50:41.649718 JablotronPy-0.4.2/JablotronPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-03 21:50:41.000000 JablotronPy-0.4.2/JablotronPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-03 21:50:41.000000 JablotronPy-0.4.2/JablotronPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 21:50:41.000000 JablotronPy-0.4.2/JablotronPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-03 21:50:41.000000 JablotronPy-0.4.2/JablotronPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 21:50:41.000000 JablotronPy-0.4.2/JablotronPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-03 21:50:21.000000 JablotronPy-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-03 21:50:21.000000 JablotronPy-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-03 21:50:41.649718 JablotronPy-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-03 21:50:21.000000 JablotronPy-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:50:41.649718 JablotronPy-0.4.2/jablotronpy/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-03 21:50:21.000000 JablotronPy-0.4.2/jablotronpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-04-03 21:50:21.000000 JablotronPy-0.4.2/jablotronpy/jablotronpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 21:50:41.649718 JablotronPy-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-03 21:50:21.000000 JablotronPy-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:50:41.649718 JablotronPy-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-03 21:50:21.000000 JablotronPy-0.4.2/tests/test_jablotron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:22.725380 JablotronPy-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:22.725380 JablotronPy-0.5.0/JablotronPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-11 07:30:22.000000 JablotronPy-0.5.0/JablotronPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-11 07:30:22.000000 JablotronPy-0.5.0/JablotronPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:30:22.000000 JablotronPy-0.5.0/JablotronPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 07:30:22.000000 JablotronPy-0.5.0/JablotronPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 07:30:22.000000 JablotronPy-0.5.0/JablotronPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-11 07:30:02.000000 JablotronPy-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 07:30:02.000000 JablotronPy-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-11 07:30:22.725380 JablotronPy-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 07:30:02.000000 JablotronPy-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:22.725380 JablotronPy-0.5.0/jablotronpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-11 07:30:02.000000 JablotronPy-0.5.0/jablotronpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-11 07:30:02.000000 JablotronPy-0.5.0/jablotronpy/jablotronpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:30:22.725380 JablotronPy-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-11 07:30:02.000000 JablotronPy-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:22.725380 JablotronPy-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-11 07:30:02.000000 JablotronPy-0.5.0/tests/test_jablotron.py
```

### Comparing `JablotronPy-0.4.2/JablotronPy.egg-info/PKG-INFO` & `JablotronPy-0.5.0/JablotronPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JablotronPy
-Version: 0.4.2
+Version: 0.5.0
 Summary: A client to interact with the Jablotron API to control Jablotron alarm systems
 Home-page: https://github.com/fdegier/JablotronPy
 Author: F. de Gier
 Author-email: freddegier@me.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `JablotronPy-0.4.2/LICENSE` & `JablotronPy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JablotronPy-0.4.2/PKG-INFO` & `JablotronPy-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JablotronPy
-Version: 0.4.2
+Version: 0.5.0
 Summary: A client to interact with the Jablotron API to control Jablotron alarm systems
 Home-page: https://github.com/fdegier/JablotronPy
 Author: F. de Gier
 Author-email: freddegier@me.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `JablotronPy-0.4.2/README.md` & `JablotronPy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `JablotronPy-0.4.2/jablotronpy/jablotronpy.py` & `JablotronPy-0.5.0/jablotronpy/jablotronpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,20 @@
             json=payload
         )
 
         data = r.json()
         if r.ok:
             if end_point == "userAuthorize.json":
                 return True, r.cookies.get("PHPSESSID")
-            return True, data["data"]
+            if data.get('data') is not None:
+                return True, data["data"]
+            else:
+                print(f"Unexpected response from API:")
+                print(data)
+                return False, None
 
         if data.get('http-code', 0) == 401:
             self.set_cookies()
             if retry >= 3:
                 print(f"Exhausted all retry options, response:")
                 print(data.json())
                 if 'errors' in data:
```

### Comparing `JablotronPy-0.4.2/setup.py` & `JablotronPy-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="JablotronPy",
-    version="0.4.2",
+    version="0.5.0",
     author="F. de Gier",
     author_email="freddegier@me.com",
     description="A client to interact with the Jablotron API to control Jablotron alarm systems",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fdegier/JablotronPy",
     packages=["jablotronpy"],
```

### Comparing `JablotronPy-0.4.2/tests/test_jablotron.py` & `JablotronPy-0.5.0/tests/test_jablotron.py`

 * *Files identical despite different names*

