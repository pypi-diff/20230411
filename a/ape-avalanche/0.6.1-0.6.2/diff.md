# Comparing `tmp/ape-avalanche-0.6.1.tar.gz` & `tmp/ape-avalanche-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-avalanche-0.6.1.tar", last modified: Wed Mar 15 02:16:17 2023, max compression
+gzip compressed data, was "ape-avalanche-0.6.2.tar", last modified: Tue Apr 11 14:20:59 2023, max compression
```

## Comparing `ape-avalanche-0.6.1.tar` & `ape-avalanche-0.6.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 02:16:17.094486 ape-avalanche-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 02:16:17.090486 ape-avalanche-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 02:16:17.090486 ape-avalanche-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 02:16:17.094486 ape-avalanche-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-15 02:16:17.098486 ape-avalanche-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 02:16:17.094486 ape-avalanche-0.6.1/ape_avalanche/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/ape_avalanche/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/ape_avalanche/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/ape_avalanche/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-15 02:16:16.000000 ape-avalanche-0.6.1/ape_avalanche/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 02:16:17.094486 ape-avalanche-0.6.1/ape_avalanche.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-15 02:16:16.000000 ape-avalanche-0.6.1/ape_avalanche.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-15 02:16:17.000000 ape-avalanche-0.6.1/ape_avalanche.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 02:16:16.000000 ape-avalanche-0.6.1/ape_avalanche.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 02:16:16.000000 ape-avalanche-0.6.1/ape_avalanche.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-15 02:16:16.000000 ape-avalanche-0.6.1/ape_avalanche.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-15 02:16:16.000000 ape-avalanche-0.6.1/ape_avalanche.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-15 02:16:17.098486 ape-avalanche-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 02:16:17.094486 ape-avalanche-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-15 02:15:09.000000 ape-avalanche-0.6.1/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.358796 ape-avalanche-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.358796 ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.358796 ape-avalanche-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/ape_avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/ape_avalanche/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/ape_avalanche/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/ape_avalanche/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/ape_avalanche.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 14:20:59.000000 ape-avalanche-0.6.2/ape_avalanche.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:59.362796 ape-avalanche-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-11 14:20:04.000000 ape-avalanche-0.6.2/tests/test_provider.py
```

### Comparing `ape-avalanche-0.6.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-avalanche-0.6.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.github/release-drafter.yml` & `ape-avalanche-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.github/workflows/codeql.yaml` & `ape-avalanche-0.6.2/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.github/workflows/commitlint.yaml` & `ape-avalanche-0.6.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.github/workflows/prtitle.yaml` & `ape-avalanche-0.6.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.github/workflows/publish.yaml` & `ape-avalanche-0.6.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.github/workflows/test.yaml` & `ape-avalanche-0.6.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.gitignore` & `ape-avalanche-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/.pre-commit-config.yaml` & `ape-avalanche-0.6.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ape-avalanche-0.6.1/CONTRIBUTING.md` & `ape-avalanche-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/LICENSE` & `ape-avalanche-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/PKG-INFO` & `ape-avalanche-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-avalanche
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-avalanche: Ape Ecosystem Plugin for Avalanche
 Home-page: https://github.com/ApeWorX/ape-avalanche
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-avalanche-0.6.1/README.md` & `ape-avalanche-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/ape_avalanche/__init__.py` & `ape-avalanche-0.6.2/ape_avalanche/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     yield Avalanche
 
 
 @plugins.register(plugins.NetworkPlugin)
 def networks():
     for network_name, network_params in NETWORKS.items():
         yield "avalanche", network_name, create_network_type(*network_params)
+        yield "avalanche", f"{network_name}-fork", NetworkAPI
 
     # NOTE: This works for development providers, as they get chain_id from themselves
     yield "avalanche", LOCAL_NETWORK_NAME, NetworkAPI
-    yield "avalanche", "mainnet-fork", NetworkAPI
 
 
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     for network_name in NETWORKS:
         yield "avalanche", network_name, GethProvider
```

### Comparing `ape-avalanche-0.6.1/ape_avalanche.egg-info/PKG-INFO` & `ape-avalanche-0.6.2/ape_avalanche.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-avalanche
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-avalanche: Ape Ecosystem Plugin for Avalanche
 Home-page: https://github.com/ApeWorX/ape-avalanche
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-avalanche-0.6.1/ape_avalanche.egg-info/SOURCES.txt` & `ape-avalanche-0.6.2/ape_avalanche.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/pyproject.toml` & `ape-avalanche-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-avalanche-0.6.1/setup.py` & `ape-avalanche-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # Auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
-        "flake8>=5.0.4",  # Style linter
+        "flake8>=6.0.0,<7",  # Style linter
         "isort>=5.10.1",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
@@ -53,15 +53,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-avalanche",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.5,<0.7.0",
+        "eth-ape>=0.6.7,<0.7.0",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape-avalanche"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
```

### Comparing `ape-avalanche-0.6.1/tests/test_integration.py` & `ape-avalanche-0.6.2/tests/test_integration.py`

 * *Files identical despite different names*

