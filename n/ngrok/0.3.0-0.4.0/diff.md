# Comparing `tmp/ngrok-0.3.0-cp37-abi3-win_amd64.whl.zip` & `tmp/ngrok-0.4.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1935892 bytes, number of entries: 7
--rw-r--r--  4.6 unx     5526 b- defN 23-Mar-29 19:14 ngrok-0.3.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Mar-29 19:14 ngrok-0.3.0.dist-info/WHEEL
--rw-r--r--  4.6 unx    11558 b- defN 23-Mar-29 19:14 ngrok-0.3.0.dist-info/license_files/LICENSE-APACHE
--rw-r--r--  4.6 unx     1056 b- defN 23-Mar-29 19:14 ngrok-0.3.0.dist-info/license_files/LICENSE-MIT
--rw-r--r--  4.6 unx      103 b- defN 23-Mar-29 19:14 ngrok/__init__.py
--rwxr-xr-x  4.6 unx  5332992 b- defN 23-Mar-29 19:14 ngrok/ngrok.pyd
--rw-r--r--  4.6 unx      560 b- defN 23-Mar-29 19:14 ngrok-0.3.0.dist-info/RECORD
-7 files, 5351891 bytes uncompressed, 1934910 bytes compressed:  63.9%
+Zip file size: 2289050 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     5525 b- defN 23-Apr-11 15:37 ngrok-0.4.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-11 15:37 ngrok-0.4.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11558 b- defN 23-Apr-11 15:37 ngrok-0.4.0.dist-info/license_files/LICENSE-APACHE
+-rw-r--r--  4.6 unx     1056 b- defN 23-Apr-11 15:37 ngrok-0.4.0.dist-info/license_files/LICENSE-MIT
+-rw-r--r--  4.6 unx      103 b- defN 23-Apr-11 15:37 ngrok/__init__.py
+-rwxr-xr-x  4.6 unx  6341120 b- defN 23-Apr-11 15:37 ngrok/ngrok.pyd
+-rw-r--r--  4.6 unx      560 b- defN 23-Apr-11 15:37 ngrok-0.4.0.dist-info/RECORD
+7 files, 6360018 bytes uncompressed, 2288068 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: ngrok-0.3.0.dist-info/METADATA
+Filename: ngrok-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: ngrok-0.3.0.dist-info/WHEEL
+Filename: ngrok-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: ngrok-0.3.0.dist-info/license_files/LICENSE-APACHE
+Filename: ngrok-0.4.0.dist-info/license_files/LICENSE-APACHE
 Comment: 
 
-Filename: ngrok-0.3.0.dist-info/license_files/LICENSE-MIT
+Filename: ngrok-0.4.0.dist-info/license_files/LICENSE-MIT
 Comment: 
 
 Filename: ngrok/__init__.py
 Comment: 
 
 Filename: ngrok/ngrok.pyd
 Comment: 
 
-Filename: ngrok-0.3.0.dist-info/RECORD
+Filename: ngrok-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ngrok-0.3.0.dist-info/METADATA` & `ngrok-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngrok
-Version: 0.3.0
+Version: 0.4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Utilities
@@ -44,15 +44,15 @@
 [mit-badge]: https://img.shields.io/badge/license-MIT-blue.svg
 [mit-url]: https://github.com/ngrok/ngrok-rs/blob/main/LICENSE-MIT
 [apache-badge]: https://img.shields.io/badge/license-Apache_2.0-blue.svg
 [apache-url]: https://github.com/ngrok/ngrok-rs/blob/main/LICENSE-APACHE
 [ci-badge]: https://github.com/ngrok/ngrok-py/actions/workflows/ci.yml/badge.svg
 [ci-url]: https://github.com/ngrok/ngrok-py/actions/workflows/ci.yml
 
-**Note: This is alpha-quality software. Interfaces may change without warning.**
+**Note: This is beta-quality software. Interfaces may change without warning.**
 
 [ngrok](https://ngrok.com) is a globally distributed reverse proxy commonly used for quickly getting a public URL to a
 service running inside a private network, such as on your local laptop. The ngrok agent is usually
 deployed inside a private network and is used to communicate with the ngrok cloud service.
 
 This is the ngrok agent in library form, suitable for integrating directly into Python
 applications. This allows you to quickly build ngrok into your application with no separate process
```

## Comparing `ngrok-0.3.0.dist-info/license_files/LICENSE-APACHE` & `ngrok-0.4.0.dist-info/license_files/LICENSE-APACHE`

 * *Files identical despite different names*

## Comparing `ngrok-0.3.0.dist-info/license_files/LICENSE-MIT` & `ngrok-0.4.0.dist-info/license_files/LICENSE-MIT`

 * *Files identical despite different names*

