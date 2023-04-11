# Comparing `tmp/apiflows-1.0.8-py3-none-any.whl.zip` & `tmp/apiflows-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 10949 bytes, number of entries: 17
--rw-r--r--  2.0 unx     4507 b- defN 23-Apr-11 09:05 apiflows.py
+Zip file size: 10950 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     4500 b- defN 23-Apr-11 09:16 apiflows.py
 -rw-r--r--  2.0 unx     1303 b- defN 23-Apr-11 09:04 config.py
--rw-r--r--  2.0 unx      616 b- defN 23-Apr-11 09:05 setup.py
+-rw-r--r--  2.0 unx      616 b- defN 23-Apr-11 09:17 setup.py
 -rw-r--r--  2.0 unx     1669 b- defN 23-Mar-17 07:48 utils.py
 -rw-r--r--  2.0 unx      589 b- defN 23-Mar-18 13:27 assertors/contains.py
 -rw-r--r--  2.0 unx      572 b- defN 23-Mar-18 13:28 assertors/eq.py
 -rw-r--r--  2.0 unx      571 b- defN 23-Mar-18 13:36 assertors/gt.py
 -rw-r--r--  2.0 unx      573 b- defN 23-Mar-18 13:37 assertors/gte.py
 -rw-r--r--  2.0 unx      571 b- defN 23-Mar-18 13:37 assertors/lt.py
 -rw-r--r--  2.0 unx      573 b- defN 23-Mar-18 13:37 assertors/lte.py
 -rw-r--r--  2.0 unx      573 b- defN 23-Mar-18 13:29 assertors/match.py
 -rw-r--r--  2.0 unx      573 b- defN 23-Mar-18 13:28 assertors/neq.py
 -rw-r--r--  2.0 unx     6646 b- defN 23-Apr-11 09:02 models/apicase.py
--rw-r--r--  2.0 unx     3290 b- defN 23-Apr-11 09:12 apiflows-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 09:12 apiflows-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 23-Apr-11 09:12 apiflows-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1219 b- defN 23-Apr-11 09:12 apiflows-1.0.8.dist-info/RECORD
-17 files, 23982 bytes uncompressed, 9001 bytes compressed:  62.5%
+-rw-r--r--  2.0 unx     3290 b- defN 23-Apr-11 09:17 apiflows-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 09:17 apiflows-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 23-Apr-11 09:17 apiflows-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1219 b- defN 23-Apr-11 09:17 apiflows-1.0.9.dist-info/RECORD
+17 files, 23975 bytes uncompressed, 9002 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: assertors/neq.py
 Comment: 
 
 Filename: models/apicase.py
 Comment: 
 
-Filename: apiflows-1.0.8.dist-info/METADATA
+Filename: apiflows-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: apiflows-1.0.8.dist-info/WHEEL
+Filename: apiflows-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: apiflows-1.0.8.dist-info/top_level.txt
+Filename: apiflows-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: apiflows-1.0.8.dist-info/RECORD
+Filename: apiflows-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## apiflows.py

```diff
@@ -141,15 +141,15 @@
     
     with open(args.output, 'w', encoding='utf-8') as f:
         # save test result to file
         logging.info("Saved test result to file:" + args.output)
         json.dump([json.loads(str(api)) for api in results], f, ensure_ascii=False, indent=4)
 
     # post testing
-    config.post_testing(results)
+    config.post_testing()
     
     # exit when failed
     for i, apicases in enumerate(results):
         for j, apicase in enumerate(apicases):
             if not apicase.is_passed():
                 sys.exit(1)
```

## setup.py

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apiflows",
-    version="1.0.8",
+    version="1.0.9",
     author="Allen",
     author_email="aiddroid@gmail.com",
     description="A yaml data-drive HTTP API testing tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aiddroid/apiflows",
     packages=setuptools.find_packages(),
```

## Comparing `apiflows-1.0.8.dist-info/METADATA` & `apiflows-1.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiflows
-Version: 1.0.8
+Version: 1.0.9
 Summary: A yaml data-drive HTTP API testing tools.
 Author-email: Allen <aiddroid@gmail.com>
 Project-URL: Homepage, https://github.com/aiddroid/apiflows
 Project-URL: Bug Tracker, https://github.com/aiddroid/apiflows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `apiflows-1.0.8.dist-info/RECORD` & `apiflows-1.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-apiflows.py,sha256=mBvsQ-PUJ2zOu98bSq6883i-CoFR8iE9sEKhypJQSdY,4507
+apiflows.py,sha256=_7rgS9YIJY8WyHgNnwmncLh-brnw3VMgbRQPa2943lo,4500
 config.py,sha256=jqUuR2r1vbCIqgcEm9jt6QAGtBcwoOok46WRaa1k3dw,1303
-setup.py,sha256=KnkTJvxzyYXq3sPoiDy7gfJQcLa6MEGCOJlfwwmi3Yo,616
+setup.py,sha256=XYdikJtHJo_Qt9DAo2KIg8Dm0FFXVtu0mxHGN4W-99M,616
 utils.py,sha256=w3WghejgmTx49qsvAxveIVLh8RuYPxfPMM9BW-Ttbfs,1669
 assertors/contains.py,sha256=0DVLuMBitB-76g3kCNklIqyYT1glSj0Lrj718BDgJDM,589
 assertors/eq.py,sha256=m1oJ331DSDFUEunznzuUZgQfywCAoT1vIvQFl8ONyrk,572
 assertors/gt.py,sha256=6oiA35LXKXphKHjv9-BThvlHebMpZt69JVBMI04zWKA,571
 assertors/gte.py,sha256=SNJ8heRbXdWhTCfRXsnlYRufcHs1VgMwHTtHy2qi8S4,573
 assertors/lt.py,sha256=6okt5rLDlxhlBPAbJ9hk3oBJ0uceee6gbun80FhbZZc,571
 assertors/lte.py,sha256=d-EbuPz9sfxqbi18HpJXg3kMCd5Xx1GEKNBGU8y4XOc,573
 assertors/match.py,sha256=q1COG440QAQpSySlrVx0tkHa3iGd8AYwv6reVwkt3Gg,573
 assertors/neq.py,sha256=7dbMad4oJWYcB0F7r6dkRLgbSoaX39lX3YEQv4BuzRY,573
 models/apicase.py,sha256=VJr7kG7DWcT1CYBk0c_IZmkJYFBkA_M4ws6ZpPq_3gs,6646
-apiflows-1.0.8.dist-info/METADATA,sha256=8La_KLudCRjgV70wQ4lvc-oyNP6j1iAs0-tmbLQUkpg,3290
-apiflows-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-apiflows-1.0.8.dist-info/top_level.txt,sha256=vwFo0Tc-dizXwUZ43OQtPd8xCnU8z_HOgsdaVXwDIFU,45
-apiflows-1.0.8.dist-info/RECORD,,
+apiflows-1.0.9.dist-info/METADATA,sha256=_aqCrUnzfC96rfVX7J-ozH3bVS5FLc5Uja_5SLyTw-w,3290
+apiflows-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+apiflows-1.0.9.dist-info/top_level.txt,sha256=vwFo0Tc-dizXwUZ43OQtPd8xCnU8z_HOgsdaVXwDIFU,45
+apiflows-1.0.9.dist-info/RECORD,,
```

