# Comparing `tmp/riscv-assembler-1.0.9.tar.gz` & `tmp/riscv-assembler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riscv-assembler-1.0.9.tar", last modified: Thu Dec 24 03:52:21 2020, max compression
+gzip compressed data, was "riscv-assembler-1.1.0.tar", last modified: Tue Apr 11 03:54:41 2023, max compression
```

## Comparing `riscv-assembler-1.0.9.tar` & `riscv-assembler-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,56 @@
-drwxr-xr-x   0 kayacelebi   (501) staff       (20)        0 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/
--rw-r--r--   0 kayacelebi   (501) staff       (20)    10815 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/PKG-INFO
--rw-r--r--   0 kayacelebi   (501) staff       (20)     8864 2020-12-24 03:51:30.000000 riscv-assembler-1.0.9/README.md
-drwxr-xr-x   0 kayacelebi   (501) staff       (20)        0 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/riscv_assembler/
--rw-r--r--   0 kayacelebi   (501) staff       (20)      231 2020-12-24 03:34:22.000000 riscv-assembler-1.0.9/riscv_assembler/__init__.py
--rw-r--r--   0 kayacelebi   (501) staff       (20)    13625 2020-12-24 03:47:36.000000 riscv-assembler-1.0.9/riscv_assembler/convert.py
-drwxr-xr-x   0 kayacelebi   (501) staff       (20)        0 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/riscv_assembler/data/
--rw-r--r--   0 kayacelebi   (501) staff       (20)     1416 2020-12-23 09:25:11.000000 riscv-assembler-1.0.9/riscv_assembler/data/instr_data.dat
--rw-r--r--   0 kayacelebi   (501) staff       (20)      451 2020-12-23 09:25:11.000000 riscv-assembler-1.0.9/riscv_assembler/data/reg_map.dat
-drwxr-xr-x   0 kayacelebi   (501) staff       (20)        0 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/riscv_assembler.egg-info/
--rw-r--r--   0 kayacelebi   (501) staff       (20)    10815 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/riscv_assembler.egg-info/PKG-INFO
--rw-r--r--   0 kayacelebi   (501) staff       (20)      298 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/riscv_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 kayacelebi   (501) staff       (20)        1 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/riscv_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 kayacelebi   (501) staff       (20)       16 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/riscv_assembler.egg-info/top_level.txt
--rw-r--r--   0 kayacelebi   (501) staff       (20)       38 2020-12-24 03:52:21.000000 riscv-assembler-1.0.9/setup.cfg
--rw-r--r--   0 kayacelebi   (501) staff       (20)      715 2020-12-24 03:50:08.000000 riscv-assembler-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.849771 riscv-assembler-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-11 03:54:41.849771 riscv-assembler-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/references/
+-rw-r--r--   0 runner    (1001) docker     (123)   289093 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/references/mdimg.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-11 03:54:41.849771 riscv-assembler-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/src/riscv_assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/src/riscv_assembler/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/data/instr_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/data/reg_map.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    17547 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/depr_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/instr_arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/project_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/tests/assembly/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.849771 riscv-assembler-1.1.0/tests/assembly/prjtest1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/argmax.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/classify.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/dot.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/main.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/matmul.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3421 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/read_matrix.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/relu.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/utils.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/write_matrix.s
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test0.s
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test1.s
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test2.s
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test3.s
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test4.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/test_class.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `riscv-assembler-1.0.9/riscv_assembler/data/instr_data.dat` & `riscv-assembler-1.1.0/src/riscv_assembler/data/instr_data.dat`

 * *Files identical despite different names*

