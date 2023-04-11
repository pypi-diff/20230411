# Comparing `tmp/creosote-2.6.0-py3-none-any.whl.zip` & `tmp/creosote-2.6.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14113 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 creosote/__about__.py
+Zip file size: 14152 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       25 b- defN 20-Feb-02 00:00 creosote/__about__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 creosote/__init__.py
 -rw-r--r--  2.0 unx     6597 b- defN 20-Feb-02 00:00 creosote/cli.py
 -rw-r--r--  2.0 unx     1109 b- defN 20-Feb-02 00:00 creosote/formatters.py
 -rw-r--r--  2.0 unx      523 b- defN 20-Feb-02 00:00 creosote/models.py
 -rw-r--r--  2.0 unx     8558 b- defN 20-Feb-02 00:00 creosote/parsers.py
 -rw-r--r--  2.0 unx     9413 b- defN 20-Feb-02 00:00 creosote/resolvers.py
-?rw-r--r--  2.0 unx    13013 b- defN 20-Feb-02 00:00 creosote-2.6.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      933 b- defN 20-Feb-02 00:00 creosote-2.6.0.dist-info/RECORD
-12 files, 41374 bytes uncompressed, 12555 bytes compressed:  69.7%
+?rw-r--r--  2.0 unx    13016 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      948 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/RECORD
+12 files, 41395 bytes uncompressed, 12564 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: creosote/parsers.py
 Comment: 
 
 Filename: creosote/resolvers.py
 Comment: 
 
-Filename: creosote-2.6.0.dist-info/METADATA
+Filename: creosote-2.6.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: creosote-2.6.0.dist-info/WHEEL
+Filename: creosote-2.6.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: creosote-2.6.0.dist-info/entry_points.txt
+Filename: creosote-2.6.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: creosote-2.6.0.dist-info/licenses/LICENSE
+Filename: creosote-2.6.0rc1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: creosote-2.6.0.dist-info/RECORD
+Filename: creosote-2.6.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## creosote/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "2.6.0"
+__version__ = "2.6.0rc1"
```

## Comparing `creosote-2.6.0.dist-info/METADATA` & `creosote-2.6.0rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creosote
-Version: 2.6.0
+Version: 2.6.0rc1
 Summary: Identify unused dependencies and avoid a bloated virtual environment.
 Project-URL: Source, https://github.com/fredrikaverpil/creosote
 Project-URL: Tracker, https://github.com/fredrikaverpil/creosote/issues
 Author-email: Fredrik Averpil <fredrik.averpil@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `creosote-2.6.0.dist-info/licenses/LICENSE` & `creosote-2.6.0rc1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `creosote-2.6.0.dist-info/RECORD` & `creosote-2.6.0rc1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-creosote/__about__.py,sha256=OEib63e0yPEGlhEXyrWE1OwRnleR0cHI7KSX7oZEQLs,22
+creosote/__about__.py,sha256=aps7uUKGDgLjYrYEPZq_WIwdMre6OFpK3sCkeJnr5v8,25
 creosote/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 creosote/cli.py,sha256=lT8Zi0N2eMTExCnGUcLXBskTU2A9DuQVHIjECtPIpI8,6597
 creosote/formatters.py,sha256=KaQhieJcUynXI7p24sbO4c08CaBzl_PfV_OyPF9tgOk,1109
 creosote/models.py,sha256=zwLjGtrHDjyRBHi3HLylmxrlUssEYuzoFNsx4trkexQ,523
 creosote/parsers.py,sha256=EWZ97sLM2XgFi3g7OizpMfeE-p0FZTQzH5kYp9ZJ7rk,8558
 creosote/resolvers.py,sha256=E0QPdFJOcwgVDyKjMzrhUJkzHWCdnmlBACLAnVGgRjw,9413
-creosote-2.6.0.dist-info/METADATA,sha256=jRHOtVgLcb671c3vBBBghWPobx8__wzclEy0oxXR2m4,13013
-creosote-2.6.0.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-creosote-2.6.0.dist-info/entry_points.txt,sha256=1WdMKnsMdlsTqCkVmpuvYDayaGWihV0Yf5qJJOa1u1o,47
-creosote-2.6.0.dist-info/licenses/LICENSE,sha256=_hQiru1DnmKFV7ndyrHSYBPcq9g5dMUxzxRqfvyxyvQ,1072
-creosote-2.6.0.dist-info/RECORD,,
+creosote-2.6.0rc1.dist-info/METADATA,sha256=j-ZMiPR9r-VooKwUEey5c-xCQFG_sLJNidMF76P5jMQ,13016
+creosote-2.6.0rc1.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+creosote-2.6.0rc1.dist-info/entry_points.txt,sha256=1WdMKnsMdlsTqCkVmpuvYDayaGWihV0Yf5qJJOa1u1o,47
+creosote-2.6.0rc1.dist-info/licenses/LICENSE,sha256=_hQiru1DnmKFV7ndyrHSYBPcq9g5dMUxzxRqfvyxyvQ,1072
+creosote-2.6.0rc1.dist-info/RECORD,,
```

