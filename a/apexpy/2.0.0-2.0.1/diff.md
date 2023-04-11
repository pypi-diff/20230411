# Comparing `tmp/apexpy-2.0.0.tar.gz` & `tmp/apexpy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apexpy-2.0.0.tar", last modified: Fri Dec  9 18:28:19 2022, max compression
+gzip compressed data, was "apexpy-2.0.1.tar", last modified: Tue Apr 11 17:30:17 2023, max compression
```

## Comparing `apexpy-2.0.0.tar` & `apexpy-2.0.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0      199 1970-01-01 00:00:00.000000 apexpy-2.0.0/.codeclimate.yml
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 apexpy-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 apexpy-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 apexpy-2.0.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 apexpy-2.0.0/.github/pull_request_template.md
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 apexpy-2.0.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3409 1970-01-01 00:00:00.000000 apexpy-2.0.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 apexpy-2.0.0/.gitignore
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 apexpy-2.0.0/.zenodo.json
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 apexpy-2.0.0/AUTHORS.rst
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 apexpy-2.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0     3364 1970-01-01 00:00:00.000000 apexpy-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 apexpy-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 apexpy-2.0.0/LICENSE
--rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 apexpy-2.0.0/MANIFEST.in
--rw-r--r--   0        0        0     5373 1970-01-01 00:00:00.000000 apexpy-2.0.0/README.rst
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/__init__.py
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/__main__.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/_gcc_build_bitness.py
--rw-r--r--   0        0        0    48855 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/apex.py
--rw-r--r--   0        0        0   244852 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/apexsh.dat
--rw-r--r--   0        0        0     6653 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/helpers.py
--rw-r--r--   0        0        0    40639 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/igrf13coeffs.txt
--rw-r--r--   0        0        0    64437 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/tests/test_Apex.py
--rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/tests/test_cmd.py
--rw-r--r--   0        0        0       42 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/tests/test_convert.txt
--rw-r--r--   0        0        0        6 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/tests/test_convert_single_line.txt
--rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/tests/test_fortranapex.py
--rw-r--r--   0        0        0    11267 1970-01-01 00:00:00.000000 apexpy-2.0.0/apexpy/tests/test_helpers.py
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/Makefile
--rw-r--r--   0        0        0     2430 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/api.rst
--rw-r--r--   0        0        0       28 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/authors.rst
--rw-r--r--   0        0        0       30 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/changelog.rst
--rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/conf.py
--rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/contributing.rst
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/examples/ex_apexh.rst
--rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/examples/ex_cli.rst
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/examples/ex_gc.rst
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/examples/ex_init.rst
--rw-r--r--   0        0        0      196 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/examples/index.rst
--rw-r--r--   0        0        0      257 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/index.rst
--rw-r--r--   0        0        0     9548 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/installation.rst
--rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/maintenance.rst
--rw-r--r--   0        0        0       27 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/readme.rst
--rw-r--r--   0        0        0       44 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      109 1970-01-01 00:00:00.000000 apexpy-2.0.0/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/Makefile
--rw-r--r--   0        0        0    26263 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/apex.f90
--rw-r--r--   0        0        0    26979 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/apexsh.f90
--rw-r--r--   0        0        0    10317 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/checkapexsh.f90
--rw-r--r--   0        0        0    28607 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/fortranapex-f2pywrappers2.f90
--rw-r--r--   0        0        0    16259 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/fortranapex.pyf
--rw-r--r--   0        0        0   126484 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/fortranapexmodule.c
--rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/igrf.f90
--rw-r--r--   0        0        0    20202 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/magfld.f90
--rw-r--r--   0        0        0    11590 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/makeapexsh.f90
--rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 apexpy-2.0.0/fortranapex/readme.txt
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 apexpy-2.0.0/meson.build
--rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 apexpy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 apexpy-2.0.0/setup.cfg
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 apexpy-2.0.0/setup.py
--rw-r--r--   0        0        0     8457 1970-01-01 00:00:00.000000 apexpy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      199 1970-01-01 00:00:00.000000 apexpy-2.0.1/.codeclimate.yml
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 apexpy-2.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 apexpy-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 apexpy-2.0.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 apexpy-2.0.1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 apexpy-2.0.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 apexpy-2.0.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 apexpy-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 apexpy-2.0.1/.zenodo.json
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 apexpy-2.0.1/AUTHORS.rst
+-rw-r--r--   0        0        0     2568 1970-01-01 00:00:00.000000 apexpy-2.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     3364 1970-01-01 00:00:00.000000 apexpy-2.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 apexpy-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 apexpy-2.0.1/LICENSE
+-rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 apexpy-2.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 apexpy-2.0.1/README.rst
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/__init__.py
+-rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/__main__.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/_gcc_build_bitness.py
+-rw-r--r--   0        0        0    48849 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/apex.py
+-rw-r--r--   0        0        0   244852 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/apexsh.dat
+-rw-r--r--   0        0        0     6653 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/helpers.py
+-rw-r--r--   0        0        0    40639 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/igrf13coeffs.txt
+-rw-r--r--   0        0        0    67396 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/tests/test_Apex.py
+-rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/tests/test_cmd.py
+-rw-r--r--   0        0        0       42 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/tests/test_convert.txt
+-rw-r--r--   0        0        0        6 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/tests/test_convert_single_line.txt
+-rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/tests/test_fortranapex.py
+-rw-r--r--   0        0        0    11267 1970-01-01 00:00:00.000000 apexpy-2.0.1/apexpy/tests/test_helpers.py
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/Makefile
+-rw-r--r--   0        0        0    27209 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/apexpy.png
+-rw-r--r--   0        0        0     2427 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/api.rst
+-rw-r--r--   0        0        0       28 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/authors.rst
+-rw-r--r--   0        0        0       30 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/changelog.rst
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/conf.py
+-rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/contributing.rst
+-rw-r--r--   0        0        0      232 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/ex_index.rst
+-rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/examples/ex_apexh.rst
+-rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/examples/ex_cli.rst
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/examples/ex_gc.rst
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/examples/ex_init.rst
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/index.rst
+-rw-r--r--   0        0        0    10645 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/installation.rst
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/maintenance.rst
+-rw-r--r--   0        0        0       27 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/readme.rst
+-rw-r--r--   0        0        0       44 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0      109 1970-01-01 00:00:00.000000 apexpy-2.0.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/Makefile
+-rw-r--r--   0        0        0    26263 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/apex.f90
+-rw-r--r--   0        0        0    26979 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/apexsh.f90
+-rw-r--r--   0        0        0    10337 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/checkapexsh.f90
+-rw-r--r--   0        0        0    28607 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/fortranapex-f2pywrappers2.f90
+-rw-r--r--   0        0        0    16259 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/fortranapex.pyf
+-rw-r--r--   0        0        0   126484 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/fortranapexmodule.c
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/igrf.f90
+-rw-r--r--   0        0        0    20216 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/magfld.f90
+-rw-r--r--   0        0        0    11590 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/makeapexsh.f90
+-rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 apexpy-2.0.1/fortranapex/readme.txt
+-rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 apexpy-2.0.1/meson.build
+-rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 apexpy-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 apexpy-2.0.1/setup.cfg
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 apexpy-2.0.1/setup.py
+-rw-r--r--   0        0        0     8530 1970-01-01 00:00:00.000000 apexpy-2.0.1/PKG-INFO
```

### Comparing `apexpy-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `apexpy-2.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `apexpy-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/.github/ISSUE_TEMPLATE/question.md` & `apexpy-2.0.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/.github/pull_request_template.md` & `apexpy-2.0.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/.github/workflows/docs.yml` & `apexpy-2.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/.github/workflows/main.yml` & `apexpy-2.0.1/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # This workflow will install Python dependencies, run tests and lint with a
 # variety of Python versions. For more information see:
 # https://help.github.com/actions/language-and-framework-guides/
 # using-python-with-github-actions
 
 name: pytest with flake8
 
