# Comparing `tmp/jupyter_ydoc-1.0.0.tar.gz` & `tmp/jupyter_ydoc-1.0.1.tar.gz`

## Comparing `jupyter_ydoc-1.0.0.tar` & `jupyter_ydoc-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,44 @@
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.licenserc.yaml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.yarnrc.yml
--rw-r--r--   0        0        0    49931 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/lerna.json
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/package.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/pytest.ini
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/readthedocs.yml
--rw-r--r--   0        0        0   185553 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/yarn.lock
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.github/workflows/auto_author_assign.yml
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.github/workflows/license-header.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.github/workflows/test.yml
--rwxr-xr-x   0        0        0  2212925 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.yarn/releases/yarn-3.4.1.cjs
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/make.bat
--rw-r--r--   0        0        0    18122 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/changelog.md
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/conf.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/custom.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/index.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/javascript_api.rst
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/overview.md
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/python_api.rst
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/schema.md
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/_static/jupyter_logo.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/docs/source/api/index.html
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/javascript/package.json
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/py.typed
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/utils.py
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/ybasedoc.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/yblob.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/yfile.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/ynotebook.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/jupyter_ydoc/yunicode.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/.gitignore
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/LICENSE
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/README.md
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.licenserc.yaml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0    51202 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/lerna.json
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/package.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/pytest.ini
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/readthedocs.yml
+-rw-r--r--   0        0        0   185553 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/yarn.lock
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.github/workflows/auto_author_assign.yml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.github/workflows/license-header.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0  2212925 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.yarn/releases/yarn-3.4.1.cjs
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/custom.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/index.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/javascript_api.rst
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/overview.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/python_api.rst
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/schema.md
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/_static/jupyter_logo.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/javascript/package.json
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/py.typed
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/utils.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/ybasedoc.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/yblob.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/yfile.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/ynotebook.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/jupyter_ydoc/yunicode.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/README.md
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 jupyter_ydoc-1.0.1/PKG-INFO
```

### Comparing `jupyter_ydoc-1.0.0/.licenserc.yaml` & `jupyter_ydoc-1.0.1/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/.pre-commit-config.yaml` & `jupyter_ydoc-1.0.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       - id: debug-statements
       - id: forbid-new-submodules
       - id: check-builtin-literals
       - id: trailing-whitespace
         exclude: ^\.yarn
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: ["--line-length", "100"]
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
```

### Comparing `jupyter_ydoc-1.0.0/CHANGELOG.md` & `jupyter_ydoc-1.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.0.1
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_ydoc/compare/@jupyter/ydoc@1.0.0...6672e3dd27c2980f45ce1037101f0198fac3d9ff))
+
+### Bugs fixed
+
+- Fix metadata issue [#158](https://github.com/jupyter-server/jupyter_ydoc/pull/158) ([@hbcarlos](https://github.com/hbcarlos))
+
+### Maintenance and upkeep improvements
+
+### Documentation improvements
+
+- Fix ignore_links [#155](https://github.com/jupyter-server/jupyter_ydoc/pull/155) ([@fcollonval](https://github.com/fcollonval))
+- Enhance the documentation [#154](https://github.com/jupyter-server/jupyter_ydoc/pull/154) ([@fcollonval](https://github.com/fcollonval))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_ydoc/graphs/contributors?from=2023-03-29&to=2023-04-11&type=c))
+
+[@fcollonval](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Afcollonval+updated%3A2023-03-29..2023-04-11&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Ahbcarlos+updated%3A2023-03-29..2023-04-11&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Apre-commit-ci+updated%3A2023-03-29..2023-04-11&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.0.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_ydoc/compare/v0.3.4...6ad2fde183a3f592d8a2ff58254b229859caba01))
 
 ### Enhancements made
 
 - Add py.typed [#152](https://github.com/jupyter-server/jupyter_ydoc/pull/152) ([@davidbrochart](https://github.com/davidbrochart))
@@ -18,16 +41,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_ydoc/graphs/contributors?from=2023-02-22&to=2023-03-28&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Adavidbrochart+updated%3A2023-02-22..2023-03-28&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Afcollonval+updated%3A2023-02-22..2023-03-28&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_ydoc+involves%3Ahbcarlos+updated%3A2023-02-22..2023-03-28&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.3.4
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_ydoc/compare/@jupyter/ydoc@0.3.3...3c3aa3e0421193f391b10ae23745f235a6923cff))
 
 ### Bugs fixed
 
 - Fix notebook undo scope [#148](https://github.com/jupyter-server/jupyter_ydoc/pull/148) ([@fcollonval](https://github.com/fcollonval))
```

### Comparing `jupyter_ydoc-1.0.0/yarn.lock` & `jupyter_ydoc-1.0.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/.github/workflows/check-release.yml` & `jupyter_ydoc-1.0.1/.github/workflows/check-release.yml`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 permissions:
   contents: write
 
 jobs:
   check_release:
     runs-on: ubuntu-latest
     strategy:
+      fail-fast: false
       matrix:
         group: [check_release, link_check]
         python-version: ["3.9"]
         node-version: ["14.x"]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
       - name: Base Setup
         uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - name: Install Dependencies
         run: |
           pip install -e .
       - name: Check Links
         if: ${{ matrix.group == 'link_check' }}
-        uses: jupyter-server/jupyter_releaser/.github/actions/check-links@v1
+        uses: jupyterlab/maintainer-tools/.github/actions/check-links@v1
+        with:
+          ignore_links: "./api/index.html"
       - name: Check Release
         if: ${{ matrix.group == 'check_release' }}
         uses: jupyter-server/jupyter_releaser/.github/actions/check-release@v2
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
       - name: Upload Distributions
         if: ${{ matrix.group == 'check_release' }}
```

### Comparing `jupyter_ydoc-1.0.0/.github/workflows/license-header.yml` & `jupyter_ydoc-1.0.1/.github/workflows/license-header.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/.github/workflows/prep-release.yml` & `jupyter_ydoc-1.0.1/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/.github/workflows/publish-release.yml` & `jupyter_ydoc-1.0.1/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/.github/workflows/test.yml` & `jupyter_ydoc-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/.yarn/releases/yarn-3.4.1.cjs` & `jupyter_ydoc-1.0.1/.yarn/releases/yarn-3.4.1.cjs`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/docs/Makefile` & `jupyter_ydoc-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/docs/make.bat` & `jupyter_ydoc-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/docs/source/conf.py` & `jupyter_ydoc-1.0.1/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,25 +80,18 @@
 def setup(app):
     # Copy changelog.md file
     dest = HERE / "changelog.md"
     shutil.copy(str(HERE.parent.parent / "CHANGELOG.md"), str(dest))
 
     # Build JavaScript Docs
     js = HERE.parent.parent / "javascript"
-    js_docs = js / "docs"
     dest_dir = Path(app.outdir) / "api"
 
-    if js_docs.exists():
-        # avoid rebuilding docs because it takes forever
-        # `make clean` to force a rebuild
-        print(f"already have {js_docs!s}")
-    else:
-        print("Building jupyterlab API docs")
-        check_call(["npm", "install"], cwd=str(js))
-        check_call(["npm", "run", "build"], cwd=str(js))
-        check_call(["npm", "run", "docs"], cwd=str(js))
+    print("Building @jupyter/ydoc API docs")
+    cmd = ["yarn"] if shutil.which("yarn") is not None else ["npm"]
+    check_call(cmd + ["install"], cwd=str(js))
+    check_call(cmd + ["run", "build"], cwd=str(js))
+    check_call(cmd + ["run", "docs"], cwd=str(js))
 
-    # Copy JavaScript Docs
-    print(f"Copying {js_docs!s} -> {dest_dir!s}")
     if dest_dir.exists():
-        shutil.rmtree(str(dest_dir))
-    shutil.copytree(str(js_docs), str(dest_dir))
+        shutil.rmtree(dest_dir)
+    shutil.copytree(str(js / "docs"), str(dest_dir))
```

### Comparing `jupyter_ydoc-1.0.0/docs/source/custom.md` & `jupyter_ydoc-1.0.1/docs/source/custom.md`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/docs/source/overview.md` & `jupyter_ydoc-1.0.1/docs/source/overview.md`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/docs/source/schema.md` & `jupyter_ydoc-1.0.1/docs/source/schema.md`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/docs/source/_static/jupyter_logo.svg` & `jupyter_ydoc-1.0.1/docs/source/_static/jupyter_logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/docs/source/_static/logo-icon.png` & `jupyter_ydoc-1.0.1/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/javascript/package.json` & `jupyter_ydoc-1.0.1/javascript/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'scripts'": "{'clean': 'rimraf lib tsconfig.tsbuildinfo docs', 'docs': 'typedoc src'}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -43,16 +43,16 @@
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyter-server/jupyter_ydoc.git"
     },
     "scripts": {
         "build": "tsc -b",
         "build:test": "tsc --build tsconfig.test.json",
-        "clean": "rimraf lib && rimraf tsconfig.tsbuildinfo",
-        "docs": "typedoc --out ./docs src",
+        "clean": "rimraf lib tsconfig.tsbuildinfo docs",
+        "docs": "typedoc src",
         "eslint": "eslint --ext .js,.jsx,.ts,.tsx --cache --fix .",
         "eslint:check": "eslint --ext .js,.jsx,.ts,.tsx --cache .",
         "integrity": "yarn tsc-esm-fix --src='src' --ext='.js'",
         "lint": "yarn integrity && yarn prettier && yarn eslint",
         "lint:check": "yarn prettier:check && yarn eslint:check",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json}\"",
         "prettier:check": "prettier --check \"**/*{.ts,.tsx,.js,.jsx,.css,.json}\"",
@@ -60,9 +60,9 @@
         "test:cov": "jest --collect-coverage",
         "test:debug": "node --inspect-brk node_modules/.bin/jest --runInBand",
         "test:debug:watch": "node --inspect-brk node_modules/.bin/jest --runInBand --watch",
         "watch": "tsc -b --watch"
     },
     "type": "module",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `jupyter_ydoc-1.0.0/jupyter_ydoc/__init__.py` & `jupyter_ydoc-1.0.1/jupyter_ydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/jupyter_ydoc/utils.py` & `jupyter_ydoc-1.0.1/jupyter_ydoc/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/jupyter_ydoc/ybasedoc.py` & `jupyter_ydoc-1.0.1/jupyter_ydoc/ybasedoc.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/jupyter_ydoc/yblob.py` & `jupyter_ydoc-1.0.1/jupyter_ydoc/yblob.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/jupyter_ydoc/ynotebook.py` & `jupyter_ydoc-1.0.1/jupyter_ydoc/ynotebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,17 +216,17 @@
                 and not cell["attachments"]
             ):
                 del cell["attachments"]
             cells.append(cell)
 
         return dict(
             cells=cells,
-            metadata=meta["metadata"],
-            nbformat=int(meta["nbformat"]),
-            nbformat_minor=int(meta["nbformat_minor"]),
+            metadata=meta.get("metadata", {}),
+            nbformat=int(meta.get("nbformat", 0)),
+            nbformat_minor=int(meta.get("nbformat_minor", 0)),
         )
 
     def set(self, value: Dict) -> None:
         """
         Sets the content of the document.
 
         :param value: The content of the document.
```

### Comparing `jupyter_ydoc-1.0.0/jupyter_ydoc/yunicode.py` & `jupyter_ydoc-1.0.1/jupyter_ydoc/yunicode.py`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/.gitignore` & `jupyter_ydoc-1.0.1/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -141,7 +141,9 @@
 .pnp.*
 .yarn/*
 !.yarn/patches
 !.yarn/plugins
 !.yarn/releases
 !.yarn/sdks
 !.yarn/versions
+docs/source/api
+docs/source/changelog.md
```

### Comparing `jupyter_ydoc-1.0.0/LICENSE` & `jupyter_ydoc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/README.md` & `jupyter_ydoc-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/pyproject.toml` & `jupyter_ydoc-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ydoc-1.0.0/PKG-INFO` & `jupyter_ydoc-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-ydoc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Document structures for collaborative editing using Ypy
 Project-URL: Homepage, https://jupyter.org
 Project-URL: Source, https://github.com/jupyter-server/jupyter_ydoc
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: jupyter,ypy
```

