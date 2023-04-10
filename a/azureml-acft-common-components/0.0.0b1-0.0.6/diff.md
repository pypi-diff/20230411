# Comparing `tmp/azureml_acft_common_components-0.0.0b1-py3-none-any.whl.zip` & `tmp/azureml_acft_common_components-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,23 @@
-Zip file size: 2909 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      249 b- defN 20-Jun-24 20:49 azureml/__init__.py
--rw-rw-rw-  2.0 fat      249 b- defN 20-Jun-24 20:49 azureml/acft/__init__.py
--rw-rw-rw-  2.0 fat      249 b- defN 20-Jun-24 20:49 azureml/acft/common/__init__.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Mar-07 17:41 azureml_acft_common_components-0.0.0b1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      422 b- defN 23-Mar-07 17:41 azureml_acft_common_components-0.0.0b1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-07 17:41 azureml_acft_common_components-0.0.0b1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-07 17:41 azureml_acft_common_components-0.0.0b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      755 b- defN 23-Mar-07 17:41 azureml_acft_common_components-0.0.0b1.dist-info/RECORD
-8 files, 3045 bytes uncompressed, 1555 bytes compressed:  48.9%
+Zip file size: 18281 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat      251 b- defN 23-Apr-10 23:37 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      317 b- defN 23-Apr-10 23:37 azureml/acft/__init__.py
+-rw-rw-rw-  2.0 fat     1226 b- defN 23-Apr-10 23:37 azureml/acft/common_components/__init__.py
+-rw-rw-rw-  2.0 fat       34 b- defN 23-Apr-10 23:44 azureml/acft/common_components/_version.py
+-rw-rw-rw-  2.0 fat      325 b- defN 23-Apr-10 23:37 azureml/acft/common_components/model_selector/__init__.py
+-rw-rw-rw-  2.0 fat     7131 b- defN 23-Apr-10 23:37 azureml/acft/common_components/model_selector/component.py
+-rw-rw-rw-  2.0 fat      762 b- defN 23-Apr-10 23:37 azureml/acft/common_components/model_selector/constants.py
+-rw-rw-rw-  2.0 fat      236 b- defN 23-Apr-10 23:37 azureml/acft/common_components/utils/__init__.py
+-rw-rw-rw-  2.0 fat    12226 b- defN 23-Apr-10 23:37 azureml/acft/common_components/utils/logging_utils.py
+-rw-rw-rw-  2.0 fat     1649 b- defN 23-Apr-10 23:37 azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py
+-rw-rw-rw-  2.0 fat      226 b- defN 23-Apr-10 23:37 azureml/acft/common_components/utils/error_handling/__init__.py
+-rw-rw-rw-  2.0 fat     6226 b- defN 23-Apr-10 23:37 azureml/acft/common_components/utils/error_handling/error_definitions.py
+-rw-rw-rw-  2.0 fat     2781 b- defN 23-Apr-10 23:37 azureml/acft/common_components/utils/error_handling/error_strings.py
+-rw-rw-rw-  2.0 fat     3650 b- defN 23-Apr-10 23:37 azureml/acft/common_components/utils/error_handling/exceptions.py
+-rw-rw-rw-  2.0 fat     5663 b- defN 23-Apr-10 23:37 azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py
+-rw-rw-rw-  2.0 fat      859 b- defN 23-Apr-10 23:44 azureml_acft_common_components-0.0.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      972 b- defN 23-Apr-10 23:44 azureml_acft_common_components-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-10 23:44 azureml_acft_common_components-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-10 23:44 azureml_acft_common_components-0.0.6.dist-info/namespace_packages.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-10 23:44 azureml_acft_common_components-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2302 b- defN 23-Apr-10 23:44 azureml_acft_common_components-0.0.6.dist-info/RECORD
+21 files, 46942 bytes uncompressed, 14311 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,25 +1,64 @@
 Filename: azureml/__init__.py
 Comment: 
 
 Filename: azureml/acft/__init__.py
 Comment: 
 
-Filename: azureml/acft/common/__init__.py
+Filename: azureml/acft/common_components/__init__.py
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.0b1.dist-info/LICENSE.txt
+Filename: azureml/acft/common_components/_version.py
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.0b1.dist-info/METADATA
+Filename: azureml/acft/common_components/model_selector/__init__.py
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.0b1.dist-info/WHEEL
+Filename: azureml/acft/common_components/model_selector/component.py
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.0b1.dist-info/top_level.txt
+Filename: azureml/acft/common_components/model_selector/constants.py
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.0b1.dist-info/RECORD
+Filename: azureml/acft/common_components/utils/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/logging_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/error_handling/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/error_handling/error_definitions.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/error_handling/error_strings.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/error_handling/exceptions.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py
+Comment: 
+
+Filename: azureml_acft_common_components-0.0.6.dist-info/LICENSE.txt
+Comment: 
+
+Filename: azureml_acft_common_components-0.0.6.dist-info/METADATA
+Comment: 
+
+Filename: azureml_acft_common_components-0.0.6.dist-info/WHEEL
+Comment: 
+
+Filename: azureml_acft_common_components-0.0.6.dist-info/namespace_packages.txt
+Comment: 
+
+Filename: azureml_acft_common_components-0.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: azureml_acft_common_components-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/__init__.py

```diff
@@ -1,4 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
+
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
```

## azureml/acft/__init__.py

```diff
@@ -1,4 +1,7 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
-__path__ = __import__('pkgutil').extend_path(__path__, __name__)
+
+"""Azure ML ACFT Common Components package."""
+
+__path__ = __import__("pkgutil").extend_path(__path__, __name__)  # type: ignore
```

## Comparing `azureml_acft_common_components-0.0.0b1.dist-info/LICENSE.txt` & `azureml_acft_common_components-0.0.6.dist-info/LICENSE.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-This Preview is made available to you on the condition that you agree to the
-[Supplemental Terms of Use for Microsoft Azure Previews][1], which supplement
-[your agreement][2] governing your use of Azure.
+This software is made available to you on the condition that you agree to
+[your agreement][1] governing your use of Azure.
 If you do not have an existing agreement governing your use of Azure, you agree that 
-your agreement governing use of Azure is the [Microsoft Online Subscription Agreement][3]
-(which incorporates the [Online Services Terms][4]).
-By using the Preview you agree to these terms. This Preview may collect data
-that is transmitted to Microsoft. Please see the [Microsoft Privacy Statement][5]
+your agreement governing use of Azure is the [Microsoft Online Subscription Agreement][2]
+(which incorporates the [Online Services Terms][3]).
+By using the software you agree to these terms. This software may collect data
+that is transmitted to Microsoft. Please see the [Microsoft Privacy Statement][4]
 to learn more about how Microsoft processes personal data.
 
-[1]: https://azure.microsoft.com/en-us/support/legal/preview-supplemental-terms/
-[2]: https://azure.microsoft.com/en-us/support/legal/
-[3]: https://azure.microsoft.com/en-us/support/legal/subscription-agreement/
-[4]: http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=46
-[5]: http://go.microsoft.com/fwlink/?LinkId=248681 
+[1]: https://azure.microsoft.com/en-us/support/legal/
+[2]: https://azure.microsoft.com/en-us/support/legal/subscription-agreement/
+[3]: http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=46
+[4]: http://go.microsoft.com/fwlink/?LinkId=248681
```

