# Comparing `tmp/brds-0.2.8.tar.gz` & `tmp/brds-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.2.8.tar", last modified: Mon Apr 10 21:58:53 2023, max compression
+gzip compressed data, was "brds-0.3.0.tar", last modified: Tue Apr 11 18:45:26 2023, max compression
```

## Comparing `brds-0.2.8.tar` & `brds-0.3.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 21:58:43.000000 brds-0.2.8/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-10 21:58:43.000000 brds-0.2.8/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:58:43.000000 brds-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 21:58:43.000000 brds-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:58:53.191722 brds-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-10 21:58:43.000000 brds-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.187722 brds-0.2.8/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:58:43.000000 brds-0.2.8/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-10 21:58:43.000000 brds-0.2.8/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-10 21:58:43.000000 brds-0.2.8/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-10 21:58:43.000000 brds-0.2.8/brds/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-10 21:58:43.000000 brds-0.2.8/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-10 21:58:43.000000 brds-0.2.8/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.187722 brds-0.2.8/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.187722 brds-0.2.8/brds/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/datasets/dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/datasets/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/datasets/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 21:58:43.000000 brds-0.2.8/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/humanize/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 21:58:43.000000 brds-0.2.8/brds/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 21:58:43.000000 brds-0.2.8/brds/humanize/sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:43.000000 brds-0.2.8/brds/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/brds/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 21:58:43.000000 brds-0.2.8/brds/templates/dataset_files.html
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-10 21:58:43.000000 brds-0.2.8/brds/templates/datasets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.187722 brds-0.2.8/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 21:58:53.000000 brds-0.2.8/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:58:53.191722 brds-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-10 21:58:43.000000 brds-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:53.191722 brds-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:58:43.000000 brds-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 21:58:43.000000 brds-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 21:58:43.000000 brds-0.2.8/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-11 18:45:13.000000 brds-0.3.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-11 18:45:13.000000 brds-0.3.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 18:45:13.000000 brds-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 18:45:13.000000 brds-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-11 18:45:26.874451 brds-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-11 18:45:13.000000 brds-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.870451 brds-0.3.0/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 18:45:13.000000 brds-0.3.0/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-11 18:45:13.000000 brds-0.3.0/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-11 18:45:13.000000 brds-0.3.0/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-11 18:45:13.000000 brds-0.3.0/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-11 18:45:13.000000 brds-0.3.0/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 18:45:13.000000 brds-0.3.0/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 18:45:13.000000 brds-0.3.0/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-11 18:45:13.000000 brds-0.3.0/brds/humanize/sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:13.000000 brds-0.3.0/brds/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-11 18:45:13.000000 brds-0.3.0/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 18:45:13.000000 brds-0.3.0/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.870451 brds-0.3.0/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:45:26.874451 brds-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-11 18:45:13.000000 brds-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:13.000000 brds-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-11 18:45:13.000000 brds-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 18:45:13.000000 brds-0.3.0/tests/test_base.py
```

### Comparing `brds-0.2.8/HISTORY.md` & `brds-0.3.0/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Release: version 0..0 🚀 [brahle]
+- Preventing exploits. [brahle]
+
+
+0.2.8 (2023-04-10)
+------------------
+- Release: version 0.2.8 🚀 [brahle]
 - Also tagging the version from the ref. [brahle]
 
 
 0.2.7 (2023-04-10)
 ------------------
 - Release: version 0.2.7 🚀 [brahle]
 - Fixing the publishing. [brahle]
```

### Comparing `brds-0.2.8/LICENSE` & `brds-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/PKG-INFO` & `brds-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.8
+Version: 0.3.0
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.8/brds/__init__.py` & `brds-0.3.0/brds/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     find,
     find_and_replace,
     find_and_replacer,
     finder,
     fload,
     get_dataset_files,
     get_logger,
+    get_safe_path,
     list_datasets,
     reader_folder_path,
     replace,
     replacer,
     root_folder_path,
     set_logging_to_debug,
     set_logging_to_info,
@@ -38,14 +39,15 @@
     "find_and_replacer",
     "find",
     "FindCallBack",
     "finder",
     "fload",
     "get_dataset_files",
     "get_logger",
+    "get_safe_path",
     "GunzipImporter",
     "Importer",
     "list_datasets",
     "reader_folder_path",
     "replace",
     "Replacement",
     "replacer",
```

### Comparing `brds-0.2.8/brds/app.py` & `brds-0.3.0/brds/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,64 @@
-from pathlib import Path as _Path
+from os.path import isfile
 from typing import Any, Dict
 
 import pandas as pd
 from fastapi import FastAPI, HTTPException, Path, Request, Response
 from fastapi.responses import FileResponse, HTMLResponse
 from fastapi.templating import Jinja2Templates
 
-from brds import fload, get_dataset_files, list_datasets, reader_folder_path
+from brds import fload, get_dataset_files, list_datasets, get_safe_path
 
 app = FastAPI()
 
 templates = Jinja2Templates(directory="./brds/templates")
 
 
 @app.get("/dictionary/{filename:path}")
 async def read_as_dict(filename: str = Path(..., regex=r"[\w\-/]+")) -> Dict[str, Any]:
     try:
