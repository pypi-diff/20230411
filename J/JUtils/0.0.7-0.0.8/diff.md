# Comparing `tmp/JUtils-0.0.7.tar.gz` & `tmp/JUtils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JUtils-0.0.7.tar", last modified: Fri Jan  6 11:38:41 2023, max compression
+gzip compressed data, was "JUtils-0.0.8.tar", last modified: Mon Apr 10 22:29:03 2023, max compression
```

## Comparing `JUtils-0.0.7.tar` & `JUtils-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-06 11:38:41.172314 JUtils-0.0.7/
--rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     8815 2023-01-06 11:38:41.172314 JUtils-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8369 2023-01-06 11:38:01.000000 JUtils-0.0.7/README.md
--rw-rw-rw-   0        0        0      522 2023-01-06 11:38:07.000000 JUtils-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-06 11:38:41.172314 JUtils-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-06 11:38:41.150988 JUtils-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-01-06 11:38:41.160276 JUtils-0.0.7/src/JUtils/
--rw-rw-rw-   0        0        0     1336 2023-01-06 11:03:26.000000 JUtils-0.0.7/src/JUtils/JArr.py
--rw-rw-rw-   0        0        0     8605 2023-01-06 11:03:27.000000 JUtils-0.0.7/src/JUtils/JColors.py
--rw-rw-rw-   0        0        0     2788 2023-01-06 11:03:27.000000 JUtils-0.0.7/src/JUtils/JConv.py
--rw-rw-rw-   0        0        0      785 2023-01-06 11:29:00.000000 JUtils-0.0.7/src/JUtils/JNum.py
--rw-rw-rw-   0        0        0      290 2023-01-06 11:03:28.000000 JUtils-0.0.7/src/JUtils/JOut.py
--rw-rw-rw-   0        0        0     1175 2023-01-06 11:14:24.000000 JUtils-0.0.7/src/JUtils/JStr.py
--rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-0.0.7/src/JUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-06 11:38:41.170794 JUtils-0.0.7/src/JUtils.egg-info/
--rw-rw-rw-   0        0        0     8815 2023-01-06 11:38:41.000000 JUtils-0.0.7/src/JUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-01-06 11:38:41.000000 JUtils-0.0.7/src/JUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-06 11:38:41.000000 JUtils-0.0.7/src/JUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-06 11:38:41.000000 JUtils-0.0.7/src/JUtils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 22:29:03.823045 JUtils-0.0.8/
+-rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     8815 2023-04-10 22:29:03.823045 JUtils-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8369 2023-01-06 11:38:01.000000 JUtils-0.0.8/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-10 22:22:08.000000 JUtils-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:29:03.823045 JUtils-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 22:29:03.770974 JUtils-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 22:29:03.807173 JUtils-0.0.8/src/JUtils/
+-rw-rw-rw-   0        0        0     1336 2023-01-06 11:03:26.000000 JUtils-0.0.8/src/JUtils/JArr.py
+-rw-rw-rw-   0        0        0     8605 2023-01-06 11:03:27.000000 JUtils-0.0.8/src/JUtils/JColors.py
+-rw-rw-rw-   0        0        0      105 2023-01-09 17:49:41.000000 JUtils-0.0.8/src/JUtils/JConst.py
+-rw-rw-rw-   0        0        0     3302 2023-04-10 21:34:08.000000 JUtils-0.0.8/src/JUtils/JConv.py
+-rw-rw-rw-   0        0        0     1148 2023-04-10 22:10:19.000000 JUtils-0.0.8/src/JUtils/JNum.py
+-rw-rw-rw-   0        0        0      645 2023-04-10 21:58:23.000000 JUtils-0.0.8/src/JUtils/JOut.py
+-rw-rw-rw-   0        0        0     2123 2023-04-10 22:21:29.000000 JUtils-0.0.8/src/JUtils/JStr.py
+-rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-0.0.8/src/JUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:29:03.820987 JUtils-0.0.8/src/JUtils.egg-info/
+-rw-rw-rw-   0        0        0     8815 2023-04-10 22:29:03.000000 JUtils-0.0.8/src/JUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-04-10 22:29:03.000000 JUtils-0.0.8/src/JUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:29:03.000000 JUtils-0.0.8/src/JUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 22:29:03.000000 JUtils-0.0.8/src/JUtils.egg-info/top_level.txt
```

### Comparing `JUtils-0.0.7/LICENSE` & `JUtils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.7/PKG-INFO` & `JUtils-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JUtils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package containing various utility functions i needed now and then, that i wanted to share
 Author-email: Jan Seifert <jan@seifert-online.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `JUtils-0.0.7/README.md` & `JUtils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.7/pyproject.toml` & `JUtils-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "JUtils"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Jan Seifert", email="jan@seifert-online.de" },
 ]
 description = "Package containing various utility functions i needed now and then, that i wanted to share"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `JUtils-0.0.7/src/JUtils/JArr.py` & `JUtils-0.0.8/src/JUtils/JArr.py`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.7/src/JUtils/JColors.py` & `JUtils-0.0.8/src/JUtils/JColors.py`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.7/src/JUtils/JConv.py` & `JUtils-0.0.8/src/JUtils/JConv.py`

 * *Files 21% similar despite different names*

```diff
@@ -92,8 +92,21 @@
         y (float): The y-coordinate.
 
     Returns:
         tuple: Polar coordinates (th, r), where r is the distance fromthe origin and th is the angle in degrees.
     '''
     r = sqrt(x*x + y*y)
     th = rad2deg(atan2(y, x))
-    return (th, r)
+    return (th, r)
+
+def rgb2gray(rgb: tuple) -> int:
+    """
+    Converts an RGB color tuple to a grayscale integer value using the luminosity method.
+    
+    Args:
+        rgb (tuple): A tuple containing 3 integers representing the RGB color values. The values
+                     should be in the range of 0-255, inclusive.
+                     
+    Returns:
+        int: The grayscale integer value representing the given RGB color tuple.
+    """
+    return int(0.299*rgb[0]//1 + 0.587*rgb[1]//1 + 0.114*rgb[2]//1)
```

### Comparing `JUtils-0.0.7/src/JUtils/JStr.py` & `JUtils-0.0.8/src/JUtils/JStr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #Functions for string analysing and modification
 
-nl = '\n' #newline constant to keep code clean
+from os import listdir
+
+NL = '\n' #newline constant to keep code clean
 
 def locBrac(string: str, brac: str, ix: int) -> int:
     '''
     Finds the index of the closing bracket that matches the opening bracket at the given index in the given string.
 
     Parameters:
         string (str): The input string.
