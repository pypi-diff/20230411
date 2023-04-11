# Comparing `tmp/mypy-boto3-ecr-public-1.26.111.tar.gz` & `tmp/mypy-boto3-ecr-public-1.26.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-public-1.26.111.tar", last modified: Tue Apr 11 21:32:35 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-public-1.26.46.tar", last modified: Mon Jan  9 20:27:39 2023, max compression
```

## Comparing `mypy-boto3-ecr-public-1.26.111.tar` & `mypy-boto3-ecr-public-1.26.46.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:32:35.046949 mypy-boto3-ecr-public-1.26.111/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-11 21:32:35.046949 mypy-boto3-ecr-public-1.26.111/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:32:35.046949 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-11 21:32:10.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-04-11 21:32:10.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-04-11 21:32:10.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:32:35.046949 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-11 21:32:34.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-11 21:32:34.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:32:34.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:32:34.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 21:32:34.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 21:32:34.000000 mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:32:35.070949 mypy-boto3-ecr-public-1.26.111/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-11 21:32:09.000000 mypy-boto3-ecr-public-1.26.111/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.312431 mypy-boto3-ecr-public-1.26.46/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-01-09 20:27:39.312431 mypy-boto3-ecr-public-1.26.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.308431 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-01-09 20:27:24.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.312431 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-09 20:27:39.000000 mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 20:27:39.312431 mypy-boto3-ecr-public-1.26.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-09 20:27:23.000000 mypy-boto3-ecr-public-1.26.46/setup.py
```

### Comparing `mypy-boto3-ecr-public-1.26.111/LICENSE` & `mypy-boto3-ecr-public-1.26.46/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-ecr-public-1.26.111/PKG-INFO` & `mypy-boto3-ecr-public-1.26.46/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.26.111
-Summary: Type annotations for boto3.ECRPublic 1.26.111 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.46
+Summary: Type annotations for boto3.ECRPublic 1.26.46 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.26.111](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,42 +417,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-ecr-public-1.26.111/README.md` & `mypy-boto3-ecr-public-1.26.46/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.26.111](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,42 +385,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/__init__.py` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/__init__.pyi` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/__main__.py` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECRPublic 1.26.111\nVersion:         1.26.111\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ECRPublic 1.26.46\nVersion:         1.26.46\nBuilder version:"
+        " 7.12.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.111")
+    print("1.26.46")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/client.py` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/client.pyi` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/literals.py` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,26 +92,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -197,15 +195,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -216,15 +213,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -375,20 +371,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/literals.pyi` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -90,26 +90,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -195,15 +193,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -214,15 +211,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -373,20 +369,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/paginator.py` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/paginator.pyi` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/type_defs.py` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public/type_defs.pyi` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/PKG-INFO` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.26.111
-Summary: Type annotations for boto3.ECRPublic 1.26.111 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.46
+Summary: Type annotations for boto3.ECRPublic 1.26.46 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ecr-public"></a>
 
 # mypy-boto3-ecr-public
 
 [![PyPI - mypy-boto3-ecr-public](https://img.shields.io/pypi/v/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr-public.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr-public)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr-public?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECRPublic 1.26.111](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[boto3.ECRPublic 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,42 +417,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-ecr-public-1.26.111/mypy_boto3_ecr_public.egg-info/SOURCES.txt` & `mypy-boto3-ecr-public-1.26.46/mypy_boto3_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.26.111/setup.py` & `mypy-boto3-ecr-public-1.26.46/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-ecr-public.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-ecr-public",
-    version="1.26.111",
+    version="1.26.46",
     packages=["mypy_boto3_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECRPublic 1.26.111 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ECRPublic 1.26.46 service generated with mypy-boto3-builder"
+        " 7.12.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

