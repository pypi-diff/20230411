# Comparing `tmp/aioflureedb-0.7.8.tar.gz` & `tmp/aioflureedb-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioflureedb-0.7.8.tar", last modified: Wed Apr  5 11:37:28 2023, max compression
+gzip compressed data, was "aioflureedb-0.7.9.tar", last modified: Wed Apr  5 11:59:03 2023, max compression
```

## Comparing `aioflureedb-0.7.8.tar` & `aioflureedb-0.7.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:37:28.756662 aioflureedb-0.7.8/
--rw-rw-r--   0 rob       (1000) rob       (1000)      774 2023-04-05 11:37:28.756662 aioflureedb-0.7.8/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     1798 2023-03-30 05:22:33.000000 aioflureedb-0.7.8/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:37:28.752662 aioflureedb-0.7.8/aioflureedb/
--rw-r--r--   0 rob       (1000) rob       (1000)    73743 2023-04-05 11:35:52.000000 aioflureedb-0.7.8/aioflureedb/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6858 2023-03-29 11:47:10.000000 aioflureedb-0.7.8/aioflureedb/__main__.py
--rw-r--r--   0 rob       (1000) rob       (1000)    25924 2022-09-14 15:46:46.000000 aioflureedb-0.7.8/aioflureedb/domain_api.py
--rw-r--r--   0 rob       (1000) rob       (1000)     7010 2022-06-30 09:29:56.000000 aioflureedb-0.7.8/aioflureedb/signing.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:37:28.756662 aioflureedb-0.7.8/aioflureedb.egg-info/
--rw-r--r--   0 rob       (1000) rob       (1000)      774 2023-04-05 11:37:28.000000 aioflureedb-0.7.8/aioflureedb.egg-info/PKG-INFO
--rw-r--r--   0 rob       (1000) rob       (1000)      289 2023-04-05 11:37:28.000000 aioflureedb-0.7.8/aioflureedb.egg-info/SOURCES.txt
--rw-r--r--   0 rob       (1000) rob       (1000)        1 2023-04-05 11:37:28.000000 aioflureedb-0.7.8/aioflureedb.egg-info/dependency_links.txt
--rw-r--r--   0 rob       (1000) rob       (1000)       66 2023-04-05 11:37:28.000000 aioflureedb-0.7.8/aioflureedb.egg-info/requires.txt
--rw-r--r--   0 rob       (1000) rob       (1000)       12 2023-04-05 11:37:28.000000 aioflureedb-0.7.8/aioflureedb.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-04-05 11:37:28.756662 aioflureedb-0.7.8/setup.cfg
--rw-r--r--   0 rob       (1000) rob       (1000)     1148 2023-04-05 11:36:13.000000 aioflureedb-0.7.8/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      774 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1798 2023-03-30 05:22:33.000000 aioflureedb-0.7.9/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/aioflureedb/
+-rw-r--r--   0 rob       (1000) rob       (1000)    74028 2023-04-05 11:57:42.000000 aioflureedb-0.7.9/aioflureedb/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6858 2023-03-29 11:47:10.000000 aioflureedb-0.7.9/aioflureedb/__main__.py
+-rw-r--r--   0 rob       (1000) rob       (1000)    25924 2022-09-14 15:46:46.000000 aioflureedb-0.7.9/aioflureedb/domain_api.py
+-rw-r--r--   0 rob       (1000) rob       (1000)     7010 2022-06-30 09:29:56.000000 aioflureedb-0.7.9/aioflureedb/signing.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/aioflureedb.egg-info/
+-rw-r--r--   0 rob       (1000) rob       (1000)      774 2023-04-05 11:59:02.000000 aioflureedb-0.7.9/aioflureedb.egg-info/PKG-INFO
+-rw-r--r--   0 rob       (1000) rob       (1000)      289 2023-04-05 11:59:03.000000 aioflureedb-0.7.9/aioflureedb.egg-info/SOURCES.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)        1 2023-04-05 11:59:02.000000 aioflureedb-0.7.9/aioflureedb.egg-info/dependency_links.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)       66 2023-04-05 11:59:03.000000 aioflureedb-0.7.9/aioflureedb.egg-info/requires.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)       12 2023-04-05 11:59:03.000000 aioflureedb-0.7.9/aioflureedb.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/setup.cfg
+-rw-r--r--   0 rob       (1000) rob       (1000)     1148 2023-04-05 11:57:53.000000 aioflureedb-0.7.9/setup.py
```

### Comparing `aioflureedb-0.7.8/PKG-INFO` & `aioflureedb-0.7.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioflureedb
-Version: 0.7.8
+Version: 0.7.9
 Summary: Asynchonous library for usage of the FlureeDB API
 Home-page: https://github.com/pibara/aioflureedb
 Author: Rob J Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql sparql graphql
 Platform: UNKNOWN