-        df = fload(filename)
+        df = fload(str(get_safe_path(filename)))
         return df.to_dict(orient="records")
     except FileNotFoundError as exc:
         raise HTTPException(status_code=404, detail=f"Parquet file '{filename}' not found") from exc
 
 
 @app.get("/raw/{filename:path}")
 async def read_raw(filename: str = Path(..., regex=r"[\w\-/]+")) -> Dict[str, Any]:
     try:
-        df = fload(filename)
+        df = fload(str(get_safe_path(filename)))
         return df.to_dict(orient="records")
     except FileNotFoundError as exc:
         raise HTTPException(status_code=404, detail=f"Parquet file '{filename}' not found") from exc
 
 
 @app.get("/html/{filename:path}", response_class=HTMLResponse)
 async def read_html(filename: str = Path(..., regex=r"[\w\-/]+")) -> str:
     try:
-        df: pd.DataFrame = fload(filename)
+        df: pd.DataFrame = fload(str(get_safe_path(filename)))
         return df.to_html()
     except FileNotFoundError as exc:
         raise HTTPException(status_code=404, detail=f"Parquet file '{filename}' not found") from exc
 
 
 @app.get("/datasets", response_class=HTMLResponse)
 async def get_datasets(request: Request) -> Response:
     datasets = list_datasets()
     return templates.TemplateResponse("datasets.html", {"request": request, "modules": datasets})
 
 
 @app.get("/download/{path:path}", response_class=FileResponse)
 async def download_file(path: str):
-    root = _Path(reader_folder_path())
-    return FileResponse(root.joinpath(path), filename=path.split("/")[-1], media_type="application/octet-stream")
+    safe_path = get_safe_path(path)
+
+    if not isfile(safe_path):
+        raise HTTPException(status_code=404, detail="File not found")
+
+    return FileResponse(safe_path, filename=path.split("/")[-1], media_type="application/octet-stream")
 
 
 @app.get("/dataset/{dataset_name:path}", response_class=HTMLResponse)
 async def dataset_files(request: Request, dataset_name: str):
-    grouped_files = get_dataset_files(dataset_name)  # Implement this function to return grouped files
+    grouped_files = get_dataset_files(str(get_safe_path(dataset_name)))
     return templates.TemplateResponse(
         "dataset_files.html", {"request": request, "dataset_name": dataset_name, "grouped_files": grouped_files}
     )
```

### Comparing `brds-0.2.8/brds/cli.py` & `brds-0.3.0/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/__init__.py` & `brds-0.3.0/brds/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     replacer,
 )
 from .environment import reader_folder_path, root_folder_path, vault_token, writer_folder_path
 from .fetch import Fetcher
 from .fs import FileReader, FileWriter, fload
 from .importer import GunzipImporter, Importer
 from .logger import get_logger, set_logging_to_debug, set_logging_to_info, set_logging_to_warn
+from .security import get_safe_path
 from .vault import Vault
 
 __all__ = [
     "DatasetInfo",
     "ExactMatch",
     "Fetcher",
     "FileReader",
@@ -27,14 +28,15 @@
     "find_and_replacer",
     "find",
     "FindCallBack",
     "finder",
     "fload",
     "get_dataset_files",
     "get_logger",
+    "get_safe_path",
     "GunzipImporter",
     "Importer",
     "list_datasets",
     "reader_folder_path",
     "replace",
     "Replacement",
     "replacer",
```

### Comparing `brds-0.2.8/brds/core/datasets/dataset_files.py` & `brds-0.3.0/brds/core/datasets/dataset_files.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/datasets/dataset_info.py` & `brds-0.3.0/brds/core/datasets/dataset_info.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/datasets/list_datasets.py` & `brds-0.3.0/brds/core/datasets/list_datasets.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/edit.py` & `brds-0.3.0/brds/core/edit.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/environment.py` & `brds-0.3.0/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/fetch/fetcher.py` & `brds-0.3.0/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/fs/reader.py` & `brds-0.3.0/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/fs/writer.py` & `brds-0.3.0/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/importer/gunizp_importer.py` & `brds-0.3.0/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/core/logger.py` & `brds-0.3.0/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/humanize/sizes.py` & `brds-0.3.0/brds/humanize/sizes.py`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/templates/dataset_files.html` & `brds-0.3.0/brds/templates/dataset_files.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds/templates/datasets.html` & `brds-0.3.0/brds/templates/datasets.html`

 * *Files identical despite different names*

### Comparing `brds-0.2.8/brds.egg-info/PKG-INFO` & `brds-0.3.0/brds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.2.8
+Version: 0.3.0
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `brds-0.2.8/brds.egg-info/SOURCES.txt` & `brds-0.3.0/brds.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 brds.egg-info/entry_points.txt
 brds.egg-info/requires.txt
 brds.egg-info/top_level.txt
 brds/core/__init__.py
 brds/core/edit.py
 brds/core/environment.py
 brds/core/logger.py
+brds/core/security.py
 brds/core/vault.py
 brds/core/datasets/__init__.py
 brds/core/datasets/dataset_files.py
 brds/core/datasets/dataset_info.py
 brds/core/datasets/list_datasets.py
 brds/core/fetch/__init__.py
 brds/core/fetch/fetcher.py
```

### Comparing `brds-0.2.8/setup.py` & `brds-0.3.0/setup.py`

 * *Files identical despite different names*

