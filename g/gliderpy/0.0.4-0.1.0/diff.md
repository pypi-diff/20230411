# Comparing `tmp/gliderpy-0.0.4.tar.gz` & `tmp/gliderpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliderpy-0.0.4.tar", last modified: Wed Aug 18 12:24:34 2021, max compression
+gzip compressed data, was "gliderpy-0.1.0.tar", last modified: Tue Apr 11 19:24:59 2023, max compression
```

## Comparing `gliderpy-0.0.4.tar` & `gliderpy-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 12:24:34.372705 gliderpy-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 12:24:34.372705 gliderpy-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 12:24:34.372705 gliderpy-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-08-18 12:24:19.000000 gliderpy-0.0.4/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-08-18 12:24:19.000000 gliderpy-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-08-18 12:24:19.000000 gliderpy-0.0.4/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2021-08-18 12:24:19.000000 gliderpy-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2021-08-18 12:24:19.000000 gliderpy-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      245 2021-08-18 12:24:19.000000 gliderpy-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2021-08-18 12:24:34.372705 gliderpy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-08-18 12:24:19.000000 gliderpy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 12:24:34.372705 gliderpy-0.0.4/gliderpy/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-08-18 12:24:19.000000 gliderpy-0.0.4/gliderpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5518 2021-08-18 12:24:19.000000 gliderpy-0.0.4/gliderpy/fetchers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-08-18 12:24:19.000000 gliderpy-0.0.4/gliderpy/plotters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2796 2021-08-18 12:24:19.000000 gliderpy-0.0.4/gliderpy/servers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 12:24:34.372705 gliderpy-0.0.4/gliderpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-08-18 12:24:34.000000 gliderpy-0.0.4/gliderpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-08-18 12:24:19.000000 gliderpy-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-08-18 12:24:19.000000 gliderpy-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-08-18 12:24:19.000000 gliderpy-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-08-18 12:24:34.372705 gliderpy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-08-18 12:24:19.000000 gliderpy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:24:59.888931 gliderpy-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:24:59.884931 gliderpy-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-11 19:24:49.000000 gliderpy-0.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:24:59.888931 gliderpy-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-11 19:24:49.000000 gliderpy-0.1.0/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-11 19:24:49.000000 gliderpy-0.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-11 19:24:49.000000 gliderpy-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 19:24:49.000000 gliderpy-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-11 19:24:49.000000 gliderpy-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-11 19:24:49.000000 gliderpy-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-11 19:24:59.888931 gliderpy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-11 19:24:49.000000 gliderpy-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:24:59.888931 gliderpy-0.1.0/gliderpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 19:24:49.000000 gliderpy-0.1.0/gliderpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-11 19:24:49.000000 gliderpy-0.1.0/gliderpy/fetchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-11 19:24:49.000000 gliderpy-0.1.0/gliderpy/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-11 19:24:49.000000 gliderpy-0.1.0/gliderpy/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:24:59.888931 gliderpy-0.1.0/gliderpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 19:24:59.000000 gliderpy-0.1.0/gliderpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-11 19:24:49.000000 gliderpy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-11 19:24:49.000000 gliderpy-0.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 19:24:49.000000 gliderpy-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:24:59.888931 gliderpy-0.1.0/setup.cfg
```

### Comparing `gliderpy-0.0.4/.github/workflows/publish.yml` & `gliderpy-0.1.0/.github/workflows/pypi.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 name: Publish to PyPI
 
 on:
+  pull_request:
+  push:
+    branches:
+      - main
   release:
     types:
       - published
 
+defaults:
+  run:
+    shell: bash
+
 jobs:
   packages:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.x
