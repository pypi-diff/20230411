# Comparing `tmp/cdktf-cdktf-provider-dnsimple-3.0.3.tar.gz` & `tmp/cdktf-cdktf-provider-dnsimple-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-dnsimple-3.0.3.tar", last modified: Tue Apr  4 07:16:38 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-dnsimple-4.0.0.tar", last modified: Tue Apr 11 13:03:52 2023, max compression
```

## Comparing `cdktf-cdktf-provider-dnsimple-3.0.3.tar` & `cdktf-cdktf-provider-dnsimple-4.0.0.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.102315 cdktf-cdktf-provider-dnsimple-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.102315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   173390 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@3.0.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    20226 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
--rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/email_forward/
--rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    33867 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/record/
--rw-r--r--   0 runner    (1001) docker     (123)    26774 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/zone_record/
--rw-r--r--   0 runner    (1001) docker     (123)    27141 2023-04-04 07:16:25.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:16:38.106315 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-04 07:16:38.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-04 07:16:38.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:16:38.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-04 07:16:38.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-04 07:16:38.000000 cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.053041 cdktf-cdktf-provider-dnsimple-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.057041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.057041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127447 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    17539 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/
+-rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    24362 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.057041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/LICENSE` & `cdktf-cdktf-provider-dnsimple-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 3.0.3
+Version: 4.0.0
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/README.md` & `cdktf-cdktf-provider-dnsimple-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/setup.py` & `cdktf-cdktf-provider-dnsimple-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-dnsimple",
-    "version": "3.0.3",
+    "version": "4.0.0",
     "description": "Prebuilt dnsimple Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-dnsimple.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,20 +25,19 @@
         "cdktf_cdktf_provider_dnsimple._jsii",
         "cdktf_cdktf_provider_dnsimple.data_dnsimple_certificate",
         "cdktf_cdktf_provider_dnsimple.data_dnsimple_zone",
         "cdktf_cdktf_provider_dnsimple.domain",
         "cdktf_cdktf_provider_dnsimple.email_forward",
         "cdktf_cdktf_provider_dnsimple.lets_encrypt_certificate",
         "cdktf_cdktf_provider_dnsimple.provider",
