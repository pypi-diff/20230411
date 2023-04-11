# Comparing `tmp/pypdfium2-4.5.0.tar.gz` & `tmp/pypdfium2-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfium2-4.5.0.tar", last modified: Tue Apr  4 04:01:23 2023, max compression
+gzip compressed data, was "pypdfium2-4.6.0.tar", last modified: Tue Apr 11 04:01:21 2023, max compression
```

## Comparing `pypdfium2-4.5.0.tar` & `pypdfium2-4.6.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.451336 pypdfium2-4.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.435337 pypdfium2-4.5.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/.reuse/dep5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.435337 pypdfium2-4.5.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/LICENSES/LicenseRef-PdfiumThirdParty.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40453 2023-04-04 04:01:23.451336 pypdfium2-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39350 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 04:01:23.451336 pypdfium2-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.431337 pypdfium2-4.5.0/setupsrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.439337 pypdfium2-4.5.0/setupsrc/pypdfium2_setup/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/setupsrc/pypdfium2_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/setupsrc/pypdfium2_setup/autorelease.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11023 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/setupsrc/pypdfium2_setup/build_pdfium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/setupsrc/pypdfium2_setup/craft_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/setupsrc/pypdfium2_setup/packaging_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/setupsrc/pypdfium2_setup/setup_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6272 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/setupsrc/pypdfium2_setup/update_pdfium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.431337 pypdfium2-4.5.0/sourcebuild/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.439337 pypdfium2-4.5.0/sourcebuild/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/sourcebuild/patches/public_headers.patch
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/sourcebuild/patches/shared_library.patch
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/sourcebuild/patches/syslibs_sourcebuild.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.439337 pypdfium2-4.5.0/sourcebuild/patches/win/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/sourcebuild/patches/win/build.patch
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/sourcebuild/patches/win/pdfium.patch
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/sourcebuild/patches/win/resources.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.431337 pypdfium2-4.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.439337 pypdfium2-4.5.0/src/pypdfium2/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.447337 pypdfium2-4.5.0/src/pypdfium2/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/arrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/extract_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/extract_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/imgtopdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/pdfinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_cli/toc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.447337 pypdfium2-4.5.0/src/pypdfium2/_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.451336 pypdfium2-4.5.0/src/pypdfium2/_helpers/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/_internal/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/_internal/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    26676 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19620 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/textpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/_helpers/unsupported.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-04 04:00:42.000000 pypdfium2-4.5.0/src/pypdfium2/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-04 04:01:05.000000 pypdfium2-4.5.0/src/pypdfium2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:01:23.443337 pypdfium2-4.5.0/src/pypdfium2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40453 2023-04-04 04:01:23.000000 pypdfium2-4.5.0/src/pypdfium2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-04 04:01:23.000000 pypdfium2-4.5.0/src/pypdfium2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 04:01:23.000000 pypdfium2-4.5.0/src/pypdfium2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-04 04:01:23.000000 pypdfium2-4.5.0/src/pypdfium2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 04:01:23.000000 pypdfium2-4.5.0/src/pypdfium2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.688130 pypdfium2-4.6.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/.reuse/dep5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/LICENSES/LicenseRef-PdfiumThirdParty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40453 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39350 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.688130 pypdfium2-4.6.0/setupsrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/autorelease.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11023 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/build_pdfium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/craft_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/packaging_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/setup_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6272 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/setupsrc/pypdfium2_setup/update_pdfium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.688130 pypdfium2-4.6.0/sourcebuild/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/sourcebuild/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/public_headers.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/shared_library.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/syslibs_sourcebuild.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/sourcebuild/patches/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/win/build.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/win/pdfium.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/sourcebuild/patches/win/resources.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.688130 pypdfium2-4.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/src/pypdfium2/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/src/pypdfium2/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/arrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/extract_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/extract_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/imgtopdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/pdfinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_cli/toc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/src/pypdfium2/_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.696130 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26676 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/textpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/_helpers/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 04:00:40.000000 pypdfium2-4.6.0/src/pypdfium2/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 04:01:04.000000 pypdfium2-4.6.0/src/pypdfium2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:21.692130 pypdfium2-4.6.0/src/pypdfium2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40453 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 04:01:21.000000 pypdfium2-4.6.0/src/pypdfium2.egg-info/top_level.txt
```

### Comparing `pypdfium2-4.5.0/.reuse/dep5` & `pypdfium2-4.6.0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/LICENSES/Apache-2.0.txt` & `pypdfium2-4.6.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/LICENSES/BSD-3-Clause.txt` & `pypdfium2-4.6.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/LICENSES/CC-BY-4.0.txt` & `pypdfium2-4.6.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/LICENSES/LicenseRef-PdfiumThirdParty.txt` & `pypdfium2-4.6.0/LICENSES/LicenseRef-PdfiumThirdParty.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/MANIFEST.in` & `pypdfium2-4.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/PKG-INFO` & `pypdfium2-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdfium2
-Version: 4.5.0
+Version: 4.6.0
 Summary: Python bindings to PDFium
 Author: pypdfium2-team
 Author-email: geisserml <geisserml@gmail.com>
 License: Apache-2.0 or BSD-3-Clause
 Project-URL: homepage, https://github.com/pypdfium2-team/pypdfium2
 Project-URL: documentation, https://pypdfium2.readthedocs.io/
 Project-URL: changelog, https://pypdfium2.readthedocs.io/en/stable/changelog.html
