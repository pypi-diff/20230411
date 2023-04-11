# Comparing `tmp/mypy-boto3-wafv2-1.26.73.tar.gz` & `tmp/mypy-boto3-wafv2-1.26.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wafv2-1.26.73.tar", last modified: Thu Feb 16 20:47:25 2023, max compression
+gzip compressed data, was "mypy-boto3-wafv2-1.26.78.tar", last modified: Thu Feb 23 20:34:58 2023, max compression
```

## Comparing `mypy-boto3-wafv2-1.26.73.tar` & `mypy-boto3-wafv2-1.26.78.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.431042 mypy-boto3-wafv2-1.26.73/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-02-16 20:47:25.431042 mypy-boto3-wafv2-1.26.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.431042 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33744 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33690 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-02-16 20:47:13.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-02-16 20:47:13.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60400 2023-02-16 20:47:15.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60325 2023-02-16 20:47:14.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.431042 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-02-16 20:47:25.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-16 20:47:25.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-16 20:47:25.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-16 20:47:25.000000 mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 20:47:25.431042 mypy-boto3-wafv2-1.26.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-16 20:47:12.000000 mypy-boto3-wafv2-1.26.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33744 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33690 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-02-23 20:34:46.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-02-23 20:34:46.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60400 2023-02-23 20:34:47.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60325 2023-02-23 20:34:47.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-23 20:34:58.000000 mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:58.732411 mypy-boto3-wafv2-1.26.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-23 20:34:45.000000 mypy-boto3-wafv2-1.26.78/setup.py
```

### Comparing `mypy-boto3-wafv2-1.26.73/LICENSE` & `mypy-boto3-wafv2-1.26.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.26.73/PKG-INFO` & `mypy-boto3-wafv2-1.26.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.26.73
-Summary: Type annotations for boto3.WAFV2 1.26.73 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.78
+Summary: Type annotations for boto3.WAFV2 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wafv2-1.26.73/README.md` & `mypy-boto3-wafv2-1.26.78/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/__main__.py` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFV2 1.26.73\nVersion:         1.26.73\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.WAFV2 1.26.78\nVersion:         1.26.78\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.73")
+    print("1.26.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/client.py` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/client.pyi` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/literals.py` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,15 +322,15 @@
 PayloadTypeType = Literal["FORM_ENCODED", "JSON"]
 PlatformType = Literal["ANDROID", "IOS"]
 PositionalConstraintType = Literal[
     "CONTAINS", "CONTAINS_WORD", "ENDS_WITH", "EXACTLY", "STARTS_WITH"
 ]
 RateBasedStatementAggregateKeyTypeType = Literal["FORWARDED_IP", "IP"]
 ResourceTypeType = Literal[
-    "API_GATEWAY", "APPLICATION_LOAD_BALANCER", "APPSYNC", "COGNITO_USER_POOL"
+    "API_GATEWAY", "APPLICATION_LOAD_BALANCER", "APPSYNC", "APP_RUNNER_SERVICE", "COGNITO_USER_POOL"
 ]
 ResponseContentTypeType = Literal["APPLICATION_JSON", "TEXT_HTML", "TEXT_PLAIN"]
 ScopeType = Literal["CLOUDFRONT", "REGIONAL"]
 SensitivityLevelType = Literal["HIGH", "LOW"]
 TextTransformationTypeType = Literal[
     "BASE64_DECODE",
     "BASE64_DECODE_EXT",
@@ -675,14 +675,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/literals.pyi` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -320,15 +320,15 @@
 PayloadTypeType = Literal["FORM_ENCODED", "JSON"]
 PlatformType = Literal["ANDROID", "IOS"]
 PositionalConstraintType = Literal[
     "CONTAINS", "CONTAINS_WORD", "ENDS_WITH", "EXACTLY", "STARTS_WITH"
 ]
 RateBasedStatementAggregateKeyTypeType = Literal["FORWARDED_IP", "IP"]
 ResourceTypeType = Literal[
-    "API_GATEWAY", "APPLICATION_LOAD_BALANCER", "APPSYNC", "COGNITO_USER_POOL"
+    "API_GATEWAY", "APPLICATION_LOAD_BALANCER", "APPSYNC", "APP_RUNNER_SERVICE", "COGNITO_USER_POOL"
 ]
 ResponseContentTypeType = Literal["APPLICATION_JSON", "TEXT_HTML", "TEXT_PLAIN"]
 ScopeType = Literal["CLOUDFRONT", "REGIONAL"]
 SensitivityLevelType = Literal["HIGH", "LOW"]
 TextTransformationTypeType = Literal[
     "BASE64_DECODE",
     "BASE64_DECODE_EXT",
@@ -673,14 +673,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/type_defs.py` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1074,15 +1074,15 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": "StatementTypeDef",
+        "Statement": Dict[str, Any],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
@@ -1535,15 +1535,15 @@
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
 _OptionalRateBasedStatementTypeDef = TypedDict(
     "_OptionalRateBasedStatementTypeDef",
     {
-        "ScopeDownStatement": Dict[str, Any],
+        "ScopeDownStatement": "StatementTypeDef",
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
 
 class RateBasedStatementTypeDef(
```

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2/type_defs.pyi` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1045,15 +1045,15 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": "StatementTypeDef",
+        "Statement": Dict[str, Any],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
@@ -1496,15 +1496,15 @@
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
 _OptionalRateBasedStatementTypeDef = TypedDict(
     "_OptionalRateBasedStatementTypeDef",
     {
-        "ScopeDownStatement": Dict[str, Any],
+        "ScopeDownStatement": "StatementTypeDef",
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
 class RateBasedStatementTypeDef(
     _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
```

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/PKG-INFO` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.26.73
-Summary: Type annotations for boto3.WAFV2 1.26.73 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.78
+Summary: Type annotations for boto3.WAFV2 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wafv2-1.26.73/mypy_boto3_wafv2.egg-info/SOURCES.txt` & `mypy-boto3-wafv2-1.26.78/mypy_boto3_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.26.73/setup.py` & `mypy-boto3-wafv2-1.26.78/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-wafv2",
-    version="1.26.73",
+    version="1.26.78",
     packages=["mypy_boto3_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFV2 1.26.73 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.WAFV2 1.26.78 service generated with mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