-        "cdktf_cdktf_provider_dnsimple.record",
         "cdktf_cdktf_provider_dnsimple.zone_record"
     ],
     "package_data": {
         "cdktf_cdktf_provider_dnsimple._jsii": [
-            "provider-dnsimple@3.0.3.jsii.tgz"
+            "provider-dnsimple@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_dnsimple": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/__init__.py` & `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,22 +107,20 @@
 __all__ = [
     "data_dnsimple_certificate",
     "data_dnsimple_zone",
     "domain",
     "email_forward",
     "lets_encrypt_certificate",
     "provider",
-    "record",
     "zone_record",
 ]
 
 publication.publish()
 
 # Loading modules to ensure their types are registered with the jsii runtime library
 from . import data_dnsimple_certificate
 from . import data_dnsimple_zone
 from . import domain
 from . import email_forward
 from . import lets_encrypt_certificate
 from . import provider
-from . import record
 from . import zone_record
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_dnsimple_certificate`
+# `dnsimple_lets_encrypt_certificate`
 
-Refer to the Terraform Registory for docs: [`data_dnsimple_certificate`](https://www.terraform.io/docs/providers/dnsimple/d/certificate).
+Refer to the Terraform Registory for docs: [`dnsimple_lets_encrypt_certificate`](https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,216 +17,266 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataDnsimpleCertificate(
-    _cdktf_9a9027ec.TerraformDataSource,
+class LetsEncryptCertificate(
+    _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dnsimple.dataDnsimpleCertificate.DataDnsimpleCertificate",
+    jsii_type="@cdktf/provider-dnsimple.letsEncryptCertificate.LetsEncryptCertificate",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate dnsimple_certificate}.'''
+    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate dnsimple_lets_encrypt_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        certificate_id: builtins.str,
-        domain: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+        domain_id: builtins.str,
+        name: builtins.str,
+        signature_algorithm: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate dnsimple_certificate} Data Source.
+        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate dnsimple_lets_encrypt_certificate} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param certificate_id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#certificate_id DataDnsimpleCertificate#certificate_id}.
-        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#domain DataDnsimpleCertificate#domain}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#id DataDnsimpleCertificate#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param auto_renew: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
+        :param domain_id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
+        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
+        :param signature_algorithm: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d2e8d5ec9706be398631839424855548229e0ad79622ff5af4b02339407a3e7a)
+            type_hints = typing.get_type_hints(_typecheckingstub__baf9170565dd5a0e411aa9fc260d074a96b9161acd4607bcb9162bf772464ea0)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = DataDnsimpleCertificateConfig(
-            certificate_id=certificate_id,
-            domain=domain,
-            id=id,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = LetsEncryptCertificateConfig(
+            auto_renew=auto_renew,
+            domain_id=domain_id,
+            name=name,
+            signature_algorithm=signature_algorithm,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
+        jsii.create(self.__class__, self, [scope, id, config])
 
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+    @jsii.member(jsii_name="resetSignatureAlgorithm")
+    def reset_signature_algorithm(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetSignatureAlgorithm", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="certificateChain")
-    def certificate_chain(self) -> typing.List[builtins.str]:
-        return typing.cast(typing.List[builtins.str], jsii.get(self, "certificateChain"))
+    @jsii.member(jsii_name="authorityIdentifier")
+    def authority_identifier(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "authorityIdentifier"))
+
+    @builtins.property
+    @jsii.member(jsii_name="createdAt")
+    def created_at(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "createdAt"))
+
+    @builtins.property
+    @jsii.member(jsii_name="csr")
+    def csr(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "csr"))
+
+    @builtins.property
+    @jsii.member(jsii_name="expiresAt")
+    def expires_at(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "expiresAt"))
 
     @builtins.property
-    @jsii.member(jsii_name="privateKey")
-    def private_key(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "privateKey"))
+    @jsii.member(jsii_name="id")
+    def id(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "id"))
 
     @builtins.property
-    @jsii.member(jsii_name="rootCertificate")
-    def root_certificate(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "rootCertificate"))
+    @jsii.member(jsii_name="state")
+    def state(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "state"))
+
+    @builtins.property
+    @jsii.member(jsii_name="updatedAt")
+    def updated_at(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "updatedAt"))
+
+    @builtins.property
+    @jsii.member(jsii_name="years")
+    def years(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "years"))
+
+    @builtins.property
+    @jsii.member(jsii_name="autoRenewInput")
+    def auto_renew_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "autoRenewInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="serverCertificate")
-    def server_certificate(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "serverCertificate"))
+    @jsii.member(jsii_name="domainIdInput")
+    def domain_id_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "domainIdInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="certificateIdInput")
-    def certificate_id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "certificateIdInput"))
+    @jsii.member(jsii_name="nameInput")
+    def name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="domainInput")
-    def domain_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "domainInput"))
+    @jsii.member(jsii_name="signatureAlgorithmInput")
+    def signature_algorithm_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "signatureAlgorithmInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
+    @jsii.member(jsii_name="autoRenew")
+    def auto_renew(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "autoRenew"))
+
+    @auto_renew.setter
+    def auto_renew(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a1c625380326aede0264f73d07321e723c6fdd40a105f44e3019b524a24c1ec6)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "autoRenew", value)
 
     @builtins.property
-    @jsii.member(jsii_name="certificateId")
-    def certificate_id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "certificateId"))
+    @jsii.member(jsii_name="domainId")
+    def domain_id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "domainId"))
 
-    @certificate_id.setter
-    def certificate_id(self, value: builtins.str) -> None:
+    @domain_id.setter
+    def domain_id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7b517103926dfdecc6d4db024b413ad4cbb0114bb01c0438addd374d9ab640df)
+            type_hints = typing.get_type_hints(_typecheckingstub__f1f0420bef8d392657f46cb05288fdcec9f81b26774869507832adb9f190c50b)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "certificateId", value)
+        jsii.set(self, "domainId", value)
 
     @builtins.property
-    @jsii.member(jsii_name="domain")
-    def domain(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "domain"))
+    @jsii.member(jsii_name="name")
+    def name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "name"))
 
-    @domain.setter
-    def domain(self, value: builtins.str) -> None:
+    @name.setter
+    def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__40e9d8291409a7e51ebfd11b64c07670f8d587eb22a54d6bb9afbf01b0120a0e)
+            type_hints = typing.get_type_hints(_typecheckingstub__9eabc0e6d5c719ce5d80048a75d4cebd06f55e946841ab50039b3663ef6d2932)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "domain", value)
+        jsii.set(self, "name", value)
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
+    @jsii.member(jsii_name="signatureAlgorithm")
+    def signature_algorithm(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "signatureAlgorithm"))
 
-    @id.setter
-    def id(self, value: builtins.str) -> None:
+    @signature_algorithm.setter
+    def signature_algorithm(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ecdedeb859a901ad942bb8e40f10cc7291eee0c8f31f2f8a504579703ef8b247)
+            type_hints = typing.get_type_hints(_typecheckingstub__655ca0045fe932de4e65bdfa00a161f01e317646b4fd62fde46768450f4db5a6)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
+        jsii.set(self, "signatureAlgorithm", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dnsimple.dataDnsimpleCertificate.DataDnsimpleCertificateConfig",
+    jsii_type="@cdktf/provider-dnsimple.letsEncryptCertificate.LetsEncryptCertificateConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "certificate_id": "certificateId",
-        "domain": "domain",
-        "id": "id",
+        "auto_renew": "autoRenew",
+        "domain_id": "domainId",
+        "name": "name",
+        "signature_algorithm": "signatureAlgorithm",
     },
 )
-class DataDnsimpleCertificateConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class LetsEncryptCertificateConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-        certificate_id: builtins.str,
-        domain: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+        domain_id: builtins.str,
+        name: builtins.str,
+        signature_algorithm: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param certificate_id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#certificate_id DataDnsimpleCertificate#certificate_id}.
-        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#domain DataDnsimpleCertificate#domain}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#id DataDnsimpleCertificate#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param auto_renew: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
+        :param domain_id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
+        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
+        :param signature_algorithm: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ca0765b33ca73367b3617b217b7c6b012e403c049ef5b5d2c6c9a819abce38da)
+            type_hints = typing.get_type_hints(_typecheckingstub__850d843c640aa5551388a4b8af50716ee9c777d9927cb4bc9dda2315153cf876)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument certificate_id", value=certificate_id, expected_type=type_hints["certificate_id"])
-            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument domain_id", value=domain_id, expected_type=type_hints["domain_id"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument signature_algorithm", value=signature_algorithm, expected_type=type_hints["signature_algorithm"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "certificate_id": certificate_id,
-            "domain": domain,
+            "auto_renew": auto_renew,
+            "domain_id": domain_id,
+            "name": name,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -234,16 +284,16 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
+        if signature_algorithm is not None:
+            self._values["signature_algorithm"] = signature_algorithm
 
     @builtins.property
     def connection(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
         '''
         :stability: experimental
@@ -300,100 +350,111 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def certificate_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#certificate_id DataDnsimpleCertificate#certificate_id}.'''
-        result = self._values.get("certificate_id")
-        assert result is not None, "Required property 'certificate_id' is missing"
-        return typing.cast(builtins.str, result)
+    def auto_renew(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.'''
+        result = self._values.get("auto_renew")
+        assert result is not None, "Required property 'auto_renew' is missing"
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
-    def domain(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#domain DataDnsimpleCertificate#domain}.'''
-        result = self._values.get("domain")
-        assert result is not None, "Required property 'domain' is missing"
+    def domain_id(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.'''
+        result = self._values.get("domain_id")
+        assert result is not None, "Required property 'domain_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#id DataDnsimpleCertificate#id}.
+    def name(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#name LetsEncryptCertificate#name}.'''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(builtins.str, result)
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
+    @builtins.property
+    def signature_algorithm(self) -> typing.Optional[builtins.str]:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.'''
+        result = self._values.get("signature_algorithm")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataDnsimpleCertificateConfig(%s)" % ", ".join(
+        return "LetsEncryptCertificateConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "DataDnsimpleCertificate",
-    "DataDnsimpleCertificateConfig",
+    "LetsEncryptCertificate",
+    "LetsEncryptCertificateConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__d2e8d5ec9706be398631839424855548229e0ad79622ff5af4b02339407a3e7a(
+def _typecheckingstub__baf9170565dd5a0e411aa9fc260d074a96b9161acd4607bcb9162bf772464ea0(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    certificate_id: builtins.str,
-    domain: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    domain_id: builtins.str,
+    name: builtins.str,
+    signature_algorithm: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7b517103926dfdecc6d4db024b413ad4cbb0114bb01c0438addd374d9ab640df(
+def _typecheckingstub__a1c625380326aede0264f73d07321e723c6fdd40a105f44e3019b524a24c1ec6(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f1f0420bef8d392657f46cb05288fdcec9f81b26774869507832adb9f190c50b(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__40e9d8291409a7e51ebfd11b64c07670f8d587eb22a54d6bb9afbf01b0120a0e(
+def _typecheckingstub__9eabc0e6d5c719ce5d80048a75d4cebd06f55e946841ab50039b3663ef6d2932(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ecdedeb859a901ad942bb8e40f10cc7291eee0c8f31f2f8a504579703ef8b247(
+def _typecheckingstub__655ca0045fe932de4e65bdfa00a161f01e317646b4fd62fde46768450f4db5a6(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ca0765b33ca73367b3617b217b7c6b012e403c049ef5b5d2c6c9a819abce38da(
+def _typecheckingstub__850d843c640aa5551388a4b8af50716ee9c777d9927cb4bc9dda2315153cf876(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    certificate_id: builtins.str,
-    domain: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    domain_id: builtins.str,
+    name: builtins.str,
+    signature_algorithm: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py` & `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
         '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/d/zone dnsimple_zone} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}.
+        :param name: Zone Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -145,15 +145,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}.
+        :param name: Zone Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9051fabefb514091998aee3b06ffda795da4195d413ca0bc91120a12dc8cf592)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -241,15 +241,18 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}.'''
+        '''Zone Name.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}
+        '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py` & `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `dnsimple_domain`
+# `dnsimple_email_forward`
 
-Refer to the Terraform Registory for docs: [`dnsimple_domain`](https://www.terraform.io/docs/providers/dnsimple/r/domain).
+Refer to the Terraform Registory for docs: [`dnsimple_email_forward`](https://www.terraform.io/docs/providers/dnsimple/r/email_forward).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,201 +17,203 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class Domain(
+class EmailForward(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dnsimple.domain.Domain",
+    jsii_type="@cdktf/provider-dnsimple.emailForward.EmailForward",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/domain dnsimple_domain}.'''
+    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward dnsimple_email_forward}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        name: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        alias_name: builtins.str,
+        destination_email: builtins.str,
+        domain: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/domain dnsimple_domain} Resource.
+        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward dnsimple_email_forward} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#name Domain#name}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#id Domain#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param alias_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.
+        :param destination_email: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.
+        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bfdaf63df24e37e02d8156377b8a72815d9c2f794e36891125e09f1d22c393b8)
+            type_hints = typing.get_type_hints(_typecheckingstub__b8786423bd640cbf734867c6903ef829c1bf2def3b03e9eb355e6581b375e104)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = DomainConfig(
-            name=name,
-            id=id,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = EmailForwardConfig(
+            alias_name=alias_name,
+            destination_email=destination_email,
+            domain=domain,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
-
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+        jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="accountId")
-    def account_id(self) -> jsii.Number:
-        return typing.cast(jsii.Number, jsii.get(self, "accountId"))
+    @jsii.member(jsii_name="aliasEmail")
+    def alias_email(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "aliasEmail"))
 
     @builtins.property
-    @jsii.member(jsii_name="autoRenew")
-    def auto_renew(self) -> _cdktf_9a9027ec.IResolvable:
-        return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "autoRenew"))
-
-    @builtins.property
-    @jsii.member(jsii_name="privateWhois")
-    def private_whois(self) -> _cdktf_9a9027ec.IResolvable:
-        return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "privateWhois"))
+    @jsii.member(jsii_name="id")
+    def id(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "id"))
 
     @builtins.property
-    @jsii.member(jsii_name="registrantId")
-    def registrant_id(self) -> jsii.Number:
-        return typing.cast(jsii.Number, jsii.get(self, "registrantId"))
+    @jsii.member(jsii_name="aliasNameInput")
+    def alias_name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "aliasNameInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="state")
-    def state(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "state"))
+    @jsii.member(jsii_name="destinationEmailInput")
+    def destination_email_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "destinationEmailInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="unicodeName")
-    def unicode_name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "unicodeName"))
+    @jsii.member(jsii_name="domainInput")
+    def domain_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "domainInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
+    @jsii.member(jsii_name="aliasName")
+    def alias_name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "aliasName"))
 
-    @builtins.property
-    @jsii.member(jsii_name="nameInput")
-    def name_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
+    @alias_name.setter
+    def alias_name(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0c391f0f167e1ce785d68334af05b90de6e3c00eac6796e1415ee3de1557c959)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "aliasName", value)
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
+    @jsii.member(jsii_name="destinationEmail")
+    def destination_email(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "destinationEmail"))
 
-    @id.setter
-    def id(self, value: builtins.str) -> None:
+    @destination_email.setter
+    def destination_email(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7b99319fa5c0158b3fc5f2a49c22880161fe52c92112d5065b594e0bd8775782)
+            type_hints = typing.get_type_hints(_typecheckingstub__aeee67e178fa004ade13e0235bc050e34e33ddb2371fd96be233943cc1ba2fe8)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
+        jsii.set(self, "destinationEmail", value)
 
     @builtins.property
-    @jsii.member(jsii_name="name")
-    def name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "name"))
+    @jsii.member(jsii_name="domain")
+    def domain(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "domain"))
 
-    @name.setter
-    def name(self, value: builtins.str) -> None:
+    @domain.setter
+    def domain(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2fad05852d82516cf8dadee6daca736650707f572e296d66f819e6947dde759c)
+            type_hints = typing.get_type_hints(_typecheckingstub__062d0fb1ae26591e344d3dc015d96e337a51de0b777d99d3aed344ea786f434c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "name", value)
+        jsii.set(self, "domain", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dnsimple.domain.DomainConfig",
+    jsii_type="@cdktf/provider-dnsimple.emailForward.EmailForwardConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "name": "name",
-        "id": "id",
+        "alias_name": "aliasName",
+        "destination_email": "destinationEmail",
+        "domain": "domain",
     },
 )
-class DomainConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class EmailForwardConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-        name: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        alias_name: builtins.str,
+        destination_email: builtins.str,
+        domain: builtins.str,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#name Domain#name}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#id Domain#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param alias_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.
+        :param destination_email: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.
+        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ccdf96388a7db479d080fabd9b5d7171adf0d0c2a040f80a4128b4e40eddb3d8)
+            type_hints = typing.get_type_hints(_typecheckingstub__7c6546ae8c4e2ee7d31438ac376a1ff2cb6b6c255b682e868b4941a86fc64016)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument alias_name", value=alias_name, expected_type=type_hints["alias_name"])
+            check_type(argname="argument destination_email", value=destination_email, expected_type=type_hints["destination_email"])
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "name": name,
+            "alias_name": alias_name,
+            "destination_email": destination_email,
+            "domain": domain,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -219,16 +221,14 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
 
     @builtins.property
     def connection(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
         '''
         :stability: experimental
@@ -285,85 +285,97 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#name Domain#name}.'''
-        result = self._values.get("name")
-        assert result is not None, "Required property 'name' is missing"
+    def alias_name(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.'''
+        result = self._values.get("alias_name")
+        assert result is not None, "Required property 'alias_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#id Domain#id}.
+    def destination_email(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.'''
+        result = self._values.get("destination_email")
+        assert result is not None, "Required property 'destination_email' is missing"
+        return typing.cast(builtins.str, result)
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
+    @builtins.property
+    def domain(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.'''
+        result = self._values.get("domain")
+        assert result is not None, "Required property 'domain' is missing"
+        return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DomainConfig(%s)" % ", ".join(
+        return "EmailForwardConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "Domain",
-    "DomainConfig",
+    "EmailForward",
+    "EmailForwardConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__bfdaf63df24e37e02d8156377b8a72815d9c2f794e36891125e09f1d22c393b8(
+def _typecheckingstub__b8786423bd640cbf734867c6903ef829c1bf2def3b03e9eb355e6581b375e104(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    name: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    alias_name: builtins.str,
+    destination_email: builtins.str,
+    domain: builtins.str,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7b99319fa5c0158b3fc5f2a49c22880161fe52c92112d5065b594e0bd8775782(
+def _typecheckingstub__0c391f0f167e1ce785d68334af05b90de6e3c00eac6796e1415ee3de1557c959(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__aeee67e178fa004ade13e0235bc050e34e33ddb2371fd96be233943cc1ba2fe8(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__2fad05852d82516cf8dadee6daca736650707f572e296d66f819e6947dde759c(
+def _typecheckingstub__062d0fb1ae26591e344d3dc015d96e337a51de0b777d99d3aed344ea786f434c(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ccdf96388a7db479d080fabd9b5d7171adf0d0c2a040f80a4128b4e40eddb3d8(
+def _typecheckingstub__7c6546ae8c4e2ee7d31438ac376a1ff2cb6b6c255b682e868b4941a86fc64016(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    name: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    alias_name: builtins.str,
+    destination_email: builtins.str,
+    domain: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py` & `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `dnsimple_email_forward`
+# `dnsimple_zone_record`
 
-Refer to the Terraform Registory for docs: [`dnsimple_email_forward`](https://www.terraform.io/docs/providers/dnsimple/r/email_forward).
+Refer to the Terraform Registory for docs: [`dnsimple_zone_record`](https://www.terraform.io/docs/providers/dnsimple/r/zone_record).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,226 +17,289 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class EmailForward(
+class ZoneRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-dnsimple.emailForward.EmailForward",
+    jsii_type="@cdktf/provider-dnsimple.zoneRecord.ZoneRecord",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward dnsimple_email_forward}.'''
+    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record dnsimple_zone_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        alias_name: builtins.str,
-        destination_email: builtins.str,
-        domain: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        name: builtins.str,
+        type: builtins.str,
+        value: builtins.str,
+        zone_name: builtins.str,
+        priority: typing.Optional[jsii.Number] = None,
+        ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward dnsimple_email_forward} Resource.
+        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record dnsimple_zone_record} Resource.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.
-        :param destination_email: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.
-        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#id EmailForward#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#name ZoneRecord#name}.
+        :param type: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#type ZoneRecord#type}.
+        :param value: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#value ZoneRecord#value}.
+        :param zone_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#zone_name ZoneRecord#zone_name}.
+        :param priority: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#priority ZoneRecord#priority}.
+        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#ttl ZoneRecord#ttl}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b8786423bd640cbf734867c6903ef829c1bf2def3b03e9eb355e6581b375e104)
+            type_hints = typing.get_type_hints(_typecheckingstub__17fe08f86dc04f40ad93499e2500792abbf08802751801af048d1c9ec1b18e9d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = EmailForwardConfig(
-            alias_name=alias_name,
-            destination_email=destination_email,
-            domain=domain,
-            id=id,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = ZoneRecordConfig(
+            name=name,
+            type=type,
+            value=value,
+            zone_name=zone_name,
+            priority=priority,
+            ttl=ttl,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
+        jsii.create(self.__class__, self, [scope, id, config])
 
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
+    @jsii.member(jsii_name="resetPriority")
+    def reset_priority(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetPriority", []))
+
+    @jsii.member(jsii_name="resetTtl")
+    def reset_ttl(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetTtl", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="aliasEmail")
-    def alias_email(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "aliasEmail"))
+    @jsii.member(jsii_name="id")
+    def id(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "id"))
+
+    @builtins.property
+    @jsii.member(jsii_name="qualifiedName")
+    def qualified_name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "qualifiedName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="zoneId")
+    def zone_id(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "zoneId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="nameInput")
+    def name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="priorityInput")
+    def priority_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "priorityInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="aliasNameInput")
-    def alias_name_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "aliasNameInput"))
+    @jsii.member(jsii_name="ttlInput")
+    def ttl_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "ttlInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="destinationEmailInput")
-    def destination_email_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "destinationEmailInput"))
+    @jsii.member(jsii_name="typeInput")
+    def type_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "typeInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="domainInput")
-    def domain_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "domainInput"))
+    @jsii.member(jsii_name="valueInput")
+    def value_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "valueInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
+    @jsii.member(jsii_name="zoneNameInput")
+    def zone_name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "zoneNameInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="aliasName")
-    def alias_name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "aliasName"))
+    @jsii.member(jsii_name="name")
+    def name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "name"))
 
-    @alias_name.setter
-    def alias_name(self, value: builtins.str) -> None:
+    @name.setter
+    def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0c391f0f167e1ce785d68334af05b90de6e3c00eac6796e1415ee3de1557c959)
+            type_hints = typing.get_type_hints(_typecheckingstub__c81d85039e11cc4da512fd0271fcb863f089e45607043af33c44e3620ff74418)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "aliasName", value)
+        jsii.set(self, "name", value)
 
     @builtins.property
-    @jsii.member(jsii_name="destinationEmail")
-    def destination_email(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "destinationEmail"))
+    @jsii.member(jsii_name="priority")
+    def priority(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "priority"))
 
-    @destination_email.setter
-    def destination_email(self, value: builtins.str) -> None:
+    @priority.setter
+    def priority(self, value: jsii.Number) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__aeee67e178fa004ade13e0235bc050e34e33ddb2371fd96be233943cc1ba2fe8)
+            type_hints = typing.get_type_hints(_typecheckingstub__7a6ef6e36231aaee7590125559800d2d0edfca2e78b3043fee0f5f1f804de788)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "destinationEmail", value)
+        jsii.set(self, "priority", value)
 
     @builtins.property
-    @jsii.member(jsii_name="domain")
-    def domain(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "domain"))
+    @jsii.member(jsii_name="ttl")
+    def ttl(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "ttl"))
 
-    @domain.setter
-    def domain(self, value: builtins.str) -> None:
+    @ttl.setter
+    def ttl(self, value: jsii.Number) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__062d0fb1ae26591e344d3dc015d96e337a51de0b777d99d3aed344ea786f434c)
+            type_hints = typing.get_type_hints(_typecheckingstub__3603af1895942cf630c9aff4a47b8b54ef91d3494645e63f8fd3a45b03abac71)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "domain", value)
+        jsii.set(self, "ttl", value)
 
     @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "id"))
+    @jsii.member(jsii_name="type")
+    def type(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "type"))
+
+    @type.setter
+    def type(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d9e08ddeda5c9efacc235bb4e4cc9e67ae0afcff24519b271243136c4ab70b64)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "type", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="value")
+    def value(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "value"))
+
+    @value.setter
+    def value(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a403f4cc075ea8a1e1b15db31a1ee6fa785f954cdbe45635c0319e28b8925e7d)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "value", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="zoneName")
+    def zone_name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "zoneName"))
 
-    @id.setter
-    def id(self, value: builtins.str) -> None:
+    @zone_name.setter
+    def zone_name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b0cf9633ccc941cd5b0e1ce120f399991a0b5a082fd57425020668e4de62e1ae)
+            type_hints = typing.get_type_hints(_typecheckingstub__2bfd34b8808cbf746f55b3087f14c8dd7f9b763dcb625925499d978f15f42352)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
+        jsii.set(self, "zoneName", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-dnsimple.emailForward.EmailForwardConfig",
+    jsii_type="@cdktf/provider-dnsimple.zoneRecord.ZoneRecordConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
-        "alias_name": "aliasName",
-        "destination_email": "destinationEmail",
-        "domain": "domain",
-        "id": "id",
+        "name": "name",
+        "type": "type",
+        "value": "value",
+        "zone_name": "zoneName",
+        "priority": "priority",
+        "ttl": "ttl",
     },
 )
-class EmailForwardConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class ZoneRecordConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-        alias_name: builtins.str,
-        destination_email: builtins.str,
-        domain: builtins.str,
-        id: typing.Optional[builtins.str] = None,
+        name: builtins.str,
+        type: builtins.str,
+        value: builtins.str,
+        zone_name: builtins.str,
+        priority: typing.Optional[jsii.Number] = None,
+        ttl: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param alias_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.
-        :param destination_email: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.
-        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#id EmailForward#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#name ZoneRecord#name}.
+        :param type: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#type ZoneRecord#type}.
+        :param value: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#value ZoneRecord#value}.
+        :param zone_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#zone_name ZoneRecord#zone_name}.
+        :param priority: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#priority ZoneRecord#priority}.
+        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#ttl ZoneRecord#ttl}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7c6546ae8c4e2ee7d31438ac376a1ff2cb6b6c255b682e868b4941a86fc64016)
+            type_hints = typing.get_type_hints(_typecheckingstub__2eba6a2da1c8a28778529225bcbec0a1100d603698c12975ebeb143083f2fc0f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument alias_name", value=alias_name, expected_type=type_hints["alias_name"])
-            check_type(argname="argument destination_email", value=destination_email, expected_type=type_hints["destination_email"])
-            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+            check_type(argname="argument zone_name", value=zone_name, expected_type=type_hints["zone_name"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "alias_name": alias_name,
-            "destination_email": destination_email,
-            "domain": domain,
+            "name": name,
+            "type": type,
+            "value": value,
+            "zone_name": zone_name,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -244,16 +307,18 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
+        if priority is not None:
+            self._values["priority"] = priority
+        if ttl is not None:
+            self._values["ttl"] = ttl
 
     @builtins.property
     def connection(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
         '''
         :stability: experimental
@@ -310,115 +375,140 @@
         '''
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    def alias_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.'''
-        result = self._values.get("alias_name")
-        assert result is not None, "Required property 'alias_name' is missing"
+    def name(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#name ZoneRecord#name}.'''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def destination_email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.'''
-        result = self._values.get("destination_email")
-        assert result is not None, "Required property 'destination_email' is missing"
+    def type(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#type ZoneRecord#type}.'''
+        result = self._values.get("type")
+        assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def domain(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.'''
-        result = self._values.get("domain")
-        assert result is not None, "Required property 'domain' is missing"
+    def value(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#value ZoneRecord#value}.'''
+        result = self._values.get("value")
+        assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#id EmailForward#id}.
+    def zone_name(self) -> builtins.str:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#zone_name ZoneRecord#zone_name}.'''
+        result = self._values.get("zone_name")
+        assert result is not None, "Required property 'zone_name' is missing"
+        return typing.cast(builtins.str, result)
 
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[builtins.str], result)
+    @builtins.property
+    def priority(self) -> typing.Optional[jsii.Number]:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#priority ZoneRecord#priority}.'''
+        result = self._values.get("priority")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def ttl(self) -> typing.Optional[jsii.Number]:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#ttl ZoneRecord#ttl}.'''
+        result = self._values.get("ttl")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "EmailForwardConfig(%s)" % ", ".join(
+        return "ZoneRecordConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "EmailForward",
-    "EmailForwardConfig",
+    "ZoneRecord",
+    "ZoneRecordConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__b8786423bd640cbf734867c6903ef829c1bf2def3b03e9eb355e6581b375e104(
+def _typecheckingstub__17fe08f86dc04f40ad93499e2500792abbf08802751801af048d1c9ec1b18e9d(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
     *,
-    alias_name: builtins.str,
-    destination_email: builtins.str,
-    domain: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    name: builtins.str,
+    type: builtins.str,
+    value: builtins.str,
+    zone_name: builtins.str,
+    priority: typing.Optional[jsii.Number] = None,
+    ttl: typing.Optional[jsii.Number] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0c391f0f167e1ce785d68334af05b90de6e3c00eac6796e1415ee3de1557c959(
+def _typecheckingstub__c81d85039e11cc4da512fd0271fcb863f089e45607043af33c44e3620ff74418(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__aeee67e178fa004ade13e0235bc050e34e33ddb2371fd96be233943cc1ba2fe8(
+def _typecheckingstub__7a6ef6e36231aaee7590125559800d2d0edfca2e78b3043fee0f5f1f804de788(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3603af1895942cf630c9aff4a47b8b54ef91d3494645e63f8fd3a45b03abac71(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d9e08ddeda5c9efacc235bb4e4cc9e67ae0afcff24519b271243136c4ab70b64(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__062d0fb1ae26591e344d3dc015d96e337a51de0b777d99d3aed344ea786f434c(
+def _typecheckingstub__a403f4cc075ea8a1e1b15db31a1ee6fa785f954cdbe45635c0319e28b8925e7d(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b0cf9633ccc941cd5b0e1ce120f399991a0b5a082fd57425020668e4de62e1ae(
+def _typecheckingstub__2bfd34b8808cbf746f55b3087f14c8dd7f9b763dcb625925499d978f15f42352(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7c6546ae8c4e2ee7d31438ac376a1ff2cb6b6c255b682e868b4941a86fc64016(
+def _typecheckingstub__2eba6a2da1c8a28778529225bcbec0a1100d603698c12975ebeb143083f2fc0f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    alias_name: builtins.str,
-    destination_email: builtins.str,
-    domain: builtins.str,
-    id: typing.Optional[builtins.str] = None,
+    name: builtins.str,
+    type: builtins.str,
+    value: builtins.str,
+    zone_name: builtins.str,
+    priority: typing.Optional[jsii.Number] = None,
+    ttl: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py` & `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,59 +29,67 @@
     '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple dnsimple}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        account: builtins.str,
-        token: builtins.str,
+        account: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        token: typing.Optional[builtins.str] = None,
         user_agent: typing.Optional[builtins.str] = None,
     ) -> None:
         '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple dnsimple} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
         :param account: The account for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#account DnsimpleProvider#account}
-        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
         :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#alias DnsimpleProvider#alias}
         :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#prefetch DnsimpleProvider#prefetch}
         :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#sandbox DnsimpleProvider#sandbox}
+        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
         :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#user_agent DnsimpleProvider#user_agent}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e7ef56b7728822c45a23750e2602fff787208bfb71fa54a96467397e10a6e47c)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DnsimpleProviderConfig(
             account=account,
-            token=token,
             alias=alias,
             prefetch=prefetch,
             sandbox=sandbox,
+            token=token,
             user_agent=user_agent,
         )
 
         jsii.create(self.__class__, self, [scope, id, config])
 
+    @jsii.member(jsii_name="resetAccount")
+    def reset_account(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetAccount", []))
+
     @jsii.member(jsii_name="resetAlias")
     def reset_alias(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetAlias", []))
 
     @jsii.member(jsii_name="resetPrefetch")
     def reset_prefetch(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetPrefetch", []))
 
     @jsii.member(jsii_name="resetSandbox")
     def reset_sandbox(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSandbox", []))
 
+    @jsii.member(jsii_name="resetToken")
+    def reset_token(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetToken", []))
+
     @jsii.member(jsii_name="resetUserAgent")
     def reset_user_agent(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetUserAgent", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
@@ -209,80 +217,70 @@
 
 
 @jsii.data_type(
     jsii_type="@cdktf/provider-dnsimple.provider.DnsimpleProviderConfig",
     jsii_struct_bases=[],
     name_mapping={
         "account": "account",
-        "token": "token",
         "alias": "alias",
         "prefetch": "prefetch",
         "sandbox": "sandbox",
+        "token": "token",
         "user_agent": "userAgent",
     },
 )
 class DnsimpleProviderConfig:
     def __init__(
         self,
         *,
-        account: builtins.str,
-        token: builtins.str,
+        account: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+        token: typing.Optional[builtins.str] = None,
         user_agent: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param account: The account for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#account DnsimpleProvider#account}
-        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
         :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#alias DnsimpleProvider#alias}
         :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#prefetch DnsimpleProvider#prefetch}
         :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#sandbox DnsimpleProvider#sandbox}
+        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
         :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#user_agent DnsimpleProvider#user_agent}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__38b8bc1cdf1e0a8d7a730ac02381391ddfa090074fe8470d004c65b043c59d30)
             check_type(argname="argument account", value=account, expected_type=type_hints["account"])
-            check_type(argname="argument token", value=token, expected_type=type_hints["token"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument prefetch", value=prefetch, expected_type=type_hints["prefetch"])
             check_type(argname="argument sandbox", value=sandbox, expected_type=type_hints["sandbox"])
+            check_type(argname="argument token", value=token, expected_type=type_hints["token"])
             check_type(argname="argument user_agent", value=user_agent, expected_type=type_hints["user_agent"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "account": account,
-            "token": token,
-        }
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if account is not None:
+            self._values["account"] = account
         if alias is not None:
             self._values["alias"] = alias
         if prefetch is not None:
             self._values["prefetch"] = prefetch
         if sandbox is not None:
             self._values["sandbox"] = sandbox
+        if token is not None:
+            self._values["token"] = token
         if user_agent is not None:
             self._values["user_agent"] = user_agent
 
     @builtins.property
-    def account(self) -> builtins.str:
+    def account(self) -> typing.Optional[builtins.str]:
         '''The account for API operations.
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#account DnsimpleProvider#account}
         '''
         result = self._values.get("account")
-        assert result is not None, "Required property 'account' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def token(self) -> builtins.str:
-        '''The API v2 token for API operations.
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
-        '''
-        result = self._values.get("token")
-        assert result is not None, "Required property 'token' is missing"
-        return typing.cast(builtins.str, result)
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#alias DnsimpleProvider#alias}
         '''
@@ -308,14 +306,23 @@
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#sandbox DnsimpleProvider#sandbox}
         '''
         result = self._values.get("sandbox")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
+    def token(self) -> typing.Optional[builtins.str]:
+        '''The API v2 token for API operations.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
+        '''
+        result = self._values.get("token")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def user_agent(self) -> typing.Optional[builtins.str]:
         '''Custom string to append to the user agent used for sending HTTP requests to the API.
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#user_agent DnsimpleProvider#user_agent}
         '''
         result = self._values.get("user_agent")
         return typing.cast(typing.Optional[builtins.str], result)
@@ -339,19 +346,19 @@
 
 publication.publish()
 
 def _typecheckingstub__e7ef56b7728822c45a23750e2602fff787208bfb71fa54a96467397e10a6e47c(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    account: builtins.str,
-    token: builtins.str,
+    account: typing.Optional[builtins.str] = None,
     alias: typing.Optional[builtins.str] = None,
     prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    token: typing.Optional[builtins.str] = None,
     user_agent: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__be9c643fcd01fe5cf275169fcc97ae0d00374eb3d20c7266c6169c4c5dcb3d1a(
     value: typing.Optional[builtins.str],
@@ -387,16 +394,16 @@
     value: typing.Optional[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__38b8bc1cdf1e0a8d7a730ac02381391ddfa090074fe8470d004c65b043c59d30(
     *,
-    account: builtins.str,
-    token: builtins.str,
+    account: typing.Optional[builtins.str] = None,
     alias: typing.Optional[builtins.str] = None,
     prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
+    token: typing.Optional[builtins.str] = None,
     user_agent: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 3.0.3
+Version: 4.0.0
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-dnsimple-3.0.3/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 src/cdktf_cdktf_provider_dnsimple/py.typed
 src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
 src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
-src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@3.0.3.jsii.tgz
+src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
 src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
 src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
 src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
 src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
-src/cdktf_cdktf_provider_dnsimple/record/__init__.py
 src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
```

