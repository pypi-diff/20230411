# Comparing `tmp/pyright_polite-1.0.4.tar.gz` & `tmp/pyright_polite-1.0.5.tar.gz`

## Comparing `pyright_polite-1.0.4.tar` & `pyright_polite-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/.justfile
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/.pylintrc
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/setup.cfg
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/__about__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/__init__.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/cli.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/main.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/platform.py
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/polite.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/src/pyright_polite/pyright.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/LICENSE
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/README.md
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/hatch.toml
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 pyright_polite-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/.justfile
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/.pylintrc
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/src/pyright_polite/__about__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/src/pyright_polite/__init__.py
+-rw-r--r--   0        0        0     8743 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/src/pyright_polite/cli.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/src/pyright_polite/main.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/src/pyright_polite/platform.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/src/pyright_polite/polite.py
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/src/pyright_polite/pyright.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/LICENSE
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/README.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/hatch.toml
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 pyright_polite-1.0.5/PKG-INFO
```

### Comparing `pyright_polite-1.0.4/.justfile` & `pyright_polite-1.0.5/.justfile`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/.pre-commit-config.yaml` & `pyright_polite-1.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/CHANGELOG.md` & `pyright_polite-1.0.5/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,23 @@
 
+<a id='changelog-v1.0.5'></a>
+# v1.0.5 — 2023-04-11
+
+## Removed
+
+- Removed unnecessary `setup.cfg`.
+
+## Added
+
+- Added some more tests.
+
+## Changed
+
+- Tiny bit of code refactoring.
+
 <a id='changelog-v1.0.4'></a>
 # v1.0.4 — 2023-04-10
 
 ## Added
 
 - Add `__slots__` to `Polite` class.
```

### Comparing `pyright_polite-1.0.4/src/pyright_polite/cli.py` & `pyright_polite-1.0.5/src/pyright_polite/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,26 +196,21 @@
 
 def deduce_mode(args: List[str]) -> Mode:
     """Deduce the mode of operation based on the arguments passed to pyright.
 
     Returns:
         Mode: The deduced mode of operation.
     """
-    mode: Mode = Mode.JSON
-
     if "--outputjson" in args:
-        return mode
-
-    if any(arg in PLAINTEXT_ARGS for arg in args):
-        mode = Mode.PLAINTEXT
+        return Mode.JSON
 
     if any(arg in UNFILTERED_ARGS for arg in args):
-        mode = Mode.UNFILTERED
+        return Mode.UNFILTERED
 