+        python-version: "3.x"
 
     - name: Get tags
       run: git fetch --depth=1 origin +refs/tags/*:refs/tags/*
-      shell: bash
 
     - name: Install build tools
       run: |
-        python -m pip install --upgrade pip wheel setuptools setuptools_scm build twine
-      shell: bash
+        python -m pip install --upgrade build
 
     - name: Build binary wheel
       run: python -m build --sdist --wheel . --outdir dist
 
     - name: CheckFiles
       run: |
         ls dist
-      shell: bash
-    - name: Test version
-      run: |
-        if [[ $(python setup.py --version) == "0.0.0" ]]; then
-          exit 1
-        fi
-      shell: bash
+        python -m pip install --upgrade check-manifest
+        check-manifest --verbose
+
     - name: Test wheels
       run: |
-        cd dist && python -m pip install gliderpy*.whl
+        cd dist && python -m pip install *.whl
+        python -m pip install --upgrade build twine
         python -m twine check *
-      shell: bash
 
     - name: Publish a Python distribution to PyPI
-      uses: pypa/gh-action-pypi-publish@master
+      if: success() && github.event_name == 'release'
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `gliderpy-0.0.4/.pre-commit-config.yaml` & `gliderpy-0.1.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 repos:
-
-- repo: https://github.com/econchick/interrogate
-  rev: 1.3.2
-  hooks:
-    - id: interrogate
-      exclude: ^(docs|setup.py|gliderpy/__init__.py|tests)
-      args: [--config=pyproject.toml]
-
-- repo: https://github.com/keewis/blackdoc
-  rev: v0.3.4
-  hooks:
-    - id: blackdoc
-
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v3.3.0
+  rev: v4.4.0
   hooks:
     - id: trailing-whitespace
-      exclude: tests/data
     - id: check-ast
     - id: debug-statements
     - id: end-of-file-fixer
-      exclude: github_deploy_key_ioos_gliderpy.enc
     - id: check-docstring-first
     - id: check-added-large-files
+      exclude_types: [yaml]
     - id: requirements-txt-fixer
     - id: file-contents-sorter
       files: requirements-dev.txt
 
-- repo: https://gitlab.com/pycqa/flake8
-  rev: 3.8.4
-  hooks:
-    - id: flake8
-      exclude: docs/source/conf.py
-      args: [--max-line-length=105]
-
-- repo: https://github.com/pre-commit/mirrors-isort
-  rev: v5.9.2
-  hooks:
-  - id: isort
-    additional_dependencies: [toml]
-    args: [--project=gliderpy, --multi-line=3, --lines-after-imports=2, --lines-between-types=1, --trailing-comma, --force-grid-wrap=0, --use-parentheses, --line-width=88]
-
-- repo: https://github.com/asottile/seed-isort-config
-  rev: v2.2.0
-  hooks:
-    - id: seed-isort-config
-
 - repo: https://github.com/psf/black
-  rev: 21.7b0
+  rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v0.790
+  rev: v1.2.0
   hooks:
   - id: mypy
     exclude: docs/source/conf.py
-    args: [--ignore-missing-imports]
+    entry: bash -c 'exec env CONDA_PREFIX="$(python -c "import sys; print(sys.executable)")"'
+    args: ["--ignore-missing-imports", "--python-executable=CONDA_PREFIX"]
+
+- repo: https://github.com/keewis/blackdoc
+  rev: v0.3.8
+  hooks:
+    - id: blackdoc
+
+- repo: https://github.com/econchick/interrogate
+  rev: 1.5.0
+  hooks:
+    - id: interrogate
+      exclude: ^(docs|setup.py|tests)
+      args: [--config=pyproject.toml]
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.0.0
+  rev: v2.2.4
   hooks:
     - id: codespell
+      exclude: >
+          (?x)^(
+              .*\.yaml
+          )$
       args:
         - --ignore-words-list=pres
-        - --quiet-level=2
+
+- repo: https://github.com/asottile/add-trailing-comma
+  rev: v2.4.0
+  hooks:
+    - id: add-trailing-comma
+
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: v0.0.261
+  hooks:
+    - id: ruff
+
+- repo: https://github.com/tox-dev/pyproject-fmt
+  rev: 0.9.2
+  hooks:
+    - id: pyproject-fmt
+
+ci:
+    autofix_commit_msg: |
+        [pre-commit.ci] auto fixes from pre-commit.com hooks
+
+        for more information, see https://pre-commit.ci
+    autofix_prs: false
+    autoupdate_commit_msg: '[pre-commit.ci] pre-commit autoupdate'
+    autoupdate_schedule: monthly
+    skip: []
+    submodules: false
```

### Comparing `gliderpy-0.0.4/LICENSE.txt` & `gliderpy-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gliderpy-0.0.4/README.md` & `gliderpy-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gliderpy-0.0.4/gliderpy/fetchers.py` & `gliderpy-0.1.0/gliderpy/fetchers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Helper methods to fetch glider data from multiple ERDDAP serves
 
 """
 
-import functools
-
 from typing import Optional
 
+import httpx
 import pandas as pd
-import requests
-
 from erddapy import ERDDAP
-from erddapy.url_handling import urlopen
-
-from gliderpy.servers import server_parameter_rename, server_select, server_vars
+from erddapy.erddapy import urlopen
 
+from gliderpy.servers import (
+    server_parameter_rename,
+    server_select,
+    server_vars,
+)
 
 OptionalStr = Optional[str]
 
 # This defaults to the IOOS glider DAC.
 _server = "https://gliders.ioos.us/erddap"
 
 
@@ -29,15 +29,15 @@
     df.columns = df.columns.str.lower()
     df.rename(columns=dict(server_parameter_rename), inplace=True)
     df.index.rename("time", inplace=True)
     df["dataset_url"] = dataset_url
     return df
 
 
-class GliderDataFetcher(object):
+class GliderDataFetcher:
     """
     Args:
         server: a glider ERDDAP server URL
 
     Attributes:
         dataset_id: a dataset unique id.
         constraints: download constraints, default None (opendap-like url)
@@ -58,25 +58,25 @@
     def to_pandas(self):
         """
         Fetches data from the server and reads into a pandas dataframe
 
         :return: pandas dataframe with datetime UTC as index
         """
         if type(self.datasets) is pd.Series:
-            df_all = pd.DataFrame()
+            df_all = []
             for dataset_id in self.datasets:
                 self.fetcher.dataset_id = dataset_id
                 df = self.fetcher.to_pandas(
                     index_col="time (UTC)",
                     parse_dates=True,
                 )
                 dataset_url = self.fetcher.get_download_url().split("?")[0]
                 df = standardise_df(df, dataset_url)
-                df_all = df_all.append(df)
-            return df_all
+                df_all.append(df)
+            return pd.concat(df_all)
 
         if not self.fetcher.dataset_id:
             return None
 
         df = self.fetcher.to_pandas(
             index_col="time (UTC)",
             parse_dates=True,
@@ -115,19 +115,19 @@
                 min_lon=min_lon,
                 max_lon=max_lon,
                 min_time=min_time,
                 max_time=max_time,
             )
             try:
                 data = urlopen(url)
-            except requests.exceptions.HTTPError:
-                print(
-                    "Error, no datasets found in supplied range. Try relaxing your constraints"
-                )
-                return
+            except httpx.HTTPError as err:
+                raise Exception(
+                    f"Error, no datasets found in supplied range. Try relaxing your constraints: {self.fetcher.constraints}",
+                ) from err
+                return None
             df = pd.read_csv(data)
             self.datasets = df["Dataset ID"]
             return df[["Title", "Institution", "Dataset ID"]]
 
         return self
 
     def platform(self, platform):
@@ -137,42 +137,36 @@
         :return: search query with platform constraint applied
         """
         self.fetcher.constraints["platform_deployment="] = platform
         return self
 
 
 class DatasetList:
-    """Search servers for glider dataset ids. Defaults to the string "glider"
+    """Build a glider dataset ids list.
 
 
     Attributes:
         e: an ERDDAP server instance
-        search_terms: A list of terms to search the server for. Multiple terms will be combined as AND
+        TODO: search_terms: A list of terms to search the server for. Multiple terms will be combined as AND
 
     """
 
     def __init__(self, server=_server):
         self.e = ERDDAP(
             server=server,
             protocol="tabledap",
         )
 
-    @functools.lru_cache(maxsize=None)
-    def _get_ids(self, search_terms):
-        """Thin wrapper where inputs can be hashed for lru_cache."""
-        dataset_ids = pd.Series(dtype=str)
-        for term in search_terms:
-            url = self.e.get_search_url(search_for=term, response="csv")
-
-            dataset_ids = dataset_ids.append(
-                pd.read_csv(url)["Dataset ID"], ignore_index=True
-            )
-        self.dataset_ids = dataset_ids.str.split(";", expand=True).stack().unique()
-
-        return self.dataset_ids
-
-    def get_ids(self, search_terms=["glider"]):
-        """Search the database using a user supplied list of comma separated strings
-        :return: Unique list of dataset ids
-        """
-        search_terms = tuple(search_terms)
-        return self._get_ids(search_terms)
+    def get_ids(self):
+        """Return the allDatasets list for the glider server."""
+        if self.e.server == "https://gliders.ioos.us/erddap":
+            self.e.dataset_id = "allDatasets"
+            dataset_ids = self.e.to_pandas()["datasetID"].to_list()
+            dataset_ids.remove("allDatasets")
+            self.dataset_ids = dataset_ids
+            return self.dataset_ids
+        else:
+            raise ValueError(f"The {self.e.server} does not supported this operation.")
+        # TODO: List the platform_deployment variable
+        # if self.e.server == "https://erddap.ifremer.fr/erddap":
+        #     dataset_id = OceanGlidersGDACTrajectories
+        #     platform_deployment
```

### Comparing `gliderpy-0.0.4/gliderpy/plotters.py` & `gliderpy-0.1.0/gliderpy/plotters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
 Some convenience functions to help visualize glider data.
 """
 
 import warnings
 
-
 try:
-
     import cartopy.crs as ccrs
     import matplotlib.dates as mdates
     import matplotlib.pyplot as plt
 except ModuleNotFoundError as err:
-    warnings.warn("gliderpy requires matplotlib and cartopy for plotting.")
+    warnings.warn(
+        "gliderpy requires matplotlib and cartopy for plotting.",
+        stacklevel=1,
+    )
     raise err
 
 
 def plot_track(df):
     """
     Plots a track of glider path coloured by temperature
     :return: figures, axes
     """
 
     x = df["longitude (degrees_east)"]
     y = df["latitude (degrees_north)"]
     dx, dy = 2, 4
 
     fig, ax = plt.subplots(
-        figsize=(9, 9), subplot_kw={"projection": ccrs.PlateCarree()}
+        figsize=(9, 9),
+        subplot_kw={"projection": ccrs.PlateCarree()},
     )
     ax.scatter(x, y, c=None, s=25, alpha=0.25, edgecolor="none")
     ax.coastlines("10m")
     ax.set_extent([x.min() - dx, x.max() + dx, y.min() - dy, y.max() + dy])
     return fig, ax
```

### Comparing `gliderpy-0.0.4/gliderpy/servers.py` & `gliderpy-0.1.0/gliderpy/servers.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,22 +28,14 @@
         "time",
         "latitude",
         "longitude",
         "PSAL",
         "TEMP",
         "PRES",
     ],
-    "https://erddap-uncabled.oceanobservatories.org/uncabled/erddap": [
-        "latitude",
-        "longitude",
-        "ctdgv_m_glider_instrument_practical_salinity",
-        "ctdgv_m_glider_instrument_sci_water_temp",
-        "ctdgv_m_glider_instrument_sci_water_pressure_dbar",
-        "time",
-    ],
 }
 
 server_parameter_rename = {
     "latitude (degrees_north)": "latitude",
     "longitude (degrees_east)": "longitude",
     "salinity (1)": "salinity",
     "psal (psu)": "salinity",
@@ -72,9 +64,9 @@
     for alias in server_alias:
         # If string matches one of the aliases, return the corresponding ERDDAP address
         if server_string.lower() == alias.lower():
             return server_alias[alias]
     # If the server is not recognised, print options of working servers and exit
     raise ValueError(
         "Supplied server/alias not recognised. Please use one of the following supported servers:\n"
-        f"{str(server_vars.keys())[10:-1]}"
+        f"{str(server_vars.keys())[10:-1]}",
     )
```

