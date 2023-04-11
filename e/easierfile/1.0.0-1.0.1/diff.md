# Comparing `tmp/easierfile-1.0.0.tar.gz` & `tmp/easierfile-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierfile-1.0.0.tar", max compression
+gzip compressed data, was "easierfile-1.0.1.tar", max compression
```

## Comparing `easierfile-1.0.0.tar` & `easierfile-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       32 2023-04-10 13:57:24.548112 easierfile-1.0.0/easierfile/__init__.py
--rw-r--r--   0        0        0     1171 2023-04-11 00:49:33.469281 easierfile-1.0.0/easierfile/file.py
--rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-1.0.0/LICENSE
--rw-r--r--   0        0        0      556 2023-04-11 01:28:34.500484 easierfile-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      934 2023-04-11 01:32:23.623996 easierfile-1.0.0/README.md
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 easierfile-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-04-10 13:57:24.548112 easierfile-1.0.1/easierfile/__init__.py
+-rw-r--r--   0        0        0     1171 2023-04-11 04:45:40.722039 easierfile-1.0.1/easierfile/file.py
+-rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-1.0.1/LICENSE
+-rw-r--r--   0        0        0      556 2023-04-11 05:01:13.479904 easierfile-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      934 2023-04-11 01:32:23.623996 easierfile-1.0.1/README.md
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 easierfile-1.0.1/PKG-INFO
```

### Comparing `easierfile-1.0.0/easierfile/file.py` & `easierfile-1.0.1/easierfile/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     @property
     def content(self):
         self.__m_file = open(self.__m_filePath, "r")
         self.__m_content = self.__m_file.read()
         self.__m_file.close()
         return self.__m_content
 
-    def ReWrite(self,content):
+    def Rewrite(self,content):
         self.__m_file = open(self.__m_filePath, "w")
         self.__m_file.write(content)
         self.__m_file.close()
 
     def Append(self,content):
         self.__m_file = open(self.__m_filePath, "a")
         self.__m_file.write(content)
```

### Comparing `easierfile-1.0.0/LICENSE` & `easierfile-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easierfile-1.0.0/pyproject.toml` & `easierfile-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easierfile"
-version = "1.0.0"
+version = "1.0.1"
 description = "A simple Python package that object-oriented encapsulates Python traditional built-in file operations."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-Easierfile"
 classifiers = [
     "Development Status :: 3 - Alpha"
```

### Comparing `easierfile-1.0.0/README.md` & `easierfile-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `easierfile-1.0.0/PKG-INFO` & `easierfile-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierfile
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple Python package that object-oriented encapsulates Python traditional built-in file operations.
 Home-page: https://github.com/leoweyr/Python-Easierfile
 License: MIT
 Author: leoweyr
 Author-email: leoweyr@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

