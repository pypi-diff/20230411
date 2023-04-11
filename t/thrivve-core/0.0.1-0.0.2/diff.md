# Comparing `tmp/thrivve_core-0.0.1.tar.gz` & `tmp/thrivve_core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-amts68or/thrivve_core-0.0.1.tar", last modified: Tue Apr 11 11:20:49 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-qit8mazn/thrivve_core-0.0.2.tar", last modified: Tue Apr 11 11:56:53 2023, max compression
```

## Comparing `thrivve_core-0.0.1.tar` & `thrivve_core-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-11 11:20:37.000000 thrivve_core-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 11:20:49.000000 thrivve_core-0.0.1/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      925 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2519 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12208 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1419 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-11 11:56:45.000000 thrivve_core-0.0.2/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-11 11:56:53.000000 thrivve_core-0.0.2/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.0.1/PKG-INFO` & `thrivve_core-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve_core
-Version: 0.0.1
+Version: 0.0.2
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.0.1/setup.py` & `thrivve_core-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_namespace_packages
 
 # reading long description from file
 # with open('DESCRIPTION.txt') as file:
 #     long_description = file.read()
 
+
 # specify requirements of your package here
 REQUIREMENTS = [
     "SQLAlchemy",
     "Flask-SQLAlchemy",
     "flask-marshmallow",
     "confluent-kafka",
     "requests",
@@ -26,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.0.1",
+    version="0.0.2",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.0.1/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.0.2/thrivve_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