@@ -31,8 +33,35 @@
     for i, ch in enumerate(string):
         if ch == brac:
             st.append(i)
         elif ch == fil[brac]:
             st.pop()
         if st == [] and i >= ix:
             return i
-    return -1
+    return -1
+
+def multiCenter(s: str, l: int) -> str:
+    """
+    Centers the text in a string by padding spaces on either side of each line.
+    
+    Args:
+        s (str): The input string to center.
+        l (int): The desired width of the centered string.
+        
+    Returns:
+        str: The centered string. Each line is padded with spaces on either side to center the text. If
+             a line already has an odd number of characters, the extra space is added to the right
+             side of the line.
+    """
+    return "\n".join([" "*((l-len(x))//2) + x + " "*((l-len(x))//2) for x in s.split("\n")])
+
+def listPath(d: str) -> list[str]:
+    """
+    Just like os.listdir(), but with appended path.
+    
+    Args:
+        d: The path to list.
+        
+    Returns:
+        list: A list of paths of files and directories in the given path.
+    """
+    return [d + "\\" + x for x in listdir(d)]
```

### Comparing `JUtils-0.0.7/src/JUtils.egg-info/PKG-INFO` & `JUtils-0.0.8/src/JUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JUtils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package containing various utility functions i needed now and then, that i wanted to share
 Author-email: Jan Seifert <jan@seifert-online.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

