# Comparing `tmp/autoresearcher-0.0.1.tar.gz` & `tmp/autoresearcher-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoresearcher-0.0.1.tar", last modified: Tue Apr 11 01:49:01 2023, max compression
+gzip compressed data, was "autoresearcher-0.0.4.tar", last modified: Tue Apr 11 03:31:22 2023, max compression
```

## Comparing `autoresearcher-0.0.1.tar` & `autoresearcher-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 01:49:01.104506 autoresearcher-0.0.1/
--rw-r--r--   0 marapelzer   (501) staff       (20)     1070 2023-04-11 00:23:06.000000 autoresearcher-0.0.1/LICENSE
--rw-r--r--   0 marapelzer   (501) staff       (20)      451 2023-04-11 01:49:01.104648 autoresearcher-0.0.1/PKG-INFO
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 01:49:01.096218 autoresearcher-0.0.1/autoresearcher/
--rw-r--r--   0 marapelzer   (501) staff       (20)       77 2023-04-11 00:38:30.000000 autoresearcher-0.0.1/autoresearcher/__init__.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 01:49:01.099615 autoresearcher-0.0.1/autoresearcher/data_sources/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.1/autoresearcher/data_sources/__init__.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 01:49:01.101517 autoresearcher-0.0.1/autoresearcher/data_sources/web_apis/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.1/autoresearcher/data_sources/web_apis/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)      585 2023-04-10 23:32:56.000000 autoresearcher-0.0.1/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     1813 2023-04-11 01:34:10.000000 autoresearcher-0.0.1/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 01:49:01.103870 autoresearcher-0.0.1/autoresearcher/utils/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.1/autoresearcher/utils/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)      366 2023-04-10 23:32:56.000000 autoresearcher-0.0.1/autoresearcher/utils/get_citations.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     1632 2023-04-11 01:04:12.000000 autoresearcher-0.0.1/autoresearcher/utils/prompts.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 01:49:01.099265 autoresearcher-0.0.1/autoresearcher.egg-info/
--rw-r--r--   0 marapelzer   (501) staff       (20)      451 2023-04-11 01:49:01.000000 autoresearcher-0.0.1/autoresearcher.egg-info/PKG-INFO
--rw-r--r--   0 marapelzer   (501) staff       (20)      569 2023-04-11 01:49:01.000000 autoresearcher-0.0.1/autoresearcher.egg-info/SOURCES.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)        1 2023-04-11 01:49:01.000000 autoresearcher-0.0.1/autoresearcher.egg-info/dependency_links.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)       88 2023-04-11 01:49:01.000000 autoresearcher-0.0.1/autoresearcher.egg-info/requires.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)       15 2023-04-11 01:49:01.000000 autoresearcher-0.0.1/autoresearcher.egg-info/top_level.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)      103 2023-04-11 00:17:53.000000 autoresearcher-0.0.1/pyproject.toml
--rw-r--r--   0 marapelzer   (501) staff       (20)      654 2023-04-11 01:49:01.105203 autoresearcher-0.0.1/setup.cfg
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.797149 autoresearcher-0.0.4/
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1070 2023-04-11 00:23:06.000000 autoresearcher-0.0.4/LICENSE
+-rw-r--r--   0 marapelzer   (501) staff       (20)     2970 2023-04-11 03:31:22.796484 autoresearcher-0.0.4/PKG-INFO
+-rw-r--r--   0 marapelzer   (501) staff       (20)     2518 2023-04-11 03:30:54.000000 autoresearcher-0.0.4/README.md
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.789309 autoresearcher-0.0.4/autoresearcher/
+-rw-r--r--   0 marapelzer   (501) staff       (20)       77 2023-04-11 00:38:30.000000 autoresearcher-0.0.4/autoresearcher/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.791559 autoresearcher-0.0.4/autoresearcher/data_sources/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/data_sources/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.792911 autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)      585 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1813 2023-04-11 01:34:10.000000 autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.794117 autoresearcher-0.0.4/autoresearcher/utils/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/utils/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)      366 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/utils/get_citations.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1632 2023-04-11 01:04:12.000000 autoresearcher-0.0.4/autoresearcher/utils/prompts.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.795088 autoresearcher-0.0.4/autoresearcher/workflows/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 02:08:49.000000 autoresearcher-0.0.4/autoresearcher/workflows/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.795546 autoresearcher-0.0.4/autoresearcher/workflows/literature_review/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/workflows/literature_review/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     5262 2023-04-10 23:32:56.000000 autoresearcher-0.0.4/autoresearcher/workflows/literature_review/literature_review.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:31:22.791278 autoresearcher-0.0.4/autoresearcher.egg-info/
+-rw-r--r--   0 marapelzer   (501) staff       (20)     2970 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/PKG-INFO
+-rw-r--r--   0 marapelzer   (501) staff       (20)      734 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/SOURCES.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)        1 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/dependency_links.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)      109 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/requires.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)       15 2023-04-11 03:31:22.000000 autoresearcher-0.0.4/autoresearcher.egg-info/top_level.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)      103 2023-04-11 00:17:53.000000 autoresearcher-0.0.4/pyproject.toml
+-rw-r--r--   0 marapelzer   (501) staff       (20)       38 2023-04-11 03:31:22.797276 autoresearcher-0.0.4/setup.cfg
+-rw-r--r--   0 marapelzer   (501) staff       (20)      935 2023-04-11 03:31:12.000000 autoresearcher-0.0.4/setup.py
```

### Comparing `autoresearcher-0.0.1/LICENSE` & `autoresearcher-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.1/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py` & `autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.1/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py` & `autoresearcher-0.0.4/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.1/autoresearcher/utils/prompts.py` & `autoresearcher-0.0.4/autoresearcher/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.1/autoresearcher.egg-info/SOURCES.txt` & `autoresearcher-0.0.4/autoresearcher.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 LICENSE
+README.md
 pyproject.toml
-setup.cfg
+setup.py
 autoresearcher/__init__.py
 autoresearcher.egg-info/PKG-INFO
 autoresearcher.egg-info/SOURCES.txt
 autoresearcher.egg-info/dependency_links.txt
 autoresearcher.egg-info/requires.txt
 autoresearcher.egg-info/top_level.txt
 autoresearcher/data_sources/__init__.py
 autoresearcher/data_sources/web_apis/__init__.py
 autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
 autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
 autoresearcher/utils/__init__.py
 autoresearcher/utils/get_citations.py
-autoresearcher/utils/prompts.py
+autoresearcher/utils/prompts.py
+autoresearcher/workflows/__init__.py
+autoresearcher/workflows/literature_review/__init__.py
+autoresearcher/workflows/literature_review/literature_review.py
```

