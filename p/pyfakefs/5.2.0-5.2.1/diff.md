# Comparing `tmp/pyfakefs-5.2.0.tar.gz` & `tmp/pyfakefs-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfakefs-5.2.0.tar", last modified: Fri Mar 31 18:30:05 2023, max compression
+gzip compressed data, was "pyfakefs-5.2.1.tar", last modified: Tue Apr 11 14:25:34 2023, max compression
```

## Comparing `pyfakefs-5.2.0.tar` & `pyfakefs-5.2.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:30:05.386912 pyfakefs-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    42610 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/COPYING
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-03-31 18:30:05.386912 pyfakefs-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:30:05.378912 pyfakefs-5.2.0/pyfakefs/
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_file.py
--rw-r--r--   0 runner    (1001) docker     (123)   114825 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_filesystem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2180 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_filesystem_shutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    42868 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_filesystem_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_open.py
--rw-r--r--   0 runner    (1001) docker     (123)    48440 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_os.py
--rw-r--r--   0 runner    (1001) docker     (123)    17959 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    34178 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/fake_scandir.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/mox3_stubout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/patched_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:30:05.382912 pyfakefs-5.2.0/pyfakefs/pytest_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_doctest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_fixture_param_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_module_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_plugin_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:30:05.386912 pyfakefs-5.2.0/pyfakefs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/all_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/all_tests_without_extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/dynamic_patch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/example_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_glob_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21750 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_shutil_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   105643 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33469 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_unittest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29625 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_vs_real_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    83871 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_open_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   229221 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_os_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_pathlib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22291 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_stat_time_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fake_tempfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:30:05.386912 pyfakefs-5.2.0/pyfakefs/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fixtures/config_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fixtures/deprecated_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/fixtures/module_with_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/import_as_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/logsio.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/mox3_stubout_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/mox3_stubout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/patched_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyfakefs/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:30:05.378912 pyfakefs-5.2.0/pyfakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-03-31 18:30:05.000000 pyfakefs-5.2.0/pyfakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-31 18:30:05.000000 pyfakefs-5.2.0/pyfakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 18:30:05.000000 pyfakefs-5.2.0/pyfakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-31 18:30:05.000000 pyfakefs-5.2.0/pyfakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 18:30:05.000000 pyfakefs-5.2.0/pyfakefs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-31 18:30:05.386912 pyfakefs-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 18:29:49.000000 pyfakefs-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    43041 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/COPYING
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.595978 pyfakefs-5.2.1/pyfakefs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114825 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_filesystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2180 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_filesystem_shutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42868 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_filesystem_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49959 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17959 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34457 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_scandir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/mox3_stubout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/patched_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.599978 pyfakefs-5.2.1/pyfakefs/pytest_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_doctest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_fixture_param_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_module_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_plugin_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/pyfakefs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/all_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/all_tests_without_extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/dynamic_patch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_glob_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22146 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_shutil_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105643 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33469 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_unittest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29625 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_vs_real_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83871 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_open_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   230257 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_os_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_pathlib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22291 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_stat_time_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_tempfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/pyfakefs/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fixtures/config_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fixtures/deprecated_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fixtures/module_with_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/import_as_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/logsio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/mox3_stubout_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/mox3_stubout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/patched_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.595978 pyfakefs-5.2.1/pyfakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/setup.py
```

### Comparing `pyfakefs-5.2.0/CHANGES.md` & `pyfakefs-5.2.1/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 # pyfakefs Release Notes
 The released versions correspond to PyPI releases.
 
