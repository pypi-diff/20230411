# Comparing `tmp/auto_pypi_uploader-1.1.1.2.tar.gz` & `tmp/auto_pypi_uploader-1.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_pypi_uploader-1.1.1.2.tar", last modified: Tue Apr 11 12:25:01 2023, max compression
+gzip compressed data, was "auto_pypi_uploader-1.1.1.3.tar", last modified: Tue Apr 11 12:27:38 2023, max compression
```

## Comparing `auto_pypi_uploader-1.1.1.2.tar` & `auto_pypi_uploader-1.1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:25:01.178146 auto_pypi_uploader-1.1.1.2/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 auto_pypi_uploader-1.1.1.2/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    13742 2023-04-11 12:25:01.177914 auto_pypi_uploader-1.1.1.2/PKG-INFO
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:25:01.177114 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 10:25:11.000000 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)     7455 2023-04-11 12:23:32.000000 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader/pypi_uploader.py
--rw-r--r--   0 Huck       (503) staff       (20)    11928 2023-04-11 10:41:50.000000 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader/setup_file_creator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:25:01.177710 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    13742 2023-04-11 12:25:01.000000 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      333 2023-04-11 12:25:01.000000 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-11 12:25:01.000000 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       37 2023-04-11 12:25:01.000000 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       19 2023-04-11 12:25:01.000000 auto_pypi_uploader-1.1.1.2/auto_pypi_uploader.egg-info/top_level.txt
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-11 12:25:01.178190 auto_pypi_uploader-1.1.1.2/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)     1417 2023-04-11 12:25:00.000000 auto_pypi_uploader-1.1.1.2/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:27:38.109769 auto_pypi_uploader-1.1.1.3/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 auto_pypi_uploader-1.1.1.3/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    13742 2023-04-11 12:27:38.109597 auto_pypi_uploader-1.1.1.3/PKG-INFO
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:27:38.108842 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 10:25:11.000000 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)     7455 2023-04-11 12:27:00.000000 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader/pypi_uploader.py
+-rw-r--r--   0 Huck       (503) staff       (20)    11928 2023-04-11 10:41:50.000000 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader/setup_file_creator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 12:27:38.109413 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    13742 2023-04-11 12:27:38.000000 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      333 2023-04-11 12:27:38.000000 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-11 12:27:38.000000 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       37 2023-04-11 12:27:38.000000 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       19 2023-04-11 12:27:38.000000 auto_pypi_uploader-1.1.1.3/auto_pypi_uploader.egg-info/top_level.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-11 12:27:38.109815 auto_pypi_uploader-1.1.1.3/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)     1417 2023-04-11 12:27:37.000000 auto_pypi_uploader-1.1.1.3/setup.py
```

### Comparing `auto_pypi_uploader-1.1.1.2/LICENSE` & `auto_pypi_uploader-1.1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_pypi_uploader-1.1.1.2/PKG-INFO` & `auto_pypi_uploader-1.1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_pypi_uploader
-Version: 1.1.1.2
+Version: 1.1.1.3
 Summary: A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.
 Home-page: https://github.com/Huckdirks/auto-pypi-exporter
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 License: MIT
 Keywords: PyPi,Pip,setup,setup.py,automation
 Classifier: Programming Language :: Python
```

### Comparing `auto_pypi_uploader-1.1.1.2/auto_pypi_uploader/pypi_uploader.py` & `auto_pypi_uploader-1.1.1.3/auto_pypi_uploader/pypi_uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,13 +131,13 @@
             try:
                 rmtree(path)
             except OSError:
                 remove(path)
         rmdir(f"{package_name}.egg-info")
 
     print("\nWaiting a sec before downloading so PyPi can update the package\n")
-    sleep(60)
+    sleep(90)
     system(f"pip install --upgrade {package_name}")
     
 
 if __name__ == "__main__":
     pypi_upload()
```

### Comparing `auto_pypi_uploader-1.1.1.2/auto_pypi_uploader/setup_file_creator.py` & `auto_pypi_uploader-1.1.1.3/auto_pypi_uploader/setup_file_creator.py`

 * *Files identical despite different names*

### Comparing `auto_pypi_uploader-1.1.1.2/auto_pypi_uploader.egg-info/PKG-INFO` & `auto_pypi_uploader-1.1.1.3/auto_pypi_uploader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-pypi-uploader
-Version: 1.1.1.2
+Version: 1.1.1.3
 Summary: A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.
 Home-page: https://github.com/Huckdirks/auto-pypi-exporter
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 License: MIT
 Keywords: PyPi,Pip,setup,setup.py,automation
 Classifier: Programming Language :: Python
```

### Comparing `auto_pypi_uploader-1.1.1.2/setup.py` & `auto_pypi_uploader-1.1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Set the long description if the README file exists
 if readme_exists:
     with open(README_PATH, "r") as file:
         long_description = file.read()
 
 setup(
     name = "auto_pypi_uploader",
-	version = "1.1.1.2",
+	version = "1.1.1.3",
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     license = "MIT",
     url = "https://github.com/Huckdirks/auto-pypi-exporter",
```

