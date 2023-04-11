# Comparing `tmp/auto_pypi_uploader-1.1.1.tar.gz` & `tmp/auto_pypi_uploader-1.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_pypi_uploader-1.1.1.tar", last modified: Tue Apr 11 12:02:18 2023, max compression
+gzip compressed data, was "auto_pypi_uploader-1.1.1.1.tar", last modified: Tue Apr 11 12:04:01 2023, max compression
```

## Comparing `auto_pypi_uploader-1.1.1.tar` & `auto_pypi_uploader-1.1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:02:18.390148 auto_pypi_uploader-1.1.1/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 auto_pypi_uploader-1.1.1/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    13740 2023-04-11 12:02:18.389975 auto_pypi_uploader-1.1.1/PKG-INFO
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:02:18.389038 auto_pypi_uploader-1.1.1/auto_pypi_uploader/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 10:25:11.000000 auto_pypi_uploader-1.1.1/auto_pypi_uploader/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)     6852 2023-04-11 11:59:51.000000 auto_pypi_uploader-1.1.1/auto_pypi_uploader/pypi_uploader.py
--rw-r--r--   0 Huck       (503) staff       (20)    11928 2023-04-11 10:41:50.000000 auto_pypi_uploader-1.1.1/auto_pypi_uploader/setup_file_creator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:02:18.389786 auto_pypi_uploader-1.1.1/auto_pypi_uploader.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    13740 2023-04-11 12:02:18.000000 auto_pypi_uploader-1.1.1/auto_pypi_uploader.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      333 2023-04-11 12:02:18.000000 auto_pypi_uploader-1.1.1/auto_pypi_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-11 12:02:18.000000 auto_pypi_uploader-1.1.1/auto_pypi_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       37 2023-04-11 12:02:18.000000 auto_pypi_uploader-1.1.1/auto_pypi_uploader.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       19 2023-04-11 12:02:18.000000 auto_pypi_uploader-1.1.1/auto_pypi_uploader.egg-info/top_level.txt
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-11 12:02:18.390190 auto_pypi_uploader-1.1.1/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)     1415 2023-04-11 12:02:18.000000 auto_pypi_uploader-1.1.1/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:04:01.991454 auto_pypi_uploader-1.1.1.1/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 auto_pypi_uploader-1.1.1.1/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    13742 2023-04-11 12:04:01.991288 auto_pypi_uploader-1.1.1.1/PKG-INFO
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:04:01.990405 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 10:25:11.000000 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)     6852 2023-04-11 12:03:27.000000 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader/pypi_uploader.py
+-rw-r--r--   0 Huck       (503) staff       (20)    11928 2023-04-11 10:41:50.000000 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader/setup_file_creator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:04:01.991096 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    13742 2023-04-11 12:04:01.000000 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      333 2023-04-11 12:04:01.000000 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-11 12:04:01.000000 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       37 2023-04-11 12:04:01.000000 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       19 2023-04-11 12:04:01.000000 auto_pypi_uploader-1.1.1.1/auto_pypi_uploader.egg-info/top_level.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-11 12:04:01.991494 auto_pypi_uploader-1.1.1.1/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)     1417 2023-04-11 12:04:01.000000 auto_pypi_uploader-1.1.1.1/setup.py
```

### Comparing `auto_pypi_uploader-1.1.1/LICENSE` & `auto_pypi_uploader-1.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_pypi_uploader-1.1.1/PKG-INFO` & `auto_pypi_uploader-1.1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_pypi_uploader
-Version: 1.1.1
+Version: 1.1.1.1
 Summary: A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.
 Home-page: https://github.com/Huckdirks/auto-pypi-exporter
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 License: MIT
 Keywords: PyPi,Pip,setup,setup.py,automation
 Classifier: Programming Language :: Python
```

### Comparing `auto_pypi_uploader-1.1.1/auto_pypi_uploader/pypi_uploader.py` & `auto_pypi_uploader-1.1.1.1/auto_pypi_uploader/pypi_uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,13 +113,13 @@
         rmtree("dist")
     if isdir ("build"):
         rmtree("build")
     if isdir (f"{package_name}.egg-info"):
         rmtree(f"{package_name}.egg-info")
 
     print("\nWaiting a sec before downloading so PyPi can update the package\n")
-    sleep(30)
+    sleep(60)
     system(f"pip install --upgrade {package_name}")
     
 
 if __name__ == "__main__":
     pypi_upload()
```

### Comparing `auto_pypi_uploader-1.1.1/auto_pypi_uploader/setup_file_creator.py` & `auto_pypi_uploader-1.1.1.1/auto_pypi_uploader/setup_file_creator.py`

 * *Files identical despite different names*

### Comparing `auto_pypi_uploader-1.1.1/auto_pypi_uploader.egg-info/PKG-INFO` & `auto_pypi_uploader-1.1.1.1/auto_pypi_uploader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-pypi-uploader
-Version: 1.1.1
+Version: 1.1.1.1
 Summary: A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.
 Home-page: https://github.com/Huckdirks/auto-pypi-exporter
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 License: MIT
 Keywords: PyPi,Pip,setup,setup.py,automation
 Classifier: Programming Language :: Python
```

### Comparing `auto_pypi_uploader-1.1.1/setup.py` & `auto_pypi_uploader-1.1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Set the long description if the README file exists
 if readme_exists:
     with open(README_PATH, "r") as file:
         long_description = file.read()
 
 setup(
     name = "auto_pypi_uploader",
-	version = "1.1.1",
+	version = "1.1.1.1",
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     license = "MIT",
     url = "https://github.com/Huckdirks/auto-pypi-exporter",
```

