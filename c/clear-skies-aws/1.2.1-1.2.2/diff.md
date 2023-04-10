# Comparing `tmp/clear-skies-aws-1.2.1.tar.gz` & `tmp/clear-skies-aws-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear-skies-aws-1.2.1.tar", last modified: Tue Apr  4 23:13:44 2023, max compression
+gzip compressed data, was "clear-skies-aws-1.2.2.tar", last modified: Mon Apr 10 23:03:36 2023, max compression
```

## Comparing `clear-skies-aws-1.2.1.tar` & `clear-skies-aws-1.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.430735 clear-skies-aws-1.2.1/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2022-01-16 00:26:29.000000 clear-skies-aws-1.2.1/LICENSE
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2022-01-16 00:26:29.000000 clear-skies-aws-1.2.1/MANIFEST.in
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-04-04 23:13:44.430735 clear-skies-aws-1.2.1/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7780 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.1/README.md
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-04-04 23:13:44.430735 clear-skies-aws-1.2.1/setup.cfg
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1375 2023-04-04 23:13:23.000000 clear-skies-aws-1.2.1/setup.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.418735 clear-skies-aws-1.2.1/src/
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.422735 clear-skies-aws-1.2.1/src/clear_skies_aws.egg-info/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-04-04 23:13:44.000000 clear-skies-aws-1.2.1/src/clear_skies_aws.egg-info/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1604 2023-04-04 23:13:44.000000 clear-skies-aws-1.2.1/src/clear_skies_aws.egg-info/SOURCES.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-04-04 23:13:44.000000 clear-skies-aws-1.2.1/src/clear_skies_aws.egg-info/dependency_links.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       36 2023-04-04 23:13:44.000000 clear-skies-aws-1.2.1/src/clear_skies_aws.egg-info/requires.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       15 2023-04-04 23:13:44.000000 clear-skies-aws-1.2.1/src/clear_skies_aws.egg-info/top_level.txt
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.422735 clear-skies-aws-1.2.1/src/clearskies_aws/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       42 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.422735 clear-skies-aws-1.2.1/src/clearskies_aws/backends/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       83 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.1/src/clearskies_aws/backends/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    27759 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/backends/dynamo_db_backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2726 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.1/src/clearskies_aws/backends/sqs_backend.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.426735 clear-skies-aws-1.2.1/src/clearskies_aws/contexts/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      290 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.1/src/clearskies_aws/contexts/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.1/src/clearskies_aws/contexts/cli.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1002 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_api_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      952 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_elb.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1009 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_http_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1183 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_invocation.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1678 2023-04-04 23:13:02.000000 clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.426735 clear-skies-aws-1.2.1/src/clearskies_aws/di/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       56 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/di/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      775 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.1/src/clearskies_aws/di/standard_dependencies.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.426735 clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      233 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2932 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_api_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      662 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_elb.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      692 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_http_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      715 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_invocation.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2047 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.426735 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      121 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-04 23:13:44.430735 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1810 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1082 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3776 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6444 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1002 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/parameter_store.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1638 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.1/src/clearskies_aws/secrets/secrets_manager.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.287349 clear-skies-aws-1.2.2/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2022-01-16 00:26:29.000000 clear-skies-aws-1.2.2/LICENSE
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2022-01-16 00:26:29.000000 clear-skies-aws-1.2.2/MANIFEST.in
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-04-10 23:03:36.287349 clear-skies-aws-1.2.2/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7780 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.2/README.md
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-04-10 23:03:36.287349 clear-skies-aws-1.2.2/setup.cfg
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1375 2023-04-10 23:01:19.000000 clear-skies-aws-1.2.2/setup.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.279349 clear-skies-aws-1.2.2/src/
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.283349 clear-skies-aws-1.2.2/src/clear_skies_aws.egg-info/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-04-10 23:03:36.000000 clear-skies-aws-1.2.2/src/clear_skies_aws.egg-info/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1604 2023-04-10 23:03:36.000000 clear-skies-aws-1.2.2/src/clear_skies_aws.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-04-10 23:03:36.000000 clear-skies-aws-1.2.2/src/clear_skies_aws.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       36 2023-04-10 23:03:36.000000 clear-skies-aws-1.2.2/src/clear_skies_aws.egg-info/requires.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       15 2023-04-10 23:03:36.000000 clear-skies-aws-1.2.2/src/clear_skies_aws.egg-info/top_level.txt
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.283349 clear-skies-aws-1.2.2/src/clearskies_aws/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       42 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.283349 clear-skies-aws-1.2.2/src/clearskies_aws/backends/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       83 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.2/src/clearskies_aws/backends/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    27759 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/backends/dynamo_db_backend.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2726 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.2/src/clearskies_aws/backends/sqs_backend.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.283349 clear-skies-aws-1.2.2/src/clearskies_aws/contexts/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      290 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.2/src/clearskies_aws/contexts/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.2/src/clearskies_aws/contexts/cli.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1002 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_api_gateway.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      952 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_elb.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1009 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_http_gateway.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1183 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_invocation.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1678 2023-04-04 23:13:02.000000 clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.283349 clear-skies-aws-1.2.2/src/clearskies_aws/di/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       56 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/di/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      775 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.2/src/clearskies_aws/di/standard_dependencies.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.283349 clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      233 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2932 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_api_gateway.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      662 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_elb.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      692 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_http_gateway.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      715 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_invocation.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2047 2023-03-26 15:10:17.000000 clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.287349 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      121 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-04-10 23:03:36.287349 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1810 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1082 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3776 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6444 2023-03-26 13:26:58.000000 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1154 2023-04-10 21:54:56.000000 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/parameter_store.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2397 2023-04-10 21:53:44.000000 clear-skies-aws-1.2.2/src/clearskies_aws/secrets/secrets_manager.py
```

### Comparing `clear-skies-aws-1.2.1/LICENSE` & `clear-skies-aws-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/PKG-INFO` & `clear-skies-aws-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.2.1
+Version: 1.2.2
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clear-skies-aws-1.2.1/README.md` & `clear-skies-aws-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/setup.py` & `clear-skies-aws-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='clear-skies-aws',
-    version='1.2.1',
+    version='1.2.2',
     description='clearskies bindings for working in AWS',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cmancone/clearskies-aws',
     author='Conor Mancone',
     author_email='cmancone@gmail.com',
     license='MIT',