+## [Version 5.2.1](https://pypi.python.org/pypi/pyfakefs/5.2.1) (2023-04-11)
+Support for latest Python 3.12 version.
+
+### Changes
+* Adapted fake pathlib to changes in Python 3.12a7 (last alpha version)
+
+### Fixes
+* Properties defining the capabilities of some `os` functions like
+  `os.supports_follow_symlinks` are now properly faked to contain the fake functions
+  if the real functions are faked (see [#799](../../issues/799))
+
 ## [Version 5.2.0](https://pypi.python.org/pypi/pyfakefs/5.2.0) (2023-03-31)
 Supports current Python 3.12 version (alpha 6). We plan to make patch releases in
 case of breaking changes in alpha or beta versions.
 
 ### Changes
 * Fake module classes previously defined in `fake_filesystem` have now moved to
   their own modules: `fake_os.FakeOsModule`, `fake_path.FakePathModule`,
```

### Comparing `pyfakefs-5.2.0/COPYING` & `pyfakefs-5.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/PKG-INFO` & `pyfakefs-5.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.2.0
+Version: 5.2.1
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyfakefs-5.2.0/README.md` & `pyfakefs-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/extra_packages.py` & `pyfakefs-5.2.1/pyfakefs/extra_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_file.py` & `pyfakefs-5.2.1/pyfakefs/fake_file.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_filesystem.py` & `pyfakefs-5.2.1/pyfakefs/fake_filesystem.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_filesystem_shutil.py` & `pyfakefs-5.2.1/pyfakefs/fake_filesystem_shutil.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_filesystem_unittest.py` & `pyfakefs-5.2.1/pyfakefs/fake_filesystem_unittest.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_io.py` & `pyfakefs-5.2.1/pyfakefs/fake_io.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_open.py` & `pyfakefs-5.2.1/pyfakefs/fake_open.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_os.py` & `pyfakefs-5.2.1/pyfakefs/fake_os.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     Callable,
     Union,
     Any,
     Tuple,
     cast,
     AnyStr,
     TYPE_CHECKING,
+    Set,
 )
 
 from pyfakefs.extra_packages import use_scandir
 from pyfakefs.fake_file import (
     FakeDirectory,
     FakeDirWrapper,
     StandardStreamWrapper,
@@ -142,14 +143,18 @@
 
         Args:
             filesystem: FakeFilesystem used to provide file system information
         """
         self.filesystem = filesystem
         self.os_module: Any = os
         self.path = FakePathModule(self.filesystem, self)
+        self._supports_follow_symlinks: Optional[Set] = None
+        self._supports_dir_fd: Optional[Set] = None
+        self._supports_effective_ids: Optional[Set] = None
+        self._supports_fd: Optional[Set] = None
 
     @property
     def devnull(self) -> str:
         return self.path.devnull
 
     @property
     def sep(self) -> str:
@@ -886,16 +891,15 @@
         try:
             path = make_string_path(path)
         except TypeError:
             # the error is handled later
             path = path
         if dir_fd is not None:
             # check if fd is supported for the built-in real function
-            real_fct = getattr(os, fct.__name__)
-            if real_fct not in self.supports_dir_fd:
+            if fct not in self.supports_dir_fd:
                 raise NotImplementedError("dir_fd unavailable on this platform")
             if isinstance(path, int):
                 raise ValueError(
                     "%s: Can't specify dir_fd without "
                     "matching path_str" % fct.__name__
                 )
             if not self.path.isabs(path):
@@ -994,15 +998,15 @@
             mode: (int) Permissions.
             dir_fd: If not `None`, the file descriptor of a directory, with
                 `path` being relative to this directory.
             follow_symlinks: (bool) If `False` and `path` points to a symlink,
                 the link itself is queried instead of the linked object.
         """
         if not follow_symlinks and (
-            os.chmod not in os.supports_follow_symlinks or IS_PYPY
+            self.chmod not in self.supports_follow_symlinks or IS_PYPY
         ):
             raise NotImplementedError(
                 "`follow_symlinks` for chmod() is not available " "on this system"
             )
         path = self._path_with_dir_fd(path, self.chmod, dir_fd)
         self.filesystem.chmod(path, mode, follow_symlinks)
 
@@ -1264,14 +1268,51 @@
             source.seek(position)
         if contents:
             written = dest.write(contents)
             dest.flush()
             return written
         return 0
 
+    def fake_functions(self, original_functions) -> Set:
+        functions = set()
+        for fn in original_functions:
+            if hasattr(self, fn.__name__):
+                functions.add(getattr(self, fn.__name__))
+            else:
+                functions.add(fn)
+        return functions
+
+    @property
+    def supports_follow_symlinks(self) -> Set[Callable]:
+        if self._supports_follow_symlinks is None:
+            self._supports_follow_symlinks = self.fake_functions(
+                self.os_module.supports_follow_symlinks
+            )
+        return self._supports_follow_symlinks
+
+    @property
+    def supports_dir_fd(self) -> Set[Callable]:
+        if self._supports_dir_fd is None:
+            self._supports_dir_fd = self.fake_functions(self.os_module.supports_dir_fd)
+        return self._supports_dir_fd
+
+    @property
+    def supports_fd(self) -> Set[Callable]:
+        if self._supports_fd is None:
+            self._supports_fd = self.fake_functions(self.os_module.supports_fd)
+        return self._supports_fd
+
+    @property
+    def supports_effective_ids(self) -> Set[Callable]:
+        if self._supports_effective_ids is None:
+            self._supports_effective_ids = self.fake_functions(
+                self.os_module.supports_effective_ids
+            )
+        return self._supports_effective_ids
+
     def __getattr__(self, name: str) -> Any:
         """Forwards any unfaked calls to the standard os module."""
         return getattr(self.os_module, name)
 
 
 if sys.version_info > (3, 10):
```

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_path.py` & `pyfakefs-5.2.1/pyfakefs/fake_path.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_pathlib.py` & `pyfakefs-5.2.1/pyfakefs/fake_pathlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             if sys.version_info < (3, 10):
                 raise TypeError(
                     "chmod() got an unexpected keyword " "argument 'follow_symlinks'"
                 )
 
             if (
                 not kwargs["follow_symlinks"]
-                and os.os_module.chmod not in os.supports_follow_symlinks
+                and os.os_module.chmod not in os.os_module.supports_follow_symlinks
             ):
                 raise NotImplementedError(
                     "`follow_symlinks` for chmod() is not available " "on this system"
                 )
         return pathobj.filesystem.chmod(str(pathobj), *args, **kwargs)
 
     mkdir = _wrap_strfunc(FakeFilesystem.makedir)
@@ -516,47 +516,49 @@
         """Creates the correct subclass based on OS."""
         if cls is FakePathlibModule.Path:
             cls = (
                 FakePathlibModule.WindowsPath
                 if cls.filesystem.is_windows_fs
                 else FakePathlibModule.PosixPath
             )
-        self = cls._from_parts(args)
-        return self
-
-    @classmethod
-    def _from_parts(cls, args, init=False):  # pylint: disable=unused-argument
-        # Overwritten to call _init to set the fake accessor,
-        # which is not done since Python 3.10
-        self = object.__new__(cls)
-        self._init()
-        parse_fct = (
-            self._parse_parts if sys.version_info >= (3, 12) else self._parse_args
-        )
-        drv, root, parts = parse_fct(args)
-        self._drv = drv
-        self._root = root
-        self._parts = parts
-        return self
+        if sys.version_info < (3, 12):
+            return cls._from_parts(args)
+        else:
+            return object.__new__(cls)
 
-    @classmethod
-    def _from_parsed_parts(cls, drv, root, parts):
-        # Overwritten to call _init to set the fake accessor,
-        # which is not done since Python 3.10
-        self = object.__new__(cls)
-        self._init()
-        self._drv = drv
-        self._root = root
-        self._parts = parts
-        return self
-
-    def _init(self, template=None):
-        """Initializer called from base class."""
-        self._accessor = _fake_accessor
-        self._closed = False
+    if sys.version_info[:2] == (3, 10):
+        # Overwritten class methods to call _init to set the fake accessor,
+        # which is not done in Python 3.10, and not needed from Python 3.11 on
+        @classmethod
+        def _from_parts(cls, args, init=False):  # pylint: disable=unused-argument
+            self = object.__new__(cls)
+            self._init()
+            drv, root, parts = self._parse_args(args)
+            self._drv = drv
+            self._root = root
+            self._parts = parts
+            return self
+
+        @classmethod
+        def _from_parsed_parts(cls, drv, root, parts):
+            self = object.__new__(cls)
+            self._drv = drv
+            self._root = root
+            self._parts = parts
+            self._init()
+            return self
+
+    if sys.version_info < (3, 11):
+
+        def _init(self, template=None):
+            """Initializer called from base class."""
+            # only needed until Python 3.10
+            self._accessor = _fake_accessor
+            # only needed until Python 3.8
+            self._closed = False
 
     def _path(self):
         """Returns the underlying path string as used by the fake
         filesystem.
         """
         return str(self)
 
@@ -587,32 +589,30 @@
                     strict = False
             else:
                 if strict is not None:
                     raise TypeError(
                         "resolve() got an unexpected keyword argument 'strict'"
                     )
                 strict = True
-            if self._closed:
-                self._raise_closed()
+            self._raise_on_closed()
             path = self._flavour.resolve(self, strict=strict)
             if path is None:
                 self.stat()
                 path = str(self.absolute())
             path = self.filesystem.absnormpath(path)
             return FakePath(path)
 
     def open(self, mode="r", buffering=-1, encoding=None, errors=None, newline=None):
         """Open the file pointed by this path and return a fake file object.
 
         Raises:
             OSError: if the target object is a directory, the path is invalid
                 or permission is denied.
         """
-        if self._closed:
-            self._raise_closed()
+        self._raise_on_closed()
         return FakeFileOpen(self.filesystem)(
             self._path(), mode, buffering, encoding, errors, newline
         )
 
     def read_bytes(self):
         """Open the fake file in bytes mode, read it, and close the file.
 
@@ -716,28 +716,31 @@
         """
         return FakePath(
             os.path.expanduser(self._path()).replace(
                 os.path.sep, self.filesystem.path_separator
             )
         )
 
+    def _raise_on_closed(self):
+        if sys.version_info < (3, 9) and self._closed:
+            self._raise_closed()
+
     def touch(self, mode=0o666, exist_ok=True):
         """Create a fake file for the path with the given access mode,
         if it doesn't exist.
 
         Args:
             mode: the file mode for the file if it does not exist
             exist_ok: if the file already exists and this is True, nothing
                 happens, otherwise FileExistError is raised
 
         Raises:
             FileExistsError: if the file exists and exits_ok is False.
         """
-        if self._closed:
-            self._raise_closed()
+        self._raise_on_closed()
         if self.exists():
             if exist_ok:
                 self.filesystem.utime(self._path(), times=None)
             else:
                 self.filesystem.raise_os_error(errno.EEXIST, self._path())
         else:
             fake_file = self.open("w")
@@ -747,15 +750,15 @@
     if sys.version_info >= (3, 12):
         """These are reimplemented for now because the original implementation
         checks the flavour against ntpath/posixpath.
         """
 
         def is_absolute(self):
             if self.filesystem.is_windows_fs:
-                return self._drv and self._root
+                return self.drive and self.root
             return os.path.isabs(self._path())
 
         def is_reserved(self):
             if not self.filesystem.is_windows_fs or not self._parts:
                 return False
             if self._parts[0].startswith("\\\\"):
                 # UNC paths are never reserved.
@@ -883,16 +886,18 @@
         """Creates the correct subclass based on OS."""
         if cls is RealPathlibModule.Path:
             cls = (
                 RealPathlibModule.WindowsPath
                 if os.name == "nt"
                 else RealPathlibModule.PosixPath
             )
-        self = cls._from_parts(args)
-        return self
+        if sys.version_info < (3, 12):
+            return cls._from_parts(args)
+        else:
+            return object.__new__(cls)
 
 
 if sys.version_info > (3, 10):
 
     def with_original_os(f: Callable) -> Callable:
         """Decorator used for real pathlib Path methods to ensure that
         real os functions instead of faked ones are used."""
```

### Comparing `pyfakefs-5.2.0/pyfakefs/fake_scandir.py` & `pyfakefs-5.2.1/pyfakefs/fake_scandir.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/helpers.py` & `pyfakefs-5.2.1/pyfakefs/helpers.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/mox3_stubout.py` & `pyfakefs-5.2.1/pyfakefs/mox3_stubout.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/patched_packages.py` & `pyfakefs-5.2.1/pyfakefs/patched_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_plugin.py` & `pyfakefs-5.2.1/pyfakefs/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_tests/conftest.py` & `pyfakefs-5.2.1/pyfakefs/pytest_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_tests/example.py` & `pyfakefs-5.2.1/pyfakefs/pytest_tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py` & `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_doctest_test.py` & `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_doctest_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_fixture_param_test.py` & `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_fixture_param_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_fixture_test.py` & `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_module_fixture_test.py` & `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_module_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/pytest_tests/pytest_plugin_test.py` & `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/all_tests.py` & `pyfakefs-5.2.1/pyfakefs/tests/all_tests.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/all_tests_without_extra_packages.py` & `pyfakefs-5.2.1/pyfakefs/tests/all_tests_without_extra_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/dynamic_patch_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/dynamic_patch_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/example.py` & `pyfakefs-5.2.1/pyfakefs/tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/example_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_glob_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_glob_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_shutil_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_shutil_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,25 @@
         shutil.copystat(src_file, dst_file)
         src_stat = os.stat(src_file)
         dst_stat = os.stat(dst_file)
         self.assertEqual(src_stat.st_mode, dst_stat.st_mode)
         self.assertAlmostEqual(src_stat.st_atime, dst_stat.st_atime, places=2)
         self.assertAlmostEqual(src_stat.st_mtime, dst_stat.st_mtime, places=2)
 
+    def test_copystat_symlinks(self):
+        """Regression test for #799"""
+        self.skip_if_symlink_not_supported()
+        f = self.make_path("xyzzy")
+        self.create_file(f)
+        sym1 = self.make_path("sym1")
+        sym2 = self.make_path("sym2")
+        self.create_symlink(sym1, f)
+        self.create_symlink(sym2, f)
+        shutil.copystat(sym1, sym2, follow_symlinks=False)
+
     def test_copy2(self):
         src_file = self.make_path("xyzzy")
         self.create_file(src_file)
         os.chmod(src_file, 0o750)
         dst_file = self.make_path("xyzzy_copy")
         self.assertTrue(os.path.exists(src_file))
         self.assertFalse(os.path.exists(dst_file))
```

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_unittest_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_unittest_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_filesystem_vs_real_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_vs_real_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_open_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_open_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_os_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_os_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -2007,15 +2007,15 @@
 
     def test_chmod_no_follow_symlink(self):
         self.check_posix_only()
         path = self.make_path("some_file")
         self.createTestFile(path)
         link_path = self.make_path("link_to_some_file")
         self.create_symlink(link_path, path)
-        if os.chmod not in os.supports_follow_symlinks or IS_PYPY:
+        if self.os.chmod not in self.os.supports_follow_symlinks or IS_PYPY:
             with self.assertRaises(NotImplementedError):
                 self.os.chmod(link_path, 0o6543, follow_symlinks=False)
         else:
             self.os.chmod(link_path, 0o6543, follow_symlinks=False)
             st = self.os.stat(link_path)
             self.assert_mode_equal(0o666, st.st_mode)
             st = self.os.stat(link_path, follow_symlinks=False)
@@ -2862,14 +2862,29 @@
 
         fd = self.os.open(file_path, os.O_RDWR)
         self.os.truncate(fd, 10)
         self.assertEqual(10, self.os.stat(file_path).st_size)
         with self.open(file_path) as f:
             self.assertEqual("0123456789", f.read())
 
+    def test_capabilities(self):
+        """Make sure that the fake capabilities are the same as the real ones."""
+        self.assertEqual(
+            self.os.stat in self.os.supports_follow_symlinks,
+            os.stat in os.supports_follow_symlinks,
+        )
+        self.assertEqual(self.os.stat in self.os.supports_fd, os.stat in os.supports_fd)
+        self.assertEqual(
+            self.os.stat in self.os.supports_dir_fd, os.stat in os.supports_dir_fd
+        )
+        self.assertEqual(
+            self.os.stat in self.os.supports_effective_ids,
+            os.stat in os.supports_effective_ids,
+        )
+
 
 class RealOsModuleTest(FakeOsModuleTest):
     def use_real_fs(self):
         return True
 
 
 class FakeOsModuleTestCaseInsensitiveFS(FakeOsModuleTestBase):
@@ -4657,234 +4672,234 @@
     def use_real_fs(self):
         return True
 
 
 class FakeOsModuleDirFdTest(FakeOsModuleTestBase):
     def setUp(self):
         super(FakeOsModuleDirFdTest, self).setUp()
-        self.os.supports_dir_fd = set()
+        self.os.supports_dir_fd.clear()
         self.filesystem.is_windows_fs = False
         self.filesystem.create_dir("/foo/bar")
         self.dir_fd = self.os.open("/foo", os.O_RDONLY)
         self.filesystem.create_file("/foo/baz")
 
     def test_access(self):
         self.assertRaises(
             NotImplementedError,
             self.os.access,
             "baz",
             self.os.F_OK,
             dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.access)
+        self.os.supports_dir_fd.add(self.os.access)
         self.assertTrue(self.os.access("baz", self.os.F_OK, dir_fd=self.dir_fd))
 
     def test_chmod(self):
         self.assertRaises(
             NotImplementedError,
             self.os.chmod,
             "baz",
             0o6543,
             dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.chmod)
+        self.os.supports_dir_fd.add(self.os.chmod)
         self.os.chmod("baz", 0o6543, dir_fd=self.dir_fd)
         st = self.os.stat("/foo/baz")
         self.assert_mode_equal(0o6543, st.st_mode)
 
     @unittest.skipIf(not hasattr(os, "chown"), "chown not on all platforms available")
     def test_chown(self):
         self.assertRaises(
             NotImplementedError,
             self.os.chown,
             "baz",
             100,
             101,
             dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.chown)
+        self.os.supports_dir_fd.add(self.os.chown)
         self.os.chown("baz", 100, 101, dir_fd=self.dir_fd)
         st = self.os.stat("/foo/baz")
         self.assertEqual(st[stat.ST_UID], 100)
         self.assertEqual(st[stat.ST_GID], 101)
 
     def test_link_src_fd(self):
         self.assertRaises(
             NotImplementedError,
             self.os.link,
             "baz",
             "/bat",
             src_dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.link)
+        self.os.supports_dir_fd.add(self.os.link)
         self.os.link("baz", "/bat", src_dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/bat"))
 
     def test_link_dst_fd(self):
         self.assertRaises(
             NotImplementedError,
             self.os.link,
             "baz",
             "/bat",
             dst_dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.link)
+        self.os.supports_dir_fd.add(self.os.link)
         self.os.link("/foo/baz", "bat", dst_dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/foo/bat"))
 
     def test_symlink(self):
         self.assertRaises(
             NotImplementedError,
             self.os.symlink,
             "baz",
             "/bat",
             dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.symlink)
+        self.os.supports_dir_fd.add(self.os.symlink)
         self.os.symlink("baz", "/bat", dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/bat"))
 
     def test_readlink(self):
         self.skip_if_symlink_not_supported()
         self.filesystem.create_symlink("/meyer/lemon/pie", "/foo/baz")
         self.filesystem.create_symlink("/geo/metro", "/meyer")
         self.assertRaises(
             NotImplementedError,
             self.os.readlink,
             "/geo/metro/lemon/pie",
             dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.readlink)
+        self.os.supports_dir_fd.add(self.os.readlink)
         self.assertEqual(
             "/foo/baz",
             self.os.readlink("/geo/metro/lemon/pie", dir_fd=self.dir_fd),
         )
 
     def test_stat(self):
         self.assertRaises(NotImplementedError, self.os.stat, "baz", dir_fd=self.dir_fd)
-        self.os.supports_dir_fd.add(os.stat)
+        self.os.supports_dir_fd.add(self.os.stat)
         st = self.os.stat("baz", dir_fd=self.dir_fd)
         self.assertEqual(st.st_mode, 0o100666)
 
     def test_lstat(self):
         self.assertRaises(NotImplementedError, self.os.lstat, "baz", dir_fd=self.dir_fd)
-        self.os.supports_dir_fd.add(os.lstat)
+        self.os.supports_dir_fd.add(self.os.lstat)
         st = self.os.lstat("baz", dir_fd=self.dir_fd)
         self.assertEqual(st.st_mode, 0o100666)
 
     def test_mkdir(self):
         self.assertRaises(
             NotImplementedError, self.os.mkdir, "newdir", dir_fd=self.dir_fd
         )
-        self.os.supports_dir_fd.add(os.mkdir)
+        self.os.supports_dir_fd.add(self.os.mkdir)
         self.os.mkdir("newdir", dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/foo/newdir"))
 
     def test_rmdir(self):
         self.assertRaises(NotImplementedError, self.os.rmdir, "bar", dir_fd=self.dir_fd)
-        self.os.supports_dir_fd.add(os.rmdir)
+        self.os.supports_dir_fd.add(self.os.rmdir)
         self.os.rmdir("bar", dir_fd=self.dir_fd)
         self.assertFalse(self.os.path.exists("/foo/bar"))
 
     @unittest.skipIf(not hasattr(os, "mknod"), "mknod not on all platforms available")
     def test_mknod(self):
         self.assertRaises(
             NotImplementedError, self.os.mknod, "newdir", dir_fd=self.dir_fd
         )
-        self.os.supports_dir_fd.add(os.mknod)
+        self.os.supports_dir_fd.add(self.os.mknod)
         self.os.mknod("newdir", dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/foo/newdir"))
 
     def test_rename_src_fd(self):
         self.assertRaises(
             NotImplementedError,
             self.os.rename,
             "baz",
             "/foo/batz",
             src_dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.rename)
+        self.os.supports_dir_fd.add(self.os.rename)
         self.os.rename("bar", "/foo/batz", src_dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/foo/batz"))
 
     def test_rename_dst_fd(self):
         self.assertRaises(
             NotImplementedError,
             self.os.rename,
             "baz",
             "/foo/batz",
             dst_dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.rename)
+        self.os.supports_dir_fd.add(self.os.rename)
         self.os.rename("/foo/bar", "batz", dst_dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/foo/batz"))
 
     def test_replace_src_fd(self):
         self.assertRaises(
             NotImplementedError,
             self.os.rename,
             "baz",
             "/foo/batz",
             src_dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.rename)
+        self.os.supports_dir_fd.add(self.os.rename)
         self.os.replace("bar", "/foo/batz", src_dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/foo/batz"))
 
     def test_replace_dst_fd(self):
         self.assertRaises(
             NotImplementedError,
             self.os.rename,
             "baz",
             "/foo/batz",
             dst_dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.rename)
+        self.os.supports_dir_fd.add(self.os.rename)
         self.os.replace("/foo/bar", "batz", dst_dir_fd=self.dir_fd)
         self.assertTrue(self.os.path.exists("/foo/batz"))
 
     def test_remove(self):
         self.assertRaises(
             NotImplementedError, self.os.remove, "baz", dir_fd=self.dir_fd
         )
-        self.os.supports_dir_fd.add(os.remove)
+        self.os.supports_dir_fd.add(self.os.remove)
         self.os.remove("baz", dir_fd=self.dir_fd)
         self.assertFalse(self.os.path.exists("/foo/baz"))
 
     def test_unlink(self):
         self.assertRaises(
             NotImplementedError, self.os.unlink, "baz", dir_fd=self.dir_fd
         )
-        self.os.supports_dir_fd.add(os.unlink)
+        self.os.supports_dir_fd.add(self.os.unlink)
         self.os.unlink("baz", dir_fd=self.dir_fd)
         self.assertFalse(self.os.path.exists("/foo/baz"))
 
     def test_utime(self):
         self.assertRaises(
             NotImplementedError,
             self.os.utime,
             "baz",
             (1, 2),
             dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.utime)
+        self.os.supports_dir_fd.add(self.os.utime)
         self.os.utime("baz", times=(1, 2), dir_fd=self.dir_fd)
         st = self.os.stat("/foo/baz")
         self.assertEqual(1, st.st_atime)
         self.assertEqual(2, st.st_mtime)
 
     def test_open(self):
         self.assertRaises(
             NotImplementedError,
             self.os.open,
             "baz",
             os.O_RDONLY,
             dir_fd=self.dir_fd,
         )
-        self.os.supports_dir_fd.add(os.open)
+        self.os.supports_dir_fd.add(self.os.open)
         fd = self.os.open("baz", os.O_RDONLY, dir_fd=self.dir_fd)
         self.assertLess(0, fd)
 
 
 class StatPropagationTest(TestCase):
     def setUp(self):
         self.filesystem = fake_filesystem.FakeFilesystem(path_separator="/")
@@ -5181,18 +5196,20 @@
         children = [dir_entry.name for dir_entry in self.os.scandir(fd)]
         assert sorted(children) == ["file1", "file2", "subdir"]
 
     def check_stat(
         self, absolute_symlink_expected_size, relative_symlink_expected_size
     ):
         self.assertEqual(self.FILE_SIZE, self.dir_entries[1].stat().st_size)
-        self.assertEqual(
-            int(self.os.stat(self.dir_path).st_ctime),
-            int(self.dir_entries[0].stat().st_ctime),
-        )
+        if not self.is_windows_fs or sys.version_info < (3, 12):
+            # behavior of st_ctime changed in 3.12, to be adapted later
+            self.assertEqual(
+                int(self.os.stat(self.dir_path).st_ctime),
+                int(self.dir_entries[0].stat().st_ctime),
+            )
 
         if self.supports_symlinks:
             self.assertEqual(self.LINKED_FILE_SIZE, self.dir_entries[3].stat().st_size)
             self.assertEqual(
                 absolute_symlink_expected_size,
                 self.dir_entries[3].stat(follow_symlinks=False).st_size,
             )
@@ -5215,18 +5232,20 @@
         self.check_stat(len(self.linked_file_path), len(self.rel_linked_file_path))
 
     @unittest.skipIf(not TestCase.is_windows, "Windows specific behavior")
     def test_stat_windows(self):
         self.check_stat(0, 0)
 
     def test_index_access_to_stat_times_returns_int(self):
-        self.assertEqual(
-            self.os.stat(self.dir_path)[stat.ST_CTIME],
-            int(self.dir_entries[0].stat().st_ctime),
-        )
+        if not self.is_windows_fs or sys.version_info < (3, 12):
+            # behavior of st_ctime changed in 3.12, to be adapted later
+            self.assertEqual(
+                self.os.stat(self.dir_path)[stat.ST_CTIME],
+                int(self.dir_entries[0].stat().st_ctime),
+            )
         if self.supports_symlinks:
             self.assertEqual(
                 self.os.stat(self.linked_dir_path)[stat.ST_MTIME],
                 int(self.dir_entries[2].stat().st_mtime),
             )
             self.assertEqual(
                 self.os.stat(self.linked_dir_path)[stat.ST_MTIME],
```

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_pathlib_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_pathlib_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         sys.version_info < (3, 10),
         "follow_symlinks argument new in Python 3.10",
     )
     def test_chmod_no_followsymlinks(self):
         self.skip_if_symlink_not_supported()
         file_stat = self.os.stat(self.file_path)
         link_stat = self.os.lstat(self.file_link_path)
-        if self.real_os.chmod not in os.supports_follow_symlinks or IS_PYPY:
+        if self.os.chmod not in self.os.supports_follow_symlinks or IS_PYPY:
             with self.assertRaises(NotImplementedError):
                 self.path(self.file_link_path).chmod(0o444, follow_symlinks=False)
         else:
             self.path(self.file_link_path).chmod(0o444, follow_symlinks=False)
             self.assertEqual(file_stat.st_mode, stat.S_IFREG | 0o666)
             # the exact mode depends on OS and Python version
             self.assertEqual(link_stat.st_mode & 0o777700, stat.S_IFLNK | 0o700)
```

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_stat_time_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_stat_time_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fake_tempfile_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/fake_tempfile_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fixtures/deprecated_property.py` & `pyfakefs-5.2.1/pyfakefs/tests/fixtures/deprecated_property.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/fixtures/module_with_attributes.py` & `pyfakefs-5.2.1/pyfakefs/tests/fixtures/module_with_attributes.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/import_as_example.py` & `pyfakefs-5.2.1/pyfakefs/tests/import_as_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/logsio.py` & `pyfakefs-5.2.1/pyfakefs/tests/logsio.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/mox3_stubout_example.py` & `pyfakefs-5.2.1/pyfakefs/tests/mox3_stubout_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/mox3_stubout_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/mox3_stubout_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/patched_packages_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/patched_packages_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/performance_test.py` & `pyfakefs-5.2.1/pyfakefs/tests/performance_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs/tests/test_utils.py` & `pyfakefs-5.2.1/pyfakefs/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/pyfakefs.egg-info/PKG-INFO` & `pyfakefs-5.2.1/pyfakefs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.2.0
+Version: 5.2.1
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyfakefs-5.2.0/pyfakefs.egg-info/SOURCES.txt` & `pyfakefs-5.2.1/pyfakefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.0/setup.cfg` & `pyfakefs-5.2.1/setup.cfg`

 * *Files identical despite different names*

