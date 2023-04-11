# Comparing `tmp/types-Pygments-2.9.8.tar.gz` & `tmp/types-Pygments-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Pygments-2.9.8.tar", last modified: Mon Dec 27 18:21:08 2021, max compression
+gzip compressed data, was "types-Pygments-2.9.9.tar", last modified: Tue Dec 28 12:31:16 2021, max compression
```

## Comparing `types-Pygments-2.9.8.tar` & `types-Pygments-2.9.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 18:21:08.248747 types-Pygments-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      572 2021-12-27 18:21:07.000000 types-Pygments-2.9.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-27 18:21:07.000000 types-Pygments-2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-12-27 18:21:08.248747 types-Pygments-2.9.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 18:21:08.244747 types-Pygments-2.9.8/pygments-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-12-27 18:21:07.000000 types-Pygments-2.9.8/pygments-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/cmdline.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/console.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      644 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/filter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 18:21:08.244747 types-Pygments-2.9.8/pygments-stubs/filters/
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/filters/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      339 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 18:21:08.248747 types-Pygments-2.9.8/pygments-stubs/formatters/
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/_mapping.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/bbcode.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/html.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/img.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/irc.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      805 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/latex.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      646 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/other.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/pangomarkup.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/rtf.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      461 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/svg.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/terminal.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      947 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/formatters/terminal256.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/lexer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 18:21:08.248747 types-Pygments-2.9.8/pygments-stubs/lexers/
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/lexers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/modeline.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      704 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/regexopt.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/scanner.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/sphinxext.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/style.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 18:21:08.248747 types-Pygments-2.9.8/pygments-stubs/styles/
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/styles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      951 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/token.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/unistring.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2021-12-27 18:20:58.000000 types-Pygments-2.9.8/pygments-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-27 18:21:08.248747 types-Pygments-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2021-12-27 18:21:07.000000 types-Pygments-2.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 18:21:08.248747 types-Pygments-2.9.8/types_Pygments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-12-27 18:21:08.000000 types-Pygments-2.9.8/types_Pygments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-12-27 18:21:08.000000 types-Pygments-2.9.8/types_Pygments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-27 18:21:08.000000 types-Pygments-2.9.8/types_Pygments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-12-27 18:21:08.000000 types-Pygments-2.9.8/types_Pygments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-27 18:21:08.000000 types-Pygments-2.9.8/types_Pygments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:31:16.610998 types-Pygments-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-12-28 12:31:16.610998 types-Pygments-2.9.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:31:16.606998 types-Pygments-2.9.9/pygments-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/pygments-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/cmdline.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/console.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/filter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:31:16.610998 types-Pygments-2.9.9/pygments-stubs/filters/
+-rw-r--r--   0 runner    (1001) docker     (121)     2209 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/filters/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:31:16.610998 types-Pygments-2.9.9/pygments-stubs/formatters/
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/_mapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/bbcode.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1055 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/img.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/irc.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/latex.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/other.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/pangomarkup.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/rtf.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/svg.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/terminal.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/formatters/terminal256.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3072 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/lexer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:31:16.610998 types-Pygments-2.9.9/pygments-stubs/lexers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/lexers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/modeline.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/regexopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/scanner.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/sphinxext.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/style.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:31:16.610998 types-Pygments-2.9.9/pygments-stubs/styles/
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/styles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/token.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/unistring.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2021-12-28 12:29:14.000000 types-Pygments-2.9.9/pygments-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-28 12:31:16.610998 types-Pygments-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1820 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:31:16.610998 types-Pygments-2.9.9/types_Pygments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/types_Pygments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/types_Pygments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/types_Pygments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/types_Pygments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-28 12:31:16.000000 types-Pygments-2.9.9/types_Pygments.egg-info/top_level.txt
```

### Comparing `types-Pygments-2.9.8/CHANGELOG.md` & `types-Pygments-2.9.9/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.9.9 (2021-12-28)
+
+Use PEP 585 syntax wherever possible (#6717)
+
 ## 2.9.8 (2021-12-27)
 
 Always alias `collections.abc.Set` (#6712)
 
 ## 2.9.7 (2021-12-26)
 
 Annotate return type of pygments.plugin.iter_entry_points (#6697)
```

### Comparing `types-Pygments-2.9.8/PKG-INFO` & `types-Pygments-2.9.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pygments
-Version: 2.9.8
+Version: 2.9.9
 Summary: Typing stubs for Pygments
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `Pygments` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `Pygments`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/Pygments. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `14e5d16c3a2de82548ea583b525869c6d2b43d42`.
+This package was generated from typeshed commit `22bf9e8a787b38b1a0e193edd5b47119e43286ca`.
```

### Comparing `types-Pygments-2.9.8/pygments-stubs/filter.pyi` & `types-Pygments-2.9.9/pygments-stubs/filter.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/filters/__init__.pyi` & `types-Pygments-2.9.9/pygments-stubs/filters/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/formatters/__init__.pyi` & `types-Pygments-2.9.9/pygments-stubs/formatters/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/formatters/html.pyi` & `types-Pygments-2.9.9/pygments-stubs/formatters/html.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/formatters/img.pyi` & `types-Pygments-2.9.9/pygments-stubs/formatters/img.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/formatters/latex.pyi` & `types-Pygments-2.9.9/pygments-stubs/formatters/latex.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/formatters/other.pyi` & `types-Pygments-2.9.9/pygments-stubs/formatters/other.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/formatters/terminal256.pyi` & `types-Pygments-2.9.9/pygments-stubs/formatters/terminal256.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/lexer.pyi` & `types-Pygments-2.9.9/pygments-stubs/lexer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Iterable, Iterator, Sequence
-from typing import Any, Tuple
+from typing import Any
 
 from pygments.token import _TokenType
 from pygments.util import Future
 
 class LexerMeta(type):
     def __new__(cls, name, bases, d): ...
     def analyse_text(self, text) -> None: ...  # actually defined in class Lexer
@@ -36,15 +36,15 @@
     def get_tokens_unprocessed(self, text: str) -> Iterator[tuple[int, _TokenType, str]]: ...
 
 class include(str): ...
 class _inherit: ...
 
 inherit: Any
 
-class combined(Tuple[Any]):
+class combined(tuple[Any]):
     def __new__(cls, *args): ...
     def __init__(self, *args) -> None: ...
 
 class _PseudoMatch:
     def __init__(self, start, text) -> None: ...
     def start(self, arg: Any | None = ...): ...
     def end(self, arg: Any | None = ...): ...
```

### Comparing `types-Pygments-2.9.8/pygments-stubs/lexers/__init__.pyi` & `types-Pygments-2.9.9/pygments-stubs/lexers/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from _typeshed import StrOrBytesPath, StrPath
 from collections.abc import Iterator
-from typing import Any, Tuple, Union
+from typing import Any, Union
 
 from pygments.lexer import Lexer, LexerMeta
 
 _OpenFile = Union[StrOrBytesPath, int]  # copy/pasted from builtins.pyi
 
 # TODO: use lower-case tuple once mypy updated
-def get_all_lexers() -> Iterator[tuple[str, Tuple[str, ...], Tuple[str, ...], Tuple[str, ...]]]: ...
+def get_all_lexers() -> Iterator[tuple[str, tuple[str, ...], tuple[str, ...], tuple[str, ...]]]: ...
 def find_lexer_class(name: str) -> LexerMeta | None: ...
 def find_lexer_class_by_name(_alias: str) -> LexerMeta: ...
 def get_lexer_by_name(_alias: str, **options: Any) -> Lexer: ...
 def load_lexer_from_file(filename: _OpenFile, lexername: str = ..., **options: Any) -> Lexer: ...
 def find_lexer_class_for_filename(_fn: StrPath, code: str | bytes | None = ...) -> LexerMeta | None: ...
 def get_lexer_for_filename(_fn: StrPath, code: str | bytes | None = ..., **options: Any) -> Lexer: ...
 def get_lexer_for_mimetype(_mime: str, **options: Any) -> Lexer: ...
```

### Comparing `types-Pygments-2.9.8/pygments-stubs/plugin.pyi` & `types-Pygments-2.9.9/pygments-stubs/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/style.pyi` & `types-Pygments-2.9.9/pygments-stubs/style.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/pygments-stubs/token.pyi` & `types-Pygments-2.9.9/pygments-stubs/token.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections.abc import Mapping
-from typing import Tuple
 
-class _TokenType(Tuple[str]):  # TODO: change to lower-case tuple once new mypy released
+class _TokenType(tuple[str]):  # TODO: change to lower-case tuple once new mypy released
     parent: _TokenType | None
     def split(self) -> list[_TokenType]: ...
     subtypes: set[_TokenType]
     def __init__(self, *args: str) -> None: ...
     def __contains__(self, val: _TokenType) -> bool: ...  # type: ignore[override]
     def __getattr__(self, name: str) -> _TokenType: ...
     def __copy__(self): ...
```

### Comparing `types-Pygments-2.9.8/pygments-stubs/util.pyi` & `types-Pygments-2.9.9/pygments-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-Pygments-2.9.8/setup.py` & `types-Pygments-2.9.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `Pygments` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `Pygments`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/Pygments. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `14e5d16c3a2de82548ea583b525869c6d2b43d42`.
+This package was generated from typeshed commit `22bf9e8a787b38b1a0e193edd5b47119e43286ca`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.9.8",
+      version="2.9.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       install_requires=['types-docutils', 'types-setuptools'],
       packages=['pygments-stubs'],
       package_data={'pygments-stubs': ['__init__.pyi', 'cmdline.pyi', 'console.pyi', 'filter.pyi', 'filters/__init__.pyi', 'formatter.pyi', 'formatters/__init__.pyi', 'formatters/_mapping.pyi', 'formatters/bbcode.pyi', 'formatters/html.pyi', 'formatters/img.pyi', 'formatters/irc.pyi', 'formatters/latex.pyi', 'formatters/other.pyi', 'formatters/pangomarkup.pyi', 'formatters/rtf.pyi', 'formatters/svg.pyi', 'formatters/terminal.pyi', 'formatters/terminal256.pyi', 'lexer.pyi', 'lexers/__init__.pyi', 'modeline.pyi', 'plugin.pyi', 'regexopt.pyi', 'scanner.pyi', 'sphinxext.pyi', 'style.pyi', 'styles/__init__.pyi', 'token.pyi', 'unistring.pyi', 'util.pyi', 'METADATA.toml']},
```

### Comparing `types-Pygments-2.9.8/types_Pygments.egg-info/PKG-INFO` & `types-Pygments-2.9.9/types_Pygments.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pygments
-Version: 2.9.8
+Version: 2.9.9
 Summary: Typing stubs for Pygments
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `Pygments` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `Pygments`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/Pygments. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `14e5d16c3a2de82548ea583b525869c6d2b43d42`.
+This package was generated from typeshed commit `22bf9e8a787b38b1a0e193edd5b47119e43286ca`.
```

### Comparing `types-Pygments-2.9.8/types_Pygments.egg-info/SOURCES.txt` & `types-Pygments-2.9.9/types_Pygments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