-    return mode
+    return Mode.PLAINTEXT
 
 
 def parse_cli() -> CommandLine:
     """Handle command-line arguments.
 
     Returns:
         CommandLine: The argv list and the deduced mode of operation.
```

### Comparing `pyright_polite-1.0.4/src/pyright_polite/main.py` & `pyright_polite-1.0.5/src/pyright_polite/main.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/src/pyright_polite/platform.py` & `pyright_polite-1.0.5/src/pyright_polite/platform.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/src/pyright_polite/polite.py` & `pyright_polite-1.0.5/src/pyright_polite/polite.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/src/pyright_polite/pyright.py` & `pyright_polite-1.0.5/src/pyright_polite/pyright.py`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/.gitignore` & `pyright_polite-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/LICENSE` & `pyright_polite-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/README.md` & `pyright_polite-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/hatch.toml` & `pyright_polite-1.0.5/hatch.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,81 +6,82 @@
 00000050: 6520 3d20 5b0a 2020 222f 2e63 6861 6e67  e = [.  "/.chang
 00000060: 656c 6f67 2e64 222c 0a20 2022 2f2e 6769  elog.d",.  "/.gi
 00000070: 7468 7562 222c 0a20 2022 2f70 6163 6b61  thub",.  "/packa
 00000080: 6765 2d6c 6f63 6b2e 6a73 6f6e 222c 0a20  ge-lock.json",. 
 00000090: 2022 2f70 6163 6b61 6765 2e6a 736f 6e22   "/package.json"
 000000a0: 2c0a 2020 222f 7465 7374 7322 2c0a 5d0a  ,.  "/tests",.].
 000000b0: 0a23 204c 6f63 616c 2074 6573 7473 0a5b  .# Local tests.[
-000000c0: 656e 7673 2e64 6566 6175 6c74 5d0a 6465  envs.default].de
-000000d0: 7065 6e64 656e 6369 6573 203d 205b 0a20  pendencies = [. 
-000000e0: 2022 626c 6163 6b20 3e3d 2032 332e 312e   "black >= 23.1.
-000000f0: 3022 2c0a 2020 2263 6f76 6572 6167 6520  0",.  "coverage 
-00000100: 7e3d 2037 2e32 222c 0a20 2022 7072 652d  ~= 7.2",.  "pre-
-00000110: 636f 6d6d 6974 207e 3d20 332e 3222 2c0a  commit ~= 3.2",.
-00000120: 2020 2270 796c 696e 7420 7e3d 2032 2e31    "pylint ~= 2.1
-00000130: 3722 2c0a 2020 2270 7974 6573 7420 7e3d  7",.  "pytest ~=
-00000140: 2037 2e32 222c 0a20 2022 7079 7465 7374   7.2",.  "pytest
-00000150: 2d61 7379 6e63 696f 207e 3d20 302e 3231  -asyncio ~= 0.21
-00000160: 222c 0a20 2022 7275 6666 203e 3d20 302e  ",.  "ruff >= 0.
-00000170: 302e 3235 3722 2c0a 2020 2273 6372 6976  0.257",.  "scriv
-00000180: 203e 3d20 312e 322e 3122 2c0a 2020 2273   >= 1.2.1",.  "s
-00000190: 736f 7274 203e 3d20 302e 3131 2e36 222c  sort >= 0.11.6",
-000001a0: 0a5d 0a5b 656e 7673 2e64 6566 6175 6c74  .].[envs.default
-000001b0: 2e73 6372 6970 7473 5d0a 636f 7620 3d20  .scripts].cov = 
-000001c0: 5b22 636f 7665 7261 6765 2072 756e 207b  ["coverage run {
-000001d0: 6172 6773 7d22 2c20 2263 6f76 6572 6167  args}", "coverag
-000001e0: 6520 7265 706f 7274 202d 6d22 5d0a 6c69  e report -m"].li
-000001f0: 6e74 203d 205b 0a20 2022 2d20 7275 6666  nt = [.  "- ruff
-00000200: 2063 6865 636b 202e 222c 0a20 2022 2d20   check .",.  "- 
-00000210: 7079 6c69 6e74 2073 7263 222c 0a20 2022  pylint src",.  "
-00000220: 2d20 626c 6163 6b20 2d2d 7175 6965 7420  - black --quiet 
-00000230: 2d2d 6368 6563 6b20 2d2d 6469 6666 202e  --check --diff .
-00000240: 222c 0a20 2022 2d20 7079 7269 6768 742d  ",.  "- pyright-
-00000250: 706f 6c69 7465 2073 7263 2074 6573 7473  polite src tests
-00000260: 2f74 6573 745f 2a2e 7079 222c 0a20 2022  /test_*.py",.  "
-00000270: 2d20 7373 6f72 7420 2d2d 6368 6563 6b20  - ssort --check 
-00000280: 2d2d 6469 6666 2073 7263 222c 0a5d 0a0a  --diff src",.]..
-00000290: 2320 5465 6d70 6c61 7465 730a 5b65 6e76  # Templates.[env
-000002a0: 732e 6261 7365 5d0a 6465 7065 6e64 656e  s.base].dependen
-000002b0: 6369 6573 203d 205b 0a20 2022 636f 7665  cies = [.  "cove
-000002c0: 7261 6765 207e 3d20 372e 3222 2c0a 2020  rage ~= 7.2",.  
-000002d0: 2270 7974 6573 7420 7e3d 2037 2e32 222c  "pytest ~= 7.2",
-000002e0: 0a20 2022 7079 7465 7374 2d61 7379 6e63  .  "pytest-async
-000002f0: 696f 207e 3d20 302e 3231 222c 0a5d 0a0a  io ~= 0.21",.]..
-00000300: 2320 7079 656e 760a 5b65 6e76 732e 7079  # pyenv.[envs.py
-00000310: 656e 765d 0a74 656d 706c 6174 6520 3d20  env].template = 
-00000320: 2262 6173 6522 0a70 6c61 7466 6f72 6d73  "base".platforms
-00000330: 203d 205b 226c 696e 7578 225d 0a5b 656e   = ["linux"].[en
-00000340: 7673 2e70 7965 6e76 2e73 6372 6970 7473  vs.pyenv.scripts
-00000350: 5d0a 636f 7620 3d20 5b22 636f 7665 7261  ].cov = ["covera
-00000360: 6765 2072 756e 207b 6172 6773 7d22 2c20  ge run {args}", 
-00000370: 2263 6f76 6572 6167 6520 7265 706f 7274  "coverage report
-00000380: 202d 6d22 5d0a 7465 7374 203d 205b 2270   -m"].test = ["p
-00000390: 7974 6573 7420 7b61 7267 737d 225d 0a5b  ytest {args}"].[
-000003a0: 5b65 6e76 732e 7079 656e 762e 6d61 7472  [envs.pyenv.matr
-000003b0: 6978 5d5d 0a70 7974 686f 6e20 3d20 5b22  ix]].python = ["
-000003c0: 332e 3722 2c20 2233 2e38 222c 2022 332e  3.7", "3.8", "3.
-000003d0: 3922 2c20 2233 2e31 3022 2c20 2233 2e31  9", "3.10", "3.1
-000003e0: 3122 5d0a 0a23 2047 6974 4875 6220 576f  1"]..# GitHub Wo
-000003f0: 726b 666c 6f77 3a20 4349 0a5b 656e 7673  rkflow: CI.[envs
-00000400: 2e63 695d 0a74 656d 706c 6174 6520 3d20  .ci].template = 
-00000410: 2262 6173 6522 0a70 6c61 7466 6f72 6d73  "base".platforms
-00000420: 203d 205b 226c 696e 7578 222c 2022 6d61   = ["linux", "ma
-00000430: 636f 7322 2c20 2277 696e 646f 7773 225d  cos", "windows"]
-00000440: 0a5b 656e 7673 2e63 692e 7363 7269 7074  .[envs.ci.script
-00000450: 735d 0a63 6f76 203d 205b 2263 6f76 6572  s].cov = ["cover
-00000460: 6167 6520 7275 6e20 7b61 7267 737d 222c  age run {args}",
-00000470: 2022 636f 7665 7261 6765 2063 6f6d 6269   "coverage combi
-00000480: 6e65 202d 7120 2d2d 6b65 6570 222c 2022  ne -q --keep", "
-00000490: 636f 7665 7261 6765 2072 6570 6f72 7420  coverage report 
-000004a0: 2d6d 225d 0a63 6f76 2d63 6f6d 6269 6e65  -m"].cov-combine
-000004b0: 203d 205b 2263 6f76 6572 6167 6520 636f   = ["coverage co
-000004c0: 6d62 696e 6520 2d71 222c 2022 636f 7665  mbine -q", "cove
-000004d0: 7261 6765 206a 736f 6e20 2d71 202d 6f20  rage json -q -o 
-000004e0: 636f 7665 7261 6765 2e6a 736f 6e22 5d0a  coverage.json"].
-000004f0: 5b5b 656e 7673 2e63 692e 6d61 7472 6978  [[envs.ci.matrix
-00000500: 5d5d 0a70 7974 686f 6e20 3d20 5b22 332e  ]].python = ["3.
-00000510: 3722 2c20 2233 2e38 222c 2022 332e 3922  7", "3.8", "3.9"
-00000520: 2c20 2233 2e31 3022 2c20 2233 2e31 3122  , "3.10", "3.11"
-00000530: 2c20 2270 7970 7933 2e37 222c 2022 7079  , "pypy3.7", "py
-00000540: 7079 332e 3822 2c20 2270 7970 7933 2e39  py3.8", "pypy3.9
-00000550: 225d 0a                                  "].
+000000c0: 656e 7673 2e64 6566 6175 6c74 5d0a 7079  envs.default].py
+000000d0: 7468 6f6e 203d 2022 332e 3131 220a 6465  thon = "3.11".de
+000000e0: 7065 6e64 656e 6369 6573 203d 205b 0a20  pendencies = [. 
+000000f0: 2022 626c 6163 6b20 3e3d 2032 332e 312e   "black >= 23.1.
+00000100: 3022 2c0a 2020 2263 6f76 6572 6167 6520  0",.  "coverage 
+00000110: 7e3d 2037 2e32 222c 0a20 2022 7072 652d  ~= 7.2",.  "pre-
+00000120: 636f 6d6d 6974 207e 3d20 332e 3222 2c0a  commit ~= 3.2",.
+00000130: 2020 2270 796c 696e 7420 7e3d 2032 2e31    "pylint ~= 2.1
+00000140: 3722 2c0a 2020 2270 7974 6573 7420 7e3d  7",.  "pytest ~=
+00000150: 2037 2e32 222c 0a20 2022 7079 7465 7374   7.2",.  "pytest
+00000160: 2d61 7379 6e63 696f 207e 3d20 302e 3231  -asyncio ~= 0.21
+00000170: 222c 0a20 2022 7275 6666 203e 3d20 302e  ",.  "ruff >= 0.
+00000180: 302e 3235 3722 2c0a 2020 2273 6372 6976  0.257",.  "scriv
+00000190: 203e 3d20 312e 322e 3122 2c0a 2020 2273   >= 1.2.1",.  "s
+000001a0: 736f 7274 203e 3d20 302e 3131 2e36 222c  sort >= 0.11.6",
+000001b0: 0a5d 0a5b 656e 7673 2e64 6566 6175 6c74  .].[envs.default
+000001c0: 2e73 6372 6970 7473 5d0a 636f 7620 3d20  .scripts].cov = 
+000001d0: 5b22 636f 7665 7261 6765 2072 756e 207b  ["coverage run {
+000001e0: 6172 6773 7d22 2c20 2263 6f76 6572 6167  args}", "coverag
+000001f0: 6520 7265 706f 7274 202d 6d22 5d0a 6c69  e report -m"].li
+00000200: 6e74 203d 205b 0a20 2022 2d20 7275 6666  nt = [.  "- ruff
+00000210: 2063 6865 636b 202e 222c 0a20 2022 2d20   check .",.  "- 
+00000220: 7079 6c69 6e74 2073 7263 222c 0a20 2022  pylint src",.  "
+00000230: 2d20 626c 6163 6b20 2d2d 7175 6965 7420  - black --quiet 
+00000240: 2d2d 6368 6563 6b20 2d2d 6469 6666 202e  --check --diff .
+00000250: 222c 0a20 2022 2d20 7079 7269 6768 742d  ",.  "- pyright-
+00000260: 706f 6c69 7465 2073 7263 2074 6573 7473  polite src tests
+00000270: 2f74 6573 745f 2a2e 7079 222c 0a20 2022  /test_*.py",.  "
+00000280: 2d20 7373 6f72 7420 2d2d 6368 6563 6b20  - ssort --check 
+00000290: 2d2d 6469 6666 2073 7263 222c 0a5d 0a0a  --diff src",.]..
+000002a0: 2320 5465 6d70 6c61 7465 730a 5b65 6e76  # Templates.[env
+000002b0: 732e 6261 7365 5d0a 6465 7065 6e64 656e  s.base].dependen
+000002c0: 6369 6573 203d 205b 0a20 2022 636f 7665  cies = [.  "cove
+000002d0: 7261 6765 207e 3d20 372e 3222 2c0a 2020  rage ~= 7.2",.  
+000002e0: 2270 7974 6573 7420 7e3d 2037 2e32 222c  "pytest ~= 7.2",
+000002f0: 0a20 2022 7079 7465 7374 2d61 7379 6e63  .  "pytest-async
+00000300: 696f 207e 3d20 302e 3231 222c 0a5d 0a0a  io ~= 0.21",.]..
+00000310: 2320 7079 656e 760a 5b65 6e76 732e 7079  # pyenv.[envs.py
+00000320: 656e 765d 0a74 656d 706c 6174 6520 3d20  env].template = 
+00000330: 2262 6173 6522 0a70 6c61 7466 6f72 6d73  "base".platforms
+00000340: 203d 205b 226c 696e 7578 225d 0a5b 656e   = ["linux"].[en
+00000350: 7673 2e70 7965 6e76 2e73 6372 6970 7473  vs.pyenv.scripts
+00000360: 5d0a 636f 7620 3d20 5b22 636f 7665 7261  ].cov = ["covera
+00000370: 6765 2072 756e 207b 6172 6773 7d22 2c20  ge run {args}", 
+00000380: 2263 6f76 6572 6167 6520 7265 706f 7274  "coverage report
+00000390: 202d 6d22 5d0a 7465 7374 203d 205b 2270   -m"].test = ["p
+000003a0: 7974 6573 7420 7b61 7267 737d 225d 0a5b  ytest {args}"].[
+000003b0: 5b65 6e76 732e 7079 656e 762e 6d61 7472  [envs.pyenv.matr
+000003c0: 6978 5d5d 0a70 7974 686f 6e20 3d20 5b22  ix]].python = ["
+000003d0: 332e 3722 2c20 2233 2e38 222c 2022 332e  3.7", "3.8", "3.
+000003e0: 3922 2c20 2233 2e31 3022 2c20 2233 2e31  9", "3.10", "3.1
+000003f0: 3122 5d0a 0a23 2047 6974 4875 6220 576f  1"]..# GitHub Wo
+00000400: 726b 666c 6f77 3a20 4349 0a5b 656e 7673  rkflow: CI.[envs
+00000410: 2e63 695d 0a74 656d 706c 6174 6520 3d20  .ci].template = 
+00000420: 2262 6173 6522 0a70 6c61 7466 6f72 6d73  "base".platforms
+00000430: 203d 205b 226c 696e 7578 222c 2022 6d61   = ["linux", "ma
+00000440: 636f 7322 2c20 2277 696e 646f 7773 225d  cos", "windows"]
+00000450: 0a5b 656e 7673 2e63 692e 7363 7269 7074  .[envs.ci.script
+00000460: 735d 0a63 6f76 203d 205b 2263 6f76 6572  s].cov = ["cover
+00000470: 6167 6520 7275 6e20 7b61 7267 737d 222c  age run {args}",
+00000480: 2022 636f 7665 7261 6765 2063 6f6d 6269   "coverage combi
+00000490: 6e65 202d 7120 2d2d 6b65 6570 222c 2022  ne -q --keep", "
+000004a0: 636f 7665 7261 6765 2072 6570 6f72 7420  coverage report 
+000004b0: 2d6d 225d 0a63 6f76 2d63 6f6d 6269 6e65  -m"].cov-combine
+000004c0: 203d 205b 2263 6f76 6572 6167 6520 636f   = ["coverage co
+000004d0: 6d62 696e 6520 2d71 222c 2022 636f 7665  mbine -q", "cove
+000004e0: 7261 6765 206a 736f 6e20 2d71 202d 6f20  rage json -q -o 
+000004f0: 636f 7665 7261 6765 2e6a 736f 6e22 5d0a  coverage.json"].
+00000500: 5b5b 656e 7673 2e63 692e 6d61 7472 6978  [[envs.ci.matrix
+00000510: 5d5d 0a70 7974 686f 6e20 3d20 5b22 332e  ]].python = ["3.
+00000520: 3722 2c20 2233 2e38 222c 2022 332e 3922  7", "3.8", "3.9"
+00000530: 2c20 2233 2e31 3022 2c20 2233 2e31 3122  , "3.10", "3.11"
+00000540: 2c20 2270 7970 7933 2e37 222c 2022 7079  , "pypy3.7", "py
+00000550: 7079 332e 3822 2c20 2270 7970 7933 2e39  py3.8", "pypy3.9
+00000560: 225d 0a                                  "].
```

### Comparing `pyright_polite-1.0.4/pyproject.toml` & `pyright_polite-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyright_polite-1.0.4/PKG-INFO` & `pyright_polite-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright-polite
-Version: 1.0.4
+Version: 1.0.5
 Summary: An intelligent cross-platform wrapper for pyright that makes it less noisy.
 Project-URL: Homepage, https://github.com/jamielinux/pyright-polite
 Project-URL: Issues, https://github.com/jamielinux/pyright-polite/issues
 Project-URL: Source, https://github.com/jamielinux/pyright-polite
 Author-email: Jamie Nguyen <j@jamielinux.com>
 License-Expression: MIT
 License-File: LICENSE
```