```

### Comparing `pypdfium2-4.5.0/README.md` & `pypdfium2-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/pyproject.toml` & `pypdfium2-4.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/setup.py` & `pypdfium2-4.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/setupsrc/pypdfium2_setup/autorelease.py` & `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/autorelease.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/setupsrc/pypdfium2_setup/build_pdfium.py` & `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/build_pdfium.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/setupsrc/pypdfium2_setup/craft_packages.py` & `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/craft_packages.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/setupsrc/pypdfium2_setup/packaging_base.py` & `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/packaging_base.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/setupsrc/pypdfium2_setup/setup_base.py` & `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/setup_base.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/setupsrc/pypdfium2_setup/update_pdfium.py` & `pypdfium2-4.6.0/setupsrc/pypdfium2_setup/update_pdfium.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/sourcebuild/patches/public_headers.patch` & `pypdfium2-4.6.0/sourcebuild/patches/public_headers.patch`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/sourcebuild/patches/win/resources.rc` & `pypdfium2-4.6.0/sourcebuild/patches/win/resources.rc`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/__main__.py` & `pypdfium2-4.6.0/src/pypdfium2/__main__.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/_parsers.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/_parsers.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/arrange.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/arrange.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/attachments.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/attachments.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/extract_images.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/extract_images.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/extract_text.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/extract_text.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/imgtopdf.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/imgtopdf.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/pageobjects.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/pageobjects.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/pdfinfo.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/pdfinfo.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/render.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/render.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/tile.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/tile.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_cli/toc.py` & `pypdfium2-4.6.0/src/pypdfium2/_cli/toc.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/__init__.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/_internal/bases.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/bases.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         
         self._finalizer = None
         if needs_free:
             self._attach_finalizer()
     
     
     def _attach_finalizer(self):
+        # this function captures the value of the `parent` property at finalizer installation time - if it changes, detach the old finalizer and create a new one
         assert self._finalizer is None
-        # FIXME if `parent` may change after finalizer installation, we've got a problem...
         self._finalizer = weakref.finalize(self._obj, AutoCloseable._close_template, self._close_func, self.raw, self._uuid, self.parent, *self._ex_args, **self._ex_kwargs)
     
     def _detach_finalizer(self):
         self._finalizer.detach()
         self._finalizer = None
     
     def _tree_closed(self):
