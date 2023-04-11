# Comparing `tmp/atomic_counter-0.1.0.tar.gz` & `tmp/atomic_counter-0.1.1.tar.gz`

## Comparing `atomic_counter-0.1.0.tar` & `atomic_counter-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,21 @@
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 atomic_counter-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     3352 2022-10-06 21:15:08.000000 atomic_counter-0.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0      501       20      118 2022-10-06 21:15:08.000000 atomic_counter-0.1.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1985 2022-10-06 21:16:27.000000 atomic_counter-0.1.0/.github/workflows/build.yml
--rw-r--r--   0      501       20     1799 2022-10-06 21:07:49.000000 atomic_counter-0.1.0/.gitignore
--rw-r--r--   0      501       20    11352 2022-10-06 21:11:58.000000 atomic_counter-0.1.0/LICENSE
--rw-r--r--   0      501       20      467 2022-10-06 21:12:05.000000 atomic_counter-0.1.0/Makefile
--rw-r--r--   0      501       20      589 2022-10-06 21:14:24.000000 atomic_counter-0.1.0/README.md
--rw-r--r--   0      501       20       14 2022-10-06 21:10:37.000000 atomic_counter-0.1.0/atomic_counter/__init__.py
--rw-r--r--   0      501       20      612 2022-10-06 21:14:27.000000 atomic_counter-0.1.0/pyproject.toml
--rw-r--r--   0      501       20      220 2022-10-06 21:16:41.000000 atomic_counter-0.1.0/src/lib.rs
--rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 atomic_counter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 atomic_counter-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123      410 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.bumpversion.cfg
+-rw-r--r--   0     1001      123      147 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.gitattributes
+-rw-r--r--   0     1001      123     3352 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123      206 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.github/dependabot.yml
+-rw-r--r--   0     1001      123     1690 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0     1001      123     4134 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      123     1817 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/.gitignore
+-rw-r--r--   0     1001      123    11352 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/LICENSE
+-rw-r--r--   0     1001      123      284 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/MANIFEST.in
+-rw-r--r--   0     1001      123     2266 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/Makefile
+-rw-r--r--   0     1001      123     1730 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/README.md
+-rw-r--r--   0     1001      123      545 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/atomic_counter/__init__.py
+-rw-r--r--   0     1001      123      454 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/atomic_counter/tests/test_daily.py
+-rw-r--r--   0     1001      123       78 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/atomic_counter/tests/test_exports.py
+-rw-r--r--   0     1001      123      930 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/atomic_counter/tests/test_offset.py
+-rw-r--r--   0     1001      123     1130 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     1166 2023-04-11 00:02:27.000000 atomic_counter-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123       10 2023-04-11 00:03:00.000000 atomic_counter-0.1.1/wheelhouse/atomic_counter-0.1.1.tar.gz
+-rw-r--r--   0     1001      123    18299 2023-04-11 00:02:58.000000 atomic_counter-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 atomic_counter-0.1.1/PKG-INFO
```

### Comparing `atomic_counter-0.1.0/.github/CODE_OF_CONDUCT.md` & `atomic_counter-0.1.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `atomic_counter-0.1.0/.gitignore` & `atomic_counter-0.1.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
+*.dylib
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
@@ -42,14 +43,15 @@
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
+junit.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 
 # Translations
 *.mo
```

### Comparing `atomic_counter-0.1.0/LICENSE` & `atomic_counter-0.1.1/LICENSE`

 * *Files identical despite different names*