```

### Comparing `aioflureedb-0.7.8/README.md` & `aioflureedb-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.7.8/aioflureedb/__init__.py` & `aioflureedb-0.7.9/aioflureedb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,14 +431,16 @@
                 kwdict[key] = value
         for reqkey in self.required:
             if reqkey not in kwset:
                 raise TypeError("SignedPoster is missing one required named argument '", reqkey, "'")
         body = json.dumps(kwdict, indent=4, sort_keys=True)
         headers = {"Content-Type": "application/json"}
         if not self.unsigned:
+            if self.debug:
+                print("Signing with:", self.signer.auth_id)
             body, headers, _ = self.signer.sign_query(kwdict)
         rval = await self._post_body_with_headers(body, headers)
         # If this is a new-db or new-legger, we need to await till it comes into existance.
         if (isinstance(rval, str) and len(rval) == 64 and
                 (
                     (self.url.split("/")[-1] == "new-db" and "db_id" in kwargs) or
                     (self.url.split("/")[-1] == "new-ledger" and "ledger_id" in kwargs)
@@ -1716,14 +1718,16 @@
 
                 Returns
                 -------
                 string
                     Return body from server
                 """
                 if self.signer:
+                    if self.debug:
+                        print("Signing with:", self.signer.auth_id)
                     body, headers, _ = self.signer.sign_query(query_body, querytype=self.api_endpoint)
                 else:
                     body = json.dumps(query_body, indent=4, sort_keys=True)
                     headers = {"Content-Type": contenttype}
                 return await self._post_body_with_headers(body, headers)
 
             async def body_signed(self, transact_obj, deps=None):
@@ -1737,14 +1741,16 @@
 
                 Returns
                 -------
                 string
                     Return body from server
 
                 """
+                if self.debug:
+                    print("Signing with:", self.signer.auth_id)
                 command = self.signer.sign_transaction(transact_obj, deps)
                 body = json.dumps(command, indent=4, sort_keys=True)
                 headers = {"content-type": "application/json"}
                 return await self._post_body_with_headers(body, headers)
 
             async def empty_post_unsigned(self):
                 """Do an HTTP POST without body and without signing
```

### Comparing `aioflureedb-0.7.8/aioflureedb/__main__.py` & `aioflureedb-0.7.9/aioflureedb/__main__.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.7.8/aioflureedb/domain_api.py` & `aioflureedb-0.7.9/aioflureedb/domain_api.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.7.8/aioflureedb/signing.py` & `aioflureedb-0.7.9/aioflureedb/signing.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.7.8/aioflureedb.egg-info/PKG-INFO` & `aioflureedb-0.7.9/aioflureedb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioflureedb
-Version: 0.7.8
+Version: 0.7.9
 Summary: Asynchonous library for usage of the FlureeDB API
 Home-page: https://github.com/pibara/aioflureedb
 Author: Rob J Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql sparql graphql
 Platform: UNKNOWN
```

### Comparing `aioflureedb-0.7.8/setup.py` & `aioflureedb-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sys import platform
 here = path.abspath(path.dirname(__file__))
 
 requirements = ["starkbank-ecdsa>=2.0.3", "aiohttp", "base58"]
 
 setup(
     name='aioflureedb',
-    version='0.7.8',
+    version='0.7.9',
     description='Asynchonous library for usage of the FlureeDB API',
     long_description="""An asynchonous client library for communicating with a FlureeDB server, making signed transactions and queries.
     """,
     url='https://github.com/pibara/aioflureedb',
     author='Rob J Meijer',
     author_email='pibara@gmail.com',
     license='BSD',
```