@@ -69,13 +69,14 @@
         # TODO add needs_parent safety check (if True, `parent` must be given)
         if (parent is not None) and parent._tree_closed():
             print(f"Parent closed before child - this is illegal ({parent}, {raw}).", file=sys.stderr)
         close_func(raw, *args, **kwargs)
     
     
     def close(self):
+        # TODO? issue a warning if needs_free=False ?
         if (self.raw is None):
             logger.warning(f"Duplicate close call suppressed on {self}.")
             return
         if self._finalizer is not None:
             self._finalizer()
             self.raw = None
```

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/_internal/consts.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/consts.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/_internal/utils.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/attachment.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/attachment.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/bitmap.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/bitmap.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/document.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/document.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/matrix.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/matrix.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/page.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,25 +204,25 @@
         """
         
         if pageobj.page:
             raise ValueError("The pageobject you attempted to insert already belongs to a page.")
         if pageobj.pdf and (pageobj.pdf is not self.pdf):
             raise ValueError("The pageobject you attempted to insert belongs to a different PDF.")
         
-        # If PDFium's API allowed inserting a page object into multiple pages, our support model would need to be changed accordingly
         pdfium_c.FPDFPage_InsertObject(self, pageobj)
         pageobj._detach_finalizer()
         pageobj.page = self
         pageobj.pdf = self.pdf
     
     
     def remove_obj(self, pageobj):
         """
         Remove a page object from the page.
-        The page object must not be used afterwards, except for its ``close()`` method.
+        As of PDFium 5692, detached page objects may be only re-inserted into existing pages of the same document.
+        If the page object is not re-inserted into a page, its ``close()`` method may be called.
         
         Parameters:
             pageobj (PdfObject): The page object to remove.
         """
                 
         if pageobj.page is not self:
             raise ValueError("The page object you attempted to remove is not part of this page.")
```

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/pageobjects.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/pageobjects.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/textpage.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/textpage.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/_helpers/unsupported.py` & `pypdfium2-4.6.0/src/pypdfium2/_helpers/unsupported.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.5.0/src/pypdfium2/version.py` & `pypdfium2-4.6.0/src/pypdfium2/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-FileCopyrightText: 2023 geisserml <geisserml@gmail.com>
 # SPDX-License-Identifier: Apache-2.0 OR BSD-3-Clause
 
 __all__ = ["V_PYPDFIUM2", "V_LIBPDFIUM", "V_BUILDNAME", "V_PDFIUM_IS_V8"]
 
 V_MAJOR = 4
-V_MINOR = 5
+V_MINOR = 6
 V_PATCH = 0
 V_BETA = None
 
 #: pypdfium2 version string
 V_PYPDFIUM2 = f"{V_MAJOR}.{V_MINOR}.{V_PATCH}"
 if V_BETA is not None:
     V_PYPDFIUM2 += f"b{V_BETA}"
 
 #: PDFium library version string (git tag or commit hash)
-V_LIBPDFIUM = "5692"
+V_LIBPDFIUM = "5705"
 
 #: String describing the included PDFium binary's origin (pdfium-binaries, source)
 V_BUILDNAME = "pdfium-binaries"
 
 #: Whether the included PDFium binary was built with V8 support or not
 V_PDFIUM_IS_V8 = False
```

### Comparing `pypdfium2-4.5.0/src/pypdfium2.egg-info/PKG-INFO` & `pypdfium2-4.6.0/src/pypdfium2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdfium2
-Version: 4.5.0
+Version: 4.6.0
 Summary: Python bindings to PDFium
 Author: pypdfium2-team
 Author-email: geisserml <geisserml@gmail.com>
 License: Apache-2.0 or BSD-3-Clause
 Project-URL: homepage, https://github.com/pypdfium2-team/pypdfium2
 Project-URL: documentation, https://pypdfium2.readthedocs.io/
 Project-URL: changelog, https://pypdfium2.readthedocs.io/en/stable/changelog.html
```

### Comparing `pypdfium2-4.5.0/src/pypdfium2.egg-info/SOURCES.txt` & `pypdfium2-4.6.0/src/pypdfium2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

