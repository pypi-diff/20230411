# Comparing `tmp/jquants_api_client-1.1.0.tar.gz` & `tmp/jquants_api_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jquants_api_client-1.1.0.tar", max compression
+gzip compressed data, was "jquants_api_client-1.1.1.tar", max compression
```

## Comparing `jquants_api_client-1.1.0.tar` & `jquants_api_client-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-07 11:26:49.404079 jquants_api_client-1.1.0/LICENSE
--rw-r--r--   0        0        0     5631 2023-04-07 11:26:49.404079 jquants_api_client-1.1.0/README.md
--rw-r--r--   0        0        0       66 2023-04-07 11:26:49.408079 jquants_api_client-1.1.0/jquantsapi/__init__.py
--rw-r--r--   0        0        0    48096 2023-04-07 11:26:49.408079 jquants_api_client-1.1.0/jquantsapi/client.py
--rw-r--r--   0        0        0    15206 2023-04-07 11:26:49.408079 jquants_api_client-1.1.0/jquantsapi/constants.py
--rw-r--r--   0        0        0      517 2023-04-07 11:26:49.408079 jquants_api_client-1.1.0/jquantsapi/enums.py
--rw-r--r--   0        0        0     1676 2023-04-07 11:27:02.236171 jquants_api_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 jquants_api_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 01:31:26.267331 jquants_api_client-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5631 2023-04-11 01:31:26.267331 jquants_api_client-1.1.1/README.md
+-rw-r--r--   0        0        0       66 2023-04-11 01:31:26.271331 jquants_api_client-1.1.1/jquantsapi/__init__.py
+-rw-r--r--   0        0        0    48163 2023-04-11 01:31:26.271331 jquants_api_client-1.1.1/jquantsapi/client.py
+-rw-r--r--   0        0        0    15206 2023-04-11 01:31:26.271331 jquants_api_client-1.1.1/jquantsapi/constants.py
+-rw-r--r--   0        0        0      517 2023-04-11 01:31:26.271331 jquants_api_client-1.1.1/jquantsapi/enums.py
+-rw-r--r--   0        0        0     1676 2023-04-11 01:31:38.435493 jquants_api_client-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7141 1970-01-01 00:00:00.000000 jquants_api_client-1.1.1/PKG-INFO
```

### Comparing `jquants_api_client-1.1.0/LICENSE` & `jquants_api_client-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.0/README.md` & `jquants_api_client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.0/jquantsapi/client.py` & `jquants_api_client-1.1.1/jquantsapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,14 +539,15 @@
         premium_flag = "MorningClose" in df.columns
         if premium_flag:
             cols = constants.PRICES_DAILY_QUOTES_PREMIUM_COLUMNS
         else:
             cols = constants.PRICES_DAILY_QUOTES_COLUMNS
         if len(df) == 0:
             return pd.DataFrame([], columns=cols)
+        df["Date"] = pd.to_datetime(df["Date"], format="%Y-%m-%d")
         df.sort_values(["Code", "Date"], inplace=True)
         return df[cols]
 
     def get_price_range(
         self,
         start_dt: DatetimeLike = "20170101",
         end_dt: DatetimeLike = datetime.now(),
```

### Comparing `jquants_api_client-1.1.0/jquantsapi/constants.py` & `jquants_api_client-1.1.1/jquantsapi/constants.py`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.0/jquantsapi/enums.py` & `jquants_api_client-1.1.1/jquantsapi/enums.py`

 * *Files identical despite different names*

### Comparing `jquants_api_client-1.1.0/pyproject.toml` & `jquants_api_client-1.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jquants-api-client"
-version = "1.1.0" # use poetry-dynamic-versioning
+version = "1.1.1" # use poetry-dynamic-versioning
 authors = [
     "J-Quants Project Contributors <j-quants@jpx.co.jp>",
 ]
 description = "J-Quants API Client Library"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `jquants_api_client-1.1.0/PKG-INFO` & `jquants_api_client-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jquants-api-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: J-Quants API Client Library
 Home-page: https://github.com/J-Quants/jquants-api-client-python
 License: Apache-2.0
 Keywords: jquants,api,client,J-Quants
 Author: J-Quants Project Contributors
 Author-email: j-quants@jpx.co.jp
 Requires-Python: >=3.7.1,<4.0.0
```