```

### Comparing `clear-skies-aws-1.2.1/src/clear_skies_aws.egg-info/PKG-INFO` & `clear-skies-aws-1.2.2/src/clear_skies_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.2.1
+Version: 1.2.2
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clear-skies-aws-1.2.1/src/clear_skies_aws.egg-info/SOURCES.txt` & `clear-skies-aws-1.2.2/src/clear_skies_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/backends/dynamo_db_backend.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/backends/dynamo_db_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/backends/sqs_backend.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/backends/sqs_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_api_gateway.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_elb.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_http_gateway.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_invocation.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/di/standard_dependencies.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_api_gateway.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_elb.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_http_gateway.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_invocation.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/input_outputs/lambda_sqs_standard.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/input_outputs/lambda_sqs_standard.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/__init__.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.2.1/src/clearskies_aws/secrets/parameter_store.py` & `clear-skies-aws-1.2.2/src/clearskies_aws/secrets/parameter_store.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     def __init__(self, boto3, environment):
         self._boto3 = boto3
         self._environment = environment
         if not self._environment.get('AWS_REGION', True):
             raise ValueError("To use parameter store you must use set the 'AWS_REGION' environment variable")
         self._ssm = self._boto3.client('ssm', region_name=self._environment.get('AWS_REGION'))
 
+    def create(self, path, value):
+        return self.update(path, value)
+
     def get(self, path):
         result = self._ssm.get_parameter(Name=path, WithDecryption=True)
         return result['Parameter']['Value']
 
     def list_secrets(self, path):
         response = self._ssm.get_parameters_by_path(Path=path, Recursive=False)
         return [parameter['Name'] for parameter in response['Parameters']]
@@ -22,7 +25,10 @@
         response = self._ssm.put_parameter(
             Name=path,
             Value=value,
             Type='String',
             Overwrite=True,
         )
         return True
+
+    def upsert(self, path, value):
+        return self.update(path, value)
```