-on: [push, pull_request]
+on:
+  pull_request:
+  push:
+  schedule:
+    - cron: "0 3 * * 1"  # Runs 03:00 UT on Mondays 
 
 jobs:
   build:
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
@@ -44,16 +48,16 @@
           python -m build .
           pip install .
 
     - name: Install on MacOS
       if: ${{ matrix.os == 'macos-latest' }}
       run: |
           brew reinstall gcc
-          python -m build .
-          pip install .
+          CC=/usr/local/bin/gcc-12 python -m build .
+          CC=/usr/local/bin/gcc-12 pip install .
 
     - name: Install on Windows
       if: ${{ matrix.os == 'windows-latest' }}
       run: |
           meson setup build
           ninja -j 2 -C build
           cd build
```

### Comparing `apexpy-2.0.0/.gitignore` & `apexpy-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/.zenodo.json` & `apexpy-2.0.1/.zenodo.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'creators'": "{insert: [(3, OrderedDict([('orcid', '0000-0001-7098-0524'), ('name', 'Lamarche, "*

 * *               "Leslie L.')]))], delete: [6]}"}*

```diff
@@ -10,29 +10,29 @@
         },
         {
             "affiliation": "Naval Research Laboratory",
             "name": "Burrell, Angeline G.",
             "orcid": "0000-0001-8875-9326"
         },
         {
+            "name": "Lamarche, Leslie L.",
+            "orcid": "0000-0001-7098-0524"
+        },
+        {
             "name": "Starr, Gregory",
             "orcid": "0000-0002-3487-3630"
         },
         {
             "name": "Reimer, Ashton S.",
             "orcid": "0000-0002-4621-3453"
         },
         {
             "affiliation": "GFZ German Research Centre for Geosciences",
             "name": "Morschhauser, Achim",
             "orcid": "0000-0001-7955-4441"
-        },
-        {
-            "name": "Lamarche, Leslie L.",
-            "orchid": "0000-0001-7098-0524"
         }
     ],
     "keywords": [
         "Magnetic Apex Coordinates",
         "Quasi Dipole Coordinates",
         "MLT",
         "Magnetic Local Time",
```

### Comparing `apexpy-2.0.0/AUTHORS.rst` & `apexpy-2.0.1/AUTHORS.rst`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 =======
 
 This python wrapper is made by:
 
 * Karl M. Laundal
 * Christer van der Meeren
 * Angeline G. Burrell (maintainer)
+* Leslie Lamarche
 * Gregory Starr
 * Ashton Reimer
 * Achim Morschhauser
-* Leslie Lamarche
 
 Fortran code by Emmert et al. [2010] [1]_. Quasi-dipole and modified
 apex coordinates are defined by Richmond [1995] [2]_. The code uses
 IGRF-12 with coefficients valid through 2020 [Thébault et al., 2015] [3]_.
 
 .. [1] Emmert, J. T., A. D. Richmond, and D. P. Drob (2010),
        A computationally compact representation of Magnetic-Apex
        and Quasi-Dipole coordinates with smooth base vectors,
-       J. Geophys. Res., 115(A8), A08322, :doi:`10.1029/2010JA015326`.
+       J. Geophys. Res., 115(A8), A08322, doi:10.1029/2010JA015326.
 
 .. [2] Richmond, A. D. (1995), Ionospheric Electrodynamics Using
        Magnetic Apex Coordinates, Journal of geomagnetism and
        geoelectricity, 47(2), 191–212,
        `doi:10.5636/jgg.47.191 <http://dx.doi.org/10.5636/jgg.47.191>`_.
 
 .. [3] Thébault, E. et al. (2015), International Geomagnetic Reference
```

### Comparing `apexpy-2.0.0/CHANGELOG.rst` & `apexpy-2.0.1/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 
 Changelog
 =========
 
+2.0.1 (2023-04-11)
+------------------
+* Expanded installation instructions in the documenation
+* Added unit tests for todays date, ensuring that `apex.dat` is current
+* Added cron unit test to GitHub Actions CI
+* Added a logo
+* Correct indexing bug in Fortran source that was causing array overflow and
+  memory errors for extrapolated years beyond the latest formal IGRF fit
+
 2.0.0 (2022-12-09)
 ------------------
 * Update Fortran source code to Fortran 90 standards
 * Removed Python 2 support
 * Updated community and package documentation
 * Updated unit test style to reduce duplication and better follow PEP8
 * Updated code style using codacy suggestions and reduced complexity
```

### Comparing `apexpy-2.0.0/CODE_OF_CONDUCT.md` & `apexpy-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/CONTRIBUTING.rst` & `apexpy-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/LICENSE` & `apexpy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/README.rst` & `apexpy-2.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+|logo|
+
 ========
 Overview
 ========
 
 |docs| |version| |doi|
 
 This is a Python wrapper for the Apex fortran library by
@@ -67,16 +69,15 @@
 
 References
 ==========
 
 .. [1] Emmert, J. T., A. D. Richmond, and D. P. Drob (2010),
        A computationally compact representation of Magnetic-Apex
        and Quasi-Dipole coordinates with smooth base vectors,
-       J. Geophys. Res., 115(A8), A08322,
-       `doi:10.1029/2010JA015326 <http://dx.doi.org/10.1029/2010JA015326>`_.
+       J. Geophys. Res., 115(A8), A08322, doi:10.1029/2010JA015326.
 
 .. [2] Richmond, A. D. (1995), Ionospheric Electrodynamics Using
        Magnetic Apex Coordinates, Journal of geomagnetism and
        geoelectricity, 47(2), 191–212,
        `doi:10.5636/jgg.47.191 <http://dx.doi.org/10.5636/jgg.47.191>`_.
 
 Badges
@@ -117,27 +118,30 @@
 
 .. |version| image:: https://img.shields.io/pypi/v/apexpy.svg?style=flat
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/apexpy/
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/apexpy.svg?style=flat
     :alt: PyPI Package monthly downloads
-    :target: https://pypi.python.org/pypi/apexpy
+    :target: https://pypi.org/project/apexpy
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/apexpy.svg?style=flat
     :alt: PyPI Wheel
-    :target: https://pypi.python.org/pypi/apexpy
+    :target: https://pypi.org/project/apexpy
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/apexpy.svg?style=flat
     :alt: Supported versions
-    :target: https://pypi.python.org/pypi/apexpy
+    :target: https://pypi.org/project/apexpy
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/apexpy.svg?style=flat
     :alt: Supported implementations
-    :target: https://pypi.python.org/pypi/apexpy
+    :target: https://pypi.org/project/apexpy
 
 .. |scrutinizer| image:: https://img.shields.io/scrutinizer/quality/g/aburrell/apexpy/main.svg?style=flat
     :alt: Scrutinizer Status
     :target: https://scrutinizer-ci.com/g/aburrell/apexpy/
 
 .. |doi| image:: https://www.zenodo.org/badge/doi/10.5281/zenodo.4585641.svg
    :target: https://doi.org/10.5281/zenodo.1214206
+
+.. |logo| image:: docs/apexpy.png
+   :alt: ApexPy logo: yellow magnetic field lines surrounding the Earth's surface, which is blue
```

### Comparing `apexpy-2.0.0/apexpy/__init__.py` & `apexpy-2.0.1/apexpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
                           "apexpy probably won't work. Failed with error: ",
                           str(ierr)]))
 
 from apexpy.apex import Apex, ApexHeightError  # noqa F401
 from apexpy import helpers  # noqa F401
 
 # Define the global variables
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __all__ = ['Apex', 'fortranapex', 'helpers', 'ApexHeightError']
```

### Comparing `apexpy-2.0.0/apexpy/__main__.py` & `apexpy-2.0.1/apexpy/__main__.py`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/apexpy/_gcc_build_bitness.py` & `apexpy-2.0.1/apexpy/_gcc_build_bitness.py`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/apexpy/apex.py` & `apexpy-2.0.1/apexpy/apex.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,15 +976,15 @@
         .. [2] Richmond, A. D. (1995), Ionospheric Electrodynamics Using
                Magnetic Apex Coordinates, Journal of geomagnetism and
                geoelectricity, 47(2), 191–212, :doi:`10.5636/jgg.47.191`.
 
         .. [3] Emmert, J. T., A. D. Richmond, and D. P. Drob (2010),
                A computationally compact representation of Magnetic-Apex
                and Quasi-Dipole coordinates with smooth base vectors,
-               J. Geophys. Res., 115(A8), A08322, :doi:`10.1029/2010JA015326`.
+               J. Geophys. Res., 115(A8), A08322, doi:10.1029/2010JA015326.
 
         """
         # Convert from current coordinates to geodetic coordinates
         glat, glon = self.convert(lat, lon, coords, 'geo', height=height,
                                   precision=precision)
 
         # Get the geodetic base vectors
@@ -1075,15 +1075,15 @@
         .. [4] Richmond, A. D. (1995), Ionospheric Electrodynamics Using
                Magnetic Apex Coordinates, Journal of geomagnetism and
                geoelectricity, 47(2), 191–212, :doi:`10.5636/jgg.47.191`.
 
         .. [5] Emmert, J. T., A. D. Richmond, and D. P. Drob (2010),
                A computationally compact representation of Magnetic-Apex
                and Quasi-Dipole coordinates with smooth base vectors,
-               J. Geophys. Res., 115(A8), A08322, :doi:`10.1029/2010JA015326`.
+               J. Geophys. Res., 115(A8), A08322, doi:10.1029/2010JA015326.
 
         """
         # Convert to geodetic coordinates from current coordinate system
         glat, glon = self.convert(lat, lon, coords, 'geo', height=height,
                                   precision=precision)
 
         # Retrieve the desired magnetic locations and base vectors
```

### Comparing `apexpy-2.0.0/apexpy/helpers.py` & `apexpy-2.0.1/apexpy/helpers.py`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/apexpy/igrf13coeffs.txt` & `apexpy-2.0.1/apexpy/igrf13coeffs.txt`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/apexpy/tests/test_Apex.py` & `apexpy-2.0.1/apexpy/tests/test_Apex.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,21 @@
     def test_init_defaults(self):
         """Test Apex class default initialization."""
         self.apex_out = apexpy.Apex()
         self.eval_date()
         self.eval_refh()
         return
 
+    def test_init_today(self):
+        """Test Apex class initialization with today's date."""
+        self.apex_out = apexpy.Apex(date=self.test_date)
+        self.eval_date()
+        self.eval_refh()
+        return
+
     @pytest.mark.parametrize("in_date",
                              [2015, 2015.5, dt.date(2015, 1, 1),
                               dt.datetime(2015, 6, 1, 18, 23, 45)])
     def test_init_date(self, in_date):
         """Test Apex class with date initialization.
 
         Parameters
@@ -309,14 +316,21 @@
 
         # Add a vector flag, if needed
         if method_name in ["apxg2all", "apxg2q"]:
             in_args.append(1)
 
         return in_args
 
+    def test_apex_conversion_today(self):
+        """Test Apex class conversion with today's date."""
+        self.apex_out = apexpy.Apex(date=dt.datetime.utcnow(), refh=300)
+        assert not np.isnan(self.apex_out.geo2apex(self.in_lat, self.in_lon,
+                                                   self.in_alt)).any()
+        return
+
     @pytest.mark.parametrize("apex_method,fortran_method,fslice",
                              [("_geo2qd", "apxg2q", slice(0, 2, 1)),
                               ("_geo2apex", "apxg2all", slice(2, 4, 1)),
                               ("_qd2geo", "apxq2g", slice(None)),
                               ("_basevec", "apxg2q", slice(2, 4, 1))])
     @pytest.mark.parametrize("lat", [0, 30, 60, 89])
     @pytest.mark.parametrize("lon", [-179, -90, 0, 90, 180])
@@ -1754,7 +1768,79 @@
 
         """
 
         fheight = self.apex_out.get_height(lat, 3000.0)
         assert abs(height - fheight) < 1.0e-7, \
             "bad height calculation: {:.7f} != {:.7f}".format(height, fheight)
         return
+
+
+class TestApexMethodExtrapolateIGRF(object):
+    """Test the Apex methods on a year when IGRF must be extrapolated.
+
+    Notes
+    -----
+    Extrapolation should be done using a year within 5 years of the latest IGRF
+    model epoch.
+
+    """
+
+    def setup_method(self):
+        """Initialize all tests."""
+        self.apex_out = apexpy.Apex(date=2025, refh=300)
+        self.in_lat = 60
+        self.in_lon = 15
+        self.in_alt = 100
+        self.in_time = dt.datetime(2024, 2, 3, 4, 5, 6)
+        return
+
+    def teardown_method(self):
+        """Clean up after each test."""
+        del self.apex_out, self.in_lat, self.in_lon, self.in_alt
+        return
+
+    @pytest.mark.parametrize("method_name, out_comp",
+                             [("geo2apex",
+                               (56.25343704223633, 92.04932403564453)),
+                              ("apex2geo",
+                               (53.84184265136719, -66.93045806884766,
+                                3.6222547805664362e-06)),
+                              ("geo2qd",
+                               (56.82968521118164, 92.04932403564453)),
+                              ("apex2qd", (60.498401178276744, 15.0)),
+                              ("qd2apex", (59.49138097045895, 15.0))])
+    def test_method_scalar_input(self, method_name, out_comp):
+        """Test the user method against set values with scalars.
+
+        Parameters
+        ----------
+        method_name : str
+            Apex class method to be tested
+        out_comp : tuple of floats
+            Expected output values
+
+        """
+        # Get the desired methods
+        user_method = getattr(self.apex_out, method_name)
+
+        # Get the user output
+        user_out = user_method(self.in_lat, self.in_lon, self.in_alt)
+
+        # Evaluate the user output
+        np.testing.assert_allclose(user_out, out_comp, rtol=1e-5, atol=1e-5)
+
+        for out_val in user_out:
+            assert np.asarray(out_val).shape == (), "output is not a scalar"
+        return
+
+    def test_convert_to_mlt(self):
+        """Test conversion from mlon to mlt with scalars."""
+
+        # Get user output
+        user_out = self.apex_out.mlon2mlt(self.in_lon, self.in_time)
+
+        # Set comparison values
+        out_comp = 23.955474853515625
+
+        # Evaluate user output
+        np.testing.assert_allclose(user_out, out_comp, rtol=1e-5, atol=1e-5)
+        return
```

### Comparing `apexpy-2.0.0/apexpy/tests/test_cmd.py` & `apexpy-2.0.1/apexpy/tests/test_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,27 +57,27 @@
         Returns
         -------
         data : np.array, NoneType, or subprocess.Popen attribute
             Numpy array of data from output file, None if no file was created,
             or the requested output from the pipe command.
 
         """
-        if command_kwargs is None:
-            command_kwargs = {}
-
-        pipe = subprocess.Popen(command, **command_kwargs)
-        out = pipe.communicate()
-        pipe.wait()
+        data = None
 
         if pipe_out:
-            data = out
-        elif os.path.isfile(self.outfile):
-            data = np.loadtxt(self.outfile)
+            if command_kwargs is None:
+                command_kwargs = {}
+
+            pipe = subprocess.Popen(command, **command_kwargs)
+            data = pipe.communicate()
+            pipe.wait()
         else:
-            data = None
+            os.system(" ".join(command))
+            if os.path.isfile(self.outfile):
+                data = np.loadtxt(self.outfile)
 
         return data
 
     @pytest.mark.parametrize("date_str", [("2015"), ("201501"), ('20150101'),
                                           ('20150101000000')])
     def test_convert_w_datetime(self, date_str):
         """Test command line with different date and time specification.
```

### Comparing `apexpy-2.0.0/apexpy/tests/test_fortranapex.py` & `apexpy-2.0.1/apexpy/tests/test_fortranapex.py`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/apexpy/tests/test_helpers.py` & `apexpy-2.0.1/apexpy/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/docs/Makefile` & `apexpy-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/docs/api.rst` & `apexpy-2.0.1/docs/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -59,8 +59,8 @@
                             input file (stdin if none specified)
       -o FILE_OUT, --output FILE_OUT
                             output file (stdout if none specified)
 
 .. [1] Emmert, J. T., A. D. Richmond, and D. P. Drob (2010),
        A computationally compact representation of Magnetic-Apex
        and Quasi-Dipole coordinates with smooth base vectors,
-       J. Geophys. Res., 115(A8), A08322, :doi:`10.1029/2010JA015326`.
+       J. Geophys. Res., 115(A8), A08322, doi:10.1029/2010JA015326.
```

### Comparing `apexpy-2.0.0/docs/examples/ex_apexh.rst` & `apexpy-2.0.1/docs/examples/ex_apexh.rst`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/docs/examples/ex_cli.rst` & `apexpy-2.0.1/docs/examples/ex_cli.rst`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/docs/examples/ex_gc.rst` & `apexpy-2.0.1/docs/examples/ex_gc.rst`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/docs/examples/ex_init.rst` & `apexpy-2.0.1/docs/examples/ex_init.rst`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/docs/installation.rst` & `apexpy-2.0.1/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 :py:mod:`apexpy` source code.
 
 The code behind this package is written in Fortran.  Because of this, you
 **MUST** have a fortran compiler installed on your system before you attempt
 the following steps.  `Gfortran <https://gcc.gnu.org/wiki/GFortran>`_ is a free
 compiler that can be installed, if one is not already available on your system.
 If you are installing this or MinGW in Windows, make sure you install it
-**after** installing the Windows Microsoft C++ Build tools. The :py:mod:`apexpy`
+**after** installing the Windows Microsoft C++ Build tools. You must also make
+sure that the compilers and Python that are installed both use the same
+processing standard (either 32-bit or 64-bit). The :py:mod:`apexpy`
 installation has been tested successfully with gfortran 7 and some more recent
 versions.  Earlier versions of gfortran may not work and are not recommended.
 
 Installation also requires a C compiler of the same type as the fortran
 compiler. `GCC <https://gcc.gnu.org/>`_ is a free compiler that works with
 Gfortran and can be installed from a variety of sources and standard package
 managers. It is recommended that you check to see if you have gcc available on
@@ -121,18 +123,20 @@
 2. Run ``curl -v -H "Authorization: token <GITHUB-ACCESS-TOKEN>" https://api.github.com/repos/aburrell/apexpy/actions/artifacts/<ARTIFACT-ID>/zip``, where
    <ITEM> should be replaced with the appropriate item string.
 3. Copy the URL from the ``Location`` output produced by the previous command
    into a browser, which will download a zip archive into your standard
    download location. Alternatively (or if this doesn't work) you can use
    `wget` to retrieve the archive.
 4. Copy the zip archive into the ``apexpy/dist`` directory and unzip.
-5. Check the archive for the expected matrix of *.whl objects
+5. Check the archive for the expected matrix of ``*.whl`` objects
 
 To install, use ``pip install .``
 
+.. _installation-build:
+
 Build from Source
 ^^^^^^^^^^^^^^^^^
 
 If you intend to modify or contribute to :py:mod:`apexpy`, you should install
 :py:mod:`apexpy` by forking the repository and installing it locally or within
 a virtual environment. After cloning the fork (see :ref:`contributing`),
 you may install by::
@@ -211,14 +215,28 @@
 
 This example assumes you are building
 locally from the cloned Git repository.  Issues on Mac OS have also been
 encountered when using clang for ``CC`` alongside gfortran.  This resulted in a
 seemly successful installation with :py:mod:`apexpy` reporting that fortranapex
 cannot be imported.
 
+Some users have reported unusual behavior when using Anaconda on Apple Silicon
+systems.  Anaconda will attempt to build and install the Intel versions of
+wheels instead of the M1 versions and run everything through Rosetta.  This
+configuration has not been fully evaluated, but it results in a seemly
+successful installation with :py:mod:`apexpy` reporting that fortranapex
+cannot be imported.  Users should confirm that wheels created by conda (both for
+apexpy and other packages) end in ``arm64.whl`` not ``osx-64.whl``.  If the
+later is true, users should consider uninstalling anaconda completely, and
+instead installing miniconda following
+`these instructions <https://conda.io/projects/conda/en/stable/user-guide/install/macos.html>`_,
+which has been confirmed to work. **WARNING:** This will remove any environments
+you have set up and likely undo all IDE settings, so be cautious and consider
+backing up your work first!
+
 
 Windows systems are known to have issues with Fortran-based codes.  The Windows
 testing we do uses miniconda, so we recommend using the Anaconda environment.
 One problem that has been encountered is a lack of LAPACK/BLAS tools that
 causes NumPy to not behave as expected.  This can be fixed by installing
 scipy before NumPy and then installing :py:mod:`apexpy`.
```

### Comparing `apexpy-2.0.0/docs/maintenance.rst` & `apexpy-2.0.1/docs/maintenance.rst`

 * *Files 22% similar despite different names*

```diff
@@ -12,82 +12,56 @@
 
 Updating IGRF
 -------------
 
 The `International Geomagnetic Reference Field <https://www.ngdc.noaa.gov/IAGA/vmod/igrf.html>`_
 is regularly updated to reflect the most recent changes to the Terrestrial
 magnetic field. apexpy currently uses IRGF-13 coefficients, which are provided
-in the ``apexpy/src/apexpy/igrf13coeff.txt`` file. To change or update the
-magnetic field coefficients used by apexpy, you need to update the python code.
+in the ``apexpy/apexpy/igrf13coeff.txt`` file. To change or update the
+magnetic field coefficients used by apexpy, you need to update the python code,
+then rerun the fortran program that builds ``apexpy/apexpy/apexsh.dat``. This 
+is what makes apexpy performant.   For more details, see Emmert et al. [2010] [1]_.
+
 Assuming your new coefficient file has the same format, the process is simple:
 
-1. Clone the repository or your fork of the repository (see :ref:`contributing`)
-2. Update ``apexpy/src/apexpy/apex.py`` variable ``igrf_fn`` by setting
-   it equal to the new target filename
-3. Install the python package from the command line
-   (see :ref:`installation-cmd`)
-
-Updating ``apexsh.dat``
------------------------
-
-After updating the IGRF coefficients file the ``apexsh.dat`` file needs to be
-rebuilt. This file is what makes apexpy performant. For more details, see
-Emmert et al. [2010] [1]_.
-
-Updating ``apexsh.dat`` is done by modifying and building the fortran source
-code in the ``apexpy/src/fortranapex`` directory. Working in that directory:
-
-1. Make sure a copy of the latest IGRF coefficient file is present in the
-   selfsame directory.
-2. Modify the ``igrffilein`` in ``checkapexsh.f90`` to the name of the IGRF
-   coefficient file (``igrf13coeff.txt``, for example).
-3. Modify ``checkapexsh.f90`` by adding the next 5 year epoch to the
+1. Clone the repository or your fork of the repository (see :ref:`contributing`).
+2. Update ``apexpy/apexpy/apex.py`` variable ``igrf_fn`` by setting
+   it equal to the new IGRF coefficient filename (``igrf13coeff.txt``, for example).
+3. In ``apexpy/fortranapex/checkapexsh.f90``, update the variable ``igrffilein``
+   to the new IGRF coefficent filename.  Relative paths are allowed.
+4. Modify ``checkapexsh.f90`` by adding the next 5 year epoch to the
    ``epochgrid`` variable and updating the ``nepochgrid`` variable as
    necessary. For example, if the newest IGRF coefficients are good up to 2025
    and ``epochgrid`` only has up to the year 2020, then add 2025 to
    ``epochgrid`` and then increment ``nepochgrid`` by 1.
-4. Build the ``apextest`` binary by running the ``make`` command.
-5. Copy the IGRF coefficient file (``cp ../apexpy/igrf13coeff.txt``) into the
-   current directory.
-6. Execute the ``apextest`` binary to generate the new ``apexsh.dat`` file.
-7. Copy the new ``apexsh.dat`` file to the ``apexpy/src/apexpy`` directory.
-
-After updating the ``apexsh.dat`` file, some of the unit tests and the
-documentation examples in the README and ``apexpy/docs/examples`` directory
-will need to be updated as well.
+5. Execute the ``apextest`` binary to generate the new ``apexsh.dat`` file.
+6. Update the unit tests in the class ``TestApexMethodExtrapolateIGRF`` in 
+   ``apexpy/apexpy/tests/test_Apex.py`` so that they check the methods are working
+   correctly with dates after the latest IGRF epoch (i.e., if the latest epoch is
+   2020, set the test to initialize with the year 2025).  You will have to update
+   the hard-coded confirmation values used by these tests.
+7. Commit all changes and create a pull request on GitHub to integrate your 
+   branch with updated IGRF into the main repository.
 
 Modifying Fortran Source
 ------------------------
 When modifying the fortran source code, it can be helpful to run a preliminary
-validation of the fortran output independent of the python wrapper.
+validation of the fortran output independent of the python wrapper. This should
+be done within the ``apexpy/fortranapex`` directory.
 
 1. Remove any existing binaries by running the ``make clean`` command.
 2. Build the ``apextest`` binary by running the ``make`` command.
-3. Copy the IGRF coefficient file (``cp ../apexpy/igrf13coeff.txt``) into the
-   current directory.
-4. Execute the ``apextext`` binary.
-5. Confirm the output printed to the screen matches the test output shown in
-   the comment blot at the bottom of ``checkapexsh.f90``.
-
-The output may not match the test output exactly due to floating point errors
-and improvements in the precision of the calculation.
-
-After updating the fortran source code, the signature file must be recreated so
-the python wrapper works correctly.  It is also a good idea to update
-``apexsh.dat`` following the instructions above.  Use `f2py <https://numpy.org/doc/stable/f2py/>`_
-to create a new signature file from the ``apexpy/src/fortranapex`` directory.
-::
-
-  f2py -m fortranapex apexsh.f90 igrf.f90 apex.f90 magfld.f90 makeapexsh.f90 -h fortranapex.pyf --overwrite-signature
-
-
-This will create the file ``fortranapex.pyf``.  Then reinstall the package with
-``pip`` from the root directory.  If the modifications involved adding or
-removing fortran source files, modify the list of extension sources in
-``setup.py``.
+3. Execute the ``apextext`` binary.
+4. Confirm the output printed to the screen matches the test output shown in
+   the comment block at the bottom of ``checkapexsh.f90``. The output may not match 
+   the test output exactly due to floating point errors and improvements in the 
+   precision of the calculation.
+5. If the modifications involved adding or removing fortran source files, modify the 
+   list of extension sources in ``setup.cfg``.
+6. Rebuild and install apexpy following the instructions in :ref:`installation-build`.
 
 Updating tests and style standards
 -----------------------------------
 
 apexpy is in the process of updating unit and integration tests to reduce code
 duplication and implementing cleaner style standards. Additionally, some parts
 of the fortran code adhere to older coding standards and raise warnings when
@@ -95,8 +69,8 @@
 (help would be appreciated), please discuss your potential contribution with
 the current maintainer to ensure a minimal duplication of effort.
 
 
 .. [1] Emmert, J. T., A. D. Richmond, and D. P. Drob (2010),
        A computationally compact representation of Magnetic-Apex
        and Quasi-Dipole coordinates with smooth base vectors,
-       J. Geophys. Res., 115(A8), A08322, :doi:`10.1029/2010JA015326`.
+       J. Geophys. Res., 115(A8), A08322, doi:10.1029/2010JA015326.
```

### Comparing `apexpy-2.0.0/fortranapex/Makefile` & `apexpy-2.0.1/fortranapex/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Ver. 1.0. 27/8-10 - Based on Makefile for Einar Stiansen.
 
 # If using Intel compilers, uncomment a line at the top of the igrf.f90 file
 FC 	= gfortran  # mpif90, ifort
 LD      = $(FC)
 LDFLAGS = #-ipo
-FFLAGS 	= -Wall -O3 -fPIC #-ipo -check bounds -check pointer -check uninit
+FFLAGS 	= -Wall -O3 -fPIC -fcheck=all -fbounds-check -pedantic -Wextra #-ipo -check bounds -check pointer -check uninit
 SFLAGS  = -static #-libgfortran -static-libgcc (AGB, static should work?)
 STATIC  = 0
 
 ifneq ($(STATIC),0)
 	LDFLAGS += $(SFLAGS)
 endif
```

### Comparing `apexpy-2.0.0/fortranapex/apex.f90` & `apexpy-2.0.1/fortranapex/apex.f90`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/fortranapex/apexsh.f90` & `apexpy-2.0.1/fortranapex/apexsh.f90`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/fortranapex/checkapexsh.f90` & `apexpy-2.0.1/fortranapex/checkapexsh.f90`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 program checkapexsh
 
   implicit none
 
   integer(4), parameter :: nepochgrid=26
   ! integer(4), parameter :: nepochgrid=3       ! For testing/debugging
   integer(4)            :: lmax=3, nmmax=6
-  character(1000)       :: apexshfile='apexsh.dat'
-  character(len=1000)   :: igrffilein='igrf13coeffs.txt'
+  character(1000)       :: apexshfile='../apexpy/apexsh.dat'
+  character(len=1000)   :: igrffilein='../apexpy/igrf13coeffs.txt'
   real(8)               :: epochgrid(0:nepochgrid - 1)
   real(8)               :: epoch
   real(8)               :: glat, glon, alt, hr, prec, error
   integer(4)            :: vecflag
   real(8)               :: qlat, qlon, mlat, mlon, rho
   real(8)               :: f1(1:2), f2(1:2), f
   real(8)               :: d1(1:3), d2(1:3), d3(1:3), d
```

### Comparing `apexpy-2.0.0/fortranapex/fortranapex-f2pywrappers2.f90` & `apexpy-2.0.1/fortranapex/fortranapex-f2pywrappers2.f90`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/fortranapex/fortranapex.pyf` & `apexpy-2.0.1/fortranapex/fortranapex.pyf`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/fortranapex/fortranapexmodule.c` & `apexpy-2.0.1/fortranapex/fortranapexmodule.c`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/fortranapex/igrf.f90` & `apexpy-2.0.1/fortranapex/igrf.f90`

 * *Files 4% similar despite different names*

```diff
@@ -44,24 +44,27 @@
     ! Skip comment lines
     do
        read(unit = 100, fmt = '(A)') s
        if (s(1:1) /= '#') exit
     end do
 
     ! Read epochs
-    num_epochs = count([(s(i:i + 3), i = 1, len_trim(s))]== 'IGRF')
-    num_epochs = count([(s(i:i + 3), i = 1, len_trim(s))]== 'DGRF') + num_epochs
+    num_epochs = 0
+    do i=1, len_trim(s)
+      if ((s(i:i+3) == 'IGRF').or.(s(i:i+3) == 'DGRF')) then
+        num_epochs = num_epochs + 1
+      end if
+    end do
     allocate(epoch(1:num_epochs))
     allocate(nmxe(1:num_epochs))
 
     ! Read epochs
-    read(100,*, iostat = state) s
-    do i = 1, num_epochs
-       epoch(i) = 1900.0 + real(i - 1) * 5.0d0
-    end do
+    read(unit = 100, fmt = '(A)', iostat = state) s
+    read(s(8:), *) epoch
+
 
     ! Number of coefficients
     do i = 1, num_epochs
        if (epoch(i) .ge. 2000.0d0) then
           nmxe(i) = 13
        elseif (epoch(i) .ge. 1900.0d0) then
           nmxe(i) = 10
@@ -85,15 +88,15 @@
     close(100)
 
     ! Restore file position, must re-open after reaching EOF
     open(unit=100, file=filename_in, status='old', iostat=state)
     call fseek(100, offset, 0, state)
 
     ! Assign the variables for Gauss coefficients
-    allocate(g(1:num_sh, 1:num_epochs))
+    allocate(g(1:num_sh, 1:num_epochs+1))
     allocate(nm(1:num_sh, 2))
 
     ! Read coefficients
     do i = 1, num_sh
        read(100,*, iostat = state) s, nm(i, 1), nm(i, 2), g(i,:)
        if (state < 0) exit
     end do
```

### Comparing `apexpy-2.0.0/fortranapex/magfld.f90` & `apexpy-2.0.1/fortranapex/magfld.f90`

 * *Files 0% similar despite different names*

```diff
@@ -168,19 +168,19 @@
       write(0, '("COFRM:  DATE "(F9.3)" preceeds earliest available "(F6.1))') date, epoch(1)
       call exit(1)
     elseif (date > epoch(nepo) + 5.) then
       write(0, '("COFRM:  DATE "(F9.3)" is after the last recommended for extrapolation "(F6.1))') date, epoch(1) + 5.
       call exit(1)
     end if
 
-    ! Set the date and time
-    iy = 1
-    do while (date > epoch(iy))
-      iy = iy + 1
+    ! Set the date and time index
+    do iy = 1, nepo
+      if (date < epoch(iy)) exit
     end do
+    iy = iy - 1
 
     ngh = nght * nepo
     nmax1 = int(nmxe(iy))
     ! time = date
     t = date - epoch(iy)
     to5 = t / 5.
     iy1 = iy + 1
```

### Comparing `apexpy-2.0.0/fortranapex/makeapexsh.f90` & `apexpy-2.0.1/fortranapex/makeapexsh.f90`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/fortranapex/readme.txt` & `apexpy-2.0.1/fortranapex/readme.txt`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/meson.build` & `apexpy-2.0.1/meson.build`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 project( 'apexpy', 'c',
   # Note that the git commit hash cannot be added dynamically here
-  version: '2.0.0',
+  version: '2.0.1',
   license: 'MIT',
   meson_version: '>= 0.63.0',
   default_options: [
     'buildtype=debugoptimized',
     # TODO: the below -Wno flags are all needed to silence warnings in
     # f2py-generated code. This should be fixed in f2py itself.
     'c_args=-Wno-unused-function -Wno-conversion -Wno-misleading-indentation -Wno-incompatible-pointer-types',
```

### Comparing `apexpy-2.0.0/pyproject.toml` & `apexpy-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/setup.cfg` & `apexpy-2.0.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apexpy
-version = 2.0.0
+version = 2.0.1
 license = MIT
 description = "A Python wrapper for Apex coordinates"
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/aburrell/apexpy
 keywords =
   apex
```

### Comparing `apexpy-2.0.0/setup.py` & `apexpy-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `apexpy-2.0.0/PKG-INFO` & `apexpy-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apexpy
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python wrapper for Apex coordinates
 Keywords: apex modified apex quasi-dipole quasi dipole coordinates magnetic coordinates mlt magnetic local time conversion converting
 Maintainer-Email: Angeline G. Burrell <angeline.burrell@nrl.navy.mil>
 License: The MIT License (MIT)
         
         Copyright (c) 2015 Christer van der Meeren
         
@@ -55,14 +55,16 @@
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: sphinx>=1.3; extra == "doc"
 Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Provides-Extra: test
 Provides-Extra: doc
 Description-Content-Type: text/x-rst
 
+|logo|
+
 ========
 Overview
 ========
 
 |docs| |version| |doi|
 
 This is a Python wrapper for the Apex fortran library by
@@ -128,16 +130,15 @@
 
 References
 ==========
 
 .. [1] Emmert, J. T., A. D. Richmond, and D. P. Drob (2010),
        A computationally compact representation of Magnetic-Apex
        and Quasi-Dipole coordinates with smooth base vectors,
-       J. Geophys. Res., 115(A8), A08322,
-       `doi:10.1029/2010JA015326 <http://dx.doi.org/10.1029/2010JA015326>`_.
+       J. Geophys. Res., 115(A8), A08322, doi:10.1029/2010JA015326.
 
 .. [2] Richmond, A. D. (1995), Ionospheric Electrodynamics Using
        Magnetic Apex Coordinates, Journal of geomagnetism and
        geoelectricity, 47(2), 191–212,
        `doi:10.5636/jgg.47.191 <http://dx.doi.org/10.5636/jgg.47.191>`_.
 
 Badges
@@ -178,27 +179,30 @@
 
 .. |version| image:: https://img.shields.io/pypi/v/apexpy.svg?style=flat
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/apexpy/
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/apexpy.svg?style=flat
     :alt: PyPI Package monthly downloads
-    :target: https://pypi.python.org/pypi/apexpy
+    :target: https://pypi.org/project/apexpy
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/apexpy.svg?style=flat
     :alt: PyPI Wheel
-    :target: https://pypi.python.org/pypi/apexpy
+    :target: https://pypi.org/project/apexpy
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/apexpy.svg?style=flat
     :alt: Supported versions
-    :target: https://pypi.python.org/pypi/apexpy
+    :target: https://pypi.org/project/apexpy
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/apexpy.svg?style=flat
     :alt: Supported implementations
-    :target: https://pypi.python.org/pypi/apexpy
+    :target: https://pypi.org/project/apexpy
 
 .. |scrutinizer| image:: https://img.shields.io/scrutinizer/quality/g/aburrell/apexpy/main.svg?style=flat
     :alt: Scrutinizer Status
     :target: https://scrutinizer-ci.com/g/aburrell/apexpy/
 
 .. |doi| image:: https://www.zenodo.org/badge/doi/10.5281/zenodo.4585641.svg
    :target: https://doi.org/10.5281/zenodo.1214206
+
+.. |logo| image:: docs/apexpy.png
+   :alt: ApexPy logo: yellow magnetic field lines surrounding the Earth's surface, which is blue
```

